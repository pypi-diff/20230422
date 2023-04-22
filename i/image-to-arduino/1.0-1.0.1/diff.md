# Comparing `tmp/image_to_arduino-1.0.tar.gz` & `tmp/image_to_arduino-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_to_arduino-1.0.tar", last modified: Fri Apr 21 16:45:07 2023, max compression
+gzip compressed data, was "image_to_arduino-1.0.1.tar", last modified: Fri Apr 21 18:16:25 2023, max compression
```

## Comparing `image_to_arduino-1.0.tar` & `image_to_arduino-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 16:45:07.168769 image_to_arduino-1.0/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image_to_arduino-1.0/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      360 2023-04-21 16:45:07.168769 image_to_arduino-1.0/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1967 2023-04-21 14:35:32.000000 image_to_arduino-1.0/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 16:45:07.168769 image_to_arduino-1.0/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      360 2023-04-21 16:45:07.000000 image_to_arduino-1.0/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      225 2023-04-21 16:45:07.000000 image_to_arduino-1.0/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-21 16:45:07.000000 image_to_arduino-1.0/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-04-21 16:45:07.000000 image_to_arduino-1.0/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-21 16:45:07.000000 image_to_arduino-1.0/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-21 16:45:07.168769 image_to_arduino-1.0/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      695 2023-04-21 16:40:16.000000 image_to_arduino-1.0/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image_to_arduino-1.0.1/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      381 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1967 2023-04-21 14:35:32.000000 image_to_arduino-1.0.1/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      381 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      696 2023-04-21 18:13:48.000000 image_to_arduino-1.0.1/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image_to_arduino-1.0.1/src/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     6664 2023-04-21 14:35:32.000000 image_to_arduino-1.0.1/src/image_to_arduino.py
```

### Comparing `image_to_arduino-1.0/LICENSE` & `image_to_arduino-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image_to_arduino-1.0/README.md` & `image_to_arduino-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `image_to_arduino-1.0/setup.py` & `image_to_arduino-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import setup, find_packages
 
 REQUIREMENTS = [i.strip() for i in open("/home/wiktor/Image_Converter_App/requirements.txt").readlines()]
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 setup(
    name='image_to_arduino',
-   version='1.0',
+   version='1.0.1',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
-   packages=find_packages('src', exclude=['image_to_arduino']),
+   packages=['src'],
+   package_data={'src': ['data/*.dat']},
    install_requires=REQUIREMENTS, 
 
 )
```

