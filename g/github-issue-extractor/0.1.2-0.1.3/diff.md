# Comparing `tmp/github_issue_extractor-0.1.2.tar.gz` & `tmp/github_issue_extractor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_issue_extractor-0.1.2.tar", last modified: Sat Apr 22 21:06:42 2023, max compression
+gzip compressed data, was "github_issue_extractor-0.1.3.tar", last modified: Sat Apr 22 21:44:49 2023, max compression
```

## Comparing `github_issue_extractor-0.1.2.tar` & `github_issue_extractor-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:06:42.063111 github_issue_extractor-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-22 21:06:25.000000 github_issue_extractor-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-22 21:06:42.063111 github_issue_extractor-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-22 21:06:25.000000 github_issue_extractor-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:06:42.063111 github_issue_extractor-0.1.2/github_issue_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-22 21:06:42.000000 github_issue_extractor-0.1.2/github_issue_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-22 21:06:42.000000 github_issue_extractor-0.1.2/github_issue_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:06:42.000000 github_issue_extractor-0.1.2/github_issue_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 21:06:42.000000 github_issue_extractor-0.1.2/github_issue_extractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:06:42.000000 github_issue_extractor-0.1.2/github_issue_extractor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 21:06:42.063111 github_issue_extractor-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-22 21:06:25.000000 github_issue_extractor-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:44:49.052898 github_issue_extractor-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-22 21:44:37.000000 github_issue_extractor-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-22 21:44:49.052898 github_issue_extractor-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-22 21:44:37.000000 github_issue_extractor-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:44:49.052898 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 21:44:49.052898 github_issue_extractor-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-22 21:44:37.000000 github_issue_extractor-0.1.3/setup.py
```

### Comparing `github_issue_extractor-0.1.2/LICENSE` & `github_issue_extractor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `github_issue_extractor-0.1.2/PKG-INFO` & `github_issue_extractor-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github_issue_extractor
-Version: 0.1.2
+Version: 0.1.3
 Summary: GitHubIssueExtractor
 Home-page: https://github.com/ssinha2103/github-issues_to_excel
 Author: Sudarshan Sinha
 Author-email: s.sinha2103@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,21 +21,26 @@
 - Filter issues by milestone number
 - Requires a GitHub access token for authentication
 
 ## Prerequisites
 - Python 3.x
 - `requests` library
 
-## Installation
+## Installation 
+ Follow either `Installation Type 1` or `Installation Type 2`
+
+### Installation Type 1
+1. `pip install github-issue-extractor`
+
+### Installation Type 2
 1. Clone the repository:
     `git clone https://github.com/ssinha2103/github-issues_to_excel`
 2. Install the required dependencies:
     `pip install -r requirements.txt`
 
-
 ## Usage
 To use the GitHub Issue Extractor, simply import the class and create an instance with the required parameters:
 
 ```python
 from github_issue_extractor import GitHubIssueExtractor
 
 milestone_number = 1
```

### Comparing `github_issue_extractor-0.1.2/README.md` & `github_issue_extractor-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,21 +7,26 @@
 - Filter issues by milestone number
 - Requires a GitHub access token for authentication
 
 ## Prerequisites
 - Python 3.x
 - `requests` library
 
-## Installation
+## Installation 
+ Follow either `Installation Type 1` or `Installation Type 2`
+
+### Installation Type 1
+1. `pip install github-issue-extractor`
+
+### Installation Type 2
 1. Clone the repository:
     `git clone https://github.com/ssinha2103/github-issues_to_excel`
 2. Install the required dependencies:
     `pip install -r requirements.txt`
 
-
 ## Usage
 To use the GitHub Issue Extractor, simply import the class and create an instance with the required parameters:
 
 ```python
 from github_issue_extractor import GitHubIssueExtractor
 
 milestone_number = 1
```

### Comparing `github_issue_extractor-0.1.2/github_issue_extractor.egg-info/PKG-INFO` & `github_issue_extractor-0.1.3/github_issue_extractor.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github-issue-extractor
-Version: 0.1.2
+Version: 0.1.3
 Summary: GitHubIssueExtractor
 Home-page: https://github.com/ssinha2103/github-issues_to_excel
 Author: Sudarshan Sinha
 Author-email: s.sinha2103@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,21 +21,26 @@
 - Filter issues by milestone number
 - Requires a GitHub access token for authentication
 
 ## Prerequisites
 - Python 3.x
 - `requests` library
 
-## Installation
+## Installation 
+ Follow either `Installation Type 1` or `Installation Type 2`
+
+### Installation Type 1
+1. `pip install github-issue-extractor`
+
+### Installation Type 2
 1. Clone the repository:
     `git clone https://github.com/ssinha2103/github-issues_to_excel`
 2. Install the required dependencies:
     `pip install -r requirements.txt`
 
-
 ## Usage
 To use the GitHub Issue Extractor, simply import the class and create an instance with the required parameters:
 
 ```python
 from github_issue_extractor import GitHubIssueExtractor
 
 milestone_number = 1
```

### Comparing `github_issue_extractor-0.1.2/setup.py` & `github_issue_extractor-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="github_issue_extractor",
-    version="0.1.2",
+    version="0.1.3",
     author="Sudarshan Sinha",
     author_email="s.sinha2103@outlook.com",
     description="GitHubIssueExtractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ssinha2103/github-issues_to_excel",
     packages=setuptools.find_packages(),
```

