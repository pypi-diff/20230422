# Comparing `tmp/measuring-tools-0.4.1.tar.gz` & `tmp/measuring-tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "measuring-tools-0.4.1.tar", last modified: Sat Sep 17 18:57:13 2022, max compression
+gzip compressed data, was "measuring-tools-0.5.0.tar", last modified: Sat Apr 22 13:24:18 2023, max compression
```

## Comparing `measuring-tools-0.4.1.tar` & `measuring-tools-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0 BlackLotus   (502) staff       (20)        0 2022-09-17 18:57:13.960000 measuring-tools-0.4.1/
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)    10758 2022-08-12 19:57:02.000000 measuring-tools-0.4.1/LICENSE
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)     1839 2022-09-17 18:57:13.990000 measuring-tools-0.4.1/PKG-INFO
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)     1310 2022-08-18 16:25:32.000000 measuring-tools-0.4.1/README.md
-drwxrwxrwx   0 BlackLotus   (502) staff       (20)        0 2022-09-17 18:57:13.960000 measuring-tools-0.4.1/measuring_tools/
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)     1278 2022-09-17 18:07:25.000000 measuring-tools-0.4.1/measuring_tools/__init__.py
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)     7710 2022-09-17 18:53:25.000000 measuring-tools-0.4.1/measuring_tools/length.py
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)     7658 2022-09-17 18:53:25.000000 measuring-tools-0.4.1/measuring_tools/mass.py
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)     6559 2022-09-17 18:53:25.000000 measuring-tools-0.4.1/measuring_tools/temperature.py
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)     6121 2022-09-17 18:53:25.000000 measuring-tools-0.4.1/measuring_tools/volume.py
-drwxrwxrwx   0 BlackLotus   (502) staff       (20)        0 2022-09-17 18:57:13.960000 measuring-tools-0.4.1/measuring_tools.egg-info/
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)     1839 2022-09-17 18:57:13.000000 measuring-tools-0.4.1/measuring_tools.egg-info/PKG-INFO
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)      317 2022-09-17 18:57:13.000000 measuring-tools-0.4.1/measuring_tools.egg-info/SOURCES.txt
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)        1 2022-09-17 18:57:13.000000 measuring-tools-0.4.1/measuring_tools.egg-info/dependency_links.txt
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)       16 2022-09-17 18:57:13.000000 measuring-tools-0.4.1/measuring_tools.egg-info/top_level.txt
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)       38 2022-09-17 18:57:13.990000 measuring-tools-0.4.1/setup.cfg
--rwxrwxrwx   0 BlackLotus   (502) staff       (20)      808 2022-09-17 18:53:25.000000 measuring-tools-0.4.1/setup.py
+drwxrwxr-x   0 blacklotus  (1000) blacklotus  (1000)        0 2023-04-22 13:24:18.101961 measuring-tools-0.5.0/
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)    10758 2022-12-24 14:09:24.000000 measuring-tools-0.5.0/LICENSE
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     1839 2023-04-22 13:24:18.100961 measuring-tools-0.5.0/PKG-INFO
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     1310 2022-12-24 14:09:24.000000 measuring-tools-0.5.0/README.md
+drwxrwxr-x   0 blacklotus  (1000) blacklotus  (1000)        0 2023-04-22 13:24:18.098961 measuring-tools-0.5.0/measuring_tools/
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     1397 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/measuring_tools/__init__.py
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     7355 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/measuring_tools/length.py
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     7329 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/measuring_tools/mass.py
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     6332 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/measuring_tools/temperature.py
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     5886 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/measuring_tools/volume.py
+drwxrwxr-x   0 blacklotus  (1000) blacklotus  (1000)        0 2023-04-22 13:24:18.099961 measuring-tools-0.5.0/measuring_tools.egg-info/
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     1839 2023-04-22 13:24:18.000000 measuring-tools-0.5.0/measuring_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)      404 2023-04-22 13:24:18.000000 measuring-tools-0.5.0/measuring_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)        1 2023-04-22 13:24:18.000000 measuring-tools-0.5.0/measuring_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)       16 2023-04-22 13:24:18.000000 measuring-tools-0.5.0/measuring_tools.egg-info/top_level.txt
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)       38 2023-04-22 13:24:18.101961 measuring-tools-0.5.0/setup.cfg
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)      808 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/setup.py
+drwxrwxr-x   0 blacklotus  (1000) blacklotus  (1000)        0 2023-04-22 13:24:18.100961 measuring-tools-0.5.0/tests/
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     7295 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/tests/test_length.py
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     2381 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/tests/test_mass.py
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     6387 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/tests/test_temperature.py
+-rw-rw-r--   0 blacklotus  (1000) blacklotus  (1000)     5110 2023-04-22 13:11:21.000000 measuring-tools-0.5.0/tests/test_volume.py
```

### Comparing `measuring-tools-0.4.1/LICENSE` & `measuring-tools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `measuring-tools-0.4.1/PKG-INFO` & `measuring-tools-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: measuring-tools
-Version: 0.4.1
+Version: 0.5.0
 Summary: Classes to help with common types of measurements
 Home-page: https://bitbucket.org/blacklotus231/measuring-tools
 Author: James Baker Jr
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `measuring-tools-0.4.1/README.md` & `measuring-tools-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `measuring-tools-0.4.1/measuring_tools/__init__.py` & `measuring-tools-0.5.0/measuring_tools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 '''Provides a check for a Python version greater than or equal to 3.10.
 Provides the Measurement base class.
 '''
 
 import platform
 
+
 if int(platform.python_version_tuple()[1]) < 10:
     raise ImportError('measuring-tools requires Python versions 3.10 or later.')
 del platform
 
+
 class Measurement:
     '''Base Class for other measurments'''
 
-    float_point_tol = 1e-05
+
+    FLOAT_POINT_TOL = 1e-05
+
 
     def __init__(self, value: int | float, measurement: str):
         self.value = value
         self.measurement = measurement
 
+
     def __repr__(self):
         return f'{self.__class__.__name__}(value={self.value}, measurement={self.measurement!r})'
 
+
     def __str__(self):
         return f'{self.value} {self.measurement}(s)'
 
+
     def __int__(self):
         return int(self.value)
 
+
     def __float__(self):
         return float(self.value)
 
+
     def __iadd__(self, other_value):
         self.value += other_value
         return self
 
+
     def __isub__(self, other_value):
         self.value -= other_value
         return self
 
+
     def __imul__(self, other_value):
         self.value *= other_value
         return self
 
+
     def __itruediv__(self, other_value):
         self.value /= other_value
         return self
 
+
     def __ifloordiv__(self, other_value):
         self.value //= other_value
-        return self
+        return self
+
+    
+    def __imod__(self, other_value):
+        self.value %= other_value
+        return self
+
```

### Comparing `measuring-tools-0.4.1/measuring_tools/length.py` & `measuring-tools-0.5.0/measuring_tools/length.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,199 +1,211 @@
 '''Functionality for length conversion and length equality checks.
-Values of two different temperatures recorded in different measurements are considered equal
-if the converted values within a relative tolerance or absolute tolerance of float_point_tol.
-The default for float_point_tol is 1e-05.
+Values of two different lengths recorded in different measurements are considered equal
+if the converted values within a relative tolerance or absolute tolerance of FLOAT_POINT_TOL.
+The default for FLOAT_POINT_TOL is 1e-05.
 '''
 
+
+import functools
 from math import isclose, floor, ceil
 from measuring_tools import Measurement
 
+
 def __dir__():
     return ('Length', 'MARATHON', '__doc__', '__file__', '__loader__', '__name__', '__package__', '__spec__')
 
+
+@functools.total_ordering
 class Length(Measurement):
-    '''Length Converter for Metric and English Imperial Units'''
+    '''Length Converter for Metric and English Imperial Units
+	* value is expected to be either an integer or a float
+	* measurement can be one of four options (defaults to meter):
+		- meter
+		- kilometer
+		- yard
+		- mile
+	'''
+
 
     def __init__(self, value: int | float, measurement: str='meter'):
         if not measurement in ('meter', 'kilometer', 'yard', 'mile'):
             raise ValueError('Value must be meter, kilometer, yard, or mile')
         super().__init__(value, measurement)
 
+
     def __round__(self, ndigits):
         return Length(round(self.value, ndigits=ndigits), self.measurement)
 
+
     def __abs__(self):
         return Length(abs(self.value), self.measurement)
 
+
     def __floor__(self):
         return Length(floor(self.value), self.measurement)
 
+
     def __ceil__(self):
         return Length(ceil(self.value), self.measurement)
 
+
     def __eq__(self, other):
         match self.measurement:
             case 'meter':
-                return isclose(self.value, other.to_meter().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
+                return isclose(self.value, other.to_meter().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'yard':
-                return isclose(self.value, other.to_yard().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
+                return isclose(self.value, other.to_yard().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'mile':
-                return isclose(self.value, other.to_mile().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
+                return isclose(self.value, other.to_mile().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'kilometer':
-                return isclose(self.value, other.to_kilometer().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
-        
-    def __ne__(self, other):
-        match self.measurement:
-            case 'meter':
-                return not self.value == other.to_meter().value
-            case 'yard':
-                return not self.value == other.to_yard().value
-            case 'mile':
-                return not self.value == other.to_mile().value
-            case 'kilometer':
-                return not self.value == other.to_kilometer().value
+                return isclose(self.value, other.to_kilometer().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
+
 
     def __lt__(self, other):
         if self == other:
             return False
         match self.measurement:
             case 'meter':
                 return self.value < other.to_meter().value
             case 'yard':
                 return self.value < other.to_yard().value
             case 'mile':
                 return self.value < other.to_mile().value
             case 'kilometer':
                 return self.value < other.to_kilometer().value
 
-    def __le__(self, other):
-        return self == other or self < other
-
-    def __gt__(self, other):
-        if self == other:
-            return False
-        match self.measurement:
-            case 'meter':
-                return self.value > other.to_meter().value
-            case 'yard':
-                return self.value > other.to_yard().value
-            case 'mile':
-                return self.value > other.to_mile().value
-            case 'kilometer':
-                return self.value > other.to_kilometer().value
-
-    def __ge__(self, other):
-        return self == other or self > other
 
     def __add__(self, other):
         match self.measurement:
             case 'meter':
                 total = self.value + other.to_meter().value
             case 'yard':
                 total = self.value + other.to_yard().value
             case 'mile':
                 total = self.value + other.to_mile().value
             case 'kilometer':
                 total = self.value + other.to_kilometer().value
         return Length(total, self.measurement)
 
+
     def __sub__(self, other):
         match self.measurement:
             case 'meter':
                 diff = self.value - other.to_meter().value
             case 'yard':
                 diff = self.value - other.to_yard().value
             case 'mile':
                 diff = self.value - other.to_mile().value
             case 'kilometer':
                 diff = self.value - other.to_kilometer().value
         return Length(diff, self.measurement)
 
+
     def __mul__(self, other):
         match self.measurement:
             case 'meter':
                 product = self.value * other.to_meter().value
             case 'yard':
                 product = self.value * other.to_yard().value
             case 'mile':
                 product = self.value * other.to_mile().value
             case 'kilometer':
                 product = self.value * other.to_kilometer().value
         return Length(product, self.measurement)
 
+
     def __truediv__(self, other):
         match self.measurement:
             case 'meter':
                 result = self.value / other.to_meter().value
             case 'yard':
                 result = self.value / other.to_yard().value
             case 'mile':
                 result = self.value / other.to_mile().value
             case 'kilometer':
                 result = self.value / other.to_kilometer().value
         return Length(result, self.measurement)
 
+
     def __floordiv__(self, other):
         match self.measurement:
             case 'meter':
                 result = self.value // other.to_meter().value
             case 'yard':
                 result = self.value // other.to_yard().value
             case 'mile':
                 result = self.value // other.to_mile().value
             case 'kilometer':
                 result = self.value // other.to_kilometer().value
         return Length(result, self.measurement)
 
+
+    def __mod__(self, other):
+        match self.measurement:
+            case 'meter':
+                result = self.value % other.to_meter().value
+            case 'yard':
+                result = self.value % other.to_yard().value
+            case 'mile':
+                result = self.value % other.to_mile().value
+            case 'kilometer':
+                result = self.value % other.to_kilometer().value
+        return Length(result, self.measurement)
+
+
     def to_meter(self):
         '''Convert the length to meter'''
         measure = 'meter'
         match self.measurement:
             case 'meter':
                 return self
             case 'yard':
                 return Length((self.value * 0.9144), measurement=measure)
             case 'mile':
                 return Length((self.value * 1_609.344), measurement=measure)
             case 'kilometer':
                 return Length((self.value * 1_000), measurement=measure)
 
+
     def to_yard(self):
         '''Convert the length to yard'''
         measure = 'yard'
         match self.measurement:
             case 'yard':
                 return self
             case 'meter':
                 return Length((self.value / 0.9144), measurement=measure)
             case 'mile':
                 return Length((self.value * 1_760), measurement=measure)
             case 'kilometer':
                 return Length((self.value * 1_093.613), measurement=measure)
 
+
     def to_mile(self):
         '''Convert the length to mile'''
         measure = 'mile'
         match self.measurement:
             case 'mile':
                 return self
             case 'meter':
                 return Length((self.value / 1_609.344), measurement=measure)
             case 'yard':
                 return Length((self.value / 1_760), measurement=measure)
             case 'kilometer':
                 return Length((self.value / 1.609344), measurement=measure)
 
+
     def to_kilometer(self):
         '''Convert the length to kilometer'''
         measure = 'kilometer'
         match self.measurement:
             case 'kilometer':
                 return self
             case 'meter':
                 return Length((self.value / 1_000), measurement=measure)
             case 'yard':
                 return Length((self.value / 1_093.613), measurement=measure)
             case 'mile':
                 return Length((self.value * 1.609344 ), measurement=measure)
 
-MARATHON = Length(42.195, measurement='kilometer')
+
+MARATHON = Length(42.195, measurement='kilometer')
```

### Comparing `measuring-tools-0.4.1/measuring_tools/mass.py` & `measuring-tools-0.5.0/measuring_tools/mass.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,197 +1,208 @@
 '''Functionality for mass conversion and mass equality checks.
-Values of two different temperatures recorded in different measurements are considered equal
-if the converted values within a relative tolerance or absolute tolerance of float_point_tol.
-The default for float_point_tol is 1e-05.
+Values of two different masses recorded in different measurements are considered equal
+if the converted values within a relative tolerance or absolute tolerance of FLOAT_POINT_TOL.
+The default for FLOAT_POINT_TOL is 1e-05.
 '''
 
+
+import functools
 from math import isclose, floor, ceil
 from measuring_tools import Measurement
 
+
 def __dir__():
     return ('Mass', '__doc__', '__file__', '__loader__', '__name__', '__package__', '__spec__')
 
+
+@functools.total_ordering
 class Mass(Measurement):
-    '''Mass Converter class'''
+    '''Mass Converter class
+    * value is expected to be either an integer or a float
+    * measurement can be one of four options (defaults to gram)
+        - gram
+        - kilogram
+        - ton_us
+        - pound
+    '''
+
 
     def __init__(self, value: int | float, measurement: str='gram'):
         if not measurement in ('gram', 'kilogram', 'ton_us', 'pound'):
             raise ValueError('Value must be gram, kilogram, ton_us, or pound')
         super().__init__(value, measurement)
 
+
     def __round__(self, ndigits):
         return Mass(round(self.value, ndigits=ndigits), self.measurement)
 
+
     def __abs__(self):
         return Mass(abs(self.value), self.measurement)
 
+
     def __floor__(self):
         return Mass(floor(self.value), self.measurement)
 
+
     def __ceil__(self):
         return Mass(ceil(self.value), self.measurement)
 
+
     def __eq__(self, other):
         match self.measurement:
             case 'gram':
-                return isclose(self.value, other.to_gram().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
-            case 'ton_us':
-                return isclose(self.value, other.to_ton_us().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
-            case 'pound':
-                return isclose(self.value, other.to_pound().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
-            case 'kilogram':
-                return isclose(self.value, other.to_kilogram().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
-        
-    def __ne__(self, other):
-        match self.measurement:
-            case 'gram':
-                return not self.value == other.to_gram().value
+                return isclose(self.value, other.to_gram().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'ton_us':
-                return not self.value == other.to_ton_us().value
+                return isclose(self.value, other.to_ton_us().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'pound':
-                return not self.value == other.to_pound().value
+                return isclose(self.value, other.to_pound().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'kilogram':
-                return not self.value == other.to_kilogram().value
+                return isclose(self.value, other.to_kilogram().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
+
 
     def __lt__(self, other):
         if self == other:
             return False
         match self.measurement:
             case 'gram':
                 return self.value < other.to_gram().value
             case 'ton_us':
                 return self.value < other.to_ton_us().value
             case 'pound':
                 return self.value < other.to_pound().value
             case 'kilogram':
                 return self.value < other.to_kilogram().value
 
-    def __le__(self, other):
-        return self == other or self < other
-
-    def __gt__(self, other):
-        if self == other:
-            return False
-        match self.measurement:
-            case 'gram':
-                return self.value > other.to_gram().value
-            case 'ton_us':
-                return self.value > other.to_ton_us().value
-            case 'pound':
-                return self.value > other.to_pound().value
-            case 'kilogram':
-                return self.value > other.to_kilogram().value
-
-    def __ge__(self, other):
-        return self == other or self > other
 
     def __add__(self, other):
         match self.measurement:
             case 'gram':
                 total = self.value + other.to_gram().value
             case 'ton_us':
                 total = self.value + other.to_ton_us().value
             case 'pound':
                 total = self.value + other.to_pound().value
             case 'kilogram':
                 total = self.value + other.to_kilogram().value
         return Mass(total, self.measurement)
 
+
     def __sub__(self, other):
         match self.measurement:
             case 'gram':
                 diff = self.value - other.to_gram().value
             case 'ton_us':
                 diff = self.value - other.to_ton_us().value
             case 'pound':
                 diff = self.value - other.to_pound().value
             case 'kilogram':
                 diff = self.value - other.to_kilogram().value
         return Mass(diff, self.measurement)
 
+
     def __mul__(self, other):
         match self.measurement:
             case 'gram':
                 product = self.value * other.to_gram().value
             case 'ton_us':
                 product = self.value * other.to_ton_us().value
             case 'pound':
                 product = self.value * other.to_pound().value
             case 'kilogram':
                 product = self.value * other.to_kilogram().value
         return Mass(product, self.measurement)
 
+
     def __truediv__(self, other):
         match self.measurement:
             case 'gram':
                 result = self.value / other.to_gram().value
             case 'ton_us':
                 result = self.value / other.to_ton_us().value
             case 'pound':
                 result = self.value / other.to_pound().value
             case 'kilogram':
                 result = self.value / other.to_kilogram().value
         return Mass(result, self.measurement)
 
+
     def __floordiv__(self, other):
         match self.measurement:
             case 'gram':
                 result = self.value // other.to_gram().value
             case 'ton_us':
                 result = self.value // other.to_ton_us().value
             case 'pound':
                 result = self.value // other.to_pound().value
             case 'kilogram':
                 result = self.value // other.to_kilogram().value
         return Mass(result, self.measurement)
 
+
+    def __mod__(self, other):
+        match self.measurement:
+            case 'gram':
+                result = self.value % other.to_gram().value
+            case 'ton_us':
+                result = self.value % other.to_ton_us().value
+            case 'pound':
+                result = self.value % other.to_pound().value
+            case 'kilogram':
+                result = self.value % other.to_kilogram().value
+        return Mass(result, self.measurement)
+
+
     def to_gram(self):
             '''Convert the length to gram'''
             measure = 'gram'
             match self.measurement:
                 case 'gram':
                     return self
                 case 'ton_us':
                     return Mass((self.value / 907_184.74) , measurement=measure)
                 case 'pound':
                     return Mass((self.value / 453.59237) , measurement=measure)
                 case 'kilogram':
                     return Mass((self.value / 1_000) , measurement=measure)
 
+
     def to_ton_us(self):
         '''Convert the length to ton_us'''
         measure = 'ton_us'
         match self.measurement:
             case 'ton_us':
                 return self
             case 'gram':
                 return Mass((self.value * 907_184.74) , measurement=measure)
             case 'pound':
                 return Mass((self.value * 2_000) , measurement=measure)
             case 'kilogram':
                 return Mass((self.value * 907.18474) , measurement=measure)
 
+
     def to_pound(self):
         '''Convert the length to pound'''
         measure = 'pound'
         match self.measurement:
             case 'pound':
                 return self
             case 'gram':
                 return Mass((self.value * 453.59237) , measurement=measure)
             case 'ton_us':
                 return Mass((self.value / 2_000) , measurement=measure)
             case 'kilogram':
                 return Mass((self.value / 2.2046226218) , measurement=measure)
 
+
     def to_kilogram(self):
         '''Convert the length to kilogram'''
         measure = 'kilogram'
         match self.measurement:
             case 'kilogram':
                 return self
             case 'gram':
                 return Mass((self.value * 1_000), measurement=measure)
             case 'ton_us':
                 return Mass((self.value / 907.18474) , measurement=measure)
             case 'pound':
-                return Mass((self.value * 2.2046226218) , measurement=measure)
+                return Mass((self.value * 2.2046226218) , measurement=measure)
```

### Comparing `measuring-tools-0.4.1/measuring_tools/temperature.py` & `measuring-tools-0.5.0/measuring_tools/temperature.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,166 +1,178 @@
 ''' Functionality for teperature conversions and temperature equality checks recorded in Fahrenheit, Celsius,
 and Kelvin. Values of two different temperatures recorded in different measurements are considered equal
-if the converted values within a relative tolerance or absolute tolerance of float_point_tol.
-The default for float_point_tol is 1e-05.
+if the converted values within a relative tolerance or absolute tolerance of FLOAT_POINT_TOL.
+The default for FLOAT_POINT_TOL is 1e-05.
 '''
 
+
+import functools
 from math import isclose, floor, ceil
 from measuring_tools import Measurement
 
+
 def __dir__():
     return ('Temperature', 'ABSOLUTE_ZERO', 'FREEZING_POINT', 'BOILING_POINT', '__doc__', '__file__', '__loader__', '__name__', '__package__', '__spec__')
 
+
+@functools.total_ordering
 class Temperature(Measurement):
-    '''Temperature Converter for Fahrenheit, Celsius, and Kelvin'''
+    '''Temperature Converter for Fahrenheit, Celsius, and Kelvin
+    * value is expected to be either an integer or a float
+    * measurement can be one of three options (defaults to fahrenheit)
+        - fahrenheit
+        - celsius
+        - kelvin
+    '''
+
 
     def __init__(self, value: int | float, measurement: str='fahrenheit'):
         if not measurement in ('fahrenheit', 'celsius', 'kelvin'):
             raise ValueError('Value must be fahrenheit, celsius, or kelvin')
         super().__init__(value, measurement)
 
+
     def __str__(self):
         return f'{self.value} degress {self.measurement}'
 
+
     def __round__(self, ndigits):
         return Temperature(round(self.value, ndigits=ndigits), self.measurement)
         
     def __abs__(self):
         return Temperature(abs(self.value), self.measurement)
 
+
     def __floor__(self):
         return Temperature(floor(self.value), self.measurement)
 
+
     def __ceil__(self):
         return Temperature(ceil(self.value), self.measurement)
 
+
     def __eq__(self, other):
         match self.measurement:
             case 'fahrenheit':
-                return isclose(self.value, other.to_fahrenheit().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
+                return isclose(self.value, other.to_fahrenheit().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'celsius':
-                return isclose(self.value, other.to_celsius().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
+                return isclose(self.value, other.to_celsius().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'kelvin':
-                return isclose(self.value, other.to_kelvin().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
+                return isclose(self.value, other.to_kelvin().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
 
-    def __ne__(self, other):
-        match self.measurement:
-            case 'fahrenheit':
-                return not self.value == other.to_fahrenheit().value
-            case 'celsius':
-                return not self.value == other.to_celsius().value
-            case 'kelvin':
-                return not self.value == other.to_kelvin().value
 
     def __lt__(self, other):
         if self == other:
             return False
         match self.measurement:
             case 'fahrenheit':
                 return self.value < other.to_fahrenheit().value
             case 'celsius':
                 return self.value < other.to_celsius().value
             case 'kelvin':
                 return self.value < other.to_kelvin().value
 
-    def __le__(self, other):
-        return self == other or self < other
-
-    def __gt__(self, other):
-        if self == other:
-            return False
-        match self.measurement:
-            case 'fahrenheit':
-                return self.value > other.to_fahrenheit().value
-            case 'celsius':
-                return self.value > other.to_celsius().value
-            case 'kelvin':
-                return self.value > other.to_kelvin().value
-
-    def __ge__(self, other):
-        return self == other or self > other
 
     def __add__(self, other):
         match self.measurement:
             case 'fahrenheit':
                 total = self.value + other.to_fahrenheit().value
             case 'celsius':
                 total = self.value + other.to_celsius().value
             case 'kelvin':
                 total = self.value + other.to_kelvin().value
         return Temperature(total, self.measurement)
 
+
     def __sub__(self, other):
         match self.measurement:
             case 'fahrenheit':
                 diff = self.value - other.to_fahrenheit().value
             case 'celsius':
                 diff = self.value - other.to_celsius().value
             case 'kelvin':
                 diff = self.value - other.to_kelvin().value
         return Temperature(diff, self.measurement)
 
+
     def __mul__(self, other):
         match self.measurement:
             case 'fahrenheit':
                 product = self.value * other.to_fahrenheit().value
             case 'celsius':
                 product = self.value * other.to_celsius().value
             case 'kelvin':
                 product = self.value * other.to_kelvin().value
         return Temperature(product, self.measurement)
 
+
     def __truediv__(self, other):
         match self.measurement:
             case 'fahrenheit':
                 result = self.value / other.to_fahrenheit().value
             case 'celsius':
                 result = self.value / other.to_celsius().value
             case 'kelvin':
                 result = self.value / other.to_kelvin().value
         return Temperature(result, self.measurement)
 
+
     def __floordiv__(self, other):
         match self.measurement:
             case 'fahrenheit':
                 quotient = self.value // other.to_fahrenheit().value
             case 'celsius':
                 quotient = self.value // other.to_celsius().value
             case 'kelvin':
                 quotient = self.value // other.to_kelvin().value
         return Temperature(quotient, self.measurement)
 
+
+    def __mod__(self, other):
+        match self.measurement:
+            case 'fahrenheit':
+                quotient = self.value % other.to_fahrenheit().value
+            case 'celsius':
+                quotient = self.value % other.to_celsius().value
+            case 'kelvin':
+                quotient = self.value % other.to_kelvin().value
+        return Temperature(quotient, self.measurement)
+
+
     def to_fahrenheit(self):
         '''Convert the temperature to Fahrenheit'''
         match self.measurement:
             case 'fahrenheit':
                 return self
             case 'celsius':
                 return Temperature((self.value * 9.0 / 5.0) + 32.0)
             case 'kelvin':
                 return Temperature((self.value - 273.15) * (9.0 / 5.0) + 32)
 
+
     def to_celsius(self):
         '''Convert the temperature to Celsius'''
         measure = 'celsius'
         match self.measurement:
             case 'celsius':
                 return self
             case 'fahrenheit':
                 return Temperature(((self.value - 32.0) * 5.0 / 9.0), measure)
             case 'kelvin':
                 return Temperature((self.value - 273.15), measure)
 
+
     def to_kelvin(self):
         '''Convert the temperature to Kelvin'''
         measure = 'kelvin'
         match self.measurement:
             case 'kelvin':
                 return self
             case 'fahrenheit':
                 return Temperature(((self.value - 32.0) * (5.0 / 9.0) + 273.15), measure)
             case 'celsius':
                 return Temperature((self.value + 273.15), measure)
 
+
 ABSOLUTE_ZERO = Temperature(0, measurement='kelvin')
 FREEZING_POINT = Temperature(0, measurement='celsius')
 BOILING_POINT = Temperature(100, measurement='celsius')
```

### Comparing `measuring-tools-0.4.1/measuring_tools/volume.py` & `measuring-tools-0.5.0/measuring_tools/volume.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,156 +1,168 @@
 '''Functionality for volume conversion and volume equality checks.
-Values of two different temperatures recorded in different measurements are considered equal
-if the converted values within a relative tolerance or absolute tolerance of float_point_tol.
-The default for float_point_tol is 1e-05.
+Values of two different volumes recorded in different measurements are considered equal
+if the converted values within a relative tolerance or absolute tolerance of FLOAT_POINT_TOL.
+The default for FLOAT_POINT_TOL is 1e-05.
 '''
 
+
+import functools
 from math import isclose, floor, ceil
 from measuring_tools import Measurement
 
+
 def __dir__():
     return ('Volume', '__doc__', '__file__', '__loader__', '__name__', '__package__', '__spec__')
 
+
+@functools.total_ordering
 class Volume(Measurement):
-    '''Volume class comparing and converting Metric, British Imperial Units, and US Units'''
+    '''Volume class comparing and converting Metric, British Imperial Units, and US Units
+    * value is expected to be either an integer or a float
+    * measurement can be one of three options (defaults to liter):
+        - liter
+        - gallon
+        - gallon_us
+    '''
+
 
     def __init__(self, value: int | float, measurement: str='liter'):
         if not measurement in ('liter', 'gallon', 'gallon_us'):
             raise ValueError('Value must be liter, gallon, gallon_us')
         super().__init__(value, measurement)
 
+
     def __round__(self, ndigits):
         return Volume(round(self.value, ndigits=ndigits), self.measurement)
 
+
     def __abs__(self):
         return Volume(abs(self.value), self.measurement)
 
+
     def __floor__(self):
         return Volume(floor(self.value), self.measurement)
 
+
     def __ceil__(self):
         return Volume(ceil(self.value), self.measurement)
 
+
     def __eq__(self, other):
         match self.measurement:
             case 'liter':
-                return isclose(self.value, other.to_liter().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
+                return isclose(self.value, other.to_liter().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'gallon':
-                return isclose(self.value, other.to_gallon().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
+                return isclose(self.value, other.to_gallon().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
             case 'gallon_us':
-                return isclose(self.value, other.to_gallon_us().value, rel_tol=self.float_point_tol, abs_tol=self.float_point_tol)
+                return isclose(self.value, other.to_gallon_us().value, rel_tol=self.FLOAT_POINT_TOL, abs_tol=self.FLOAT_POINT_TOL)
 
-    def __ne__(self, other):
-        match self.measurement:
-            case 'liter':
-                return not self.value == other.to_liter().value
-            case 'gallon':
-                return not self.value == other.to_gallon().value
-            case 'gallon_us':
-                return not self.value == other.to_gallon_us().value
 
     def __lt__(self, other):
         if self == other:
             return False
         match self.measurement:
             case 'liter':
                 return self.value < other.to_liter().value
             case 'gallon':
                 return self.value < other.to_gallon().value
             case 'gallon_us':
                 return self.value < other.to_gallon_us().value
 
-    def __le__(self, other):
-        return self == other or self < other
-
-    def __gt__(self, other):
-        if self == other: return False
-        match self.measurement:
-            case 'liter':
-                return self.value > other.to_liter().value
-            case 'gallon':
-                return self.value > other.to_gallon().value
-            case 'gallon_us':
-                return self.value > other.to_gallon_us().value
-
-    def __ge__(self, other):
-        return self == other or self > other
 
     def __add__(self, other):
         match self.measurement:
             case 'liter':
                 total = self.value + other.to_liter().value
             case 'gallon':
                 total = self.value + other.to_gallon().value
             case 'gallon_us':
                 total = self.value + other.to_gallon_us().value
         return Volume(total, self.measurement)
 
+
     def __sub__(self, other):
         match self.measurement:
             case 'liter':
                 diff = self.value - other.to_liter().value
             case 'gallon':
                 diff = self.value - other.to_gallon().value
             case 'gallon_us':
                 diff = self.value - other.to_gallon_us().value
         return Volume(diff, self.measurement)
 
+
     def __mul__(self, other):
         match self.measurement:
             case 'liter':
                 product = self.value * other.to_liter().value
             case 'gallon':
                 product = self.value * other.to_gallon().value
             case 'gallon_us':
                 product = self.value * other.to_gallon_us().value
         return Volume(product, self.measurement)
 
+
     def __truediv__(self, other):
         match self.measurement:
             case 'liter':
                 result = self.value / other.to_liter().value
             case 'gallon':
                 result = self.value / other.to_gallon().value
             case 'gallon_us':
                 result = self.value / other.to_gallon_us().value
         return Volume(result, self.measurement)
 
+
     def __floordiv__(self, other):
         match self.measurement:
             case 'liter':
                 result = self.value // other.to_liter().value
             case 'gallon':
                 result = self.value // other.to_gallon().value
             case 'gallon_us':
                 result = self.value // other.to_gallon_us().value
         return Volume(result, self.measurement)
 
+
+    def __mod__(self, other):
+        match self.measurement:
+            case 'liter':
+                result = self.value % other.to_liter().value
+            case 'gallon':
+                result = self.value % other.to_gallon().value
+            case 'gallon_us':
+                result = self.value % other.to_gallon_us().value
+        return Volume(result, self.measurement)
+
+
     def to_liter(self):
         '''Convert the volume to liter'''
         measure = 'liter'
         match self.measurement:
             case 'liter':
                 return self
             case 'gallon':
                 return Volume((self.value * 4.54609513), measurement=measure)
             case 'gallon_us':
                 return Volume((self.value * 3.78541178), measurement=measure)
 
+
     def to_gallon(self):
         '''Convert the volume to British Imperial Gallons'''
         measure = 'gallon'
         match self.measurement:
             case 'gallon':
                 return self
             case 'liter':
                 return Volume((self.value * 0.219969157), measurement=measure)
             case 'gallon_us':
                 return Volume((self.value * 0.8326741846), measurement=measure)
 
+
     def to_gallon_us(self):
         '''Convert the volume to US Gallons'''
         measure = 'gallon_us'
         match self.measurement:
             case 'gallon_us':
                 return self
             case 'liter':
```

### Comparing `measuring-tools-0.4.1/measuring_tools.egg-info/PKG-INFO` & `measuring-tools-0.5.0/measuring_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: measuring-tools
-Version: 0.4.1
+Version: 0.5.0
 Summary: Classes to help with common types of measurements
 Home-page: https://bitbucket.org/blacklotus231/measuring-tools
 Author: James Baker Jr
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `measuring-tools-0.4.1/setup.py` & `measuring-tools-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='measuring-tools',
-    version='0.4.1',
+    version='0.5.0',
     description='Classes to help with common types of measurements',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/blacklotus231/measuring-tools',
     author='James Baker Jr',
     license='Apache License 2.0',
     python_requires='>=3.10',
```

