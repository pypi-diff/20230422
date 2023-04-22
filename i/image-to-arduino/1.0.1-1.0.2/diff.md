# Comparing `tmp/image_to_arduino-1.0.1.tar.gz` & `tmp/image_to_arduino-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_to_arduino-1.0.1.tar", last modified: Fri Apr 21 18:16:25 2023, max compression
+gzip compressed data, was "image_to_arduino-1.0.2.tar", last modified: Sat Apr 22 13:11:07 2023, max compression
```

## Comparing `image_to_arduino-1.0.1.tar` & `image_to_arduino-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image_to_arduino-1.0.1/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      381 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1967 2023-04-21 14:35:32.000000 image_to_arduino-1.0.1/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      381 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-04-21 18:16:24.000000 image_to_arduino-1.0.1/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      696 2023-04-21 18:13:48.000000 image_to_arduino-1.0.1/setup.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 18:16:25.007041 image_to_arduino-1.0.1/src/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image_to_arduino-1.0.1/src/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     6664 2023-04-21 14:35:32.000000 image_to_arduino-1.0.1/src/image_to_arduino.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-04-21 14:35:32.000000 image_to_arduino-1.0.2/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1967 2023-04-21 14:35:32.000000 image_to_arduino-1.0.2/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      362 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      265 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       86 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        4 2023-04-22 13:11:07.000000 image_to_arduino-1.0.2/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      696 2023-04-22 13:10:31.000000 image_to_arduino-1.0.2/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-04-22 13:11:07.214821 image_to_arduino-1.0.2/src/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-04-21 14:35:32.000000 image_to_arduino-1.0.2/src/__init__.py
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)     6690 2023-04-22 13:00:58.000000 image_to_arduino-1.0.2/src/image_to_arduino.py
```

### Comparing `image_to_arduino-1.0.1/LICENSE` & `image_to_arduino-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `image_to_arduino-1.0.1/README.md` & `image_to_arduino-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `image_to_arduino-1.0.1/setup.py` & `image_to_arduino-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 REQUIREMENTS = [i.strip() for i in open("/home/wiktor/Image_Converter_App/requirements.txt").readlines()]
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 setup(
    name='image_to_arduino',
-   version='1.0.1',
+   version='1.0.2',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
```

### Comparing `image_to_arduino-1.0.1/src/image_to_arduino.py` & `image_to_arduino-1.0.2/src/image_to_arduino.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/usr/bin/env python3
 import tkinter as tk
 import customtkinter 
 from tkinter import filedialog
 import cv2
 import numpy as np
 from PIL import Image, ImageTk, ImageOps
 import os
@@ -162,8 +163,8 @@
 # "Clear all" button 
 clear_all_button = customtkinter.CTkButton(root, text="Clear All", command=clear_all)
 clear_all_button.grid(row=4, column=0, pady=5, padx=10, columnspan=1, sticky="nsew")  
 
 # Configure the window to not be resizable
 root.resizable(False, False)
 
-root.mainloop()
+root.mainloop()
```

