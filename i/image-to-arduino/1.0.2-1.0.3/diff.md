# Comparing `tmp/image_to_arduino-1.0.2.tar.gz` & `tmp/image_to_arduino-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_to_arduino-1.0.2.tar", last modified: Sat Apr 22 13:11:07 2023, max compression
+gzip compressed data, was "image_to_arduino-1.0.3.tar", last modified: Sat Apr 22 13:24:03 2023, max compression
```

## Comparing `image_to_arduino-1.0.2.tar` & `image_to_arduino-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image_to_arduino-1.0.2/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1967 2023-04-21 14:35:32.000000 image_to_arduino-1.0.2/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       86 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      696 2023-04-22 13:10:31.000000 image_to_arduino-1.0.2/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image_to_arduino-1.0.2/src/__init__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     6690 2023-04-22 13:00:58.000000 image_to_arduino-1.0.2/src/image_to_arduino.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1967 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-04-22 13:24:03.000000 image_to_arduino-1.0.3/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      696 2023-04-22 13:23:36.000000 image_to_arduino-1.0.3/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:24:03.421831 image_to_arduino-1.0.3/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image_to_arduino-1.0.3/src/__init__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     6690 2023-04-22 13:00:58.000000 image_to_arduino-1.0.3/src/image_to_arduino.py
```

### Comparing `image_to_arduino-1.0.2/LICENSE` & `image_to_arduino-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `image_to_arduino-1.0.2/README.md` & `image_to_arduino-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `image_to_arduino-1.0.2/setup.py` & `image_to_arduino-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 REQUIREMENTS = [i.strip() for i in open("/home/wiktor/Image_Converter_App/requirements.txt").readlines()]
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 setup(
    name='image_to_arduino',
-   version='1.0.2',
+   version='1.0.3',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
```

### Comparing `image_to_arduino-1.0.2/src/image_to_arduino.py` & `image_to_arduino-1.0.3/src/image_to_arduino.py`

 * *Files identical despite different names*

