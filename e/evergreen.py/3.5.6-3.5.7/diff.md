# Comparing `tmp/evergreen.py-3.5.6.tar.gz` & `tmp/evergreen.py-3.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evergreen.py-3.5.6.tar", max compression
+gzip compressed data, was "evergreen.py-3.5.7.tar", max compression
```

## Comparing `evergreen.py-3.5.6.tar` & `evergreen.py-3.5.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11336 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/LICENSE
--rw-r--r--   0        0        0     5548 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/README.md
--rw-r--r--   0        0        0     1375 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/pyproject.toml
--rw-r--r--   0        0        0      717 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/__init__.py
--rw-r--r--   0        0        0     1453 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/alias.py
--rw-r--r--   0        0        0    51068 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/api.py
--rw-r--r--   0        0        0     2264 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/api_requests.py
--rw-r--r--   0        0        0     3039 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/base.py
--rw-r--r--   0        0        0     4558 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/build.py
--rw-r--r--   0        0        0        0 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/cli/__init__.py
--rw-r--r--   0        0        0    16690 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/cli/main.py
--rw-r--r--   0        0        0     1538 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/commitqueue.py
--rw-r--r--   0        0        0     1745 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/config.py
--rw-r--r--   0        0        0     7450 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/distro.py
--rw-r--r--   0        0        0        0 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/errors/__init__.py
--rw-r--r--   0        0        0     1444 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/errors/exceptions.py
--rw-r--r--   0        0        0     3381 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/host.py
--rw-r--r--   0        0        0     1788 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/manifest.py
--rw-r--r--   0        0        0        0 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/metrics/__init__.py
--rw-r--r--   0        0        0    15510 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/metrics/buildmetrics.py
--rw-r--r--   0        0        0     9141 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/metrics/versionmetrics.py
--rw-r--r--   0        0        0     6576 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/patch.py
--rw-r--r--   0        0        0    10706 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/performance_results.py
--rw-r--r--   0        0        0     1737 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/project.py
--rw-r--r--   0        0        0        0 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/py.typed
--rw-r--r--   0        0        0     1250 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/resource_type_permissions.py
--rw-r--r--   0        0        0     1633 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/stats.py
--rw-r--r--   0        0        0    14468 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/task.py
--rw-r--r--   0        0        0     2668 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/task_annotations.py
--rw-r--r--   0        0        0     1271 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/task_reliability.py
--rw-r--r--   0        0        0     1741 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/tst.py
--rw-r--r--   0        0        0      585 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/users_for_role.py
--rw-r--r--   0        0        0     3424 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/util.py
--rw-r--r--   0        0        0     8010 2023-04-14 16:45:11.283889 evergreen.py-3.5.6/src/evergreen/version.py
--rw-r--r--   0        0        0     6737 2023-04-14 16:45:49.049163 evergreen.py-3.5.6/setup.py
--rw-r--r--   0        0        0     6455 2023-04-14 16:45:49.049752 evergreen.py-3.5.6/PKG-INFO
+-rw-r--r--   0        0        0    11336 2023-04-21 22:35:53.324108 evergreen.py-3.5.7/LICENSE
+-rw-r--r--   0        0        0     6438 2023-04-21 22:35:53.324108 evergreen.py-3.5.7/README.md
+-rw-r--r--   0        0        0     1375 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/pyproject.toml
+-rw-r--r--   0        0        0      717 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/__init__.py
+-rw-r--r--   0        0        0     1453 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/alias.py
+-rw-r--r--   0        0        0    51068 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/api.py
+-rw-r--r--   0        0        0     2264 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/api_requests.py
+-rw-r--r--   0        0        0     3039 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/base.py
+-rw-r--r--   0        0        0     4558 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/build.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/cli/__init__.py
+-rw-r--r--   0        0        0    16690 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/cli/main.py
+-rw-r--r--   0        0        0     1538 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/commitqueue.py
+-rw-r--r--   0        0        0     1745 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/config.py
+-rw-r--r--   0        0        0     7450 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/distro.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/errors/__init__.py
+-rw-r--r--   0        0        0     1444 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/errors/exceptions.py
+-rw-r--r--   0        0        0     3381 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/host.py
+-rw-r--r--   0        0        0     1788 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/manifest.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/metrics/__init__.py
+-rw-r--r--   0        0        0    15510 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/metrics/buildmetrics.py
+-rw-r--r--   0        0        0     9141 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/metrics/versionmetrics.py
+-rw-r--r--   0        0        0     6576 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/patch.py
+-rw-r--r--   0        0        0    10706 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/performance_results.py
+-rw-r--r--   0        0        0     1737 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/project.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/py.typed
+-rw-r--r--   0        0        0     1250 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/resource_type_permissions.py
+-rw-r--r--   0        0        0     1633 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/stats.py
+-rw-r--r--   0        0        0    14468 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/task.py
+-rw-r--r--   0        0        0     2668 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/task_annotations.py
+-rw-r--r--   0        0        0     1271 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/task_reliability.py
+-rw-r--r--   0        0        0     1741 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/tst.py
+-rw-r--r--   0        0        0      585 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/users_for_role.py
+-rw-r--r--   0        0        0     3424 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/util.py
+-rw-r--r--   0        0        0     8010 2023-04-21 22:35:53.328108 evergreen.py-3.5.7/src/evergreen/version.py
+-rw-r--r--   0        0        0     7659 2023-04-21 22:36:36.706465 evergreen.py-3.5.7/setup.py
+-rw-r--r--   0        0        0     7345 2023-04-21 22:36:36.707100 evergreen.py-3.5.7/PKG-INFO
```

### Comparing `evergreen.py-3.5.6/LICENSE` & `evergreen.py-3.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/README.md` & `evergreen.py-3.5.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,76 +10,82 @@
 1. [Description](#description)
 2. [Getting Help](#getting-help)
 3. [Dependencies](#dependencies)
 4. [Installation](#installation)
 5. [Usage](#usage)
 6. [Documentation](#documentation)
 7. [Contributor's Guide](#contributors-guide)
-    - [Setting up a local development environment](#setting-up-a-local-development-environment)
-    - [Linting/formatting](#lintingformatting)
-    - [Running tests](#running-tests)
-    - [Automatically running checks on commit](#automatically-running-checks-on-commit)
-    - [Versioning](#versioning)
-    - [Code Review](#code-review)
-    - [Deployment](#deployment)
+   - [Setting up a local development environment](#setting-up-a-local-development-environment)
+   - [Linting/formatting](#lintingformatting)
+   - [Running tests](#running-tests)
+   - [Automatically running checks on commit](#automatically-running-checks-on-commit)
+   - [Versioning](#versioning)
+   - [Code Review](#code-review)
+   - [Deployment](#deployment)
 
 ## Description
 
 This is a Python client library for interacting with Evergreen and Evergreen objects. It currently only
 supports the V2 version of Evergreen's api. It can be used either by Python code in a separate application
 or on the command line to get data about Evergreen objects quickly and easily.
 
 ## Getting Help
 
 ### What's the right channel to ask my question?
+
 If you have a question about evergreen.py, please mention @dag-on-call in
 slack channel [#evergreen-users](https://mongodb.slack.com/messages/#evergreen-users/),
 or email us at
 dev-prod-dag@mongodb.com.
 
 ### How can I request a change/report a bug in evergreen.py?
+
 Create a [DAG ticket](https://jira.mongodb.org/projects/DAG).
 
 ### What should I include in my ticket or #evergreen-users question?
+
 Since #evergreen-users questions are interrupts,
 please include as much information as possible.
 This can help avoid long information-gathering threads.
 
 Please include the following:
-* **Motivation for Request**
-  * provide us the motivation for this change.
-* **Context**
-  * provide some background contexts for this issue.
-* **Description**
-  * provide some descriptions on how this issue happened.
+
+- **Motivation for Request**
+  - provide us the motivation for this change.
+- **Context**
+  - provide some background contexts for this issue.
+- **Description**
+  - provide some descriptions on how this issue happened.
 
 ## Dependencies
 
-* Python 3.7 or later
+- Python 3.7 or later
 
 ## Installation
 
 ```bash
 $ pip install evergreen.py
 ```
 
 ## Usage
 
 This client can be used either in code or directly via the command line.
 
 In code:
+
 ```python
 >> from evergreen.api import EvgAuth, EvergreenApi
 >> api = EvergreenApi.get_api(EvgAuth('david.bradford', '***'))
 >> project = api.project_by_id('mongodb-mongo-master')
 >> project.display_name
 'MongoDB (master)'
 ```
 
 Cli:
+
 ```bash
 $ evg-api --json list-hosts
 {
     "host_id": "host num 0",
     "host_url": "host.num.com",
     "distro": {
         "distro_id": "ubuntu1804-build",
@@ -98,32 +104,58 @@
         "version_id": null,
         "build_id": null
     },
     "user_host": false
 }
 ```
 
-The `patch_from_diff` API requires the Evergreen CLI to be installed. Add the following to the host's DOCKERFILE:
+The `patch_from_diff` API requires the Evergreen CLI to be installed.
+
+Add the following to the host's DOCKERFILE:
 
 ```bash
 RUN wget https://evergreen.mongodb.com/clients/linux_amd64/evergreen
 RUN chmod +x evergreen
 ENV PATH="/project:$PATH"
 ```
 
+You will need to provide an .evergreen.yml file with credentials to use the CLI. Assuming you are using the [web-app](https://github.com/10gen/helm-charts/tree/master/charts/web-app) chart this can be done by [mounting](https://kanopy.corp.mongodb.com/docs/getting_started/application_configuration/#configuration-filesvolumes) [kubernetes secrets](https://kanopy.corp.mongodb.com/docs/cheatsheet/#interacting-with-kubernetes-secrets) in your pod.
+
+Store the secret in the cluster:
+
+```bash
+kubectl create secret generic <secret_name> --from-file .evergreen.yml --namespace <namespace>
+```
+
+In environments/deployment.yml configure the file to be mounted and linked to the correct location:
+
+```yaml
+volumeSecrets:
+  - name: <secret_name>
+    path: /etc/secrets
+lifecycle:
+  postStart:
+    type: exec
+    command:
+      - /bin/sh
+      - -c
+      - ln -sf /etc/secrets/.evergreen.yml
+```
+
 ## Documentation
 
 You can find the documentation [here](https://evergreen-ci.github.io/evergreen.py/).
 
 ## Contributor's Guide
 
 ### Setting up a local development environment
 
 #### Requirements
-* Poetry 1.1 or later
+
+- Poetry 1.1 or later
 
 You will need Evergreen credentials on your local machine to use this library or the attached CLI. You
 can set up your credentials by following the link [here](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool).
 
 ### Linting/formatting
 
 This project uses [black](https://github.com/psf/black) for formatting.
```

### Comparing `evergreen.py-3.5.6/pyproject.toml` & `evergreen.py-3.5.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evergreen.py"
-version = "3.5.6"
+version = "3.5.7"
 description = "Python client for the Evergreen API"
 authors = [
     "Dev Prod DAG <dev-prod-dag@mongodb.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/evergreen-ci/evergreen.py"
```

### Comparing `evergreen.py-3.5.6/src/evergreen/__init__.py` & `evergreen.py-3.5.7/src/evergreen/__init__.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/alias.py` & `evergreen.py-3.5.7/src/evergreen/alias.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/api.py` & `evergreen.py-3.5.7/src/evergreen/api.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/api_requests.py` & `evergreen.py-3.5.7/src/evergreen/api_requests.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/base.py` & `evergreen.py-3.5.7/src/evergreen/base.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/build.py` & `evergreen.py-3.5.7/src/evergreen/build.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/cli/main.py` & `evergreen.py-3.5.7/src/evergreen/cli/main.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/commitqueue.py` & `evergreen.py-3.5.7/src/evergreen/commitqueue.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/config.py` & `evergreen.py-3.5.7/src/evergreen/config.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/distro.py` & `evergreen.py-3.5.7/src/evergreen/distro.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/errors/exceptions.py` & `evergreen.py-3.5.7/src/evergreen/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/host.py` & `evergreen.py-3.5.7/src/evergreen/host.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/manifest.py` & `evergreen.py-3.5.7/src/evergreen/manifest.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/metrics/buildmetrics.py` & `evergreen.py-3.5.7/src/evergreen/metrics/buildmetrics.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/metrics/versionmetrics.py` & `evergreen.py-3.5.7/src/evergreen/metrics/versionmetrics.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/patch.py` & `evergreen.py-3.5.7/src/evergreen/patch.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/performance_results.py` & `evergreen.py-3.5.7/src/evergreen/performance_results.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/project.py` & `evergreen.py-3.5.7/src/evergreen/project.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/resource_type_permissions.py` & `evergreen.py-3.5.7/src/evergreen/resource_type_permissions.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/stats.py` & `evergreen.py-3.5.7/src/evergreen/stats.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/task.py` & `evergreen.py-3.5.7/src/evergreen/task.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/task_annotations.py` & `evergreen.py-3.5.7/src/evergreen/task_annotations.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/task_reliability.py` & `evergreen.py-3.5.7/src/evergreen/task_reliability.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/tst.py` & `evergreen.py-3.5.7/src/evergreen/tst.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/users_for_role.py` & `evergreen.py-3.5.7/src/evergreen/users_for_role.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/util.py` & `evergreen.py-3.5.7/src/evergreen/util.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/src/evergreen/version.py` & `evergreen.py-3.5.7/src/evergreen/version.py`

 * *Files identical despite different names*

### Comparing `evergreen.py-3.5.6/setup.py` & `evergreen.py-3.5.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,17 +20,17 @@
  'tenacity>=5']
 
 entry_points = \
 {'console_scripts': ['evg-api = evergreen.cli.main:main']}
 
 setup_kwargs = {
     'name': 'evergreen.py',
-    'version': '3.5.6',
+    'version': '3.5.7',
     'description': 'Python client for the Evergreen API',
-    'long_description': '# Evergreen.py\n\nA client library for the Evergreen API written in python. Currently supports the V2 version of\nthe API. For more details, see https://github.com/evergreen-ci/evergreen/wiki/REST-V2-Usage.\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evergreen.py) [![PyPI](https://img.shields.io/pypi/v/evergreen.py.svg)](https://pypi.org/project/evergreen.py/) [![Coverage Status](https://coveralls.io/repos/github/evergreen-ci/evergreen.py/badge.svg?branch=master)](https://coveralls.io/github/evergreen-ci/evergreen.py?branch=master)\n\n## Table of contents\n\n1. [Description](#description)\n2. [Getting Help](#getting-help)\n3. [Dependencies](#dependencies)\n4. [Installation](#installation)\n5. [Usage](#usage)\n6. [Documentation](#documentation)\n7. [Contributor\'s Guide](#contributors-guide)\n    - [Setting up a local development environment](#setting-up-a-local-development-environment)\n    - [Linting/formatting](#lintingformatting)\n    - [Running tests](#running-tests)\n    - [Automatically running checks on commit](#automatically-running-checks-on-commit)\n    - [Versioning](#versioning)\n    - [Code Review](#code-review)\n    - [Deployment](#deployment)\n\n## Description\n\nThis is a Python client library for interacting with Evergreen and Evergreen objects. It currently only\nsupports the V2 version of Evergreen\'s api. It can be used either by Python code in a separate application\nor on the command line to get data about Evergreen objects quickly and easily.\n\n## Getting Help\n\n### What\'s the right channel to ask my question?\nIf you have a question about evergreen.py, please mention @dag-on-call in\nslack channel [#evergreen-users](https://mongodb.slack.com/messages/#evergreen-users/),\nor email us at\ndev-prod-dag@mongodb.com.\n\n### How can I request a change/report a bug in evergreen.py?\nCreate a [DAG ticket](https://jira.mongodb.org/projects/DAG).\n\n### What should I include in my ticket or #evergreen-users question?\nSince #evergreen-users questions are interrupts,\nplease include as much information as possible.\nThis can help avoid long information-gathering threads.\n\nPlease include the following:\n* **Motivation for Request**\n  * provide us the motivation for this change.\n* **Context**\n  * provide some background contexts for this issue.\n* **Description**\n  * provide some descriptions on how this issue happened.\n\n## Dependencies\n\n* Python 3.7 or later\n\n## Installation\n\n```bash\n$ pip install evergreen.py\n```\n\n## Usage\n\nThis client can be used either in code or directly via the command line.\n\nIn code:\n```python\n>> from evergreen.api import EvgAuth, EvergreenApi\n>> api = EvergreenApi.get_api(EvgAuth(\'david.bradford\', \'***\'))\n>> project = api.project_by_id(\'mongodb-mongo-master\')\n>> project.display_name\n\'MongoDB (master)\'\n```\n\nCli:\n```bash\n$ evg-api --json list-hosts\n{\n    "host_id": "host num 0",\n    "host_url": "host.num.com",\n    "distro": {\n        "distro_id": "ubuntu1804-build",\n        "provider": "static",\n        "image_id": ""\n    },\n    "provisioned": true,\n    "started_by": "mci",\n    "host_type": "",\n    "user": "mci-exec",\n    "status": "running",\n    "running_task": {\n        "task_id": null,\n        "name": null,\n        "dispatch_time": null,\n        "version_id": null,\n        "build_id": null\n    },\n    "user_host": false\n}\n```\n\nThe `patch_from_diff` API requires the Evergreen CLI to be installed. Add the following to the host\'s DOCKERFILE:\n\n```bash\nRUN wget https://evergreen.mongodb.com/clients/linux_amd64/evergreen\nRUN chmod +x evergreen\nENV PATH="/project:$PATH"\n```\n\n## Documentation\n\nYou can find the documentation [here](https://evergreen-ci.github.io/evergreen.py/).\n\n## Contributor\'s Guide\n\n### Setting up a local development environment\n\n#### Requirements\n* Poetry 1.1 or later\n\nYou will need Evergreen credentials on your local machine to use this library or the attached CLI. You\ncan set up your credentials by following the link [here](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool).\n\n### Linting/formatting\n\nThis project uses [black](https://github.com/psf/black) for formatting.\n\n```bash\npoetry run black src tests\n```\n\n### Running tests\n\n```bash\npoetry run pytest\n```\n\nThere are a few tests that are slow running. These tests are not run by default, but can be included\nby setting the env variable RUN_SLOW_TESTS to any value.\n\n```\n$ RUN_SLOW_TEST=1 poetry run pytest\n```\n\nTo get code coverage information:\n\n```\n$ poetry run pytest --cov=src --cov-report=html\n```\n\n### Automatically running checks on commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time. To enable pre-commit on your local repository run:\n\n```bash\n$ poetry run pre-commit install\n```\n\n### Versioning\n\nBefore deploying a new version, please update the `CHANGELOG.md` file with a description of what\nis being changed.\n\nDeploys to [PyPi](https://pypi.org/project/evergreen.py/) are done automatically on merges to master.\nIn order to avoid overwriting a previous deploy, the version should be updated on all changes. The\n[semver](https://semver.org/) versioning scheme should be used for determining the version number.\n\nThe version is found in the `pyproject.toml` file.\n\n### Code Review\n\nThis project uses the [Evergreen Commit Queue](https://github.com/evergreen-ci/evergreen/wiki/Commit-Queue#pr).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to production is automatically triggered on merges to master.\n',
+    'long_description': '# Evergreen.py\n\nA client library for the Evergreen API written in python. Currently supports the V2 version of\nthe API. For more details, see https://github.com/evergreen-ci/evergreen/wiki/REST-V2-Usage.\n\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/evergreen.py) [![PyPI](https://img.shields.io/pypi/v/evergreen.py.svg)](https://pypi.org/project/evergreen.py/) [![Coverage Status](https://coveralls.io/repos/github/evergreen-ci/evergreen.py/badge.svg?branch=master)](https://coveralls.io/github/evergreen-ci/evergreen.py?branch=master)\n\n## Table of contents\n\n1. [Description](#description)\n2. [Getting Help](#getting-help)\n3. [Dependencies](#dependencies)\n4. [Installation](#installation)\n5. [Usage](#usage)\n6. [Documentation](#documentation)\n7. [Contributor\'s Guide](#contributors-guide)\n   - [Setting up a local development environment](#setting-up-a-local-development-environment)\n   - [Linting/formatting](#lintingformatting)\n   - [Running tests](#running-tests)\n   - [Automatically running checks on commit](#automatically-running-checks-on-commit)\n   - [Versioning](#versioning)\n   - [Code Review](#code-review)\n   - [Deployment](#deployment)\n\n## Description\n\nThis is a Python client library for interacting with Evergreen and Evergreen objects. It currently only\nsupports the V2 version of Evergreen\'s api. It can be used either by Python code in a separate application\nor on the command line to get data about Evergreen objects quickly and easily.\n\n## Getting Help\n\n### What\'s the right channel to ask my question?\n\nIf you have a question about evergreen.py, please mention @dag-on-call in\nslack channel [#evergreen-users](https://mongodb.slack.com/messages/#evergreen-users/),\nor email us at\ndev-prod-dag@mongodb.com.\n\n### How can I request a change/report a bug in evergreen.py?\n\nCreate a [DAG ticket](https://jira.mongodb.org/projects/DAG).\n\n### What should I include in my ticket or #evergreen-users question?\n\nSince #evergreen-users questions are interrupts,\nplease include as much information as possible.\nThis can help avoid long information-gathering threads.\n\nPlease include the following:\n\n- **Motivation for Request**\n  - provide us the motivation for this change.\n- **Context**\n  - provide some background contexts for this issue.\n- **Description**\n  - provide some descriptions on how this issue happened.\n\n## Dependencies\n\n- Python 3.7 or later\n\n## Installation\n\n```bash\n$ pip install evergreen.py\n```\n\n## Usage\n\nThis client can be used either in code or directly via the command line.\n\nIn code:\n\n```python\n>> from evergreen.api import EvgAuth, EvergreenApi\n>> api = EvergreenApi.get_api(EvgAuth(\'david.bradford\', \'***\'))\n>> project = api.project_by_id(\'mongodb-mongo-master\')\n>> project.display_name\n\'MongoDB (master)\'\n```\n\nCli:\n\n```bash\n$ evg-api --json list-hosts\n{\n    "host_id": "host num 0",\n    "host_url": "host.num.com",\n    "distro": {\n        "distro_id": "ubuntu1804-build",\n        "provider": "static",\n        "image_id": ""\n    },\n    "provisioned": true,\n    "started_by": "mci",\n    "host_type": "",\n    "user": "mci-exec",\n    "status": "running",\n    "running_task": {\n        "task_id": null,\n        "name": null,\n        "dispatch_time": null,\n        "version_id": null,\n        "build_id": null\n    },\n    "user_host": false\n}\n```\n\nThe `patch_from_diff` API requires the Evergreen CLI to be installed.\n\nAdd the following to the host\'s DOCKERFILE:\n\n```bash\nRUN wget https://evergreen.mongodb.com/clients/linux_amd64/evergreen\nRUN chmod +x evergreen\nENV PATH="/project:$PATH"\n```\n\nYou will need to provide an .evergreen.yml file with credentials to use the CLI. Assuming you are using the [web-app](https://github.com/10gen/helm-charts/tree/master/charts/web-app) chart this can be done by [mounting](https://kanopy.corp.mongodb.com/docs/getting_started/application_configuration/#configuration-filesvolumes) [kubernetes secrets](https://kanopy.corp.mongodb.com/docs/cheatsheet/#interacting-with-kubernetes-secrets) in your pod.\n\nStore the secret in the cluster:\n\n```bash\nkubectl create secret generic <secret_name> --from-file .evergreen.yml --namespace <namespace>\n```\n\nIn environments/deployment.yml configure the file to be mounted and linked to the correct location:\n\n```yaml\nvolumeSecrets:\n  - name: <secret_name>\n    path: /etc/secrets\nlifecycle:\n  postStart:\n    type: exec\n    command:\n      - /bin/sh\n      - -c\n      - ln -sf /etc/secrets/.evergreen.yml\n```\n\n## Documentation\n\nYou can find the documentation [here](https://evergreen-ci.github.io/evergreen.py/).\n\n## Contributor\'s Guide\n\n### Setting up a local development environment\n\n#### Requirements\n\n- Poetry 1.1 or later\n\nYou will need Evergreen credentials on your local machine to use this library or the attached CLI. You\ncan set up your credentials by following the link [here](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool).\n\n### Linting/formatting\n\nThis project uses [black](https://github.com/psf/black) for formatting.\n\n```bash\npoetry run black src tests\n```\n\n### Running tests\n\n```bash\npoetry run pytest\n```\n\nThere are a few tests that are slow running. These tests are not run by default, but can be included\nby setting the env variable RUN_SLOW_TESTS to any value.\n\n```\n$ RUN_SLOW_TEST=1 poetry run pytest\n```\n\nTo get code coverage information:\n\n```\n$ poetry run pytest --cov=src --cov-report=html\n```\n\n### Automatically running checks on commit\n\nThis project has [pre-commit](https://pre-commit.com/) configured. Pre-commit will run\nconfigured checks at git commit time. To enable pre-commit on your local repository run:\n\n```bash\n$ poetry run pre-commit install\n```\n\n### Versioning\n\nBefore deploying a new version, please update the `CHANGELOG.md` file with a description of what\nis being changed.\n\nDeploys to [PyPi](https://pypi.org/project/evergreen.py/) are done automatically on merges to master.\nIn order to avoid overwriting a previous deploy, the version should be updated on all changes. The\n[semver](https://semver.org/) versioning scheme should be used for determining the version number.\n\nThe version is found in the `pyproject.toml` file.\n\n### Code Review\n\nThis project uses the [Evergreen Commit Queue](https://github.com/evergreen-ci/evergreen/wiki/Commit-Queue#pr).\nAdd a PR comment with `evergreen merge` to trigger a merge.\n\n### Deployment\n\nDeployment to production is automatically triggered on merges to master.\n',
     'author': 'Dev Prod DAG',
     'author_email': 'dev-prod-dag@mongodb.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/evergreen-ci/evergreen.py',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `evergreen.py-3.5.6/PKG-INFO` & `evergreen.py-3.5.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evergreen.py
-Version: 3.5.6
+Version: 3.5.7
 Summary: Python client for the Evergreen API
 Home-page: https://github.com/evergreen-ci/evergreen.py
 License: Apache-2.0
 Author: Dev Prod DAG
 Author-email: dev-prod-dag@mongodb.com
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -35,76 +35,82 @@
 1. [Description](#description)
 2. [Getting Help](#getting-help)
 3. [Dependencies](#dependencies)
 4. [Installation](#installation)
 5. [Usage](#usage)
 6. [Documentation](#documentation)
 7. [Contributor's Guide](#contributors-guide)
-    - [Setting up a local development environment](#setting-up-a-local-development-environment)
-    - [Linting/formatting](#lintingformatting)
-    - [Running tests](#running-tests)
-    - [Automatically running checks on commit](#automatically-running-checks-on-commit)
-    - [Versioning](#versioning)
-    - [Code Review](#code-review)
-    - [Deployment](#deployment)
+   - [Setting up a local development environment](#setting-up-a-local-development-environment)
+   - [Linting/formatting](#lintingformatting)
+   - [Running tests](#running-tests)
+   - [Automatically running checks on commit](#automatically-running-checks-on-commit)
+   - [Versioning](#versioning)
+   - [Code Review](#code-review)
+   - [Deployment](#deployment)
 
 ## Description
 
 This is a Python client library for interacting with Evergreen and Evergreen objects. It currently only
 supports the V2 version of Evergreen's api. It can be used either by Python code in a separate application
 or on the command line to get data about Evergreen objects quickly and easily.
 
 ## Getting Help
 
 ### What's the right channel to ask my question?
+
 If you have a question about evergreen.py, please mention @dag-on-call in
 slack channel [#evergreen-users](https://mongodb.slack.com/messages/#evergreen-users/),
 or email us at
 dev-prod-dag@mongodb.com.
 
 ### How can I request a change/report a bug in evergreen.py?
+
 Create a [DAG ticket](https://jira.mongodb.org/projects/DAG).
 
 ### What should I include in my ticket or #evergreen-users question?
+
 Since #evergreen-users questions are interrupts,
 please include as much information as possible.
 This can help avoid long information-gathering threads.
 
 Please include the following:
-* **Motivation for Request**
-  * provide us the motivation for this change.
-* **Context**
-  * provide some background contexts for this issue.
-* **Description**
-  * provide some descriptions on how this issue happened.
+
+- **Motivation for Request**
+  - provide us the motivation for this change.
+- **Context**
+  - provide some background contexts for this issue.
+- **Description**
+  - provide some descriptions on how this issue happened.
 
 ## Dependencies
 
-* Python 3.7 or later
+- Python 3.7 or later
 
 ## Installation
 
 ```bash
 $ pip install evergreen.py
 ```
 
 ## Usage
 
 This client can be used either in code or directly via the command line.
 
 In code:
+
 ```python
 >> from evergreen.api import EvgAuth, EvergreenApi
 >> api = EvergreenApi.get_api(EvgAuth('david.bradford', '***'))
 >> project = api.project_by_id('mongodb-mongo-master')
 >> project.display_name
 'MongoDB (master)'
 ```
 
 Cli:
+
 ```bash
 $ evg-api --json list-hosts
 {
     "host_id": "host num 0",
     "host_url": "host.num.com",
     "distro": {
         "distro_id": "ubuntu1804-build",
@@ -123,32 +129,58 @@
         "version_id": null,
         "build_id": null
     },
     "user_host": false
 }
 ```
 
-The `patch_from_diff` API requires the Evergreen CLI to be installed. Add the following to the host's DOCKERFILE:
+The `patch_from_diff` API requires the Evergreen CLI to be installed.
+
+Add the following to the host's DOCKERFILE:
 
 ```bash
 RUN wget https://evergreen.mongodb.com/clients/linux_amd64/evergreen
 RUN chmod +x evergreen
 ENV PATH="/project:$PATH"
 ```
 
+You will need to provide an .evergreen.yml file with credentials to use the CLI. Assuming you are using the [web-app](https://github.com/10gen/helm-charts/tree/master/charts/web-app) chart this can be done by [mounting](https://kanopy.corp.mongodb.com/docs/getting_started/application_configuration/#configuration-filesvolumes) [kubernetes secrets](https://kanopy.corp.mongodb.com/docs/cheatsheet/#interacting-with-kubernetes-secrets) in your pod.
+
+Store the secret in the cluster:
+
+```bash
+kubectl create secret generic <secret_name> --from-file .evergreen.yml --namespace <namespace>
+```
+
+In environments/deployment.yml configure the file to be mounted and linked to the correct location:
+
+```yaml
+volumeSecrets:
+  - name: <secret_name>
+    path: /etc/secrets
+lifecycle:
+  postStart:
+    type: exec
+    command:
+      - /bin/sh
+      - -c
+      - ln -sf /etc/secrets/.evergreen.yml
+```
+
 ## Documentation
 
 You can find the documentation [here](https://evergreen-ci.github.io/evergreen.py/).
 
 ## Contributor's Guide
 
 ### Setting up a local development environment
 
 #### Requirements
-* Poetry 1.1 or later
+
+- Poetry 1.1 or later
 
 You will need Evergreen credentials on your local machine to use this library or the attached CLI. You
 can set up your credentials by following the link [here](https://github.com/evergreen-ci/evergreen/wiki/Using-the-Command-Line-Tool#downloading-the-command-line-tool).
 
 ### Linting/formatting
 
 This project uses [black](https://github.com/psf/black) for formatting.
```

