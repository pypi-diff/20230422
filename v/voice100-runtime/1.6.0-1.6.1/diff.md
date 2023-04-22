# Comparing `tmp/voice100_runtime-1.6.0.tar.gz` & `tmp/voice100_runtime-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voice100_runtime-1.6.0.tar", max compression
+gzip compressed data, was "voice100_runtime-1.6.1.tar", max compression
```

## Comparing `voice100_runtime-1.6.0.tar` & `voice100_runtime-1.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-02-04 10:48:47.702386 voice100_runtime-1.6.0/LICENSE
--rw-r--r--   0        0        0     1780 2023-02-04 10:48:47.670386 voice100_runtime-1.6.0/README.md
--rw-r--r--   0        0        0      764 2023-04-22 04:21:21.525617 voice100_runtime-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     4377 2023-04-19 13:41:08.899907 voice100_runtime-1.6.0/voice100_runtime/__init__.py
--rw-r--r--   0        0        0     2284 2023-04-19 13:41:08.903907 voice100_runtime-1.6.0/voice100_runtime/asr.py
--rw-r--r--   0        0        0     1060 2023-04-19 13:41:08.903907 voice100_runtime-1.6.0/voice100_runtime/audio.py
--rw-r--r--   0        0        0     4303 2023-04-19 13:41:08.903907 voice100_runtime-1.6.0/voice100_runtime/text.py
--rw-r--r--   0        0        0     4374 2023-04-19 13:41:08.903907 voice100_runtime-1.6.0/voice100_runtime/tts.py
--rw-r--r--   0        0        0     1046 2023-02-04 10:48:49.490391 voice100_runtime-1.6.0/voice100_runtime/vocoder.py
--rw-r--r--   0        0        0     2626 1970-01-01 00:00:00.000000 voice100_runtime-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-04 10:48:47.702386 voice100_runtime-1.6.1/LICENSE
+-rw-r--r--   0        0        0     1780 2023-02-04 10:48:47.670386 voice100_runtime-1.6.1/README.md
+-rw-r--r--   0        0        0      764 2023-04-22 06:07:39.635162 voice100_runtime-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4404 2023-04-22 05:10:29.076898 voice100_runtime-1.6.1/voice100_runtime/__init__.py
+-rw-r--r--   0        0        0     2360 2023-04-22 04:48:44.688442 voice100_runtime-1.6.1/voice100_runtime/asr.py
+-rw-r--r--   0        0        0     1060 2023-04-19 13:41:08.903907 voice100_runtime-1.6.1/voice100_runtime/audio.py
+-rw-r--r--   0        0        0     4341 2023-04-22 05:26:49.539897 voice100_runtime-1.6.1/voice100_runtime/text.py
+-rw-r--r--   0        0        0     4338 2023-04-22 05:12:36.821976 voice100_runtime-1.6.1/voice100_runtime/tts.py
+-rw-r--r--   0        0        0     1046 2023-02-04 10:48:49.490391 voice100_runtime-1.6.1/voice100_runtime/vocoder.py
+-rw-r--r--   0        0        0     2626 1970-01-01 00:00:00.000000 voice100_runtime-1.6.1/PKG-INFO
```

### Comparing `voice100_runtime-1.6.0/LICENSE` & `voice100_runtime-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voice100_runtime-1.6.0/README.md` & `voice100_runtime-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `voice100_runtime-1.6.0/pyproject.toml` & `voice100_runtime-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voice100-runtime"
-version = "1.6.0"
+version = "1.6.1"
 description = "Voice100 Runtime is a TTS/ASR sample app that uses ONNX Runtime, WORLD and Voice100 neural TTS/ASR models on Python. Inference of Voice100 is low cost as its models are tiny and only depend on CNN without recursion."
 authors = ["Katsuya Iida <katsuya.iida@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `voice100_runtime-1.6.0/voice100_runtime/__init__.py` & `voice100_runtime-1.6.1/voice100_runtime/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,70 +5,70 @@
 import sys
 
 CACHE_DIR = os.path.expanduser("~/.cache/voice100_runtime")
 
 MODEL_URLS = {
     "asr_en": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.1.1/asr_en_conv_base_ctc-20220126.onnx",
-        None
+        []
     ],
     "asr_en_phone": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.1.0/asr_en_phone_conv_base_ctc-20220115.onnx",
-        None
+        []
     ],
     "asr_ja": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v0.2/stt_ja_conv_base_ctc-20211127.onnx",
-        None
+        []
     ],
     "tts_en": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.3.0/ttsalign_en_conv_base-20220409.onnx",
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.0.1/ttsaudio_en_conv_base-20220107.onnx",
-        None
+        []
     ],
     "tts_en_phone": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.3.0/ttsalign_en_phone_conv_base-20220409.onnx",
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.1.0/ttsaudio_en_phone_conv_base-20220105.onnx",
-        "phone"
+        ["phone"]
     ],
     "tts_en_mt": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.3.0/ttsalign_en_conv_base-20220409.onnx",
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.2.0/ttsaudio_en_mt_conv_base-20220316.onnx",
-        "mt"
+        ["mt"]
     ],
     "tts_ja": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.3.0/ttsalign_ja_conv_base-20220411.onnx",
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.3.1/ttsaudio_ja_conv_base-20220416.onnx",
-        None
+        []
     ],
     "asr_en_v2": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/asr_en_base-20230319.onnx",
-        "v2"
+        ["v2"]
     ],
     "asr_en_phone_v2": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/asr_en_phone_base-20230314.onnx",
-        "phone_v2"
+        ["phone", "v2"]
     ],
     "asr_ja_phone_v2": [
-        "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/asr_en_phone_base-20230104.onnx",
-        "phone_v2"
+        "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/asr_ja_phone_base-20230104.onnx",
+        ["ja", "phone", "v2"]
     ],
     "tts_en_v2": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/align_en_base-20230401.onnx",
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/tts_en_base-20230407.onnx",
-        "v2"
+        ["v2"]
     ],
     "tts_en_phone_v2": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/align_en_phone_base-20230407.onnx",
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/tts_en_phone_base-20230401.onnx",
-        "phone_v2"
+        ["phone", "v2"]
     ],
     "tts_ja_phone_v2": [
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/align_ja_phone_base-20230203.onnx",
         "https://github.com/kaiidams/voice100-runtime/releases/download/v1.4.0/tts_ja_phone_base-20230204.onnx",
-        "ja_phone_v2"
+        ["ja", "phone", "v2"]
     ],
 }
 
 
 def download_model(url: Text) -> Text:
     if not os.path.exists(CACHE_DIR):
         os.makedirs(CACHE_DIR)
```

### Comparing `voice100_runtime-1.6.0/voice100_runtime/asr.py` & `voice100_runtime-1.6.1/voice100_runtime/asr.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,36 +2,39 @@
 
 from typing import Text
 import numpy as np
 import onnxruntime as ort
 
 from .text import (
     CharTokenizer,
-    CMUTokenizer)
+    BasicTokenizer)
 from .audio import MelSpectrogram
 
 
 class ASR:
     def __init__(
         self, model_path: str,
         model_type: Text = None
     ) -> None:
         self.sample_rate = 16000
         self._model_type = model_type
-        if self._model_type == "phone" or self._model_type == "phone_v2":
-            self._tokenizer = CMUTokenizer()
+        if "phone" in self._model_type:
+            if "ja" in self._model_type:
+                self._tokenizer = BasicTokenizer(language="ja")
+            else:
+                self._tokenizer = BasicTokenizer(language="en")
         else:
             self._tokenizer = CharTokenizer()
         self._transform = MelSpectrogram()
         self._asr_sess = ort.InferenceSession(model_path)
 
     def __call__(
         self, waveform: np.ndarray, sample_rate: int, aligned: bool = True
     ) -> np.ndarray:
-        if self._model_type == "v2" or self._model_type == "phone_v2":
+        if "v2" in self._model_type:
             return self._v2(waveform, sample_rate, aligned)
         else:
             return self._v1(waveform, sample_rate, aligned)
 
     def _v1(
         self, waveform: np.ndarray, sample_rate: int, aligned: bool = True
     ) -> np.ndarray:
```

### Comparing `voice100_runtime-1.6.0/voice100_runtime/audio.py` & `voice100_runtime-1.6.1/voice100_runtime/audio.py`

 * *Files identical despite different names*

### Comparing `voice100_runtime-1.6.0/voice100_runtime/text.py` & `voice100_runtime-1.6.1/voice100_runtime/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from typing import Text
 import re
 import numpy as np
 
 __all__ = [
     "BasicPhonemizer",
+    "BasicTokenizer",
     "CharTokenizer",
     "CMUPhonemizer",
-    "CMUTokenizer",
 ]
 
 DEFAULT_CHARACTERS = "_ abcdefghijklmnopqrstuvwxyz'"
 NOT_DEFAULT_CHARACTERS_RX = re.compile("[^" + DEFAULT_CHARACTERS[1:] + "]")
 DEFAULT_VOCAB_SIZE = len(DEFAULT_CHARACTERS)
 assert DEFAULT_VOCAB_SIZE == 29
 
@@ -41,19 +41,20 @@
 assert len(JA_VOCAB) == 44
 
 REPEATED_TOKENS_RX = re.compile(r'\n([^\n]+)(\n\1)+(?=\n)')
 REPEATED_BLANKS_RX = re.compile(r'(\n\t)+(?=\n)')
 
 
 def make_aligntext(text, align, head=5, tail=5) -> np.ndarray:
-    aligntext_len = head + int(np.sum(align)) + tail
+    aligntext_len = head + int(np.sum(align) - align[0, 0]) + tail
     aligntext = np.zeros(aligntext_len, dtype=text.dtype)
     t = head
     for i in range(align.shape[0]):
-        t += align[i, 0].item()
+        if i > 0:
+            t += align[i, 0].item()
         s = round(t)
         t += align[i, 1].item()
         e = round(t)
         if s == e:
             s = max(0, s - 1)
         for j in range(s, e):
             aligntext[j] = text[i]
```

### Comparing `voice100_runtime-1.6.0/voice100_runtime/tts.py` & `voice100_runtime-1.6.1/voice100_runtime/tts.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,35 +14,36 @@
 class TTS:
     def __init__(
         self, align_model_path: Text, audio_model_path: Text,
         model_type: Text = None
     ):
         self.sample_rate = 16000
         self._model_type = model_type
-        if self._model_type == "mt":
+        if "mt" in self._model_type:
             self._phonemizer = BasicPhonemizer()
             self._tokenizer = CharTokenizer()
             self._output_tokenizer = BasicTokenizer(language="en")
-        elif self._model_type in "phone" or self._model_type == "phone_v2":
-            self._phonemizer = CMUPhonemizer()
-            self._tokenizer = BasicTokenizer(language="en")
-        elif self._model_type in "ja_phone_v2":
-            self._phonemizer = None
-            self._tokenizer = BasicTokenizer(language="ja")
+        elif "phone" in self._model_type:
+            if "ja" in self._model_type:
+                self._phonemizer = None
+                self._tokenizer = BasicTokenizer(language="ja")
+            else:
+                self._phonemizer = CMUPhonemizer()
+                self._tokenizer = BasicTokenizer(language="en")
         else:
             self._phonemizer = BasicPhonemizer()
             self._tokenizer = CharTokenizer()
         self._vocoder = WORLDVocoder()
         self._align_sess = ort.InferenceSession(align_model_path)
         self._audio_sess = ort.InferenceSession(audio_model_path)
 
     def __call__(
         self, input_text: str, return_align: bool = False
     ) -> Union[Tuple[np.ndarray, int], Tuple[np.ndarray, int, Text]]:
-        if self._model_type in ['v2', "phone_v2", "ja_phone_v2"]:
+        if "v2" in self._model_type:
             return self._v2(input_text, return_align)
         else:
             return self._v1(input_text, return_align)
 
     def _v1(
         self, input_text: str, return_align: bool = False
     ) -> Union[Tuple[np.ndarray, int], Tuple[np.ndarray, int, Text]]:
@@ -51,15 +52,15 @@
         (align,) = self._align_sess.run(
             output_names=["align"], input_feed={"text": text[None, :]}
         )
         align = np.clip(align, a_min=0, a_max=None)
         align = np.exp(align) - 1
         align = align[0]
         aligntext = make_aligntext(text, align)
-        if self._model_type == "mt":
+        if "mt" in self._model_type:
             f0, logspc, codeap, logits = self._audio_sess.run(
                 output_names=["f0", "logspc", "codeap", "logits"],
                 input_feed={"aligntext": aligntext[None, :]},
             )
             waveform = self._vocoder.decode(f0[0], logspc[0], codeap[0])
             if return_align:
                 outputtext = np.argmax(logits, axis=1)
```

### Comparing `voice100_runtime-1.6.0/voice100_runtime/vocoder.py` & `voice100_runtime-1.6.1/voice100_runtime/vocoder.py`

 * *Files identical despite different names*

### Comparing `voice100_runtime-1.6.0/PKG-INFO` & `voice100_runtime-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voice100-runtime
-Version: 1.6.0
+Version: 1.6.1
 Summary: Voice100 Runtime is a TTS/ASR sample app that uses ONNX Runtime, WORLD and Voice100 neural TTS/ASR models on Python. Inference of Voice100 is low cost as its models are tiny and only depend on CNN without recursion.
 License: MIT
 Author: Katsuya Iida
 Author-email: katsuya.iida@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

