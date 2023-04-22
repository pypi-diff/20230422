# Comparing `tmp/poetry_polylith_plugin-1.5.2.tar.gz` & `tmp/poetry_polylith_plugin-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_polylith_plugin-1.5.2.tar", max compression
+gzip compressed data, was "poetry_polylith_plugin-1.6.0.tar", max compression
```

## Comparing `poetry_polylith_plugin-1.5.2.tar` & `poetry_polylith_plugin-1.6.0.tar`

### file list

```diff
@@ -1,55 +1,63 @@
--rw-r--r--   0        0        0     1475 2023-03-26 20:11:55.858371 poetry_polylith_plugin-1.5.2/README.md
--rw-r--r--   0        0        0      244 2022-11-08 07:28:40.662859 poetry_polylith_plugin-1.5.2/polylith/bricks/__init__.py
--rw-r--r--   0        0        0      555 2023-02-17 18:12:11.442075 poetry_polylith_plugin-1.5.2/polylith/bricks/base.py
--rw-r--r--   0        0        0     1045 2023-02-20 14:40:39.599185 poetry_polylith_plugin-1.5.2/polylith/bricks/brick.py
--rw-r--r--   0        0        0     1096 2023-03-13 16:15:02.726313 poetry_polylith_plugin-1.5.2/polylith/bricks/component.py
--rw-r--r--   0        0        0       56 2023-02-13 17:04:54.666249 poetry_polylith_plugin-1.5.2/polylith/check/__init__.py
--rw-r--r--   0        0        0     1051 2023-03-05 09:12:59.774422 poetry_polylith_plugin-1.5.2/polylith/check/grouping.py
--rw-r--r--   0        0        0     1870 2023-04-04 19:03:03.390298 poetry_polylith_plugin-1.5.2/polylith/check/report.py
--rw-r--r--   0        0        0       98 2022-11-02 17:12:23.977141 poetry_polylith_plugin-1.5.2/polylith/development/__init__.py
--rw-r--r--   0        0        0      211 2022-12-27 08:11:31.407975 poetry_polylith_plugin-1.5.2/polylith/development/development.py
--rw-r--r--   0        0        0       75 2022-11-14 11:36:16.519559 poetry_polylith_plugin-1.5.2/polylith/diff/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-04 19:32:03.326381 poetry_polylith_plugin-1.5.2/polylith/diff/collect.py
--rw-r--r--   0        0        0     2781 2023-03-13 17:19:22.526709 poetry_polylith_plugin-1.5.2/polylith/diff/report.py
--rw-r--r--   0        0        0       68 2022-11-02 17:12:23.977917 poetry_polylith_plugin-1.5.2/polylith/dirs/__init__.py
--rw-r--r--   0        0        0      273 2023-01-06 10:47:07.824141 poetry_polylith_plugin-1.5.2/polylith/dirs/dirs.py
--rw-r--r--   0        0        0       72 2022-11-02 17:12:23.978829 poetry_polylith_plugin-1.5.2/polylith/files/__init__.py
--rw-r--r--   0        0        0      145 2022-12-22 20:33:19.860064 poetry_polylith_plugin-1.5.2/polylith/files/files.py
--rw-r--r--   0        0        0      426 2023-03-26 19:47:00.762194 poetry_polylith_plugin-1.5.2/polylith/info/__init__.py
--rw-r--r--   0        0        0     1692 2023-03-26 19:47:00.762913 poetry_polylith_plugin-1.5.2/polylith/info/collect.py
--rw-r--r--   0        0        0     2339 2023-03-26 19:47:00.763423 poetry_polylith_plugin-1.5.2/polylith/info/report.py
--rw-r--r--   0        0        0       91 2022-11-02 17:12:23.979601 poetry_polylith_plugin-1.5.2/polylith/interface/__init__.py
--rw-r--r--   0        0        0      876 2023-02-17 18:12:11.443769 poetry_polylith_plugin-1.5.2/polylith/interface/interfaces.py
--rw-r--r--   0        0        0      277 2023-04-04 19:03:03.392187 poetry_polylith_plugin-1.5.2/polylith/libs/__init__.py
--rw-r--r--   0        0        0     1607 2023-04-04 19:03:03.393504 poetry_polylith_plugin-1.5.2/polylith/libs/grouping.py
--rw-r--r--   0        0        0     1298 2023-04-04 19:03:03.394867 poetry_polylith_plugin-1.5.2/polylith/libs/imports.py
--rw-r--r--   0        0        0     3794 2023-04-01 11:11:39.008392 poetry_polylith_plugin-1.5.2/polylith/libs/report.py
--rw-r--r--   0        0        0     4156 2023-04-05 16:07:40.714954 poetry_polylith_plugin-1.5.2/polylith/libs/stdlib.py
--rw-r--r--   0        0        0      717 2023-04-04 19:03:03.396088 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/__init__.py
--rw-r--r--   0        0        0     2188 2023-03-26 19:47:00.765011 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/check.py
--rw-r--r--   0        0        0      552 2023-02-17 18:12:11.444317 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create.py
--rw-r--r--   0        0        0      634 2023-02-17 18:12:11.444887 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create_base.py
--rw-r--r--   0        0        0      674 2023-03-26 12:16:38.669733 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create_component.py
--rw-r--r--   0        0        0      680 2023-02-17 18:12:11.446154 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create_project.py
--rw-r--r--   0        0        0      949 2022-11-13 15:37:24.280622 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create_workspace.py
--rw-r--r--   0        0        0     1744 2023-04-04 19:32:03.326950 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/diff.py
--rw-r--r--   0        0        0      876 2023-03-26 13:11:39.932369 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/info.py
--rw-r--r--   0        0        0     2328 2023-03-26 19:47:00.766358 poetry_polylith_plugin-1.5.2/polylith/poetry/commands/libs.py
--rw-r--r--   0        0        0       87 2022-11-02 17:12:23.974544 poetry_polylith_plugin-1.5.2/polylith/poetry_plugin/__init__.py
--rw-r--r--   0        0        0      925 2023-04-04 19:03:03.376731 poetry_polylith_plugin-1.5.2/polylith/poetry_plugin/plugin.py
--rw-r--r--   0        0        0      305 2023-04-04 19:03:03.397463 poetry_polylith_plugin-1.5.2/polylith/project/__init__.py
--rw-r--r--   0        0        0     1577 2023-04-04 19:32:03.327496 poetry_polylith_plugin-1.5.2/polylith/project/create.py
--rw-r--r--   0        0        0     1433 2023-04-04 19:03:03.415645 poetry_polylith_plugin-1.5.2/polylith/project/get.py
--rw-r--r--   0        0        0      433 2023-03-26 19:47:00.767617 poetry_polylith_plugin-1.5.2/polylith/project/parser.py
--rw-r--r--   0        0        0      142 2023-02-17 18:12:11.447324 poetry_polylith_plugin-1.5.2/polylith/readme/__init__.py
--rw-r--r--   0        0        0     1067 2023-04-04 19:32:03.328075 poetry_polylith_plugin-1.5.2/polylith/readme/readme.py
--rw-r--r--   0        0        0      374 2022-11-07 20:40:56.909336 poetry_polylith_plugin-1.5.2/polylith/repo/__init__.py
--rw-r--r--   0        0        0      985 2022-11-07 20:40:56.910072 poetry_polylith_plugin-1.5.2/polylith/repo/repo.py
--rw-r--r--   0        0        0       71 2022-11-02 17:12:23.985824 poetry_polylith_plugin-1.5.2/polylith/test/__init__.py
--rw-r--r--   0        0        0      859 2022-11-13 15:37:24.282091 poetry_polylith_plugin-1.5.2/polylith/test/tests.py
--rw-r--r--   0        0        0       94 2023-02-19 21:57:26.720321 poetry_polylith_plugin-1.5.2/polylith/workspace/__init__.py
--rw-r--r--   0        0        0     1089 2023-02-17 18:12:11.448456 poetry_polylith_plugin-1.5.2/polylith/workspace/create.py
--rw-r--r--   0        0        0     1789 2023-02-17 18:12:11.448944 poetry_polylith_plugin-1.5.2/polylith/workspace/parser.py
--rw-r--r--   0        0        0      949 2023-02-19 21:57:26.720906 poetry_polylith_plugin-1.5.2/polylith/workspace/paths.py
--rw-r--r--   0        0        0      781 2023-04-05 16:12:21.226503 poetry_polylith_plugin-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1475 2023-03-26 20:11:55.858371 poetry_polylith_plugin-1.6.0/README.md
+-rw-r--r--   0        0        0      244 2022-11-08 07:28:40.662859 poetry_polylith_plugin-1.6.0/polylith/bricks/__init__.py
+-rw-r--r--   0        0        0      555 2023-02-17 18:12:11.442075 poetry_polylith_plugin-1.6.0/polylith/bricks/base.py
+-rw-r--r--   0        0        0     1045 2023-02-20 14:40:39.599185 poetry_polylith_plugin-1.6.0/polylith/bricks/brick.py
+-rw-r--r--   0        0        0     1096 2023-03-13 16:15:02.726313 poetry_polylith_plugin-1.6.0/polylith/bricks/component.py
+-rw-r--r--   0        0        0       56 2023-02-13 17:04:54.666249 poetry_polylith_plugin-1.6.0/polylith/check/__init__.py
+-rw-r--r--   0        0        0     1051 2023-03-05 09:12:59.774422 poetry_polylith_plugin-1.6.0/polylith/check/grouping.py
+-rw-r--r--   0        0        0     1756 2023-04-22 15:22:45.897523 poetry_polylith_plugin-1.6.0/polylith/check/report.py
+-rw-r--r--   0        0        0       98 2022-11-02 17:12:23.977141 poetry_polylith_plugin-1.6.0/polylith/development/__init__.py
+-rw-r--r--   0        0        0      211 2022-12-27 08:11:31.407975 poetry_polylith_plugin-1.6.0/polylith/development/development.py
+-rw-r--r--   0        0        0       75 2022-11-14 11:36:16.519559 poetry_polylith_plugin-1.6.0/polylith/diff/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-16 08:27:58.640337 poetry_polylith_plugin-1.6.0/polylith/diff/collect.py
+-rw-r--r--   0        0        0     2670 2023-04-22 15:22:45.898218 poetry_polylith_plugin-1.6.0/polylith/diff/report.py
+-rw-r--r--   0        0        0       68 2022-11-02 17:12:23.977917 poetry_polylith_plugin-1.6.0/polylith/dirs/__init__.py
+-rw-r--r--   0        0        0      273 2023-01-06 10:47:07.824141 poetry_polylith_plugin-1.6.0/polylith/dirs/dirs.py
+-rw-r--r--   0        0        0       72 2022-11-02 17:12:23.978829 poetry_polylith_plugin-1.6.0/polylith/files/__init__.py
+-rw-r--r--   0        0        0      145 2022-12-22 20:33:19.860064 poetry_polylith_plugin-1.6.0/polylith/files/files.py
+-rw-r--r--   0        0        0      151 2023-04-22 15:22:45.913554 poetry_polylith_plugin-1.6.0/polylith/imports/__init__.py
+-rw-r--r--   0        0        0     1687 2023-04-22 15:22:45.914360 poetry_polylith_plugin-1.6.0/polylith/imports/parser.py
+-rw-r--r--   0        0        0      426 2023-03-26 19:47:00.762194 poetry_polylith_plugin-1.6.0/polylith/info/__init__.py
+-rw-r--r--   0        0        0     1692 2023-03-26 19:47:00.762913 poetry_polylith_plugin-1.6.0/polylith/info/collect.py
+-rw-r--r--   0        0        0     2216 2023-04-22 15:22:45.914914 poetry_polylith_plugin-1.6.0/polylith/info/report.py
+-rw-r--r--   0        0        0       91 2022-11-02 17:12:23.979601 poetry_polylith_plugin-1.6.0/polylith/interface/__init__.py
+-rw-r--r--   0        0        0      876 2023-02-17 18:12:11.443769 poetry_polylith_plugin-1.6.0/polylith/interface/interfaces.py
+-rw-r--r--   0        0        0      201 2023-04-22 15:22:45.915728 poetry_polylith_plugin-1.6.0/polylith/libs/__init__.py
+-rw-r--r--   0        0        0     1220 2023-04-22 15:22:45.916666 poetry_polylith_plugin-1.6.0/polylith/libs/grouping.py
+-rw-r--r--   0        0        0     3677 2023-04-22 15:22:45.917187 poetry_polylith_plugin-1.6.0/polylith/libs/report.py
+-rw-r--r--   0        0        0     4156 2023-04-16 08:27:58.676339 poetry_polylith_plugin-1.6.0/polylith/libs/stdlib.py
+-rw-r--r--   0        0        0      790 2023-04-22 15:22:45.918035 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/__init__.py
+-rw-r--r--   0        0        0     2188 2023-03-26 19:47:00.765011 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/check.py
+-rw-r--r--   0        0        0      552 2023-02-17 18:12:11.444317 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create.py
+-rw-r--r--   0        0        0      634 2023-02-17 18:12:11.444887 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_base.py
+-rw-r--r--   0        0        0      674 2023-03-26 12:16:38.669733 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_component.py
+-rw-r--r--   0        0        0      680 2023-02-17 18:12:11.446154 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_project.py
+-rw-r--r--   0        0        0      949 2022-11-13 15:37:24.280622 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_workspace.py
+-rw-r--r--   0        0        0     1744 2023-04-16 08:27:58.696930 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/diff.py
+-rw-r--r--   0        0        0      876 2023-03-26 13:11:39.932369 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/info.py
+-rw-r--r--   0        0        0     2328 2023-03-26 19:47:00.766358 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/libs.py
+-rw-r--r--   0        0        0     1676 2023-04-22 15:22:45.936406 poetry_polylith_plugin-1.6.0/polylith/poetry/commands/sync.py
+-rw-r--r--   0        0        0       87 2022-11-02 17:12:23.974544 poetry_polylith_plugin-1.6.0/polylith/poetry_plugin/__init__.py
+-rw-r--r--   0        0        0      959 2023-04-22 15:22:45.896775 poetry_polylith_plugin-1.6.0/polylith/poetry_plugin/plugin.py
+-rw-r--r--   0        0        0      331 2023-04-22 15:22:45.947457 poetry_polylith_plugin-1.6.0/polylith/project/__init__.py
+-rw-r--r--   0        0        0     1577 2023-04-16 08:27:58.716399 poetry_polylith_plugin-1.6.0/polylith/project/create.py
+-rw-r--r--   0        0        0     1433 2023-04-22 15:22:45.948301 poetry_polylith_plugin-1.6.0/polylith/project/get.py
+-rw-r--r--   0        0        0      433 2023-03-26 19:47:00.767617 poetry_polylith_plugin-1.6.0/polylith/project/parser.py
+-rw-r--r--   0        0        0      142 2023-02-17 18:12:11.447324 poetry_polylith_plugin-1.6.0/polylith/readme/__init__.py
+-rw-r--r--   0        0        0     1067 2023-04-16 08:27:58.749480 poetry_polylith_plugin-1.6.0/polylith/readme/readme.py
+-rw-r--r--   0        0        0      374 2022-11-07 20:40:56.909336 poetry_polylith_plugin-1.6.0/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      985 2022-11-07 20:40:56.910072 poetry_polylith_plugin-1.6.0/polylith/repo/repo.py
+-rw-r--r--   0        0        0       58 2023-04-22 15:22:45.972545 poetry_polylith_plugin-1.6.0/polylith/reporting/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-22 15:22:45.973024 poetry_polylith_plugin-1.6.0/polylith/reporting/theme.py
+-rw-r--r--   0        0        0      188 2023-04-22 15:22:45.985436 poetry_polylith_plugin-1.6.0/polylith/sync/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-22 15:22:45.985876 poetry_polylith_plugin-1.6.0/polylith/sync/collect.py
+-rw-r--r--   0        0        0      794 2023-04-22 15:22:45.986174 poetry_polylith_plugin-1.6.0/polylith/sync/report.py
+-rw-r--r--   0        0        0     1787 2023-04-22 15:22:45.986750 poetry_polylith_plugin-1.6.0/polylith/sync/update.py
+-rw-r--r--   0        0        0       71 2022-11-02 17:12:23.985824 poetry_polylith_plugin-1.6.0/polylith/test/__init__.py
+-rw-r--r--   0        0        0      859 2022-11-13 15:37:24.282091 poetry_polylith_plugin-1.6.0/polylith/test/tests.py
+-rw-r--r--   0        0        0       94 2023-02-19 21:57:26.720321 poetry_polylith_plugin-1.6.0/polylith/workspace/__init__.py
+-rw-r--r--   0        0        0     1089 2023-02-17 18:12:11.448456 poetry_polylith_plugin-1.6.0/polylith/workspace/create.py
+-rw-r--r--   0        0        0     1789 2023-04-16 09:04:04.273168 poetry_polylith_plugin-1.6.0/polylith/workspace/parser.py
+-rw-r--r--   0        0        0      949 2023-02-19 21:57:26.720906 poetry_polylith_plugin-1.6.0/polylith/workspace/paths.py
+-rw-r--r--   0        0        0      781 2023-04-22 15:23:18.770242 poetry_polylith_plugin-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 poetry_polylith_plugin-1.6.0/PKG-INFO
```

### Comparing `poetry_polylith_plugin-1.5.2/README.md` & `poetry_polylith_plugin-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/bricks/base.py` & `poetry_polylith_plugin-1.6.0/polylith/bricks/base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/bricks/brick.py` & `poetry_polylith_plugin-1.6.0/polylith/bricks/brick.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/bricks/component.py` & `poetry_polylith_plugin-1.6.0/polylith/bricks/component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/check/grouping.py` & `poetry_polylith_plugin-1.6.0/polylith/check/grouping.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/check/report.py` & `poetry_polylith_plugin-1.6.0/polylith/check/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 from pathlib import Path
 from typing import Set
 
-from polylith import libs, workspace
+from polylith import imports, libs, workspace
 from polylith.check import grouping
+from polylith.reporting import theme
 from rich.console import Console
-from rich.theme import Theme
-
-info_theme = Theme(
-    {
-        "data": "#999966",
-        "proj": "#8A2BE2",
-        "comp": "#32CD32",
-        "base": "#6495ED",
-    }
-)
 
 
 def print_missing_deps(brick_imports: dict, deps: Set[str], project_name: str) -> bool:
     diff = libs.report.calculate_diff(brick_imports, deps)
 
     if not diff:
         return True
 
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
 
     missing = ", ".join(sorted(diff))
 
     console.print(f":thinking_face: Cannot locate {missing} in {project_name}")
     return False
 
 
@@ -37,16 +28,16 @@
 
     bases = {b for b in project_data.get("bases", [])}
     components = {c for c in project_data.get("components", [])}
 
     bases_paths = workspace.paths.collect_bases_paths(root, ns, bases)
     components_paths = workspace.paths.collect_components_paths(root, ns, components)
 
-    all_imports_in_bases = libs.fetch_all_imports(bases_paths)
-    all_imports_in_components = libs.fetch_all_imports(components_paths)
+    all_imports_in_bases = imports.fetch_all_imports(bases_paths)
+    all_imports_in_components = imports.fetch_all_imports(components_paths)
 
     brick_imports = {
         "bases": grouping.extract_brick_imports(all_imports_in_bases, ns),
         "components": grouping.extract_brick_imports(all_imports_in_components, ns),
     }
 
     third_party_imports = {
```

### Comparing `poetry_polylith_plugin-1.5.2/polylith/diff/collect.py` & `poetry_polylith_plugin-1.6.0/polylith/diff/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/diff/report.py` & `poetry_polylith_plugin-1.6.0/polylith/diff/report.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,15 @@
 from typing import List
 
+from polylith.reporting import theme
 from rich import box
 from rich.columns import Columns
 from rich.console import Console
 from rich.padding import Padding
 from rich.table import Table
-from rich.theme import Theme
-
-info_theme = Theme(
-    {
-        "data": "#999966",
-        "proj": "#8A2BE2",
-        "comp": "#32CD32",
-        "base": "#6495ED",
-    }
-)
 
 
 def brick_status(brick, bricks) -> str:
     status = ":gear:" if brick in bricks else "-"
 
     return f"[data]{status}[/]"
 
@@ -26,15 +17,15 @@
 def print_diff_details(
     projects_data: List[dict], bases: List[str], components: List[str]
 ) -> None:
 
     if not bases and not components:
         return
 
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
     table = Table(box=box.SIMPLE_HEAD)
     table.add_column("[data]changed brick[/]")
 
     proj_cols = [f"[proj]{project['name']}[/]" for project in projects_data]
     table.add_column(Columns(proj_cols, align="center", expand=True))
 
     for brick in sorted(components):
@@ -48,22 +39,22 @@
     console.print(table, overflow="ellipsis")
 
 
 def print_detected_changes_in_projects(projects: List[str]) -> None:
     if not projects:
         return
 
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
 
     for project in sorted(projects):
         console.print(f"[data]:gear: Changes found in [/][proj]{project}[/]")
 
 
 def print_diff_summary(tag: str, bases: List[str], components: List[str]) -> None:
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
 
     console.print(Padding(f"[data]Diff: based on the {tag} tag[/]", (1, 0, 1, 0)))
 
     if not bases and not components:
         console.print("[data]No brick changes found.[/]")
         return
 
@@ -94,9 +85,9 @@
 
     a = _changed_projects(projects_data, "components", components)
     b = _changed_projects(projects_data, "bases", bases)
     c = set(projects)
 
     res = {*a, *b, *c}
 
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
     console.print(",".join(res))
```

### Comparing `poetry_polylith_plugin-1.5.2/polylith/info/collect.py` & `poetry_polylith_plugin-1.6.0/polylith/info/collect.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/info/report.py` & `poetry_polylith_plugin-1.6.0/polylith/info/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,15 @@
 from typing import List
 
+from polylith.reporting import theme
 from rich import box
 from rich.columns import Columns
 from rich.console import Console
 from rich.padding import Padding
 from rich.table import Table
-from rich.theme import Theme
-
-info_theme = Theme(
-    {
-        "data": "#999966",
-        "proj": "#8A2BE2",
-        "comp": "#32CD32",
-        "base": "#6495ED",
-    }
-)
 
 
 def brick_status(brick, bricks) -> str:
     status = ":heavy_check_mark:" if brick in bricks else "-"
 
     return f"[data]{status}[/]"
 
@@ -38,15 +29,15 @@
 
 def print_bricks_in_projects(
     projects_data: List[dict], bases: List[str], components: List[str]
 ) -> None:
     if not components and not bases:
         return
 
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
     table = Table(box=box.SIMPLE_HEAD)
     table.add_column("[data]brick[/]")
 
     proj_cols = [printable_name(project) for project in projects_data]
     table.add_column(Columns(proj_cols, align="center", expand=True))
 
     for brick in sorted(components):
@@ -59,15 +50,15 @@
 
     console.print(table, overflow="ellipsis")
 
 
 def print_workspace_summary(
     projects_data: List[dict], bases: List[str], components: List[str]
 ) -> None:
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
 
     console.print(Padding("[data]Workspace summary[/]", (1, 0, 1, 0)))
 
     number_of_projects = len([p for p in projects_data if is_project(p)])
     number_of_components = len(components)
     number_of_bases = len(bases)
     number_of_dev = len([p for p in projects_data if not is_project(p)])
```

### Comparing `poetry_polylith_plugin-1.5.2/polylith/interface/interfaces.py` & `poetry_polylith_plugin-1.6.0/polylith/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/libs/grouping.py` & `poetry_polylith_plugin-1.6.0/polylith/libs/grouping.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,24 @@
 import sys
 from pathlib import Path
 from typing import Set
 
 from polylith import workspace
-from polylith.libs.imports import list_imports
+from polylith.imports import extract_top_ns, fetch_all_imports
 from polylith.libs.stdlib import standard_libs
 
 
 def get_python_version() -> str:
     return f"{sys.version_info.major}.{sys.version_info.minor}"
 
 
 def get_standard_libs(python_version: str) -> Set[str]:
     return standard_libs.get(python_version, set())
 
 
-def fetch_all_imports(paths: Set[Path]) -> dict:
-    rows = [{p.name: list_imports(p)} for p in paths]
-
-    return {k: v for row in rows for k, v in row.items()}
-
-
-def extract_top_ns_from_imports(imports: Set[str]) -> Set:
-    return {imp.split(".")[0] for imp in imports}
-
-
-def extract_top_ns(import_data: dict) -> dict:
-    return {k: extract_top_ns_from_imports(v) for k, v in import_data.items()}
-
-
 def exclude_libs(import_data: dict, to_exclude: Set) -> dict:
     return {k: v - to_exclude for k, v in import_data.items()}
 
 
 def exclude_empty(import_data: dict) -> dict:
     return {k: v for k, v in import_data.items() if v}
```

### Comparing `poetry_polylith_plugin-1.5.2/polylith/libs/report.py` & `poetry_polylith_plugin-1.6.0/polylith/libs/report.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 import difflib
 from pathlib import Path
 from typing import Set
 
 from polylith import info, workspace
 from polylith.libs import grouping
+from polylith.reporting import theme
 from rich import box
 from rich.console import Console
 from rich.padding import Padding
 from rich.table import Table
-from rich.theme import Theme
-
-info_theme = Theme(
-    {
-        "data": "#999966",
-        "proj": "#8A2BE2",
-        "comp": "#32CD32",
-        "base": "#6495ED",
-    }
-)
 
 
 def get_third_party_imports(root: Path, ns: str, project_data: dict) -> dict:
     bases = {b for b in project_data.get("bases", [])}
     components = {c for c in project_data.get("components", [])}
 
     bases_paths = workspace.paths.collect_bases_paths(root, ns, bases)
@@ -52,15 +43,15 @@
     imports = flatten_brick_imports(brick_imports)
     unknown_imports = imports.difference(deps)
 
     return filter_close_matches(unknown_imports, deps)
 
 
 def print_libs_summary(brick_imports: dict, project_data: dict) -> None:
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
 
     name = project_data["name"]
     is_project = info.is_project(project_data)
 
     printable_name = f"[proj]{name}[/]" if is_project else "[data]development[/]"
     console.print(
         Padding(f"[data]Libraries summary for [/]{printable_name}", (1, 0, 1, 0))
@@ -78,15 +69,15 @@
 def print_libs_in_bricks(brick_imports: dict) -> None:
     bases_imports = flatten_imports(brick_imports, "bases")
     components_imports = flatten_imports(brick_imports, "components")
 
     if not bases_imports and not components_imports:
         return
 
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
     table = Table(box=box.SIMPLE_HEAD)
 
     bases = brick_imports.get("bases", {})
     components = brick_imports.get("components", {})
 
     table.add_column("[data]brick[/]")
     table.add_column("[data]libraries[/]")
@@ -104,15 +95,15 @@
     brick_imports: dict, third_party_libs: Set[str], project_name: str
 ) -> bool:
     diff = calculate_diff(brick_imports, third_party_libs)
 
     if not diff:
         return True
 
-    console = Console(theme=info_theme)
+    console = Console(theme=theme.poly_theme)
 
     missing = ", ".join(sorted(diff))
 
     console.print(
         f"[data]Could not locate all libraries in [/][proj]{project_name}[/]. [data]Caused by missing dependencies?[/]"
     )
```

### Comparing `poetry_polylith_plugin-1.5.2/polylith/libs/stdlib.py` & `poetry_polylith_plugin-1.6.0/polylith/libs/stdlib.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/__init__.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from polylith.poetry.commands.create_base import CreateBaseCommand
 from polylith.poetry.commands.create_component import CreateComponentCommand
 from polylith.poetry.commands.create_project import CreateProjectCommand
 from polylith.poetry.commands.create_workspace import CreateWorkspaceCommand
 from polylith.poetry.commands.diff import DiffCommand
 from polylith.poetry.commands.info import InfoCommand
 from polylith.poetry.commands.libs import LibsCommand
+from polylith.poetry.commands.sync import SyncCommand
 
 __all__ = [
     "CheckCommand",
     "CreateBaseCommand",
     "CreateComponentCommand",
     "CreateProjectCommand",
     "CreateWorkspaceCommand",
     "DiffCommand",
     "InfoCommand",
     "LibsCommand",
+    "SyncCommand",
 ]
```

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/check.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/check.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create_base.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_base.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create_component.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_component.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create_project.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_project.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/create_workspace.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/create_workspace.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/diff.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/diff.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/info.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/info.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry/commands/libs.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry/commands/libs.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/poetry_plugin/plugin.py` & `poetry_polylith_plugin-1.6.0/polylith/poetry_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
     CreateBaseCommand,
     CreateComponentCommand,
     CreateProjectCommand,
     CreateWorkspaceCommand,
     DiffCommand,
     InfoCommand,
     LibsCommand,
+    SyncCommand,
 )
 
 commands = [
     CheckCommand,
     CreateBaseCommand,
     CreateComponentCommand,
     CreateProjectCommand,
     CreateWorkspaceCommand,
     DiffCommand,
     InfoCommand,
     LibsCommand,
+    SyncCommand,
 ]
 
 
 def register_command(application: Application, command) -> None:
     application.command_loader.register_factory(command.name, command)
```

### Comparing `poetry_polylith_plugin-1.5.2/polylith/project/create.py` & `poetry_polylith_plugin-1.6.0/polylith/project/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/project/get.py` & `poetry_polylith_plugin-1.6.0/polylith/project/get.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     return data["tool"]["poetry"].get("packages", [])
 
 
 def get_project_name(data) -> str:
     return data["tool"]["poetry"]["name"]
 
 
-def get_toml(root: Path) -> tomlkit.TOMLDocument:
-    with root.open(encoding="utf-8", errors="ignore") as f:
+def get_toml(path: Path) -> tomlkit.TOMLDocument:
+    with path.open(encoding="utf-8", errors="ignore") as f:
         return tomlkit.loads(f.read())
 
 
 def get_project_files(root: Path) -> dict:
     projects = sorted(root.glob(f"projects/**/{default_toml}"))
     development = Path(root / default_toml)
```

### Comparing `poetry_polylith_plugin-1.5.2/polylith/readme/readme.py` & `poetry_polylith_plugin-1.6.0/polylith/readme/readme.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/repo/repo.py` & `poetry_polylith_plugin-1.6.0/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/test/tests.py` & `poetry_polylith_plugin-1.6.0/polylith/test/tests.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/workspace/create.py` & `poetry_polylith_plugin-1.6.0/polylith/workspace/create.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/workspace/parser.py` & `poetry_polylith_plugin-1.6.0/polylith/workspace/parser.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/polylith/workspace/paths.py` & `poetry_polylith_plugin-1.6.0/polylith/workspace/paths.py`

 * *Files identical despite different names*

### Comparing `poetry_polylith_plugin-1.5.2/pyproject.toml` & `poetry_polylith_plugin-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-polylith-plugin"
-version = "1.5.2"
+version = "1.6.0"
 description = "A Poetry plugin that adds tooling support for the Polylith Architecture"
 authors = ["David Vujic"]
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 readme = "README.md"
 packages = [
     {include = "polylith"},
```

### Comparing `poetry_polylith_plugin-1.5.2/PKG-INFO` & `poetry_polylith_plugin-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-polylith-plugin
-Version: 1.5.2
+Version: 1.6.0
 Summary: A Poetry plugin that adds tooling support for the Polylith Architecture
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 Author: David Vujic
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

