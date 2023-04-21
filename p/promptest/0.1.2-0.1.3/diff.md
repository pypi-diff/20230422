# Comparing `tmp/promptest-0.1.2.tar.gz` & `tmp/promptest-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptest-0.1.2.tar", last modified: Thu Apr 20 21:08:37 2023, max compression
+gzip compressed data, was "promptest-0.1.3.tar", last modified: Fri Apr 21 22:52:43 2023, max compression
```

## Comparing `promptest-0.1.2.tar` & `promptest-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-20 21:08:37.161599 promptest-0.1.2/
--rw-r--r--   0 yenkel     (501) staff       (20)     1075 2023-04-20 18:44:34.000000 promptest-0.1.2/LICENSE
--rw-r--r--   0 yenkel     (501) staff       (20)      156 2023-04-20 21:08:37.161486 promptest-0.1.2/PKG-INFO
--rw-r--r--   0 yenkel     (501) staff       (20)     4494 2023-04-20 20:54:25.000000 promptest-0.1.2/README.md
-drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-20 21:08:37.160656 promptest-0.1.2/promptest/
--rw-r--r--   0 yenkel     (501) staff       (20)       32 2023-04-20 20:52:02.000000 promptest-0.1.2/promptest/__init__.py
--rw-r--r--   0 yenkel     (501) staff       (20)     2836 2023-04-20 21:06:38.000000 promptest-0.1.2/promptest/main.py
--rw-r--r--   0 yenkel     (501) staff       (20)     1835 2023-04-20 21:02:03.000000 promptest-0.1.2/promptest/tester.py
-drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-20 21:08:37.161336 promptest-0.1.2/promptest.egg-info/
--rw-r--r--   0 yenkel     (501) staff       (20)      156 2023-04-20 21:08:37.000000 promptest-0.1.2/promptest.egg-info/PKG-INFO
--rw-r--r--   0 yenkel     (501) staff       (20)      286 2023-04-20 21:08:37.000000 promptest-0.1.2/promptest.egg-info/SOURCES.txt
--rw-r--r--   0 yenkel     (501) staff       (20)        1 2023-04-20 21:08:37.000000 promptest-0.1.2/promptest.egg-info/dependency_links.txt
--rw-r--r--   0 yenkel     (501) staff       (20)       51 2023-04-20 21:08:37.000000 promptest-0.1.2/promptest.egg-info/entry_points.txt
--rw-r--r--   0 yenkel     (501) staff       (20)       17 2023-04-20 21:08:37.000000 promptest-0.1.2/promptest.egg-info/requires.txt
--rw-r--r--   0 yenkel     (501) staff       (20)       10 2023-04-20 21:08:37.000000 promptest-0.1.2/promptest.egg-info/top_level.txt
--rw-r--r--   0 yenkel     (501) staff       (20)       38 2023-04-20 21:08:37.161641 promptest-0.1.2/setup.cfg
--rw-r--r--   0 yenkel     (501) staff       (20)      306 2023-04-20 20:53:11.000000 promptest-0.1.2/setup.py
+drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-21 22:52:43.703542 promptest-0.1.3/
+-rw-r--r--   0 yenkel     (501) staff       (20)     1075 2023-04-20 18:44:34.000000 promptest-0.1.3/LICENSE
+-rw-r--r--   0 yenkel     (501) staff       (20)      156 2023-04-21 22:52:43.703426 promptest-0.1.3/PKG-INFO
+-rw-r--r--   0 yenkel     (501) staff       (20)     4688 2023-04-21 22:50:59.000000 promptest-0.1.3/README.md
+drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-21 22:52:43.702622 promptest-0.1.3/promptest/
+-rw-r--r--   0 yenkel     (501) staff       (20)       32 2023-04-20 21:23:20.000000 promptest-0.1.3/promptest/__init__.py
+-rw-r--r--   0 yenkel     (501) staff       (20)     2836 2023-04-20 21:23:43.000000 promptest-0.1.3/promptest/main.py
+-rw-r--r--   0 yenkel     (501) staff       (20)     3264 2023-04-21 22:41:16.000000 promptest-0.1.3/promptest/tester.py
+drwxr-xr-x   0 yenkel     (501) staff       (20)        0 2023-04-21 22:52:43.703284 promptest-0.1.3/promptest.egg-info/
+-rw-r--r--   0 yenkel     (501) staff       (20)      156 2023-04-21 22:52:43.000000 promptest-0.1.3/promptest.egg-info/PKG-INFO
+-rw-r--r--   0 yenkel     (501) staff       (20)      286 2023-04-21 22:52:43.000000 promptest-0.1.3/promptest.egg-info/SOURCES.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)        1 2023-04-21 22:52:43.000000 promptest-0.1.3/promptest.egg-info/dependency_links.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)       51 2023-04-21 22:52:43.000000 promptest-0.1.3/promptest.egg-info/entry_points.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)       17 2023-04-21 22:52:43.000000 promptest-0.1.3/promptest.egg-info/requires.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)       10 2023-04-21 22:52:43.000000 promptest-0.1.3/promptest.egg-info/top_level.txt
+-rw-r--r--   0 yenkel     (501) staff       (20)       38 2023-04-21 22:52:43.703577 promptest-0.1.3/setup.cfg
+-rw-r--r--   0 yenkel     (501) staff       (20)      306 2023-04-21 20:24:39.000000 promptest-0.1.3/setup.py
```

### Comparing `promptest-0.1.2/LICENSE` & `promptest-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `promptest-0.1.2/README.md` & `promptest-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # promptest
-`promptest` is a command-line tool for testing language models (LLMs) using a given template and inputs. It supports testing multiple LLM models and outputs detailed results for each model.
+`promptest` is a command-line tool to test prompts with language models (LLMs).
 
 ## Installation
 To install `promptest`, run the following command:
 ```bash
 pip install promptest
 ```
 
@@ -24,15 +24,17 @@
 For more information on the command line arguments that `promptest` supports, run:
 ```bash
 promptest --help
 ```
 
 
 ## Example
-Here is an example of how to use `promptest` to test an LLM model:
+Here are a few examples of how to use `promptest` to test LLM prompts.
+
+### Test output with exact match
 
 1. Create a YAML file `prompt.yaml` containing the template for your LLM:
     ```yaml
     template: |
         Provide the longest word in terms of characters in an input piece of text.
         Only provide the word, no other text.
         Provide the word exactly as written in the text, do not modify it, capitalize it, etc.
@@ -40,15 +42,15 @@
         The text is:
         {text}
     input_variables:
         - text
     output_key: longest_word
     ```
 
-2. Create a YAML file `inputs.yaml` containing the inputs for your tests:
+2. Create a YAML file `tests.yaml` containing the inputs for your tests:
     ```yaml
     model_names:
 	- text-davinci-003
     temperature: 0
     max_tokens: 30
     tests:
         - variables:
@@ -59,66 +61,87 @@
         - variables:
             text: "the longest word in this text is confusing"
         expected_output:
             type: "string"
             value: "confusing"
     ```
 
-3. Run the following command to test the prompt templates:
+### Test output with another prompt
+1. Create a `prompt.yml` file containing the template for your prompt:
+```yaml
+template: |
+    Generate a short story in the {genre} genre. It should be at most 150 words long.
+input_variables:
+    - genre
+output_key: story
+```
+
+2. Create a tests.yaml file containing the inputs for your tests and the conditions the output should meet:
+```yaml
+model_names: ['text-davinci-003']
+temperature: 0.9
+max_tokens: 500
+tests:
+  - variables:
+      genre: "sci-fi"
+    expected_output:
+      type: prompt
+      model: 'text-davinci-003'
+      value:
+        conditions:
+          - "contains at least one futuristic element"
+          - "story has a clear beginning, middle, and end"
+  - variables:
+      genre: "mystery"
+    expected_output:
+      type: prompt
+      model: 'text-davinci-003'
+      value:
+        conditions:
+          - "contains a mystery or puzzle to be solved"
+          - "story has a clear beginning, middle, and end"
+```
+
+In this example, the tests uses another prompt to check if the generated story contains specific genre elements and has a clear structure with a beginning, middle, and end.
+
+### Running the tests
+Run the following command to test the prompt templates:
 ```bash
 promptest --prompt prompt.yaml --tests tests.yaml
 ```
 
-This will output detailed results for each model, including the number of test cases passed and the pass ratio.
+### Output
+The tests output detailed results for each model, including the number of test cases passed and the pass ratio.
 
 When you run `promptest`, the tool will execute tests for each LLM model specified in the `tests.yaml` file. For each model, `promptest` will run the tests and output the results to the console. In addition to the console output, `promptest` will also create a file containing the detailed test results.
 
-The file will be named model_name_test_result.yml, where model_name is the name of the LLM model being tested (e.g., gpt, gpt2, etc.). The file will be written to a directory named prompt_test_results in the current working directory. The directory will be named with a timestamp and the name of the template file being used, in the following format:
+The file will be named model_name_test_result.yml, where model_name is the name of the LLM model being tested (e.g., text-davinci-002, text-ada-001, etc.). The file will be written to a directory named prompt_test_results in the current working directory. The directory will be named with a timestamp and the name of the template file being used, in the following format:
 ```
 prompt_test_results/YYYY_MM_DD_HH_MM_template_name/
 ```
 
 The YAML file will contain the following information:
 
-Yes, you're correct. I apologize for the mistake in my previous response. The output directory will include the date and time when the test was run, as well as the name of the template file being used. Here's an updated markdown block:
-
-When you run promptest, the tool will execute tests for each LLM model specified in the inputs.yaml file. For each model, promptest will run the tests and output the results to the console. In addition to the console output, promptest will also create a file containing the detailed test results.
-
-The file will be named model_name_test_result.yml, where model_name is the name of the LLM model being tested (e.g., gpt, gpt2, etc.). The file will be written to a directory named prompt_test_results in the current working directory. The directory will be named with a timestamp and the name of the template file being used.
-
-The YAML file will contain the following information:
-
 ```yaml
 max_tokens: 30
 model: text-davinci-003
-prompt_template: 'Provide the longest word in terms of characters in an input piece
-  of text.
-
+prompt_template: |
+  Provide the longest word in terms of characters in an input piece of text.
   Only provide the word, no other text.
-
-  Provide the word exactly as written in the text, do not modify it, capitalize it,
-  etc.
-
+  Provide the word exactly as written in the text, do not modify it, capitalize it, etc.
 
   The text is:
-
   {text}
-
-  '
 results:
 - comparison_result: true
-  inputs:
-    text: the longest word in this text is longest
+  inputs: {text: the longest word in this text is longest}
   output: longest
 - comparison_result: true
-  inputs:
-    text: the longest word in this text is confusing
+  inputs: {text: the longest word in this text is confusing}
   output: confusing
 temperature: 0
-totals:
-  passes: 2
-  total: 2
+totals: {passes: 2, total: 2}
 ```
 
 ## License
 
 `promptest` is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `promptest-0.1.2/promptest/main.py` & `promptest-0.1.3/promptest/main.py`

 * *Files identical despite different names*

