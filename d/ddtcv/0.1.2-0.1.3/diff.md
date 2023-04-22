# Comparing `tmp/ddtcv-0.1.2.tar.gz` & `tmp/ddtcv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddtcv-0.1.2.tar", max compression
+gzip compressed data, was "ddtcv-0.1.3.tar", max compression
```

## Comparing `ddtcv-0.1.2.tar` & `ddtcv-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      151 2023-04-22 15:05:55.252636 ddtcv-0.1.2/ddtcv/__init__.py
--rw-r--r--   0        0        0      159 2023-02-04 06:36:15.784718 ddtcv-0.1.2/ddtcv/abstract.py
--rw-r--r--   0        0        0     1050 2023-04-22 15:04:47.018605 ddtcv-0.1.2/ddtcv/angle.py
--rw-r--r--   0        0        0     1205 2023-02-04 06:26:36.847666 ddtcv-0.1.2/ddtcv/onnx.py
--rw-r--r--   0        0        0  1873116 2022-11-18 10:08:59.992000 ddtcv-0.1.2/ddtcv/static/model/angle_1_rec_en_number_lite/angle_1_rec_en_number_lite.onnx
--rw-r--r--   0        0        0       31 2022-11-18 10:08:59.992000 ddtcv-0.1.2/ddtcv/static/model/angle_1_rec_en_number_lite/angle_dict.txt
--rw-r--r--   0        0        0  1873116 2022-11-18 10:09:00.005000 ddtcv-0.1.2/ddtcv/static/model/wind_1_rec_en_number_lite/wind_1_rec_en_number_lite.onnx
--rw-r--r--   0        0        0       31 2022-11-18 10:09:00.005000 ddtcv-0.1.2/ddtcv/static/model/wind_1_rec_en_number_lite/wind_dict.txt
--rw-r--r--   0        0        0        0 2023-02-04 06:54:16.389323 ddtcv-0.1.2/ddtcv/tests/__init__.py
--rw-r--r--   0        0        0      653 2023-02-04 07:08:24.143450 ddtcv-0.1.2/ddtcv/tests/__pycache__/test_angle.cpython-37.pyc
--rw-r--r--   0        0        0      863 2023-02-04 06:32:06.991371 ddtcv-0.1.2/ddtcv/tests/__pycache__/test_onnx.cpython-37.pyc
--rw-r--r--   0        0        0      875 2023-04-22 15:06:45.193590 ddtcv-0.1.2/ddtcv/tests/__pycache__/test_wind.cpython-37.pyc
--rw-r--r--   0        0        0     2227 2023-02-04 06:25:01.374255 ddtcv-0.1.2/ddtcv/tests/image/img.png
--rw-r--r--   0        0        0   824656 2022-11-26 04:20:44.960000 ddtcv-0.1.2/ddtcv/tests/image/img2.png
--rw-r--r--   0        0        0     5322 2023-04-22 15:06:45.519492 ddtcv-0.1.2/ddtcv/tests/image/img2_wind.png
--rw-r--r--   0        0        0      429 2023-04-22 15:07:24.538656 ddtcv-0.1.2/ddtcv/tests/test_angle.py
--rw-r--r--   0        0        0      511 2023-02-07 03:13:32.466139 ddtcv-0.1.2/ddtcv/tests/test_onnx.py
--rw-r--r--   0        0        0      423 2023-04-22 15:06:44.990437 ddtcv-0.1.2/ddtcv/tests/test_wind.py
--rw-r--r--   0        0        0      339 2023-02-04 06:30:40.393471 ddtcv-0.1.2/ddtcv/tools/__pycache__/load_model.cpython-37.pyc
--rw-r--r--   0        0        0     3741 2023-02-04 06:30:40.483492 ddtcv-0.1.2/ddtcv/tools/__pycache__/postprocess.cpython-37.pyc
--rw-r--r--   0        0        0     1400 2023-02-04 06:30:40.458484 ddtcv-0.1.2/ddtcv/tools/__pycache__/preprocess.cpython-37.pyc
--rw-r--r--   0        0        0      165 2022-11-18 10:08:59.971000 ddtcv-0.1.2/ddtcv/tools/load_model.py
--rw-r--r--   0        0        0     4291 2022-11-18 10:08:59.971000 ddtcv-0.1.2/ddtcv/tools/postprocess.py
--rw-r--r--   0        0        0     1377 2022-11-18 10:08:59.971000 ddtcv-0.1.2/ddtcv/tools/preprocess.py
--rw-r--r--   0        0        0     1044 2023-04-22 15:04:47.018605 ddtcv-0.1.2/ddtcv/wind.py
--rw-r--r--   0        0        0      493 2023-04-22 15:08:19.675464 ddtcv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      161 2023-02-07 03:02:09.212799 ddtcv-0.1.2/README.md
--rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 ddtcv-0.1.2/setup.py
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 ddtcv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-04-22 15:25:45.668497 ddtcv-0.1.3/ddtcv/__init__.py
+-rw-r--r--   0        0        0      159 2023-02-04 06:36:15.784718 ddtcv-0.1.3/ddtcv/abstract.py
+-rw-r--r--   0        0        0     1211 2023-04-22 15:24:28.224045 ddtcv-0.1.3/ddtcv/angle.py
+-rw-r--r--   0        0        0     1205 2023-02-04 06:26:36.847666 ddtcv-0.1.3/ddtcv/onnx.py
+-rw-r--r--   0        0        0  1873116 2022-11-18 10:08:59.992000 ddtcv-0.1.3/ddtcv/static/model/angle_1_rec_en_number_lite/angle_1_rec_en_number_lite.onnx
+-rw-r--r--   0        0        0       31 2022-11-18 10:08:59.992000 ddtcv-0.1.3/ddtcv/static/model/angle_1_rec_en_number_lite/angle_dict.txt
+-rw-r--r--   0        0        0  1873116 2022-11-18 10:09:00.005000 ddtcv-0.1.3/ddtcv/static/model/wind_1_rec_en_number_lite/wind_1_rec_en_number_lite.onnx
+-rw-r--r--   0        0        0       31 2022-11-18 10:09:00.005000 ddtcv-0.1.3/ddtcv/static/model/wind_1_rec_en_number_lite/wind_dict.txt
+-rw-r--r--   0        0        0        0 2023-02-04 06:54:16.389323 ddtcv-0.1.3/ddtcv/tests/__init__.py
+-rw-r--r--   0        0        0      879 2023-04-22 15:24:49.362104 ddtcv-0.1.3/ddtcv/tests/__pycache__/test_angle.cpython-37.pyc
+-rw-r--r--   0        0        0      863 2023-02-04 06:32:06.991371 ddtcv-0.1.3/ddtcv/tests/__pycache__/test_onnx.cpython-37.pyc
+-rw-r--r--   0        0        0      875 2023-04-22 15:06:45.193590 ddtcv-0.1.3/ddtcv/tests/__pycache__/test_wind.cpython-37.pyc
+-rw-r--r--   0        0        0     2227 2023-02-04 06:25:01.374255 ddtcv-0.1.3/ddtcv/tests/image/img.png
+-rw-r--r--   0        0        0   824656 2022-11-26 04:20:44.960000 ddtcv-0.1.3/ddtcv/tests/image/img2.png
+-rw-r--r--   0        0        0     5322 2023-04-22 15:06:45.519492 ddtcv-0.1.3/ddtcv/tests/image/img2_wind.png
+-rw-r--r--   0        0        0      429 2023-04-22 15:07:24.538656 ddtcv-0.1.3/ddtcv/tests/test_angle.py
+-rw-r--r--   0        0        0      511 2023-02-07 03:13:32.466139 ddtcv-0.1.3/ddtcv/tests/test_onnx.py
+-rw-r--r--   0        0        0      423 2023-04-22 15:06:44.990437 ddtcv-0.1.3/ddtcv/tests/test_wind.py
+-rw-r--r--   0        0        0      339 2023-02-04 06:30:40.393471 ddtcv-0.1.3/ddtcv/tools/__pycache__/load_model.cpython-37.pyc
+-rw-r--r--   0        0        0     3741 2023-02-04 06:30:40.483492 ddtcv-0.1.3/ddtcv/tools/__pycache__/postprocess.cpython-37.pyc
+-rw-r--r--   0        0        0     1400 2023-02-04 06:30:40.458484 ddtcv-0.1.3/ddtcv/tools/__pycache__/preprocess.cpython-37.pyc
+-rw-r--r--   0        0        0      165 2022-11-18 10:08:59.971000 ddtcv-0.1.3/ddtcv/tools/load_model.py
+-rw-r--r--   0        0        0     4291 2022-11-18 10:08:59.971000 ddtcv-0.1.3/ddtcv/tools/postprocess.py
+-rw-r--r--   0        0        0     1377 2022-11-18 10:08:59.971000 ddtcv-0.1.3/ddtcv/tools/preprocess.py
+-rw-r--r--   0        0        0     1210 2023-04-22 15:25:32.781242 ddtcv-0.1.3/ddtcv/wind.py
+-rw-r--r--   0        0        0      493 2023-04-22 15:25:58.825808 ddtcv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-02-07 03:02:09.212799 ddtcv-0.1.3/README.md
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 ddtcv-0.1.3/setup.py
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 ddtcv-0.1.3/PKG-INFO
```

### Comparing `ddtcv-0.1.2/ddtcv/angle.py` & `ddtcv-0.1.3/ddtcv/angle.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,16 +14,20 @@
 _default_character_dict_fp = os.path.join(_static_dir, "model/angle_1_rec_en_number_lite/angle_dict.txt")
 _default_wind_rec_model = ONNXModel(_default_onnx_model_fp, _default_character_dict_fp)
 default_x_slice = slice(555, 576)
 default_y_slice = slice(29, 73)
 
 
 def Angle(image: np.ndarray, rec_model: ONNXModel = _default_wind_rec_model, x_slice: slice = default_x_slice,
-          y_slice: slice = default_y_slice):
+          y_slice: slice = default_y_slice) -> int:
     x = image[x_slice, y_slice]
-    res = rec_model.predict(x)
-    return int(res)
+    res = rec_angle(x, rec_model)
+    return res
+
+
+def rec_angle(angle_image: np.ndarray, rec_model: ONNXModel = _default_wind_rec_model) -> int:
+    return int(rec_model.predict(angle_image))
 
 
 def save_angle_image(filename: str, image: np.ndarray, x_slice: slice = default_x_slice,
-                     y_slice: slice = default_y_slice):
+                     y_slice: slice = default_y_slice) -> None:
     cv.imwrite(filename, image[x_slice, y_slice])
```

### Comparing `ddtcv-0.1.2/ddtcv/onnx.py` & `ddtcv-0.1.3/ddtcv/onnx.py`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/static/model/angle_1_rec_en_number_lite/angle_1_rec_en_number_lite.onnx` & `ddtcv-0.1.3/ddtcv/static/model/angle_1_rec_en_number_lite/angle_1_rec_en_number_lite.onnx`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/static/model/wind_1_rec_en_number_lite/wind_1_rec_en_number_lite.onnx` & `ddtcv-0.1.3/ddtcv/static/model/wind_1_rec_en_number_lite/wind_1_rec_en_number_lite.onnx`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/tests/__pycache__/test_onnx.cpython-37.pyc` & `ddtcv-0.1.3/ddtcv/tests/__pycache__/test_onnx.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/tests/__pycache__/test_wind.cpython-37.pyc` & `ddtcv-0.1.3/ddtcv/tests/__pycache__/test_wind.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/tests/image/img.png` & `ddtcv-0.1.3/ddtcv/tests/image/img.png`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/tests/image/img2.png` & `ddtcv-0.1.3/ddtcv/tests/image/img2.png`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/tests/image/img2_wind.png` & `ddtcv-0.1.3/ddtcv/tests/image/img2_wind.png`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/tools/__pycache__/postprocess.cpython-37.pyc` & `ddtcv-0.1.3/ddtcv/tools/__pycache__/postprocess.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/tools/__pycache__/preprocess.cpython-37.pyc` & `ddtcv-0.1.3/ddtcv/tools/__pycache__/preprocess.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/tools/postprocess.py` & `ddtcv-0.1.3/ddtcv/tools/postprocess.py`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/ddtcv/tools/preprocess.py` & `ddtcv-0.1.3/ddtcv/tools/preprocess.py`

 * *Files identical despite different names*

### Comparing `ddtcv-0.1.2/setup.py` & `ddtcv-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = \
 ['numpy>=1.21.6,<2.0.0',
  'onnxruntime>=1.13.1,<2.0.0',
  'opencv-python>=4.4.0.46,<5.0.0.0']
 
 setup_kwargs = {
     'name': 'ddtcv',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'DDT CV.',
     'long_description': 'Examples are as follows.\n```python\nimport ddtcv\n\nwind_value = ddtcv.Wind("your_image_array")\nangle_value = ddtcv.Angle("your_image_array")\n```\nThat\'s all.',
     'author': 'TsangHans',
     'author_email': 'gzzenghan@189.cn',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ddtcv-0.1.2/PKG-INFO` & `ddtcv-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddtcv
-Version: 0.1.2
+Version: 0.1.3
 Summary: DDT CV.
 License: MIT
 Author: TsangHans
 Author-email: gzzenghan@189.cn
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

