# Comparing `tmp/autoMMM-0.1.4.tar.gz` & `tmp/autoMMM-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoMMM-0.1.4.tar", last modified: Wed Apr 19 20:58:27 2023, max compression
+gzip compressed data, was "autoMMM-0.1.5.tar", last modified: Sat Apr 22 13:34:30 2023, max compression
```

## Comparing `autoMMM-0.1.4.tar` & `autoMMM-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 20:58:27.659669 autoMMM-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-04-19 20:58:27.643959 autoMMM-0.1.4/AutoMMM/
--rw-rw-rw-   0        0        0        0 2023-04-08 15:41:28.000000 autoMMM-0.1.4/AutoMMM/__init__.py
--rw-rw-rw-   0        0        0     2849 2023-04-19 20:57:48.000000 autoMMM-0.1.4/AutoMMM/autoholidays.py
--rw-rw-rw-   0        0        0    11953 2023-04-18 11:17:07.000000 autoMMM-0.1.4/AutoMMM/automodeller.py
--rw-rw-rw-   0        0        0    10898 2023-04-19 20:58:27.659669 autoMMM-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    10132 2023-04-12 09:34:42.000000 autoMMM-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 20:58:27.659669 autoMMM-0.1.4/autoMMM.egg-info/
--rw-rw-rw-   0        0        0    10898 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 20:58:27.000000 autoMMM-0.1.4/autoMMM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 20:58:27.659669 autoMMM-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      995 2023-04-19 20:58:05.000000 autoMMM-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 13:34:30.323320 autoMMM-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-04-22 13:34:30.273780 autoMMM-0.1.5/AutoMMM/
+-rw-rw-rw-   0        0        0        0 2023-04-08 15:41:28.000000 autoMMM-0.1.5/AutoMMM/__init__.py
+-rw-rw-rw-   0        0        0     2849 2023-04-19 20:57:48.000000 autoMMM-0.1.5/AutoMMM/autoholidays.py
+-rw-rw-rw-   0        0        0    11953 2023-04-18 11:17:07.000000 autoMMM-0.1.5/AutoMMM/automodeller.py
+-rw-rw-rw-   0        0        0     9225 2023-04-22 13:33:13.000000 autoMMM-0.1.5/AutoMMM/bayes.py
+-rw-rw-rw-   0        0        0    10898 2023-04-22 13:34:30.323320 autoMMM-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10132 2023-04-12 09:34:42.000000 autoMMM-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 13:34:30.315165 autoMMM-0.1.5/autoMMM.egg-info/
+-rw-rw-rw-   0        0        0    10898 2023-04-22 13:34:30.000000 autoMMM-0.1.5/autoMMM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-04-22 13:34:30.000000 autoMMM-0.1.5/autoMMM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 13:34:30.000000 autoMMM-0.1.5/autoMMM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-04-22 13:34:30.000000 autoMMM-0.1.5/autoMMM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-22 13:34:30.000000 autoMMM-0.1.5/autoMMM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 13:34:30.323320 autoMMM-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1029 2023-04-22 13:30:55.000000 autoMMM-0.1.5/setup.py
```

### Comparing `autoMMM-0.1.4/AutoMMM/autoholidays.py` & `autoMMM-0.1.5/AutoMMM/autoholidays.py`

 * *Files identical despite different names*

### Comparing `autoMMM-0.1.4/AutoMMM/automodeller.py` & `autoMMM-0.1.5/AutoMMM/automodeller.py`

 * *Files identical despite different names*

### Comparing `autoMMM-0.1.4/PKG-INFO` & `autoMMM-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `autoMMM-0.1.4/README.md` & `autoMMM-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `autoMMM-0.1.4/autoMMM.egg-info/PKG-INFO` & `autoMMM-0.1.5/autoMMM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoMMM
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `autoMMM-0.1.4/setup.py` & `autoMMM-0.1.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="autoMMM",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "pandas",
         "scikit-learn",
         "statsmodels",
         "matplotlib",
         "openai",
         "holidays",
+        "seaborn",
+        "pymc"
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

