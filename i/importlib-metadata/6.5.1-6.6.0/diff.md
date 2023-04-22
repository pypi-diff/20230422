# Comparing `tmp/importlib_metadata-6.5.1.tar.gz` & `tmp/importlib_metadata-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_metadata-6.5.1.tar", last modified: Sat Apr 22 02:51:09 2023, max compression
+gzip compressed data, was "importlib_metadata-6.6.0.tar", last modified: Sat Apr 22 12:56:52 2023, max compression
```

## Comparing `importlib_metadata-6.5.1.tar` & `importlib_metadata-6.6.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.642492 importlib_metadata-6.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.638492 importlib_metadata-6.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.638492 importlib_metadata-6.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21107 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-22 02:51:09.642492 importlib_metadata-6.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.638492 importlib_metadata-6.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/docs/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/exercises.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.638492 importlib_metadata-6.5.1/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    29051 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.638492 importlib_metadata-6.5.1/importlib_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-22 02:51:09.000000 importlib_metadata-6.5.1/importlib_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-22 02:51:09.000000 importlib_metadata-6.5.1/importlib_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 02:51:09.000000 importlib_metadata-6.5.1/importlib_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-22 02:51:09.000000 importlib_metadata-6.5.1/importlib_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 02:51:09.000000 importlib_metadata-6.5.1/importlib_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.622492 importlib_metadata-6.5.1/prepare/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.642492 importlib_metadata-6.5.1/prepare/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.642492 importlib_metadata-6.5.1/prepare/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/prepare/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/prepare/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.642492 importlib_metadata-6.5.1/prepare/example2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.642492 importlib_metadata-6.5.1/prepare/example2/example2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/prepare/example2/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/prepare/example2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-22 02:51:09.642492 importlib_metadata-6.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.642492 importlib_metadata-6.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 02:51:09.642492 importlib_metadata-6.5.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/data/example-21.12-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/data/example-21.12-py3.6.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/data/example2-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/test_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tests/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-22 02:50:48.000000 importlib_metadata-6.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.086147 importlib_metadata-6.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.086147 importlib_metadata-6.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.086147 importlib_metadata-6.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/exercises.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    29949 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/importlib_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 12:56:52.000000 importlib_metadata-6.6.0/importlib_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.082147 importlib_metadata-6.6.0/prepare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/prepare/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/prepare/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/prepare/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/prepare/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/prepare/example2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.090148 importlib_metadata-6.6.0/prepare/example2/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/prepare/example2/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/prepare/example2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:52.094148 importlib_metadata-6.6.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/data/example-21.12-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/data/example-21.12-py3.6.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/data/example2-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tests/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-22 12:56:31.000000 importlib_metadata-6.6.0/tox.ini
```

### Comparing `importlib_metadata-6.5.1/.github/workflows/main.yml` & `importlib_metadata-6.6.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/CHANGES.rst` & `importlib_metadata-6.6.0/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v6.6.0
+======
+
+* #449: Expanded type annotations.
+
 v6.5.1
 ======
 
 * python/cpython#103661: Removed excess error suppression in
   ``_read_files_egginfo_installed`` and fixed path handling
   on Windows.
```

### Comparing `importlib_metadata-6.5.1/LICENSE` & `importlib_metadata-6.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/PKG-INFO` & `importlib_metadata-6.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_metadata
-Version: 6.5.1
+Version: 6.6.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.5.1/README.rst` & `importlib_metadata-6.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/conftest.py` & `importlib_metadata-6.6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/docs/conf.py` & `importlib_metadata-6.6.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         None,
     ),
 )
 
 nitpick_ignore = [
     # Workaround for #316
     ('py:class', 'importlib_metadata.EntryPoints'),
+    ('py:class', 'importlib_metadata.PackagePath'),
     ('py:class', 'importlib_metadata.SelectableGroups'),
     ('py:class', 'importlib_metadata._meta._T'),
     # Workaround for #435
     ('py:class', '_T'),
     # Other workarounds
     ('py:class', 'importlib_metadata.DeprecatedNonAbstract'),
 ]
```

### Comparing `importlib_metadata-6.5.1/docs/index.rst` & `importlib_metadata-6.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/docs/migration.rst` & `importlib_metadata-6.6.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/docs/using.rst` & `importlib_metadata-6.6.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/exercises.py` & `importlib_metadata-6.6.0/exercises.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/importlib_metadata/__init__.py` & `importlib_metadata-6.6.0/importlib_metadata/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import os
 import re
 import abc
 import csv
 import sys
 import zipp
 import email
+import inspect
 import pathlib
 import operator
 import textwrap
 import warnings
 import functools
 import itertools
 import posixpath
 import contextlib
 import collections
-import inspect
 
 from . import _adapters, _meta, _py39compat
 from ._collections import FreezableDefaultDict, Pair
 from ._compat import (
     NullFinder,
+    StrPath,
     install,
     pypy_partial,
 )
 from ._functools import method_cache, pass_none
 from ._itertools import always_iterable, unique_everseen
 from ._meta import PackageMetadata, SimplePath
 
 from contextlib import suppress
 from importlib import import_module
 from importlib.abc import MetaPathFinder
 from itertools import starmap
-from typing import List, Mapping, Optional, cast
-
+from typing import Iterable, List, Mapping, Optional, Set, cast
 
 __all__ = [
     'Distribution',
     'DistributionFinder',
     'PackageMetadata',
     'PackageNotFoundError',
     'distribution',
@@ -49,19 +49,19 @@
     'version',
 ]
 
 
 class PackageNotFoundError(ModuleNotFoundError):
     """The package was not found."""
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"No package metadata was found for {self.name}"
 
     @property
-    def name(self):
+    def name(self) -> str:  # type: ignore[override]
         (name,) = self.args
         return name
 
 
 class Sectioned:
     """
     A simple entry point config parser for performance
@@ -119,15 +119,15 @@
             section_match = value.startswith('[') and value.endswith(']')
             if section_match:
                 name = value.strip('[]')
                 continue
             yield Pair(name, value)
 
     @staticmethod
-    def valid(line):
+    def valid(line: str):
         return line and not line.startswith('#')
 
 
 class DeprecatedTuple:
     """
     Provide subscript item access for backward compatibility.
 
@@ -194,40 +194,43 @@
 
     name: str
     value: str
     group: str
 
     dist: Optional['Distribution'] = None
 
-    def __init__(self, name, value, group):
+    def __init__(self, name: str, value: str, group: str) -> None:
         vars(self).update(name=name, value=value, group=group)
 
     def load(self):
         """Load the entry point from its definition. If only a module
         is indicated by the value, return that module. Otherwise,
         return the named object.
         """
         match = self.pattern.match(self.value)
         module = import_module(match.group('module'))
         attrs = filter(None, (match.group('attr') or '').split('.'))
         return functools.reduce(getattr, attrs, module)
 
     @property
-    def module(self):
+    def module(self) -> str:
         match = self.pattern.match(self.value)
+        assert match is not None
         return match.group('module')
 
     @property
-    def attr(self):
+    def attr(self) -> str:
         match = self.pattern.match(self.value)
+        assert match is not None
         return match.group('attr')
 
     @property
-    def extras(self):
+    def extras(self) -> List[str]:
         match = self.pattern.match(self.value)
+        assert match is not None
         return re.findall(r'\w+', match.group('extras') or '')
 
     def _for(self, dist):
         vars(self).update(dist=dist)
         return self
 
     def matches(self, **params):
@@ -267,26 +270,26 @@
 
     def __repr__(self):
         return (
             f'EntryPoint(name={self.name!r}, value={self.value!r}, '
             f'group={self.group!r})'
         )
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return hash(self._key())
 
 
 class EntryPoints(tuple):
     """
     An immutable collection of selectable EntryPoint objects.
     """
 
     __slots__ = ()
 
-    def __getitem__(self, name):  # -> EntryPoint:
+    def __getitem__(self, name: str) -> EntryPoint:  # type: ignore[override]
         """
         Get the EntryPoint in self matching name.
         """
         try:
             return next(iter(self.select(name=name)))
         except StopIteration:
             raise KeyError(name)
@@ -295,22 +298,22 @@
         """
         Select entry points from self that match the
         given parameters (typically group and/or name).
         """
         return EntryPoints(ep for ep in self if _py39compat.ep_matches(ep, **params))
 
     @property
-    def names(self):
+    def names(self) -> Set[str]:
         """
         Return the set of all names of all entry points.
         """
         return {ep.name for ep in self}
 
     @property
-    def groups(self):
+    def groups(self) -> Set[str]:
         """
         Return the set of all groups of all entry points.
         """
         return {ep.group for ep in self}
 
     @classmethod
     def _from_text_for(cls, text, dist):
@@ -323,32 +326,36 @@
             for item in Sectioned.section_pairs(text or '')
         )
 
 
 class PackagePath(pathlib.PurePosixPath):
     """A reference to a path in a package"""
 
-    def read_text(self, encoding='utf-8'):
+    hash: Optional["FileHash"]
+    size: int
+    dist: "Distribution"
+
+    def read_text(self, encoding: str = 'utf-8') -> str:  # type: ignore[override]
         with self.locate().open(encoding=encoding) as stream:
             return stream.read()
 
-    def read_binary(self):
+    def read_binary(self) -> bytes:
         with self.locate().open('rb') as stream:
             return stream.read()
 
-    def locate(self):
+    def locate(self) -> pathlib.Path:
         """Return a path-like object for this path"""
         return self.dist.locate_file(self)
 
 
 class FileHash:
-    def __init__(self, spec):
+    def __init__(self, spec: str) -> None:
         self.mode, _, self.value = spec.partition('=')
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<FileHash mode: {self.mode} value: {self.value}>'
 
 
 class DeprecatedNonAbstract:
     def __new__(cls, *args, **kwargs):
         all_names = {
             name for subclass in inspect.getmro(cls) for name in vars(subclass)
@@ -375,40 +382,40 @@
         """Attempt to load metadata file given by the name.
 
         :param filename: The name of the file in the distribution info.
         :return: The text if found, otherwise None.
         """
 
     @abc.abstractmethod
-    def locate_file(self, path):
+    def locate_file(self, path: StrPath) -> pathlib.Path:
         """
         Given a path to a file in this distribution, return a path
         to it.
         """
 
     @classmethod
-    def from_name(cls, name: str):
+    def from_name(cls, name: str) -> "Distribution":
         """Return the Distribution for the given package name.
 
         :param name: The name of the distribution package to search for.
         :return: The Distribution instance (or subclass thereof) for the named
             package, if found.
         :raises PackageNotFoundError: When the named package's distribution
             metadata cannot be found.
         :raises ValueError: When an invalid value is supplied for name.
         """
         if not name:
             raise ValueError("A distribution name is required.")
         try:
-            return next(cls.discover(name=name))
+            return next(iter(cls.discover(name=name)))
         except StopIteration:
             raise PackageNotFoundError(name)
 
     @classmethod
-    def discover(cls, **kwargs):
+    def discover(cls, **kwargs) -> Iterable["Distribution"]:
         """Return an iterable of Distribution objects for all packages.
 
         Pass a ``context`` or pass keyword arguments for constructing
         a context.
 
         :context: A ``DistributionFinder.Context`` object.
         :return: Iterable of Distribution objects for all packages.
@@ -418,15 +425,15 @@
             raise ValueError("cannot accept context and kwargs")
         context = context or DistributionFinder.Context(**kwargs)
         return itertools.chain.from_iterable(
             resolver(context) for resolver in cls._discover_resolvers()
         )
 
     @staticmethod
-    def at(path):
+    def at(path: StrPath) -> "Distribution":
         """Return a Distribution for the indicated metadata path
 
         :param path: a string or path-like object
         :return: a concrete Distribution instance for the path
         """
         return PathDistribution(pathlib.Path(path))
 
@@ -453,34 +460,34 @@
             # (which points to the egg-info file) attribute unchanged.
             or self.read_text('')
         )
         text = cast(str, opt_text)
         return _adapters.Message(email.message_from_string(text))
 
     @property
-    def name(self):
+    def name(self) -> str:
         """Return the 'Name' metadata for the distribution package."""
         return self.metadata['Name']
 
     @property
     def _normalized_name(self):
         """Return a normalized version of the name."""
         return Prepared.normalize(self.name)
 
     @property
-    def version(self):
+    def version(self) -> str:
         """Return the 'Version' metadata for the distribution package."""
         return self.metadata['Version']
 
     @property
-    def entry_points(self):
+    def entry_points(self) -> EntryPoints:
         return EntryPoints._from_text_for(self.read_text('entry_points.txt'), self)
 
     @property
-    def files(self):
+    def files(self) -> Optional[List[PackagePath]]:
         """Files in this distribution.
 
         :return: List of PackagePath for this distribution or None
 
         Result is `None` if the metadata file that enumerates files
         (i.e. RECORD for dist-info, or installed-files.txt or
         SOURCES.txt for egg-info) is missing.
@@ -557,15 +564,15 @@
         there (e.g. setup.py) may not correctly reflect the files
         that are present after the package has been installed.
         """
         text = self.read_text('SOURCES.txt')
         return text and map('"{}"'.format, text.splitlines())
 
     @property
-    def requires(self):
+    def requires(self) -> Optional[List[str]]:
         """Generated requirements specified for this Distribution"""
         reqs = self._read_dist_info_reqs() or self._read_egg_info_reqs()
         return reqs and list(reqs)
 
     def _read_dist_info_reqs(self):
         return self.metadata.get_all('Requires-Dist')
 
@@ -636,26 +643,26 @@
         A name of ``None`` matches all distributions.
         """
 
         def __init__(self, **kwargs):
             vars(self).update(kwargs)
 
         @property
-        def path(self):
+        def path(self) -> List[str]:
             """
             The sequence of directory path that a distribution finder
             should search.
 
             Typically refers to Python installed package paths such as
             "site-packages" directories and defaults to ``sys.path``.
             """
             return vars(self).get('path', sys.path)
 
     @abc.abstractmethod
-    def find_distributions(self, context=Context()):
+    def find_distributions(self, context=Context()) -> Iterable[Distribution]:
         """
         Find distributions.
 
         Return an iterable of all Distribution instances capable of
         loading the metadata for packages matching the ``context``,
         a DistributionFinder.Context instance.
         """
@@ -782,15 +789,17 @@
 class MetadataPathFinder(NullFinder, DistributionFinder):
     """A degenerate finder for distribution packages on the file system.
 
     This finder supplies only a find_distributions() method for versions
     of Python that do not have a PathFinder find_distributions().
     """
 
-    def find_distributions(self, context=DistributionFinder.Context()):
+    def find_distributions(
+        self, context=DistributionFinder.Context()
+    ) -> Iterable["PathDistribution"]:
         """
         Find distributions.
 
         Return an iterable of all Distribution instances capable of
         loading the metadata for packages matching ``context.name``
         (or all names if ``None`` indicated) along the paths in the list
         of directories ``context.path``.
@@ -802,39 +811,41 @@
     def _search_paths(cls, name, paths):
         """Find metadata directories in paths heuristically."""
         prepared = Prepared(name)
         return itertools.chain.from_iterable(
             path.search(prepared) for path in map(FastPath, paths)
         )
 
-    def invalidate_caches(cls):
+    def invalidate_caches(cls) -> None:
         FastPath.__new__.cache_clear()
 
 
 class PathDistribution(Distribution):
-    def __init__(self, path: SimplePath):
+    def __init__(self, path: SimplePath) -> None:
         """Construct a distribution.
 
         :param path: SimplePath indicating the metadata directory.
         """
         self._path = path
 
-    def read_text(self, filename):
+    def read_text(self, filename: StrPath) -> Optional[str]:
         with suppress(
             FileNotFoundError,
             IsADirectoryError,
             KeyError,
             NotADirectoryError,
             PermissionError,
         ):
             return self._path.joinpath(filename).read_text(encoding='utf-8')
 
+        return None
+
     read_text.__doc__ = Distribution.read_text.__doc__
 
-    def locate_file(self, path):
+    def locate_file(self, path: StrPath) -> pathlib.Path:
         return self._path.parent / path
 
     @property
     def _normalized_name(self):
         """
         Performance optimization: where possible, resolve the
         normalized name from the file system path.
@@ -859,24 +870,24 @@
         filename, ext = os.path.splitext(stem)
         if ext not in ('.dist-info', '.egg-info'):
             return
         name, sep, rest = filename.partition('-')
         return name
 
 
-def distribution(distribution_name):
+def distribution(distribution_name) -> Distribution:
     """Get the ``Distribution`` instance for the named package.
 
     :param distribution_name: The name of the distribution package as a string.
     :return: A ``Distribution`` instance (or subclass thereof).
     """
     return Distribution.from_name(distribution_name)
 
 
-def distributions(**kwargs):
+def distributions(**kwargs) -> Iterable[Distribution]:
     """Get all ``Distribution`` instances in the current environment.
 
     :return: An iterable of ``Distribution`` instances.
     """
     return Distribution.discover(**kwargs)
 
 
@@ -885,15 +896,15 @@
 
     :param distribution_name: The name of the distribution package to query.
     :return: A PackageMetadata containing the parsed metadata.
     """
     return Distribution.from_name(distribution_name).metadata
 
 
-def version(distribution_name):
+def version(distribution_name) -> str:
     """Get the version string for the named package.
 
     :param distribution_name: The name of the distribution package to query.
     :return: The version string for the package as defined in the package's
         "Version" metadata key.
     """
     return distribution(distribution_name).version
@@ -919,28 +930,28 @@
     """
     eps = itertools.chain.from_iterable(
         dist.entry_points for dist in _unique(distributions())
     )
     return EntryPoints(eps).select(**params)
 
 
-def files(distribution_name):
+def files(distribution_name) -> Optional[List[PackagePath]]:
     """Return a list of files for the named package.
 
     :param distribution_name: The name of the distribution package to query.
     :return: List of files composing the distribution.
     """
     return distribution(distribution_name).files
 
 
-def requires(distribution_name):
+def requires(distribution_name) -> Optional[List[str]]:
     """
     Return a list of requirements for the named package.
 
-    :return: An iterator of requirements, suitable for
+    :return: An iterable of requirements, suitable for
         packaging.requirement.Requirement.
     """
     return distribution(distribution_name).requires
 
 
 def packages_distributions() -> Mapping[str, List[str]]:
     """
```

### Comparing `importlib_metadata-6.5.1/importlib_metadata/_adapters.py` & `importlib_metadata-6.6.0/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/importlib_metadata/_collections.py` & `importlib_metadata-6.6.0/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/importlib_metadata/_compat.py` & `importlib_metadata-6.6.0/importlib_metadata/_compat.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import os
 import sys
 import platform
 
+from typing import Union
+
 
 __all__ = ['install', 'NullFinder', 'Protocol']
 
 
 try:
     from typing import Protocol
 except ImportError:  # pragma: no cover
@@ -66,7 +69,14 @@
     """
     Adjust for variable stacklevel on partial under PyPy.
 
     Workaround for #327.
     """
     is_pypy = platform.python_implementation() == 'PyPy'
     return val + is_pypy
+
+
+if sys.version_info >= (3, 9):
+    StrPath = Union[str, os.PathLike[str]]
+else:
+    # PathLike is only subscriptable at runtime in 3.9+
+    StrPath = Union[str, "os.PathLike[str]"]  # pragma: no cover
```

### Comparing `importlib_metadata-6.5.1/importlib_metadata/_functools.py` & `importlib_metadata-6.6.0/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/importlib_metadata/_itertools.py` & `importlib_metadata-6.6.0/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/importlib_metadata/_meta.py` & `importlib_metadata-6.6.0/importlib_metadata/_meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 class SimplePath(Protocol[_T]):
     """
     A minimal subset of pathlib.Path required by PathDistribution.
     """
 
-    def joinpath(self) -> _T:
+    def joinpath(self, other: Union[str, _T]) -> _T:
         ...  # pragma: no cover
 
     def __truediv__(self, other: Union[str, _T]) -> _T:
         ...  # pragma: no cover
 
     @property
     def parent(self) -> _T:
```

### Comparing `importlib_metadata-6.5.1/importlib_metadata/_py39compat.py` & `importlib_metadata-6.6.0/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/importlib_metadata/_text.py` & `importlib_metadata-6.6.0/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/importlib_metadata.egg-info/PKG-INFO` & `importlib_metadata-6.6.0/importlib_metadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-metadata
-Version: 6.5.1
+Version: 6.6.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `importlib_metadata-6.5.1/importlib_metadata.egg-info/SOURCES.txt` & `importlib_metadata-6.6.0/importlib_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/pytest.ini` & `importlib_metadata-6.6.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/setup.cfg` & `importlib_metadata-6.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/_path.py` & `importlib_metadata-6.6.0/tests/_path.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/data/example-21.12-py3-none-any.whl` & `importlib_metadata-6.6.0/tests/data/example-21.12-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/data/example-21.12-py3.6.egg` & `importlib_metadata-6.6.0/tests/data/example-21.12-py3.6.egg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/data/example2-1.0.0-py3-none-any.whl` & `importlib_metadata-6.6.0/tests/data/example2-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/fixtures.py` & `importlib_metadata-6.6.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/test_api.py` & `importlib_metadata-6.6.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/test_integration.py` & `importlib_metadata-6.6.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/test_main.py` & `importlib_metadata-6.6.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/test_py39compat.py` & `importlib_metadata-6.6.0/tests/test_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tests/test_zip.py` & `importlib_metadata-6.6.0/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.5.1/tox.ini` & `importlib_metadata-6.6.0/tox.ini`

 * *Files identical despite different names*

