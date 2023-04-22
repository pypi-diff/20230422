# Comparing `tmp/voice100-1.3.2.tar.gz` & `tmp/voice100-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voice100-1.3.2.tar", last modified: Tue Apr 26 12:42:41 2022, max compression
+gzip compressed data, was "voice100-1.6.0.tar", max compression
```

## Comparing `voice100-1.3.2.tar` & `voice100-1.6.0.tar`

### file list

```diff
@@ -1,39 +1,34 @@
-drwxr-xr-x   0 kaiida    (1000) kaiida    (1000)        0 2022-04-26 12:42:41.067993 voice100-1.3.2/
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1068 2021-05-31 08:19:37.000000 voice100-1.3.2/LICENSE
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      552 2022-04-26 12:42:41.067993 voice100-1.3.2/PKG-INFO
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)    10634 2022-04-23 01:39:09.000000 voice100-1.3.2/README.md
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)       38 2022-04-26 12:42:41.067993 voice100-1.3.2/setup.cfg
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1721 2022-04-26 12:39:31.000000 voice100-1.3.2/setup.py
-drwxr-xr-x   0 kaiida    (1000) kaiida    (1000)        0 2022-04-26 12:42:41.057993 voice100-1.3.2/voice100/
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)        0 2021-12-12 01:33:29.000000 voice100-1.3.2/voice100/__init__.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     2196 2022-04-24 13:34:09.000000 voice100-1.3.2/voice100/align_text.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     3620 2022-04-01 12:51:37.000000 voice100-1.3.2/voice100/audio.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      674 2022-03-13 13:47:49.000000 voice100-1.3.2/voice100/cache_dataset.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     2771 2022-03-26 04:00:21.000000 voice100-1.3.2/voice100/calc_stat.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     2119 2022-01-26 23:33:22.000000 voice100-1.3.2/voice100/convert_phone.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)    25481 2022-04-26 12:30:17.000000 voice100-1.3.2/voice100/datasets.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     6289 2022-03-18 11:25:09.000000 voice100-1.3.2/voice100/export_onnx.py
-drwxr-xr-x   0 kaiida    (1000) kaiida    (1000)        0 2022-04-26 12:42:41.067993 voice100-1.3.2/voice100/japanese/
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      772 2022-01-08 01:40:14.000000 voice100-1.3.2/voice100/japanese/__init__.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     6521 2022-01-08 01:40:14.000000 voice100-1.3.2/voice100/japanese/kata2ipa.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     7724 2022-01-08 01:40:14.000000 voice100-1.3.2/voice100/japanese/phonemizer.py
-drwxr-xr-x   0 kaiida    (1000) kaiida    (1000)        0 2022-04-26 12:42:41.067993 voice100-1.3.2/voice100/models/
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)        0 2022-01-08 01:40:14.000000 voice100-1.3.2/voice100/models/__init__.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     6598 2022-04-16 06:04:25.000000 voice100-1.3.2/voice100/models/align.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     7301 2022-04-16 06:04:25.000000 voice100-1.3.2/voice100/models/asr.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)    19630 2022-04-16 06:04:25.000000 voice100-1.3.2/voice100/models/tts.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     2852 2022-01-26 23:33:22.000000 voice100-1.3.2/voice100/text.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1092 2022-04-26 12:31:05.000000 voice100-1.3.2/voice100/train_align.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1314 2022-03-13 13:47:49.000000 voice100-1.3.2/voice100/train_asr.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1031 2022-04-16 06:23:27.000000 voice100-1.3.2/voice100/train_ttsalign.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1069 2022-04-26 12:31:05.000000 voice100-1.3.2/voice100/train_ttsaudio.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1167 2022-03-18 11:25:09.000000 voice100-1.3.2/voice100/train_ttsaudio_mt.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     4768 2022-04-24 13:36:46.000000 voice100-1.3.2/voice100/update_samples.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     4850 2022-03-20 04:47:56.000000 voice100-1.3.2/voice100/vocoder.py
-drwxr-xr-x   0 kaiida    (1000) kaiida    (1000)        0 2022-04-26 12:42:41.067993 voice100-1.3.2/voice100.egg-info/
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      552 2022-04-26 12:42:40.000000 voice100-1.3.2/voice100.egg-info/PKG-INFO
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      786 2022-04-26 12:42:40.000000 voice100-1.3.2/voice100.egg-info/SOURCES.txt
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)        1 2022-04-26 12:42:40.000000 voice100-1.3.2/voice100.egg-info/dependency_links.txt
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      571 2022-04-26 12:42:40.000000 voice100-1.3.2/voice100.egg-info/entry_points.txt
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      153 2022-04-26 12:42:40.000000 voice100-1.3.2/voice100.egg-info/requires.txt
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)        9 2022-04-26 12:42:40.000000 voice100-1.3.2/voice100.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1068 2023-03-20 23:47:11.742569 voice100-1.6.0/LICENSE
+-rw-r--r--   0        0        0    14151 2023-04-22 02:26:14.132227 voice100-1.6.0/README.md
+-rw-r--r--   0        0        0     1507 2023-04-22 03:36:21.002703 voice100-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-20 23:47:11.782570 voice100-1.6.0/voice100/__init__.py
+-rw-r--r--   0        0        0     2220 2023-04-09 11:30:02.209077 voice100-1.6.0/voice100/align_text.py
+-rw-r--r--   0        0        0     4060 2023-03-20 23:47:11.782570 voice100-1.6.0/voice100/audio.py
+-rw-r--r--   0        0        0      763 2023-03-20 23:47:11.782570 voice100-1.6.0/voice100/cache_dataset.py
+-rw-r--r--   0        0        0     3267 2023-03-20 23:47:11.782570 voice100-1.6.0/voice100/calc_stat.py
+-rw-r--r--   0        0        0    26858 2023-04-22 02:29:26.987373 voice100-1.6.0/voice100/data_modules.py
+-rw-r--r--   0        0        0     5084 2023-04-20 12:16:53.827643 voice100-1.6.0/voice100/export_onnx.py
+-rw-r--r--   0        0        0     6289 2023-03-20 23:47:11.786570 voice100-1.6.0/voice100/export_onnx_v1.py
+-rw-r--r--   0        0        0     1349 2023-04-22 02:29:26.987373 voice100-1.6.0/voice100/japanese/__init__.py
+-rw-r--r--   0        0        0     7736 2023-04-22 02:29:26.999373 voice100-1.6.0/voice100/japanese/phonemizer.py
+-rw-r--r--   0        0        0      433 2023-03-20 23:47:11.786570 voice100-1.6.0/voice100/main.py
+-rw-r--r--   0        0        0      481 2023-04-22 03:36:34.706912 voice100-1.6.0/voice100/models/__init__.py
+-rw-r--r--   0        0        0     4044 2023-03-20 23:47:11.786570 voice100-1.6.0/voice100/models/_align_v2.py
+-rw-r--r--   0        0        0     4722 2023-03-29 13:55:46.380429 voice100-1.6.0/voice100/models/_asr_v2.py
+-rw-r--r--   0        0        0      144 2023-03-20 23:47:11.790570 voice100-1.6.0/voice100/models/_base.py
+-rw-r--r--   0        0        0     5263 2023-03-20 23:47:11.790570 voice100-1.6.0/voice100/models/_layers_v1.py
+-rw-r--r--   0        0        0     7244 2023-03-20 23:47:11.790570 voice100-1.6.0/voice100/models/_layers_v2.py
+-rw-r--r--   0        0        0     7403 2023-04-22 02:26:14.132227 voice100-1.6.0/voice100/models/_tts_v2.py
+-rw-r--r--   0        0        0     6961 2023-03-20 23:47:11.790570 voice100-1.6.0/voice100/models/align.py
+-rw-r--r--   0        0        0     7563 2023-03-20 23:47:11.790570 voice100-1.6.0/voice100/models/asr.py
+-rw-r--r--   0        0        0    16195 2023-03-20 23:47:11.794570 voice100-1.6.0/voice100/models/tts.py
+-rw-r--r--   0        0        0     2811 2023-04-09 11:25:31.052470 voice100-1.6.0/voice100/prepare_dataset.py
+-rw-r--r--   0        0        0     4463 2023-04-22 02:29:26.999373 voice100-1.6.0/voice100/text.py
+-rw-r--r--   0        0        0     1165 2023-03-20 23:47:11.794570 voice100-1.6.0/voice100/train_align.py
+-rw-r--r--   0        0        0     1371 2023-03-20 23:47:11.794570 voice100-1.6.0/voice100/train_asr.py
+-rw-r--r--   0        0        0     1035 2023-03-20 23:47:11.794570 voice100-1.6.0/voice100/train_ttsalign.py
+-rw-r--r--   0        0        0     1179 2023-03-20 23:47:11.794570 voice100-1.6.0/voice100/train_ttsaudio.py
+-rw-r--r--   0        0        0     1294 2023-03-20 23:47:11.794570 voice100-1.6.0/voice100/train_ttsaudio_mt.py
+-rw-r--r--   0        0        0     4776 2023-04-22 02:29:26.999373 voice100-1.6.0/voice100/update_samples.py
+-rw-r--r--   0        0        0     5096 2023-03-20 23:47:11.798570 voice100-1.6.0/voice100/vocoder.py
+-rw-r--r--   0        0        0    15104 1970-01-01 00:00:00.000000 voice100-1.6.0/PKG-INFO
```

### Comparing `voice100-1.3.2/LICENSE` & `voice100-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voice100-1.3.2/voice100/align_text.py` & `voice100-1.6.0/voice100/align_text.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
 from argparse import ArgumentParser
 import torch
 import os
 from tqdm import tqdm
 
-from .models.align import AudioAlignCTC
-from .datasets import AudioTextDataModule
+from .models import AudioToAlignText
+from .data_modules import AudioTextDataModule
 
 
 def cli_main():
     parser = ArgumentParser()
     parser = AudioTextDataModule.add_argparse_args(parser)
     parser.add_argument("--checkpoint", required=True, type=str, help="Load from checkpoint")
     parser.add_argument("--split", default="train", type=str, help="Split to use")
+    parser.set_defaults(vocoder="mel")
     args = parser.parse_args()
     args.write_cache = False
     args.timing = True
     if args.use_phone:
         args.output = f'data/{args.dataset}-phone-align-{args.split}.txt'
     else:
         args.output = f'data/{args.dataset}-align-{args.split}.txt'
 
-    data: AudioTextDataModule = AudioTextDataModule.from_argparse_args(args, vocoder="mel")
-    model = AudioAlignCTC.load_from_checkpoint(args.checkpoint)
+    data: AudioTextDataModule = AudioTextDataModule.from_argparse_args(args)
+    model = AudioToAlignText.load_from_checkpoint(args.checkpoint)
     if args.split == "train":
         data.setup("predict")
     else:
         data.setup()
-    encoder = data.text_transform.tokenizer
+    tokenizer = data.text_transform
     model.eval()
     with open(args.output, 'w') as f:
         if args.split == "train":
             loader = data.predict_dataloader()
         elif args.split == "valid":
             loader = data.val_dataloader()
         for idx, batch in enumerate(tqdm(loader)):
@@ -45,15 +46,15 @@
                 }, file)
 
             for i in range(path.shape[0]):
                 align = [0] * (2 * text_len[i] + 1)
                 for j in hist[i, :path_len[i]]:
                     align[j] += 1
                 align = ' '.join([str(x) for x in align])
-                raw_text = encoder.decode(text[i, :text_len[i]])
+                raw_text = tokenizer.decode(text[i, :text_len[i]])
 
-                raw_align_text = encoder.decode(path[i, :path_len[i]])
+                raw_align_text = tokenizer.decode(path[i, :path_len[i]])
                 f.write(raw_text + '|' + raw_align_text + '|' + align + '\n')
 
 
 if __name__ == '__main__':
     cli_main()
```

### Comparing `voice100-1.3.2/voice100/audio.py` & `voice100-1.6.0/voice100/audio.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
 from typing import Tuple
+import math
 import torch
 from torch import nn
 import random
 
 __all__ = [
     "BatchSpectrogramAugumentation"
 ]
 
 SPECTROGRAM_AUGUMENT_RATE = 0.2
+LOG_OFFSET = 1e-6
 
 
 class BatchSpectrogramAugumentation(nn.Module):
+    """Augment mel-spectrogram data
+    """
 
-    def __init__(self, do_timestretch=True):
+    def __init__(self, do_timestretch=True, log_offset=LOG_OFFSET):
         super().__init__()
         self.do_timestretch = do_timestretch
+        self.log_offset = log_offset
+        self.blank_audio = math.log(log_offset)
 
     @torch.no_grad()
     def forward(
         self, audio: torch.Tensor, audio_len: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         assert len(audio.shape) == 3
+        assert audio.dtype == torch.float32
 
         if self.do_timestretch and random.random() < SPECTROGRAM_AUGUMENT_RATE:
             audio, audio_len = self.timestretch(audio, audio_len)
         if random.random() < SPECTROGRAM_AUGUMENT_RATE:
             audio = self.pitchshift(audio)
         if random.random() < SPECTROGRAM_AUGUMENT_RATE:
             audio = self.ampshift(audio)
@@ -61,39 +68,41 @@
         return audio - rate
 
     def timemask(self, audio):
         audio = audio.clone()
         n = random.randint(1, 3)
         for i in range(n):
             t = random.randrange(0, audio.shape[1])
-            hw = random.randint(1, 20)
+            hw = random.randint(1, 3)
             s = int(t - hw)
             e = int(t + hw)
-            audio[:, s:e, :] = -20.0
+            a = random.uniform(-self.blank_audio, -5)
+            audio[:, s:e, :] = a
         return audio
 
     def freqmask(self, audio):
         audio = audio.clone()
         t = random.randrange(0, audio.shape[2])
-        hw = random.randint(1, 3)
+        hw = random.randint(1, 10)
         s = int(t - hw)
         e = int(t + hw)
-        audio[:, :, s:e] = -20.0
+        a = random.uniform(-self.blank_audio, -5)
+        audio[:, :, s:e] = a
         return audio
 
     def mixnoise(self, audio):
         low = -5.0 + 5.0 * random.random()
         high = -5.0 + 5.0 * random.random()
         std = 5.0 * random.random()
         scale = torch.linspace(low, high, 64, device=audio.device)[None, :]
         noise = torch.rand(audio.shape, device=audio.device) * std + scale
-        return torch.log(torch.exp(audio) + torch.exp(noise))
+        return torch.log(torch.clamp(torch.exp(audio) + torch.exp(noise), min=self.log_offset))
 
     def mixaudio(self, audio, audio_len):
         audio_mask = (torch.arange(audio.shape[1], device=audio.device)[None, :, None] < audio_len[:, None, None]).float()
         x = torch.exp(audio) * audio_mask
         y = torch.cat([x[1:], x[:1]], axis=0)
-        return torch.log(0.9 * x + 0.1 * y + 1e-15) * audio_mask
+        return torch.log(torch.clamp((0.9 * x + 0.1 * y) * audio_mask, min=self.log_offset))
 
     def maskaudio(self, audio, audio_len):
         audio_mask = (torch.arange(audio.shape[1], device=audio.device)[None, :, None] < audio_len[:, None, None]).float()
-        return audio * audio_mask
+        return torch.log(torch.clamp(torch.exp(audio) * audio_mask, min=self.log_offset))
```

### Comparing `voice100-1.3.2/voice100/cache_dataset.py` & `voice100-1.6.0/voice100/cache_dataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
 from argparse import ArgumentParser
 import pytorch_lightning as pl
 from tqdm import tqdm
 
-from .datasets import AudioTextDataModule
+from .data_modules import AudioTextDataModule
 
 
 def cli_main():
     pl.seed_everything(1234)
 
-    parser = ArgumentParser()
+    parser = ArgumentParser("Cache encoded WORLD data")
     parser = pl.Trainer.add_argparse_args(parser)
     parser = AudioTextDataModule.add_argparse_args(parser)
+    parser.set_defaults(vocoder="world")
     args = parser.parse_args()
-    data: AudioTextDataModule = AudioTextDataModule.from_argparse_args(args, vocoder="world")
+    assert args.vocoder == "world"
+    data: AudioTextDataModule = AudioTextDataModule.from_argparse_args(args)
     data.setup()
     for _ in tqdm(data.val_dataloader()):
         pass
     for _ in tqdm(data.train_dataloader()):
         pass
```

### Comparing `voice100-1.3.2/voice100/calc_stat.py` & `voice100-1.6.0/voice100/calc_stat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
+from typing import Text
 from argparse import ArgumentParser
 import torch
 from tqdm import tqdm
 
-from .datasets import AudioTextDataModule
+from .data_modules import AudioTextDataModule
 
 
 def generate_padding_mask(x: torch.Tensor, length: torch.Tensor) -> torch.Tensor:
     """
     Args:
         x: tensor of shape [batch_size, length]
         length: tensor of shape [batch_size]
@@ -16,62 +17,68 @@
         float tensor of shape [batch_size, length]
     """
     assert x.dim() == 2
     assert length.dim() == 1
     return (torch.arange(x.shape[1], device=x.device)[None, :] < length[:, None]).to(x.dtype)
 
 
-def calc_stat(data, stat_path):
+def calc_stat(data: AudioTextDataModule, output_path: Text):
 
-    logspc_size = 257
-    codeap_size = 1
+    f0_dim, logspc_or_mcep_size, codeap_size = data.audio_transform.vocoder.output_dims
+    print(logspc_or_mcep_size)
+    assert f0_dim == 1
+    assert logspc_or_mcep_size == 257 or logspc_or_mcep_size == 25
+    assert codeap_size == 1
 
     f0_sum = torch.zeros(1, dtype=torch.double)
-    logspc_sum = torch.zeros(logspc_size, dtype=torch.double)
+    logspc_sum = torch.zeros(logspc_or_mcep_size, dtype=torch.double)
     codeap_sum = torch.zeros(codeap_size, dtype=torch.double)
     f0_sqrsum = torch.zeros(1, dtype=torch.double)
-    logspc_sqrsum = torch.zeros(logspc_size, dtype=torch.double)
+    logspc_sqrsum = torch.zeros(logspc_or_mcep_size, dtype=torch.double)
     codeap_sqrsum = torch.zeros(codeap_size, dtype=torch.double)
     f0_count = 0
     logspc_count = 0
-    for batch_idx, batch in enumerate(tqdm(data.train_dataloader())):
+    for batch_idx, batch in enumerate(tqdm(data.predict_dataloader())):
         (f0, f0_len, logspc, codeap), (text, text_len) = batch
         with torch.no_grad():
             mask = generate_padding_mask(f0, f0_len)
             f0mask = (f0 > 30.0).float() * mask
+            codeapmask = (codeap < -0.2).float() * mask[:, :, None]
 
             f0_sum += torch.sum(f0 * f0mask)
             f0_sqrsum += torch.sum(f0 ** 2 * f0mask)
             f0_count += torch.sum(f0mask)
 
             logspc_sum += torch.sum(torch.sum(logspc * mask[:, :, None], axis=1), axis=0)
             logspc_sqrsum += torch.sum(torch.sum(logspc ** 2 * mask[:, :, None], axis=1), axis=0)
             logspc_count += torch.sum(mask)
 
-            codeap_sum += torch.sum(torch.sum(codeap * mask[:, :, None], axis=1), axis=0)
-            codeap_sqrsum += torch.sum(torch.sum(codeap ** 2 * mask[:, :, None], axis=1), axis=0)
+            codeap_sum += torch.sum(torch.sum(codeap * codeapmask, axis=1), axis=0)
+            codeap_sqrsum += torch.sum(torch.sum(codeap ** 2 * codeapmask, axis=1), axis=0)
 
     codeap_count = logspc_count
     state_dict = {
         'f0_mean': f0_sum / f0_count,
         'f0_std': torch.sqrt((f0_sqrsum / f0_count) - (f0_sum / f0_count) ** 2),
         'logspc_mean': logspc_sum / logspc_count,
         'logspc_std': torch.sqrt((logspc_sqrsum / logspc_count) - (logspc_sum / logspc_count) ** 2),
         'codeap_mean': codeap_sum / codeap_count,
         'codeap_std': torch.sqrt((codeap_sqrsum / codeap_count) - (codeap_sum / codeap_count) ** 2),
     }
     print('saving...')
-    torch.save(state_dict, stat_path)
+    torch.save(state_dict, output_path)
 
 
 def cli_main():
-    parser = ArgumentParser()
+    parser = ArgumentParser(description="Make stat file for TTS (audio_stat.pt)")
+    parser.add_argument("--output", type=str, required=True)
     parser = AudioTextDataModule.add_argparse_args(parser)
+    parser.set_defaults(vocoder="world")
     args = parser.parse_args()
-    data = AudioTextDataModule.from_argparse_args(args, vocoder="world")
-    data.setup()
-    stat_path = f'data/{args.dataset}-stat.pt'
-    calc_stat(data, stat_path)
+    assert args.vocoder == "world" or args.vocoder == "world_mcep"
+    data = AudioTextDataModule.from_argparse_args(args)
+    data.setup("predict")
+    calc_stat(data, args.output)
 
 
 if __name__ == '__main__':
     cli_main()
```

### Comparing `voice100-1.3.2/voice100/datasets.py` & `voice100-1.6.0/voice100/data_modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 r"""Definition of Dataset for reading data from speech datasets.
 """
 
 import os
 import logging
 from glob import glob
 from typing import Union, Tuple, List, Text, Optional, Any
+import math
 import torch
 from torch import nn
 import torchaudio
 from torchaudio.transforms import MelSpectrogram
 import torch.utils.data
 from torch.utils.data import Dataset, DataLoader
 from torch.nn.utils.rnn import pad_sequence
 import pytorch_lightning as pl
 import hashlib
 
-from .text import BasicPhonemizer, CharTokenizer, CMUTokenizer
+from .text import CharTokenizer, BasicTokenizer
 
 BLANK_IDX = 0
 MELSPEC_DIM = 64
+LOG_OFFSET = 1e-6
+BLANK_AUDIO = math.log(LOG_OFFSET)
 
 logger = logging.getLogger(__name__)
 
 
 class MetafileDataset(Dataset):
     r"""``Dataset`` for reading from speech datasets with TSV metafile,
     like LJ Speech Corpus and Mozilla Common Voice.
@@ -114,27 +117,27 @@
 
 
 class MergeDataset(Dataset):
     def __init__(
         self,
         audiotext_ds: Dataset,
         align_ds: Optional[Dataset] = None,
-        phone_ds: Optional[Dataset] = None,
+        text_ds: Optional[Dataset] = None,
         target_ds: Optional[Dataset] = None,
     ) -> None:
         super().__init__()
         if align_ds is not None:
             assert len(audiotext_ds) == len(align_ds)
-        if phone_ds is not None:
-            assert len(audiotext_ds) == len(phone_ds)
+        if text_ds is not None:
+            assert len(audiotext_ds) == len(text_ds)
         if target_ds is not None:
             assert len(audiotext_ds) == len(target_ds)
         self._audiotext_ds = audiotext_ds
         self._align_ds = align_ds
-        self._phone_ds = phone_ds
+        self._text_ds = text_ds
         self._target_ds = target_ds
 
     def __len__(self) -> int:
         return len(self._audiotext_ds)
 
     def __getitem__(
         self, index: int
@@ -145,19 +148,19 @@
             _, aligntext = self._align_ds[index]
             _, targettext = self._target_ds[index]
             return id1, audio, aligntext, targettext
         elif self._align_ds is not None:
             # For TTS audio model
             _, aligntext = self._align_ds[index]
             return id1, audio, aligntext
-        elif self._phone_ds is not None:
+        elif self._text_ds is not None:
             # For ASR model and align model
-            id2, phonetext = self._phone_ds[index]
+            id2, text = self._text_ds[index]
             assert id1 == id2
-            return id1, audio, phonetext
+            return id1, audio, text
 
 
 class EncodedCacheDataset(Dataset):
     def __init__(
         self,
         dataset: Dataset,
         audio_transform: nn.Module,
@@ -168,19 +171,28 @@
         super().__init__()
         self._dataset = dataset
         self.audio_transform = audio_transform
         self.text_transform = text_transform
         self.targettext_transform = targettext_transform
         self._cachedir = cachedir
         self._salt = salt
-        self.save_mcep = isinstance(self.audio_transform, WORLDAudioProcessor)
-        if self.save_mcep:
-            from .vocoder import create_mc2sp_matrix, create_sp2mc_matrix
-            self.mc2sp_matrix = torch.from_numpy(create_mc2sp_matrix(512, 24, 0.410)).float()
-            self.sp2mc_matrix = torch.from_numpy(create_sp2mc_matrix(512, 24, 0.410)).float()
+        self.save_mcep = False
+        if isinstance(self.audio_transform, WORLDAudioProcessor):
+            vocoder = self.audio_transform.vocoder
+            if not vocoder.use_mcep:
+                from .vocoder import create_mc2sp_matrix, create_sp2mc_matrix
+                self.save_mcep = True
+                if vocoder.sample_rate == 16000:
+                    self.mc2sp_matrix = torch.from_numpy(create_mc2sp_matrix(512, 24, 0.410)).float()
+                    self.sp2mc_matrix = torch.from_numpy(create_sp2mc_matrix(512, 24, 0.410)).float()
+                elif vocoder.sample_rate == 22050:
+                    self.mc2sp_matrix = torch.from_numpy(create_mc2sp_matrix(1024, 34, 0.455)).float()
+                    self.sp2mc_matrix = torch.from_numpy(create_sp2mc_matrix(1024, 34, 0.455)).float()
+                else:
+                    raise ValueError("Unsupported sample rate")
 
     def __len__(self) -> int:
         return len(self._dataset)
 
     def __getitem__(self, index):
         data = self._dataset[index]
         if self.targettext_transform is not None:
@@ -226,15 +238,15 @@
         h.update(id_.encode('utf-8'))
         cachefile = '%s.pt' % (h.hexdigest())
         cachefile = os.path.join(self._cachedir, cachefile)
         return cachefile
 
 
 class AlignTextDataset(Dataset):
-    def __init__(self, file: Text, encoder: Union[CharTokenizer, CMUTokenizer]) -> None:
+    def __init__(self, file: Text, encoder: Union[CharTokenizer, BasicTokenizer]) -> None:
         self.tokenizer = encoder
         self.data = []
         with open(file, 'rt') as f:
             for line in f:
                 parts = line.rstrip('\r\n').split('|')
                 text = self.tokenizer(parts[0])
                 align = torch.tensor(data=[int(x) for x in parts[2].split()], dtype=torch.int32)
@@ -251,143 +263,148 @@
     def __init__(
         self,
         sample_rate: int = 16000,
         n_fft: int = 512,
         win_length: int = 400,
         hop_length: int = 160,
         n_mels: int = MELSPEC_DIM,
-        log_offset: float = 1e-6
+        log_offset: float = LOG_OFFSET
     ) -> None:
         super().__init__()
         self.log_offset = log_offset
-        self.effects = [
-            ["remix", "1"],
-            ["rate", f"{sample_rate}"],
-        ]
-
+        self.sample_rate = sample_rate
+        self.n_mels = n_mels
         self.melspec = MelSpectrogram(
             sample_rate=sample_rate,
             n_fft=n_fft,
             win_length=win_length,
             hop_length=hop_length,
             n_mels=n_mels)
 
+    @property
+    def audio_size(self) -> int:
+        return self.n_mels
+
     def forward(self, audiopath: Text) -> torch.Tensor:
-        waveform, _ = torchaudio.sox_effects.apply_effects_file(
-            audiopath, effects=self.effects)
+        waveform, sr = torchaudio.load(audiopath)
+        waveform = torchaudio.functional.resample(waveform[0], sr, self.sample_rate)
         audio = self.melspec(waveform)
-        audio = torch.transpose(audio[0, :, :], 0, 1)
-        audio = torch.log(audio + self.log_offset)
+        audio = torch.log(audio.T + self.log_offset)
         return audio
 
 
 class WORLDAudioProcessor(nn.Module):
     def __init__(
         self,
-        sample_rate: int
+        sample_rate: int,
+        use_mcep: bool
     ) -> None:
         from .vocoder import WORLDVocoder
         super().__init__()
         self.target_effects = [
             ["remix", "1"],
             ["rate", f"{sample_rate}"],
         ]
-        self.vocoder = WORLDVocoder(sample_rate=sample_rate)
+        self.vocoder = WORLDVocoder(sample_rate=sample_rate, use_mcep=use_mcep)
+
+    @property
+    def audio_size(self) -> int:
+        return sum(self.vocoder.output_dims)
 
     def forward(self, audiopath: Text) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         waveform, _ = torchaudio.sox_effects.apply_effects_file(audiopath, effects=self.target_effects)
-        f0, logspc, codeap = self.vocoder(waveform[0])
-        return f0, logspc, codeap
-
-
-class TextProcessor(nn.Module):
-    def __init__(
-        self,
-        phonemizer: Any,
-        tokenizer: Any,
-    ) -> None:
-        super().__init__()
-        self.phonemizer = phonemizer
-        self.tokenizer = tokenizer
-
-    def forward(self, text: Text) -> torch.Tensor:
-        phoneme = self.phonemizer(text) if self.phonemizer is not None else text
-        encoded = self.tokenizer(phoneme)
-        return encoded
-
-    @property
-    def vocab_size(self) -> int:
-        return self.tokenizer.vocab_size
+        f0, logspc_or_mcep, codeap = self.vocoder(waveform[0])
+        return f0, logspc_or_mcep, codeap
 
 
 def get_dataset(
+    data_dir: Text,
     dataset: Text,
     split: Text,
     use_align: bool = False,
     use_phone: bool = False,
     use_target: bool = False,
 ) -> Dataset:
+    r"""Get ``Dataset``
+
+    Args:
+        data_dir (str): Root directory of the dataset.
+        use_align (bool): Include aligned text or aligned
+            phone text. Used for TTS.
+        use_target (bool): Include both aligned phone text and
+            aligned text. Used for multi-task TTS.
+    """
+
     chained_ds: Dataset = None
     for dataset in dataset.split(','):
-        ds = get_base_dataset(dataset, split)
+        ds = get_base_dataset(data_dir, dataset, split)
 
         if use_target:
             assert use_align
-            alignfile = f'./data/{dataset}-align-{split}.txt'
+            alignfile = os.path.join(data_dir, f'{dataset}-align-{split}.txt')
             align_ds = TextDataset(alignfile, idcol=-1, textcol=1)
-            phonealignfile = f'./data/{dataset}-phone-align-{split}.txt'
+            phonealignfile = os.path.join(data_dir, f'{dataset}-phone-align-{split}.txt')
             phonealign_ds = TextDataset(phonealignfile, idcol=-1, textcol=1)
             ds = MergeDataset(ds, align_ds=align_ds, target_ds=phonealign_ds)
 
         elif use_align:
             if use_phone:
-                alignfile = f'./data/{dataset}-phone-align-{split}.txt'
+                alignfile = os.path.join(data_dir, f'{dataset}-phone-align-{split}.txt')
             else:
-                alignfile = f'./data/{dataset}-align-{split}.txt'
+                alignfile = os.path.join(data_dir, f'{dataset}-align-{split}.txt')
             align_ds = TextDataset(alignfile, idcol=-1, textcol=1)
             ds = MergeDataset(ds, align_ds=align_ds)
 
-        elif use_phone:
-            phonefile = f'./data/{dataset}-phone-{split}.txt'
-            phone_ds = TextDataset(phonefile)
-            ds = MergeDataset(ds, phone_ds=phone_ds)
+        else:
+            if use_phone:
+                textfile = os.path.join(data_dir, f'{dataset}-phone-{split}.txt')
+            else:
+                textfile = os.path.join(data_dir, f'{dataset}-{split}.txt')
+            text_ds = TextDataset(textfile)
+            ds = MergeDataset(ds, text_ds=text_ds)
 
         chained_ds = chained_ds + ds if chained_ds is not None else ds
 
     return chained_ds
 
 
-def get_base_dataset(dataset: Text, split: Text):
-    if dataset == 'librispeech':
-        ds = get_dataset_librispeech(split, variant="100")
+def get_base_dataset(data_dir: Text, dataset: Text, split: Text) -> Dataset:
+    if dataset.startswith('dummy_'):
+        language = dataset.replace('dummy_', '', 1)
+        root = os.path.join(data_dir, f'dummy-speech-{language}')
+        ds = MetafileDataset(
+            root, metafile='metadata.csv',
+            sep='|', header=False, idcol=0, ext='.wav')
+    elif dataset == 'librispeech':
+        ds = get_dataset_librispeech(data_dir, split, variant="100")
     elif dataset == 'librispeech_360':
-        ds = get_dataset_librispeech(split, variant="360")
+        ds = get_dataset_librispeech(data_dir, split, variant="360")
     elif dataset == 'ljspeech':
-        root = './data/LJSpeech-1.1'
+        root = os.path.join(data_dir, 'LJSpeech-1.1')
         ds = MetafileDataset(
             root, metafile='metadata.csv',
             sep='|', header=False, idcol=0, ext='.flac')
     elif dataset == 'cv_ja':
-        root = './data/cv-corpus-6.1-2020-12-11/ja'
+        root = os.path.join(data_dir, 'cv-corpus-12.0-2022-12-07/ja')
         ds = MetafileDataset(
             root,
             sep='\t', idcol=1, textcol=2, wavsdir='clips', ext='')
     elif dataset.startswith("kokoro_"):
         dataset_size = dataset.replace("kokoro_", "")
-        root = f'./data/kokoro-speech-v1_1-{dataset_size}'
+        root = os.path.join(data_dir, f'kokoro-speech-v1_2-{dataset_size}')
         ds = MetafileDataset(
             root, metafile='metadata.csv',
             sep='|', header=False, idcol=0, ext='.flac')
     else:
         raise ValueError("Unknown dataset")
     return ds
 
 
-def get_dataset_librispeech(split: Text, variant="100") -> Dataset:
-    root = "./data/LibriSpeech"
+def get_dataset_librispeech(data_dir: Text, split: Text, variant="100") -> Dataset:
+    root = os.path.join(data_dir, "LibriSpeech")
     if split == "train":
         root += "/train-clean-%s" % variant
     elif split == "valid":
         root += "/dev-clean"
     elif split == "test":
         root += "/test-clean"
     else:
@@ -395,53 +412,32 @@
     return LibriSpeechDataset(root)
 
 
 def get_audio_transform(vocoder: Text, sample_rate: int):
     if vocoder == 'mel':
         audio_transform = MelSpectrogramAudioTransform(sample_rate=sample_rate)
     elif vocoder == 'world':
-        audio_transform = WORLDAudioProcessor(sample_rate=sample_rate)
+        audio_transform = WORLDAudioProcessor(sample_rate=sample_rate, use_mcep=False)
+    elif vocoder == 'world_mcep':
+        audio_transform = WORLDAudioProcessor(sample_rate=sample_rate, use_mcep=True)
     else:
         raise ValueError('Unknown vocoder')
     return audio_transform
 
 
-def get_text_transform(language: Text, use_align: bool, use_phone: bool):
-    phonemizer = get_phonemizer(language=language, use_align=use_align, use_phone=use_phone)
-    tokenizer = get_tokenizer(language=language, use_phone=use_phone)
-    return TextProcessor(phonemizer, tokenizer)
-
-
-def get_phonemizer(language: Text, use_align: bool, use_phone: bool):
-    if use_align:
-        # Aligned texts are already phonemized.
-        return None
-    if use_phone:
-        assert language == "en"
-        return None
-    if language == 'en':
-        return BasicPhonemizer()
-    elif language == 'ja':
-        from .japanese import JapanesePhonemizer
-        return JapanesePhonemizer()
-    else:
-        raise ValueError(f"Unsupported language {language}")
-
-
 def get_tokenizer(language: Text, use_phone: bool):
     if use_phone:
-        assert language == "en"
-        return CMUTokenizer()
+        return BasicTokenizer(language=language)
     return CharTokenizer()
 
 
 def get_collate_fn(vocoder, use_target):
     if vocoder == "mel":
         collate_fn = generate_audio_text_batch
-    elif vocoder == "world":
+    elif vocoder == "world" or vocoder == "world_mcep":
         if use_target:
             collate_fn = generate_audio_text_align_target_batch
         else:
             collate_fn = generate_audio_text_align_batch
     else:
         raise ValueError('Unknown vocoder')
     return collate_fn
@@ -450,15 +446,15 @@
 def generate_audio_text_batch(data_batch):
     audio_batch, text_batch = [], []
     for audio_item, text_item in data_batch:
         audio_batch.append(audio_item)
         text_batch.append(text_item)
     audio_len = torch.tensor([len(x) for x in audio_batch], dtype=torch.int32)
     text_len = torch.tensor([len(x) for x in text_batch], dtype=torch.int32)
-    audio_batch = pad_sequence(audio_batch, batch_first=True, padding_value=0)
+    audio_batch = pad_sequence(audio_batch, batch_first=True, padding_value=BLANK_AUDIO)
     text_batch = pad_sequence(text_batch, batch_first=True, padding_value=BLANK_IDX)
     return (audio_batch, audio_len), (text_batch, text_len)
 
 
 def generate_audio_text_align_batch(data_batch):
     f0_batch, spec_batch, codeap_batch, aligntext_batch = [], [], [], []
     for (f0_item, spec_item, codeap_item), aligntext_item in data_batch:
@@ -496,121 +492,142 @@
     codeap_batch = pad_sequence(codeap_batch, batch_first=True, padding_value=0)
     text_batch = pad_sequence(text_batch, batch_first=True, padding_value=BLANK_IDX)
     targettext_batch = pad_sequence(targettext_batch, batch_first=True, padding_value=BLANK_IDX)
 
     return (f0_batch, f0_len, spec_batch, codeap_batch), (text_batch, text_len), (targettext_batch, targettext_len)
 
 
-class AudioTextDataModule(pl.LightningDataModule):
+class Voice100DataModuleBase(pl.LightningDataModule):
+    pass
+
+
+class AudioTextDataModule(Voice100DataModuleBase):
     """Data module to read text and audio pairs and optionally aligned texts.
 
         Args:
-            task: ``mel`` or ``world``
+            vocoder: ``mel`` or ``world``
             dataset: Dataset to use
             sample_rate: Sampling rate of audio
             language: Language
             use_phone: Use phoneme for input
             cache: Cache directory
             batch_size: Batch size
             valid_ratio: Validation split ratio
             test: Unit test mode
     """
 
     def __init__(
         self,
-        vocoder: Text,
+        vocoder: Text = None,
         dataset: Text = "ljspeech",
         sample_rate: int = 16000,
         language: Text = "en",
         use_align: bool = False,
         use_phone: bool = False,
         use_target: bool = False,
-        cache: Text = './cache',
+        data_dir: Text = './data',
+        cache_dir: Text = './cache',
         batch_size: int = 128,
+        num_workers: int = 0,
         valid_ratio: float = 0.1
     ) -> None:
         super().__init__()
         self.vocoder = vocoder
         self.dataset = dataset
         self.split_dataset = dataset != "librispeech"
         self.valid_ratio = valid_ratio
         self.sample_rate = sample_rate
         self.language = language
+        self.use_align = use_align
         self.use_phone = use_phone
         self.use_target = use_target
-        self.cache = cache
-        self.cache_salt = self.vocoder.encode('utf-8')
+        self.data_dir = data_dir
+        self.cache_dir = cache_dir
+        self.cache_salt = ("world" if self.vocoder == "world_mcep" else self.vocoder).encode('utf-8')
         self.batch_size = batch_size
-        self.num_workers = 2
+        self.num_workers = num_workers
         self.collate_fn = get_collate_fn(self.vocoder, self.use_target)
         self.audio_transform = get_audio_transform(self.vocoder, self.sample_rate)
-        self.text_transform = get_text_transform(self.language, use_align=use_align, use_phone=use_phone)
+        self.text_transform = get_tokenizer(language=self.language, use_phone=use_phone)
         if use_target:
-            self.targettext_transform = get_text_transform(self.language, use_align=use_align, use_phone=True)
+            self.targettext_transform = get_tokenizer(language=self.language, use_phone=True)
         else:
             self.targettext_transform = None
-        self.audio_size = MELSPEC_DIM
         self.train_ds = None
         self.valid_ds = None
         self.test_ds = None
         self.predict_ds = None
 
     @property
+    def audio_size(self) -> int:
+        return self.audio_transform.audio_size
+
+    @property
     def vocab_size(self) -> int:
         return self.text_transform.vocab_size
 
     @property
     def target_vocab_size(self) -> int:
         return self.targettext_transform.vocab_size
 
     def setup(self, stage: Optional[str] = None):
         ds = get_dataset(
+            self.data_dir,
             self.dataset,
             split="train",
-            use_align=self.vocoder == "world",
+            use_align=self.use_align,
             use_phone=self.use_phone,
             use_target=self.use_target)
-        os.makedirs(self.cache, exist_ok=True)
+        os.makedirs(self.cache_dir, exist_ok=True)
 
         if stage == "predict":
             self.predict_ds = EncodedCacheDataset(
                 ds,
                 audio_transform=self.audio_transform,
                 text_transform=self.text_transform,
                 targettext_transform=self.targettext_transform,
-                cachedir=self.cache, salt=self.cache_salt)
+                cachedir=self.cache_dir, salt=self.cache_salt)
+
+        elif stage == "test":
+            self.test_ds = EncodedCacheDataset(
+                ds,
+                audio_transform=self.audio_transform,
+                text_transform=self.text_transform,
+                targettext_transform=self.targettext_transform,
+                cachedir=self.cache_dir, salt=self.cache_salt)
 
         else:
             if self.split_dataset:
                 # Split the dataset
                 total_len = len(ds)
                 valid_len = int(total_len * self.valid_ratio)
                 train_len = total_len - valid_len
                 train_ds, valid_ds = torch.utils.data.random_split(ds, [train_len, valid_len])
             else:
                 train_ds = ds
                 valid_ds = get_dataset(
+                    self.data_dir,
                     self.dataset,
                     split="valid",
-                    use_align=self.vocoder == "world",
+                    use_align=self.use_align,
                     use_phone=self.use_phone,
                     use_target=self.use_target)
 
             self.train_ds = EncodedCacheDataset(
                 train_ds,
                 audio_transform=self.audio_transform,
                 text_transform=self.text_transform,
                 targettext_transform=self.targettext_transform,
-                cachedir=self.cache, salt=self.cache_salt)
+                cachedir=self.cache_dir, salt=self.cache_salt)
             self.valid_ds = EncodedCacheDataset(
                 valid_ds,
                 audio_transform=self.audio_transform,
                 text_transform=self.text_transform,
                 targettext_transform=self.targettext_transform,
-                cachedir=self.cache, salt=self.cache_salt)
+                cachedir=self.cache_dir, salt=self.cache_salt)
 
     def train_dataloader(self):
         if self.train_ds is None:
             return None
         return DataLoader(
             self.train_ds,
             batch_size=self.batch_size,
@@ -661,48 +678,50 @@
     text_len = torch.tensor([len(x) for x in text_batch], dtype=torch.int32)
     align_len = torch.tensor([len(x) for x in align_batch], dtype=torch.int32)
     text_batch = pad_sequence(text_batch, batch_first=True, padding_value=BLANK_IDX)
     align_batch = pad_sequence(align_batch, batch_first=True, padding_value=0)
     return (text_batch, text_len), (align_batch, align_len)
 
 
-class AlignTextDataModule(pl.LightningDataModule):
+class AlignTextDataModule(Voice100DataModuleBase):
     """Data module to read text and audio pairs and optionally aligned texts.
 
         Args:
             dataset: Dataset to use
             batch_size: Batch size
     """
 
     def __init__(
         self,
+        data_dir: Text = "./data",
         dataset: Text = "ljspeech",
         language: Text = "en",
         use_phone: bool = False,
         valid_ratio: float = 0.1,
         batch_size: int = 256
     ) -> None:
         super().__init__()
+        self.data_dir = data_dir
         self.dataset = dataset
         self.use_phone = use_phone
         self.valid_ratio = valid_ratio
         self.num_workers = 2
         self.collate_fn = generate_text_align_batch
         self.encoder = get_tokenizer(language, use_phone)
         self.batch_size = batch_size
 
     @property
     def vocab_size(self) -> int:
         return self.encoder.vocab_size
 
     def setup(self, stage: Optional[str] = None):
         if self.use_phone:
-            file = f"./data/{self.dataset}-phone-align-train.txt"
+            file = os.path.join(self.data_dir, f"{self.dataset}-phone-align-train.txt")
         else:
-            file = f"./data/{self.dataset}-align-train.txt"
+            file = os.path.join(self.data_dir, f"{self.dataset}-align-train.txt")
         ds = AlignTextDataset(file, encoder=self.encoder)
         # Split the dataset
         total_len = len(ds)
         valid_len = int(total_len * self.valid_ratio)
         train_len = total_len - valid_len
         self.train_ds, self.valid_ds = torch.utils.data.random_split(ds, [train_len, valid_len])
```

### Comparing `voice100-1.3.2/voice100/export_onnx.py` & `voice100-1.6.0/voice100/export_onnx_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
             "audio": {0: "batch_size", 1: "audio_len"},
             "logits": {0: "batch_size", 1: "logits_len"},
         },
     )
 
 
 def export_onnx_asr(args):
-    from .models.asr import AudioToCharCTC
+    from .models.asr import AudioToTextCTC
 
-    model = AudioToCharCTC.load_from_checkpoint(args.checkpoint)
+    model = AudioToTextCTC.load_from_checkpoint(args.checkpoint)
     model.eval()
 
     audio = torch.rand(size=[1, 100, MELSPEC_DIM], dtype=torch.float32)
 
     torch.onnx.export(
         model,
         audio,
```

### Comparing `voice100-1.3.2/voice100/japanese/__init__.py` & `voice100-1.6.0/voice100/japanese/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,24 +7,38 @@
 
 __all__ = [
     "JapanesePhonemizer",
 ]
 
 _CHOON_RX = re.compile(r'(.):')
 _CLEAN_RX = re.compile(r"[^ a-z']")
+_SPACES_RX = re.compile(r"\s+")
 
 
 class JapanesePhonemizer(nn.Module):
+    """Phonemizer class that translates Japanese kana-kanji texts to Julius-style phonemes.
+    """
 
-    def __init__(self):
+    def __init__(self, use_phone: bool = False):
         super().__init__()
+        self._use_phone = use_phone
 
     def forward(self, text: Text) -> Text:
         text = text2kata(text)
         text = kata2phoneme(text)
+        if self._use_phone:
+            text = text.replace('N', "n'")
+            text = text.lower()
+            text = text.replace("n'", 'N')
+            text = text.replace('-', '')
+            text = text.replace('c ', 'k ')
+            text = text.replace('x', 'k')
+            text = text.replace('v', 'b')
+            text = _SPACES_RX.sub(' ', text)
+            return text
         text = text.replace(' ', '')
         text = text.replace(',', ' ')
         text = text.replace('.', ' ')
         text = _CHOON_RX.sub(r'\1\1', text)
         text = text.replace("N", "n'")
         text = text.replace('q', "'")
         text = _CLEAN_RX.sub(r'', text.lower())
```

### Comparing `voice100-1.3.2/voice100/japanese/phonemizer.py` & `voice100-1.6.0/voice100/japanese/phonemizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Convert Japanese text to phonemes which is
 # compatible with Julius https://github.com/julius-speech/segmentation-kit
 
 import re
-import MeCab
+import fugashi
 from typing import Text
 
 _CONVRULES = [
     # Conversion of 2 letters
     'アァ/ a a',
     'イィ/ i i',
     'イェ/ i e',
@@ -305,17 +305,17 @@
 ]
 
 _COLON_RX = re.compile(':+')
 _REJECT_RX = re.compile('[^ a-zA-Z:,.?]')
 
 
 def _makerulemap():
-    l = [tuple(x.split('/')) for x in _CONVRULES]
+    rules = [tuple(x.split('/')) for x in _CONVRULES]
     return tuple(
-        {k: v for k, v in l if len(k) == i}
+        {k: v for k, v in rules if len(k) == i}
         for i in (1, 2)
     )
 
 
 _RULEMAP1, _RULEMAP2 = _makerulemap()
 
 
@@ -350,15 +350,15 @@
 def hira2kata(text: Text) -> Text:
     text = text.translate(_HIRA2KATATRANS)
     return text.replace('う゛', 'ヴ')
 
 
 _SYMBOL_TOKENS = set(list('・、。？！'))
 _NO_YOMI_TOKENS = set(list('「」『』―（）［］[]　…'))
-_TAGGER = MeCab.Tagger()
+_TAGGER = fugashi.Tagger()
 
 
 def text2kata(text: Text) -> Text:
     parsed = _TAGGER.parse(text)
     res = []
     for line in parsed.split('\n'):
         if line == 'EOS':
```

### Comparing `voice100-1.3.2/voice100/models/align.py` & `voice100-1.6.0/voice100/models/align.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
-from argparse import ArgumentParser
+from argparse import _ArgumentGroup
 from typing import Tuple
 import torch
 import numpy as np
 from torch import nn
-import pytorch_lightning as pl
 from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence, pad_sequence
 
+from ._base import Voice100ModelBase
 from ..audio import BatchSpectrogramAugumentation
 
 __all__ = [
     'AudioAlignCTC',
 ]
 
 
@@ -22,15 +22,15 @@
     # Expand label with blanks
     tmp = labels
     labels = np.zeros(labels.shape[0] * 2 + 1, dtype=labels.dtype)
     labels[1::2] = tmp
     labels_len = labels.shape[0]
 
     beams = [np.array([-1, -1], dtype=np.int32)]
-    scores = np.array([logits[0, 0], logits[0, labels[0]]], logits.dtype)
+    scores = np.array([logits[0, labels[0]], logits[0, labels[1]]], dtype=logits.dtype)
 
     for i in range(1, logits_len):
 
         next_label_pos_min = 0
         next_label_pos_max = min(scores.shape[0] + max_move - 1, labels_len)
 
         next_beam = np.zeros([max_move, next_label_pos_max - next_label_pos_min], dtype=np.int32)
@@ -62,32 +62,34 @@
         j = beams[i][j]
 
     best_labels = labels[best_path]
 
     return best_score, best_path, best_labels
 
 
-class AudioAlignCTC(pl.LightningModule):
+class AudioAlignCTC(Voice100ModelBase):
 
     def __init__(self, audio_size, vocab_size, hidden_size, num_layers, learning_rate):
         super().__init__()
         self.save_hyperparameters()
         self.conv = nn.Conv1d(audio_size, hidden_size, kernel_size=3, stride=2, padding=1)
+        self.relu = nn.ReLU()
         self.lstm = nn.LSTM(
             input_size=hidden_size, hidden_size=hidden_size,
             num_layers=num_layers, dropout=0.2, bidirectional=True)
         self.dense = nn.Linear(hidden_size * 2, vocab_size)
-        self.loss_fn = nn.CTCLoss()
+        # zero_infinity for broken short audio clips
+        self.criterion = nn.CTCLoss(zero_infinity=True)
         self.batch_augment = BatchSpectrogramAugumentation()
 
     def forward(self, audio: torch.Tensor, audio_len: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         # audio: [batch_size, audio_len, audio_size]
         x = torch.transpose(audio, 1, 2)
         x = self.conv(x)
-        x = torch.relu(x)
+        x = self.relu(x)
         x_len = torch.divide(audio_len + 1, 2, rounding_mode='trunc')
         x = torch.transpose(x, 1, 2)
         packed_audio = pack_padded_sequence(x, x_len.cpu(), batch_first=True, enforce_sorted=False)
         packed_lstm_out, _ = self.lstm(packed_audio)
         lstm_out, lstm_out_len = pad_packed_sequence(packed_lstm_out, batch_first=False)
         return self.dense(lstm_out), lstm_out_len
 
@@ -98,50 +100,55 @@
             audio, audio_len = self.batch_augment(audio, audio_len)
         # audio: [batch_size, audio_len, audio_size]
         # text: [batch_size, text_len]
         logits, logits_len = self.forward(audio, audio_len)
         # logits: [audio_len, batch_size, vocab_size]
         log_probs = nn.functional.log_softmax(logits, dim=-1)
         log_probs_len = logits_len
-        return self.loss_fn(log_probs, text, log_probs_len, text_len)
+        return self.criterion(log_probs, text, log_probs_len, text_len)
 
     def training_step(self, batch, batch_idx):
-        self.optimizers().param_groups[0]['lr'] = 0.001
         loss = self._calc_batch_loss(batch)
-        self.log('train_loss', loss)
+        metrics = {"train_loss": loss}
+        self.log_dict(metrics)
         return loss
 
     def validation_step(self, batch, batch_idx):
         loss = self._calc_batch_loss(batch)
-        self.log('val_loss', loss)
+        metrics = {"val_loss": loss}
+        self.log_dict(metrics)
+        return metrics
 
     def test_step(self, batch, batch_idx):
         loss = self._calc_batch_loss(batch)
-        self.log('test_loss', loss)
+        metrics = {"test_loss": loss}
+        self.log_dict(metrics)
+        return metrics
 
     def configure_optimizers(self):
         optimizer = torch.optim.Adam(
             self.parameters(),
-            lr=self.hparams.learning_rate,
-            weight_decay=0.00004)
+            lr=self.hparams.learning_rate)
         return optimizer
 
     @torch.no_grad()
     def ctc_best_path(
         self, audio: torch.Tensor = None,
         audio_len: torch.Tensor = None, text: torch.Tensor = None,
         text_len: torch.Tensor = None, logits: torch.Tensor = None
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
         # logits [audio_len, batch_size, vocab_size]
         if logits is None:
             logits, logits_len = self.forward(audio, audio_len)
+            logits = nn.functional.log_softmax(logits, dim=-1)
         else:
             logits_len = audio_len
         if text is None:
             return logits.argmax(axis=-1)
+        text_len = torch.minimum(logits_len, text_len.cpu())  # For very short audio
         score = []
         hist = []
         path = []
         for i in range(logits.shape[1]):
             one_logits_len = logits_len[i].cpu().item()
             one_logits = logits[:one_logits_len, i, :].cpu().numpy()
             one_text_len = text_len[i].cpu().numpy()
@@ -153,20 +160,20 @@
             path.append(torch.from_numpy(one_path))
         score = torch.tensor(one_path, dtype=torch.float32)
         hist = pad_sequence(hist, batch_first=True, padding_value=0)
         path = pad_sequence(path, batch_first=True, padding_value=0)
         return score, hist, path, logits_len
 
     @staticmethod
-    def add_model_specific_args(parent_parser):
-        parser = ArgumentParser(parents=[parent_parser], add_help=False)
-        parser.add_argument('--learning_rate', type=float, default=0.001)
-        parser.add_argument('--hidden_size', type=float, default=128)
+    def add_model_specific_args(parent_parser: _ArgumentGroup):
+        parser = parent_parser.add_argument_group("voice100.models.align.AudioAlignCTC")
+        parser.add_argument('--hidden_size', type=int, default=128)
         parser.add_argument('--num_layers', type=int, default=2)
-        return parser
+        parser.add_argument('--learning_rate', type=float, default=0.001)
+        return parent_parser
 
     @staticmethod
     def from_argparse_args(args, **kwargs):
         return AudioAlignCTC(
             hidden_size=args.hidden_size,
             num_layers=args.num_layers,
             learning_rate=args.learning_rate,
```

### Comparing `voice100-1.3.2/voice100/models/asr.py` & `voice100-1.6.0/voice100/models/asr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
-from argparse import ArgumentParser
+from argparse import _ArgumentGroup
 import torch
 from torch import nn
-import pytorch_lightning as pl
 
 from ..audio import BatchSpectrogramAugumentation
+from ._base import Voice100ModelBase
 
 __all__ = [
-    'AudioToCharCTC',
+    'AudioToTextCTC',
 ]
 
 
 def generate_padding_mask(x: torch.Tensor, length: torch.Tensor) -> torch.Tensor:
     """
     Args:
         x: tensor of shape [batch_size, length, audio_dim]
@@ -90,23 +90,24 @@
             nn.Dropout(0.2),
             nn.Conv1d(in_channels, out_channels, kernel_size=1, padding=0, bias=True))
 
     def forward(self, enc_out) -> torch.Tensor:
         return self.layers(enc_out)
 
 
-class AudioToCharCTC(pl.LightningModule):
+class AudioToTextCTC(Voice100ModelBase):
 
     def __init__(self, audio_size, embed_size, vocab_size, hidden_size, learning_rate, weight_decay):
         super().__init__()
         self.save_hyperparameters()
         self.embed_size = embed_size
         self.encoder = ConvVoiceEncoder(audio_size, embed_size, hidden_size)
         self.decoder = LinearCharDecoder(embed_size, vocab_size)
-        self.loss_fn = nn.CTCLoss()
+        # zero_infinity for broken short audio clips
+        self.criterion = nn.CTCLoss(zero_infinity=True)
         self.batch_augment = BatchSpectrogramAugumentation()
         self.do_normalize = False
 
     def forward(self, audio) -> torch.Tensor:
         audio = torch.transpose(audio, 1, 2)
         enc_out = self.encoder(audio)
         logits = self.decoder(enc_out)
@@ -144,47 +145,52 @@
         # logits: [batch_size, audio_len, vocab_size]
         logits_len = self.output_length(audio_len)
 
         logits = torch.transpose(logits, 0, 1)
         # logits: [audio_len, batch_size, vocab_size]
         log_probs = nn.functional.log_softmax(logits, dim=-1)
         log_probs_len = logits_len
-        return self.loss_fn(log_probs, text, log_probs_len, text_len)
+        return self.criterion(log_probs, text, log_probs_len, text_len)
 
     def training_step(self, batch, batch_idx):
         loss = self._calc_batch_loss(batch)
-        self.log('train_loss', loss)
+        metrics = {"train_loss": loss}
+        self.log_dict(metrics)
         return loss
 
     def validation_step(self, batch, batch_idx):
         loss = self._calc_batch_loss(batch)
-        self.log('val_loss', loss)
+        metrics = {"val_loss": loss}
+        self.log_dict(metrics)
+        return metrics
 
     def test_step(self, batch, batch_idx):
         loss = self._calc_batch_loss(batch)
-        self.log('test_loss', loss)
+        metrics = {"test_loss": loss}
+        self.log_dict(metrics)
+        return metrics
 
     def configure_optimizers(self):
         optimizer = torch.optim.Adam(
             self.parameters(),
             lr=self.hparams.learning_rate,
             weight_decay=self.hparams.weight_decay)
         scheduler = torch.optim.lr_scheduler.StepLR(optimizer, step_size=1, gamma=0.98)
         return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
     @staticmethod
-    def add_model_specific_args(parent_parser):
-        parser = ArgumentParser(parents=[parent_parser], add_help=False)
-        parser.add_argument('--learning_rate', type=float, default=0.0001)
+    def add_model_specific_args(parent_parser: _ArgumentGroup):
+        parser = parent_parser.add_argument_group("voice100.models.asr.AudioToTextCTC")
+        parser.add_argument('--learning_rate', type=float, default=0.001)
         parser.add_argument('--weight_decay', type=float, default=0.00004)
         parser.add_argument('--hidden_size', type=float, default=512)
         parser.add_argument('--embed_size', type=float, default=512)
-        return parser
+        return parent_parser
 
     @staticmethod
     def from_argparse_args(args, **kwargs):
-        return AudioToCharCTC(
+        return AudioToTextCTC(
             embed_size=args.embed_size,
             hidden_size=args.hidden_size,
             learning_rate=args.learning_rate,
             weight_decay=args.weight_decay,
             **kwargs)
```

### Comparing `voice100-1.3.2/voice100/models/tts.py` & `voice100-1.6.0/voice100/models/tts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,19 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
 from argparse import ArgumentParser
 from typing import Tuple
-import pytorch_lightning as pl
 import torch
 from torch import nn
 
+from ._base import Voice100ModelBase
+from ._layers_v1 import generate_padding_mask, WORLDNorm, WORLDLoss
 from .asr import InvertedResidual
 
 
-def generate_padding_mask(x: torch.Tensor, length: torch.Tensor) -> torch.Tensor:
-    """
-    Args:
-        x: tensor of shape [batch_size, length]
-        length: tensor of shape [batch_size]
-    Returns:
-        float tensor of shape [batch_size, length]
-    """
-    assert x.dim() == 2
-    assert length.dim() == 1
-    return (torch.arange(x.shape[1], device=x.device)[None, :] < length[:, None]).to(x.dtype)
-
-
 class VoiceDecoder(nn.Module):
     def __init__(self, hidden_size, out_channels) -> None:
         super().__init__()
         half_hidden_size = hidden_size // 2
         self.layers = nn.Sequential(
             InvertedResidual(hidden_size, hidden_size, kernel_size=65),
             InvertedResidual(hidden_size, hidden_size, kernel_size=33),
@@ -72,96 +60,15 @@
     if x.shape[1] > y.shape[1]:
         return x[:, :y.shape[1]], y
     if x.shape[1] < y.shape[1]:
         return x, y[:, :x.shape[1]]
     return x, y
 
 
-class WORLDNorm(nn.Module):
-    def __init__(self, logspc_size: int, codeap_size: int, device=None, dtype=None):
-        factory_kwargs = {'device': device, 'dtype': dtype}
-        super().__init__()
-        self.f0_std = nn.Parameter(
-            torch.ones([1], **factory_kwargs),
-            requires_grad=False)
-        self.f0_mean = nn.Parameter(
-            torch.zeros([1], **factory_kwargs),
-            requires_grad=False)
-        self.logspc_std = nn.Parameter(
-            torch.ones([logspc_size], **factory_kwargs),
-            requires_grad=False)
-        self.logspc_mean = nn.Parameter(
-            torch.zeros([logspc_size], **factory_kwargs),
-            requires_grad=False)
-        self.codeap_std = nn.Parameter(
-            torch.ones([codeap_size], **factory_kwargs),
-            requires_grad=False)
-        self.codeap_mean = nn.Parameter(
-            torch.zeros([codeap_size], **factory_kwargs),
-            requires_grad=False)
-
-    def forward(self, f0, mcep, codeap):
-        return self.normalize(f0, mcep, codeap)
-
-    @torch.no_grad()
-    def normalize(
-        self, f0: torch.Tensor, mcep: torch.Tensor, codeap: torch.Tensor
-    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        f0 = (f0 - self.f0_mean) / self.f0_std
-        mcep = (mcep - self.logspc_mean) / self.logspc_std
-        codeap = (codeap - self.codeap_mean) / self.codeap_std
-        return f0, mcep, codeap
-
-    @torch.no_grad()
-    def unnormalize(
-        self, f0: torch.Tensor, mcep: torch.Tensor, codeap: torch.Tensor
-    ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        f0 = self.f0_std * f0 + self.f0_mean
-        mcep = self.logspc_std * mcep + self.logspc_mean
-        codeap = self.codeap_std * codeap + self.codeap_mean
-        return f0, mcep, codeap
-
-
-class WORLDLoss(nn.Module):
-    def __init__(self, sample_rate: int = 16000, n_fft: int = 512, device=None, dtype=None):
-        super().__init__()
-        self.bce_loss = nn.BCEWithLogitsLoss(reduction='none')
-        self.l1_loss = nn.L1Loss(reduction='none')
-
-        f = (sample_rate / n_fft) * torch.arange(
-            n_fft // 2 + 1, device=device, dtype=dtype if dtype is not None else torch.float32)
-        dm = 1127 / (700 + f)
-        logspc_weights = dm / torch.sum(dm)
-        self.register_buffer('logspc_weights', logspc_weights, persistent=False)
-
-    def forward(
-        self, length: torch.Tensor,
-        hasf0_logits: torch.Tensor, f0_hat: torch.Tensor, logspc_hat: torch.Tensor, codeap_hat: torch.Tensor,
-        hasf0: torch.Tensor, f0: torch.Tensor, logspc: torch.Tensor, codeap: torch.Tensor
-    ) -> torch.Tensor:
-
-        hasf0_logits, hasf0 = adjust_size(hasf0_logits, hasf0)
-        f0_hat, f0 = adjust_size(f0_hat, f0)
-        logspc_hat, logspc = adjust_size(logspc_hat, logspc)
-        codeap_hat, codeap = adjust_size(codeap_hat, codeap)
-
-        mask = generate_padding_mask(f0, length)
-        hasf0_loss = self.bce_loss(hasf0_logits, hasf0) * mask
-        f0_loss = self.l1_loss(f0_hat, f0) * hasf0 * mask
-        logspc_loss = torch.sum(self.l1_loss(logspc_hat, logspc) * self.logspc_weights[None, None, :], axis=2) * mask
-        codeap_loss = torch.mean(self.l1_loss(codeap_hat, codeap), axis=2) * mask
-        mask_sum = torch.sum(mask)
-        hasf0_loss = torch.sum(hasf0_loss) / mask_sum
-        f0_loss = torch.sum(f0_loss) / mask_sum
-        logspc_loss = torch.sum(logspc_loss) / mask_sum
-        codeap_loss = torch.sum(codeap_loss) / mask_sum
-        return hasf0_loss, f0_loss, logspc_loss, codeap_loss
-
-
-class TextToAlignTextModel(pl.LightningModule):
+class TextToAlignTextModel(Voice100ModelBase):
     def __init__(self, vocab_size, hidden_size, learning_rate) -> None:
         super().__init__()
         self.save_hyperparameters()
         self.embedding = nn.Embedding(vocab_size, hidden_size)
         self.layers = nn.Sequential(
             InvertedResidual(hidden_size, hidden_size, kernel_size=5),
             InvertedResidual(hidden_size, hidden_size, kernel_size=11),
@@ -238,33 +145,33 @@
     def from_argparse_args(args, **kwargs):
         return TextToAlignTextModel(
             hidden_size=args.hidden_size,
             learning_rate=args.learning_rate,
             **kwargs)
 
 
-class AlignTextToAudioModel(pl.LightningModule):
+class AlignTextToAudioModel(Voice100ModelBase):
     def __init__(
-        self, vocab_size: int, hidden_size: int, learning_rate: float
+        self, vocab_size: int, hidden_size: int, learning_rate: float, use_mcep: bool = False
     ) -> None:
         super().__init__()
         self.save_hyperparameters()
         self.hidden_size = hidden_size
         self.vocab_size = vocab_size
         self.sample_rate = 16000
         self.n_fft = 512
         self.hasf0_size = 1
         self.f0_size = 1
-        self.logspc_size = self.n_fft // 2 + 1
+        self.logspc_size = 25 if use_mcep else self.n_fft // 2 + 1
         self.codeap_size = 1
         self.embedding = nn.Embedding(vocab_size, hidden_size)
         self.audio_size = self.hasf0_size + self.f0_size + self.logspc_size + self.codeap_size
         self.decoder = VoiceDecoder(hidden_size, self.audio_size)
         self.norm = WORLDNorm(self.logspc_size, self.codeap_size)
-        self.criteria = WORLDLoss(sample_rate=self.sample_rate, n_fft=self.n_fft)
+        self.criterion = WORLDLoss(use_mel_weights=not use_mcep, sample_rate=self.sample_rate, n_fft=self.n_fft)
 
     def forward(
         self, aligntext: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
 
         x = self.embedding(aligntext)
         x = torch.transpose(x, 1, 2)
@@ -296,15 +203,15 @@
     def _calc_batch_loss(self, batch) -> Tuple[torch.Tensor, ...]:
         (f0, f0_len, logspc, codeap), (aligntext, aligntext_len) = batch
         hasf0 = (f0 >= 30.0).to(torch.float32)
         f0, logspc, codeap = self.norm.normalize(f0, logspc, codeap)
 
         hasf0_logits, f0_hat, logspc_hat, codeap_hat = self.forward(aligntext)
 
-        hasf0_loss, f0_loss, logspc_loss, codeap_loss = self.criteria(
+        hasf0_loss, f0_loss, logspc_loss, codeap_loss = self.criterion(
             f0_len, hasf0_logits, f0_hat, logspc_hat, codeap_hat, hasf0, f0, logspc, codeap)
 
         return hasf0_loss, f0_loss, logspc_loss, codeap_loss
 
     def training_step(self, batch, batch_idx) -> torch.Tensor:
         hasf0_loss, f0_loss, logspc_loss, codeap_loss = self._calc_batch_loss(batch)
         loss = hasf0_loss + f0_loss + logspc_loss + codeap_loss
@@ -333,50 +240,53 @@
             self.parameters(),
             lr=self.hparams.learning_rate)
 
     @staticmethod
     def add_model_specific_args(parent_parser):
         parser = ArgumentParser(parents=[parent_parser], add_help=False)
         parser.add_argument('--hidden_size', type=int, default=512)
+        parser.add_argument('--audio_stat', type=str)
         parser.add_argument('--learning_rate', type=float, default=1e-3)
         return parser
 
     @staticmethod
     def from_argparse_args(args, **kwargs):
         model = AlignTextToAudioModel(
             hidden_size=args.hidden_size,
             learning_rate=args.learning_rate,
+            use_mcep=args.vocoder == "world_mcep",
             **kwargs)
         if not args.resume_from_checkpoint:
-            args.audio_stat = f'./data/{args.dataset}-stat.pt'
+            if args.audio_stat is None:
+                args.audio_stat = f'./data/{args.dataset}-stat.pt'
             model.norm.load_state_dict(torch.load(args.audio_stat))
         return model
 
 
-class AlignTextToAudioMultiTaskModel(pl.LightningModule):
+class AlignTextToAudioMultiTaskModel(Voice100ModelBase):
     def __init__(
-        self, vocab_size: int, target_vocab_size: int, hidden_size: int, learning_rate: float
+        self, vocab_size: int, target_vocab_size: int, hidden_size: int, learning_rate: float, use_mcep: bool = False
     ) -> None:
         super().__init__()
         self.save_hyperparameters()
         self.hidden_size = hidden_size
         self.vocab_size = vocab_size
         self.target_vocab_size = target_vocab_size
         self.sample_rate = 16000
         self.n_fft = 512
         self.hasf0_size = 1
         self.f0_size = 1
-        self.logspc_size = self.n_fft // 2 + 1
+        self.logspc_size = 25 if use_mcep else self.n_fft // 2 + 1
         self.codeap_size = 1
         self.embedding = nn.Embedding(vocab_size, hidden_size)
         self.audio_size = self.hasf0_size + self.f0_size + self.logspc_size + self.codeap_size
         self.decoder = VoiceMultiTaskDecoder(hidden_size, self.audio_size, self.target_vocab_size)
         self.norm = WORLDNorm(self.logspc_size, self.codeap_size)
-        self.criteria = WORLDLoss(sample_rate=self.sample_rate, n_fft=self.n_fft)
-        self.target_criteria = nn.CrossEntropyLoss(reduction='none')
+        self.criterion = WORLDLoss(sample_rate=self.sample_rate, n_fft=self.n_fft, use_logspc_weights=not use_mcep)
+        self.target_criterion = nn.CrossEntropyLoss(reduction='none')
 
     def forward(
         self, aligntext: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
 
         x = self.embedding(aligntext)
         x = torch.transpose(x, 1, 2)
@@ -409,17 +319,17 @@
     def _calc_batch_loss(self, batch) -> Tuple[torch.Tensor, ...]:
         (f0, f0_len, logspc, codeap), (aligntext, aligntext_len), (phonetext, phonetext_len) = batch
         hasf0 = (f0 >= 30.0).to(torch.float32)
         f0, logspc, codeap = self.norm.normalize(f0, logspc, codeap)
 
         hasf0_logits, f0_hat, logspc_hat, codeap_hat, target_logits = self.forward(aligntext)
 
-        hasf0_loss, f0_loss, logspc_loss, codeap_loss = self.criteria(
+        hasf0_loss, f0_loss, logspc_loss, codeap_loss = self.criterion(
             f0_len, hasf0_logits, f0_hat, logspc_hat, codeap_hat, hasf0, f0, logspc, codeap)
-        phone_loss = self.target_criteria(target_logits, phonetext)
+        phone_loss = self.target_criterion(target_logits, phonetext)
         mask = generate_padding_mask(phonetext, phonetext_len)
         mask_sum = torch.sum(mask)
         phone_loss = torch.sum(phone_loss * mask) / mask_sum
 
         return hasf0_loss, f0_loss, logspc_loss, codeap_loss, phone_loss
 
     def training_step(self, batch, batch_idx) -> torch.Tensor:
@@ -451,20 +361,23 @@
             self.parameters(),
             lr=self.hparams.learning_rate)
 
     @staticmethod
     def add_model_specific_args(parent_parser):
         parser = ArgumentParser(parents=[parent_parser], add_help=False)
         parser.add_argument('--hidden_size', type=int, default=512)
+        parser.add_argument('--audio_stat', type=str)
         parser.add_argument('--learning_rate', type=float, default=1e-3)
         return parser
 
     @staticmethod
     def from_argparse_args(args, **kwargs):
         model = AlignTextToAudioMultiTaskModel(
             hidden_size=args.hidden_size,
             learning_rate=args.learning_rate,
+            use_mcep=args.vocoder == "world_mcep",
             **kwargs)
         if not args.resume_from_checkpoint:
-            args.audio_stat = f'./data/{args.dataset}-stat.pt'
+            if args.audio_stat is None:
+                args.audio_stat = f'./data/{args.dataset}-stat.pt'
             model.norm.load_state_dict(torch.load(args.audio_stat))
         return model
```

### Comparing `voice100-1.3.2/voice100/text.py` & `voice100-1.6.0/voice100/text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
 import torch
 from torch import nn
 import re
-from typing import Text
+from typing import Text, List, Optional
 
 __all__ = [
     'BasicPhonemizer',
     'CharTokenizer',
-    'CMUTokenizer'
+    'BasicTokenizer'
 ]
 
 DEFAULT_CHARACTERS = "_ abcdefghijklmnopqrstuvwxyz'"
 NOT_DEFAULT_CHARACTERS_RX = re.compile("[^" + DEFAULT_CHARACTERS[1:] + "]")
 DEFAULT_VOCAB_SIZE = len(DEFAULT_CHARACTERS)
 assert DEFAULT_VOCAB_SIZE == 29
 
@@ -24,27 +24,62 @@
     'EY2', 'F', 'G', 'HH',
     'IH0', 'IH1', 'IH2', 'IY0', 'IY1', 'IY2', 'JH', 'K', 'L',
     'M', 'N', 'NG', 'OW0', 'OW1',
     'OW2', 'OY0', 'OY1', 'OY2', 'P', 'R', 'S', 'SH', 'T', 'TH',
     'UH0', 'UH1', 'UH2', 'UW',
     'UW0', 'UW1', 'UW2', 'V', 'W', 'Y', 'Z', 'ZH']
 
+assert len(CMU_VOCAB) == 71
+
+JA_VOCAB = [
+    '-', '!', ',', '.', '?', 'N', 'a', 'a:', 'b', 'by',
+    'ch', 'd', 'e', 'e:', 'f', 'g', 'gy', 'h', 'hy', 'i',
+    'i:', 'j', 'k', 'ky', 'm', 'my', 'n', 'ny', 'o', 'o:',
+    'p', 'py', 'q', 'r', 'ry', 's', 'sh', 't', 'ts', 'u',
+    'u:', 'w', 'y', 'z'
+]
+
+assert len(JA_VOCAB) == 44
+
+REPEATED_TOKENS_RX = re.compile(r'\n([^\n]+)(\n\1)+(?=\n)')
+REPEATED_BLANKS_RX = re.compile(r'(\n\t)+(?=\n)')
+
 
 class BasicPhonemizer(nn.Module):
+    """Phonemizer class that removes non-alphabet characters and keep
+    the others as it is.
+    """
 
     def __init__(self):
         super().__init__()
 
     def forward(self, text: Text) -> Text:
         return NOT_DEFAULT_CHARACTERS_RX.sub('', text.lower())
 
 
+class CMUPhonemizer(nn.Module):
+    """Phonemizer class to translate English texts to CMU phonemes.
+    Phonemes are separated by slashes (`/`)
+    """
+
+    def __init__(self):
+        super().__init__()
+        from g2p_en import G2p
+        self.g2p = G2p()
+
+    def forward(self, text: Text) -> Text:
+        phone = self.g2p(text)
+        return '/'.join(phone)
+
+
 class CharTokenizer(nn.Module):
+    """Tokenizer class that encodes one character to one token.
+    """
 
-    def __init__(self, vocab=None) -> None:
+    def __init__(self, vocab: Optional[List[Text]] = None) -> None:
         super().__init__()
         if vocab is None:
             vocab = DEFAULT_CHARACTERS
         self.vocab_size = len(vocab)
         self._vocab = vocab
         self._v2i = {x: i for i, x in enumerate(vocab)}
 
@@ -65,31 +100,46 @@
         text = re.sub(r'(.)\1+', r'\1', text)
         text = text.replace('_', '')
         if text == ' ':
             text = ''
         return text
 
 
-class CMUTokenizer(nn.Module):
-    def __init__(self, vocab=None):
+class BasicTokenizer(nn.Module):
+    """Tokenizer class to encode CMU phonemes.
+    Phonemes are separated by separators.
+    """
+
+    def __init__(self, language: Text) -> None:
         super().__init__()
-        if vocab is None:
+        if language == 'en':
             vocab = CMU_VOCAB
+            separator = '/'
+        elif language == 'ja':
+            vocab = JA_VOCAB
+            separator = ' '
+        else:
+            raise ValueError()
         self.vocab_size = len(vocab)
+        self._separator = separator
         self._vocab = vocab
         self._v2i = {x: i for i, x in enumerate(vocab)}
 
     def forward(self, text: Text) -> torch.Tensor:
         return self.encode(text)
 
     def encode(self, text: Text) -> torch.Tensor:
-        encoded = [self._v2i[ch] for ch in text.split('/') if ch in self._v2i]
+        encoded = [self._v2i[ch] for ch in text.split(self._separator) if ch in self._v2i]
         return torch.tensor(encoded, dtype=torch.long)
 
     def decode(self, encoded: torch.Tensor) -> Text:
-        return '/'.join([
+        return self._separator.join([
             self._vocab[x]
             for x in encoded
             if 0 <= x < len(self._vocab)])
 
     def merge_repeated(self, text: Text) -> Text:
-        raise NotImplementedError()
+        text = text.replace(self._separator, '\n')
+        text = text.replace(self._vocab[0], '\t')
+        text = re.sub(REPEATED_TOKENS_RX, r'\n\1', '\n' + text + '\n')
+        text = re.sub(REPEATED_BLANKS_RX, '', text)
+        return text.strip('\n').replace('\n', self._separator)
```

### Comparing `voice100-1.3.2/voice100/train_align.py` & `voice100-1.6.0/voice100/train_asr.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
 from argparse import ArgumentParser
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks import ModelCheckpoint
+from pytorch_lightning.callbacks import LearningRateMonitor
 
-from .datasets import AudioTextDataModule
-from .models.align import AudioAlignCTC
+from .data_modules import AudioTextDataModule
+from .models.asr import AudioToTextCTC
 
 
 def cli_main():
     pl.seed_everything(1234)
 
     parser = ArgumentParser()
     parser = pl.Trainer.add_argparse_args(parser)
     parser = AudioTextDataModule.add_argparse_args(parser)
-    parser = AudioAlignCTC.add_model_specific_args(parser)
-    parser.set_defaults(batch_size=256, log_every_n_steps=10)
-    args = parser.parse_args()
-    data = AudioTextDataModule.from_argparse_args(
-        args,
+    parser = AudioToTextCTC.add_model_specific_args(parser)
+    parser.set_defaults(
+        batch_size=32,
+        dataset="librispeech",
+        max_epochs=100,
+        log_every_n_steps=10,
         vocoder="mel")
-    model = AudioAlignCTC.from_argparse_args(
+    args = parser.parse_args()
+    assert not args.use_align
+    assert args.vocoder == "mel"
+    data: AudioTextDataModule = AudioTextDataModule.from_argparse_args(args)
+    model = AudioToTextCTC.from_argparse_args(
         args,
         audio_size=data.audio_size,
         vocab_size=data.vocab_size)
-    checkpoint_callback = ModelCheckpoint(monitor='val_loss', save_last=True, every_n_epochs=10)
-    trainer = pl.Trainer.from_argparse_args(
+    checkpoint_callback = ModelCheckpoint(monitor='val_loss', save_last=True)
+    lr_monitor = LearningRateMonitor(logging_interval='epoch')
+    trainer: pl.Trainer = pl.Trainer.from_argparse_args(
         args,
-        callbacks=[checkpoint_callback])
+        callbacks=[lr_monitor, checkpoint_callback])
     trainer.fit(model, data)
 
 
 if __name__ == '__main__':
     cli_main()
```

### Comparing `voice100-1.3.2/voice100/train_asr.py` & `voice100-1.6.0/voice100/train_ttsaudio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
 from argparse import ArgumentParser
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks import ModelCheckpoint
-from pytorch_lightning.callbacks import LearningRateMonitor
 
-from .datasets import AudioTextDataModule
-from .models.asr import AudioToCharCTC
+from .models.tts import AlignTextToAudioModel
+from .data_modules import AudioTextDataModule
 
 
 def cli_main():
     pl.seed_everything(1234)
 
     parser = ArgumentParser()
     parser = pl.Trainer.add_argparse_args(parser)
     parser = AudioTextDataModule.add_argparse_args(parser)
-    parser = AudioToCharCTC.add_model_specific_args(parser)
-    parser.set_defaults(
-        batch_size=32,
-        dataset="librispeech",
-        max_epochs=100,
-        log_every_n_steps=10)
+    parser = AlignTextToAudioModel.add_model_specific_args(parser)
+    parser.set_defaults(batch_size=32, vocoder="world")
     args = parser.parse_args()
+    assert args.vocoder == "world" or args.vocoder == "world_mcep"
     data: AudioTextDataModule = AudioTextDataModule.from_argparse_args(
-        args,
-        vocoder="mel")
-    model = AudioToCharCTC.from_argparse_args(
-        args,
-        audio_size=data.audio_size,
-        vocab_size=data.vocab_size)
-
-    checkpoint_callback = ModelCheckpoint(monitor='val_loss', save_last=True)
-    lr_monitor = LearningRateMonitor(logging_interval='epoch')
+        args, use_target=False, use_align=True)
+    model = AlignTextToAudioModel.from_argparse_args(
+        args, vocab_size=data.vocab_size)
+    checkpoint_callback = ModelCheckpoint(monitor='val_loss', save_last=True, every_n_epochs=10)
     trainer: pl.Trainer = pl.Trainer.from_argparse_args(
         args,
-        callbacks=[lr_monitor, checkpoint_callback])
+        callbacks=[checkpoint_callback])
     trainer.fit(model, data)
 
 
 if __name__ == '__main__':
     cli_main()
```

### Comparing `voice100-1.3.2/voice100/train_ttsalign.py` & `voice100-1.6.0/voice100/train_ttsalign.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
 from argparse import ArgumentParser
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks import ModelCheckpoint
 
-from .datasets import AlignTextDataModule
+from .data_modules import AlignTextDataModule
 from .models.tts import TextToAlignTextModel
 
 
 def cli_main():
     pl.seed_everything(1234)
 
     parser = ArgumentParser()
```

### Comparing `voice100-1.3.2/voice100/train_ttsaudio.py` & `voice100-1.6.0/voice100/train_ttsaudio_mt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
 from argparse import ArgumentParser
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks import ModelCheckpoint
 
-from .models.tts import AlignTextToAudioModel
-from .datasets import AudioTextDataModule
+from .models.tts import AlignTextToAudioMultiTaskModel
+from .data_modules import AudioTextDataModule
 
 
 def cli_main():
     pl.seed_everything(1234)
 
     parser = ArgumentParser()
     parser = pl.Trainer.add_argparse_args(parser)
     parser = AudioTextDataModule.add_argparse_args(parser)
-    parser = AlignTextToAudioModel.add_model_specific_args(parser)
+    parser = AlignTextToAudioMultiTaskModel.add_model_specific_args(parser)
+    parser.set_defaults(batch_size=32, vocoder="world")
     args = parser.parse_args()
+    assert args.vocoder == "world" or args.vocoder == "world_mcep"
+    assert not args.use_phone
     data: AudioTextDataModule = AudioTextDataModule.from_argparse_args(
-        args, vocoder="world", use_target=False, use_align=True)
-    model = AlignTextToAudioModel.from_argparse_args(
-        args, vocab_size=data.vocab_size)
+        args, vocoder="world", use_target=True, use_align=True)
+    model = AlignTextToAudioMultiTaskModel.from_argparse_args(
+        args, vocab_size=data.vocab_size, target_vocab_size=data.target_vocab_size)
     checkpoint_callback = ModelCheckpoint(monitor='val_loss', save_last=True, every_n_epochs=10)
     trainer: pl.Trainer = pl.Trainer.from_argparse_args(
         args,
         callbacks=[checkpoint_callback])
     trainer.fit(model, data)
```

### Comparing `voice100-1.3.2/voice100/update_samples.py` & `voice100-1.6.0/voice100/update_samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import numpy as np
 import soundfile as sf
 import torch
 from torch.nn.utils.rnn import pad_sequence
 from voice100.models.tts import TextToAlignTextModel
 from voice100.models.tts import AlignTextToAudioModel
 from voice100.models.tts import AlignTextToAudioMultiTaskModel
-from voice100.datasets import get_phonemizer, get_tokenizer
-from voice100.datasets import get_audio_transform
+from voice100.data_modules import get_phonemizer, get_tokenizer
+from voice100.data_modules import get_audio_transform
 
 
 def make_samples(
     align_model: Text,
     audio_model: Text,
     sample_texts: List[Text],
     language: Text,
```

### Comparing `voice100-1.3.2/voice100/vocoder.py` & `voice100-1.6.0/voice100/vocoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class WORLDVocoder(nn.Module):
 
     def __init__(
         self,
         sample_rate: int = 16000,
         frame_period: int = 10.0,
         n_fft: int = None,
-        use_mc: bool = False,
+        use_mcep: bool = False,
         log_offset: float = 1e-15
     ) -> None:
         super().__init__()
         self.sample_rate = sample_rate
         self.frame_period = frame_period
         self.n_fft = n_fft
         if sample_rate == 16000:
@@ -35,23 +35,30 @@
             self.mcep_dim = 34
             self.mcep_alpha = 0.455
             self.codeap_dim = 2
             if self.n_fft is None:
                 self.n_fft = 1024
         else:
             raise ValueError("Unsupported sample rate")
-        self.use_mc = use_mc
-        if use_mc:
+        self.use_mcep = use_mcep
+        if use_mcep:
             self.sp2mc_matrix = create_sp2mc_matrix(self.n_fft, self.mcep_dim, alpha=self.mcep_alpha)
             self.mc2sp_matrix = create_mc2sp_matrix(self.n_fft, self.mcep_dim, alpha=self.mcep_alpha)
         else:
             self.sp2mc_matrix = None
             self.mc2sp_matrix = None
         self.log_offset = log_offset
 
+    @property
+    def output_dims(self) -> Tuple[int, int, int]:
+        if self.use_mcep:
+            return 1, self.mcep_dim + 1, self.codeap_dim
+        else:
+            return 1, self.n_fft // 2 + 1, self.codeap_dim
+
     def forward(self, waveform: torch.Tensor):
         return self.encode(waveform)
 
     def encode(
         self,
         waveform: torch.Tensor,
         f0_floor: float = 80.0, f0_ceil: float = 400.0
@@ -61,37 +68,37 @@
             waveform, self.sample_rate, f0_floor=f0_floor,
             f0_ceil=f0_ceil, frame_period=self.frame_period)
         spc = pyworld.cheaptrick(waveform, f0, time_axis, self.sample_rate, fft_size=self.n_fft)
         logspc = np.log(spc + self.log_offset)
         ap = pyworld.d4c(waveform, f0, time_axis, self.sample_rate, fft_size=self.n_fft)
         codeap = pyworld.code_aperiodicity(ap, self.sample_rate)
 
-        if self.use_mc:
-            mc = logspc @ self.sp2mc_matrix
+        if self.use_mcep:
+            mcep = logspc @ self.sp2mc_matrix
             return (
                 torch.from_numpy(f0.astype(np.float32)),
-                torch.from_numpy(mc.astype(np.float32)),
+                torch.from_numpy(mcep.astype(np.float32)),
                 torch.from_numpy(codeap.astype(np.float32))
             )
         else:
             return (
                 torch.from_numpy(f0.astype(np.float32)),
                 torch.from_numpy(logspc.astype(np.float32)),
                 torch.from_numpy(codeap.astype(np.float32))
             )
 
     def decode(
-        self, f0: torch.Tensor, logspc_or_mc: torch.Tensor, codeap: torch.Tensor
-    ) -> torch.Tensor:
+        self, f0: torch.Tensor, logspc_or_mcep: torch.Tensor, codeap: torch.Tensor
+    ) -> np.ndarray:
         f0 = f0.cpu().numpy().astype(np.double, order='C')
-        if self.use_mc:
-            mc = logspc_or_mc.cpu().numpy().astype(np.double)
-            logspc = mc @ self.mc2sp_matrix
+        if self.use_mcep:
+            mcep = logspc_or_mcep.cpu().numpy().astype(np.double)
+            logspc = mcep @ self.mc2sp_matrix
         else:
-            logspc = logspc_or_mc.cpu().numpy().astype(np.double)
+            logspc = logspc_or_mcep.cpu().numpy().astype(np.double)
         codeap = codeap.cpu().numpy().astype(np.double, order='C')
         spc = np.maximum(np.exp(logspc) - self.log_offset, 0).copy(order='C')
         ap = pyworld.decode_aperiodicity(codeap, self.sample_rate, self.n_fft)
         waveform = pyworld.synthesize(f0, spc, ap, self.sample_rate, frame_period=self.frame_period)
         return waveform
```

