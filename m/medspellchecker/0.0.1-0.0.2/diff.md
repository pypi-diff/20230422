# Comparing `tmp/medspellchecker-0.0.1.tar.gz` & `tmp/medspellchecker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medspellchecker-0.0.1.tar", last modified: Fri Dec 16 23:07:58 2022, max compression
+gzip compressed data, was "medspellchecker-0.0.2.tar", last modified: Sat Apr 22 11:07:44 2023, max compression
```

## Comparing `medspellchecker-0.0.1.tar` & `medspellchecker-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2022-12-16 23:07:58.487130 medspellchecker-0.0.1/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    11357 2022-08-03 12:33:44.000000 medspellchecker-0.0.1/LICENSE
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     3882 2022-12-16 23:07:58.487130 medspellchecker-0.0.1/PKG-INFO
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2879 2022-08-03 12:33:44.000000 medspellchecker-0.0.1/README.md
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2022-12-16 23:07:58.483130 medspellchecker-0.0.1/medspellchecker/
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2022-12-16 23:07:58.487130 medspellchecker-0.0.1/medspellchecker/tool/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     8081 2022-12-16 21:23:05.000000 medspellchecker-0.0.1/medspellchecker/tool/abstract_bert_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2261 2022-12-16 21:23:05.000000 medspellchecker-0.0.1/medspellchecker/tool/abstract_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    14945 2022-12-16 21:23:05.000000 medspellchecker-0.0.1/medspellchecker/tool/candidate_generator.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      330 2022-12-14 21:21:48.000000 medspellchecker-0.0.1/medspellchecker/tool/candidate_word.py
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2022-12-16 23:07:58.487130 medspellchecker-0.0.1/medspellchecker/tool/data/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)  4603445 2022-08-03 12:33:45.000000 medspellchecker-0.0.1/medspellchecker/tool/data/processed_lemmatized_all_dict.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      581 2022-12-16 21:23:05.000000 medspellchecker-0.0.1/medspellchecker/tool/distilbert_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4393 2022-12-14 21:21:48.000000 medspellchecker-0.0.1/medspellchecker/tool/edit_distance.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2434 2022-12-14 21:21:48.000000 medspellchecker-0.0.1/medspellchecker/tool/gpu_utils.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     9585 2022-12-16 21:23:05.000000 medspellchecker-0.0.1/medspellchecker/tool/medspellchecker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      169 2022-12-14 21:21:48.000000 medspellchecker-0.0.1/medspellchecker/tool/mistake_type.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2067 2022-12-16 21:23:05.000000 medspellchecker-0.0.1/medspellchecker/tool/pre_post_processor.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      568 2022-12-16 21:23:05.000000 medspellchecker-0.0.1/medspellchecker/tool/roberta_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      569 2022-12-16 21:23:05.000000 medspellchecker-0.0.1/medspellchecker/tool/rubert_tiny2_candidate_ranker.py
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      618 2022-12-14 21:21:48.000000 medspellchecker-0.0.1/medspellchecker/tool/word.py
-drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2022-12-16 23:07:58.483130 medspellchecker-0.0.1/medspellchecker.egg-info/
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     3882 2022-12-16 23:07:58.000000 medspellchecker-0.0.1/medspellchecker.egg-info/PKG-INFO
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      844 2022-12-16 23:07:58.000000 medspellchecker-0.0.1/medspellchecker.egg-info/SOURCES.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        1 2022-12-16 23:07:58.000000 medspellchecker-0.0.1/medspellchecker.egg-info/dependency_links.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      173 2022-12-16 23:07:58.000000 medspellchecker-0.0.1/medspellchecker.egg-info/requires.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       16 2022-12-16 23:07:58.000000 medspellchecker-0.0.1/medspellchecker.egg-info/top_level.txt
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       38 2022-12-16 23:07:58.487130 medspellchecker-0.0.1/setup.cfg
--rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2035 2022-12-16 22:48:21.000000 medspellchecker-0.0.1/setup.py
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.716633 medspellchecker-0.0.2/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    11357 2022-08-03 12:33:44.000000 medspellchecker-0.0.2/LICENSE
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4011 2023-04-22 11:07:44.716633 medspellchecker-0.0.2/PKG-INFO
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     3028 2023-04-02 21:46:08.000000 medspellchecker-0.0.2/README.md
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.708633 medspellchecker-0.0.2/medspellchecker/
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.712633 medspellchecker-0.0.2/medspellchecker/tool/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     8720 2023-03-24 21:02:33.000000 medspellchecker-0.0.2/medspellchecker/tool/abstract_bert_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     3080 2023-03-24 21:02:33.000000 medspellchecker-0.0.2/medspellchecker/tool/abstract_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    14945 2022-12-16 21:23:05.000000 medspellchecker-0.0.2/medspellchecker/tool/candidate_generator.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      330 2022-12-14 21:21:48.000000 medspellchecker-0.0.2/medspellchecker/tool/candidate_word.py
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.712633 medspellchecker-0.0.2/medspellchecker/tool/data/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)  4603445 2022-08-03 12:33:45.000000 medspellchecker-0.0.2/medspellchecker/tool/data/processed_lemmatized_all_dict.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      581 2022-12-16 21:23:05.000000 medspellchecker-0.0.2/medspellchecker/tool/distilbert_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4393 2022-12-14 21:21:48.000000 medspellchecker-0.0.2/medspellchecker/tool/edit_distance.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2434 2022-12-14 21:21:48.000000 medspellchecker-0.0.2/medspellchecker/tool/gpu_utils.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)    13812 2023-04-10 20:03:39.000000 medspellchecker-0.0.2/medspellchecker/tool/medspellchecker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      169 2023-03-23 20:05:58.000000 medspellchecker-0.0.2/medspellchecker/tool/mistake_type.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4089 2023-04-10 18:03:51.000000 medspellchecker-0.0.2/medspellchecker/tool/pre_post_processor.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      568 2022-12-16 21:23:05.000000 medspellchecker-0.0.2/medspellchecker/tool/roberta_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      569 2022-12-16 23:37:30.000000 medspellchecker-0.0.2/medspellchecker/tool/rubert_tiny2_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      556 2023-03-17 18:40:55.000000 medspellchecker-0.0.2/medspellchecker/tool/rubioberta_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      563 2023-03-17 18:40:55.000000 medspellchecker-0.0.2/medspellchecker/tool/rubioroberta_candidate_ranker.py
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      938 2023-04-08 20:00:29.000000 medspellchecker-0.0.2/medspellchecker/tool/word.py
+drwxrwxr-x   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        0 2023-04-22 11:07:44.708633 medspellchecker-0.0.2/medspellchecker.egg-info/
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     4011 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/PKG-INFO
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      950 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/SOURCES.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)        1 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/dependency_links.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)      173 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/requires.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       16 2023-04-22 11:07:44.000000 medspellchecker-0.0.2/medspellchecker.egg-info/top_level.txt
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)       38 2023-04-22 11:07:44.716633 medspellchecker-0.0.2/setup.cfg
+-rw-rw-r--   0 dmitrypogrebnoy  (1000) dmitrypogrebnoy  (1000)     2036 2023-04-22 11:07:33.000000 medspellchecker-0.0.2/setup.py
```

### Comparing `medspellchecker-0.0.1/LICENSE` & `medspellchecker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.1/PKG-INFO` & `medspellchecker-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: medspellchecker
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fast and effective spellchecker for Russian medical texts
 Home-page: https://github.com/DmitryPogrebnoy/MedSpellChecker
 Author: Dmitry Pogrebnoy
 Author-email: pogrebnoy.inc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/DmitryPogrebnoy/MedSpellChecker/issues
 Project-URL: Funding, https://donate.pypi.org
 Keywords: spellchecker,nlp,medical,text correction
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Editors :: Word Processors
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,26 +31,32 @@
 Fast and effective tool for correcting spelling errors in Russian medical texts.
 The tool takes the raw medical text and returns the corrected text in lemmatized form.
 
 This project is under active development and is gradually improving.
 
 ## Demo
 
-Tool demo is not yet ready and will be added later.
+Here is an example of how to correct a spelling mistake with MedSpellChecker.
+
+![Demo](https://github.com/DmitryPogrebnoy/MedSpellChecker/blob/main/presentation_materials/readme/demo/demo_correct_message.gif)
+
+Steps for reproducing the demo:
+
+1. Clone the project
+2. Install all requirements
+3. Go to `demo` folder
+3. Run demo Flask server
+4. Open demo website and enjoy!
 
 ## Supported errors
 
 **MedSpellChecker** supports fixing the following types of errors.
 
 ![Supported errors](https://github.com/DmitryPogrebnoy/MedSpellChecker/blob/main/presentation_materials/figures/misspelling_types.drawio.png)
 
-For now, skip and extra space handling is in the prototype stage and may not work or
-may significantly affect performance.
-Other types of errors are handled stably well.
-
 ## Internals
 
 **MedSpellChecker** uses the SymDel algorithm to speed up the generation of correction candidates,
 and a fine-tuned BERT-based machine learning model to rank candidates and select the best fit.
 
 The architecture of the **MedSpellChecker** tool is shown below.
 
@@ -71,9 +76,7 @@
 
 ## More information
 
 This project is part of master's thesis. The current state is the result of the first year of work.
 More details about **MedSpellCHecker** you can find in the text of the
 [term report](https://github.com/DmitryPogrebnoy/MedSpellChecker/blob/main/presentation_materials/summer-report/Dmitry_Pogrebnoy_term_work.pdf)
 .
-
-
```

### Comparing `medspellchecker-0.0.1/README.md` & `medspellchecker-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,32 @@
 Fast and effective tool for correcting spelling errors in Russian medical texts.
 The tool takes the raw medical text and returns the corrected text in lemmatized form.
 
 This project is under active development and is gradually improving.
 
 ## Demo
 
-Tool demo is not yet ready and will be added later.
+Here is an example of how to correct a spelling mistake with MedSpellChecker.
+
+![Demo](https://github.com/DmitryPogrebnoy/MedSpellChecker/blob/main/presentation_materials/readme/demo/demo_correct_message.gif)
+
+Steps for reproducing the demo:
+
+1. Clone the project
+2. Install all requirements
+3. Go to `demo` folder
+3. Run demo Flask server
+4. Open demo website and enjoy!
 
 ## Supported errors
 
 **MedSpellChecker** supports fixing the following types of errors.
 
 ![Supported errors](https://github.com/DmitryPogrebnoy/MedSpellChecker/blob/main/presentation_materials/figures/misspelling_types.drawio.png)
 
-For now, skip and extra space handling is in the prototype stage and may not work or
-may significantly affect performance.
-Other types of errors are handled stably well.
-
 ## Internals
 
 **MedSpellChecker** uses the SymDel algorithm to speed up the generation of correction candidates,
 and a fine-tuned BERT-based machine learning model to rank candidates and select the best fit.
 
 The architecture of the **MedSpellChecker** tool is shown below.
```

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/abstract_bert_candidate_ranker.py` & `medspellchecker-0.0.2/medspellchecker/tool/abstract_bert_candidate_ranker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from abc import abstractmethod
+import dataclasses
 import itertools
 import logging
-from abc import abstractmethod
 from typing import List, Optional, Tuple
 
-import torch
 from accelerate import Accelerator
+import torch
 from torch import IntTensor
-from transformers import AutoTokenizer, AutoModelForMaskedLM, PreTrainedTokenizer, PreTrainedModel
+from transformers import AutoModelForMaskedLM, AutoTokenizer, PreTrainedModel, PreTrainedTokenizer
 
 from medspellchecker.tool.abstract_candidate_ranker import AbstractCandidateRanker
 from medspellchecker.tool.candidate_word import CandidateWord
 from medspellchecker.tool.gpu_utils import set_device
 from medspellchecker.tool.word import Word
 
 logger = logging.getLogger(__name__)
@@ -58,18 +59,16 @@
             patched_input_ids: IntTensor = IntTensor([list(itertools.chain.from_iterable(
                 [input_ids_before, candidate_ids_before,
                  [self._tokenizer.mask_token_id], candidate_ids_after, input_ids_after]))])
             patched_attention_mask: IntTensor = IntTensor([list(itertools.repeat(1, patched_input_ids.size()[1]))])
             results.append((patched_input_ids, patched_attention_mask))
         return results
 
-    def predict_score(self, current_word: Word,
-                      correct_words_before: List[Word],
-                      words_after: List[Word],
-                      candidate_value: str) -> Optional[float]:
+    def predict_score(self, correct_words_before: List[Word], words_after: List[Word], candidate_value: str) -> \
+            Optional[float]:
         text_with_mask = self.prepare_text_for_prediction(correct_words_before, words_after)
         candidate_token_ids = self._tokenizer.encode(candidate_value, add_special_tokens=False)
         logger.debug(f"Candidate token ids: {candidate_token_ids}")
 
         inputs = self._tokenizer(text_with_mask, return_tensors='pt')
         logger.debug(f"Input token ids: {inputs}")
 
@@ -102,41 +101,30 @@
         candidate_mean_score = candidate_mean_score / len(candidate_token_ids)
         logger.debug(f"Candidate - {candidate_value}, score {candidate_mean_score}")
         if self._use_treshold and candidate_mean_score > self._treshold or not self._use_treshold:
             return candidate_mean_score
         else:
             return None
 
-    def _process_candidates(self, current_word: Word,
-                            correct_words_before: List[Word],
-                            words_after: List[Word],
-                            candidate: CandidateWord) -> Optional[Tuple[CandidateWord, float]]:
-        candidate_score = self.predict_score(current_word, correct_words_before, words_after, candidate.value)
-        if candidate_score:
-            return candidate, candidate_score
-        else:
-            return None
-
     def rank_candidates(self, current_word: Word,
                         correct_words_before: List[Word],
                         words_after: List[Word],
                         candidates: List[CandidateWord]) -> List[CandidateWord]:
         if not candidates:
             return candidates
 
         # candidates must be ordered by edit distance
         candidates.sort(key=lambda x: x.distance)
 
         candidate_score_pairs = []
 
         for candidate in candidates:
-            processed_candidate_score = self._process_candidates(current_word, correct_words_before, words_after,
-                                                                 candidate)
-            if processed_candidate_score:
-                candidate_score_pairs.append(processed_candidate_score)
+            candidate_score = self.predict_score(correct_words_before, words_after, candidate.value)
+            if candidate_score:
+                candidate_score_pairs.append((candidate, candidate_score))
 
         ranked_candidate_score_pairs = sorted(candidate_score_pairs, key=lambda x: x[1])
         ranked_candidates = map(lambda x: x[0], ranked_candidate_score_pairs)
         return list(ranked_candidates)
 
     def pick_top_candidate(self, current_word: Word,
                            correct_words_before: List[Word],
@@ -145,24 +133,49 @@
         if not candidates:
             return None
 
         # candidates must be ordered by edit distance
         candidates.sort(key=lambda x: x.distance)
 
         candidate_score_pairs = []
-        previous_edit_distance_candidate = candidates[0].distance
+        candidates = list(filter(lambda x: x.distance == candidates[0].distance, candidates))
 
         for candidate in candidates:
-            if candidate.distance > previous_edit_distance_candidate:
-                break
+            candidate_score = self.predict_score(correct_words_before, words_after, candidate.value)
+            if candidate_score:
+                candidate_score_pairs.append((candidate, candidate_score))
+
+        if candidate_score_pairs:
+            ranked_candidate_score_pairs = sorted(candidate_score_pairs, key=lambda x: x[1])
+            return ranked_candidate_score_pairs[0]
+        else:
+            return None
+
+    def pick_top_candidate_with_next_word(self, current_word: Word,
+                                          next_word_str: str,
+                                          correct_words_before: List[Word],
+                                          words_after: List[Word],
+                                          candidates: List[CandidateWord]) -> Optional[Tuple[CandidateWord, float]]:
+        if not candidates:
+            return None
 
-            processed_candidate_score = self._process_candidates(current_word, correct_words_before, words_after,
-                                                                 candidate)
-            if processed_candidate_score:
-                candidate_score_pairs.append(processed_candidate_score)
-                previous_edit_distance_candidate = candidate.distance
+        # candidates must be ordered by edit distance
+        candidates.sort(key=lambda x: x.distance)
+
+        candidate_score_pairs = []
+        candidates = list(filter(lambda x: x.distance == candidates[0].distance, candidates))
+
+        for candidate in candidates:
+            candidate_score = self.predict_score(correct_words_before, words_after, candidate.value)
+            corrected_current_word = dataclasses.replace(current_word)
+            corrected_current_word.corrected_value = candidate.value
+            before = correct_words_before + [corrected_current_word]
+            after = words_after[1:]
+            next_word_score = self.predict_score(before, after, next_word_str)
+            if candidate_score and next_word_score:
+                candidate_score_pairs.append((candidate, (candidate_score + next_word_score) / 2))
 
         if candidate_score_pairs:
             ranked_candidate_score_pairs = sorted(candidate_score_pairs, key=lambda x: x[1])
             return ranked_candidate_score_pairs[0]
         else:
             return None
```

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/abstract_candidate_ranker.py` & `medspellchecker-0.0.2/medspellchecker/tool/abstract_candidate_ranker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-from abc import abstractmethod, ABC
+from abc import ABC, abstractmethod
 from typing import List, Optional, Tuple
 
 from medspellchecker.tool.candidate_word import CandidateWord
 from medspellchecker.tool.word import Word
 
 
 class AbstractCandidateRanker(ABC):
     @abstractmethod
-    def predict_score(self, current_word: Word,
-                      correct_words_before: List[Word],
-                      words_after: List[Word],
-                      candidate_value: str) -> Optional[float]:
+    def predict_score(self, correct_words_before: List[Word], words_after: List[Word], candidate_value: str) -> \
+    Optional[float]:
         """Returns score of candidate word
 
             Args:
                 current_word: current word
                 correct_words_before: corrected words before
                 words_after: words after (not corrected yet)
                 candidate_value: Value for computing score
@@ -52,7 +50,26 @@
                 correct_words_before: correct words before current word
                 words_after: not processed yet words after current word
                 candidates: Candidates for right word
 
             Returns:
                 Most suitable candidate and it's score
         """
+
+    @abstractmethod
+    def pick_top_candidate_with_next_word(self, current_word: Word,
+                                          next_word: Word,
+                                          correct_words_before: List[Word],
+                                          words_after: List[Word],
+                                          candidates: List[CandidateWord]) -> Optional[Tuple[CandidateWord, float]]:
+        """Returns most suitable candidate (with next word) for fixing incorrect words
+
+            Args:
+                current_word: The words that need correction
+                next_word: Next word
+                correct_words_before: correct words before current word
+                words_after: not processed yet words after current word
+                candidates: Candidates for right word
+
+            Returns:
+                Most suitable candidate and it's score
+        """
```

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/candidate_generator.py` & `medspellchecker-0.0.2/medspellchecker/tool/candidate_generator.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/data/processed_lemmatized_all_dict.txt` & `medspellchecker-0.0.2/medspellchecker/tool/data/processed_lemmatized_all_dict.txt`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/distilbert_candidate_ranker.py` & `medspellchecker-0.0.2/medspellchecker/tool/distilbert_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/edit_distance.py` & `medspellchecker-0.0.2/medspellchecker/tool/edit_distance.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/gpu_utils.py` & `medspellchecker-0.0.2/medspellchecker/tool/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/medspellchecker.py` & `medspellchecker-0.0.2/medspellchecker/tool/medspellchecker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import logging
 import os
 from pathlib import Path
-from typing import final, List, Optional, Union, IO, Set, Tuple, Dict
+from typing import Dict, final, IO, List, Optional, Set, Tuple, Union
+
 import numpy as np
 from pkg_resources import resource_filename
+from pymorphy2.tagset import OpencorporaTag
 
 from medspellchecker.tool.abstract_candidate_ranker import AbstractCandidateRanker
 from medspellchecker.tool.candidate_generator import CandidateGenerator
 from medspellchecker.tool.candidate_word import CandidateWord
 from medspellchecker.tool.edit_distance import EditDistanceAlgo
 from medspellchecker.tool.mistake_type import MistakeType
 from medspellchecker.tool.pre_post_processor import PreProcessor
@@ -53,25 +55,51 @@
         self._candidate_generator.save_state(path)
 
     def _pick_top_missing_space_candidate(self, word: Word,
                                           valid_words_before: List[Word],
                                           valid_words_after: List[Word]) -> Optional[Tuple[CandidateWord, float]]:
         candidate_words = []
         for i in range(len(word.original_value)):
-            first_word = self._pre_processor.lemmatize(word.original_value[:i])
-            second_part = self._pre_processor.lemmatize(word.original_value[i:])
-            if first_word in self.words and second_part in self.words:
-                candidate_word = f"{first_word} {second_part}"
-                score = self._candidate_ranker.predict_score(word, valid_words_before, valid_words_after,
-                                                             candidate_word)
-                if score:
-                    candidate_words.append((CandidateWord(candidate_word, 1), score))
+            first_part: Tuple[str, OpencorporaTag] = self._pre_processor.lemmatize_and_tag(word.original_value[:i])
+            second_part: Tuple[str, OpencorporaTag] = self._pre_processor.lemmatize_and_tag(word.original_value[i:])
+            if first_part[0] in self.words and second_part[0] in self.words:
+                candidate_word = f"{first_part[0]} {second_part[0]}"
+                first_word: Word = Word(word.position, first_part[0], True, corrected_value=first_part[0])
+                second_word: Word = Word(word.position, second_part[0], True, corrected_value=second_part[0])
+                first_score = self._candidate_ranker.predict_score(
+                    valid_words_before,
+                    [second_word] + valid_words_after,
+                    first_part[0]
+                )
+                second_score = self._candidate_ranker.predict_score(
+                    valid_words_before + [first_word],
+                    valid_words_after,
+                    second_part[0]
+                )
+                if first_score and second_score:
+                    candidate_words.append(
+                        (CandidateWord(candidate_word, 1),
+                         (first_score + second_score) / 2,
+                         first_part[1],
+                         second_part[1])
+                    )
         if candidate_words:
             candidate_words.sort(key=lambda x: x[1])
-            return candidate_words[0]
+            best_candidate_word_tuple = candidate_words[0]
+            best_candidate_word_split = best_candidate_word_tuple[0].value.split()
+            best_candidate_word_part_first: str = best_candidate_word_split[0]
+            best_candidate_word_part_second: str = best_candidate_word_split[1]
+
+            restored_first_part: str = self._pre_processor.str_restore_original_form(
+                best_candidate_word_part_first, best_candidate_word_tuple[2])
+            restored_second_part: str = self._pre_processor.str_restore_original_form(
+                best_candidate_word_part_second, best_candidate_word_tuple[3])
+
+            # return CandidateWord(f"{restored_first_part} {restored_second_part}", 1), best_candidate_word_tuple[1]
+            return best_candidate_word_tuple[0], best_candidate_word_tuple[1]
         else:
             return None
 
     # TODO: Do I need to save the formatting after fixing? -- no for now,
     #  usually formatting is not necessary for ml tasks
     def fix_text(self, text: str) -> str:
         # Remove newlines as the MosesTokenizer fails on newlines.
@@ -82,99 +110,147 @@
         # Build internal representation of words
         words: List[Word] = [word for word in self._pre_processor.generate_words_from_tokens(tokens)]
 
         current_word_idx = 0
         while current_word_idx < len(words):
             current_word = words[current_word_idx]
 
-            if not current_word.should_correct or current_word.original_value in self.words:
+            if (not current_word.should_correct) or (current_word.original_value in self.words) or \
+                    (current_word.lemma_normal_form in self.words):
                 current_word.corrected_value = current_word.original_value
                 current_word_idx += 1
                 continue
 
             valid_words_before: List[Word] = [word for word in words[:current_word_idx] if word.should_correct]
             valid_words_after: List[Word] = [word for word in words[current_word_idx + 1:] if word.should_correct]
 
-            # Consider non-spacing types of mistakes
-            # Generate list of candidates for fix
-            single_candidates_list: List[CandidateWord] = self._candidate_generator.generate_fixing_candidates(
-                current_word)
-            top_single_word_candidate_pair: Optional[Tuple[CandidateWord, float]] = \
-                self._candidate_ranker.pick_top_candidate(current_word, valid_words_before,
-                                                          valid_words_after, single_candidates_list)
+            mistake_type_to_candidate: Dict[MistakeType, Tuple[CandidateWord, float]] = {}
 
-            # If we shouldn't handle spacing mistakes then that's it
-            if not self._handle_compound_words:
-                if top_single_word_candidate_pair:
-                    current_word.corrected_value = top_single_word_candidate_pair[0].value
-                else:
-                    current_word.corrected_value = current_word.original_value
-                current_word_idx += 1
-                continue
+            # Compute score of original word
+            original_word_score: Optional[float] = self._candidate_ranker.predict_score(
+                valid_words_before, valid_words_after, current_word.get_lemma_normal_or_original_form())
 
-            # Else we need to process handle cases, but first of all create candidate dict
-            candidate_by_types: Dict[MistakeType, Tuple[CandidateWord, float]] = {}
-            if top_single_word_candidate_pair:
-                candidate_by_types[MistakeType.SINGLE_WORD_MISTAKE] = top_single_word_candidate_pair
-
-            # Consider missing space mistake
-            top_split_candidate_pair: Optional[Tuple[CandidateWord, float]] = \
-                self._pick_top_missing_space_candidate(current_word, valid_words_before, valid_words_after)
-            if top_split_candidate_pair:
-                candidate_by_types[MistakeType.MISSING_SPACE_MISTAKE] = top_split_candidate_pair
-
-            # Consider extra space mistake
-            new_word: Optional[Word] = None
-            if current_word_idx + 1 < len(words):
-                next_word: Word = words[current_word_idx + 1]
-                new_word_str: str = current_word.original_value + next_word.original_value
-                new_word: Word = next(self._pre_processor.generate_words_from_tokens([new_word_str]))
-                if new_word.should_correct and new_word.original_value in self.words:
-                    extra_space_candidate: CandidateWord = CandidateWord(new_word_str, 1)
-                    top_extra_space_candidate_pair: Optional[Tuple[CandidateWord, float]] = \
-                        self._candidate_ranker.pick_top_candidate(
-                            new_word, valid_words_before, valid_words_after[1:], [extra_space_candidate])
-                    if top_extra_space_candidate_pair:
-                        candidate_by_types[MistakeType.EXTRA_SPACE_MISTAKE] = top_extra_space_candidate_pair
+            if original_word_score is None:
+                original_word_score = 1.0
 
-            # Now we have collected all possible candidates. So let's pick most suitable one
-            candidate_by_types_list: List[Tuple[MistakeType, Tuple[CandidateWord, float]]] = \
-                list(candidate_by_types.items())
+            # If we shouldn't handle spacing mistakes then that's it
+            if self._handle_compound_words:
+                # Else we need to process handle cases
+                # Consider missing space mistake
+                if len(current_word.get_lemma_normal_or_original_form()) > 3:
+                    top_split_candidate_pair: Optional[Tuple[CandidateWord, float]] = \
+                        self._pick_top_missing_space_candidate(current_word, valid_words_before, valid_words_after)
+                    if top_split_candidate_pair:
+                        mistake_type_to_candidate[MistakeType.MISSING_SPACE_MISTAKE] = top_split_candidate_pair
+
+                # Consider extra space mistake
+                compound_word: Optional[Word] = self._create_compound_word(current_word_idx, current_word, words)
+                top_extra_space_candidate_pair: Optional[Tuple[CandidateWord, float]] = \
+                    self._get_top_extra_space_candidate(compound_word, valid_words_before, valid_words_after)
+                if top_extra_space_candidate_pair:
+                    mistake_type_to_candidate[MistakeType.EXTRA_SPACE_MISTAKE] = top_extra_space_candidate_pair
+            else:
+                compound_word = None
 
-            if not candidate_by_types_list:
-                current_word.corrected_value = current_word.original_value
+            # Consider non-spacing types of mistakes
+            # Generate list of candidates for fix
+            if len(current_word.get_lemma_normal_or_original_form()) > 3:
+                single_candidates_list: List[CandidateWord] = self._candidate_generator.generate_fixing_candidates(
+                    current_word, include_unknown=False)
+
+                if self._handle_compound_words and current_word_idx + 1 < len(words):
+                    top_single_word_candidate_pair: Optional[Tuple[CandidateWord, float]] = \
+                        self._candidate_ranker.pick_top_candidate_with_next_word(
+                            current_word,
+                            words[current_word_idx + 1].get_lemma_normal_or_original_form(),
+                            valid_words_before,
+                            valid_words_after,
+                            single_candidates_list
+                        )
+                else:
+                    top_single_word_candidate_pair: Optional[Tuple[CandidateWord, float]] = \
+                        self._candidate_ranker.pick_top_candidate(current_word, valid_words_before,
+                                                                  valid_words_after, single_candidates_list)
+                if top_single_word_candidate_pair:
+                    mistake_type_to_candidate[MistakeType.SINGLE_WORD_MISTAKE] = top_single_word_candidate_pair
+
+            # Early skip
+            if not mistake_type_to_candidate:
+                current_word.corrected_value = current_word.get_lemma_normal_or_original_form()
                 current_word_idx += 1
                 continue
 
-            min_distance_candidate = min(candidate_by_types_list, key=lambda x: x[1][0].distance)
-            filtered_candidate_by_types_list: List[Tuple[MistakeType, Tuple[CandidateWord, float]]] = \
-                list(filter(lambda x: x[1][0].distance == min_distance_candidate[1][0].distance,
-                            candidate_by_types_list))
-            candidate_scores: List[float] = list(map(lambda x: x[1][1], filtered_candidate_by_types_list))
-            top_candidate_idx: int = np.argmax(candidate_scores)
+            # Now we have collected all possible candidates. So let's pick most suitable one
             top_candidate: Tuple[MistakeType, Tuple[CandidateWord, float]] = \
-                filtered_candidate_by_types_list[top_candidate_idx]
+                self._find_top_candidate(mistake_type_to_candidate)
+            self._fix_word_by_top_candidate(
+                top_candidate,
+                original_word_score,
+                current_word,
+                current_word_idx,
+                words,
+                compound_word
+            )
+            current_word_idx += 1
+
+        corrected_text = self._build_result_text(words)
+        return corrected_text
 
-            top_candidate_type: MistakeType = top_candidate[0]
-            top_candidate_word: CandidateWord = top_candidate[1][0]
+    def _create_compound_word(self, current_word_idx: int, current_word: Word, words: List[Word]) -> Optional[Word]:
+        if current_word_idx + 1 < len(words):
+            next_word: Word = words[current_word_idx + 1]
+            new_word_str: str = current_word.original_value + next_word.original_value
+            new_word: Word = next(self._pre_processor.generate_words_from_tokens([new_word_str]))
+            return new_word
+        return None
+
+    def _get_top_extra_space_candidate(self, compound_word: Optional[Word],
+                                       valid_words_before: List[Word],
+                                       valid_words_after: List[Word]) -> Optional[Tuple[CandidateWord, float]]:
+        if compound_word and compound_word.should_correct and compound_word.get_lemma_normal_or_original_form() in self.words:
+            extra_space_candidate: CandidateWord = CandidateWord(compound_word.get_lemma_normal_or_original_form(), 1)
+            top_extra_space_candidate_pair: Optional[Tuple[CandidateWord, float]] = \
+                self._candidate_ranker.pick_top_candidate(
+                    compound_word, valid_words_before, valid_words_after[1:], [extra_space_candidate])
+            return top_extra_space_candidate_pair
+        return None
+
+    def _fix_word_by_top_candidate(self,
+                                   top_candidate: Tuple[MistakeType, Tuple[CandidateWord, float]],
+                                   original_word_score: float,
+                                   current_word: Word,
+                                   current_word_idx: int,
+                                   words: List[Word],
+                                   compound_word: Optional[Word]):
+        top_candidate_type: MistakeType = top_candidate[0]
+        top_candidate_word: CandidateWord = top_candidate[1][0]
+        top_candidate_score: float = top_candidate[1][1]
 
+        if original_word_score < top_candidate_score:
             if top_candidate_type == MistakeType.SINGLE_WORD_MISTAKE:
                 current_word.corrected_value = top_candidate_word.value
-                current_word_idx += 1
-                continue
-            elif top_candidate_type == MistakeType.MISSING_SPACE_MISTAKE:
-                # Here we didn't create two separate words due to the performance reasons
-                current_word.corrected_value = top_candidate_word.value
-                current_word_idx += 1
-                continue
-            elif top_candidate_type == MistakeType.EXTRA_SPACE_MISTAKE:
-                del words[current_word_idx + 1]
-                new_word.corrected_value = top_candidate_word.value
-                words[current_word_idx] = new_word
-                current_word_idx += 1
-                continue
-
-            current_word.corrected_value = current_word.original_value
-            current_word_idx += 1
-
-        corrected_text = ' '.join(map(lambda word: word.corrected_value, words))
-        return corrected_text
+                return
+            elif self._handle_compound_words:
+                if top_candidate_type == MistakeType.MISSING_SPACE_MISTAKE:
+                    # Here we didn't create two separate words due to the performance reasons
+                    current_word.corrected_value = top_candidate_word.value
+                    return
+                elif top_candidate_type == MistakeType.EXTRA_SPACE_MISTAKE:
+                    del words[current_word_idx + 1]
+                    compound_word.corrected_value = top_candidate_word.value
+                    words[current_word_idx] = compound_word
+                    return
+
+        current_word.corrected_value = current_word.get_lemma_normal_or_original_form()
+
+    def _find_top_candidate(self, mistake_type_to_candidate: Dict[MistakeType, Tuple[CandidateWord, float]]) \
+            -> Tuple[MistakeType, Tuple[CandidateWord, float]]:
+        mistake_type_candidate_list: List[Tuple[MistakeType, Tuple[CandidateWord, float]]] = \
+            list(mistake_type_to_candidate.items())
+
+        candidate_scores: List[float] = list(map(lambda x: x[1][1], mistake_type_candidate_list))
+        top_candidate_idx: int = np.argmax(candidate_scores)
+        return mistake_type_candidate_list[top_candidate_idx]
+
+    def _build_result_text(self, words: List[Word]) -> str:
+        result_list = [self._pre_processor.word_restore_original_form(word) for word in words]
+        return ' '.join(result_list)
```

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/roberta_candidate_ranker.py` & `medspellchecker-0.0.2/medspellchecker/tool/roberta_candidate_ranker.py`

 * *Files identical despite different names*

### Comparing `medspellchecker-0.0.1/medspellchecker/tool/rubert_tiny2_candidate_ranker.py` & `medspellchecker-0.0.2/medspellchecker/tool/rubert_tiny2_candidate_ranker.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from medspellchecker.tool.abstract_bert_candidate_ranker import AbstractBertCandidateRanker
 
 logger = logging.getLogger(__name__)
 
 
 @final
-class RuBertTyni2CandidateRanker(AbstractBertCandidateRanker):
+class RuBertTiny2CandidateRanker(AbstractBertCandidateRanker):
     _pretrained_model_checkpoint: str = "DmitryPogrebnoy/MedRuBertTiny2"
 
     def __init__(self, use_treshold: bool = True, use_gpu: bool = True):
-        super().__init__(RuBertTyni2CandidateRanker._pretrained_model_checkpoint, use_treshold, 0.0000001, use_gpu)
+        super().__init__(RuBertTiny2CandidateRanker._pretrained_model_checkpoint, use_treshold, 0.0000001, use_gpu)
 
     @property
     def _version(self) -> int:
         return 1
```

### Comparing `medspellchecker-0.0.1/medspellchecker.egg-info/PKG-INFO` & `medspellchecker-0.0.2/medspellchecker.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: medspellchecker
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fast and effective spellchecker for Russian medical texts
 Home-page: https://github.com/DmitryPogrebnoy/MedSpellChecker
 Author: Dmitry Pogrebnoy
 Author-email: pogrebnoy.inc@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/DmitryPogrebnoy/MedSpellChecker/issues
 Project-URL: Funding, https://donate.pypi.org
 Keywords: spellchecker,nlp,medical,text correction
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Editors :: Word Processors
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,26 +31,32 @@
 Fast and effective tool for correcting spelling errors in Russian medical texts.
 The tool takes the raw medical text and returns the corrected text in lemmatized form.
 
 This project is under active development and is gradually improving.
 
 ## Demo
 
-Tool demo is not yet ready and will be added later.
+Here is an example of how to correct a spelling mistake with MedSpellChecker.
+
+![Demo](https://github.com/DmitryPogrebnoy/MedSpellChecker/blob/main/presentation_materials/readme/demo/demo_correct_message.gif)
+
+Steps for reproducing the demo:
+
+1. Clone the project
+2. Install all requirements
+3. Go to `demo` folder
+3. Run demo Flask server
+4. Open demo website and enjoy!
 
 ## Supported errors
 
 **MedSpellChecker** supports fixing the following types of errors.
 
 ![Supported errors](https://github.com/DmitryPogrebnoy/MedSpellChecker/blob/main/presentation_materials/figures/misspelling_types.drawio.png)
 
-For now, skip and extra space handling is in the prototype stage and may not work or
-may significantly affect performance.
-Other types of errors are handled stably well.
-
 ## Internals
 
 **MedSpellChecker** uses the SymDel algorithm to speed up the generation of correction candidates,
 and a fine-tuned BERT-based machine learning model to rank candidates and select the best fit.
 
 The architecture of the **MedSpellChecker** tool is shown below.
 
@@ -71,9 +76,7 @@
 
 ## More information
 
 This project is part of master's thesis. The current state is the result of the first year of work.
 More details about **MedSpellCHecker** you can find in the text of the
 [term report](https://github.com/DmitryPogrebnoy/MedSpellChecker/blob/main/presentation_materials/summer-report/Dmitry_Pogrebnoy_term_work.pdf)
 .
-
-
```

### Comparing `medspellchecker-0.0.1/medspellchecker.egg-info/SOURCES.txt` & `medspellchecker-0.0.2/medspellchecker.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,9 +14,11 @@
 medspellchecker/tool/edit_distance.py
 medspellchecker/tool/gpu_utils.py
 medspellchecker/tool/medspellchecker.py
 medspellchecker/tool/mistake_type.py
 medspellchecker/tool/pre_post_processor.py
 medspellchecker/tool/roberta_candidate_ranker.py
 medspellchecker/tool/rubert_tiny2_candidate_ranker.py
+medspellchecker/tool/rubioberta_candidate_ranker.py
+medspellchecker/tool/rubioroberta_candidate_ranker.py
 medspellchecker/tool/word.py
 medspellchecker/tool/data/processed_lemmatized_all_dict.txt
```

### Comparing `medspellchecker-0.0.1/setup.py` & `medspellchecker-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from setuptools import setup, find_packages
 import pathlib
 
+from setuptools import setup, find_packages
+
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 print(find_packages(where='spellchecker'))
 
 setup(
     name='medspellchecker',
-    version='0.0.1',
+    version='0.0.2',
     description='Fast and effective spellchecker for Russian medical texts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DmitryPogrebnoy/MedSpellChecker',
     author='Dmitry Pogrebnoy',
     author_email='pogrebnoy.inc@gmail.com',
     license='Apache License 2.0',
@@ -41,13 +42,13 @@
                       'nltk>=3.6.7',
                       'editdistpy>=0.1.3',
                       'accelerate>=0.12.0',
                       'transformers>=4.22.2',
                       'sacremoses>=0.0.49',
                       'pynvml>=11.4.1'],
     include_package_data=True,
-    package_data={'medspellchecker.tool' : ['data/processed_lemmatized_all_dict.txt']},
+    package_data={'medspellchecker.tool': ['data/processed_lemmatized_all_dict.txt']},
     project_urls={
         'Bug Reports': 'https://github.com/DmitryPogrebnoy/MedSpellChecker/issues',
         'Funding': 'https://donate.pypi.org',
     },
-)
+)
```

