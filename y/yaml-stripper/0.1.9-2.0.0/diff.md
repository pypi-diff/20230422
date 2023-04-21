# Comparing `tmp/yaml-stripper-0.1.9.tar.gz` & `tmp/yaml-stripper-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-stripper-0.1.9.tar", last modified: Fri Apr 21 19:48:10 2023, max compression
+gzip compressed data, was "yaml-stripper-2.0.0.tar", last modified: Fri Apr 21 22:25:50 2023, max compression
```

## Comparing `yaml-stripper-0.1.9.tar` & `yaml-stripper-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:48:10.743608 yaml-stripper-0.1.9/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:48:10.743422 yaml-stripper-0.1.9/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-0.1.9/README.md
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:48:10.742205 yaml-stripper-0.1.9/YamlStripper/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:26:23.000000 yaml-stripper-0.1.9/YamlStripper/__init__.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      847 2023-04-21 19:47:42.000000 yaml-stripper-0.1.9/YamlStripper/cli.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1161 2023-04-21 19:16:58.000000 yaml-stripper-0.1.9/YamlStripper/yaml_stripper.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 19:48:10.743652 yaml-stripper-0.1.9/setup.cfg
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1173 2023-04-21 19:47:59.000000 yaml-stripper-0.1.9/setup.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:48:10.742417 yaml-stripper-0.1.9/test/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1711 2023-04-21 19:47:42.000000 yaml-stripper-0.1.9/test/test_yaml_stripper.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:48:10.743245 yaml-stripper-0.1.9/yaml_stripper.egg-info/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3497 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      344 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/SOURCES.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/dependency_links.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       66 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/entry_points.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       27 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/requires.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       13 2023-04-21 19:48:10.000000 yaml-stripper-0.1.9/yaml_stripper.egg-info/top_level.txt
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 22:25:50.769141 yaml-stripper-2.0.0/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3493 2023-04-21 22:25:50.768994 yaml-stripper-2.0.0/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-2.0.0/README.md
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 22:25:50.767319 yaml-stripper-2.0.0/YamlStripper/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:26:23.000000 yaml-stripper-2.0.0/YamlStripper/__init__.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      467 2023-04-21 20:23:10.000000 yaml-stripper-2.0.0/YamlStripper/cli.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1605 2023-04-21 22:11:08.000000 yaml-stripper-2.0.0/YamlStripper/yaml_stripper.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 22:25:50.769195 yaml-stripper-2.0.0/setup.cfg
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1237 2023-04-21 22:23:26.000000 yaml-stripper-2.0.0/setup.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 22:25:50.767620 yaml-stripper-2.0.0/test/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:53:32.000000 yaml-stripper-2.0.0/test/__init__.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1103 2023-04-21 22:04:17.000000 yaml-stripper-2.0.0/test/test_yaml_stripper.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 22:25:50.768798 yaml-stripper-2.0.0/yaml_stripper.egg-info/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3493 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      361 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/SOURCES.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/dependency_links.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       56 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/entry_points.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       33 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/requires.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       18 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/top_level.txt
```

### Comparing `yaml-stripper-0.1.9/PKG-INFO` & `yaml-stripper-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.9
+Version: 2.0.0
 Summary: A command-line tool for removing specified fields from YAML files.
-Home-page: https://github.com/your_username/yaml-stripper
+Home-page: https://github.com/vavasilva/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
 Project-URL: Homepage, https://github.com/vavasilva/YamlStripper
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yaml-stripper-0.1.9/README.md` & `yaml-stripper-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `yaml-stripper-0.1.9/YamlStripper/yaml_stripper.py` & `yaml-stripper-2.0.0/YamlStripper/yaml_stripper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,43 @@
 import argparse
 import yaml
 
 
+def remove_field(data, field):
+    """
+    Recursively remove field from data
+    """
+    if field in data:
+        del data[field]
+    for k, v in data.items():
+        if isinstance(v, dict):
+            remove_field(v, field)
+        elif isinstance(v, list):
+            for item in v:
+                if isinstance(item, dict):
+                    remove_field(item, field)
+
+
 def remove_fields(yaml_file, fields_to_remove, new_yaml_file):
     """Remove specified fields from a YAML file.
 
     Args:
         yaml_file (str): The input YAML file.
         fields_to_remove (list): The fields to remove.
         new_yaml_file (str): The output YAML file without the specified fields.
 
     """
-
     with open(yaml_file, 'r') as f:
         data = yaml.load(f, Loader=yaml.FullLoader)
 
     for field in fields_to_remove:
-        if field in data:
-            del data[field]
+        remove_field(data, field)
+
+    # Remove empty dictionary items
+    data = {k:v for k, v in data.items() if v}
 
     with open(new_yaml_file, 'w') as f:
         yaml.dump(data, f)
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(
```

### Comparing `yaml-stripper-0.1.9/setup.py` & `yaml-stripper-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,38 @@
+import os
+
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+USERNAME = os.getenv('PYPI_USERNAME')
+PASSWORD = os.getenv('PYPI_PASSWORD')
+
 setuptools.setup(
     name="yaml-stripper",
-    version="0.1.9",
+    version="2.0.0",
     author="Wagner Silva",
     author_email="wra.silva@gmail.com",
     description="A command-line tool for removing specified fields from YAML files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/your_username/yaml-stripper",
+    url="https://github.com/vavasilva/yaml-stripper",
     packages=setuptools.find_packages(),
     project_urls={
         "Bug Tracker": "https://github.com/vavasilva/YamlStripper",
         "Documentation": "https://github.com/vavasilva/YamlStripper",
         "Source Code": "https://github.com/vavasilva/YamlStripper",
         "Homepage": "https://github.com/vavasilva/YamlStripper"
     },
     entry_points={
-        'console_scripts': ['yaml-stripper=YamlStripper.yaml_stripper:main'],
+        'console_scripts': ['yaml-stripper=YamlStripper.cli:main']
     },
-    install_requires=[
-        'PyYAML>=5.3.1',
-        'click>=8.0.0',
-    ],
+    install_requires=['PyYAML>=6.0', 'click>=8.1.3', 'keyring']
+    ,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
 )
```

### Comparing `yaml-stripper-0.1.9/yaml_stripper.egg-info/PKG-INFO` & `yaml-stripper-2.0.0/yaml_stripper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 0.1.9
+Version: 2.0.0
 Summary: A command-line tool for removing specified fields from YAML files.
-Home-page: https://github.com/your_username/yaml-stripper
+Home-page: https://github.com/vavasilva/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
 Project-URL: Homepage, https://github.com/vavasilva/YamlStripper
 Classifier: Programming Language :: Python :: 3
```

