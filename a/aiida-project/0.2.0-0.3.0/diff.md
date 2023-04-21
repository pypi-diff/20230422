# Comparing `tmp/aiida-project-0.2.0.tar.gz` & `tmp/aiida-project-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-project-0.2.0.tar", last modified: Wed Apr 19 15:36:14 2023, max compression
+gzip compressed data, was "aiida-project-0.3.0.tar", last modified: Fri Apr 21 23:23:52 2023, max compression
```

## Comparing `aiida-project-0.2.0.tar` & `aiida-project-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1171 2023-04-19 15:36:09.721393 aiida-project-0.2.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1508 2023-04-19 15:36:09.721393 aiida-project-0.2.0/.github/workflows/validate_release_tag.py
--rw-r--r--   0        0        0      255 2023-04-19 15:36:09.721393 aiida-project-0.2.0/.gitignore
--rw-r--r--   0        0        0      298 2023-04-19 15:36:09.721393 aiida-project-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1311 2023-04-19 15:36:09.721393 aiida-project-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      255 2023-04-19 15:36:09.721393 aiida-project-0.2.0/README.md
--rw-r--r--   0        0        0      689 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/__init__.py
--rw-r--r--   0        0        0      125 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/commands/__init__.py
--rw-r--r--   0        0        0     2365 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/commands/create.py
--rw-r--r--   0        0        0       91 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/commands/main.py
--rw-r--r--   0        0        0       59 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/__init__.py
--rw-r--r--   0        0        0      775 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/base.py
--rw-r--r--   0        0        0     1424 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/conda.py
--rw-r--r--   0        0        0      287 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/factory.py
--rw-r--r--   0        0        0     1119 2023-04-19 15:36:09.721393 aiida-project-0.2.0/aiida_project/engine/virtualenv.py
--rw-r--r--   0        0        0     1036 2023-04-19 15:36:09.721393 aiida-project-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 aiida-project-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1171 2023-04-21 23:23:47.731673 aiida-project-0.3.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1564 2023-04-21 23:23:47.731673 aiida-project-0.3.0/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0      255 2023-04-21 23:23:47.731673 aiida-project-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1005 2023-04-21 23:23:47.731673 aiida-project-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1349 2023-04-21 23:23:47.731673 aiida-project-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1312 2023-04-21 23:23:47.731673 aiida-project-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      255 2023-04-21 23:23:47.731673 aiida-project-0.3.0/README.md
+-rw-r--r--   0        0        0      665 2023-04-21 23:23:47.731673 aiida-project-0.3.0/aiida_project/__init__.py
+-rw-r--r--   0        0        0      186 2023-04-21 23:23:47.731673 aiida-project-0.3.0/aiida_project/commands/__init__.py
+-rw-r--r--   0        0        0     2740 2023-04-21 23:23:47.731673 aiida-project-0.3.0/aiida_project/commands/create.py
+-rw-r--r--   0        0        0      714 2023-04-21 23:23:47.731673 aiida-project-0.3.0/aiida_project/commands/destroy.py
+-rw-r--r--   0        0        0       91 2023-04-21 23:23:47.735673 aiida-project-0.3.0/aiida_project/commands/main.py
+-rw-r--r--   0        0        0     2381 2023-04-21 23:23:47.735673 aiida-project-0.3.0/aiida_project/config.py
+-rw-r--r--   0        0        0      240 2023-04-21 23:23:47.735673 aiida-project-0.3.0/aiida_project/project/__init__.py
+-rw-r--r--   0        0        0     1746 2023-04-21 23:23:47.735673 aiida-project-0.3.0/aiida_project/project/base.py
+-rw-r--r--   0        0        0     1574 2023-04-21 23:23:47.735673 aiida-project-0.3.0/aiida_project/project/conda.py
+-rw-r--r--   0        0        0     2017 2023-04-21 23:23:47.735673 aiida-project-0.3.0/aiida_project/project/virtualenv.py
+-rw-r--r--   0        0        0     1317 2023-04-21 23:23:47.735673 aiida-project-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 aiida-project-0.3.0/PKG-INFO
```

### Comparing `aiida-project-0.2.0/.github/workflows/cd.yml` & `aiida-project-0.3.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `aiida-project-0.2.0/.github/workflows/validate_release_tag.py` & `aiida-project-0.3.0/.github/workflows/validate_release_tag.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-# -*- coding: utf-8 -*-
 """Validate that the version in the tag label matches the version of the package."""
 import argparse
 import ast
 from pathlib import Path
 
 
 def get_version_from_module(content: str) -> str:
     """Get the ``__version__`` attribute from a module.
 
     .. note:: This has been adapted from :mod:`setuptools.config`.
     """
     try:
         module = ast.parse(content)
     except SyntaxError as exception:
-        raise IOError('Unable to parse module.') from exception
+        raise OSError("Unable to parse module.") from exception
 
     try:
         return next(
-            ast.literal_eval(statement.value) for statement in module.body if isinstance(statement, ast.Assign)
-            for target in statement.targets if isinstance(target, ast.Name) and target.id == '__version__'
+            ast.literal_eval(statement.value)
+            for statement in module.body
+            if isinstance(statement, ast.Assign)
+            for target in statement.targets
+            if isinstance(target, ast.Name) and target.id == "__version__"
         )
     except StopIteration as exception:
-        raise IOError('Unable to find the `__version__` attribute in the module.') from exception
+        raise OSError("Unable to find the `__version__` attribute in the module.") from exception
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     parser = argparse.ArgumentParser()
-    parser.add_argument('GITHUB_REF', help='The GITHUB_REF environmental variable')
+    parser.add_argument("GITHUB_REF", help="The GITHUB_REF environmental variable")
     args = parser.parse_args()
-    assert args.GITHUB_REF.startswith('refs/tags/v'), f'GITHUB_REF should start with "refs/tags/v": {args.GITHUB_REF}'
+    assert args.GITHUB_REF.startswith(
+        "refs/tags/v"
+    ), f'GITHUB_REF should start with "refs/tags/v": {args.GITHUB_REF}'
     tag_version = args.GITHUB_REF[11:]
-    package_version = get_version_from_module(Path('aiida_project/__init__.py').read_text(encoding='utf-8'))
-    error_message = f'The tag version `{tag_version}` is different from the package version `{package_version}`'
+    package_version = get_version_from_module(
+        Path("aiida_project/__init__.py").read_text(encoding="utf-8")
+    )
+    error_message = (
+        f"The tag version `{tag_version}` is different from the package version `{package_version}`"
+    )
     assert tag_version == package_version, error_message
```

### Comparing `aiida-project-0.2.0/LICENSE.txt` & `aiida-project-0.3.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+THE SOFTWARE.
```

### Comparing `aiida-project-0.2.0/aiida_project/__init__.py` & `aiida-project-0.3.0/aiida_project/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
 ###########################################################################
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """The `aiida-project` module."""
 
-__version__ = '0.2.0'
+__version__ = "0.3.0"
```

### Comparing `aiida-project-0.2.0/aiida_project/engine/conda.py` & `aiida-project-0.3.0/aiida_project/project/conda.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,49 @@
-import os
-import subprocess
-import py
-import json
-
-from aiida_project.engine.base import BaseEngine
-
-
-class CondaEngine(BaseEngine):
-
-    def __init__(self, project_path):
-        super(CondaEngine, self).__init__(project_path)
-        self.conda_info = json.loads(subprocess.check_output(['conda', 'info', '-a', '--json']))
-
-    @property
-    def conda_path(self):
-        return py.path.local(conda_info['conda_prefix'])
-
-    @property
-    def venv_path(self):
-        for path in self.conda_info['envs_dirs']:
-            env_collection_path = py.path.local(path)
-            env_path = env_collection_path.join(self.venv_name)
-            if env_path.exists():
-                return env_path
-        return None
-
-    def create(self, name, python=None):
-        self._venv_name = name
-        if not self.venv_path:
-            conda_command = ['conda', 'create', '-y', '-n', name, 'python=2']
-            subprocess.check_call(conda_command)
-
-    def add_activate_script(self, path):
-        activate_d_path = self.venv_path.join('etc', 'conda', 'activate.d')
-        activate_d_path.ensure_dir()
-        os.symlink(path.strpath, activate_d_path.join(path.basename).strpath)
-
-    def add_deactivate_scritp(self, path):
-        deactivate_d_path = self.venv_path.join('etc', 'conda', 'deactivate.d')
-        deactivate_d_path.ensure_dir()
-        os.symlink(path.strpath, deactivate_d_path.join(path.basename).strpath)
+# import json
+# import os
+# import subprocess
+
+# import py  # type: ignore
+
+from aiida_project.project.base import BaseProject
+
+
+class CondaProject(BaseProject):
+    """Conda environment."""
+
+    _engine = "conda"
+
+
+#     def __init__(self, project_path):
+#         super().__init__(project_path)
+#         self.conda_info = json.loads(
+#             subprocess.check_output(["conda", "info", "-a", "--json"])
+#         )
+
+#     @property
+#     def conda_path(self):
+#         return py.path.local(self.conda_info["conda_prefix"])
+
+#     @property
+#     def venv_path(self):
+#         for path in self.conda_info["envs_dirs"]:
+#             env_collection_path = py.path.local(path)
+#             env_path = env_collection_path.join(self.venv_name)
+#             if env_path.exists():
+#                 return env_path
+#         return None
+
+#     def create(self, name, python=None):
+#         self._venv_name = name
+#         if not self.venv_path:
+#             conda_command = ["conda", "create", "-y", "-n", name, "python=2"]
+#             subprocess.check_call(conda_command)
+
+#     def add_activate_script(self, path):
+#         activate_d_path = self.venv_path.join("etc", "conda", "activate.d")
+#         activate_d_path.ensure_dir()
+#         os.symlink(path.strpath, activate_d_path.join(path.basename).strpath)
+
+#     def add_deactivate_scritp(self, path):
+#         deactivate_d_path = self.venv_path.join("etc", "conda", "deactivate.d")
+#         deactivate_d_path.ensure_dir()
+#         os.symlink(path.strpath, deactivate_d_path.join(path.basename).strpath)
```

### Comparing `aiida-project-0.2.0/pyproject.toml` & `aiida-project-0.3.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -23,14 +23,35 @@
     "Topic :: Scientific/Engineering"
 ]
 keywords = ["aiida", "workflows"]
 requires-python = ">=3.8"
 dependencies = [
   "click~=8.1.2",
   "py~=1.11.0",
+  "pydantic~=1.10.7",
+  "python-dotenv~=1.0.0",
 ]
 
 [project.urls]
 Source = "https://github.com/aiidateam/aiida-project"
 
 [project.scripts]
 aiida-project = "aiida_project.commands:main"
+
+[project.optional-dependencies]
+dev = [
+  "pre-commit~=3.2.2",
+]
+
+[tool.black]
+line-length = 100
+
+[tool.ruff]
+line-length = 100
+
+[[tool.mypy.overrides]]
+module = [
+  "dotenv",
+  "pydantic",
+  "yaml",
+]
+ignore_missing_imports = true
```

### Comparing `aiida-project-0.2.0/PKG-INFO` & `aiida-project-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-project
-Version: 0.2.0
+Version: 0.3.0
 Summary: An AiiDA environment manager
 Keywords: aiida,workflows
 Author-email: The AiiDA team <developers@aiida.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: AiiDA
@@ -15,15 +15,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: click~=8.1.2
 Requires-Dist: py~=1.11.0
+Requires-Dist: pydantic~=1.10.7
+Requires-Dist: python-dotenv~=1.0.0
+Requires-Dist: pre-commit~=3.2.2 ; extra == "dev"
 Project-URL: Source, https://github.com/aiidateam/aiida-project
+Provides-Extra: dev
 
 # AiiDA-Project
 
 This python package provides cli commands to manage separate AiiDA environments (called "projects").
 
 The main intention is to collect all the pieces that make this possible together, to eventually get this functionality built into AiiDA
```

