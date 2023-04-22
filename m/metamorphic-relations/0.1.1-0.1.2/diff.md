# Comparing `tmp/metamorphic_relations-0.1.1.tar.gz` & `tmp/metamorphic_relations-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamorphic_relations-0.1.1.tar", last modified: Sat Apr 22 16:57:30 2023, max compression
+gzip compressed data, was "metamorphic_relations-0.1.2.tar", last modified: Sat Apr 22 17:40:09 2023, max compression
```

## Comparing `metamorphic_relations-0.1.1.tar` & `metamorphic_relations-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 16:57:29.993238 metamorphic_relations-0.1.1/
--rw-rw-rw-   0        0        0      653 2023-04-22 16:57:29.993238 metamorphic_relations-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       74 2023-03-20 09:32:57.000000 metamorphic_relations-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 16:57:29.957229 metamorphic_relations-0.1.1/metamorphic_relations/
--rw-rw-rw-   0        0        0     4355 2023-04-07 15:30:39.000000 metamorphic_relations-0.1.1/metamorphic_relations/Data.py
--rw-rw-rw-   0        0        0     2311 2023-03-22 17:39:31.000000 metamorphic_relations-0.1.1/metamorphic_relations/ImageMR.py
--rw-rw-rw-   0        0        0     2942 2023-04-07 10:16:07.000000 metamorphic_relations-0.1.1/metamorphic_relations/Info.py
--rw-rw-rw-   0        0        0    10833 2023-04-17 10:15:08.000000 metamorphic_relations-0.1.1/metamorphic_relations/MR.py
--rw-rw-rw-   0        0        0    16722 2023-04-17 10:15:31.000000 metamorphic_relations-0.1.1/metamorphic_relations/MRModel.py
--rw-rw-rw-   0        0        0     8441 2023-04-17 11:05:00.000000 metamorphic_relations-0.1.1/metamorphic_relations/Results.py
--rw-rw-rw-   0        0        0      675 2023-04-03 15:33:06.000000 metamorphic_relations-0.1.1/metamorphic_relations/Transform.py
--rw-rw-rw-   0        0        0       41 2023-03-20 16:38:17.000000 metamorphic_relations-0.1.1/metamorphic_relations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 16:57:29.993238 metamorphic_relations-0.1.1/metamorphic_relations.egg-info/
--rw-rw-rw-   0        0        0      653 2023-04-22 16:57:29.000000 metamorphic_relations-0.1.1/metamorphic_relations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      498 2023-04-22 16:57:29.000000 metamorphic_relations-0.1.1/metamorphic_relations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 16:57:29.000000 metamorphic_relations-0.1.1/metamorphic_relations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-22 16:57:29.000000 metamorphic_relations-0.1.1/metamorphic_relations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-22 16:57:29.000000 metamorphic_relations-0.1.1/metamorphic_relations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 16:57:30.000231 metamorphic_relations-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1442 2023-04-22 16:55:57.000000 metamorphic_relations-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:40:09.046939 metamorphic_relations-0.1.2/
+-rw-rw-rw-   0        0        0     4916 2023-04-22 17:40:09.046939 metamorphic_relations-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4236 2023-04-22 17:39:11.000000 metamorphic_relations-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-22 17:40:09.021837 metamorphic_relations-0.1.2/metamorphic_relations/
+-rw-rw-rw-   0        0        0     4355 2023-04-07 15:30:39.000000 metamorphic_relations-0.1.2/metamorphic_relations/Data.py
+-rw-rw-rw-   0        0        0     2311 2023-03-22 17:39:31.000000 metamorphic_relations-0.1.2/metamorphic_relations/ImageMR.py
+-rw-rw-rw-   0        0        0     2942 2023-04-07 10:16:07.000000 metamorphic_relations-0.1.2/metamorphic_relations/Info.py
+-rw-rw-rw-   0        0        0    10833 2023-04-17 10:15:08.000000 metamorphic_relations-0.1.2/metamorphic_relations/MR.py
+-rw-rw-rw-   0        0        0    16722 2023-04-17 10:15:31.000000 metamorphic_relations-0.1.2/metamorphic_relations/MRModel.py
+-rw-rw-rw-   0        0        0     8441 2023-04-17 11:05:00.000000 metamorphic_relations-0.1.2/metamorphic_relations/Results.py
+-rw-rw-rw-   0        0        0      675 2023-04-03 15:33:06.000000 metamorphic_relations-0.1.2/metamorphic_relations/Transform.py
+-rw-rw-rw-   0        0        0       41 2023-03-20 16:38:17.000000 metamorphic_relations-0.1.2/metamorphic_relations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-22 17:40:09.041837 metamorphic_relations-0.1.2/metamorphic_relations.egg-info/
+-rw-rw-rw-   0        0        0     4916 2023-04-22 17:40:08.000000 metamorphic_relations-0.1.2/metamorphic_relations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2023-04-22 17:40:08.000000 metamorphic_relations-0.1.2/metamorphic_relations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-22 17:40:08.000000 metamorphic_relations-0.1.2/metamorphic_relations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-22 17:40:08.000000 metamorphic_relations-0.1.2/metamorphic_relations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-22 17:40:08.000000 metamorphic_relations-0.1.2/metamorphic_relations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-22 17:40:09.046939 metamorphic_relations-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1442 2023-04-22 17:39:50.000000 metamorphic_relations-0.1.2/setup.py
```

### Comparing `metamorphic_relations-0.1.1/metamorphic_relations/Data.py` & `metamorphic_relations-0.1.2/metamorphic_relations/Data.py`

 * *Files identical despite different names*

### Comparing `metamorphic_relations-0.1.1/metamorphic_relations/ImageMR.py` & `metamorphic_relations-0.1.2/metamorphic_relations/ImageMR.py`

 * *Files identical despite different names*

### Comparing `metamorphic_relations-0.1.1/metamorphic_relations/Info.py` & `metamorphic_relations-0.1.2/metamorphic_relations/Info.py`

 * *Files identical despite different names*

### Comparing `metamorphic_relations-0.1.1/metamorphic_relations/MR.py` & `metamorphic_relations-0.1.2/metamorphic_relations/MR.py`

 * *Files identical despite different names*

### Comparing `metamorphic_relations-0.1.1/metamorphic_relations/MRModel.py` & `metamorphic_relations-0.1.2/metamorphic_relations/MRModel.py`

 * *Files identical despite different names*

### Comparing `metamorphic_relations-0.1.1/metamorphic_relations/Results.py` & `metamorphic_relations-0.1.2/metamorphic_relations/Results.py`

 * *Files identical despite different names*

### Comparing `metamorphic_relations-0.1.1/metamorphic_relations/Transform.py` & `metamorphic_relations-0.1.2/metamorphic_relations/Transform.py`

 * *Files identical despite different names*

### Comparing `metamorphic_relations-0.1.1/setup.py` & `metamorphic_relations-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name='metamorphic_relations',
-    version="0.1.1",
+    version="0.1.2",
     description="Metamorphic relations library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://3200-metamorphic-relations-lib.readthedocs.io",
     author="Daniel Costantini",
     classifiers=[
         "Intended Audience :: Developers",
```

