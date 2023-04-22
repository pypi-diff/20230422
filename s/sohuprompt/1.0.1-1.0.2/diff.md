# Comparing `tmp/sohuprompt-1.0.1.tar.gz` & `tmp/sohuprompt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sohuprompt-1.0.1.tar", last modified: Sat Apr 22 09:25:58 2023, max compression
+gzip compressed data, was "sohuprompt-1.0.2.tar", last modified: Sat Apr 22 12:44:16 2023, max compression
```

## Comparing `sohuprompt-1.0.1.tar` & `sohuprompt-1.0.2.tar`

### file list

```diff
@@ -1,84 +1,85 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:25:58.534090 sohuprompt-1.0.1/
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-22 09:25:58.534090 sohuprompt-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 09:25:58.534090 sohuprompt-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2023-04-22 09:25:14.000000 sohuprompt-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:25:58.527090 sohuprompt-1.0.1/sohuprompt/
--rw-r--r--   0 root         (0) root         (0)      366 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5195 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:25:58.529090 sohuprompt-1.0.1/sohuprompt/data_utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:25:58.530090 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/
--rw-r--r--   0 root         (0) root         (0)      304 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/closed_QA.py
--rw-r--r--   0 root         (0) root         (0)     2538 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/coreference.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/entity_typing.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/generation.py
--rw-r--r--   0 root         (0) root         (0)     3857 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/nli.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/paraphrase.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/processor.py
--rw-r--r--   0 root         (0) root         (0)    16857 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/reading_comprehensation.py
--rw-r--r--   0 root         (0) root         (0)     4168 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/relation.py
--rw-r--r--   0 root         (0) root         (0)    11478 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/sentiment.py
--rw-r--r--   0 root         (0) root         (0)     3604 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/summarization.py
--rw-r--r--   0 root         (0) root         (0)     5336 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/ZH/topic_classification.py
--rw-r--r--   0 root         (0) root         (0)     2884 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5039 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/conditional_generation_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5009 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/data_sampler.py
--rw-r--r--   0 root         (0) root         (0)    15671 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/fewglue_dataset.py
--rw-r--r--   0 root         (0) root         (0)    10269 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/huggingface_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5583 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/lama_dataset.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/nli_dataset.py
--rw-r--r--   0 root         (0) root         (0)    14301 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/relation_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)    16683 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/text_classification_dataset.py
--rw-r--r--   0 root         (0) root         (0)     6379 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/typing_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11734 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/data_utils/utils.py
--rw-r--r--   0 root         (0) root         (0)    15591 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/default_config.py
--rw-r--r--   0 root         (0) root         (0)     8986 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/lm_bff_trainer.py
--rw-r--r--   0 root         (0) root         (0)    33757 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/pipeline_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:25:58.531090 sohuprompt-1.0.1/sohuprompt/plms/
--rw-r--r--   0 root         (0) root         (0)     7763 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:25:58.531090 sohuprompt-1.0.1/sohuprompt/plms/glm/
--rw-r--r--   0 root         (0) root         (0)      199 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/glm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4119 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/glm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/glm/glm.py
--rw-r--r--   0 root         (0) root         (0)    56656 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/glm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    15054 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/glm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    17877 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/glm/tokenization_chatglm.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/lm.py
--rw-r--r--   0 root         (0) root         (0)     3820 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/mlm.py
--rw-r--r--   0 root         (0) root         (0)    17199 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/seq2seq.py
--rw-r--r--   0 root         (0) root         (0)     9699 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/plms/utils.py
--rw-r--r--   0 root         (0) root         (0)    27881 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompt_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:25:58.533090 sohuprompt-1.0.1/sohuprompt/prompts/
--rw-r--r--   0 root         (0) root         (0)     3846 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11510 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/automatic_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8002 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/generation_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8815 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/knowledgeable_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/manual_template.py
--rw-r--r--   0 root         (0) root         (0)     9645 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/manual_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     8620 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/mixed_template.py
--rw-r--r--   0 root         (0) root         (0)     8052 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/one2one_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)    12707 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/prefix_tuning_template.py
--rw-r--r--   0 root         (0) root         (0)    23406 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/prompt_generator.py
--rw-r--r--   0 root         (0) root         (0)    15008 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/prototypical_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     5266 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/ptr_prompts.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/ptuning_prompts.py
--rw-r--r--   0 root         (0) root         (0)     5057 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/soft_template.py
--rw-r--r--   0 root         (0) root         (0)     9069 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/prompts/soft_verbalizer.py
--rw-r--r--   0 root         (0) root         (0)     6948 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/protoverb_trainer.py
--rw-r--r--   0 root         (0) root         (0)    31323 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:25:58.534090 sohuprompt-1.0.1/sohuprompt/utils/
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3866 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/utils/calibrate.py
--rw-r--r--   0 root         (0) root         (0)    10852 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/utils/crossfit_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/utils/cuda.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/utils/logging.py
--rw-r--r--   0 root         (0) root         (0)     5906 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/utils/metrics.py
--rw-r--r--   0 root         (0) root         (0)      510 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/utils/reproduciblity.py
--rw-r--r--   0 root         (0) root         (0)     2592 2023-04-22 09:08:12.000000 sohuprompt-1.0.1/sohuprompt/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 09:25:58.528090 sohuprompt-1.0.1/sohuprompt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      218 2023-04-22 09:25:58.000000 sohuprompt-1.0.1/sohuprompt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2604 2023-04-22 09:25:58.000000 sohuprompt-1.0.1/sohuprompt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 09:25:58.000000 sohuprompt-1.0.1/sohuprompt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-22 09:25:58.000000 sohuprompt-1.0.1/sohuprompt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-22 09:25:58.000000 sohuprompt-1.0.1/sohuprompt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.270747 sohuprompt-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-04-22 12:44:16.270747 sohuprompt-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4942 2023-04-22 12:39:37.000000 sohuprompt-1.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-22 12:44:16.270747 sohuprompt-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      682 2023-04-22 12:41:22.000000 sohuprompt-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.263747 sohuprompt-1.0.2/sohuprompt/
+-rw-r--r--   0 root         (0) root         (0)      366 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5195 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.265747 sohuprompt-1.0.2/sohuprompt/data_utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.266747 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/closed_QA.py
+-rw-r--r--   0 root         (0) root         (0)     2538 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/coreference.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/entity_typing.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/generation.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/nli.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/paraphrase.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/processor.py
+-rw-r--r--   0 root         (0) root         (0)    16857 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/reading_comprehensation.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/relation.py
+-rw-r--r--   0 root         (0) root         (0)    11478 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/sentiment.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/summarization.py
+-rw-r--r--   0 root         (0) root         (0)     5336 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/ZH/topic_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2884 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5039 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/conditional_generation_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5009 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     7875 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/data_sampler.py
+-rw-r--r--   0 root         (0) root         (0)    15671 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/fewglue_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10269 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/huggingface_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/lama_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/nli_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14301 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/relation_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    16683 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/text_classification_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     6379 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/typing_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11734 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/data_utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15591 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/default_config.py
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/lm_bff_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    33757 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/pipeline_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.266747 sohuprompt-1.0.2/sohuprompt/plms/
+-rw-r--r--   0 root         (0) root         (0)     7763 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.267747 sohuprompt-1.0.2/sohuprompt/plms/glm/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4119 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/glm.py
+-rw-r--r--   0 root         (0) root         (0)    56656 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    15054 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    17877 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/glm/tokenization_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/lm.py
+-rw-r--r--   0 root         (0) root         (0)     3820 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/mlm.py
+-rw-r--r--   0 root         (0) root         (0)    17199 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/seq2seq.py
+-rw-r--r--   0 root         (0) root         (0)     9699 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/plms/utils.py
+-rw-r--r--   0 root         (0) root         (0)    27881 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompt_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.269747 sohuprompt-1.0.2/sohuprompt/prompts/
+-rw-r--r--   0 root         (0) root         (0)     3846 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/automatic_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8002 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/generation_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8815 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/knowledgeable_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/manual_template.py
+-rw-r--r--   0 root         (0) root         (0)     9645 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/manual_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     8620 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/mixed_template.py
+-rw-r--r--   0 root         (0) root         (0)     8052 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/one2one_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)    12707 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/prefix_tuning_template.py
+-rw-r--r--   0 root         (0) root         (0)    23406 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/prompt_generator.py
+-rw-r--r--   0 root         (0) root         (0)    15008 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/prototypical_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     5266 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/ptr_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/ptuning_prompts.py
+-rw-r--r--   0 root         (0) root         (0)     5057 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/soft_template.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/prompts/soft_verbalizer.py
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/protoverb_trainer.py
+-rw-r--r--   0 root         (0) root         (0)    31323 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.269747 sohuprompt-1.0.2/sohuprompt/utils/
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3866 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/calibrate.py
+-rw-r--r--   0 root         (0) root         (0)    10852 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/crossfit_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/cuda.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/logging.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      510 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/reproduciblity.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-04-22 09:08:12.000000 sohuprompt-1.0.2/sohuprompt/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 12:44:16.264747 sohuprompt-1.0.2/sohuprompt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-22 12:44:16.000000 sohuprompt-1.0.2/sohuprompt.egg-info/top_level.txt
```

### Comparing `sohuprompt-1.0.1/setup.py` & `sohuprompt-1.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(name='sohuprompt',
-        version='1.0.1',
+        version='1.0.2',
         packages=find_packages(),  # 查找包的路径
         # package_dir={'': 'src'},  # 包的root路径映射到的实际路径
         # include_package_data=False,
         # package_data={'data': []},
         description='A python lib for sohuprompt',
         # long_description='',
         author='senhaowang,chencheng',
         author_email='senhaowang@sohu-inc.com',
         # url='http://www.xxxxx.com/',  # homepage
         license='MIT',
-        install_requires=['transformers', 'torch', 'numpy', 'pandas', 'tqdm', 'sklearn'],
+        install_requires=['transformers', 'torch', 'numpy', 'pandas', 'tqdm', 'sklearn', 'jieba'],
         )
```

### Comparing `sohuprompt-1.0.1/sohuprompt/config.py` & `sohuprompt-1.0.2/sohuprompt/config.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/closed_QA.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/closed_QA.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/coreference.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/coreference.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/entity_typing.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/entity_typing.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/generation.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/generation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/nli.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/nli.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/paraphrase.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/paraphrase.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/reading_comprehensation.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/reading_comprehensation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/relation.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/relation.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/sentiment.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/sentiment.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/summarization.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/summarization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/ZH/topic_classification.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/ZH/topic_classification.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/__init__.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/conditional_generation_dataset.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/conditional_generation_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/data_processor.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/data_processor.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/data_sampler.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/data_sampler.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/fewglue_dataset.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/fewglue_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/huggingface_dataset.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/huggingface_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/lama_dataset.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/lama_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/nli_dataset.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/nli_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/relation_classification_dataset.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/relation_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/text_classification_dataset.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/typing_dataset.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/typing_dataset.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/data_utils/utils.py` & `sohuprompt-1.0.2/sohuprompt/data_utils/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/default_config.py` & `sohuprompt-1.0.2/sohuprompt/default_config.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/lm_bff_trainer.py` & `sohuprompt-1.0.2/sohuprompt/lm_bff_trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/pipeline_base.py` & `sohuprompt-1.0.2/sohuprompt/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/__init__.py` & `sohuprompt-1.0.2/sohuprompt/plms/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/glm/configuration_chatglm.py` & `sohuprompt-1.0.2/sohuprompt/plms/glm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/glm/glm.py` & `sohuprompt-1.0.2/sohuprompt/plms/glm/glm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/glm/modeling_chatglm.py` & `sohuprompt-1.0.2/sohuprompt/plms/glm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/glm/quantization.py` & `sohuprompt-1.0.2/sohuprompt/plms/glm/quantization.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/glm/tokenization_chatglm.py` & `sohuprompt-1.0.2/sohuprompt/plms/glm/tokenization_chatglm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/lm.py` & `sohuprompt-1.0.2/sohuprompt/plms/lm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/mlm.py` & `sohuprompt-1.0.2/sohuprompt/plms/mlm.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/seq2seq.py` & `sohuprompt-1.0.2/sohuprompt/plms/seq2seq.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/plms/utils.py` & `sohuprompt-1.0.2/sohuprompt/plms/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompt_base.py` & `sohuprompt-1.0.2/sohuprompt/prompt_base.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/__init__.py` & `sohuprompt-1.0.2/sohuprompt/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/automatic_verbalizer.py` & `sohuprompt-1.0.2/sohuprompt/prompts/automatic_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/generation_verbalizer.py` & `sohuprompt-1.0.2/sohuprompt/prompts/generation_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/knowledgeable_verbalizer.py` & `sohuprompt-1.0.2/sohuprompt/prompts/knowledgeable_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/manual_template.py` & `sohuprompt-1.0.2/sohuprompt/prompts/manual_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/manual_verbalizer.py` & `sohuprompt-1.0.2/sohuprompt/prompts/manual_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/mixed_template.py` & `sohuprompt-1.0.2/sohuprompt/prompts/mixed_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/one2one_verbalizer.py` & `sohuprompt-1.0.2/sohuprompt/prompts/one2one_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/prefix_tuning_template.py` & `sohuprompt-1.0.2/sohuprompt/prompts/prefix_tuning_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/prompt_generator.py` & `sohuprompt-1.0.2/sohuprompt/prompts/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/prototypical_verbalizer.py` & `sohuprompt-1.0.2/sohuprompt/prompts/prototypical_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/ptr_prompts.py` & `sohuprompt-1.0.2/sohuprompt/prompts/ptr_prompts.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/ptuning_prompts.py` & `sohuprompt-1.0.2/sohuprompt/prompts/ptuning_prompts.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/soft_template.py` & `sohuprompt-1.0.2/sohuprompt/prompts/soft_template.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/prompts/soft_verbalizer.py` & `sohuprompt-1.0.2/sohuprompt/prompts/soft_verbalizer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/protoverb_trainer.py` & `sohuprompt-1.0.2/sohuprompt/protoverb_trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/trainer.py` & `sohuprompt-1.0.2/sohuprompt/trainer.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/utils/calibrate.py` & `sohuprompt-1.0.2/sohuprompt/utils/calibrate.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/utils/crossfit_metrics.py` & `sohuprompt-1.0.2/sohuprompt/utils/crossfit_metrics.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/utils/cuda.py` & `sohuprompt-1.0.2/sohuprompt/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/utils/logging.py` & `sohuprompt-1.0.2/sohuprompt/utils/logging.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/utils/metrics.py` & `sohuprompt-1.0.2/sohuprompt/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt/utils/utils.py` & `sohuprompt-1.0.2/sohuprompt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sohuprompt-1.0.1/sohuprompt.egg-info/SOURCES.txt` & `sohuprompt-1.0.2/sohuprompt.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 sohuprompt/__init__.py
 sohuprompt/config.py
 sohuprompt/default_config.py
 sohuprompt/lm_bff_trainer.py
 sohuprompt/pipeline_base.py
 sohuprompt/prompt_base.py
```

