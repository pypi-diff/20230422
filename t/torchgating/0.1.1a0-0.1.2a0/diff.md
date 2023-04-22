# Comparing `tmp/torchgating-0.1.1a0.tar.gz` & `tmp/torchgating-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchgating-0.1.1a0.tar", last modified: Wed Apr 12 20:38:24 2023, max compression
+gzip compressed data, was "torchgating-0.1.2a0.tar", last modified: Sat Apr 22 14:58:06 2023, max compression
```

## Comparing `torchgating-0.1.1a0.tar` & `torchgating-0.1.2a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:38:24.986551 torchgating-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-12 20:38:24.986551 torchgating-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:38:24.986551 torchgating-0.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:38:24.982551 torchgating-0.1.1a0/torchgating/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/torchgating.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 20:38:15.000000 torchgating-0.1.1a0/torchgating/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:38:24.986551 torchgating-0.1.1a0/torchgating.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 20:38:24.000000 torchgating-0.1.1a0/torchgating.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:58:06.912802 torchgating-0.1.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-22 14:57:56.000000 torchgating-0.1.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-22 14:58:06.912802 torchgating-0.1.2a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-04-22 14:57:56.000000 torchgating-0.1.2a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 14:58:06.912802 torchgating-0.1.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-22 14:57:56.000000 torchgating-0.1.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:58:06.912802 torchgating-0.1.2a0/torchgating/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-22 14:57:56.000000 torchgating-0.1.2a0/torchgating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-22 14:57:56.000000 torchgating-0.1.2a0/torchgating/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-22 14:57:56.000000 torchgating-0.1.2a0/torchgating/torchgating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-22 14:57:56.000000 torchgating-0.1.2a0/torchgating/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-22 14:57:56.000000 torchgating-0.1.2a0/torchgating/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:58:06.912802 torchgating-0.1.2a0/torchgating.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-04-22 14:58:06.000000 torchgating-0.1.2a0/torchgating.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-22 14:58:06.000000 torchgating-0.1.2a0/torchgating.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:58:06.000000 torchgating-0.1.2a0/torchgating.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-22 14:58:06.000000 torchgating-0.1.2a0/torchgating.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-22 14:58:06.000000 torchgating-0.1.2a0/torchgating.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 14:58:06.000000 torchgating-0.1.2a0/torchgating.egg-info/top_level.txt
```

### Comparing `torchgating-0.1.1a0/LICENSE` & `torchgating-0.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchgating-0.1.1a0/PKG-INFO` & `torchgating-0.1.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchgating
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: A PyTorch-based implementation of Spectral Gating, an algorithm for denoising audio signals
 Home-page: https://github.com/nuniz/TorchSpectralGating
 Author: Asaf Zorea
 Author-email: zoreasaf@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,29 +46,14 @@
 torch==2.0.0.dev20221210+cu117
 ```
 
 Please note that TorchSpectralGating may work on other versions of the above dependencies, but these are the versions that were tested.
 
 ***
 
-
-## Implementation Scheme
-TorchSpectralGate supports both stationary and non-stationary noise reduction. To enable parallel computation, a few modifications were made to the original algorithm. In the non-stationary spectral gating, an FIR filter was implemented instead of an IIR filter.
-
-### Spectral Gating
-TF-Mask can be estimated using stationary and non-stationary methods.
-![Spectral Gating](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/NonStationaryMaskScheme.png)
-### Stationary Mask Estimation
-Stationary TF-Mask estimation.
-![Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/StationaryMaskScheme.png)
-### Non-Stationary Mask Estimation
-Non-stationary TF-Mask estimation.
-![Non-Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/NonStationaryMaskScheme.png)
-***
-
 ## TorchGating Class
 Class for performing parallel spectral gating.
 
 ### Usage
 ```
 import torch
 from torchgating import TorchGating as TG
@@ -126,14 +111,27 @@
 * --figsize: Figure size for the spectrogram plots in inches (default: (10, 6)).
 * --figformat: If figformat is set, it determines the output format (default: png).
 * --vmin: Minimum value for the color scale in dB (default: -80).
 * --vmax: Maximum value for the color scale in dB (default: None).
 * --cmap: Name of the colormap to use for the spectrogram plots (default: 'magma').
 ***
 
+## Implementation Scheme
+TorchSpectralGate supports both stationary and non-stationary noise reduction. To enable parallel computation, a few modifications were made to the original algorithm. In the non-stationary spectral gating, an FIR filter was implemented instead of an IIR filter.
+
+### Spectral Gating
+TF-Mask can be estimated using stationary and non-stationary methods.
+![Spectral Gating](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/SpectralGatingScheme.png)
+### Stationary Mask Estimation
+Stationary TF-Mask estimation.
+![Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/StationaryMaskScheme.png)
+### Non-Stationary Mask Estimation
+Non-stationary TF-Mask estimation.
+![Non-Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/NonStationaryMaskScheme.png)
+***
 
 ## Run Time Comparison
 A comparison of run time was conducted using the timeit module (@number=30) on a system equipped with an NVIDIA GeForce RTX 3070 GPU. 
 The purpose of the comparison was to evaluate the computational efficiency of the TorchSpectralGate implementation of the Spectral Gating algorithm compared to the original implementation.
 
 
 **Stationary**
```

### Comparing `torchgating-0.1.1a0/README.md` & `torchgating-0.1.2a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,29 +31,14 @@
 torch==2.0.0.dev20221210+cu117
 ```
 
 Please note that TorchSpectralGating may work on other versions of the above dependencies, but these are the versions that were tested.
 
 ***
 
-
-## Implementation Scheme
-TorchSpectralGate supports both stationary and non-stationary noise reduction. To enable parallel computation, a few modifications were made to the original algorithm. In the non-stationary spectral gating, an FIR filter was implemented instead of an IIR filter.
-
-### Spectral Gating
-TF-Mask can be estimated using stationary and non-stationary methods.
-![Spectral Gating](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/NonStationaryMaskScheme.png)
-### Stationary Mask Estimation
-Stationary TF-Mask estimation.
-![Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/StationaryMaskScheme.png)
-### Non-Stationary Mask Estimation
-Non-stationary TF-Mask estimation.
-![Non-Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/NonStationaryMaskScheme.png)
-***
-
 ## TorchGating Class
 Class for performing parallel spectral gating.
 
 ### Usage
 ```
 import torch
 from torchgating import TorchGating as TG
@@ -111,14 +96,27 @@
 * --figsize: Figure size for the spectrogram plots in inches (default: (10, 6)).
 * --figformat: If figformat is set, it determines the output format (default: png).
 * --vmin: Minimum value for the color scale in dB (default: -80).
 * --vmax: Maximum value for the color scale in dB (default: None).
 * --cmap: Name of the colormap to use for the spectrogram plots (default: 'magma').
 ***
 
+## Implementation Scheme
+TorchSpectralGate supports both stationary and non-stationary noise reduction. To enable parallel computation, a few modifications were made to the original algorithm. In the non-stationary spectral gating, an FIR filter was implemented instead of an IIR filter.
+
+### Spectral Gating
+TF-Mask can be estimated using stationary and non-stationary methods.
+![Spectral Gating](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/SpectralGatingScheme.png)
+### Stationary Mask Estimation
+Stationary TF-Mask estimation.
+![Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/StationaryMaskScheme.png)
+### Non-Stationary Mask Estimation
+Non-stationary TF-Mask estimation.
+![Non-Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/NonStationaryMaskScheme.png)
+***
 
 ## Run Time Comparison
 A comparison of run time was conducted using the timeit module (@number=30) on a system equipped with an NVIDIA GeForce RTX 3070 GPU. 
 The purpose of the comparison was to evaluate the computational efficiency of the TorchSpectralGate implementation of the Spectral Gating algorithm compared to the original implementation.
 
 
 **Stationary**
```

### Comparing `torchgating-0.1.1a0/setup.py` & `torchgating-0.1.2a0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="torchgating",
-    version="0.1.1-alpha",
+    version="0.1.2-alpha",
     author="Asaf Zorea",
     author_email="zoreasaf@gmail.com",
     description="A PyTorch-based implementation of Spectral Gating, an algorithm for denoising audio signals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     url="https://github.com/nuniz/TorchSpectralGating",
```

### Comparing `torchgating-0.1.1a0/torchgating/__init__.py` & `torchgating-0.1.2a0/torchgating/__init__.py`

 * *Files identical despite different names*

### Comparing `torchgating-0.1.1a0/torchgating/run.py` & `torchgating-0.1.2a0/torchgating/run.py`

 * *Files identical despite different names*

### Comparing `torchgating-0.1.1a0/torchgating/torchgating.py` & `torchgating-0.1.2a0/torchgating/torchgating.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         if n_grad_time == 1 and n_grad_freq == 1:
             return None
 
         v_f = torch.cat([linspace(0, 1, n_grad_freq + 1, endpoint=False), linspace(1, 0, n_grad_freq + 2)])[1:-1]
         v_t = torch.cat([linspace(0, 1, n_grad_time + 1, endpoint=False), linspace(1, 0, n_grad_time + 2)])[1:-1]
         smoothing_filter = torch.outer(v_f, v_t).unsqueeze(0).unsqueeze(0)
 
-        return smoothing_filter
+        return smoothing_filter / smoothing_filter.sum()
 
     @torch.no_grad()
     def _stationary_mask(self, X_db: torch.Tensor, xn: Optional[torch.Tensor] = None) -> torch.Tensor:
         """
         Computes a stationary binary mask to filter out noise in a log-magnitude spectrogram.
 
         Arguments:
@@ -103,16 +103,22 @@
             xn (torch.Tensor): 1D tensor containing the audio signal corresponding to X_db.
 
         Returns:
             sig_mask (torch.Tensor): Binary mask of the same shape as X_db, where values greater than the threshold
             are set to 1, and the rest are set to 0.
         """
         if xn is not None:
-            XN = torch.stft(xn, n_fft=self.n_fft, hop_length=self.hop_length, win_length=self.win_length,
-                            return_complex=True, pad_mode='constant', center=True)
+            XN = torch.stft(xn,
+                            n_fft=self.n_fft,
+                            hop_length=self.hop_length,
+                            win_length=self.win_length,
+                            return_complex=True,
+                            pad_mode='constant',
+                            center=True,
+                            window=torch.hann_window(self.win_length).to(xn.device))
 
             XN_db = amp_to_db(XN).to(dtype=X_db.dtype)
         else:
             XN_db = X_db
 
         # calculate mean and standard deviation along the frequency axis
         std_freq_noise, mean_freq_noise = torch.std_mean(XN_db, dim=-1)
@@ -171,15 +177,16 @@
         X = torch.stft(
             x,
             n_fft=self.n_fft,
             hop_length=self.hop_length,
             win_length=self.win_length,
             return_complex=True,
             pad_mode='constant',
-            center=True
+            center=True,
+            window=torch.hann_window(self.win_length).to(x.device)
         )
 
         # Compute signal mask based on stationary or nonstationary assumptions
         if self.nonstationary:
             sig_mask = self._nonstationary_mask(X.abs())
         else:
             sig_mask = self._stationary_mask(amp_to_db(X), xn)
@@ -188,19 +195,21 @@
         sig_mask = self.prop_decrease * (sig_mask * 1.0 - 1.0) + 1.0
 
         # Smooth signal mask with 2D convolution
         if self.smoothing_filter is not None:
             sig_mask = conv2d(sig_mask.unsqueeze(1), self.smoothing_filter.to(sig_mask.dtype), padding='same')
 
         # Apply signal mask to STFT magnitude and phase components
-        Y = X.abs() * sig_mask.squeeze(1) * torch.exp(1j * X.angle())
+        Y = X * sig_mask.squeeze(1)
+        # Y = X.abs() * sig_mask.squeeze(1) * torch.exp(1j * X.angle())
 
         # Inverse STFT to obtain time-domain signal
         y = torch.istft(
             Y,
             n_fft=self.n_fft,
             hop_length=self.hop_length,
             win_length=self.win_length,
-            center=True
+            center=True,
+            window=torch.hann_window(self.win_length).to(Y.device)
         )
 
         return y.to(dtype=x.dtype)
```

### Comparing `torchgating-0.1.1a0/torchgating/utils.py` & `torchgating-0.1.2a0/torchgating/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import torch
 from torch.types import Number
 
 
 @torch.no_grad()
-def amp_to_db(x: torch.Tensor, eps=torch.finfo(torch.float32).eps) -> torch.Tensor:
+def amp_to_db(x: torch.Tensor, eps=torch.finfo(torch.float64).eps, top_db=40) -> torch.Tensor:
     """
     Convert the input tensor from amplitude to decibel scale.
 
     Arguments:
         x {[torch.Tensor]} -- [Input tensor.]
 
     Keyword Arguments:
         eps {[float]} -- [Small value to avoid numerical instability.]
-                          (default: {torch.finfo(torch.float32).eps})
+                          (default: {torch.finfo(torch.float64).eps})
+        top_db {[float]} -- [threshold the output at ``top_db`` below the peak]
+            `             (default: {40})
 
     Returns:
         [torch.Tensor] -- [Output tensor in decibel scale.]
     """
-    return torch.log10(x.abs() + eps)
+    x_db = 20 * torch.log10(x.abs() + eps)
+    return torch.max(x_db, (x_db.max(-1).values - top_db).unsqueeze(-1))
 
 
 @torch.no_grad()
 def temperature_sigmoid(x: torch.Tensor, x0: float, temp_coeff: float) -> torch.Tensor:
     """
     Apply a sigmoid function with temperature scaling.
```

### Comparing `torchgating-0.1.1a0/torchgating.egg-info/PKG-INFO` & `torchgating-0.1.2a0/torchgating.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchgating
-Version: 0.1.1a0
+Version: 0.1.2a0
 Summary: A PyTorch-based implementation of Spectral Gating, an algorithm for denoising audio signals
 Home-page: https://github.com/nuniz/TorchSpectralGating
 Author: Asaf Zorea
 Author-email: zoreasaf@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,29 +46,14 @@
 torch==2.0.0.dev20221210+cu117
 ```
 
 Please note that TorchSpectralGating may work on other versions of the above dependencies, but these are the versions that were tested.
 
 ***
 
-
-## Implementation Scheme
-TorchSpectralGate supports both stationary and non-stationary noise reduction. To enable parallel computation, a few modifications were made to the original algorithm. In the non-stationary spectral gating, an FIR filter was implemented instead of an IIR filter.
-
-### Spectral Gating
-TF-Mask can be estimated using stationary and non-stationary methods.
-![Spectral Gating](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/NonStationaryMaskScheme.png)
-### Stationary Mask Estimation
-Stationary TF-Mask estimation.
-![Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/StationaryMaskScheme.png)
-### Non-Stationary Mask Estimation
-Non-stationary TF-Mask estimation.
-![Non-Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/NonStationaryMaskScheme.png)
-***
-
 ## TorchGating Class
 Class for performing parallel spectral gating.
 
 ### Usage
 ```
 import torch
 from torchgating import TorchGating as TG
@@ -126,14 +111,27 @@
 * --figsize: Figure size for the spectrogram plots in inches (default: (10, 6)).
 * --figformat: If figformat is set, it determines the output format (default: png).
 * --vmin: Minimum value for the color scale in dB (default: -80).
 * --vmax: Maximum value for the color scale in dB (default: None).
 * --cmap: Name of the colormap to use for the spectrogram plots (default: 'magma').
 ***
 
+## Implementation Scheme
+TorchSpectralGate supports both stationary and non-stationary noise reduction. To enable parallel computation, a few modifications were made to the original algorithm. In the non-stationary spectral gating, an FIR filter was implemented instead of an IIR filter.
+
+### Spectral Gating
+TF-Mask can be estimated using stationary and non-stationary methods.
+![Spectral Gating](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/SpectralGatingScheme.png)
+### Stationary Mask Estimation
+Stationary TF-Mask estimation.
+![Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/StationaryMaskScheme.png)
+### Non-Stationary Mask Estimation
+Non-stationary TF-Mask estimation.
+![Non-Stationary Mask](https://github.com/nuniz/TorchSpectralGating/blob/main/supplementary_material/graphs/NonStationaryMaskScheme.png)
+***
 
 ## Run Time Comparison
 A comparison of run time was conducted using the timeit module (@number=30) on a system equipped with an NVIDIA GeForce RTX 3070 GPU. 
 The purpose of the comparison was to evaluate the computational efficiency of the TorchSpectralGate implementation of the Spectral Gating algorithm compared to the original implementation.
 
 
 **Stationary**
```

