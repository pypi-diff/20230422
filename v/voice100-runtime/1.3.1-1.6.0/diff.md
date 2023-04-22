# Comparing `tmp/voice100-runtime-1.3.1.tar.gz` & `tmp/voice100_runtime-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voice100-runtime-1.3.1.tar", last modified: Thu Apr 21 23:47:51 2022, max compression
+gzip compressed data, was "voice100_runtime-1.6.0.tar", max compression
```

## Comparing `voice100-runtime-1.3.1.tar` & `voice100_runtime-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,10 @@
-drwxr-xr-x   0 kaiida    (1000) kaiida    (1000)        0 2022-04-21 23:47:51.083512 voice100-runtime-1.3.1/
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1069 2021-08-11 04:24:09.000000 voice100-runtime-1.3.1/LICENSE
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      501 2022-04-21 23:47:51.083512 voice100-runtime-1.3.1/PKG-INFO
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1780 2022-03-18 11:58:22.000000 voice100-runtime-1.3.1/README.md
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)       38 2022-04-21 23:47:51.083512 voice100-runtime-1.3.1/setup.cfg
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      723 2022-04-21 23:38:45.000000 voice100-runtime-1.3.1/setup.py
-drwxr-xr-x   0 kaiida    (1000) kaiida    (1000)        0 2022-04-21 23:47:51.073512 voice100-runtime-1.3.1/voice100_runtime/
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     2979 2022-04-21 23:39:06.000000 voice100-runtime-1.3.1/voice100_runtime/__init__.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      968 2022-01-18 12:31:54.000000 voice100-runtime-1.3.1/voice100_runtime/asr.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1058 2021-12-12 01:47:08.000000 voice100-runtime-1.3.1/voice100_runtime/audio.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     3609 2022-01-18 12:31:54.000000 voice100-runtime-1.3.1/voice100_runtime/text.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     2672 2022-03-18 11:48:59.000000 voice100-runtime-1.3.1/voice100_runtime/tts.py
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)     1046 2021-12-12 01:47:08.000000 voice100-runtime-1.3.1/voice100_runtime/vocoder.py
-drwxr-xr-x   0 kaiida    (1000) kaiida    (1000)        0 2022-04-21 23:47:51.083512 voice100-runtime-1.3.1/voice100_runtime.egg-info/
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      501 2022-04-21 23:47:50.000000 voice100-runtime-1.3.1/voice100_runtime.egg-info/PKG-INFO
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)      381 2022-04-21 23:47:50.000000 voice100-runtime-1.3.1/voice100_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)        1 2022-04-21 23:47:50.000000 voice100-runtime-1.3.1/voice100_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)       58 2022-04-21 23:47:50.000000 voice100-runtime-1.3.1/voice100_runtime.egg-info/requires.txt
--rw-r--r--   0 kaiida    (1000) kaiida    (1000)       17 2022-04-21 23:47:50.000000 voice100-runtime-1.3.1/voice100_runtime.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1069 2023-02-04 10:48:47.702386 voice100_runtime-1.6.0/LICENSE
+-rw-r--r--   0        0        0     1780 2023-02-04 10:48:47.670386 voice100_runtime-1.6.0/README.md
+-rw-r--r--   0        0        0      764 2023-04-22 04:21:21.525617 voice100_runtime-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4377 2023-04-19 13:41:08.899907 voice100_runtime-1.6.0/voice100_runtime/__init__.py
+-rw-r--r--   0        0        0     2284 2023-04-19 13:41:08.903907 voice100_runtime-1.6.0/voice100_runtime/asr.py
+-rw-r--r--   0        0        0     1060 2023-04-19 13:41:08.903907 voice100_runtime-1.6.0/voice100_runtime/audio.py
+-rw-r--r--   0        0        0     4303 2023-04-19 13:41:08.903907 voice100_runtime-1.6.0/voice100_runtime/text.py
+-rw-r--r--   0        0        0     4374 2023-04-19 13:41:08.903907 voice100_runtime-1.6.0/voice100_runtime/tts.py
+-rw-r--r--   0        0        0     1046 2023-02-04 10:48:49.490391 voice100_runtime-1.6.0/voice100_runtime/vocoder.py
+-rw-r--r--   0        0        0     2626 1970-01-01 00:00:00.000000 voice100_runtime-1.6.0/PKG-INFO
```

### Comparing `voice100-runtime-1.3.1/LICENSE` & `voice100_runtime-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voice100-runtime-1.3.1/README.md` & `voice100_runtime-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `voice100-runtime-1.3.1/voice100_runtime/audio.py` & `voice100_runtime-1.6.0/voice100_runtime/audio.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.hop_length = hop_length
         self.win_length = win_length
         self.n_mels = n_mels
         self.log_offset = log_offset
 
     def __call__(self, waveform: np.ndarray) -> np.ndarray:
         audio: np.ndarray = librosa.feature.melspectrogram(
-            waveform,
+            y=waveform,
             sr=self.sample_rate,
             n_fft=self.n_fft,
             hop_length=self.hop_length,
             win_length=self.win_length,
             center=True,
             pad_mode="reflect",
             power=2.0,
```

### Comparing `voice100-runtime-1.3.1/voice100_runtime/text.py` & `voice100_runtime-1.6.0/voice100_runtime/text.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,29 @@
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
 
 def make_aligntext(text, align, head=5, tail=5) -> np.ndarray:
     aligntext_len = head + int(np.sum(align)) + tail
     aligntext = np.zeros(aligntext_len, dtype=text.dtype)
     t = head
     for i in range(align.shape[0]):
         t += align[i, 0].item()
@@ -49,14 +64,51 @@
     def __init__(self):
         super().__init__()
 
     def __call__(self, text: Text) -> Text:
         return NOT_DEFAULT_CHARACTERS_RX.sub("", text.lower())
 
 
+class BasicTokenizer():
+    def __init__(self, language=None):
+        super().__init__()
+        if language == 'en':
+            vocab = CMU_VOCAB
+            separator = '/'
+        elif language == 'ja':
+            vocab = JA_VOCAB
+            separator = ' '
+        else:
+            raise ValueError()
+        self.vocab_size = len(vocab)
+        self._separator = separator
+        self._vocab = vocab
+        self._v2i = {x: i for i, x in enumerate(vocab)}
+
+    def __call__(self, text: Text) -> np.ndarray:
+        return self.encode(text)
+
+    def encode(self, text: Text) -> np.ndarray:
+        encoded = [self._v2i[ch] for ch in text.split(self._separator) if ch in self._v2i]
+        return np.array(encoded, dtype=np.int64)
+
+    def decode(self, encoded: np.ndarray) -> Text:
+        return self._separator.join([
+            self._vocab[x]
+            for x in encoded
+            if 0 <= x < len(self._vocab)])
+
+    def merge_repeated(self, text: Text) -> Text:
+        text = text.replace(self._separator, '\n')
+        text = text.replace(self._vocab[0], '\t')
+        text = re.sub(REPEATED_TOKENS_RX, r'\n\1', '\n' + text + '\n')
+        text = re.sub(REPEATED_BLANKS_RX, '', text)
+        return text.strip('\n').replace('\n', self._separator)
+
+
 class CharTokenizer:
     def __init__(self, vocab=None):
         super().__init__()
         if vocab is None:
             vocab = DEFAULT_CHARACTERS
         self.vocab_size = len(vocab)
         self._vocab = vocab
@@ -83,40 +135,7 @@
 class CMUPhonemizer():
     def __init__(self):
         from g2p_en import G2p
         self.g2p = G2p()
 
     def __call__(self, text: Text) -> Text:
         return "/".join(self.g2p(text))
-
-
-class CMUTokenizer():
-    def __init__(self, vocab=None):
-        super().__init__()
-        if vocab is None:
-            vocab = CMU_VOCAB
-        self.vocab_size = len(vocab)
-        self._vocab = vocab
-        self._v2i = {x: i for i, x in enumerate(vocab)}
-
-    def __call__(self, text: Text) -> np.ndarray:
-        return self.encode(text)
-
-    def encode(self, text: Text) -> np.ndarray:
-        encoded = [self._v2i[ch] for ch in text.split('/') if ch in self._v2i]
-        return np.array(encoded, dtype=np.int64)
-
-    def decode(self, encoded: np.ndarray) -> Text:
-        return '/'.join([
-            self._vocab[x]
-            for x in encoded
-            if 0 <= x < len(self._vocab)])
-
-    def merge_repeated(self, text: Text) -> Text:
-        tokens = []
-        prev_token = None
-        for token in text.split("/"):
-            if token != prev_token:
-                if token != "_":
-                    tokens.append(token)
-                prev_token = token
-        return "/".join(tokens)
```

### Comparing `voice100-runtime-1.3.1/voice100_runtime/tts.py` & `voice100_runtime-1.6.0/voice100_runtime/tts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 # Copyright (C) 2021 Katsuya Iida. All rights reserved.
 
-from typing import Text, Union
+from typing import Text, Union, Tuple
 import numpy as np
 import onnxruntime as ort
-from typing import Tuple
 
 from .text import (
     make_aligntext,
-    BasicPhonemizer, CharTokenizer,
-    CMUPhonemizer, CMUTokenizer)
+    BasicPhonemizer, BasicTokenizer, CharTokenizer,
+    CMUPhonemizer)
 from .vocoder import WORLDVocoder
 
 
 class TTS:
     def __init__(
         self, align_model_path: Text, audio_model_path: Text,
-        modeltype: Text = None
+        model_type: Text = None
     ):
         self.sample_rate = 16000
-        self._modeltype = modeltype
-        if self._modeltype == "mt":
+        self._model_type = model_type
+        if self._model_type == "mt":
             self._phonemizer = BasicPhonemizer()
             self._tokenizer = CharTokenizer()
-            self._output_tokenizer = CMUTokenizer()
-        elif self._modeltype == "phone":
+            self._output_tokenizer = BasicTokenizer(language="en")
+        elif self._model_type in "phone" or self._model_type == "phone_v2":
             self._phonemizer = CMUPhonemizer()
-            self._tokenizer = CMUTokenizer()
+            self._tokenizer = BasicTokenizer(language="en")
+        elif self._model_type in "ja_phone_v2":
+            self._phonemizer = None
+            self._tokenizer = BasicTokenizer(language="ja")
         else:
             self._phonemizer = BasicPhonemizer()
             self._tokenizer = CharTokenizer()
         self._vocoder = WORLDVocoder()
         self._align_sess = ort.InferenceSession(align_model_path)
         self._audio_sess = ort.InferenceSession(audio_model_path)
 
     def __call__(
         self, input_text: str, return_align: bool = False
     ) -> Union[Tuple[np.ndarray, int], Tuple[np.ndarray, int, Text]]:
+        if self._model_type in ['v2', "phone_v2", "ja_phone_v2"]:
+            return self._v2(input_text, return_align)
+        else:
+            return self._v1(input_text, return_align)
+
+    def _v1(
+        self, input_text: str, return_align: bool = False
+    ) -> Union[Tuple[np.ndarray, int], Tuple[np.ndarray, int, Text]]:
         text = self._phonemizer(input_text)
         text = self._tokenizer(text)
         (align,) = self._align_sess.run(
             output_names=["align"], input_feed={"text": text[None, :]}
         )
         align = np.clip(align, a_min=0, a_max=None)
         align = np.exp(align) - 1
         align = align[0]
         aligntext = make_aligntext(text, align)
-        if self._modeltype == "mt":
+        if self._model_type == "mt":
             f0, logspc, codeap, logits = self._audio_sess.run(
                 output_names=["f0", "logspc", "codeap", "logits"],
                 input_feed={"aligntext": aligntext[None, :]},
             )
             waveform = self._vocoder.decode(f0[0], logspc[0], codeap[0])
             if return_align:
                 outputtext = np.argmax(logits, axis=1)
@@ -62,7 +72,36 @@
                 input_feed={"aligntext": aligntext[None, :]},
             )
             waveform = self._vocoder.decode(f0[0], logspc[0], codeap[0])
             if return_align:
                 aligntext = self._tokenizer.decode(aligntext)
                 return waveform, self.sample_rate, aligntext
             return waveform, self.sample_rate
+
+    def _v2(
+        self, input_text: str, return_align: bool = False
+    ) -> Union[Tuple[np.ndarray, int], Tuple[np.ndarray, int, Text]]:
+        if self._phonemizer is not None:
+            text = self._phonemizer(input_text)
+        else:
+            text = input_text
+        text = self._tokenizer(text)
+        text_len = np.array([text.shape[0]], dtype=np.int64)
+        (align,) = self._align_sess.run(
+            output_names=["align"],
+            input_feed={"text": text[None, :], "text_len": text_len}
+        )
+        align = align[0]
+        aligntext = make_aligntext(text, align)
+        aligntext_len = np.array([aligntext.shape[0]], dtype=np.int64)
+        f0, logspc, codeap = self._audio_sess.run(
+            output_names=["f0", "logspc", "codeap"],
+            input_feed={
+                "aligntext": aligntext[None, :],
+                "aligntext_len": aligntext_len
+            },
+        )
+        waveform = self._vocoder.decode(f0[0], logspc[0], codeap[0])
+        if return_align:
+            aligntext = self._tokenizer.decode(aligntext)
+            return waveform, self.sample_rate, aligntext
+        return waveform, self.sample_rate
```

### Comparing `voice100-runtime-1.3.1/voice100_runtime/vocoder.py` & `voice100_runtime-1.6.0/voice100_runtime/vocoder.py`

 * *Files identical despite different names*

