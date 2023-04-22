# Comparing `tmp/adafruit-circuitpython-requests-1.9.8.tar.gz` & `tmp/adafruit-circuitpython-requests-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-requests-1.9.8.tar", last modified: Wed Mar  3 00:04:11 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-requests-1.9.9.tar", last modified: Thu Apr  8 17:55:08 2021, max compression
```

## Comparing `adafruit-circuitpython-requests-1.9.8.tar` & `adafruit-circuitpython-requests-1.9.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:04:11.238279 adafruit-circuitpython-requests-1.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:04:11.230279 adafruit-circuitpython-requests-1.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:04:11.234279 adafruit-circuitpython-requests-1.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/.github/workflows/release.yml
--rwxr-xr-x   0 runner    (1001) docker     (116)      189 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (116)    16231 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/.pylintrc
--rwxr-xr-x   0 runner    (1001) docker     (116)      162 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (116)     6147 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (116)     1098 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:04:11.234279 adafruit-circuitpython-requests-1.9.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3562 2021-03-03 00:04:11.238279 adafruit-circuitpython-requests-1.9.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (116)     2205 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:04:11.234279 adafruit-circuitpython-requests-1.9.8/adafruit_circuitpython_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3562 2021-03-03 00:04:11.000000 adafruit-circuitpython-requests-1.9.8/adafruit_circuitpython_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1367 2021-03-03 00:04:11.000000 adafruit-circuitpython-requests-1.9.8/adafruit_circuitpython_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-03 00:04:11.000000 adafruit-circuitpython-requests-1.9.8/adafruit_circuitpython_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2021-03-03 00:04:11.000000 adafruit-circuitpython-requests-1.9.8/adafruit_circuitpython_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2021-03-03 00:04:11.000000 adafruit-circuitpython-requests-1.9.8/adafruit_circuitpython_requests.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    23233 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/adafruit_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:04:11.234279 adafruit-circuitpython-requests-1.9.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:04:11.234279 adafruit-circuitpython-requests-1.9.8/docs/_static/
--rwxr-xr-x   0 runner    (1001) docker     (116)     4414 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/docs/_static/favicon.ico.license
--rwxr-xr-x   0 runner    (1001) docker     (116)      267 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (116)     5437 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      190 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/docs/examples.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (116)      901 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:04:11.238279 adafruit-circuitpython-requests-1.9.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     2183 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_advanced.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2028 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_advanced_cellular.py
--rw-r--r--   0 runner    (1001) docker     (116)      844 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_advanced_cpython.py
--rw-r--r--   0 runner    (1001) docker     (116)     1764 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_advanced_ethernet.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      515 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_github_cpython.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1853 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_https_circuitpython.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1348 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_https_cpython.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2807 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2506 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_simpletest_cellular.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     1307 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (116)     3556 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/examples/requests_simpletest_ethernet.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      119 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-03 00:04:11.238279 adafruit-circuitpython-requests-1.9.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (116)     1977 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-03 00:04:11.238279 adafruit-circuitpython-requests-1.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     3707 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/chunk_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     3043 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/header_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     1200 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/legacy_mocket.py
--rw-r--r--   0 runner    (1001) docker     (116)     6530 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/legacy_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     1837 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (116)      954 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/parse_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     2358 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/post_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     3093 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/protocol_test.py
--rw-r--r--   0 runner    (1001) docker     (116)     6444 2021-03-03 00:04:00.000000 adafruit-circuitpython-requests-1.9.8/tests/reuse_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.177097 adafruit-circuitpython-requests-1.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.181098 adafruit-circuitpython-requests-1.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.github/workflows/release.yml
+-rwxr-xr-x   0 runner    (1001) docker     (121)      189 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1389 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (121)    16223 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.pylintrc
+-rwxr-xr-x   0 runner    (1001) docker     (121)      162 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/.readthedocs.yml
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6147 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1098 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.181098 adafruit-circuitpython-requests-1.9.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2205 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.181098 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2021-04-08 17:55:07.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-04-08 17:55:08.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-08 17:55:07.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-04-08 17:55:07.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-04-08 17:55:07.000000 adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    23369 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/adafruit_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.181098 adafruit-circuitpython-requests-1.9.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/docs/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4414 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/_static/favicon.ico.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)      267 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5437 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      190 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/examples.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)      901 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2183 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_advanced.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2028 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1764 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_ethernet.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      515 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_github_cpython.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1853 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_https_circuitpython.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1348 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_https_cpython.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2986 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2506 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_cellular.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1307 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3556 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_ethernet.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      119 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1977 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-08 17:55:08.185098 adafruit-circuitpython-requests-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     3921 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/chunk_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3168 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/header_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1350 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/legacy_mocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6638 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/legacy_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2157 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1027 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/parse_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2482 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/post_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3282 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/protocol_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6858 2021-04-08 17:54:57.000000 adafruit-circuitpython-requests-1.9.9/tests/reuse_test.py
```

### Comparing `adafruit-circuitpython-requests-1.9.8/.github/workflows/build.yml` & `adafruit-circuitpython-requests-1.9.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/.github/workflows/release.yml` & `adafruit-circuitpython-requests-1.9.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/.pre-commit-config.yaml` & `adafruit-circuitpython-requests-1.9.9/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,24 @@
     -   id: trailing-whitespace
 -   repo: https://github.com/pycqa/pylint
     rev: pylint-2.7.1
     hooks:
     -   id: pylint
         name: pylint (library code)
         types: [python]
-        exclude: "^(docs/|examples/|setup.py$)"
+        exclude: "^(docs/|examples/|tests/|setup.py$)"
 -   repo: local
     hooks:
     -   id: pylint_examples
         name: pylint (examples code)
         description: Run pylint rules on "examples/*.py" files
         entry: /usr/bin/env bash -c
         args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
         language: system
+-   repo: local
+    hooks:
+    -   id: pylint_tests
+        name: pylint (tests code)
+        description: Run pylint rules on "tests/*.py" files
+        entry: /usr/bin/env bash -c
+        args: ['([[ ! -d "tests" ]] || for example in $(find . -path "./tests/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
+        language: system
```

### Comparing `adafruit-circuitpython-requests-1.9.8/.pylintrc` & `adafruit-circuitpython-requests-1.9.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
-# jobs=1
-jobs=2
+jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
 load-plugins=
 
 # Pickle collected data for later comparisons.
 persistent=yes
@@ -249,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-requests-1.9.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-requests-1.9.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/LICENSE` & `adafruit-circuitpython-requests-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-requests-1.9.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/LICENSES/MIT.txt` & `adafruit-circuitpython-requests-1.9.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-requests-1.9.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/PKG-INFO` & `adafruit-circuitpython-requests-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 1.9.8
+Version: 1.9.9
 Summary: A requests-like library for web interfacing
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-requests-1.9.8/README.rst` & `adafruit-circuitpython-requests-1.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/adafruit_circuitpython_requests.egg-info/PKG-INFO` & `adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-requests
-Version: 1.9.8
+Version: 1.9.9
 Summary: A requests-like library for web interfacing
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Requests
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-requests-1.9.8/adafruit_circuitpython_requests.egg-info/SOURCES.txt` & `adafruit-circuitpython-requests-1.9.9/adafruit_circuitpython_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/adafruit_requests.py` & `adafruit-circuitpython-requests-1.9.9/adafruit_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -648,17 +648,20 @@
         # pylint: disable=unused-argument
         return _FakeSSLSocket(socket, self._iface.TLS_MODE)
 
 
 def set_socket(sock, iface=None):
     """Legacy API for setting the socket and network interface. Use a `Session` instead."""
     global _default_session  # pylint: disable=global-statement,invalid-name
-    _default_session = Session(sock, _FakeSSLContext(iface))
-    if iface:
-        sock.set_interface(iface)
+    if not iface:
+        # pylint: disable=protected-access
+        _default_session = Session(sock, _FakeSSLContext(sock._the_interface))
+    else:
+        _default_session = Session(sock, _FakeSSLContext(iface))
+    sock.set_interface(iface)
 
 
 def request(method, url, data=None, json=None, headers=None, stream=False, timeout=1):
     """Send HTTP request"""
     # pylint: disable=too-many-arguments
     _default_session.request(
         method,
```

### Comparing `adafruit-circuitpython-requests-1.9.8/docs/_static/favicon.ico` & `adafruit-circuitpython-requests-1.9.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/docs/conf.py` & `adafruit-circuitpython-requests-1.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/docs/index.rst` & `adafruit-circuitpython-requests-1.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_advanced.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_advanced.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_advanced_cellular.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_advanced_cpython.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_advanced_ethernet.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_advanced_ethernet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_github_cpython.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_github_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_https_circuitpython.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_https_circuitpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_https_cpython.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_https_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_simpletest.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 esp32_reset = DigitalInOut(board.ESP_RESET)
 
 # If you have an externally connected ESP32:
 # esp32_cs = DigitalInOut(board.D9)
 # esp32_ready = DigitalInOut(board.D10)
 # esp32_reset = DigitalInOut(board.D5)
 
+# If you have an AirLift Featherwing or ItsyBitsy Airlift:
+# esp32_cs = DigitalInOut(board.D13)
+# esp32_ready = DigitalInOut(board.D11)
+# esp32_reset = DigitalInOut(board.D12)
+
 spi = busio.SPI(board.SCK, board.MOSI, board.MISO)
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 
 print("Connecting to AP...")
 while not esp.is_connected:
     try:
         esp.connect_AP(secrets["ssid"], secrets["password"])
@@ -42,16 +47,16 @@
 print("Connected to", str(esp.ssid, "utf-8"), "\tRSSI:", esp.rssi)
 
 # Initialize a requests object with a socket and esp32spi interface
 socket.set_interface(esp)
 requests.set_socket(socket, esp)
 
 TEXT_URL = "http://wifitest.adafruit.com/testwifi/index.html"
-JSON_GET_URL = "http://httpbin.org/get"
-JSON_POST_URL = "http://httpbin.org/post"
+JSON_GET_URL = "https://httpbin.org/get"
+JSON_POST_URL = "https://httpbin.org/post"
 
 print("Fetching text from %s" % TEXT_URL)
 response = requests.get(TEXT_URL)
 print("-" * 40)
 
 print("Text Response: ", response.text)
 print("-" * 40)
```

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_simpletest_cellular.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_simpletest_cpython.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/examples/requests_simpletest_ethernet.py` & `adafruit-circuitpython-requests-1.9.9/examples/requests_simpletest_ethernet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/setup.py` & `adafruit-circuitpython-requests-1.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-requests-1.9.8/tests/chunk_test.py` & `adafruit-circuitpython-requests-1.9.9/tests/chunk_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
+""" Chunk Tests """
+
 from unittest import mock
 import mocket
 import adafruit_requests
 
-ip = "1.2.3.4"
-host = "wifitest.adafruit.com"
-path = "/testwifi/index.html"
-text = b"This is a test of Adafruit WiFi!\r\nIf you can read this, its working :)"
-headers = b"HTTP/1.0 200 OK\r\nTransfer-Encoding: chunked\r\n\r\n"
-headers_extra_space = b"HTTP/1.0 200 OK\r\nTransfer-Encoding:  chunked\r\n\r\n"
+IP = "1.2.3.4"
+HOST = "wifitest.adafruit.com"
+PATH = "/testwifi/index.html"
+TEXT = b"This is a test of Adafruit WiFi!\r\nIf you can read this, its working :)"
+HEADERS = b"HTTP/1.0 200 OK\r\nTransfer-Encoding: chunked\r\n\r\n"
+HEADERS_EXTRA_SPACE = b"HTTP/1.0 200 OK\r\nTransfer-Encoding:  chunked\r\n\r\n"
 
 
 def _chunk(response, split, extra=b""):
     i = 0
     chunked = b""
     while i < len(response):
         remaining = len(response) - i
@@ -32,26 +34,28 @@
         )
         i = new_i
     # The final chunk is zero length.
     chunked += b"0\r\n\r\n"
     return chunked
 
 
-def do_test_get_text(extra=b""):
+def do_test_get_text(
+    extra=b"",
+):
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    c = _chunk(text, 33, extra)
-    print(c)
-    sock = mocket.Mocket(headers + c)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    chunk = _chunk(TEXT, 33, extra)
+    print(chunk)
+    sock = mocket.Mocket(HEADERS + chunk)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
-    r = s.get("http://" + host + path)
+    requests_session = adafruit_requests.Session(pool)
+    response = requests_session.get("http://" + HOST + PATH)
 
-    sock.connect.assert_called_once_with((ip, 80))
+    sock.connect.assert_called_once_with((IP, 80))
 
     sock.send.assert_has_calls(
         [
             mock.call(b"GET"),
             mock.call(b" /"),
             mock.call(b"testwifi/index.html"),
             mock.call(b" HTTP/1.1\r\n"),
@@ -59,38 +63,41 @@
     )
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
             mock.call(b"wifitest.adafruit.com"),
         ]
     )
-    assert r.text == str(text, "utf-8")
+    assert response.text == str(TEXT, "utf-8")
 
 
 def test_get_text():
     do_test_get_text()
 
 
 def test_get_text_extra():
     do_test_get_text(b";blahblah; blah")
 
 
-def do_test_close_flush(extra=b""):
-    """Test that a chunked response can be closed even when the request contents were not accessed."""
+def do_test_close_flush(
+    extra=b"",
+):
+    """Test that a chunked response can be closed even when the
+    request contents were not accessed."""
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    c = _chunk(text, 33, extra)
-    print(c)
-    sock = mocket.Mocket(headers + c)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    chunk = _chunk(TEXT, 33, extra)
+    print(chunk)
+    sock = mocket.Mocket(HEADERS + chunk)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
-    r = s.get("http://" + host + path)
+    requests_session = adafruit_requests.Session(pool)
+    response = requests_session.get("http://" + HOST + PATH)
 
-    sock.connect.assert_called_once_with((ip, 80))
+    sock.connect.assert_called_once_with((IP, 80))
 
     sock.send.assert_has_calls(
         [
             mock.call(b"GET"),
             mock.call(b" /"),
             mock.call(b"testwifi/index.html"),
             mock.call(b" HTTP/1.1\r\n"),
@@ -99,37 +106,39 @@
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
             mock.call(b"wifitest.adafruit.com"),
         ]
     )
 
-    r.close()
+    response.close()
 
 
 def test_close_flush():
     do_test_close_flush()
 
 
 def test_close_flush_extra():
     do_test_close_flush(b";blahblah; blah")
 
 
-def do_test_get_text_extra_space(extra=b""):
+def do_test_get_text_extra_space(
+    extra=b"",
+):
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    c = _chunk(text, 33, extra)
-    print(c)
-    sock = mocket.Mocket(headers_extra_space + c)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    chunk = _chunk(TEXT, 33, extra)
+    print(chunk)
+    sock = mocket.Mocket(HEADERS_EXTRA_SPACE + chunk)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
-    r = s.get("http://" + host + path)
+    requests_session = adafruit_requests.Session(pool)
+    response = requests_session.get("http://" + HOST + PATH)
 
-    sock.connect.assert_called_once_with((ip, 80))
+    sock.connect.assert_called_once_with((IP, 80))
 
     sock.send.assert_has_calls(
         [
             mock.call(b"GET"),
             mock.call(b" /"),
             mock.call(b"testwifi/index.html"),
             mock.call(b" HTTP/1.1\r\n"),
@@ -137,8 +146,8 @@
     )
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
             mock.call(b"wifitest.adafruit.com"),
         ]
     )
-    assert r.text == str(text, "utf-8")
+    assert response.text == str(TEXT, "utf-8")
```

### Comparing `adafruit-circuitpython-requests-1.9.8/tests/concurrent_test.py` & `adafruit-circuitpython-requests-1.9.9/tests/concurrent_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,102 +1,101 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
+""" Concurrent Tests """
+
+import errno
 from unittest import mock
 import mocket
-import pytest
-import errno
 import adafruit_requests
 
-ip = "1.2.3.4"
-host = "wifitest.adafruit.com"
-host2 = "wifitest2.adafruit.com"
-path = "/testwifi/index.html"
-text = b"This is a test of Adafruit WiFi!\r\nIf you can read this, its working :)"
-response = b"HTTP/1.0 200 OK\r\nContent-Length: 70\r\n\r\n" + text
+IP = "1.2.3.4"
+HOST = "wifitest.adafruit.com"
+HOST2 = "test.adafruit.com"
+PATH = "/testwifi/index.html"
+TEXT = b"This is a test of Adafruit WiFi!\r\nIf you can read this, its working :)"
+RESPONSE = b"HTTP/1.0 200 OK\r\nContent-Length: 70\r\n\r\n" + TEXT
 
 
-def test_second_connect_fails_memoryerror():
+def test_second_connect_fails_memoryerror():  # pylint: disable=invalid-name
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(response)
-    sock2 = mocket.Mocket(response)
-    sock3 = mocket.Mocket(response)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE)
+    sock2 = mocket.Mocket(RESPONSE)
+    sock3 = mocket.Mocket(RESPONSE)
     pool.socket.call_count = 0  # Reset call count
     pool.socket.side_effect = [sock, sock2, sock3]
     sock2.connect.side_effect = MemoryError()
 
     ssl = mocket.SSLContext()
 
-    s = adafruit_requests.Session(pool, ssl)
-    r = s.get("https://" + host + path)
+    requests_session = adafruit_requests.Session(pool, ssl)
+    response = requests_session.get("https://" + HOST + PATH)
 
     sock.send.assert_has_calls(
         [
             mock.call(b"testwifi/index.html"),
         ]
     )
 
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
             mock.call(b"wifitest.adafruit.com"),
             mock.call(b"\r\n"),
         ]
     )
-    assert r.text == str(text, "utf-8")
+    assert response.text == str(TEXT, "utf-8")
 
-    host2 = "test.adafruit.com"
-    s.get("https://" + host2 + path)
+    requests_session.get("https://" + HOST2 + PATH)
 
-    sock.connect.assert_called_once_with((host, 443))
-    sock2.connect.assert_called_once_with((host2, 443))
-    sock3.connect.assert_called_once_with((host2, 443))
+    sock.connect.assert_called_once_with((HOST, 443))
+    sock2.connect.assert_called_once_with((HOST2, 443))
+    sock3.connect.assert_called_once_with((HOST2, 443))
     # Make sure that the socket is closed after send fails.
     sock.close.assert_called_once()
     sock2.close.assert_called_once()
     assert sock3.close.call_count == 0
     assert pool.socket.call_count == 3
 
 
-def test_second_connect_fails_oserror():
+def test_second_connect_fails_oserror():  # pylint: disable=invalid-name
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(response)
-    sock2 = mocket.Mocket(response)
-    sock3 = mocket.Mocket(response)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE)
+    sock2 = mocket.Mocket(RESPONSE)
+    sock3 = mocket.Mocket(RESPONSE)
     pool.socket.call_count = 0  # Reset call count
     pool.socket.side_effect = [sock, sock2, sock3]
     sock2.connect.side_effect = OSError(errno.ENOMEM)
 
     ssl = mocket.SSLContext()
 
-    s = adafruit_requests.Session(pool, ssl)
-    r = s.get("https://" + host + path)
+    requests_session = adafruit_requests.Session(pool, ssl)
+    response = requests_session.get("https://" + HOST + PATH)
 
     sock.send.assert_has_calls(
         [
             mock.call(b"testwifi/index.html"),
         ]
     )
 
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
             mock.call(b"wifitest.adafruit.com"),
             mock.call(b"\r\n"),
         ]
     )
-    assert r.text == str(text, "utf-8")
+    assert response.text == str(TEXT, "utf-8")
 
-    host2 = "test.adafruit.com"
-    s.get("https://" + host2 + path)
+    requests_session.get("https://" + HOST2 + PATH)
 
-    sock.connect.assert_called_once_with((host, 443))
-    sock2.connect.assert_called_once_with((host2, 443))
-    sock3.connect.assert_called_once_with((host2, 443))
+    sock.connect.assert_called_once_with((HOST, 443))
+    sock2.connect.assert_called_once_with((HOST2, 443))
+    sock3.connect.assert_called_once_with((HOST2, 443))
     # Make sure that the socket is closed after send fails.
     sock.close.assert_called_once()
     sock2.close.assert_called_once()
     assert sock3.close.call_count == 0
     assert pool.socket.call_count == 3
```

### Comparing `adafruit-circuitpython-requests-1.9.8/tests/legacy_mocket.py` & `adafruit-circuitpython-requests-1.9.9/tests/legacy_mocket.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
+""" Mock for Legacy Socket """
+
 from unittest import mock
 
 SOCK_STREAM = 0
 
 set_interface = mock.Mock()
 interface = mock.MagicMock()
 getaddrinfo = mock.Mock()
 socket = mock.Mock()
 
 
-class Mocket:
+class Mocket:  # pylint: disable=too-few-public-methods
+    """  Mock Socket """
+
     def __init__(self, response):
         self.settimeout = mock.Mock()
         self.close = mock.Mock()
         self.connect = mock.Mock()
         self.send = mock.Mock(side_effect=self._send)
         self.readline = mock.Mock(side_effect=self._readline)
         self.recv = mock.Mock(side_effect=self._recv)
         self.fail_next_send = False
         self._response = response
         self._position = 0
 
-    def _send(self, data):
+    def _send(self, data):  # pylint: disable=unused-argument
         if self.fail_next_send:
             self.fail_next_send = False
             raise RuntimeError("Send failed")
-        return None
 
     def _readline(self):
         i = self._response.find(b"\r\n", self._position)
-        r = self._response[self._position : i + 2]
+        response = self._response[self._position : i + 2]
         self._position = i + 2
-        return r
+        return response
 
     def _recv(self, count):
         end = self._position + count
-        r = self._response[self._position : end]
+        response = self._response[self._position : end]
         self._position = end
-        print(r)
-        return r
+        print(response)
+        return response
```

### Comparing `adafruit-circuitpython-requests-1.9.8/tests/legacy_test.py` & `adafruit-circuitpython-requests-1.9.9/tests/legacy_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,208 +1,208 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
+""" Legacy Tests """
+
 from unittest import mock
-import legacy_mocket as mocket
 import json
-import pytest
+import legacy_mocket as mocket
 import adafruit_requests
 
-ip = "1.2.3.4"
-host = "httpbin.org"
-response = {"Date": "July 25, 2019"}
-encoded = json.dumps(response).encode("utf-8")
-headers = "HTTP/1.0 200 OK\r\nContent-Length: {}\r\n\r\n".format(len(encoded)).encode(
+IP = "1.2.3.4"
+HOST = "httpbin.org"
+RESPONSE = {"Date": "July 25, 2019"}
+ENCODED = json.dumps(RESPONSE).encode("utf-8")
+HEADERS = "HTTP/1.0 200 OK\r\nContent-Length: {}\r\n\r\n".format(len(ENCODED)).encode(
     "utf-8"
 )
 
 
 def test_get_json():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
+    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
     mocket.socket.return_value = sock
 
     adafruit_requests.set_socket(mocket, mocket.interface)
-    r = adafruit_requests.get("http://" + host + "/get")
+    response = adafruit_requests.get("http://" + HOST + "/get")
 
-    sock.connect.assert_called_once_with((ip, 80))
-    assert r.json() == response
-    r.close()
+    sock.connect.assert_called_once_with((IP, 80))
+    assert response.json() == RESPONSE
+    response.close()
 
 
 def test_tls_mode():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
+    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
     mocket.socket.return_value = sock
 
     adafruit_requests.set_socket(mocket, mocket.interface)
-    r = adafruit_requests.get("https://" + host + "/get")
+    response = adafruit_requests.get("https://" + HOST + "/get")
 
-    sock.connect.assert_called_once_with((host, 443), mocket.interface.TLS_MODE)
-    assert r.json() == response
-    r.close()
+    sock.connect.assert_called_once_with((HOST, 443), mocket.interface.TLS_MODE)
+    assert response.json() == RESPONSE
+    response.close()
 
 
 def test_post_string():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
+    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
     mocket.socket.return_value = sock
 
     adafruit_requests.set_socket(mocket, mocket.interface)
     data = "31F"
-    r = adafruit_requests.post("http://" + host + "/post", data=data)
-    sock.connect.assert_called_once_with((ip, 80))
+    response = adafruit_requests.post("http://" + HOST + "/post", data=data)
+    sock.connect.assert_called_once_with((IP, 80))
     sock.send.assert_called_with(b"31F")
-    r.close()
+    response.close()
 
 
 def test_second_tls_send_fails():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
-    sock2 = mocket.Mocket(headers + encoded)
+    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
+    sock2 = mocket.Mocket(HEADERS + ENCODED)
     mocket.socket.call_count = 0  # Reset call count
     mocket.socket.side_effect = [sock, sock2]
 
     adafruit_requests.set_socket(mocket, mocket.interface)
-    r = adafruit_requests.get("https://" + host + "/testwifi/index.html")
+    response = adafruit_requests.get("https://" + HOST + "/testwifi/index.html")
 
     sock.send.assert_has_calls(
         [
             mock.call(b"testwifi/index.html"),
         ]
     )
 
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
-            mock.call(host.encode("utf-8")),
+            mock.call(HOST.encode("utf-8")),
             mock.call(b"\r\n"),
         ]
     )
-    assert r.text == str(encoded, "utf-8")
+    assert response.text == str(ENCODED, "utf-8")
 
     sock.fail_next_send = True
-    adafruit_requests.get("https://" + host + "/get2")
+    adafruit_requests.get("https://" + HOST + "/get2")
 
-    sock.connect.assert_called_once_with((host, 443), mocket.interface.TLS_MODE)
-    sock2.connect.assert_called_once_with((host, 443), mocket.interface.TLS_MODE)
+    sock.connect.assert_called_once_with((HOST, 443), mocket.interface.TLS_MODE)
+    sock2.connect.assert_called_once_with((HOST, 443), mocket.interface.TLS_MODE)
     # Make sure that the socket is closed after send fails.
     sock.close.assert_called_once()
     assert sock2.close.call_count == 0
     assert mocket.socket.call_count == 2
 
 
 def test_second_send_fails():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
-    sock2 = mocket.Mocket(headers + encoded)
+    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
+    sock2 = mocket.Mocket(HEADERS + ENCODED)
     mocket.socket.call_count = 0  # Reset call count
     mocket.socket.side_effect = [sock, sock2]
 
     adafruit_requests.set_socket(mocket, mocket.interface)
-    r = adafruit_requests.get("http://" + host + "/testwifi/index.html")
+    response = adafruit_requests.get("http://" + HOST + "/testwifi/index.html")
 
     sock.send.assert_has_calls(
         [
             mock.call(b"testwifi/index.html"),
         ]
     )
 
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
-            mock.call(host.encode("utf-8")),
+            mock.call(HOST.encode("utf-8")),
             mock.call(b"\r\n"),
         ]
     )
-    assert r.text == str(encoded, "utf-8")
+    assert response.text == str(ENCODED, "utf-8")
 
     sock.fail_next_send = True
-    adafruit_requests.get("http://" + host + "/get2")
+    adafruit_requests.get("http://" + HOST + "/get2")
 
-    sock.connect.assert_called_once_with((ip, 80))
-    sock2.connect.assert_called_once_with((ip, 80))
+    sock.connect.assert_called_once_with((IP, 80))
+    sock2.connect.assert_called_once_with((IP, 80))
     # Make sure that the socket is closed after send fails.
     sock.close.assert_called_once()
     assert sock2.close.call_count == 0
     assert mocket.socket.call_count == 2
 
 
 def test_first_read_fails():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
+    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
     sock = mocket.Mocket(b"")
-    sock2 = mocket.Mocket(headers + encoded)
+    sock2 = mocket.Mocket(HEADERS + ENCODED)
     mocket.socket.call_count = 0  # Reset call count
     mocket.socket.side_effect = [sock, sock2]
 
     adafruit_requests.set_socket(mocket, mocket.interface)
-
-    r = adafruit_requests.get("http://" + host + "/testwifi/index.html")
+    adafruit_requests.get("http://" + HOST + "/testwifi/index.html")
 
     sock.send.assert_has_calls(
         [
             mock.call(b"testwifi/index.html"),
         ]
     )
 
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
-            mock.call(host.encode("utf-8")),
+            mock.call(HOST.encode("utf-8")),
             mock.call(b"\r\n"),
         ]
     )
 
     sock2.send.assert_has_calls(
         [
             mock.call(b"Host: "),
-            mock.call(host.encode("utf-8")),
+            mock.call(HOST.encode("utf-8")),
             mock.call(b"\r\n"),
         ]
     )
 
-    sock.connect.assert_called_once_with((ip, 80))
-    sock2.connect.assert_called_once_with((ip, 80))
+    sock.connect.assert_called_once_with((IP, 80))
+    sock2.connect.assert_called_once_with((IP, 80))
     # Make sure that the socket is closed after the first receive fails.
     sock.close.assert_called_once()
     assert mocket.socket.call_count == 2
 
 
 def test_second_tls_connect_fails():
-    mocket.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
-    sock2 = mocket.Mocket(headers + encoded)
-    sock3 = mocket.Mocket(headers + encoded)
+    mocket.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
+    sock2 = mocket.Mocket(HEADERS + ENCODED)
+    sock3 = mocket.Mocket(HEADERS + ENCODED)
     mocket.socket.call_count = 0  # Reset call count
     mocket.socket.side_effect = [sock, sock2, sock3]
     sock2.connect.side_effect = RuntimeError("error connecting")
 
     adafruit_requests.set_socket(mocket, mocket.interface)
-    r = adafruit_requests.get("https://" + host + "/testwifi/index.html")
+    response = adafruit_requests.get("https://" + HOST + "/testwifi/index.html")
 
     sock.send.assert_has_calls(
         [
             mock.call(b"testwifi/index.html"),
         ]
     )
 
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
-            mock.call(host.encode("utf-8")),
+            mock.call(HOST.encode("utf-8")),
             mock.call(b"\r\n"),
         ]
     )
-    assert r.text == str(encoded, "utf-8")
+    assert response.text == str(ENCODED, "utf-8")
 
     host2 = "test.adafruit.com"
-    r = adafruit_requests.get("https://" + host2 + "/get2")
+    response = adafruit_requests.get("https://" + host2 + "/get2")
 
-    sock.connect.assert_called_once_with((host, 443), mocket.interface.TLS_MODE)
+    sock.connect.assert_called_once_with((HOST, 443), mocket.interface.TLS_MODE)
     sock2.connect.assert_called_once_with((host2, 443), mocket.interface.TLS_MODE)
     sock3.connect.assert_called_once_with((host2, 443), mocket.interface.TLS_MODE)
     # Make sure that the socket is closed after send fails.
     sock.close.assert_called_once()
     sock2.close.assert_called_once()
     assert sock3.close.call_count == 0
     assert mocket.socket.call_count == 3
```

### Comparing `adafruit-circuitpython-requests-1.9.8/tests/mocket.py` & `adafruit-circuitpython-requests-1.9.9/tests/mocket.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
+""" Mock Socket """
+
 from unittest import mock
 
 
-class MocketPool:
+class MocketPool:  # pylint: disable=too-few-public-methods
+    """ Mock SocketPool """
+
     SOCK_STREAM = 0
 
     def __init__(self):
         self.getaddrinfo = mock.Mock()
         self.socket = mock.Mock()
 
 
-class Mocket:
+class Mocket:  # pylint: disable=too-few-public-methods
+    """ Mock Socket """
+
     def __init__(self, response):
         self.settimeout = mock.Mock()
         self.close = mock.Mock()
         self.connect = mock.Mock()
         self.send = mock.Mock(side_effect=self._send)
         self.readline = mock.Mock(side_effect=self._readline)
         self.recv = mock.Mock(side_effect=self._recv)
@@ -30,35 +36,39 @@
         if self.fail_next_send:
             self.fail_next_send = False
             return 0
         return len(data)
 
     def _readline(self):
         i = self._response.find(b"\r\n", self._position)
-        r = self._response[self._position : i + 2]
+        response = self._response[self._position : i + 2]
         self._position = i + 2
-        return r
+        return response
 
     def _recv(self, count):
         end = self._position + count
-        r = self._response[self._position : end]
+        response = self._response[self._position : end]
         self._position = end
-        return r
+        return response
 
     def _recv_into(self, buf, nbytes=0):
         assert isinstance(nbytes, int) and nbytes >= 0
         read = nbytes if nbytes > 0 else len(buf)
         remaining = len(self._response) - self._position
         if read > remaining:
             read = remaining
         end = self._position + read
         buf[:read] = self._response[self._position : end]
         self._position = end
         return read
 
 
-class SSLContext:
+class SSLContext:  # pylint: disable=too-few-public-methods
+    """ Mock SSL Context """
+
     def __init__(self):
         self.wrap_socket = mock.Mock(side_effect=self._wrap_socket)
 
-    def _wrap_socket(self, sock, server_hostname=None):
+    def _wrap_socket(
+        self, sock, server_hostname=None
+    ):  # pylint: disable=no-self-use,unused-argument
         return sock
```

### Comparing `adafruit-circuitpython-requests-1.9.8/tests/parse_test.py` & `adafruit-circuitpython-requests-1.9.9/tests/parse_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
-from unittest import mock
-import mocket
+"""  Parse Tests """
+
 import json
+import mocket
 import adafruit_requests
 
-ip = "1.2.3.4"
-host = "httpbin.org"
-response = {"Date": "July 25, 2019"}
-encoded = json.dumps(response).encode("utf-8")
+IP = "1.2.3.4"
+HOST = "httpbin.org"
+RESPONSE = {"Date": "July 25, 2019"}
+ENCODED = json.dumps(RESPONSE).encode("utf-8")
 # Padding here tests the case where a header line is exactly 32 bytes buffered by
 # aligning the Content-Type header after it.
-headers = "HTTP/1.0 200 OK\r\npadding: 000\r\nContent-Type: application/json\r\nContent-Length: {}\r\n\r\n".format(
-    len(encoded)
-).encode(
-    "utf-8"
+HEADERS = (
+    (
+        "HTTP/1.0 200 OK\r\npadding: 000\r\n"
+        "Content-Type: application/json\r\nContent-Length: {}\r\n\r\n"
+    )
+    .format(len(ENCODED))
+    .encode("utf-8")
 )
 
 
 def test_json():
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
-    r = s.get("http://" + host + "/get")
-    sock.connect.assert_called_once_with((ip, 80))
-    assert r.json() == response
+    requests_session = adafruit_requests.Session(pool)
+    response = requests_session.get("http://" + HOST + "/get")
+    sock.connect.assert_called_once_with((IP, 80))
+    assert response.json() == RESPONSE
```

### Comparing `adafruit-circuitpython-requests-1.9.8/tests/post_test.py` & `adafruit-circuitpython-requests-1.9.9/tests/post_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
+""" Post Tests """
+
 from unittest import mock
-import mocket
 import json
+import mocket
 import adafruit_requests
 
-ip = "1.2.3.4"
-host = "httpbin.org"
-response = {}
-encoded = json.dumps(response).encode("utf-8")
-headers = "HTTP/1.0 200 OK\r\nContent-Length: {}\r\n\r\n".format(len(encoded)).encode(
+IP = "1.2.3.4"
+HOST = "httpbin.org"
+RESPONSE = {}
+ENCODED = json.dumps(RESPONSE).encode("utf-8")
+HEADERS = "HTTP/1.0 200 OK\r\nContent-Length: {}\r\n\r\n".format(len(ENCODED)).encode(
     "utf-8"
 )
 
 
 def test_method():
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
-    r = s.post("http://" + host + "/post")
-    sock.connect.assert_called_once_with((ip, 80))
+    requests_session = adafruit_requests.Session(pool)
+    requests_session.post("http://" + HOST + "/post")
+    sock.connect.assert_called_once_with((IP, 80))
 
     sock.send.assert_has_calls(
         [
             mock.call(b"POST"),
             mock.call(b" /"),
             mock.call(b"post"),
             mock.call(b" HTTP/1.1\r\n"),
@@ -40,42 +42,42 @@
             mock.call(b"httpbin.org"),
         ]
     )
 
 
 def test_string():
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
+    requests_session = adafruit_requests.Session(pool)
     data = "31F"
-    r = s.post("http://" + host + "/post", data=data)
-    sock.connect.assert_called_once_with((ip, 80))
+    requests_session.post("http://" + HOST + "/post", data=data)
+    sock.connect.assert_called_once_with((IP, 80))
     sock.send.assert_called_with(b"31F")
 
 
 def test_form():
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
+    requests_session = adafruit_requests.Session(pool)
     data = {"Date": "July 25, 2019"}
-    r = s.post("http://" + host + "/post", data=data)
-    sock.connect.assert_called_once_with((ip, 80))
+    requests_session.post("http://" + HOST + "/post", data=data)
+    sock.connect.assert_called_once_with((IP, 80))
     sock.send.assert_called_with(b"Date=July 25, 2019")
 
 
 def test_json():
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(headers + encoded)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(HEADERS + ENCODED)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
+    requests_session = adafruit_requests.Session(pool)
     json_data = {"Date": "July 25, 2019"}
-    r = s.post("http://" + host + "/post", json=json_data)
-    sock.connect.assert_called_once_with((ip, 80))
+    requests_session.post("http://" + HOST + "/post", json=json_data)
+    sock.connect.assert_called_once_with((IP, 80))
     sock.send.assert_called_with(b'{"Date": "July 25, 2019"}')
```

### Comparing `adafruit-circuitpython-requests-1.9.8/tests/protocol_test.py` & `adafruit-circuitpython-requests-1.9.9/tests/protocol_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
+""" Protocol Tests """
+
 from unittest import mock
 import mocket
 import pytest
 import adafruit_requests
 
-ip = "1.2.3.4"
-host = "wifitest.adafruit.com"
-path = "/testwifi/index.html"
-text = b"This is a test of Adafruit WiFi!\r\nIf you can read this, its working :)"
-response = b"HTTP/1.0 200 OK\r\nContent-Length: 70\r\n\r\n" + text
+IP = "1.2.3.4"
+HOST = "wifitest.adafruit.com"
+PATH = "/testwifi/index.html"
+TEXT = b"This is a test of Adafruit WiFi!\r\nIf you can read this, its working :)"
+RESPONSE = b"HTTP/1.0 200 OK\r\nContent-Length: 70\r\n\r\n" + TEXT
 
 
 def test_get_https_no_ssl():
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(response)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
+    requests_session = adafruit_requests.Session(pool)
     with pytest.raises(RuntimeError):
-        r = s.get("https://" + host + path)
+        requests_session.get("https://" + HOST + PATH)
 
 
 def test_get_https_text():
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(response)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE)
     pool.socket.return_value = sock
     ssl = mocket.SSLContext()
 
-    s = adafruit_requests.Session(pool, ssl)
-    r = s.get("https://" + host + path)
+    requests_session = adafruit_requests.Session(pool, ssl)
+    response = requests_session.get("https://" + HOST + PATH)
 
-    sock.connect.assert_called_once_with((host, 443))
+    sock.connect.assert_called_once_with((HOST, 443))
 
     sock.send.assert_has_calls(
         [
             mock.call(b"GET"),
             mock.call(b" /"),
             mock.call(b"testwifi/index.html"),
             mock.call(b" HTTP/1.1\r\n"),
@@ -47,30 +49,30 @@
     )
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
             mock.call(b"wifitest.adafruit.com"),
         ]
     )
-    assert r.text == str(text, "utf-8")
+    assert response.text == str(TEXT, "utf-8")
 
     # Close isn't needed but can be called to release the socket early.
-    r.close()
+    response.close()
 
 
 def test_get_http_text():
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(response)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
-    r = s.get("http://" + host + path)
+    requests_session = adafruit_requests.Session(pool)
+    response = requests_session.get("http://" + HOST + PATH)
 
-    sock.connect.assert_called_once_with((ip, 80))
+    sock.connect.assert_called_once_with((IP, 80))
 
     sock.send.assert_has_calls(
         [
             mock.call(b"GET"),
             mock.call(b" /"),
             mock.call(b"testwifi/index.html"),
             mock.call(b" HTTP/1.1\r\n"),
@@ -78,28 +80,28 @@
     )
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
             mock.call(b"wifitest.adafruit.com"),
         ]
     )
-    assert r.text == str(text, "utf-8")
+    assert response.text == str(TEXT, "utf-8")
 
 
 def test_get_close():
     """Test that a response can be closed without the contents being accessed."""
     pool = mocket.MocketPool()
-    pool.getaddrinfo.return_value = ((None, None, None, None, (ip, 80)),)
-    sock = mocket.Mocket(response)
+    pool.getaddrinfo.return_value = ((None, None, None, None, (IP, 80)),)
+    sock = mocket.Mocket(RESPONSE)
     pool.socket.return_value = sock
 
-    s = adafruit_requests.Session(pool)
-    r = s.get("http://" + host + path)
+    requests_session = adafruit_requests.Session(pool)
+    response = requests_session.get("http://" + HOST + PATH)
 
-    sock.connect.assert_called_once_with((ip, 80))
+    sock.connect.assert_called_once_with((IP, 80))
 
     sock.send.assert_has_calls(
         [
             mock.call(b"GET"),
             mock.call(b" /"),
             mock.call(b"testwifi/index.html"),
             mock.call(b" HTTP/1.1\r\n"),
@@ -107,8 +109,8 @@
     )
     sock.send.assert_has_calls(
         [
             mock.call(b"Host: "),
             mock.call(b"wifitest.adafruit.com"),
         ]
     )
-    r.close()
+    response.close()
```

