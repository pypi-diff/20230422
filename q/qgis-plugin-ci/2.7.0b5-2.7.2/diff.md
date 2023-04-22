# Comparing `tmp/qgis-plugin-ci-2.7.0b5.tar.gz` & `tmp/qgis-plugin-ci-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgis-plugin-ci-2.7.0b5.tar", last modified: Mon Mar  6 14:32:17 2023, max compression
+gzip compressed data, was "qgis-plugin-ci-2.7.2.tar", last modified: Sat Apr 22 18:20:14 2023, max compression
```

## Comparing `qgis-plugin-ci-2.7.0b5.tar` & `qgis-plugin-ci-2.7.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.539490 qgis-plugin-ci-2.7.0b5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.531490 qgis-plugin-ci-2.7.0b5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.531490 qgis-plugin-ci-2.7.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.github/workflows/docs_builder.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.github/workflows/wheel.yml
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/.qgis-plugin-ci
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-03-06 14:32:17.539490 qgis-plugin-ci-2.7.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.531490 qgis-plugin-ci-2.7.0b5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.531490 qgis-plugin-ci-2.7.0b5/docs/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/configuration/exclude.md
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/configuration/options.md
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/configuration/submodules.md
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/configuration/translation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.531490 qgis-plugin-ci-2.7.0b5/docs/development/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/development/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/development/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/development/environment.md
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/development/history.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/development/testing.md
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.531490 qgis-plugin-ci-2.7.0b5/docs/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/misc/credits.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/misc/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.535490 qgis-plugin-ci-2.7.0b5/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/usage/ci_docker.md
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/usage/ci_github.md
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/usage/ci_gitlab.md
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/usage/ci_travis.md
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/usage/cli_changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/usage/cli_package.md
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/usage/cli_release.md
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/docs/usage/cli_translation.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/nose2.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.535490 qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1310 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.535490 qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/icons/opengisch.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/metadata.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1617 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/qgis_plugin_ci_testing_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/resources.qrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.535490 qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/ui/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9628 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/ui/config.ui
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.535490 qgis-plugin-ci-2.7.0b5/qgis_plugin_ci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-03-06 14:32:17.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_ci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-06 14:32:17.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_ci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 14:32:17.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_ci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-06 14:32:17.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_ci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-06 14:32:17.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_ci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-06 14:32:17.000000 qgis-plugin-ci-2.7.0b5/qgis_plugin_ci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.535490 qgis-plugin-ci-2.7.0b5/qgispluginci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/changelog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8606 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/plugins.xml.template
--rw-r--r--   0 runner    (1001) docker     (123)    21627 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/release.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.535490 qgis-plugin-ci-2.7.0b5/qgispluginci/translation_clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/translation_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/translation_clients/baseclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/translation_clients/transifex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/qgispluginci/version_note.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.539490 qgis-plugin-ci-2.7.0b5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/requirements/development.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/requirements/documentation.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/requirements/translation.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.539490 qgis-plugin-ci-2.7.0b5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-06 14:32:17.539490 qgis-plugin-ci-2.7.0b5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.539490 qgis-plugin-ci-2.7.0b5/test/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:32:17.539490 qgis-plugin-ci-2.7.0b5/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/test/fixtures/.qgis-plugin-ci-test-changelog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/test/fixtures/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/test/plugins.xml.expected
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/test/test_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/test/test_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/test/test_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-06 14:31:47.000000 qgis-plugin-ci-2.7.0b5/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.684294 qgis-plugin-ci-2.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.676294 qgis-plugin-ci-2.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.676294 qgis-plugin-ci-2.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.github/workflows/docs_builder.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/.qgis-plugin-ci
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-22 18:20:14.684294 qgis-plugin-ci-2.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.676294 qgis-plugin-ci-2.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.680294 qgis-plugin-ci-2.7.2/docs/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/configuration/exclude.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/configuration/options.md
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/configuration/submodules.md
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/configuration/translation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.680294 qgis-plugin-ci-2.7.2/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/development/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/development/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/development/environment.md
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/development/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/development/testing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.680294 qgis-plugin-ci-2.7.2/docs/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/misc/credits.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/misc/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.680294 qgis-plugin-ci-2.7.2/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/usage/ci_docker.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/usage/ci_github.md
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/usage/ci_gitlab.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/usage/ci_travis.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/usage/cli_changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/usage/cli_package.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/usage/cli_release.md
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/docs/usage/cli_translation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/nose2.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.680294 qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1310 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.680294 qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/icons/opengisch.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/metadata.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1617 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/qgis_plugin_ci_testing_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/resources.qrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.680294 qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/ui/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9628 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/ui/config.ui
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.680294 qgis-plugin-ci-2.7.2/qgis_plugin_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-22 18:20:14.000000 qgis-plugin-ci-2.7.2/qgis_plugin_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-22 18:20:14.000000 qgis-plugin-ci-2.7.2/qgis_plugin_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 18:20:14.000000 qgis-plugin-ci-2.7.2/qgis_plugin_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-22 18:20:14.000000 qgis-plugin-ci-2.7.2/qgis_plugin_ci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-22 18:20:14.000000 qgis-plugin-ci-2.7.2/qgis_plugin_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-22 18:20:14.000000 qgis-plugin-ci-2.7.2/qgis_plugin_ci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.684294 qgis-plugin-ci-2.7.2/qgispluginci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/changelog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8601 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      453 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/plugins.xml.template
+-rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.684294 qgis-plugin-ci-2.7.2/qgispluginci/translation_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/translation_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/translation_clients/baseclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/translation_clients/transifex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/qgispluginci/version_note.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.684294 qgis-plugin-ci-2.7.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/requirements/development.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/requirements/documentation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/requirements/translation.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.684294 qgis-plugin-ci-2.7.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-22 18:20:14.688294 qgis-plugin-ci-2.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.684294 qgis-plugin-ci-2.7.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 18:20:14.684294 qgis-plugin-ci-2.7.2/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/test/fixtures/.qgis-plugin-ci-test-changelog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/test/fixtures/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/test/plugins.xml.expected
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/test/test_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/test/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/test/test_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-22 18:19:48.000000 qgis-plugin-ci-2.7.2/test/utils.py
```

### Comparing `qgis-plugin-ci-2.7.0b5/.github/workflows/docs_builder.yml` & `qgis-plugin-ci-2.7.2/.github/workflows/docs_builder.yml`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/.github/workflows/release.yml` & `qgis-plugin-ci-2.7.2/.github/workflows/release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         uses: actions/download-artifact@v3
         with:
           name: python_wheel
           path: dist/
 
       # -- FROM HERE, A TAG IS REQUIRED ---
       - name: Deploy to PyPI
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
 
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
 
       - name: Create/update release on GitHub
         uses: ncipollo/release-action@v1.12.0
```

### Comparing `qgis-plugin-ci-2.7.0b5/.github/workflows/test.yml` & `qgis-plugin-ci-2.7.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/.github/workflows/wheel.yml` & `qgis-plugin-ci-2.7.2/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/.pre-commit-config.yaml` & `qgis-plugin-ci-2.7.2/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -14,16 +14,22 @@
       - id: end-of-file-fixer
       - id: fix-byte-order-marker
       - id: fix-encoding-pragma
         args: [--remove]
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
 
+  - repo: https://github.com/asottile/pyupgrade
+    rev: v3.3.1
+    hooks:
+      - id: pyupgrade
+        args: [--py38-plus]
+
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
```

### Comparing `qgis-plugin-ci-2.7.0b5/CHANGELOG.md` & `qgis-plugin-ci-2.7.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/CONTRIBUTING.md` & `qgis-plugin-ci-2.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/LICENSE` & `qgis-plugin-ci-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/PKG-INFO` & `qgis-plugin-ci-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-ci
-Version: 2.7.0b5
+Version: 2.7.2
 Summary: Let qgis-plugin-ci package and release your QGIS plugins for you. Have a tea or go hiking meanwhile. Contains scripts to perform automated testing and deployment for QGIS plugins. These scripts are written for and tested on GitHub Actions, GitLab CI, Travis-CI, and Transifex.
 Author-email: Denis Rouzaud <denis@opengis.ch>, Etienne Trimaille <etienne.trimaille@gmail.com>, Julien Moura <dev@ingeoveritas.com>
 License: GPLv3
 Project-URL: homepage, https://opengisch.github.io/qgis-plugin-ci/
 Project-URL: documentation, https://opengisch.github.io/qgis-plugin-ci/
 Project-URL: repository, https://github.com/opengisch/qgis-plugin-ci/
 Project-URL: tracker, https://github.com/opengisch/qgis-plugin-ci/issues
```

### Comparing `qgis-plugin-ci-2.7.0b5/README.md` & `qgis-plugin-ci-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/conf.py` & `qgis-plugin-ci-2.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/configuration/options.md` & `qgis-plugin-ci-2.7.2/docs/configuration/options.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/development/documentation.md` & `qgis-plugin-ci-2.7.2/docs/development/documentation.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/index.md` & `qgis-plugin-ci-2.7.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/misc/faq.md` & `qgis-plugin-ci-2.7.2/docs/misc/faq.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/usage/ci_docker.md` & `qgis-plugin-ci-2.7.2/docs/usage/ci_docker.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/usage/ci_github.md` & `qgis-plugin-ci-2.7.2/docs/usage/ci_github.md`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         with:
           python-version: 3.8
 
        # Needed if the plugin is using Transifex, to have the lrelease command
        # - name: Install Qt lrelease
        #   run: |
        #    sudo apt-get update
-       #    sudo apt-get install qt5-default qttools5-dev-tools
+       #    sudo apt-get install qt5-make qttools5-dev-tools
 
       - name: Install qgis-plugin-ci
         run: pip3 install qgis-plugin-ci
 
       - name: Deploy plugin
         run: >-
           qgis-plugin-ci
```

### Comparing `qgis-plugin-ci-2.7.0b5/docs/usage/ci_travis.md` & `qgis-plugin-ci-2.7.2/docs/usage/ci_travis.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/usage/cli_changelog.md` & `qgis-plugin-ci-2.7.2/docs/usage/cli_changelog.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/usage/cli_package.md` & `qgis-plugin-ci-2.7.2/docs/usage/cli_package.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/usage/cli_release.md` & `qgis-plugin-ci-2.7.2/docs/usage/cli_release.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/docs/usage/cli_translation.md` & `qgis-plugin-ci-2.7.2/docs/usage/cli_translation.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/pyproject.toml` & `qgis-plugin-ci-2.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/__init__.py` & `qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/icons/opengisch.png` & `qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/icons/opengisch.png`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/metadata.txt` & `qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/metadata.txt`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/qgis_plugin_ci_testing_plugin.py` & `qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/qgis_plugin_ci_testing_plugin.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgis_plugin_CI_testing/ui/config.ui` & `qgis-plugin-ci-2.7.2/qgis_plugin_CI_testing/ui/config.ui`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgis_plugin_ci.egg-info/PKG-INFO` & `qgis-plugin-ci-2.7.2/qgis_plugin_ci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgis-plugin-ci
-Version: 2.7.0b5
+Version: 2.7.2
 Summary: Let qgis-plugin-ci package and release your QGIS plugins for you. Have a tea or go hiking meanwhile. Contains scripts to perform automated testing and deployment for QGIS plugins. These scripts are written for and tested on GitHub Actions, GitLab CI, Travis-CI, and Transifex.
 Author-email: Denis Rouzaud <denis@opengis.ch>, Etienne Trimaille <etienne.trimaille@gmail.com>, Julien Moura <dev@ingeoveritas.com>
 License: GPLv3
 Project-URL: homepage, https://opengisch.github.io/qgis-plugin-ci/
 Project-URL: documentation, https://opengisch.github.io/qgis-plugin-ci/
 Project-URL: repository, https://github.com/opengisch/qgis-plugin-ci/
 Project-URL: tracker, https://github.com/opengisch/qgis-plugin-ci/issues
```

### Comparing `qgis-plugin-ci-2.7.0b5/qgis_plugin_ci.egg-info/SOURCES.txt` & `qgis-plugin-ci-2.7.2/qgis_plugin_ci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/changelog.py` & `qgis-plugin-ci-2.7.2/qgispluginci/changelog.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/cli.py` & `qgis-plugin-ci-2.7.2/qgispluginci/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         parser.print_help()
         parser.exit()
 
     exit_val = 0
 
     if os.path.isfile(".qgis-plugin-ci"):
         # We read the .qgis-plugin-ci file
-        with open(".qgis-plugin-ci", "r", encoding="utf8") as f:
+        with open(".qgis-plugin-ci", encoding="utf8") as f:
             arg_dict = yaml.safe_load(f)
     else:
         config = configparser.ConfigParser()
         config.read("setup.cfg")
         if "qgis-plugin-ci" in config.sections():
             # We read the setup.cfg file
             arg_dict = dict(config.items("qgis-plugin-ci"))
```

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/parameters.py` & `qgis-plugin-ci-2.7.2/qgispluginci/parameters.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/plugins.xml.template` & `qgis-plugin-ci-2.7.2/qgispluginci/plugins.xml.template`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/release.py` & `qgis-plugin-ci-2.7.2/qgispluginci/release.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,40 +85,38 @@
         if parser.has_changelog():
             try:
                 content = parser.last_items(
                     count=parameters.changelog_number_of_entries
                 )
                 if content:
                     replace_in_file(
-                        "{}/metadata.txt".format(parameters.plugin_path),
+                        f"{parameters.plugin_path}/metadata.txt",
                         r"^changelog=.*$",
-                        "changelog={}".format(content),
+                        f"changelog={content}",
                     )
             except Exception as exc:
                 # Do not fail the release process if something is wrong when parsing the changelog
                 replace_in_file(
-                    "{}/metadata.txt".format(parameters.plugin_path),
+                    f"{parameters.plugin_path}/metadata.txt",
                     r"^changelog=.*$",
                     "",
                 )
                 logger.warning(
                     f"An exception occurred while parsing the changelog file: {exc}",
                     exc_info=exc,
                 )
     else:
         # Remove the changelog line
-        replace_in_file(
-            "{}/metadata.txt".format(parameters.plugin_path), r"^changelog=.*$", ""
-        )
+        replace_in_file(f"{parameters.plugin_path}/metadata.txt", r"^changelog=.*$", "")
 
     # set version in metadata
     replace_in_file(
-        "{}/metadata.txt".format(parameters.plugin_path),
+        f"{parameters.plugin_path}/metadata.txt",
         r"^version=.*$",
-        "version={}".format(release_version),
+        f"version={release_version}",
     )
 
     # Commit number
     replace_in_file(
         f"{parameters.plugin_path}/metadata.txt",
         r"^commitNumber=.*$",
         f"commitNumber={len(list(repo.iter_commits()))}",
@@ -140,29 +138,29 @@
         r"^dateTime=.*$",
         f"dateTime={date_time}",
     )
 
     # set the plugin as experimental on a pre-release
     if is_prerelease:
         replace_in_file(
-            "{}/metadata.txt".format(parameters.plugin_path),
+            f"{parameters.plugin_path}/metadata.txt",
             r"^experimental=.*$",
-            "experimental={}".format(True if is_prerelease else False),
+            f"experimental={True if is_prerelease else False}",
         )
 
     if raise_min_version:
         replace_in_file(
-            "{}/metadata.txt".format(parameters.plugin_path),
+            f"{parameters.plugin_path}/metadata.txt",
             r"^qgisMinimumVersion=.*$",
-            "qgisMinimumVersion={}".format(raise_min_version),
+            f"qgisMinimumVersion={raise_min_version}",
         )
 
     # replace any DEBUG=False in all Python files
     if not is_prerelease:
-        for file in glob("{}/**/*.py".format(parameters.plugin_path), recursive=True):
+        for file in glob(f"{parameters.plugin_path}/**/*.py", recursive=True):
             replace_in_file(file, r"^DEBUG\s*=\s*True", "DEBUG = False")
 
     # keep track of current state
     try:
         stash = repo.git.stash("create")
     except git.exc.GitCommandError:
         stash = "HEAD"
```

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/translation.py` & `qgis-plugin-ci-2.7.2/qgispluginci/translation.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/translation_clients/baseclient.py` & `qgis-plugin-ci-2.7.2/qgispluginci/translation_clients/baseclient.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/translation_clients/transifex.py` & `qgis-plugin-ci-2.7.2/qgispluginci/translation_clients/transifex.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 logger = logging.getLogger(__name__)
 
 
 class TransifexClient(BaseClient):
     def __init__(
         self, config: TranslationConfig, update_string_fcn, create_project: bool = True
     ):
-        super(TransifexClient, self).__init__(config, update_string_fcn, create_project)
+        super().__init__(config, update_string_fcn, create_project)
 
     def login(self):
         tx_api.setup(auth=self.config.api_token)
         self.organization = self.get_organization()
         logger.info(f"Logged in as organization: {self.config.organization_name}")
 
     def get_organization(self):
@@ -77,15 +77,15 @@
         resource = tx_api.Resource.create(
             project=self.get_project(),
             name=self.config.resource_slug,
             slug=self.config.resource_slug,
             i18n_format=tx_api.I18nFormat(id=self.config.i18n_type),
         )
 
-        with open(self.config.resource_file_path, "r") as fh:
+        with open(self.config.resource_file_path) as fh:
             content = fh.read()
 
         tx_api.ResourceStringsAsyncUpload.upload(content, resource=resource)
         logger.info(f"Resource created: {self.config.resource_slug}")
 
     def get_resource(self):
         resources = self.get_project().fetch("resources")
@@ -108,15 +108,15 @@
             logger.debug(f"Adding {language.code} to {self.config.project_slug}")
             self.get_project().add("languages", [language])
 
         # if coordinators:
         #    self.get_project().add("coordinators", coordinators)
 
     def update_source_translation(self):
-        with open(self.config.resource_file_path, "r") as fh:
+        with open(self.config.resource_file_path) as fh:
             content = fh.read()
 
         tx_api.ResourceStringsAsyncUpload.upload(content, resource=self.get_resource())
         logger.info(f"Source updated for resource: {self.config.resource_slug}")
 
     def get_translation(
         self,
@@ -129,15 +129,19 @@
         Path.mkdir(path_to_parent, parents=True, exist_ok=True)
         language = tx_api.Language.get(code=language_code)
 
         url = tx_api.ResourceTranslationsAsyncDownload.download(
             resource=self.get_resource(), language=language
         )
 
-        translated_content = requests.get(url).text
+        r = requests.get(url)
+        # transifex returns None encoding and the apparent_encoding is Windows-1254 what leads to malformed result strings. So we set the encoding hardcoded to utf-8.
+        if not r.encoding:
+            r.encoding = "utf-8"
+        translated_content = r.text
         with open(path_to_output_file, "w") as fh:
             fh.write(translated_content)
 
         logger.info(
             f"Translations downloaded and written to file (resource: {self.config.resource_slug})"
         )
         return str(path_to_output_file)
```

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/utils.py` & `qgis-plugin-ci-2.7.2/qgispluginci/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from qgispluginci.version_note import VersionNote
 
 # GLOBALS
 logger = logging.getLogger(__name__)
 
 
 def replace_in_file(file_path: str, pattern, new: str, encoding: str = "utf8"):
-    with open(file_path, "r", encoding=encoding) as f:
+    with open(file_path, encoding=encoding) as f:
         content = f.read()
     content = re.sub(pattern, new, content, flags=re.M)
     with open(file_path, "w", encoding=encoding) as f:
         f.write(content)
 
 
 def configure_file(source_file: str, dest_file: str, replace: dict):
-    with open(source_file, "r", encoding="utf-8") as f:
+    with open(source_file, encoding="utf-8") as f:
         content = f.read()
     for pattern, new in replace.items():
         content = re.sub(pattern, new, content, flags=re.M)
     with open(dest_file, "w", encoding="utf-8") as f:
         f.write(content)
 
 
@@ -47,15 +47,15 @@
 
     # conversion
     size_name = ("octets", "Ko", "Mo", "Go", "To", "Po")
     i = int(floor(math_log(octets, 1024)))
     p = pow(1024, i)
     s = round(octets / p, 2)
 
-    return "%s %s" % (s, size_name[i])
+    return f"{s} {size_name[i]}"
 
 
 def touch_file(path, update_time: bool = False, create_dir: bool = True):
     basedir = os.path.dirname(path)
     if create_dir and not os.path.exists(basedir):
         os.makedirs(basedir)
     with open(path, "a"):
```

### Comparing `qgis-plugin-ci-2.7.0b5/qgispluginci/version_note.py` & `qgis-plugin-ci-2.7.2/qgispluginci/version_note.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/setup.cfg` & `qgis-plugin-ci-2.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/test/fixtures/CHANGELOG.md` & `qgis-plugin-ci-2.7.2/test/fixtures/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/test/plugins.xml.expected` & `qgis-plugin-ci-2.7.2/test/plugins.xml.expected`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/test/test_changelog.py` & `qgis-plugin-ci-2.7.2/test/test_changelog.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/test/test_release.py` & `qgis-plugin-ci-2.7.2/test/test_release.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # If changed, also update CHANGELOG.md
 RELEASE_VERSION_TEST = "0.1.2"
 
 
 class TestRelease(unittest.TestCase):
     def setUp(self):
-        with open(".qgis-plugin-ci", "r", encoding="utf8") as f:
+        with open(".qgis-plugin-ci", encoding="utf8") as f:
             arg_dict = yaml.safe_load(f)
         self.parameters = Parameters(arg_dict)
         self.tx_api_token = os.getenv("tx_api_token")
         self.github_token = os.getenv("github_token")
         self.repo = None
         self.t = None
         if self.github_token:
```

### Comparing `qgis-plugin-ci-2.7.0b5/test/test_translation.py` & `qgis-plugin-ci-2.7.2/test/test_translation.py`

 * *Files identical despite different names*

### Comparing `qgis-plugin-ci-2.7.0b5/test/test_utils.py` & `qgis-plugin-ci-2.7.2/test/test_utils.py`

 * *Files identical despite different names*

