# Comparing `tmp/dask4dvc-0.2.1.tar.gz` & `tmp/dask4dvc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask4dvc-0.2.1.tar", max compression
+gzip compressed data, was "dask4dvc-0.2.2.tar", max compression
```

## Comparing `dask4dvc-0.2.1.tar` & `dask4dvc-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.2.1/LICENSE
--rw-r--r--   0        0        0     1791 2023-04-21 11:17:08.062984 dask4dvc-0.2.1/README.md
--rw-r--r--   0        0        0      651 2023-04-19 15:02:16.124501 dask4dvc-0.2.1/dask4dvc/__init__.py
--rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.2.1/dask4dvc/cli/__init__.py
--rw-r--r--   0        0        0     2795 2023-04-21 11:17:08.062984 dask4dvc-0.2.1/dask4dvc/cli/main.py
--rw-r--r--   0        0        0     4265 2023-04-21 11:17:08.062984 dask4dvc-0.2.1/dask4dvc/methods.py
--rw-r--r--   0        0        0      142 2023-04-19 15:36:27.742838 dask4dvc-0.2.1/dask4dvc/utils/__init__.py
--rw-r--r--   0        0        0      272 2023-04-19 15:36:27.742838 dask4dvc-0.2.1/dask4dvc/utils/config.py
--rw-r--r--   0        0        0     1055 2023-04-13 11:02:16.867293 dask4dvc-0.2.1/dask4dvc/utils/dask.py
--rw-r--r--   0        0        0      136 2023-04-19 15:36:27.742838 dask4dvc-0.2.1/dask4dvc/utils/main.py
--rw-r--r--   0        0        0     1256 2023-04-21 11:17:08.072984 dask4dvc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 dask4dvc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2252 2023-04-22 14:35:15.965210 dask4dvc-0.2.2/README.md
+-rw-r--r--   0        0        0      656 2023-04-22 14:35:15.975209 dask4dvc-0.2.2/dask4dvc/__init__.py
+-rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.2.2/dask4dvc/cli/__init__.py
+-rw-r--r--   0        0        0     4437 2023-04-22 14:47:14.907460 dask4dvc-0.2.2/dask4dvc/cli/main.py
+-rw-r--r--   0        0        0     3547 2023-04-22 14:47:14.907460 dask4dvc-0.2.2/dask4dvc/dvc_queue.py
+-rw-r--r--   0        0        0     5655 2023-04-22 14:35:15.975209 dask4dvc-0.2.2/dask4dvc/dvc_repro.py
+-rw-r--r--   0        0        0      142 2023-04-19 15:36:27.742838 dask4dvc-0.2.2/dask4dvc/utils/__init__.py
+-rw-r--r--   0        0        0      272 2023-04-22 10:39:57.388361 dask4dvc-0.2.2/dask4dvc/utils/config.py
+-rw-r--r--   0        0        0     1184 2023-04-22 14:35:15.975209 dask4dvc-0.2.2/dask4dvc/utils/dask.py
+-rw-r--r--   0        0        0      136 2023-04-19 15:36:27.742838 dask4dvc-0.2.2/dask4dvc/utils/main.py
+-rw-r--r--   0        0        0     1274 2023-04-22 14:35:15.975209 dask4dvc-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 dask4dvc-0.2.2/PKG-INFO
```

### Comparing `dask4dvc-0.2.1/LICENSE` & `dask4dvc-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.2.1/README.md` & `dask4dvc-0.2.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,27 @@
 
 # Dask4DVC - Distributed Node Exectuion
 [DVC](dvc.org) provides tools for building and executing the computational graph locally through various methods. 
 The `dask4dvc` package combines [Dask Distributed](https://distributed.dask.org/) with DVC to make it easier to use with HPC managers like [Slurm](https://github.com/SchedMD/slurm).
 
 The `dask4dvc` package will try to run the DVC graph in parallel.
 
-> :warning: dask4dvc will disbale a few of the checks that DVC implements. Do not make changes to your workspace during the runtime of `dask4dvc repro`.
+> :warning: This is an experimental package **not** affiliated in any way with iterative or DVC. ``dask4dvc`` will disbale a few of the checks that DVC implements. Do not make changes to your workspace during the runtime of `dask4dvc`.
 
 ## Usage
 Dask4DVC provides a CLI similar to DVC.
 
 - `dvc repro` becomes `dask4dvc repro`.
+- `dvc queue start --jobs 1` becomes `dask4dvc run`
+
+You can follow the progress using `dask4dvc <cmd> --dashboard`.
+
+> `dask4dvc run --parallel` is available for `dvc queue start --jobs <max-workers>` but it currently leads to the failure of some experiments.
+
+> The `dask4dvc` error messages are currently really sparse. For better error messages please use the DVC commands.
 
 ### SLURM Cluster
 
 You can use `dask4dvc` easily with a slurm cluster.
 This requires a running dask scheduler:
 ```python
 from dask_jobqueue import SLURMCluster
```

### Comparing `dask4dvc-0.2.1/dask4dvc/__init__.py` & `dask4dvc-0.2.2/dask4dvc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """The 'dask4dvc' package."""
 import importlib.metadata
 import logging
 import sys
+
 import dvc.logger
 
-from dask4dvc import cli, methods, utils
+from dask4dvc import cli, dvc_repro, utils
 
-__all__ = ["cli", "utils", "methods"]
+__all__ = ["cli", "utils", "dvc_repro"]
 
 __version__ = importlib.metadata.version("dask4dvc")
 
 log = logging.getLogger(__name__)
 log.setLevel(logging.DEBUG)
 
 # Formatter for advanced logging
```

### Comparing `dask4dvc-0.2.1/dask4dvc/methods.py` & `dask4dvc-0.2.2/dask4dvc/dvc_repro.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Some general 'dask4dvc' methods."""
 
 
 import contextlib
-import typing
 import logging
+import os
+import random
+import subprocess
+import time
+import typing
 
 import dask.distributed
-import dvc.lock
 import dvc.exceptions
+import dvc.lock
 import dvc.repo
-from dvc.repo.reproduce import _get_steps
-import dvc.utils.strictyaml
 import dvc.stage
+import dvc.utils.strictyaml
+from dvc.repo.reproduce import _get_steps
 from dvc.stage.cache import RunCacheNotFoundError
-import random
-import time
-import subprocess
 
 from dask4dvc import utils
 
 log = logging.getLogger(__name__)
 
 
 def _run_locked_cmd(
@@ -62,22 +63,24 @@
     RunCacheNotFoundError:
         if the stage is not cached.
     """
     with dvc.repo.lock_repo(repo):
         with repo.scm_context():
             repo.stage_cache.restore(stage=stage)
             log.info(
-                f"Stage '{stage.addressing}' is cached - skipping run, checking out"
-                " outputs "
+                f"Stage '{stage.name}' is cached - skipping run, checking out outputs "
             )
 
 
-def submit_stage(name: str, force: bool, successors: list) -> str:
+def submit_stage(
+    name: str, force: bool, successors: list, root_dir: str
+) -> typing.List[str]:
     """Submit a stage to the Dask cluster."""
-    repo = dvc.repo.Repo()
+    os.chdir(root_dir)
+    repo = dvc.repo.Repo(root_dir)
 
     if force:
         stages = [repo.stage.get_target(name)]
     else:
         # dvc reproduce returns the stages that are not checked out
         stages = _run_locked_cmd(repo, repo.reproduce, name, dry=True, single_item=True)
 
@@ -98,23 +101,60 @@
                     return name
             # if not, run the stage
             log.info(f"Running stage '{name}': \n > {stage.cmd}")
             subprocess.check_call(stage.cmd, shell=True)
             # add the stage to the run cache
             _run_locked_cmd(repo, repo.commit, name, force=True)
 
-    return name
+    return [x.name for x in stages]
+
+
+def reproduce(
+    repo: dvc.repo.Repo,
+    targets=None,
+    recursive=False,
+    pipeline=False,
+    all_pipelines=False,
+    after_repro_callback=None,  # TODO
+    client: dask.distributed.Client = None,
+    prefix: str = None,
+    **kwargs,
+) -> typing.List[dvc.stage.PipelineStage]:
+    """Parallel Exectuion drop-in replacement for 'dvc.repo.Repo.reproduce'.
+
+    Use with functools.partial to set the client and prefix
+    """
+    if targets is None:
+        targets = []
+    mapping = parallel_submit(
+        client,
+        targets,
+        force=kwargs.get("force", False),
+        root_dir=repo.root_dir,
+        prefix=prefix,
+    )
+    results: typing.Dict[str, list] = utils.dask.wait_for_futures(client, mapping)
+    result = []
+    for stages in results.values():
+        if isinstance(stages, str):  # TODO this should always be a list?
+            stages = [stages]
+        result.extend([repo.stage.get_target(x) for x in stages])
+    return result
 
 
 def parallel_submit(
-    client: dask.distributed.Client, targets: list[str], force: bool
+    client: dask.distributed.Client,
+    targets: list[str],
+    force: bool,
+    root_dir: str = None,
+    prefix: str = None,
 ) -> typing.Dict[str, dask.distributed.Future]:
     """Submit all stages to the Dask cluster."""
     mapping = {}
-    repo = dvc.repo.Repo()
+    repo = dvc.repo.Repo(root_dir)
 
     if len(targets) == 0:
         targets = repo.index.graph.nodes
     else:
         targets = [repo.stage.get_target(x) for x in targets]
 
     nodes = _get_steps(repo.index.graph, targets, downstream=False, single_item=False)
@@ -125,21 +165,26 @@
             # we don't need to run it
             mapping[node] = None
             continue
         successors = [
             mapping[successor] for successor in repo.index.graph.successors(node)
         ]
 
+        if len(successors) == 0 and prefix is not None:
+            successors = [dask.distributed.Variable(prefix).get()]
+        # https://docs.dask.org/en/stable/futures.html#distributed.Variable to connect to main graph
+
         mapping[node] = client.submit(
             submit_stage,
-            node.addressing,
+            node.name,
             force=force,
+            root_dir=repo.root_dir,
             successors=successors,
             pure=False,
-            key=node.addressing,
+            key=f"{prefix}_{node.name}" if prefix else node.name,
         )
 
     mapping = {
-        node.addressing: future for node, future in mapping.items() if future is not None
+        node.name: future for node, future in mapping.items() if future is not None
     }
 
     return mapping
```

### Comparing `dask4dvc-0.2.1/dask4dvc/utils/dask.py` & `dask4dvc-0.2.2/dask4dvc/utils/dask.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 """Utils that are related to 'dask'."""
 import logging
 import pathlib
 import typing
 
 import dask_jobqueue
 import yaml
-from dask.distributed import Future
+from dask.distributed import Client, Future, wait
 
 log = logging.getLogger(__name__)
 
 
-def wait_for_futures(futures: typing.Union[Future, typing.Dict[str, Future]]) -> None:
+def wait_for_futures(
+    client: Client, futures: typing.Union[Future, typing.Dict[str, Future]]
+) -> dict:
     """Wait for all given future objects to complete.
 
     Raises
     ------
     This will fail if one of them fails.
     """
     if isinstance(futures, Future):
         futures = {"main": futures}
 
-    for future in futures.values():
+    wait(list(futures.values()))
+
+    results = {}
+    for name, future in futures.items():
         try:
-            _ = future.result()
+            results[name] = client.gather(future)
         except Exception as err:
             log.critical(f"Waiting for result from '{future}' failed with {err}")
+    return results
 
 
 def get_cluster_from_config(file: str) -> dask_jobqueue.core.JobQueueCluster:
     """Read 'dask4dvc' config file and create a cluster."""
     data = yaml.safe_load(pathlib.Path(file).read_text())
     default = data["default"]
     cluster_name = next(iter(default))
```

### Comparing `dask4dvc-0.2.1/pyproject.toml` & `dask4dvc-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dask4dvc"
-version = "0.2.1"
+version = "0.2.2"
 description = "Use dask to run the DVC graph"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "HPC", "dask", "DVC"]
 readme = "README.md"
 
 [tool.poetry.urls]
@@ -13,15 +13,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 dask = "^2022.7.1"
 distributed = "^2022.7.1"
 dask-jobqueue = "^0.8.1"
 dvc = "^2.54.0"
 typer = {extras = ["all"], version = "^0.7.0"}
-bokeh = "^2"
+bokeh = ">=2.4.2,<3"
 # for bokeh see https://distributed.dask.org/en/stable/changelog.html#v2022-11-1
 
 [tool.poetry.scripts]
 dask4dvc = 'dask4dvc.cli.main:app'
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^3.4.4"
@@ -50,9 +50,9 @@
 multi_line_output = 3
 
 [tool.ruff]
 line-length = 90
 
 select = ["E", "F", "D", "N", "C", "ANN"]
 extend-ignore = [
-    "D213", "D203", "ANN401"
+    "D213", "D203", "ANN401", "ANN101"
 ]
```

### Comparing `dask4dvc-0.2.1/PKG-INFO` & `dask4dvc-0.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dask4dvc
-Version: 0.2.1
+Version: 0.2.2
 Summary: Use dask to run the DVC graph
 License: Apache-2.0
 Keywords: data-science,HPC,dask,DVC
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bokeh (>=2,<3)
+Requires-Dist: bokeh (>=2.4.2,<3)
 Requires-Dist: dask (>=2022.7.1,<2023.0.0)
 Requires-Dist: dask-jobqueue (>=0.8.1,<0.9.0)
 Requires-Dist: distributed (>=2022.7.1,<2023.0.0)
 Requires-Dist: dvc (>=2.54.0,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Project-URL: repository, https://github.com/zincware/dask4dvc
 Description-Content-Type: text/markdown
@@ -29,20 +29,27 @@
 
 # Dask4DVC - Distributed Node Exectuion
 [DVC](dvc.org) provides tools for building and executing the computational graph locally through various methods. 
 The `dask4dvc` package combines [Dask Distributed](https://distributed.dask.org/) with DVC to make it easier to use with HPC managers like [Slurm](https://github.com/SchedMD/slurm).
 
 The `dask4dvc` package will try to run the DVC graph in parallel.
 
-> :warning: dask4dvc will disbale a few of the checks that DVC implements. Do not make changes to your workspace during the runtime of `dask4dvc repro`.
+> :warning: This is an experimental package **not** affiliated in any way with iterative or DVC. ``dask4dvc`` will disbale a few of the checks that DVC implements. Do not make changes to your workspace during the runtime of `dask4dvc`.
 
 ## Usage
 Dask4DVC provides a CLI similar to DVC.
 
 - `dvc repro` becomes `dask4dvc repro`.
+- `dvc queue start --jobs 1` becomes `dask4dvc run`
+
+You can follow the progress using `dask4dvc <cmd> --dashboard`.
+
+> `dask4dvc run --parallel` is available for `dvc queue start --jobs <max-workers>` but it currently leads to the failure of some experiments.
+
+> The `dask4dvc` error messages are currently really sparse. For better error messages please use the DVC commands.
 
 ### SLURM Cluster
 
 You can use `dask4dvc` easily with a slurm cluster.
 This requires a running dask scheduler:
 ```python
 from dask_jobqueue import SLURMCluster
```

