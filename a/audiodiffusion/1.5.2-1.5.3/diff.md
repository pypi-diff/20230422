# Comparing `tmp/audiodiffusion-1.5.2.tar.gz` & `tmp/audiodiffusion-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiodiffusion-1.5.2.tar", last modified: Wed Feb  8 08:38:23 2023, max compression
+gzip compressed data, was "audiodiffusion-1.5.3.tar", last modified: Sat Apr 22 08:37:15 2023, max compression
```

## Comparing `audiodiffusion-1.5.2.tar` & `audiodiffusion-1.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-02-08 08:38:23.744733 audiodiffusion-1.5.2/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    35149 2022-08-16 17:16:58.000000 audiodiffusion-1.5.2/LICENSE
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-02-08 08:38:23.744733 audiodiffusion-1.5.2/PKG-INFO
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13229 2023-02-05 11:03:03.000000 audiodiffusion-1.5.2/README.md
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-02-08 08:38:23.744733 audiodiffusion-1.5.2/audiodiffusion/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     5296 2023-02-08 08:37:52.000000 audiodiffusion-1.5.2/audiodiffusion/__init__.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     3490 2022-12-24 15:06:00.000000 audiodiffusion-1.5.2/audiodiffusion/audio_encoder.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)     5671 2023-02-01 22:49:09.000000 audiodiffusion-1.5.2/audiodiffusion/mel.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    11404 2023-02-01 22:49:16.000000 audiodiffusion-1.5.2/audiodiffusion/pipeline_audio_diffusion.py
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    12150 2022-12-24 18:47:40.000000 audiodiffusion-1.5.2/audiodiffusion/utils.py
-drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-02-08 08:38:23.744733 audiodiffusion-1.5.2/audiodiffusion.egg-info/
--rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-02-08 08:38:23.000000 audiodiffusion-1.5.2/audiodiffusion.egg-info/PKG-INFO
--rw-rw-r--   0 teticio   (1000) teticio   (1000)      425 2023-02-08 08:38:23.000000 audiodiffusion-1.5.2/audiodiffusion.egg-info/SOURCES.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2023-02-08 08:38:23.000000 audiodiffusion-1.5.2/audiodiffusion.egg-info/dependency_links.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2022-12-02 17:31:12.000000 audiodiffusion-1.5.2/audiodiffusion.egg-info/not-zip-safe
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       61 2023-02-08 08:38:23.000000 audiodiffusion-1.5.2/audiodiffusion.egg-info/requires.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       15 2023-02-08 08:38:23.000000 audiodiffusion-1.5.2/audiodiffusion.egg-info/top_level.txt
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       57 2022-12-24 11:03:28.000000 audiodiffusion-1.5.2/pyproject.toml
--rw-rw-r--   0 teticio   (1000) teticio   (1000)      478 2023-02-08 08:38:23.748733 audiodiffusion-1.5.2/setup.cfg
--rw-rw-r--   0 teticio   (1000) teticio   (1000)       92 2022-08-28 13:28:51.000000 audiodiffusion-1.5.2/setup.py
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-04-22 08:37:15.793655 audiodiffusion-1.5.3/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    35149 2022-08-16 17:16:58.000000 audiodiffusion-1.5.3/LICENSE
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-04-22 08:37:15.793655 audiodiffusion-1.5.3/PKG-INFO
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13229 2023-02-05 11:03:03.000000 audiodiffusion-1.5.3/README.md
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-04-22 08:37:15.789655 audiodiffusion-1.5.3/audiodiffusion/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     5296 2023-04-22 08:32:34.000000 audiodiffusion-1.5.3/audiodiffusion/__init__.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     3490 2022-12-24 15:06:00.000000 audiodiffusion-1.5.3/audiodiffusion/audio_encoder.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)     5671 2023-02-01 22:49:09.000000 audiodiffusion-1.5.3/audiodiffusion/mel.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    10809 2023-04-22 08:29:21.000000 audiodiffusion-1.5.3/audiodiffusion/pipeline_audio_diffusion.py
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    12150 2022-12-24 18:47:40.000000 audiodiffusion-1.5.3/audiodiffusion/utils.py
+drwxrwxr-x   0 teticio   (1000) teticio   (1000)        0 2023-04-22 08:37:15.793655 audiodiffusion-1.5.3/audiodiffusion.egg-info/
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)    13485 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/PKG-INFO
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)      425 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)        1 2022-12-02 17:31:12.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/not-zip-safe
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       61 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/requires.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       15 2023-04-22 08:37:15.000000 audiodiffusion-1.5.3/audiodiffusion.egg-info/top_level.txt
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       57 2022-12-24 11:03:28.000000 audiodiffusion-1.5.3/pyproject.toml
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)      478 2023-04-22 08:37:15.793655 audiodiffusion-1.5.3/setup.cfg
+-rw-rw-r--   0 teticio   (1000) teticio   (1000)       92 2022-08-28 13:28:51.000000 audiodiffusion-1.5.3/setup.py
```

### Comparing `audiodiffusion-1.5.2/LICENSE` & `audiodiffusion-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.2/PKG-INFO` & `audiodiffusion-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiodiffusion
-Version: 1.5.2
+Version: 1.5.3
 Summary: Generate Mel spectrogram dataset from directory of audio files.
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
```

### Comparing `audiodiffusion-1.5.2/README.md` & `audiodiffusion-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.2/audiodiffusion/__init__.py` & `audiodiffusion-1.5.3/audiodiffusion/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from librosa.beat import beat_track
 from PIL import Image
 from tqdm.auto import tqdm
 
 # from diffusers import AudioDiffusionPipeline
 from .pipeline_audio_diffusion import AudioDiffusionPipeline
 
-VERSION = "1.5.2"
+VERSION = "1.5.3"
 
 
 class AudioDiffusion:
     def __init__(
         self,
         model_id: str = "teticio/audio-diffusion-256",
         cuda: bool = torch.cuda.is_available(),
```

### Comparing `audiodiffusion-1.5.2/audiodiffusion/audio_encoder.py` & `audiodiffusion-1.5.3/audiodiffusion/audio_encoder.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.2/audiodiffusion/mel.py` & `audiodiffusion-1.5.3/audiodiffusion/mel.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.2/audiodiffusion/pipeline_audio_diffusion.py` & `audiodiffusion-1.5.3/audiodiffusion/pipeline_audio_diffusion.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,29 +55,14 @@
         unet: UNet2DConditionModel,
         mel: Mel,
         scheduler: Union[DDIMScheduler, DDPMScheduler],
     ):
         super().__init__()
         self.register_modules(unet=unet, scheduler=scheduler, mel=mel, vqvae=vqvae)
 
-    def get_input_dims(self) -> Tuple:
-        """Returns dimension of input image
-
-        Returns:
-            `Tuple`: (height, width)
-        """
-        input_module = self.vqvae if self.vqvae is not None else self.unet
-        # For backwards compatibility
-        sample_size = (
-            (input_module.sample_size, input_module.sample_size)
-            if type(input_module.sample_size) == int
-            else input_module.sample_size
-        )
-        return sample_size
-
     def get_default_steps(self) -> int:
         """Returns default number of steps recommended for inference
 
         Returns:
             `int`: number of steps
         """
         return 50 if isinstance(self.scheduler, DDIMScheduler) else 1000
@@ -127,16 +112,14 @@
 
         steps = steps or self.get_default_steps()
         self.scheduler.set_timesteps(steps)
         step_generator = step_generator or generator
         # For backwards compatibility
         if type(self.unet.sample_size) == int:
             self.unet.sample_size = (self.unet.sample_size, self.unet.sample_size)
-        input_dims = self.get_input_dims()
-        self.mel.set_resolution(x_res=input_dims[1], y_res=input_dims[0])
         if noise is None:
             noise = torch.randn(
                 (
                     batch_size,
                     self.unet.in_channels,
                     self.unet.sample_size[0],
                     self.unet.sample_size[1],
@@ -238,15 +221,15 @@
         sample = np.array(
             [np.frombuffer(image.tobytes(), dtype="uint8").reshape((1, image.height, image.width)) for image in images]
         )
         sample = (sample / 255) * 2 - 1
         sample = torch.Tensor(sample).to(self.device)
 
         for t in self.progress_bar(torch.flip(self.scheduler.timesteps, (0,))):
-            prev_timestep = t - self.scheduler.num_train_timesteps // self.scheduler.num_inference_steps
+            prev_timestep = t - self.scheduler.config.num_train_timesteps // self.scheduler.num_inference_steps
             alpha_prod_t = self.scheduler.alphas_cumprod[t]
             alpha_prod_t_prev = (
                 self.scheduler.alphas_cumprod[prev_timestep]
                 if prev_timestep >= 0
                 else self.scheduler.final_alpha_cumprod
             )
             beta_prod_t = 1 - alpha_prod_t
```

### Comparing `audiodiffusion-1.5.2/audiodiffusion/utils.py` & `audiodiffusion-1.5.3/audiodiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `audiodiffusion-1.5.2/audiodiffusion.egg-info/PKG-INFO` & `audiodiffusion-1.5.3/audiodiffusion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiodiffusion
-Version: 1.5.2
+Version: 1.5.3
 Summary: Generate Mel spectrogram dataset from directory of audio files.
 License: GPL3
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ---
```

