# Comparing `tmp/github_issue_extractor-0.1.0.tar.gz` & `tmp/github_issue_extractor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_issue_extractor-0.1.0.tar", last modified: Fri Apr 21 13:42:40 2023, max compression
+gzip compressed data, was "github_issue_extractor-0.1.1.tar", last modified: Sat Apr 22 20:47:42 2023, max compression
```

## Comparing `github_issue_extractor-0.1.0.tar` & `github_issue_extractor-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:42:40.937780 github_issue_extractor-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-21 13:42:40.937780 github_issue_extractor-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-21 13:42:29.000000 github_issue_extractor-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:42:40.937780 github_issue_extractor-0.1.0/github_issue_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-21 13:42:40.000000 github_issue_extractor-0.1.0/github_issue_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-21 13:42:40.000000 github_issue_extractor-0.1.0/github_issue_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:42:40.000000 github_issue_extractor-0.1.0/github_issue_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-21 13:42:40.000000 github_issue_extractor-0.1.0/github_issue_extractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:42:40.000000 github_issue_extractor-0.1.0/github_issue_extractor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 13:42:40.937780 github_issue_extractor-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-21 13:42:29.000000 github_issue_extractor-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:47:42.481761 github_issue_extractor-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-22 20:47:29.000000 github_issue_extractor-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-22 20:47:42.481761 github_issue_extractor-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-22 20:47:29.000000 github_issue_extractor-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:47:42.481761 github_issue_extractor-0.1.1/github_issue_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-22 20:47:42.000000 github_issue_extractor-0.1.1/github_issue_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-22 20:47:42.000000 github_issue_extractor-0.1.1/github_issue_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:47:42.000000 github_issue_extractor-0.1.1/github_issue_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 20:47:42.000000 github_issue_extractor-0.1.1/github_issue_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:47:42.000000 github_issue_extractor-0.1.1/github_issue_extractor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 20:47:42.481761 github_issue_extractor-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-22 20:47:29.000000 github_issue_extractor-0.1.1/setup.py
```

### Comparing `github_issue_extractor-0.1.0/setup.py` & `github_issue_extractor-0.1.1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import setuptools
 
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+
 setuptools.setup(
     name="github_issue_extractor",
-    version="0.1.0",
+    version="0.1.1",
     author="Sudarshan Sinha",
     author_email="s.sinha2103@outlook.com",
     description="GitHubIssueExtractor",
-    long_description="GitHubIssueExtractor",
+    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ssinha2103/github-issues_to_excel",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

