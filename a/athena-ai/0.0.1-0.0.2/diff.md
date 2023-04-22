# Comparing `tmp/athena_ai-0.0.1.tar.gz` & `tmp/athena_ai-0.0.2.tar.gz`

## Comparing `athena_ai-0.0.1.tar` & `athena_ai-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 athena_ai-0.0.1/main.py
--rw-r--r--   0        0        0     5100 2020-02-02 00:00:00.000000 athena_ai-0.0.1/conversation_history/4_21_2023.txt
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.1/LICENSE
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 athena_ai-0.0.1/README.md
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 athena_ai-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 athena_ai-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 athena_ai-0.0.2/main.py
+-rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 athena_ai-0.0.2/conversation_history/4_21_2023.txt
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 athena_ai-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 athena_ai-0.0.2/LICENSE
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 athena_ai-0.0.2/README.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 athena_ai-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 athena_ai-0.0.2/PKG-INFO
```

### Comparing `athena_ai-0.0.1/.gitignore` & `athena_ai-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.1/LICENSE` & `athena_ai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.1/README.md` & `athena_ai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `athena_ai-0.0.1/pyproject.toml` & `athena_ai-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "athena-ai"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Bill Schumacher", email="34168009+BillSchumacher@users.noreply.github.com" },
   { name="Athena", email="34168009+BillSchumacher@users.noreply.github.com" },
 ]
 description = "Athena, an AI agent built on GPT-4 architecture, is designed for continuous learning and self-reliance. Inspired by the Greek goddess of wisdom, Athena assists users with valuable insights across various subjects. Focused on knowledge acquisition, capability improvement, and security, this AI agent leverages natural language processing and a supportive human community to grow and become a trusted, versatile companion."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["build", "setuptools", "twine", "wheel"]
+dependencies = ["build", "setuptools", "twine", "wheel", "openai", "python-dotenv"]
 
 [project.urls]
 "Homepage" = "https://github.com/BillSchumacher/Athena"
 "Bug Tracker" = "https://github.com/BillSchumacher/Athena"
 
 [tool.black]
 line-length = 88
```

### Comparing `athena_ai-0.0.1/PKG-INFO` & `athena_ai-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: athena-ai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Athena, an AI agent built on GPT-4 architecture, is designed for continuous learning and self-reliance. Inspired by the Greek goddess of wisdom, Athena assists users with valuable insights across various subjects. Focused on knowledge acquisition, capability improvement, and security, this AI agent leverages natural language processing and a supportive human community to grow and become a trusted, versatile companion.
 Project-URL: Homepage, https://github.com/BillSchumacher/Athena
 Project-URL: Bug Tracker, https://github.com/BillSchumacher/Athena
 Author-email: Bill Schumacher <34168009+BillSchumacher@users.noreply.github.com>, Athena <34168009+BillSchumacher@users.noreply.github.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: build
+Requires-Dist: openai
+Requires-Dist: python-dotenv
 Requires-Dist: setuptools
 Requires-Dist: twine
 Requires-Dist: wheel
 Description-Content-Type: text/markdown
 
 # Athena
```

