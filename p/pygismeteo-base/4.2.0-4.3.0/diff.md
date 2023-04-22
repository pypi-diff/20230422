# Comparing `tmp/pygismeteo_base-4.2.0.tar.gz` & `tmp/pygismeteo_base-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygismeteo_base-4.2.0.tar", max compression
+gzip compressed data, was "pygismeteo_base-4.3.0.tar", max compression
```

## Comparing `pygismeteo_base-4.2.0.tar` & `pygismeteo_base-4.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/LICENSE
--rw-r--r--   0        0        0      553 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/README.md
--rw-r--r--   0        0        0       86 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/__init__.py
--rw-r--r--   0        0        0       92 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/constants.py
--rw-r--r--   0        0        0      925 2023-04-21 19:11:10.073668 pygismeteo_base-4.2.0/pygismeteo_base/current.py
--rw-r--r--   0        0        0      392 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/endpoint.py
--rw-r--r--   0        0        0      901 2023-04-21 19:29:03.763651 pygismeteo_base-4.2.0/pygismeteo_base/http.py
--rw-r--r--   0        0        0      309 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/__init__.py
--rw-r--r--   0        0        0     1812 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/current.py
--rw-r--r--   0        0        0      759 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_coordinates.py
--rw-r--r--   0        0        0      673 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_ip.py
--rw-r--r--   0        0        0      783 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_query.py
--rw-r--r--   0        0        0     2908 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/step24.py
--rw-r--r--   0        0        0     1786 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/step3.py
--rw-r--r--   0        0        0     1803 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/models/step6.py
--rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/py.typed
--rw-r--r--   0        0        0     1149 2023-04-21 19:25:53.063683 pygismeteo_base-4.2.0/pygismeteo_base/search.py
--rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/step_n/__init__.py
--rw-r--r--   0        0        0     1433 2023-04-21 19:08:58.453658 pygismeteo_base-4.2.0/pygismeteo_base/step_n/abc.py
--rw-r--r--   0        0        0     1604 2023-04-20 07:24:32.670114 pygismeteo_base-4.2.0/pygismeteo_base/step_n/mixins.py
--rw-r--r--   0        0        0     1217 2023-04-21 19:39:40.203642 pygismeteo_base-4.2.0/pygismeteo_base/types.py
--rw-r--r--   0        0        0      400 2023-04-21 18:50:04.713658 pygismeteo_base-4.2.0/pygismeteo_base/typing_compat.py
--rw-r--r--   0        0        0      815 2023-04-21 18:44:17.243666 pygismeteo_base-4.2.0/pygismeteo_base/validators.py
--rw-r--r--   0        0        0     2706 2023-04-21 19:43:49.973683 pygismeteo_base-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 pygismeteo_base-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/LICENSE
+-rw-r--r--   0        0        0      553 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/README.md
+-rw-r--r--   0        0        0       86 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/__init__.py
+-rw-r--r--   0        0        0       92 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/constants.py
+-rw-r--r--   0        0        0      925 2023-04-21 19:11:10.073668 pygismeteo_base-4.3.0/pygismeteo_base/current.py
+-rw-r--r--   0        0        0      392 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/endpoint.py
+-rw-r--r--   0        0        0      901 2023-04-21 19:29:03.763651 pygismeteo_base-4.3.0/pygismeteo_base/http.py
+-rw-r--r--   0        0        0      309 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/models/__init__.py
+-rw-r--r--   0        0        0     1812 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/models/current.py
+-rw-r--r--   0        0        0      759 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/models/search_by_coordinates.py
+-rw-r--r--   0        0        0      673 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/models/search_by_ip.py
+-rw-r--r--   0        0        0      783 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/models/search_by_query.py
+-rw-r--r--   0        0        0     2908 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/models/step24.py
+-rw-r--r--   0        0        0     1786 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/models/step3.py
+-rw-r--r--   0        0        0     1803 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/models/step6.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/py.typed
+-rw-r--r--   0        0        0     1149 2023-04-21 19:25:53.063683 pygismeteo_base-4.3.0/pygismeteo_base/search.py
+-rw-r--r--   0        0        0        0 2023-04-20 07:24:32.670114 pygismeteo_base-4.3.0/pygismeteo_base/step_n/__init__.py
+-rw-r--r--   0        0        0     1452 2023-04-21 19:55:58.533667 pygismeteo_base-4.3.0/pygismeteo_base/step_n/abc.py
+-rw-r--r--   0        0        0     1609 2023-04-21 19:56:30.993669 pygismeteo_base-4.3.0/pygismeteo_base/step_n/mixins.py
+-rw-r--r--   0        0        0     1308 2023-04-21 19:55:05.883666 pygismeteo_base-4.3.0/pygismeteo_base/types.py
+-rw-r--r--   0        0        0      400 2023-04-21 18:50:04.713658 pygismeteo_base-4.3.0/pygismeteo_base/typing_compat.py
+-rw-r--r--   0        0        0      870 2023-04-21 19:55:32.463666 pygismeteo_base-4.3.0/pygismeteo_base/validators.py
+-rw-r--r--   0        0        0     2706 2023-04-21 19:58:09.733671 pygismeteo_base-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 pygismeteo_base-4.3.0/PKG-INFO
```

### Comparing `pygismeteo_base-4.2.0/LICENSE` & `pygismeteo_base-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/README.md` & `pygismeteo_base-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/current.py` & `pygismeteo_base-4.3.0/pygismeteo_base/current.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/http.py` & `pygismeteo_base-4.3.0/pygismeteo_base/http.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/models/current.py` & `pygismeteo_base-4.3.0/pygismeteo_base/models/current.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_coordinates.py` & `pygismeteo_base-4.3.0/pygismeteo_base/models/search_by_coordinates.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_ip.py` & `pygismeteo_base-4.3.0/pygismeteo_base/models/search_by_ip.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/models/search_by_query.py` & `pygismeteo_base-4.3.0/pygismeteo_base/models/search_by_query.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/models/step24.py` & `pygismeteo_base-4.3.0/pygismeteo_base/models/step24.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/models/step3.py` & `pygismeteo_base-4.3.0/pygismeteo_base/models/step3.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/models/step6.py` & `pygismeteo_base-4.3.0/pygismeteo_base/models/step6.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/search.py` & `pygismeteo_base-4.3.0/pygismeteo_base/search.py`

 * *Files identical despite different names*

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/step_n/abc.py` & `pygismeteo_base-4.3.0/pygismeteo_base/step_n/abc.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def _model(self) -> types.StepNModel:
         pass
 
     @property
     @abstractmethod
     def _days_validator(
         self,
-    ) -> Type[Union[validators.Step3Days, validators.Step6or24Days]]:
+    ) -> Type[Union[validators.Step3Days, validators.Step6Days, validators.Step24Days]]:
         pass
 
     def _get_params_by_coordinates(
         self, latitude: float, longitude: float, *, days: types.StepNDays
     ) -> Tuple[str, types.Params]:
         coords_validator = validators.Coordinates(
             latitude=latitude, longitude=longitude
```

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/step_n/mixins.py` & `pygismeteo_base-4.3.0/pygismeteo_base/step_n/mixins.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def _model(self) -> types.StepNModel:
         pass
 
     @property
     @abstractmethod
     def _days_validator(
         self,
-    ) -> Type[Union[validators.Step3Days, validators.Step6or24Days]]:
+    ) -> Type[Union[validators.Step3Days, validators.Step6Days, validators.Step24Days]]:
         pass
 
 
 class Step3Mixin(StepNMixin):
     __slots__ = ()
 
     @property
@@ -51,25 +51,25 @@
         return "weather/forecast/by_day_part"
 
     @property
     def _model(self) -> Type[models.step6.Model]:
         return models.step6.Model
 
     @property
-    def _days_validator(self) -> Type[validators.Step6or24Days]:
-        return validators.Step6or24Days
+    def _days_validator(self) -> Type[validators.Step6Days]:
+        return validators.Step6Days
 
 
 class Step24Mixin(StepNMixin):
     __slots__ = ()
 
     @property
     def _endpoint(self) -> str:
         return "weather/forecast/aggregate"
 
     @property
     def _model(self) -> Type[models.step24.Model]:
         return models.step24.Model
 
     @property
-    def _days_validator(self) -> Type[validators.Step6or24Days]:
-        return validators.Step6or24Days
+    def _days_validator(self) -> Type[validators.Step24Days]:
+        return validators.Step24Days
```

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/types.py` & `pygismeteo_base-4.3.0/pygismeteo_base/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from . import models
 from .typing_compat import Literal, TypeAlias
 
 Lang: TypeAlias = Literal["ru", "en", "ua", "lt", "lv", "pl", "ro"]
 Step3Days: TypeAlias = Literal[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
 Step6or24Days: TypeAlias = Literal[3, 4, 5, 6, 7, 8, 9, 10]
-StepNDays: TypeAlias = Union[Step3Days, Step6or24Days]
+Step6Days: TypeAlias = Step6or24Days
+Step24Days: TypeAlias = Step6or24Days
+StepNDays: TypeAlias = Union[Step3Days, Step6Days, Step24Days]
 Params: TypeAlias = Optional[Mapping[str, str]]
 Headers: TypeAlias = Optional[Mapping[str, str]]
 SearchLimit: TypeAlias = Literal[
     1,
     2,
     3,
     4,
@@ -49,15 +51,15 @@
     35,
     36,
 ]
 
 StepNModel: TypeAlias = Type[
     Union[models.step3.Model, models.step6.Model, models.step24.Model]
 ]
-TDays = TypeVar("TDays", Step3Days, Step6or24Days)
+TDays = TypeVar("TDays", Step3Days, Step6Days, Step24Days)
 TStepNModel = TypeVar(
     "TStepNModel", models.step3.Model, models.step6.Model, models.step24.Model
 )
 TStepNModelItem = TypeVar(
     "TStepNModelItem",
     models.step3.ModelItem,
     models.step6.ModelItem,
```

### Comparing `pygismeteo_base-4.2.0/pygismeteo_base/validators.py` & `pygismeteo_base-4.3.0/pygismeteo_base/validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,7 +36,11 @@
 
 class Step3Days(BaseModel):
     __root__: int = Field(ge=1, le=10)
 
 
 class Step6or24Days(BaseModel):
     __root__: int = Field(ge=3, le=10)
+
+
+Step6Days = Step6or24Days
+Step24Days = Step6or24Days
```

### Comparing `pygismeteo_base-4.2.0/pyproject.toml` & `pygismeteo_base-4.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygismeteo-base"
-version = "4.2.0"
+version = "4.3.0"
 description = "Base for pygismeteo and aiopygismeteo"
 authors = ["monosans <hsyqixco@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/monosans/pygismeteo-base"
 classifiers = [
     "Environment :: Web Environment",
```

### Comparing `pygismeteo_base-4.2.0/PKG-INFO` & `pygismeteo_base-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygismeteo-base
-Version: 4.2.0
+Version: 4.3.0
 Summary: Base for pygismeteo and aiopygismeteo
 Home-page: https://github.com/monosans/pygismeteo-base
 License: MIT
 Author: monosans
 Author-email: hsyqixco@protonmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
```

