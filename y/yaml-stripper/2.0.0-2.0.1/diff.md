# Comparing `tmp/yaml-stripper-2.0.0.tar.gz` & `tmp/yaml-stripper-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-stripper-2.0.0.tar", last modified: Fri Apr 21 22:25:50 2023, max compression
+gzip compressed data, was "yaml-stripper-2.0.1.tar", last modified: Sat Apr 22 00:42:24 2023, max compression
```

## Comparing `yaml-stripper-2.0.0.tar` & `yaml-stripper-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 22:25:50.769141 yaml-stripper-2.0.0/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3493 2023-04-21 22:25:50.768994 yaml-stripper-2.0.0/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-2.0.0/README.md
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 22:25:50.767319 yaml-stripper-2.0.0/YamlStripper/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:26:23.000000 yaml-stripper-2.0.0/YamlStripper/__init__.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      467 2023-04-21 20:23:10.000000 yaml-stripper-2.0.0/YamlStripper/cli.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1605 2023-04-21 22:11:08.000000 yaml-stripper-2.0.0/YamlStripper/yaml_stripper.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-21 22:25:50.769195 yaml-stripper-2.0.0/setup.cfg
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1237 2023-04-21 22:23:26.000000 yaml-stripper-2.0.0/setup.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 22:25:50.767620 yaml-stripper-2.0.0/test/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:53:32.000000 yaml-stripper-2.0.0/test/__init__.py
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1103 2023-04-21 22:04:17.000000 yaml-stripper-2.0.0/test/test_yaml_stripper.py
-drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 22:25:50.768798 yaml-stripper-2.0.0/yaml_stripper.egg-info/
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3493 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/PKG-INFO
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      361 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/SOURCES.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/dependency_links.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       56 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/entry_points.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       33 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/requires.txt
--rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       18 2023-04-21 22:25:50.000000 yaml-stripper-2.0.0/yaml_stripper.egg-info/top_level.txt
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-22 00:42:24.980585 yaml-stripper-2.0.1/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3493 2023-04-22 00:42:24.980332 yaml-stripper-2.0.1/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     2769 2023-04-21 18:52:32.000000 yaml-stripper-2.0.1/README.md
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-22 00:42:24.978129 yaml-stripper-2.0.1/YamlStripper/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:26:23.000000 yaml-stripper-2.0.1/YamlStripper/__init__.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      467 2023-04-21 20:23:10.000000 yaml-stripper-2.0.1/YamlStripper/cli.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1605 2023-04-22 00:35:40.000000 yaml-stripper-2.0.1/YamlStripper/yaml_stripper.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       38 2023-04-22 00:42:24.980666 yaml-stripper-2.0.1/setup.cfg
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     1237 2023-04-22 00:41:10.000000 yaml-stripper-2.0.1/setup.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-22 00:42:24.978680 yaml-stripper-2.0.1/test/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-21 19:53:32.000000 yaml-stripper-2.0.1/test/__init__.py
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      635 2023-04-22 00:36:22.000000 yaml-stripper-2.0.1/test/test_yaml_stripper.py
+drwxr-xr-x   0 wagnerrodrigues   (501) staff       (20)        0 2023-04-22 00:42:24.979977 yaml-stripper-2.0.1/yaml_stripper.egg-info/
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)     3493 2023-04-22 00:42:24.000000 yaml-stripper-2.0.1/yaml_stripper.egg-info/PKG-INFO
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)      361 2023-04-22 00:42:24.000000 yaml-stripper-2.0.1/yaml_stripper.egg-info/SOURCES.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)        1 2023-04-22 00:42:24.000000 yaml-stripper-2.0.1/yaml_stripper.egg-info/dependency_links.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       56 2023-04-22 00:42:24.000000 yaml-stripper-2.0.1/yaml_stripper.egg-info/entry_points.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       33 2023-04-22 00:42:24.000000 yaml-stripper-2.0.1/yaml_stripper.egg-info/requires.txt
+-rw-r--r--   0 wagnerrodrigues   (501) staff       (20)       18 2023-04-22 00:42:24.000000 yaml-stripper-2.0.1/yaml_stripper.egg-info/top_level.txt
```

### Comparing `yaml-stripper-2.0.0/PKG-INFO` & `yaml-stripper-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 2.0.0
+Version: 2.0.1
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/vavasilva/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
```

### Comparing `yaml-stripper-2.0.0/README.md` & `yaml-stripper-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `yaml-stripper-2.0.0/YamlStripper/yaml_stripper.py` & `yaml-stripper-2.0.1/YamlStripper/yaml_stripper.py`

 * *Files identical despite different names*

### Comparing `yaml-stripper-2.0.0/setup.py` & `yaml-stripper-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 USERNAME = os.getenv('PYPI_USERNAME')
 PASSWORD = os.getenv('PYPI_PASSWORD')
 
 setuptools.setup(
     name="yaml-stripper",
-    version="2.0.0",
+    version="2.0.1",
     author="Wagner Silva",
     author_email="wra.silva@gmail.com",
     description="A command-line tool for removing specified fields from YAML files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/vavasilva/yaml-stripper",
     packages=setuptools.find_packages(),
```

### Comparing `yaml-stripper-2.0.0/yaml_stripper.egg-info/PKG-INFO` & `yaml-stripper-2.0.1/yaml_stripper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-stripper
-Version: 2.0.0
+Version: 2.0.1
 Summary: A command-line tool for removing specified fields from YAML files.
 Home-page: https://github.com/vavasilva/yaml-stripper
 Author: Wagner Silva
 Author-email: wra.silva@gmail.com
 Project-URL: Bug Tracker, https://github.com/vavasilva/YamlStripper
 Project-URL: Documentation, https://github.com/vavasilva/YamlStripper
 Project-URL: Source Code, https://github.com/vavasilva/YamlStripper
```

