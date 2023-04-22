# Comparing `tmp/bigxml-0.8.0.tar.gz` & `tmp/bigxml-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigxml-0.8.0.tar", last modified: Sun Aug 28 09:22:36 2022, max compression
+gzip compressed data, was "bigxml-0.9.0.tar", last modified: Sun Nov  6 15:41:06 2022, max compression
```

## Comparing `bigxml-0.8.0.tar` & `bigxml-0.9.0.tar`

### file list

```diff
@@ -1,92 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.168197 bigxml-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-08-28 09:22:29.000000 bigxml-0.8.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.136196 bigxml-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.148197 bigxml-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2022-08-28 09:22:29.000000 bigxml-0.8.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-28 09:22:29.000000 bigxml-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-28 09:22:29.000000 bigxml-0.8.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-28 09:22:29.000000 bigxml-0.8.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-08-28 09:22:29.000000 bigxml-0.8.0/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.152197 bigxml-0.8.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-28 09:22:29.000000 bigxml-0.8.0/.vscode/env
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-28 09:22:29.000000 bigxml-0.8.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-08-28 09:22:29.000000 bigxml-0.8.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)     5964 2022-08-28 09:22:29.000000 bigxml-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-08-28 09:22:29.000000 bigxml-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-08-28 09:22:36.168197 bigxml-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-08-28 09:22:29.000000 bigxml-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-08-28 09:22:29.000000 bigxml-0.8.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.152197 bigxml-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.160197 bigxml-0.8.0/docs/src/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.160197 bigxml-0.8.0/docs/src/css/
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/decorators.md
--rw-r--r--   0 runner    (1001) docker     (121)     1981 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/encodings.md
--rw-r--r--   0 runner    (1001) docker     (121)     4834 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/faq.md
--rw-r--r--   0 runner    (1001) docker     (121)     6978 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/handlers.md
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     5080 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/namespaces.md
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/nodes.md
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/parser.md
--rw-r--r--   0 runner    (1001) docker     (121)     5752 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (121)     7927 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/recipes.md
--rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/streams.md
--rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-08-28 09:22:29.000000 bigxml-0.8.0/docs/src/typing.md
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-08-28 09:22:29.000000 bigxml-0.8.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-08-28 09:22:29.000000 bigxml-0.8.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-08-28 09:22:36.168197 bigxml-0.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)       81 2022-08-28 09:22:29.000000 bigxml-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.140196 bigxml-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.160197 bigxml-0.8.0/src/bigxml/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5638 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/handle_mgr.py
--rw-r--r--   0 runner    (1001) docker     (121)     7405 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/handler_creator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3973 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/handler_marker.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/marks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3870 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)     1577 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-08-28 09:22:29.000000 bigxml-0.8.0/src/bigxml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.164197 bigxml-0.8.0/src/bigxml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-08-28 09:22:36.000000 bigxml-0.8.0/src/bigxml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-08-28 09:22:36.000000 bigxml-0.8.0/src/bigxml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-28 09:22:36.000000 bigxml-0.8.0/src/bigxml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-08-28 09:22:36.000000 bigxml-0.8.0/src/bigxml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-28 09:22:36.000000 bigxml-0.8.0/src/bigxml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.140196 bigxml-0.8.0/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.164197 bigxml-0.8.0/stubs/defusedxml/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-08-28 09:22:29.000000 bigxml-0.8.0/stubs/defusedxml/ElementTree.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-28 09:22:29.000000 bigxml-0.8.0/stubs/defusedxml/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.164197 bigxml-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.164197 bigxml-0.8.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (121)     2321 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/test_maths.py
--rw-r--r--   0 runner    (1001) docker     (121)     3639 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/test_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/test_ram_usage.py
--rw-r--r--   0 runner    (1001) docker     (121)     3429 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/test_security.py
--rw-r--r--   0 runner    (1001) docker     (121)     9505 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/test_wikipedia_export.py
--rw-r--r--   0 runner    (1001) docker     (121)   118848 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/integration/wikipedia_python_export.xml.xz
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 09:22:36.168197 bigxml-0.8.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_handle_mgr.py
--rw-r--r--   0 runner    (1001) docker     (121)    25764 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_handler_creator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_handler_marker.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_marks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_nodes_element_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_nodes_element_get_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     5464 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5865 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_utils_autostart_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_utils_extract_namespace_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_utils_get_mandatory_params.py
--rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_utils_iter_with_rollback.py
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-08-28 09:22:29.000000 bigxml-0.8.0/tests/unit/test_utils_iterable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1084 2022-08-28 09:22:29.000000 bigxml-0.8.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.818158 bigxml-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-06 15:41:00.000000 bigxml-0.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.790156 bigxml-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.794156 bigxml-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-11-06 15:41:00.000000 bigxml-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-06 15:41:00.000000 bigxml-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-11-06 15:41:00.000000 bigxml-0.9.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-06 15:41:00.000000 bigxml-0.9.0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-11-06 15:41:00.000000 bigxml-0.9.0/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.798156 bigxml-0.9.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (121)       86 2022-11-06 15:41:00.000000 bigxml-0.9.0/.vscode/env
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-11-06 15:41:00.000000 bigxml-0.9.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-11-06 15:41:00.000000 bigxml-0.9.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (121)     6608 2022-11-06 15:41:00.000000 bigxml-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-06 15:41:00.000000 bigxml-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-11-06 15:41:06.818158 bigxml-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-11-06 15:41:00.000000 bigxml-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-06 15:41:00.000000 bigxml-0.9.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.798156 bigxml-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     2040 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.802157 bigxml-0.9.0/docs/src/
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.802157 bigxml-0.9.0/docs/src/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      977 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/encodings.md
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4834 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/faq.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6979 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/handlers.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2573 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/index.md
+-rw-r--r--   0 runner    (1001) docker     (121)     5080 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/namespaces.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/nodes.md
+-rw-r--r--   0 runner    (1001) docker     (121)      560 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/parser.md
+-rw-r--r--   0 runner    (1001) docker     (121)     5751 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (121)     7927 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/recipes.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1493 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/streams.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3482 2022-11-06 15:41:00.000000 bigxml-0.9.0/docs/src/typing.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-06 15:41:00.000000 bigxml-0.9.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-11-06 15:41:00.000000 bigxml-0.9.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-11-06 15:41:06.818158 bigxml-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)       81 2022-11-06 15:41:00.000000 bigxml-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.790156 bigxml-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.806157 bigxml-0.9.0/src/bigxml/
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5835 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/handle_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7405 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/handler_creator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3973 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/handler_marker.py
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/marks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3870 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2591 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-11-06 15:41:00.000000 bigxml-0.9.0/src/bigxml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.806157 bigxml-0.9.0/src/bigxml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2494 2022-11-06 15:41:06.000000 bigxml-0.9.0/src/bigxml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-11-06 15:41:06.000000 bigxml-0.9.0/src/bigxml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-06 15:41:06.000000 bigxml-0.9.0/src/bigxml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       71 2022-11-06 15:41:06.000000 bigxml-0.9.0/src/bigxml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-06 15:41:06.000000 bigxml-0.9.0/src/bigxml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.790156 bigxml-0.9.0/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.810157 bigxml-0.9.0/stubs/defusedxml/
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-11-06 15:41:00.000000 bigxml-0.9.0/stubs/defusedxml/ElementTree.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-06 15:41:00.000000 bigxml-0.9.0/stubs/defusedxml/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.810157 bigxml-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.814158 bigxml-0.9.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/test_invalid_xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1879 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/test_maths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3639 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/test_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1832 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/test_ram_usage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3825 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9335 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/test_wikipedia_export.py
+-rw-r--r--   0 runner    (1001) docker     (121)   118848 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/integration/wikipedia_python_export.xml.xz
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-06 15:41:06.818158 bigxml-0.9.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1459 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_handle_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25711 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_handler_creator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_handler_marker.py
+-rw-r--r--   0 runner    (1001) docker     (121)      543 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_marks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2210 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_nodes_element_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_nodes_element_get_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5460 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5865 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_utils_autostart_generator.py
+-rw-r--r--   0 runner    (1001) docker     (121)      396 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_utils_extract_namespace_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1484 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_utils_get_mandatory_params.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1744 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_utils_iter_with_rollback.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-11-06 15:41:00.000000 bigxml-0.9.0/tests/unit/test_utils_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-11-06 15:41:00.000000 bigxml-0.9.0/tox.ini
```

### Comparing `bigxml-0.8.0/.github/workflows/build.yml` & `bigxml-0.9.0/.github/workflows/build.yml`

 * *Files 12% similar despite different names*

```diff
@@ -11,110 +11,111 @@
     strategy:
       matrix:
         python:
           - "3.7"
           - "3.8"
           - "3.9"
           - "3.10"
+          - "3.11"
           - "pypy-3.7"
           - "pypy-3.8"
           - "pypy-3.9"
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Setup Python ${{ matrix.python }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Install dependencies
         run: pip install tox
       - name: Run tests
         run: tox -e py
 
   tests-misc:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         env: [type, lint, format]
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install dependencies
         run: pip install tox
       - name: Run ${{ matrix.env }}
         run: tox -e ${{ matrix.env }}
 
   docs:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install dependencies
         run: pip install tox
       - name: Run docs
         run: |
           tox -e docs
           mkdir -p dist
           tar czf dist/docs.tar.gz -C build docs
       - name: Save docs artifacts
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: docs
           path: dist/docs.tar.gz
 
   build:
     needs: [tests-py, tests-misc, docs]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           # fetch all commits for setuptools_scm
           fetch-depth: 0
       - name: Setup Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Build
         run: python setup.py sdist bdist_wheel
       - name: Save build artifacts
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v3
         with:
           name: dist
           path: dist
 
   publish:
     if: startsWith(github.ref, 'refs/tags')
     needs: build
     runs-on: ubuntu-latest
     steps:
       - name: Restore build artifacts
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: dist
           path: dist
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.pypi_password }}
 
   deploy-docs:
     needs: publish
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Restore build artifacts
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: docs
           path: dist
       - name: Extract docs
         run: tar xf dist/docs.tar.gz -C dist
       - name: Deploy docs
-        uses: JamesIves/github-pages-deploy-action@4.1.0
+        uses: JamesIves/github-pages-deploy-action@v4
         with:
           branch: gh-pages
           folder: dist/docs
```

### Comparing `bigxml-0.8.0/.vscode/settings.json` & `bigxml-0.9.0/.vscode/settings.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'python.linting.mypyEnabled'": 'True'}*

```diff
@@ -28,13 +28,14 @@
         ".pytest_cache": true,
         ".tox": true,
         "env": true
     },
     "files.insertFinalNewline": true,
     "python.envFile": "${workspaceFolder}/.vscode/env",
     "python.formatting.provider": "black",
+    "python.linting.mypyEnabled": true,
     "python.linting.pylintEnabled": true,
     "python.sortImports.args": [
         "-sp .isort.cfg"
     ],
     "python.testing.pytestEnabled": true
 }
```

### Comparing `bigxml-0.8.0/CHANGELOG.md` & `bigxml-0.9.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,37 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/), and this project
 adheres to [Semantic Versioning](https://semver.org/).
 
+## [0.9.0] - 2022-11-06
+
+[0.9.0]: https://github.com/rogdham/bigxml/compare/v0.8.0...v0.9.0
+
+v0.9.0 introduces custom exceptions.
+
+### :boom: Breaking changes
+
+- All exceptions raised due to invalid stream content are now instances of
+  `BigXmlException` instead of `xml.etree.ElementTree.ParseError` or
+  `defusedxml.DefusedXmlException`.
+
+### :bug: Fixes
+
+- Add a workaround against pylint `not-an-iterable` false-positive on `iter_from`
+
+### :house: Internal
+
+- Necessary code changes following dev dependency update: mypy, pylint, pytest
+- Add tests for CPython 3.11
+- Use CPython 3.11 for misc. tests
+- Update Github actions dependencies
+
 ## [0.8.0] - 2022-08-28
 
 [0.8.0]: https://github.com/rogdham/bigxml/compare/v0.7.0...v0.8.0
 
 v0.8.0 brings type hints!
 
 ### :boom: Breaking changes
```

### Comparing `bigxml-0.8.0/LICENSE.txt` & `bigxml-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/PKG-INFO` & `bigxml-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigxml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pythonic xml parser to handle big files or streams
 Home-page: https://github.com/rogdham/bigxml
 Author: Rogdham
 Author-email: contact@rogdham.net
 License: MIT
 Project-URL: Documentation, https://bigxml.rogdham.net/
 Project-URL: Source, https://github.com/rogdham/bigxml
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <div align="center" size="15px">
```

### Comparing `bigxml-0.8.0/README.md` & `bigxml-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/docs/conftest.py` & `bigxml-0.9.0/docs/conftest.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/docs/mkdocs.yml` & `bigxml-0.9.0/docs/mkdocs.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 site_name: BigXML
 site_description: Parse big xml files and streams with ease
 site_author: Rogdham
 repo_url: https://github.com/rogdham/bigxml
 site_url: https://bigxml.rogdham.net/
+edit_uri: blob/master/docs/src
 docs_dir: src
 site_dir: ../build/docs
 nav:
   - Home: index.md
   - User guide:
       - Quickstart: quickstart.md
       - Recipes: recipes.md
@@ -16,14 +17,15 @@
       - FAQ: faq.md
   - API reference:
       - Parser: parser.md
       - Streams: streams.md
       - Handlers: handlers.md
       - Decorators: decorators.md
       - Nodes: nodes.md
+      - Exceptions: exceptions.md
   - External Links:
       - Changelog: https://github.com/rogdham/bigxml/blob/master/CHANGELOG.md
       - Issue tracker: https://github.com/rogdham/bigxml/issues
       - BigXML @ GitHub: https://github.com/rogdham/bigxml
       - BigXML @ PyPI: https://pypi.org/project/bigxml
 theme: readthedocs
 extra_css:
```

### Comparing `bigxml-0.8.0/docs/src/css/extra.css` & `bigxml-0.9.0/docs/src/css/extra.css`

 * *Files 14% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 
 .wy-menu > .caption {
   text-align: center;
 }
 .wy-menu > ul {
   margin-bottom: 32px;
 }
+.wy-menu-vertical li.toctree-l1.current > a button {
+    display: none;
+}
 
 footer {
   visibility: hidden;
 }
 footer div {
   visibility: visible;
 }
```

### Comparing `bigxml-0.8.0/docs/src/decorators.md` & `bigxml-0.9.0/docs/src/decorators.md`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/docs/src/encodings.md` & `bigxml-0.9.0/docs/src/encodings.md`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     ...     yield node.text
 
     >>> stream_bytes = b"<root>\xe0\xe9\xef\xf4\xf9</root>"  # ISO-8859-1
 
     >>> Parser(stream_bytes).return_from(handler)
     Traceback (most recent call last):
         ...
-    xml.etree.ElementTree.ParseError: not well-formed (invalid token)...
+    bigxml.exceptions.BigXmlException: Not well-formed (invalid token)...
 
 If you know that there is no XML declaration, you can add one before the stream:
 
     :::python
     >>> Parser(
     ...    "<?xml version='1.0' encoding='ISO-8859-1'?>".encode("ISO-8859-1"),
     ...    stream_bytes,
```

### Comparing `bigxml-0.8.0/docs/src/faq.md` & `bigxml-0.9.0/docs/src/faq.md`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/docs/src/handlers.md` & `bigxml-0.9.0/docs/src/handlers.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ...         print(f"{ean} ({kind})")
     9780261103573 (book)
     5702014975200 (toy)
     0883929452996 (dvd)
 
 !!! Note
 
-    To handle different kind of nodes at once, the same function can be decorated
+    To handle different kinds of nodes at once, the same function can be decorated
     several times with `xml_handle_element` or `xml_handle_text` as shown above.
 
 ## Classes
 
 Passing a class as a handler is a good way to group the handling of a node and its
 children.
```

### Comparing `bigxml-0.8.0/docs/src/index.md` & `bigxml-0.9.0/docs/src/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 As a general rule, all Python versions that are both [released and still officially
 supported][python-versions] are supported by `bigxml` and tested against (both CPython
 and PyPy implementations).
 
 If you have other use cases or find issues with some Python versions, feel free to
 [open a ticket](https://github.com/Rogdham/bigxml/issues/new)!
 
-[python-versions]: https://devguide.python.org/#status-of-python-branches
+[python-versions]: https://devguide.python.org/versions/#supported-versions
 
 ## Status of the project
 
 _BigXML_ is currently in **beta**. It is well tested, and the API should not change
 drastically but breaking changes may still occur in future releases. Changes are well
 detailed in the [changelog], and the version numbering follow [semver].
```

### Comparing `bigxml-0.8.0/docs/src/namespaces.md` & `bigxml-0.9.0/docs/src/namespaces.md`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/docs/src/nodes.md` & `bigxml-0.9.0/docs/src/nodes.md`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/docs/src/parser.md` & `bigxml-0.9.0/docs/src/parser.md`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/docs/src/quickstart.md` & `bigxml-0.9.0/docs/src/quickstart.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 Say we want to get the comics' titles. To do so, we will create a handler function. We
 pass the path to the `title` XML elements we are interested in as arguments of the
 `xml_handle_element` decorator:
 
     :::python
     >>> @xml_handle_element("feed", "entry", "title")
     ... def handler(node):
-    ...     yield node.text  # node contents as a str
+    ...     yield node.text  # node content as a str
 
 Next, we need to instantiate a `Parser` with a stream. In our case, we have the atom
 feed saved into a file, so we pass the file object.
 
 Finally, we call `iter_from` to obtain an iterator that will get though all the items
 yielded by the handler:
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 that into an `atom.xml` file (we will learn to parse HTTP responses in
 streaming later). Make sure you have [_BigXML_ installed]
 (index.md#installation) so that you can follow along. ## Getting nodes and data
 Say we want to get the comics' titles. To do so, we will create a handler
 function. We pass the path to the `title` XML elements we are interested in as
 arguments of the `xml_handle_element` decorator: :::python >>>
 @xml_handle_element("feed", "entry", "title") ... def handler(node): ... yield
-node.text # node contents as a str Next, we need to instantiate a `Parser` with
+node.text # node content as a str Next, we need to instantiate a `Parser` with
 a stream. In our case, we have the atom feed saved into a file, so we pass the
 file object. Finally, we call `iter_from` to obtain an iterator that will get
 though all the items yielded by the handler: :::python >>> with open
 ("atom.xml", "rb") as f: ... for item in Parser(f).iter_from(handler): ...
 print(item) Solar System Cartogram Siri Post-Vaccine Party Circles ## Accessing
 attributes Now, we will get the links to the comics. This time, we are
 interested in the value of the `href` attribute of the `link` elements: :::
```

### Comparing `bigxml-0.8.0/docs/src/recipes.md` & `bigxml-0.9.0/docs/src/recipes.md`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/docs/src/streams.md` & `bigxml-0.9.0/docs/src/streams.md`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/docs/src/typing.md` & `bigxml-0.9.0/docs/src/typing.md`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/mypy.ini` & `bigxml-0.9.0/mypy.ini`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Import discovery
 files = src
 ignore_missing_imports = False
 follow_imports = normal
 mypy_path = stubs,src
 
 # Platform configuration
-python_version = 3.10
+python_version = 3.11
 
 # Disallow dynamic typing
 disallow_any_unimported = True
 disallow_any_decorated = True
 disallow_any_generics = True
 disallow_subclassing_any = True
```

### Comparing `bigxml-0.8.0/setup.cfg` & `bigxml-0.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Utilities
 	Topic :: Text Processing :: Markup :: XML
 
 [options]
 include_package_data = True
 package_dir = =src
 packages = bigxml
```

### Comparing `bigxml-0.8.0/src/bigxml/handle_mgr.py` & `bigxml-0.9.0/src/bigxml/handle_mgr.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,18 @@
 
     # iter_from
 
     @overload
     def iter_from(
         self,
     ) -> Iterator["Never"]:
-        ...
+        # we don't have '...' as body in this overload as a workaround
+        # to prevent 'not-an-iterable' error in pylint
+        # see https://github.com/PyCQA/astroid/issues/1015
+        return iter(())
 
     @overload
     def iter_from(
         self,
         *handlers: Union[
             str,
             List[str],
```

### Comparing `bigxml-0.8.0/src/bigxml/handler_creator.py` & `bigxml-0.9.0/src/bigxml/handler_creator.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/src/bigxml/handler_marker.py` & `bigxml-0.9.0/src/bigxml/handler_marker.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 
 # Also, a lot of the typing complexity comes from the fact that
 # decorators can be applied on both functions, methods & staticmethods
 # plus xml_handle_text can be applied without parenthesis as well
 
 
 class ___xml_handle_xxx_wrapped(Protocol[T_co]):  # pylint: disable=invalid-name
+    # wrapper for classes
+    @overload
+    def __call__(
+        self,
+        obj: K,
+    ) -> K:
+        ...
+
     # wrapper for functions
     @overload
     def __call__(
         self,
         obj: Callable[[T_co], Optional[Iterable[T]]],
     ) -> Callable[[Union[XMLElement, XMLText]], Optional[Iterable[T]]]:
         ...
@@ -28,22 +36,14 @@
     @overload
     def __call__(
         self,
         obj: Callable[[U, T_co], Optional[Iterable[T]]],
     ) -> Callable[[U, Union[XMLElement, XMLText]], Optional[Iterable[T]]]:
         ...
 
-    # wrapper for classes
-    @overload
-    def __call__(
-        self,
-        obj: K,
-    ) -> K:
-        ...
-
 
 def xml_handle_element(*args: str) -> ___xml_handle_xxx_wrapped[XMLElement]:
     if not args:
         raise TypeError("Call to xml_handle_element without any args")
 
     def wrapper(obj: F) -> F:
         markable = obj
@@ -59,14 +59,22 @@
 
     return cast(
         ___xml_handle_xxx_wrapped[XMLElement],
         wrapper,
     )
 
 
+# @xml_handle_text (for classes)
+@overload
+def xml_handle_text(
+    obj: K,
+) -> K:
+    ...
+
+
 # @xml_handle_text (for functions)
 @overload
 def xml_handle_text(
     obj: Callable[[XMLText], Optional[Iterable[T]]],
 ) -> Callable[[Union[XMLElement, XMLText]], Optional[Iterable[T]]]:
     ...
 
@@ -75,22 +83,14 @@
 @overload
 def xml_handle_text(
     obj: Callable[[U, XMLText], Optional[Iterable[T]]],
 ) -> Callable[[U, Union[XMLElement, XMLText]], Optional[Iterable[T]]]:
     ...
 
 
-# @xml_handle_text (for classes)
-@overload
-def xml_handle_text(
-    obj: K,
-) -> K:
-    ...
-
-
 # @xml_handle_text(...) (for functions & methods)
 @overload
 def xml_handle_text(*args: str) -> ___xml_handle_xxx_wrapped[XMLText]:
     ...
 
 
 def xml_handle_text(*args: Any, **_kwargs: Any) -> Any:
```

### Comparing `bigxml-0.8.0/src/bigxml/nodes.py` & `bigxml-0.9.0/src/bigxml/nodes.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/src/bigxml/parser.py` & `bigxml-0.9.0/src/bigxml/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import TYPE_CHECKING, Callable, Iterator, Optional, Tuple, Union
 
 from defusedxml.ElementTree import iterparse
 
+from bigxml.exceptions import rewrite_exceptions
 from bigxml.handle_mgr import HandleMgr
 from bigxml.nodes import XMLElement, XMLElementAttributes, XMLText
 from bigxml.stream import StreamChain
 from bigxml.typing import Streamable, T
 from bigxml.utils import IterWithRollback
 
 if TYPE_CHECKING:
@@ -67,9 +68,16 @@
 
         else:  # pragma: no cover
             raise RuntimeError  # should not happen
 
 
 class Parser(HandleMgr):
     def __init__(self, *streams: Streamable) -> None:
-        iterator = IterWithRollback(iterparse(StreamChain(*streams), ("start", "end")))
+        iterator = IterWithRollback(
+            rewrite_exceptions(
+                iterparse(
+                    StreamChain(*streams),
+                    ("start", "end"),
+                )
+            )
+        )
         self._handle = lambda h: _parse(iterator, h, (), None, 0)
```

### Comparing `bigxml-0.8.0/src/bigxml/stream.py` & `bigxml-0.9.0/src/bigxml/stream.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/src/bigxml/typing.py` & `bigxml-0.9.0/src/bigxml/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 if sys.version_info < (3, 10):  # pragma: no cover
     from typing_extensions import ParamSpec
 else:  # pragma: no cover
     from typing import ParamSpec
 
 
-# pylint: disable=invalid-name, unused-argument
+# pylint: disable=unused-argument
 
 
 P = ParamSpec("P")
 T = TypeVar("T")
 U = TypeVar("U")
 F = TypeVar("F", bound=Callable[..., Any])
 K = TypeVar("K", bound=Type[Any])
```

### Comparing `bigxml-0.8.0/src/bigxml/utils.py` & `bigxml-0.9.0/src/bigxml/utils.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/src/bigxml.egg-info/PKG-INFO` & `bigxml-0.9.0/src/bigxml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigxml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Pythonic xml parser to handle big files or streams
 Home-page: https://github.com/rogdham/bigxml
 Author: Rogdham
 Author-email: contact@rogdham.net
 License: MIT
 Project-URL: Documentation, https://bigxml.rogdham.net/
 Project-URL: Source, https://github.com/rogdham/bigxml
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: Topic :: Text Processing :: Markup :: XML
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <div align="center" size="15px">
```

### Comparing `bigxml-0.8.0/src/bigxml.egg-info/SOURCES.txt` & `bigxml-0.9.0/src/bigxml.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 .vscode/launch.json
 .vscode/settings.json
 docs/conftest.py
 docs/mkdocs.yml
 docs/src/CNAME
 docs/src/decorators.md
 docs/src/encodings.md
+docs/src/exceptions.md
 docs/src/faq.md
 docs/src/handlers.md
 docs/src/index.md
 docs/src/namespaces.md
 docs/src/nodes.md
 docs/src/parser.md
 docs/src/quickstart.md
 docs/src/recipes.md
 docs/src/streams.md
 docs/src/typing.md
 docs/src/css/extra.css
 src/bigxml/__init__.py
+src/bigxml/exceptions.py
 src/bigxml/handle_mgr.py
 src/bigxml/handler_creator.py
 src/bigxml/handler_marker.py
 src/bigxml/marks.py
 src/bigxml/nodes.py
 src/bigxml/parser.py
 src/bigxml/py.typed
@@ -50,21 +52,23 @@
 src/bigxml.egg-info/top_level.txt
 stubs/defusedxml/ElementTree.pyi
 stubs/defusedxml/__init__.pyi
 tests/conftest.py
 tests/integration/README.md
 tests/integration/test_comments.py
 tests/integration/test_encodings.py
+tests/integration/test_invalid_xml.py
 tests/integration/test_maths.py
 tests/integration/test_namespaces.py
 tests/integration/test_ram_usage.py
 tests/integration/test_security.py
 tests/integration/test_typing.py
 tests/integration/test_wikipedia_export.py
 tests/integration/wikipedia_python_export.xml.xz
+tests/unit/test_exceptions.py
 tests/unit/test_handle_mgr.py
 tests/unit/test_handler_creator.py
 tests/unit/test_handler_marker.py
 tests/unit/test_marks.py
 tests/unit/test_nodes_element_attributes.py
 tests/unit/test_nodes_element_get_text.py
 tests/unit/test_parser.py
```

### Comparing `bigxml-0.8.0/tests/conftest.py` & `bigxml-0.9.0/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,18 @@
 from pathlib import Path
 import sys
-from typing import TYPE_CHECKING, List
+from typing import List
 
 import pytest
 
-if TYPE_CHECKING:
-    # see https://github.com/pytest-dev/pytest/issues/7469
-    # for pytest exporting from pytest and not _pytest
-    from _pytest.config import Config
-    from _pytest.nodes import Item
-
 
 def pytest_collection_modifyitems(
     # pylint: disable=unused-argument
-    config: "Config",
-    items: List["Item"],
+    config: pytest.Config,
+    items: List[pytest.Item],
 ) -> None:
     root = Path(__file__).parent.parent
     for item in items:
         relative = Path(item.fspath).parent.relative_to(root)
         if relative.parent.name == "docs":
             mark = "docs"
         elif relative.parent.name == "tests":
```

### Comparing `bigxml-0.8.0/tests/integration/test_comments.py` & `bigxml-0.9.0/tests/integration/test_comments.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/integration/test_encodings.py` & `bigxml-0.9.0/tests/integration/test_encodings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Iterator
-import xml.etree.ElementTree as ET
 
 import pytest
 
-from bigxml import Parser, XMLElement, xml_handle_element
+from bigxml import BigXmlException, Parser, XMLElement, xml_handle_element
 
 TXT_STR = "aàâæcçeéèêëiïîoôuùûü"
 XML_STR = f"<élément>{TXT_STR}</élément>"
 
 
 @pytest.mark.parametrize(
     "xml",
@@ -63,9 +62,11 @@
 
     assert Parser(xml).return_from(handler) == TXT_STR
 
 
 def test_wrong_explicit_encoding() -> None:
     xml = ("<?xml version='1.0' encoding='ISO-8859-1'?>" + XML_STR).encode("utf_8")
     parser = Parser(xml)
-    with pytest.raises(ET.ParseError):
+    with pytest.raises(BigXmlException) as exc_info:
         parser.return_from()
+    assert str(exc_info.value) == "Not well-formed (invalid token): line 1, column 45"
+    assert not exc_info.value.security
```

### Comparing `bigxml-0.8.0/tests/integration/test_maths.py` & `bigxml-0.9.0/tests/integration/test_maths.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/integration/test_namespaces.py` & `bigxml-0.9.0/tests/integration/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/integration/test_ram_usage.py` & `bigxml-0.9.0/tests/integration/test_ram_usage.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/integration/test_typing.py` & `bigxml-0.9.0/tests/integration/test_typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,14 @@
     from typing_extensions import assert_type
 else:
 
     def assert_type(val: Any, _: Any) -> Any:
         return val
 
 
-# workaround against pylint false-positive
-# see https://github.com/PyCQA/pylint/issues/7368
-assert_type  # pylint: disable=used-before-assignment, pointless-statement
-
-
 # Note: the aim of this file is to test the typing of return-values
 # for iter_from and return_from as they would be used in the wild.
 # As a result, we don't try to factor code or do anything smart here.
 
 
 XML = b"""
 <root>
```

### Comparing `bigxml-0.8.0/tests/integration/test_wikipedia_export.py` & `bigxml-0.9.0/tests/integration/test_wikipedia_export.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/integration/wikipedia_python_export.xml.xz` & `bigxml-0.9.0/tests/integration/wikipedia_python_export.xml.xz`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/unit/test_handle_mgr.py` & `bigxml-0.9.0/tests/unit/test_handle_mgr.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/unit/test_handler_creator.py` & `bigxml-0.9.0/tests/unit/test_handler_creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from bigxml.handler_creator import CLASS_HANDLER_METHOD_NAME, create_handler
 from bigxml.handler_marker import xml_handle_element, xml_handle_text
 from bigxml.nodes import XMLElement, XMLElementAttributes, XMLText
 
 if TYPE_CHECKING:
     # see https://github.com/pytest-dev/pytest/issues/7469
     # for pytest exporting from pytest and not _pytest
-    from _pytest.mark import MarkDecorator, ParameterSet
+    from _pytest.mark import ParameterSet
 
 
 def create_nodes(
     *path: str, parent: Optional[Union[XMLElement, XMLText]] = None
 ) -> List[Union[XMLElement, XMLText]]:
     # create nodes
     nodes = [parent] if parent is not None else []
@@ -65,27 +65,27 @@
         except IndexError:
             pass
 
         # create handle
         def handle(
             handler: Callable[[Union[XMLElement, XMLText]], Iterator[object]],
             children: List[Union[XMLElement, XMLText]],
-        ) -> Iterable[object]:  # pylint: disable=dangerous-default-value
+        ) -> Iterable[object]:
             for child in children:
                 yield from handler(child)
 
         # pylint: disable=protected-access
         node_parent._handle = partial(handle, children=children)  # type: ignore[assignment]
 
     return nodes
 
 
 def cases(
     *args: Tuple[Tuple[str, ...], Optional[str], Optional[str]]
-) -> "MarkDecorator":
+) -> pytest.MarkDecorator:
     tests: List["ParameterSet"] = []
     for node_path, expected_text, expected_node_name in args:
         nodes = create_nodes(*node_path)
         if expected_node_name is None:
             assert expected_text is None
             expected_node = None
         else:
```

### Comparing `bigxml-0.8.0/tests/unit/test_handler_marker.py` & `bigxml-0.9.0/tests/unit/test_handler_marker.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/unit/test_marks.py` & `bigxml-0.9.0/tests/unit/test_marks.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 def test_marks(instanciate: bool) -> None:
     class Markable:
         pass
 
     obj = Markable() if instanciate else Markable
 
     assert not has_marks(obj)
-    assert (
-        # pylint: disable=use-implicit-booleaness-not-comparison
-        get_marks(obj)
-        == ()
-    )
+    assert not get_marks(obj)
 
     add_mark(obj, ("abc",))
     assert has_marks(obj)
     assert get_marks(obj) == (("abc",),)
 
     add_mark(obj, ("def", "ghi", "jkl"))
     assert has_marks(obj)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bigxml-0.8.0/tests/unit/test_nodes_element_attributes.py` & `bigxml-0.9.0/tests/unit/test_nodes_element_attributes.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/unit/test_nodes_element_get_text.py` & `bigxml-0.9.0/tests/unit/test_nodes_element_get_text.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/unit/test_parser.py` & `bigxml-0.9.0/tests/unit/test_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 text_w_node = XMLText("World", (root_node,))
 
 # to make sure that text are not in buffer, we generate huge texts
 BIG_TEXT_LEN = 1_000_000
 
 
 @pytest.mark.parametrize(
-    "xml_contents, nodes",
+    "xml_content, nodes",
     [
         [b"", []],
         [b"Hello", [text_h_node]],
         [b"<foo />", [elem_f_node]],
         [b"Hello<foo />", [text_h_node, elem_f_node]],
         [b"<foo />World", [elem_f_node, text_w_node]],
         [b"Hello<foo />World", [text_h_node, elem_f_node, text_w_node]],
@@ -126,27 +126,27 @@
         "element + text",
         "text + element + text",
         "text + element + text + element + text",
         "depth",
         "big texts",
     ],
 )
-def test_contents(
-    xml_contents: bytes,
+def test_content(
+    xml_content: bytes,
     nodes: List[Union[XMLElement, XMLText]],
     # pylint: disable=redefined-outer-name
     handler: HANDLER_TYPE,
 ) -> None:
     @xml_handle_element("root")
     def root_handler(
         node: XMLElement,
     ) -> Iterator[Tuple[str, Union[XMLElement, XMLText]]]:
         yield from node.iter_from(handler)
 
-    parser = Parser(b"<root>", xml_contents, b"</root>")
+    parser = Parser(b"<root>", xml_content, b"</root>")
     assert list(parser.iter_from(root_handler)) == [
         (f"handler-yield-{i}", node) for i, node in enumerate(nodes)
     ]
 
 
 def test_out_of_order() -> None:
     @xml_handle_element("foo")
```

### Comparing `bigxml-0.8.0/tests/unit/test_stream.py` & `bigxml-0.9.0/tests/unit/test_stream.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/unit/test_utils_autostart_generator.py` & `bigxml-0.9.0/tests/unit/test_utils_autostart_generator.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/unit/test_utils_get_mandatory_params.py` & `bigxml-0.9.0/tests/unit/test_utils_get_mandatory_params.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/unit/test_utils_iter_with_rollback.py` & `bigxml-0.9.0/tests/unit/test_utils_iter_with_rollback.py`

 * *Files identical despite different names*

### Comparing `bigxml-0.8.0/tests/unit/test_utils_iterable.py` & `bigxml-0.9.0/tests/unit/test_utils_iterable.py`

 * *Files identical despite different names*

