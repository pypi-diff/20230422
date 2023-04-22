# Comparing `tmp/frechet_audio_distance-0.0.4.tar.gz` & `tmp/frechet_audio_distance-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frechet_audio_distance-0.0.4.tar", last modified: Sun Dec 11 07:14:56 2022, max compression
+gzip compressed data, was "frechet_audio_distance-0.1.0.tar", last modified: Sat Apr 22 03:53:38 2023, max compression
```

## Comparing `frechet_audio_distance-0.0.4.tar` & `frechet_audio_distance-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2022-12-11 07:14:56.352365 frechet_audio_distance-0.0.4/
--rw-r--r--   0 haohao_tan   (501) staff       (20)     1087 2022-12-11 06:36:10.000000 frechet_audio_distance-0.0.4/LICENSE
--rw-r--r--   0 haohao_tan   (501) staff       (20)     2356 2022-12-11 07:14:56.352127 frechet_audio_distance-0.0.4/PKG-INFO
--rw-r--r--   0 haohao_tan   (501) staff       (20)      654 2022-12-11 06:36:10.000000 frechet_audio_distance-0.0.4/README.md
-drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2022-12-11 07:14:56.350051 frechet_audio_distance-0.0.4/frechet_audio_distance/
--rw-r--r--   0 haohao_tan   (501) staff       (20)       18 2022-12-11 06:36:10.000000 frechet_audio_distance-0.0.4/frechet_audio_distance/__init__.py
--rw-r--r--   0 haohao_tan   (501) staff       (20)     8120 2022-12-11 06:36:10.000000 frechet_audio_distance-0.0.4/frechet_audio_distance/fad.py
-drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2022-12-11 07:14:56.351777 frechet_audio_distance-0.0.4/frechet_audio_distance.egg-info/
--rw-r--r--   0 haohao_tan   (501) staff       (20)     2356 2022-12-11 07:14:56.000000 frechet_audio_distance-0.0.4/frechet_audio_distance.egg-info/PKG-INFO
--rw-r--r--   0 haohao_tan   (501) staff       (20)      326 2022-12-11 07:14:56.000000 frechet_audio_distance-0.0.4/frechet_audio_distance.egg-info/SOURCES.txt
--rw-r--r--   0 haohao_tan   (501) staff       (20)        1 2022-12-11 07:14:56.000000 frechet_audio_distance-0.0.4/frechet_audio_distance.egg-info/dependency_links.txt
--rw-r--r--   0 haohao_tan   (501) staff       (20)       41 2022-12-11 07:14:56.000000 frechet_audio_distance-0.0.4/frechet_audio_distance.egg-info/requires.txt
--rw-r--r--   0 haohao_tan   (501) staff       (20)       23 2022-12-11 07:14:56.000000 frechet_audio_distance-0.0.4/frechet_audio_distance.egg-info/top_level.txt
--rw-r--r--   0 haohao_tan   (501) staff       (20)      722 2022-12-11 07:14:34.000000 frechet_audio_distance-0.0.4/pyproject.toml
--rw-r--r--   0 haohao_tan   (501) staff       (20)       38 2022-12-11 07:14:56.352495 frechet_audio_distance-0.0.4/setup.cfg
+drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.157359 frechet_audio_distance-0.1.0/
+-rw-r--r--   0 haohao_tan   (501) staff       (20)     1087 2022-12-11 06:36:10.000000 frechet_audio_distance-0.1.0/LICENSE
+-rw-r--r--   0 haohao_tan   (501) staff       (20)     3756 2023-04-22 03:53:38.157114 frechet_audio_distance-0.1.0/PKG-INFO
+-rw-r--r--   0 haohao_tan   (501) staff       (20)     2085 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/README.md
+drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.153614 frechet_audio_distance-0.1.0/frechet_audio_distance/
+-rw-r--r--   0 haohao_tan   (501) staff       (20)       18 2023-04-16 14:03:24.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/__init__.py
+-rw-r--r--   0 haohao_tan   (501) staff       (20)     8809 2023-04-22 03:47:22.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/fad.py
+drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.156474 frechet_audio_distance-0.1.0/frechet_audio_distance/models/
+-rw-r--r--   0 haohao_tan   (501) staff       (20)        0 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/models/__init__.py
+-rw-r--r--   0 haohao_tan   (501) staff       (20)   121695 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/models/pann.py
+-rw-r--r--   0 haohao_tan   (501) staff       (20)     8452 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/frechet_audio_distance/models/pytorch_utils.py
+drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.155511 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/
+-rw-r--r--   0 haohao_tan   (501) staff       (20)     3756 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/PKG-INFO
+-rw-r--r--   0 haohao_tan   (501) staff       (20)      475 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/SOURCES.txt
+-rw-r--r--   0 haohao_tan   (501) staff       (20)        1 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/dependency_links.txt
+-rw-r--r--   0 haohao_tan   (501) staff       (20)       41 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/requires.txt
+-rw-r--r--   0 haohao_tan   (501) staff       (20)       23 2023-04-22 03:53:38.000000 frechet_audio_distance-0.1.0/frechet_audio_distance.egg-info/top_level.txt
+-rw-r--r--   0 haohao_tan   (501) staff       (20)      722 2023-04-22 03:52:13.000000 frechet_audio_distance-0.1.0/pyproject.toml
+-rw-r--r--   0 haohao_tan   (501) staff       (20)       38 2023-04-22 03:53:38.157438 frechet_audio_distance-0.1.0/setup.cfg
+drwxr-xr-x   0 haohao_tan   (501) staff       (20)        0 2023-04-22 03:53:38.156772 frechet_audio_distance-0.1.0/test/
+-rw-r--r--   0 haohao_tan   (501) staff       (20)     2352 2023-04-17 14:32:46.000000 frechet_audio_distance-0.1.0/test/test_examples.py
```

### Comparing `frechet_audio_distance-0.0.4/LICENSE` & `frechet_audio_distance-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frechet_audio_distance-0.0.4/frechet_audio_distance/fad.py` & `frechet_audio_distance-0.1.0/frechet_audio_distance/fad.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import torch
 from torch import nn
 from scipy import linalg
 from tqdm import tqdm
 import soundfile as sf
 import resampy
 from multiprocessing.dummy import Pool as ThreadPool
+from .models.pann import Cnn14_16k
 
 
 SAMPLE_RATE = 16000
 
 
 def load_audio_task(fname):
     wav_data, sr = sf.read(fname, dtype='int16')
@@ -27,69 +28,73 @@
     # Convert to mono
     if len(wav_data.shape) > 1:
         wav_data = np.mean(wav_data, axis=1)
 
     if sr != SAMPLE_RATE:
         wav_data = resampy.resample(wav_data, sr, SAMPLE_RATE)
 
-    return wav_data, SAMPLE_RATE
+    return wav_data
 
 
 class FrechetAudioDistance:
-    def __init__(self, use_pca=False, use_activation=False, verbose=False, audio_load_worker=8):
-        self.__get_model(use_pca=use_pca, use_activation=use_activation)
+    def __init__(self, model_name="vggish", use_pca=False, use_activation=False, verbose=False, audio_load_worker=8):
+        self.model_name = model_name
+        self.device = torch.device('cuda') if torch.cuda.is_available() else torch.device('cpu')
+        self.__get_model(model_name=model_name, use_pca=use_pca, use_activation=use_activation)
         self.verbose = verbose
         self.audio_load_worker = audio_load_worker
     
-    def __get_model(self, use_pca=False, use_activation=False):
+    def __get_model(self, model_name="vggish", use_pca=False, use_activation=False):
         """
         Params:
         -- x   : Either 
             (i) a string which is the directory of a set of audio files, or
             (ii) a np.ndarray of shape (num_samples, sample_length)
         """
-        self.model = torch.hub.load('harritaylor/torchvggish', 'vggish')
-        if not use_pca:
-            self.model.postprocess = False
-        if not use_activation:
-            self.model.embeddings = nn.Sequential(*list(self.model.embeddings.children())[:-1])
+        if model_name == "vggish":
+            # S. Hershey et al., "CNN Architectures for Large-Scale Audio Classification", ICASSP 2017
+            self.model = torch.hub.load('harritaylor/torchvggish', 'vggish')
+            if not use_pca:
+                self.model.postprocess = False
+            if not use_activation:
+                self.model.embeddings = nn.Sequential(*list(self.model.embeddings.children())[:-1])
+        
+        elif model_name == "pann":
+            # Kong et al., "PANNs: Large-Scale Pretrained Audio Neural Networks for Audio Pattern Recognition", IEEE/ACM Transactions on Audio, Speech, and Language Processing 28 (2020)
+            model_path = os.path.join(torch.hub.get_dir(), "Cnn14_16k_mAP%3D0.438.pth")
+            if not(os.path.exists(model_path)):
+                torch.hub.download_url_to_file('https://zenodo.org/record/3987831/files/Cnn14_16k_mAP%3D0.438.pth', torch.hub.get_dir())
+            self.model = Cnn14_16k(sample_rate=16000, window_size=512, hop_size=160, mel_bins=64, fmin=50, fmax=8000, classes_num=527)
+            checkpoint = torch.load(model_path, map_location=self.device)
+            self.model.load_state_dict(checkpoint['model'])
+
         self.model.eval()
     
-    def get_embeddings(self, x, sr=16000):
+    def get_embeddings(self, x, sr=SAMPLE_RATE):
         """
         Get embeddings using VGGish model.
         Params:
-        -- x    : Either 
-            (i) a string which is the directory of a set of audio files, or
-            (ii) a list of np.ndarray audio samples
+        -- x    : a list of np.ndarray audio samples
         -- sr   : Sampling rate, if x is a list of audio samples. Default value is 16000.
         """
         embd_lst = []
-        if isinstance(x, list):
-            try:
-                for audio, sr in tqdm(x, disable=(not self.verbose)):
+        try:
+            for audio in tqdm(x, disable=(not self.verbose)):
+                if self.model_name == "vggish":
                     embd = self.model.forward(audio, sr)
-                    if self.model.device == torch.device('cuda'):
-                        embd = embd.cpu()
-                    embd = embd.detach().numpy()
-                    embd_lst.append(embd)
-            except Exception as e:
-                print("[Frechet Audio Distance] get_embeddings throw an exception: {}".format(str(e)))
-        elif isinstance(x, str):
-            try:
-                for fname in tqdm(os.listdir(x), disable=(not self.verbose)):
-                    embd = self.model.forward(os.path.join(x, fname))
-                    if self.model.device == torch.device('cuda'):
-                        embd = embd.cpu()
-                    embd = embd.detach().numpy()
-                    embd_lst.append(embd)
-            except Exception as e:
-                print("[Frechet Audio Distance] get_embeddings throw an exception: {}".format(str(e)))
-        else:
-            raise AttributeError
+                elif self.model_name == "pann":
+                    with torch.no_grad():
+                        out = self.model(torch.tensor(audio).float().unsqueeze(0), None)
+                        embd = out['embedding'].data[0]
+                if self.device == torch.device('cuda'):
+                    embd = embd.cpu()
+                embd = embd.detach().numpy()
+                embd_lst.append(embd)
+        except Exception as e:
+            print("[Frechet Audio Distance] get_embeddings throw an exception: {}".format(str(e)))
         
         return np.concatenate(embd_lst, axis=0)
     
     def calculate_embd_statistics(self, embd_lst):
         if isinstance(embd_lst, list):
             embd_lst = np.array(embd_lst)
         mu = np.mean(embd_lst, axis=0)
```

### Comparing `frechet_audio_distance-0.0.4/pyproject.toml` & `frechet_audio_distance-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frechet_audio_distance"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
   { name="Hao Hao Tan", email="helloharry66@gmail.com" },
 ]
 description = "A lightweight library of Frechet Audio Distance calculation."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

