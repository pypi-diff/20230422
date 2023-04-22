# Comparing `tmp/corallium-0.2.0.tar.gz` & `tmp/corallium-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corallium-0.2.0.tar", max compression
+gzip compressed data, was "corallium-0.2.1.tar", max compression
```

## Comparing `corallium-0.2.0.tar` & `corallium-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1066 2023-04-08 17:23:14.679517 corallium-0.2.0/LICENSE
--rw-r--r--   0        0        0      505 2023-04-22 05:19:47.212966 corallium-0.2.0/corallium/__init__.py
--rw-r--r--   0        0        0     8449 2023-04-22 05:00:10.595599 corallium-0.2.0/corallium/file_helpers.py
--rw-r--r--   0        0        0     3671 2023-02-25 15:48:42.282044 corallium-0.2.0/corallium/log.py
--rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-0.2.0/corallium/loggers/__init__.py
--rw-r--r--   0        0        0      526 2023-04-22 04:53:47.931473 corallium-0.2.0/corallium/loggers/plain_printer.py
--rw-r--r--   0        0        0     2109 2023-04-08 00:00:16.873929 corallium-0.2.0/corallium/loggers/rich_printer.py
--rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-0.2.0/corallium/loggers/structlog_logger/__init__.py
--rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-0.2.0/corallium/loggers/structlog_logger/_structlog_logger.py
--rw-r--r--   0        0        0     2122 2023-02-25 16:07:54.214330 corallium-0.2.0/corallium/loggers/styles.py
--rw-r--r--   0        0        0     4486 2023-04-22 05:00:46.991583 corallium-0.2.0/corallium/pretty_process.py
--rw-r--r--   0        0        0     2493 2023-04-07 23:59:07.213515 corallium-0.2.0/corallium/shell.py
--rw-r--r--   0        0        0      192 2023-02-22 03:38:37.960591 corallium-0.2.0/corallium/tomllib.py
--rw-r--r--   0        0        0     2833 2023-04-22 05:19:52.786277 corallium-0.2.0/docs/README.md
--rw-r--r--   0        0        0     1586 2023-04-22 05:19:47.228674 corallium-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 corallium-0.2.0/setup.py
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 corallium-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-08 17:23:14.679517 corallium-0.2.1/LICENSE
+-rw-r--r--   0        0        0      505 2023-04-22 15:34:34.274654 corallium-0.2.1/corallium/__init__.py
+-rw-r--r--   0        0        0     8688 2023-04-22 15:33:16.021263 corallium-0.2.1/corallium/file_helpers.py
+-rw-r--r--   0        0        0     3671 2023-02-25 15:48:42.282044 corallium-0.2.1/corallium/log.py
+-rw-r--r--   0        0        0        0 2023-02-23 12:18:48.616595 corallium-0.2.1/corallium/loggers/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-22 04:53:47.931473 corallium-0.2.1/corallium/loggers/plain_printer.py
+-rw-r--r--   0        0        0     2109 2023-04-08 00:00:16.873929 corallium-0.2.1/corallium/loggers/rich_printer.py
+-rw-r--r--   0        0        0      274 2023-04-22 04:52:34.549543 corallium-0.2.1/corallium/loggers/structlog_logger/__init__.py
+-rw-r--r--   0        0        0      758 2023-04-22 04:57:25.576582 corallium-0.2.1/corallium/loggers/structlog_logger/_structlog_logger.py
+-rw-r--r--   0        0        0     2122 2023-02-25 16:07:54.214330 corallium-0.2.1/corallium/loggers/styles.py
+-rw-r--r--   0        0        0     4486 2023-04-22 05:00:46.991583 corallium-0.2.1/corallium/pretty_process.py
+-rw-r--r--   0        0        0     2493 2023-04-22 07:02:25.379564 corallium-0.2.1/corallium/shell.py
+-rw-r--r--   0        0        0      192 2023-02-22 03:38:37.960591 corallium-0.2.1/corallium/tomllib.py
+-rw-r--r--   0        0        0     2833 2023-04-22 15:34:38.535754 corallium-0.2.1/docs/README.md
+-rw-r--r--   0        0        0     1586 2023-04-22 15:34:34.284201 corallium-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3769 1970-01-01 00:00:00.000000 corallium-0.2.1/setup.py
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 corallium-0.2.1/PKG-INFO
```

### Comparing `corallium-0.2.0/LICENSE` & `corallium-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corallium-0.2.0/corallium/file_helpers.py` & `corallium-0.2.1/corallium/file_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 """mkdocs.yml Path."""
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Read General Text Files
 
 
 @beartype
-def read_lines(path_file: Path) -> List[str]:
+def read_lines(path_file: Path, encoding: Optional[str] = 'utf-8', errors: Optional[str] = None) -> List[str]:
     """Read a file and split on newlines for later parsing.
 
     Args:
         path_file: path to the file
+        encoding: defaults to 'utf-8'
+        encoding: defaults to None, Use 'ignore' if needed'
 
     Returns:
         List[str]: lines of text as list
 
     """
-    return path_file.read_text().splitlines() if path_file.is_file() else []
+    return path_file.read_text(encoding=encoding, errors=errors).splitlines() if path_file.is_file() else []
 
 
 @beartype
 def tail_lines(path_file: Path, *, count: int) -> List[str]:
     """Tail a file for up to the last count (or full file) lines.
 
     Based on: https://stackoverflow.com/a/54278929
@@ -109,15 +111,15 @@
     """Read the 'pyproject.toml' file once."""
     toml_path = find_in_parents(name='pyproject.toml', cwd=cwd)
     try:
         pyproject_txt = toml_path.read_text(encoding='utf-8')
     except Exception as exc:
         msg = f'Could not locate: {toml_path}'
         raise RuntimeError(msg) from exc
-    return tomllib.loads(pyproject_txt)
+    return tomllib.loads(pyproject_txt)  # pyright: ignore[reportGeneralTypeIssues]
 
 
 @lru_cache(maxsize=5)
 @beartype
 def read_package_name(cwd: Optional[Path] = None) -> str:
     """Read the package name once."""
     poetry_config = read_pyproject(cwd=cwd)
```

### Comparing `corallium-0.2.0/corallium/log.py` & `corallium-0.2.1/corallium/log.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.0/corallium/loggers/plain_printer.py` & `corallium-0.2.1/corallium/loggers/plain_printer.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.0/corallium/loggers/rich_printer.py` & `corallium-0.2.1/corallium/loggers/rich_printer.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.0/corallium/loggers/structlog_logger/_structlog_logger.py` & `corallium-0.2.1/corallium/loggers/structlog_logger/_structlog_logger.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.0/corallium/loggers/styles.py` & `corallium-0.2.1/corallium/loggers/styles.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.0/corallium/pretty_process.py` & `corallium-0.2.1/corallium/pretty_process.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.0/corallium/shell.py` & `corallium-0.2.1/corallium/shell.py`

 * *Files identical despite different names*

### Comparing `corallium-0.2.0/docs/README.md` & `corallium-0.2.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `corallium-0.2.0/pyproject.toml` & `corallium-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "0.2.0"
+version = "0.2.1"
 version_files = ["corallium/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
@@ -22,15 +22,15 @@
 include = ["LICENSE"]
 keywords = []
 license = "MIT"
 maintainers = []
 name = "corallium"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/corallium"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 beartype = ">=0.12.0"
 pydantic = ">=1.10.4"
 rich = ">=12.6.0"
 tomli = {markers = "python_version < '3.11'", version = ">=2.0.1"}
```

### Comparing `corallium-0.2.0/setup.py` & `corallium-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['beartype>=0.12.0', 'pydantic>=1.10.4', 'rich>=12.6.0']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1']}
 
 setup_kwargs = {
     'name': 'corallium',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'Shared functionality for calcipy-ecosystem',
     'long_description': '# corallium\n\nShared functionality for the calcipy-ecosystem.\n\n## Installation\n\n1. `poetry add corallium`\n\n1. Take advantage of the logger or other common functionality\n\n    ```sh\n    form corallium.log import logger\n\n    logger.info(\'Hello!\')\n    ```\n\n## Usage\n\n<!-- < TODO: Show an example (screenshots, terminal recording, etc.) >\n\n- **log**: TBD\n- **pretty_process**: TBD\n- **shell**: TBD\n- **file_helpers**: TBD\n- **tomllib**: This is a lightweight wrapper to backport `tomli` in place of `tomllib` until we can use Python >3.11. Use with `from corallium.tomllib import tomllib`\n- **dot_dict**: has one function `ddict`, which is a light-weight wrapper around whatever is the most [maintained dotted-dictionary package in Python](https://pypi.org/search/?q=dot+accessible+dictionary&o=). Dotted dictionaries can sometimes improve code readability, but they aren\'t a one-size fits all solution. Sometimes `attr.s` or `dataclass` are more appropriate.\n    - The benefit of this wrapper is a stable interface that can be replaced with better internal implementations, such [Bunch](https://pypi.org/project/bunch/), [Chunk](https://pypi.org/project/chunk/), [Munch](https://pypi.org/project/munch/), [flexible-dotdict](https://pypi.org/project/flexible-dotdict/), [classy-json](https://pypi.org/project/classy-json/), and now [Python-Box](https://pypi.org/project/python-box/)\n -->\n\nFor more example code, see the [scripts] directory or the [tests].\n\n## Project Status\n\nSee the `Open Issues` and/or the [CODE_TAG_SUMMARY]. For release history, see the [CHANGELOG].\n\n## Contributing\n\nWe welcome pull requests! For your pull request to be accepted smoothly, we suggest that you first open a GitHub issue to discuss your idea. For resources on getting started with the code base, see the below documentation:\n\n- [DEVELOPER_GUIDE]\n- [STYLE_GUIDE]\n\n## Code of Conduct\n\nWe follow the [Contributor Covenant Code of Conduct][contributor-covenant].\n\n### Open Source Status\n\nWe try to reasonably meet most aspects of the "OpenSSF scorecard" from [Open Source Insights](https://deps.dev/pypi/corallium)\n\n## Responsible Disclosure\n\nIf you have any security issue to report, please contact the project maintainers privately. You can reach us at [dev.act.kyle@gmail.com](mailto:dev.act.kyle@gmail.com).\n\n## License\n\n[LICENSE]\n\n[changelog]: https://corallium.kyleking.me/docs/CHANGELOG\n[code_tag_summary]: https://corallium.kyleking.me/docs/CODE_TAG_SUMMARY\n[contributor-covenant]: https://www.contributor-covenant.org\n[developer_guide]: https://corallium.kyleking.me/docs/DEVELOPER_GUIDE\n[license]: https://github.com/kyleking/corallium/blob/main/LICENSE\n[scripts]: https://github.com/kyleking/corallium/blob/main/scripts\n[style_guide]: https://corallium.kyleking.me/docs/STYLE_GUIDE\n[tests]: https://github.com/kyleking/corallium/blob/main/tests\n',
     'author': 'Kyle King',
     'author_email': 'dev.act.kyle@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyleking/corallium',
```

### Comparing `corallium-0.2.0/PKG-INFO` & `corallium-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corallium
-Version: 0.2.0
+Version: 0.2.1
 Summary: Shared functionality for calcipy-ecosystem
 Home-page: https://github.com/kyleking/corallium
 License: MIT
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

