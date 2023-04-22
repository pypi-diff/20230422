# Comparing `tmp/ddtcv-0.1.1.tar.gz` & `tmp/ddtcv-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddtcv-0.1.1.tar", max compression
+gzip compressed data, was "ddtcv-0.1.2.tar", max compression
```

## Comparing `ddtcv-0.1.1.tar` & `ddtcv-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      116 2023-02-07 03:11:06.202053 ddtcv-0.1.1/ddtcv/__init__.py
--rw-r--r--   0        0        0      159 2023-02-04 06:36:15.784718 ddtcv-0.1.1/ddtcv/abstract.py
--rw-r--r--   0        0        0      829 2023-02-04 07:07:57.912377 ddtcv-0.1.1/ddtcv/angle.py
--rw-r--r--   0        0        0     1205 2023-02-04 06:26:36.847666 ddtcv-0.1.1/ddtcv/onnx.py
--rw-r--r--   0        0        0  1873116 2022-11-18 10:08:59.992000 ddtcv-0.1.1/ddtcv/static/model/angle_1_rec_en_number_lite/angle_1_rec_en_number_lite.onnx
--rw-r--r--   0        0        0       31 2022-11-18 10:08:59.992000 ddtcv-0.1.1/ddtcv/static/model/angle_1_rec_en_number_lite/angle_dict.txt
--rw-r--r--   0        0        0  1873116 2022-11-18 10:09:00.005000 ddtcv-0.1.1/ddtcv/static/model/wind_1_rec_en_number_lite/wind_1_rec_en_number_lite.onnx
--rw-r--r--   0        0        0       31 2022-11-18 10:09:00.005000 ddtcv-0.1.1/ddtcv/static/model/wind_1_rec_en_number_lite/wind_dict.txt
--rw-r--r--   0        0        0        0 2023-02-04 06:54:16.389323 ddtcv-0.1.1/ddtcv/tests/__init__.py
--rw-r--r--   0        0        0      653 2023-02-04 07:08:24.143450 ddtcv-0.1.1/ddtcv/tests/__pycache__/test_angle.cpython-37.pyc
--rw-r--r--   0        0        0      863 2023-02-04 06:32:06.991371 ddtcv-0.1.1/ddtcv/tests/__pycache__/test_onnx.cpython-37.pyc
--rw-r--r--   0        0        0      652 2023-02-04 07:05:27.907078 ddtcv-0.1.1/ddtcv/tests/__pycache__/test_wind.cpython-37.pyc
--rw-r--r--   0        0        0     2227 2023-02-04 06:25:01.374255 ddtcv-0.1.1/ddtcv/tests/image/img.png
--rw-r--r--   0        0        0   824656 2022-11-26 04:20:44.960000 ddtcv-0.1.1/ddtcv/tests/image/img2.png
--rw-r--r--   0        0        0      277 2023-02-07 03:13:32.423804 ddtcv-0.1.1/ddtcv/tests/test_angle.py
--rw-r--r--   0        0        0      511 2023-02-07 03:13:32.466139 ddtcv-0.1.1/ddtcv/tests/test_onnx.py
--rw-r--r--   0        0        0      273 2023-02-07 03:13:32.442511 ddtcv-0.1.1/ddtcv/tests/test_wind.py
--rw-r--r--   0        0        0      339 2023-02-04 06:30:40.393471 ddtcv-0.1.1/ddtcv/tools/__pycache__/load_model.cpython-37.pyc
--rw-r--r--   0        0        0     3741 2023-02-04 06:30:40.483492 ddtcv-0.1.1/ddtcv/tools/__pycache__/postprocess.cpython-37.pyc
--rw-r--r--   0        0        0     1400 2023-02-04 06:30:40.458484 ddtcv-0.1.1/ddtcv/tools/__pycache__/preprocess.cpython-37.pyc
--rw-r--r--   0        0        0      165 2022-11-18 10:08:59.971000 ddtcv-0.1.1/ddtcv/tools/load_model.py
--rw-r--r--   0        0        0     4291 2022-11-18 10:08:59.971000 ddtcv-0.1.1/ddtcv/tools/postprocess.py
--rw-r--r--   0        0        0     1377 2022-11-18 10:08:59.971000 ddtcv-0.1.1/ddtcv/tools/preprocess.py
--rw-r--r--   0        0        0      826 2023-02-04 06:58:09.619550 ddtcv-0.1.1/ddtcv/wind.py
--rw-r--r--   0        0        0      491 2023-02-07 09:29:57.008053 ddtcv-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      161 2023-02-07 03:02:09.212799 ddtcv-0.1.1/README.md
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 ddtcv-0.1.1/setup.py
--rw-r--r--   0        0        0      810 1970-01-01 00:00:00.000000 ddtcv-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      151 2023-04-22 15:05:55.252636 ddtcv-0.1.2/ddtcv/__init__.py
+-rw-r--r--   0        0        0      159 2023-02-04 06:36:15.784718 ddtcv-0.1.2/ddtcv/abstract.py
+-rw-r--r--   0        0        0     1050 2023-04-22 15:04:47.018605 ddtcv-0.1.2/ddtcv/angle.py
+-rw-r--r--   0        0        0     1205 2023-02-04 06:26:36.847666 ddtcv-0.1.2/ddtcv/onnx.py
+-rw-r--r--   0        0        0  1873116 2022-11-18 10:08:59.992000 ddtcv-0.1.2/ddtcv/static/model/angle_1_rec_en_number_lite/angle_1_rec_en_number_lite.onnx
+-rw-r--r--   0        0        0       31 2022-11-18 10:08:59.992000 ddtcv-0.1.2/ddtcv/static/model/angle_1_rec_en_number_lite/angle_dict.txt
+-rw-r--r--   0        0        0  1873116 2022-11-18 10:09:00.005000 ddtcv-0.1.2/ddtcv/static/model/wind_1_rec_en_number_lite/wind_1_rec_en_number_lite.onnx
+-rw-r--r--   0        0        0       31 2022-11-18 10:09:00.005000 ddtcv-0.1.2/ddtcv/static/model/wind_1_rec_en_number_lite/wind_dict.txt
+-rw-r--r--   0        0        0        0 2023-02-04 06:54:16.389323 ddtcv-0.1.2/ddtcv/tests/__init__.py
+-rw-r--r--   0        0        0      653 2023-02-04 07:08:24.143450 ddtcv-0.1.2/ddtcv/tests/__pycache__/test_angle.cpython-37.pyc
+-rw-r--r--   0        0        0      863 2023-02-04 06:32:06.991371 ddtcv-0.1.2/ddtcv/tests/__pycache__/test_onnx.cpython-37.pyc
+-rw-r--r--   0        0        0      875 2023-04-22 15:06:45.193590 ddtcv-0.1.2/ddtcv/tests/__pycache__/test_wind.cpython-37.pyc
+-rw-r--r--   0        0        0     2227 2023-02-04 06:25:01.374255 ddtcv-0.1.2/ddtcv/tests/image/img.png
+-rw-r--r--   0        0        0   824656 2022-11-26 04:20:44.960000 ddtcv-0.1.2/ddtcv/tests/image/img2.png
+-rw-r--r--   0        0        0     5322 2023-04-22 15:06:45.519492 ddtcv-0.1.2/ddtcv/tests/image/img2_wind.png
+-rw-r--r--   0        0        0      429 2023-04-22 15:07:24.538656 ddtcv-0.1.2/ddtcv/tests/test_angle.py
+-rw-r--r--   0        0        0      511 2023-02-07 03:13:32.466139 ddtcv-0.1.2/ddtcv/tests/test_onnx.py
+-rw-r--r--   0        0        0      423 2023-04-22 15:06:44.990437 ddtcv-0.1.2/ddtcv/tests/test_wind.py
+-rw-r--r--   0        0        0      339 2023-02-04 06:30:40.393471 ddtcv-0.1.2/ddtcv/tools/__pycache__/load_model.cpython-37.pyc
+-rw-r--r--   0        0        0     3741 2023-02-04 06:30:40.483492 ddtcv-0.1.2/ddtcv/tools/__pycache__/postprocess.cpython-37.pyc
+-rw-r--r--   0        0        0     1400 2023-02-04 06:30:40.458484 ddtcv-0.1.2/ddtcv/tools/__pycache__/preprocess.cpython-37.pyc
+-rw-r--r--   0        0        0      165 2022-11-18 10:08:59.971000 ddtcv-0.1.2/ddtcv/tools/load_model.py
+-rw-r--r--   0        0        0     4291 2022-11-18 10:08:59.971000 ddtcv-0.1.2/ddtcv/tools/postprocess.py
+-rw-r--r--   0        0        0     1377 2022-11-18 10:08:59.971000 ddtcv-0.1.2/ddtcv/tools/preprocess.py
+-rw-r--r--   0        0        0     1044 2023-04-22 15:04:47.018605 ddtcv-0.1.2/ddtcv/wind.py
+-rw-r--r--   0        0        0      493 2023-04-22 15:08:19.675464 ddtcv-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-02-07 03:02:09.212799 ddtcv-0.1.2/README.md
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 ddtcv-0.1.2/setup.py
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 ddtcv-0.1.2/PKG-INFO
```

### Comparing `ddtcv-0.1.1/ddtcv/angle.py` & `ddtcv-0.1.2/ddtcv/angle.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """
 create_time: 2023/2/4 14:03
 author: TsangHans
 """
 import os
 import ddtcv
-
+import cv2 as cv
 import numpy as np
 
 from ddtcv.onnx import ONNXModel
 
 _static_dir = os.path.join(ddtcv.__path__[0], "static")
 _default_onnx_model_fp = os.path.join(_static_dir, "model/angle_1_rec_en_number_lite/angle_1_rec_en_number_lite.onnx")
 _default_character_dict_fp = os.path.join(_static_dir, "model/angle_1_rec_en_number_lite/angle_dict.txt")
 _default_wind_rec_model = ONNXModel(_default_onnx_model_fp, _default_character_dict_fp)
 default_x_slice = slice(555, 576)
 default_y_slice = slice(29, 73)
 
 
 def Angle(image: np.ndarray, rec_model: ONNXModel = _default_wind_rec_model, x_slice: slice = default_x_slice,
-         y_slice: slice = default_y_slice):
+          y_slice: slice = default_y_slice):
     x = image[x_slice, y_slice]
     res = rec_model.predict(x)
-    return int(res)
+    return int(res)
+
+
+def save_angle_image(filename: str, image: np.ndarray, x_slice: slice = default_x_slice,
+                     y_slice: slice = default_y_slice):
+    cv.imwrite(filename, image[x_slice, y_slice])
```

### Comparing `ddtcv-0.1.1/ddtcv/onnx.py` & `ddtcv-0.1.2/ddtcv/onnx.py`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/static/model/angle_1_rec_en_number_lite/angle_1_rec_en_number_lite.onnx` & `ddtcv-0.1.2/ddtcv/static/model/angle_1_rec_en_number_lite/angle_1_rec_en_number_lite.onnx`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/static/model/wind_1_rec_en_number_lite/wind_1_rec_en_number_lite.onnx` & `ddtcv-0.1.2/ddtcv/static/model/wind_1_rec_en_number_lite/wind_1_rec_en_number_lite.onnx`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/tests/__pycache__/test_angle.cpython-37.pyc` & `ddtcv-0.1.2/ddtcv/tests/__pycache__/test_angle.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/tests/__pycache__/test_onnx.cpython-37.pyc` & `ddtcv-0.1.2/ddtcv/tests/__pycache__/test_onnx.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/tests/image/img.png` & `ddtcv-0.1.2/ddtcv/tests/image/img.png`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/tests/image/img2.png` & `ddtcv-0.1.2/ddtcv/tests/image/img2.png`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/tools/__pycache__/postprocess.cpython-37.pyc` & `ddtcv-0.1.2/ddtcv/tools/__pycache__/postprocess.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/tools/__pycache__/preprocess.cpython-37.pyc` & `ddtcv-0.1.2/ddtcv/tools/__pycache__/preprocess.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/tools/postprocess.py` & `ddtcv-0.1.2/ddtcv/tools/postprocess.py`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/ddtcv/tools/preprocess.py` & `ddtcv-0.1.2/ddtcv/tools/preprocess.py`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.1/setup.py` & `ddtcv-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 package_data = \
 {'': ['*'],
  'ddtcv': ['static/model/angle_1_rec_en_number_lite/*',
            'static/model/wind_1_rec_en_number_lite/*'],
  'ddtcv.tests': ['image/*']}
 
 install_requires = \
-['numpy==1.21.6', 'onnxruntime==1.13.1', 'opencv_python==4.4.0.46']
+['numpy>=1.21.6,<2.0.0',
+ 'onnxruntime>=1.13.1,<2.0.0',
+ 'opencv-python>=4.4.0.46,<5.0.0.0']
 
 setup_kwargs = {
     'name': 'ddtcv',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'DDT CV.',
     'long_description': 'Examples are as follows.\n```python\nimport ddtcv\n\nwind_value = ddtcv.Wind("your_image_array")\nangle_value = ddtcv.Angle("your_image_array")\n```\nThat\'s all.',
     'author': 'TsangHans',
     'author_email': 'gzzenghan@189.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7',
+    'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `ddtcv-0.1.1/PKG-INFO` & `ddtcv-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ddtcv
-Version: 0.1.1
+Version: 0.1.2
 Summary: DDT CV.
 License: MIT
 Author: TsangHans
 Author-email: gzzenghan@189.cn
-Requires-Python: >=3.7
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (==1.21.6)
-Requires-Dist: onnxruntime (==1.13.1)
-Requires-Dist: opencv_python (==4.4.0.46)
+Requires-Dist: numpy (>=1.21.6,<2.0.0)
+Requires-Dist: onnxruntime (>=1.13.1,<2.0.0)
+Requires-Dist: opencv-python (>=4.4.0.46,<5.0.0.0)
 Description-Content-Type: text/markdown
 
 Examples are as follows.
 ```python
 import ddtcv
 
 wind_value = ddtcv.Wind("your_image_array")
```

