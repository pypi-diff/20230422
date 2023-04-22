# Comparing `tmp/PyTurboJPEG-1.7.0.tar.gz` & `tmp/PyTurboJPEG-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTurboJPEG-1.7.0.tar", last modified: Mon Nov  7 14:08:28 2022, max compression
+gzip compressed data, was "PyTurboJPEG-1.7.1.tar", last modified: Sat Apr 22 16:50:30 2023, max compression
```

## Comparing `PyTurboJPEG-1.7.0.tar` & `PyTurboJPEG-1.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lilohuang   (501) staff       (20)        0 2022-11-07 14:08:28.240391 PyTurboJPEG-1.7.0/
--rw-r--r--   0 lilohuang   (501) staff       (20)     1092 2022-11-07 14:08:14.000000 PyTurboJPEG-1.7.0/LICENSE
--rw-r--r--   0 lilohuang   (501) staff       (20)     6558 2022-11-07 14:08:28.240223 PyTurboJPEG-1.7.0/PKG-INFO
-drwxr-xr-x   0 lilohuang   (501) staff       (20)        0 2022-11-07 14:08:28.240015 PyTurboJPEG-1.7.0/PyTurboJPEG.egg-info/
--rw-r--r--   0 lilohuang   (501) staff       (20)     6558 2022-11-07 14:08:27.000000 PyTurboJPEG-1.7.0/PyTurboJPEG.egg-info/PKG-INFO
--rw-r--r--   0 lilohuang   (501) staff       (20)      213 2022-11-07 14:08:27.000000 PyTurboJPEG-1.7.0/PyTurboJPEG.egg-info/SOURCES.txt
--rw-r--r--   0 lilohuang   (501) staff       (20)        1 2022-11-07 14:08:27.000000 PyTurboJPEG-1.7.0/PyTurboJPEG.egg-info/dependency_links.txt
--rw-r--r--   0 lilohuang   (501) staff       (20)        6 2022-11-07 14:08:27.000000 PyTurboJPEG-1.7.0/PyTurboJPEG.egg-info/requires.txt
--rw-r--r--   0 lilohuang   (501) staff       (20)       10 2022-11-07 14:08:27.000000 PyTurboJPEG-1.7.0/PyTurboJPEG.egg-info/top_level.txt
--rw-r--r--   0 lilohuang   (501) staff       (20)     6223 2022-11-07 14:08:14.000000 PyTurboJPEG-1.7.0/README.md
--rw-r--r--   0 lilohuang   (501) staff       (20)       38 2022-11-07 14:08:28.240437 PyTurboJPEG-1.7.0/setup.cfg
--rw-r--r--   0 lilohuang   (501) staff       (20)      543 2022-11-07 14:08:14.000000 PyTurboJPEG-1.7.0/setup.py
--rw-r--r--   0 lilohuang   (501) staff       (20)    37030 2022-11-07 14:08:14.000000 PyTurboJPEG-1.7.0/turbojpeg.py
+drwxr-xr-x   0 lilohuang   (501) staff       (20)        0 2023-04-22 16:50:30.427491 PyTurboJPEG-1.7.1/
+-rw-r--r--   0 lilohuang   (501) staff       (20)     1092 2023-04-22 16:50:18.000000 PyTurboJPEG-1.7.1/LICENSE
+-rw-r--r--   0 lilohuang   (501) staff       (20)     6558 2023-04-22 16:50:30.427231 PyTurboJPEG-1.7.1/PKG-INFO
+drwxr-xr-x   0 lilohuang   (501) staff       (20)        0 2023-04-22 16:50:30.426974 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/
+-rw-r--r--   0 lilohuang   (501) staff       (20)     6558 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/PKG-INFO
+-rw-r--r--   0 lilohuang   (501) staff       (20)      213 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/SOURCES.txt
+-rw-r--r--   0 lilohuang   (501) staff       (20)        1 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/dependency_links.txt
+-rw-r--r--   0 lilohuang   (501) staff       (20)        6 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/requires.txt
+-rw-r--r--   0 lilohuang   (501) staff       (20)       10 2023-04-22 16:50:29.000000 PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/top_level.txt
+-rw-r--r--   0 lilohuang   (501) staff       (20)     6223 2023-04-22 16:50:18.000000 PyTurboJPEG-1.7.1/README.md
+-rw-r--r--   0 lilohuang   (501) staff       (20)       38 2023-04-22 16:50:30.427539 PyTurboJPEG-1.7.1/setup.cfg
+-rw-r--r--   0 lilohuang   (501) staff       (20)      543 2023-04-22 16:50:18.000000 PyTurboJPEG-1.7.1/setup.py
+-rw-r--r--   0 lilohuang   (501) staff       (20)    37195 2023-04-22 16:50:18.000000 PyTurboJPEG-1.7.1/turbojpeg.py
```

### Comparing `PyTurboJPEG-1.7.0/LICENSE` & `PyTurboJPEG-1.7.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2022 Lilo Huang <kuso.cc@gmail.com>
+Copyright (c) 2018-2023 Lilo Huang <kuso.cc@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `PyTurboJPEG-1.7.0/PKG-INFO` & `PyTurboJPEG-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTurboJPEG
-Version: 1.7.0
+Version: 1.7.1
 Summary: A Python wrapper of libjpeg-turbo for decoding and encoding JPEG image.
 Home-page: https://github.com/lilohuang/PyTurboJPEG
 Author: Lilo Huang
 Author-email: kuso.cc@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyTurboJPEG-1.7.0/PyTurboJPEG.egg-info/PKG-INFO` & `PyTurboJPEG-1.7.1/PyTurboJPEG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTurboJPEG
-Version: 1.7.0
+Version: 1.7.1
 Summary: A Python wrapper of libjpeg-turbo for decoding and encoding JPEG image.
 Home-page: https://github.com/lilohuang/PyTurboJPEG
 Author: Lilo Huang
 Author-email: kuso.cc@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyTurboJPEG-1.7.0/README.md` & `PyTurboJPEG-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `PyTurboJPEG-1.7.0/setup.py` & `PyTurboJPEG-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
 from setuptools import setup, find_packages
 setup(
     name='PyTurboJPEG',
-    version='1.7.0',
+    version='1.7.1',
     description='A Python wrapper of libjpeg-turbo for decoding and encoding JPEG image.',
     author='Lilo Huang',
     author_email='kuso.cc@gmail.com',
     url='https://github.com/lilohuang/PyTurboJPEG',
     license='MIT',
     install_requires=['numpy'],
     py_modules=['turbojpeg'],
```

### Comparing `PyTurboJPEG-1.7.0/turbojpeg.py` & `PyTurboJPEG-1.7.1/turbojpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: UTF-8 -*-
 #
 # PyTurboJPEG - A Python wrapper of libjpeg-turbo for decoding and encoding JPEG image.
 #
-# Copyright (c) 2018-2022, Lilo Huang. All rights reserved.
+# Copyright (c) 2018-2023, Lilo Huang. All rights reserved.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,15 +19,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 __author__ = 'Lilo Huang <kuso.cc@gmail.com>'
-__version__ = '1.7.0'
+__version__ = '1.7.1'
 
 from ctypes import *
 from ctypes.util import find_library
 import platform
 import numpy as np
 import math
 import warnings
@@ -583,15 +583,15 @@
             self.__free(dest_array)
             if status != 0:
                 self.__report_error(handle)
             return dest_buf.raw
         finally:
             self.__destroy(handle)
 
-    def crop_multiple(self, jpeg_buf, crop_parameters, background_luminance=1.0, gray=False):
+    def crop_multiple(self, jpeg_buf, crop_parameters, background_luminance=1.0, gray=False, copynone=False):
         """Lossless crop and/or extension operations on jpeg image.
         Crop origin(s) needs be divisable by the MCU block size and inside
         the input image, or OSError: Invalid crop request is raised.
 
         Parameters
         ----------
         jpeg_buf: bytes
@@ -600,14 +600,16 @@
             List of crop parameters defining start x and y origin and width
             and height of each crop operation.
         background_luminance: float
             Luminance level (0 -1 ) to fill background when extending image.
             Default to 1, resulting in white background.
         gray: bool
             Produce greyscale output
+        copynone: bool
+            True = do not copy EXIF data (False by default)
 
         Returns
         ----------
         List[bytes]
             Cropped and/or extended jpeg images.
         """
         handle = self.__init_transform()
@@ -655,23 +657,23 @@
                             background_luminance
                         )
                     )
                     callback = CUSTOMFILTER(fill_background)
                     crop_transforms[i] = TransformStruct(
                         crop_region,
                         TJXOP_NONE,
-                        TJXOPT_PERFECT | TJXOPT_CROP | (gray and TJXOPT_GRAY),
+                        TJXOPT_PERFECT | TJXOPT_CROP | (gray and TJXOPT_GRAY) | (copynone and TJXOPT_COPYNONE),
                         pointer(callback_data),
                         callback
                     )
                 else:
                     crop_transforms[i] = TransformStruct(
                         crop_region,
                         TJXOP_NONE,
-                        TJXOPT_PERFECT | TJXOPT_CROP | (gray and TJXOPT_GRAY)
+                        TJXOPT_PERFECT | TJXOPT_CROP | (gray and TJXOPT_GRAY) | (copynone and TJXOPT_COPYNONE)
                     )
 
             # Pointers to output image buffers and buffer size
             dest_array = (c_void_p * number_of_operations)()
             dest_size = (c_ulong * number_of_operations)()
 
             # Do the transforms
```

