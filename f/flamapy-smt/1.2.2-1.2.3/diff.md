# Comparing `tmp/flamapy-smt-1.2.2.tar.gz` & `tmp/flamapy-smt-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-smt-1.2.2.tar", last modified: Thu Mar  2 00:15:09 2023, max compression
+gzip compressed data, was "flamapy-smt-1.2.3.tar", last modified: Sat Apr 22 14:43:15 2023, max compression
```

## Comparing `flamapy-smt-1.2.2.tar` & `flamapy-smt-1.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:15:09.725707 flamapy-smt-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-02 00:15:09.725707 flamapy-smt-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:15:09.717707 flamapy-smt-1.2.2/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:15:09.717707 flamapy-smt-1.2.2/flamapy/metamodels/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:15:09.721707 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:15:09.721707 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/models/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/models/pysmt_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:15:09.721707 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/complete_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/config_by_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/filter_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/maximize_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/minimize_impact.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/number_of_products.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/valid_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/valid_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:15:09.721707 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/transformations/network_to_smt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:15:09.721707 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/utils/config_sanitizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 00:15:09.725707 flamapy-smt-1.2.2/flamapy_smt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-03-02 00:15:09.000000 flamapy-smt-1.2.2/flamapy_smt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-02 00:15:09.000000 flamapy-smt-1.2.2/flamapy_smt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 00:15:09.000000 flamapy-smt-1.2.2/flamapy_smt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-02 00:15:09.000000 flamapy-smt-1.2.2/flamapy_smt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-02 00:15:09.000000 flamapy-smt-1.2.2/flamapy_smt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 00:15:09.725707 flamapy-smt-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-02 00:14:52.000000 flamapy-smt-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.315339 flamapy-smt-1.2.3/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.315339 flamapy-smt-1.2.3/flamapy/metamodels/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.315339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.315339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/models/pysmt_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/complete_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/config_by_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/filter_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/maximize_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/minimize_impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/number_of_products.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/valid_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/valid_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/transformations/graph_to_smt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/utils/config_sanitizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/flamapy_smt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-22 14:43:15.000000 flamapy-smt-1.2.3/flamapy_smt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 14:43:15.319339 flamapy-smt-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-22 14:43:03.000000 flamapy-smt-1.2.3/setup.py
```

### Comparing `flamapy-smt-1.2.2/LICENSE.md` & `flamapy-smt-1.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.2/PKG-INFO` & `flamapy-smt-1.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-smt
-Version: 1.2.2
+Version: 1.2.3
 Summary: This repo host the SMT model concrete classes
 Home-page: https://github.com/flamapy/smt_metamodel
 Author: Antonio Germán Márquez Trujillo
 Author-email: amtrujillo@us.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/__init__.py` & `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/complete_config.py` & `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/config_by_impact.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-from z3 import Int, sat, Optimize
+from z3 import sat, Optimize, Abs
 
 from flamapy.core.operations import Operation
 from flamapy.metamodels.smt_metamodel.models import PySMTModel
 from flamapy.metamodels.smt_metamodel.utils import config_sanitizer
 
 
-class CompleteConfig(Operation):
+class ConfigByImpact(Operation):
 
     def __init__(
         self,
-        file_name: str,
-        config: dict[str, int]
+        impact: float
     ) -> None:
-        self.file_name: str = file_name
-        self.config: dict[str, int] = config
-        self.result: dict[str, float | int] = {}
+        self.impact: float = impact
+        self.result: list[dict[str, float | int]] = []
 
-    def get_result(self) -> dict[str, float | int]:
+    def get_result(self) -> list[dict[str, float | int]]:
         return self.result
 
     def execute(self, model: PySMTModel) -> None:
         solver = Optimize()
-        if model.cvvs:
-            cvss_f = model.cvvs[self.file_name]
-            solver.minimize(cvss_f)
+        if model.func_obj_var is not None:
+            cvss_f = model.func_obj_var
+            obj = Abs(cvss_f - self.impact)
+            solver.minimize(obj)
 
-        formula = model.domains[self.file_name]
+        formula = model.domain
         solver.add(formula)
-        for package, count in self.config.items():
-            solver.add(Int(package) == count)
-
         while solver.check() == sat:
             config = solver.model()
             sanitized_config = config_sanitizer(config)
-            self.result = sanitized_config
+            self.result.append(sanitized_config)
             break
```

### Comparing `flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/config_by_impact.py` & `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/maximize_impact.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-from z3 import sat, Optimize, Abs
+from z3 import Or, Optimize, sat
 
 from flamapy.core.operations import Operation
 from flamapy.metamodels.smt_metamodel.models import PySMTModel
 from flamapy.metamodels.smt_metamodel.utils import config_sanitizer
 
 
-class ConfigByImpact(Operation):
+class MaximizeImpact(Operation):
 
     def __init__(
         self,
-        file_name: str,
-        impact: float
+        limit: int
     ) -> None:
-        self.file_name: str = file_name
-        self.impact: float = impact
-        self.result: dict[str, float | int] = {}
+        self.limit: int = limit
+        self.result: list[dict[str, float | int]] = []
 
-    def get_result(self) -> dict[str, float | int]:
+    def get_result(self) -> list[dict[str, float | int]]:
         return self.result
 
     def execute(self, model: PySMTModel) -> None:
         solver = Optimize()
-        if model.cvvs:
-            cvss_f = model.cvvs[self.file_name]
-            obj = Abs(cvss_f - self.impact)
-            solver.minimize(obj)
+        if model.func_obj_var is not None:
+            cvss_f = model.func_obj_var
+            solver.maximize(cvss_f)
 
-        formula = model.domains[self.file_name]
+        formula = model.domain
         solver.add(formula)
-        while solver.check() == sat:
+        while len(self.result) < self.limit and solver.check() == sat:
             config = solver.model()
             sanitized_config = config_sanitizer(config)
-            self.result = sanitized_config
-            break
+            self.result.append(sanitized_config)
+
+            block = []
+            for var in config:
+                if str(var) != '/0':
+                    variable = var()
+                    if 'CVSS' not in str(variable):
+                        block.append(config[var] != variable)
+
+            solver.add(Or(block))
```

### Comparing `flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/filter_configs.py` & `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/filter_configs.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,36 +5,34 @@
 from flamapy.metamodels.smt_metamodel.utils import config_sanitizer
 
 
 class FilterConfigs(Operation):
 
     def __init__(
         self,
-        file_name: str,
         max_threshold: float,
         min_threshold: float,
         limit: int
     ) -> None:
-        self.file_name: str = file_name
         self.max_threshold: float = max_threshold
         self.min_threshold: float = min_threshold
         self.limit: int = limit
         self.result: list[dict[str, float | int]] = []
 
     def get_result(self) -> list[dict[str, float | int]]:
         return self.result
 
     def execute(self, model: PySMTModel) -> None:
-        if model.cvvs:
-            cvss_f = model.cvvs[self.file_name]
+        if model.func_obj_var is not None:
+            cvss_f = model.func_obj_var
             max_ctc = cvss_f <= self.max_threshold
             min_ctc = cvss_f >= self.min_threshold
 
         solver = Solver()
-        formula = And([model.domains[self.file_name], max_ctc, min_ctc])
+        formula = And([model.domain, max_ctc, min_ctc])
         solver.add(formula)
         while len(self.result) < self.limit and solver.check() == sat:
             config = solver.model()
             sanitized_config = config_sanitizer(config)
             self.result.append(sanitized_config)
 
             block = []
```

### Comparing `flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/maximize_impact.py` & `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/minimize_impact.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 from z3 import Or, Optimize, sat
 
 from flamapy.core.operations import Operation
 from flamapy.metamodels.smt_metamodel.models import PySMTModel
 from flamapy.metamodels.smt_metamodel.utils import config_sanitizer
 
 
-class MaximizeImpact(Operation):
+class MinimizeImpact(Operation):
 
     def __init__(
         self,
-        file_name: str,
         limit: int
     ) -> None:
-        self.file_name: str = file_name
         self.limit: int = limit
         self.result: list[dict[str, float | int]] = []
 
     def get_result(self) -> list[dict[str, float | int]]:
         return self.result
 
     def execute(self, model: PySMTModel) -> None:
         solver = Optimize()
-        if model.cvvs:
-            cvss_f = model.cvvs[self.file_name]
-            solver.maximize(cvss_f)
+        if model.func_obj_var is not None:
+            cvss_f = model.func_obj_var
+            solver.minimize(cvss_f)
 
-        formula = model.domains[self.file_name]
+        formula = model.domain
         solver.add(formula)
         while len(self.result) < self.limit and solver.check() == sat:
             config = solver.model()
             sanitized_config = config_sanitizer(config)
             self.result.append(sanitized_config)
 
             block = []
```

### Comparing `flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/minimize_impact.py` & `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/complete_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-from z3 import Or, Optimize, sat
+from z3 import Int, sat, Optimize
 
 from flamapy.core.operations import Operation
 from flamapy.metamodels.smt_metamodel.models import PySMTModel
 from flamapy.metamodels.smt_metamodel.utils import config_sanitizer
 
 
-class MinimizeImpact(Operation):
+class CompleteConfig(Operation):
 
     def __init__(
         self,
-        file_name: str,
-        limit: int
+        config: dict[str, int]
     ) -> None:
-        self.limit: int = limit
+        self.config: dict[str, int] = config
         self.result: list[dict[str, float | int]] = []
-        self.file_name: str = file_name
 
     def get_result(self) -> list[dict[str, float | int]]:
         return self.result
 
     def execute(self, model: PySMTModel) -> None:
         solver = Optimize()
-        if model.cvvs:
-            cvss_f = model.cvvs[self.file_name]
+        if model.func_obj_var is not None:
+            cvss_f = model.func_obj_var
             solver.minimize(cvss_f)
 
-        formula = model.domains[self.file_name]
+        formula = model.domain
         solver.add(formula)
-        while len(self.result) < self.limit and solver.check() == sat:
+        for package, count in self.config.items():
+            solver.add(Int(package) == count)
+
+        while solver.check() == sat:
             config = solver.model()
             sanitized_config = config_sanitizer(config)
             self.result.append(sanitized_config)
-
-            block = []
-            for var in config:
-                if str(var) != '/0':
-                    variable = var()
-                    if 'CVSS' not in str(variable):
-                        block.append(config[var] != variable)
-
-            solver.add(Or(block))
+            break
```

### Comparing `flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/number_of_products.py` & `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/number_of_products.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 
 from flamapy.core.operations import Operation
 from flamapy.metamodels.smt_metamodel.models import PySMTModel
 
 
 class NumberOfProducts(Operation):
 
-    def __init__(self, file_name: str) -> None:
-        self.file_name: str = file_name
+    def __init__(self) -> None:
         self.result: int = 0
 
     def get_result(self) -> int:
         return self.result
 
     def execute(self, model: PySMTModel) -> None:
-        formula = model.domains[self.file_name]
+        formula = model.domain
         solver = Solver()
         solver.add(formula)
         while solver.check() == sat:
             config = solver.model()
 
             block = []
             for var in config:
```

### Comparing `flamapy-smt-1.2.2/flamapy/metamodels/smt_metamodel/operations/valid_config.py` & `flamapy-smt-1.2.3/flamapy/metamodels/smt_metamodel/operations/valid_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,22 @@
 from flamapy.metamodels.smt_metamodel.models import PySMTModel
 
 
 class ValidConfig(Operation):
 
     def __init__(
         self,
-        file_name: str,
         config: dict[str, int]
     ) -> None:
-        self.file_name: str = file_name
         self.config: dict[str, int] = config
         self.result: bool = True
 
     def get_result(self) -> bool:
         return self.result
 
     def execute(self, model: PySMTModel) -> None:
-        formula = model.domains[self.file_name]
+        formula = model.domain
         solver = Solver()
         solver.add(formula)
         for package, count in self.config.items():
             solver.add(Int(package) == count)
         self.result = solver.check() == sat
```

### Comparing `flamapy-smt-1.2.2/flamapy_smt.egg-info/PKG-INFO` & `flamapy-smt-1.2.3/flamapy_smt.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flamapy-smt
-Version: 1.2.2
+Version: 1.2.3
 Summary: This repo host the SMT model concrete classes
 Home-page: https://github.com/flamapy/smt_metamodel
 Author: Antonio Germán Márquez Trujillo
 Author-email: amtrujillo@us.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `flamapy-smt-1.2.2/flamapy_smt.egg-info/SOURCES.txt` & `flamapy-smt-1.2.3/flamapy_smt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 flamapy/metamodels/smt_metamodel/operations/filter_configs.py
 flamapy/metamodels/smt_metamodel/operations/maximize_impact.py
 flamapy/metamodels/smt_metamodel/operations/minimize_impact.py
 flamapy/metamodels/smt_metamodel/operations/number_of_products.py
 flamapy/metamodels/smt_metamodel/operations/valid_config.py
 flamapy/metamodels/smt_metamodel/operations/valid_model.py
 flamapy/metamodels/smt_metamodel/transformations/__init__.py
-flamapy/metamodels/smt_metamodel/transformations/network_to_smt.py
+flamapy/metamodels/smt_metamodel/transformations/graph_to_smt.py
 flamapy/metamodels/smt_metamodel/utils/__init__.py
 flamapy/metamodels/smt_metamodel/utils/config_sanitizer.py
 flamapy_smt.egg-info/PKG-INFO
 flamapy_smt.egg-info/SOURCES.txt
 flamapy_smt.egg-info/dependency_links.txt
 flamapy_smt.egg-info/requires.txt
 flamapy_smt.egg-info/top_level.txt
```

### Comparing `flamapy-smt-1.2.2/setup.py` & `flamapy-smt-1.2.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='flamapy-smt',
-    version='1.2.2',
+    version='1.2.3',
     author='Antonio Germán Márquez Trujillo',
     author_email='amtrujillo@us.es',
     description='This repo host the SMT model concrete classes',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/flamapy/smt_metamodel',
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: OS Independent'
     ],
     python_requires='>=3.10',
     install_requires=[
-        'z3-solver==4.11.2.0',
-        'flamapy==1.0.1',
-        'flamapy-dn==1.1.6'
+        'z3-solver==4.12.1.0',
+        'flamapy==1.0.1'
     ],
     tests_requires=[
         'prospector[with_everything]==1.8.3',
         'mypy==0.982',
-        'types-setuptools==65.4.0'
+        'types-setuptools==67.6.0.8'
     ]
 )
```

