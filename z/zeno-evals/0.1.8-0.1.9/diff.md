# Comparing `tmp/zeno_evals-0.1.8.tar.gz` & `tmp/zeno_evals-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeno_evals-0.1.8.tar", max compression
+gzip compressed data, was "zeno_evals-0.1.9.tar", max compression
```

## Comparing `zeno_evals-0.1.8.tar` & `zeno_evals-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     1303 2023-04-18 18:06:34.832884 zeno_evals-0.1.8/README.md
--rw-r--r--   0        0        0      537 2023-04-21 13:07:11.143849 zeno_evals-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       84 2023-04-18 15:03:49.480326 zeno_evals-0.1.8/zeno_evals/__init__.py
--rw-r--r--   0        0        0       29 2023-04-18 15:06:35.651777 zeno_evals-0.1.8/zeno_evals/__main__.py
--rw-r--r--   0        0        0     6368 2023-04-21 13:06:44.157476 zeno_evals-0.1.8/zeno_evals/main.py
--rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 zeno_evals-0.1.8/setup.py
--rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 zeno_evals-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-15 21:16:29.862397 zeno_evals-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     1303 2023-04-18 18:06:34.832884 zeno_evals-0.1.9/README.md
+-rw-r--r--   0        0        0      537 2023-04-21 14:16:40.848721 zeno_evals-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-04-21 14:09:32.753706 zeno_evals-0.1.9/zeno_evals/__init__.py
+-rw-r--r--   0        0        0       29 2023-04-18 15:06:35.651777 zeno_evals-0.1.9/zeno_evals/__main__.py
+-rw-r--r--   0        0        0     7083 2023-04-21 14:11:26.929921 zeno_evals-0.1.9/zeno_evals/main.py
+-rw-r--r--   0        0        0     2132 1970-01-01 00:00:00.000000 zeno_evals-0.1.9/setup.py
+-rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 zeno_evals-0.1.9/PKG-INFO
```

### Comparing `zeno_evals-0.1.8/LICENSE.md` & `zeno_evals-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zeno_evals-0.1.8/README.md` & `zeno_evals-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `zeno_evals-0.1.8/pyproject.toml` & `zeno_evals-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeno-evals"
-version = "0.1.8"
+version = "0.1.9"
 description = "Visualize OpenAI evals with Zeno"
 authors = ["Alex Cabrera <alex.cabrera@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "zeno_evals" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<=3.11"
```

### Comparing `zeno_evals-0.1.8/zeno_evals/main.py` & `zeno_evals-0.1.9/zeno_evals/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,116 @@
 import json
 import os
 import sys
 from contextlib import contextmanager
 from importlib import util
 from inspect import getmembers, isfunction
+from typing import Dict
 
 import fire
 import pandas as pd
+from pandas import DataFrame
 from zeno import (
     DistillReturn,
     ModelReturn,
     ZenoParameters,
     distill,
     metric,
     model,
     zeno,
 )
 from zeno.api import MetricReturn, ZenoOptions
 
-dfs = {}
+
+class ZenoEvals:
+    def __init__(
+        self,
+        results_file: str,
+        second_results_file: str = None,
+        functions_file: str = None,
+    ):
+        self.dfs = {}
+        self.results_file = results_file
+        self.second_results_file = second_results_file
+        self.functions_file = functions_file
+
+    def generate_zeno_config(self) -> ZenoParameters:
+        if not os.path.exists(self.results_file):
+            print("ERROR: file '{}' does not exist.".format(self.results_file))
+            sys.exit(1)
+
+        data = []
+        with open(self.results_file) as f:
+            for line in f:
+                data.append(json.loads(line))
+
+        df, metric_names = read_results_file(data)
+        self.dfs[get_model_name(data)] = df
+
+        models = [get_model_name(data)]
+        if self.second_results_file is not None:
+            data2 = []
+            with open(self.second_results_file) as f:
+                for line in f:
+                    data2.append(json.loads(line))
+
+            models.append(get_model_name(data2))
+            df2, _ = read_results_file(data2)
+            self.dfs[get_model_name(data2)] = df2
+
+        functions = [get_model_fn(self.dfs)]
+        if self.functions_file is not None:
+            functions = functions + parse_testing_file(self.functions_file)
+
+        base_df_columns = ["id", "prompt"]
+
+        for m in metric_names:
+            functions = functions + [get_metric_function(m)]
+
+        if "expected" in df.columns:
+            functions = functions + [get_correct_fn(self.dfs), avg_correct]
+            base_df_columns = base_df_columns + ["expected"]
+
+        zeno_config = ZenoParameters(
+            metadata=df[base_df_columns],
+            models=models,
+            functions=functions,
+            view="openai-chat",
+            data_column="prompt",
+            id_column="id",
+            cache_path="./.zeno_cache_" + data[0]["spec"]["eval_name"],
+            port=8080,
+            batch_size=100,
+            samples=5,
+        )
+
+        if "expected" in df.columns:
+            zeno_config.label_column = "expected"
+
+        return zeno_config
+
+
+def get_model_fn(dfs: Dict[str, DataFrame]):
+    def model_fn(name):
+        model_df = dfs[name]
+
+        def mod(df, ops: ZenoOptions):
+            return ModelReturn(model_output=model_df["sampled"].loc[df["id"]].tolist())
+
+        return mod
+
+    return model(model_fn)
+
+
+def get_correct_fn(dfs: Dict[str, DataFrame]):
+    def correct(df, ops: ZenoOptions):
+        mod = [mod for mod in list(dfs.keys()) if mod in ops.output_column][0]
+        return DistillReturn(distill_output=dfs[mod]["correct"].loc[df["id"]])
+
+    return distill(correct)
 
 
 @contextmanager
 def add_to_path(p):
     old_path = sys.path
     sys.path = sys.path[:]
     sys.path.insert(0, p)
@@ -67,31 +155,14 @@
         return MetricReturn(metric=df[metric_name].mean())
 
     metric_function.__name__ = metric_name
 
     return metric(metric_function)
 
 
-@model
-def model_fn(name):
-    model_df = dfs[name]
-
-    def mod(df, ops):
-        return ModelReturn(model_output=model_df["sampled"].loc[df["id"]].tolist())
-
-    return mod
-
-
-@distill
-def correct(df, ops: ZenoOptions):
-    model_name = [i for i in dfs.keys() if i in ops.output_column]
-    model_df = dfs[model_name[0]]
-    return DistillReturn(distill_output=model_df["correct"].loc[df["id"]])
-
-
 @metric
 def avg_correct(df, ops: ZenoOptions):
     return MetricReturn(
         metric=df[ops.distill_columns["correct"]].astype(int).mean() * 100
     )
 
 
@@ -147,72 +218,14 @@
 
 
 def get_model_name(data):
     name = data[0]["spec"]["completion_fns"][0]
     return name.replace(".", "_")
 
 
-def generate_zeno_config(
-    results_file: str, second_results_file: str = None, functions_file: str = None
-) -> ZenoParameters:
-    if not os.path.exists(results_file):
-        print("ERROR: file '{}' does not exist.".format(results_file))
-        sys.exit(1)
-
-    data = []
-    with open(results_file) as f:
-        for line in f:
-            data.append(json.loads(line))
-
-    df, metric_names = read_results_file(data)
-    dfs[get_model_name(data)] = df
-
-    models = [get_model_name(data)]
-    if second_results_file is not None:
-        data2 = []
-        with open(second_results_file) as f:
-            for line in f:
-                data2.append(json.loads(line))
-
-        models.append(get_model_name(data2))
-        df2, _ = read_results_file(data2)
-        dfs[get_model_name(data2)] = df2
-
-    functions = [model_fn]
-    if functions_file is not None:
-        functions = functions + parse_testing_file(functions_file)
-
-    base_df_columns = ["id", "prompt"]
-
-    for m in metric_names:
-        functions = functions + [get_metric_function(m)]
-
-    if "expected" in df.columns:
-        functions = functions + [correct, avg_correct]
-        base_df_columns = base_df_columns + ["expected"]
-
-    zeno_config = ZenoParameters(
-        metadata=df[base_df_columns],
-        models=models,
-        functions=functions,
-        view="openai-chat",
-        data_column="prompt",
-        id_column="id",
-        cache_path="./.zeno_cache_" + data[0]["spec"]["base_eval"],
-        port=8080,
-        batch_size=100,
-        samples=5,
-    )
-
-    if "expected" in df.columns:
-        zeno_config.label_column = "expected"
-
-    return zeno_config
-
-
 def main(
     results_file: str, second_results_file: str = None, functions_file: str = None
 ):
     """Visualize a result from OpenAI evals using Zeno.
 
     Args:
             results_file (path): Result .jsonl file from OpenAI evals.
@@ -221,13 +234,14 @@
             second_results_file (path): Second result .jsonl file from OpenAI
             evals for comparison. Often stored in the /tmp/evallogs/ directory.
 
             functions_file (path, optional): Path to a Python file containing
             additional Zeno processing functions. Defaults to None.
     """
 
-    config = generate_zeno_config(results_file, second_results_file, functions_file)
+    eval = ZenoEvals(results_file, second_results_file, functions_file)
+    config = eval.generate_zeno_config()
     zeno(config)
 
 
 def cli():
     fire.Fire(main)
```

### Comparing `zeno_evals-0.1.8/setup.py` & `zeno_evals-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['fire>=0.5.0,<0.6.0', 'pandas>=1.5.3,<2.0.0', 'zenoml>=0.4.10,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['zeno-evals = zeno_evals.main:cli']}
 
 setup_kwargs = {
     'name': 'zeno-evals',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Visualize OpenAI evals with Zeno',
     'long_description': '# Zeno 🤝 OpenAI Evals\n\nUse [Zeno](https://github.com/zeno-ml/zeno) to visualize the results of [OpenAI Evals](https://github.com/openai/evals/blob/main/docs/eval-templates.md).\n\nhttps://user-images.githubusercontent.com/4563691/225655166-9fd82784-cf35-47c1-8306-96178cdad7c1.mov\n\n_Example using `zeno-evals` to explore the results of an OpenAI eval on multiple choice medicine questions (MedMCQA)_\n\n### Usage\n\n```bash\npip install zeno-evals\n```\n\nRun an evaluation following the [evals instructions](https://github.com/openai/evals/blob/main/docs/run-evals.md). This will produce a cache file in `/tmp/evallogs/`.\n\nPass this file to the `zeno-evals` command:\n\n```bash\nzeno-evals /tmp/evallogs/my_eval_cache.jsonl\n```\n\n### Example\n\nSingle example looking at US tort law questions:\n\n```bash\nzeno-evals ./examples/example.jsonl\n```\n\nAnd an example of comparison between two models:\n\n```bash\nzeno-evals ./examples/crossword-turbo.jsonl --second-results-file ./examples/crossword-turbo-0301.jsonl\n```\n\nAnd lastly, we can pass additional [Zeno functions](https://zenoml.com/docs/api) to provide more context to the results:\n\n```bash\npip install wordfreq\nzeno-evals ./examples/crossword-turbo.jsonl --second-results-file ./examples/crossword-turbo-0301.jsonl --functions_file ./examples/crossword_fns.py\n```\n',
     'author': 'Alex Cabrera',
     'author_email': 'alex.cabrera@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `zeno_evals-0.1.8/PKG-INFO` & `zeno_evals-0.1.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno-evals
-Version: 0.1.8
+Version: 0.1.9
 Summary: Visualize OpenAI evals with Zeno
 Author: Alex Cabrera
 Author-email: alex.cabrera@gmail.com
 Requires-Python: >=3.9,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

