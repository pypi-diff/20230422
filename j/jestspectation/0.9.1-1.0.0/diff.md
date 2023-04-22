# Comparing `tmp/Jestspectation-0.9.1.tar.gz` & `tmp/jestspectation-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jestspectation-0.9.1.tar", last modified: Wed Mar  1 05:03:09 2023, max compression
+gzip compressed data, was "jestspectation-1.0.0.tar", max compression
```

## Comparing `Jestspectation-0.9.1.tar` & `jestspectation-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 05:03:09.331910 Jestspectation-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 05:03:09.331910 Jestspectation-0.9.1/Jestspectation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-01 05:03:09.000000 Jestspectation-0.9.1/Jestspectation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-01 05:03:09.000000 Jestspectation-0.9.1/Jestspectation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 05:03:09.000000 Jestspectation-0.9.1/Jestspectation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-01 05:03:09.000000 Jestspectation-0.9.1/Jestspectation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-01 05:03:09.331910 Jestspectation-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 05:03:09.331910 Jestspectation-0.9.1/jestspectation/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__any.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 05:03:09.331910 Jestspectation-0.9.1/jestspectation/__config/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__config/__config.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__equals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__float_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__jestspectation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__py_diffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 05:03:09.331910 Jestspectation-0.9.1/jestspectation/__strings/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__strings/__containing.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__strings/__lines_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__strings/__matching_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__strings/__text_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/__util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 05:03:09.331910 Jestspectation-0.9.1/jestspectation/logicals/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/logicals/__and.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/logicals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/logicals/__not.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/logicals/__or.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/logicals/__xor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/jestspectation/pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-01 05:02:53.000000 Jestspectation-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-01 05:03:09.331910 Jestspectation-0.9.1/setup.cfg
+-rw-r--r--   0        0        0     1073 2023-04-22 18:13:30.788580 jestspectation-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1421 2023-04-22 18:13:30.788580 jestspectation-1.0.0/README.md
+-rw-r--r--   0        0        0     1455 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__any.py
+-rw-r--r--   0        0        0      609 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__config/__config.py
+-rw-r--r--   0        0        0      105 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__config/__init__.py
+-rw-r--r--   0        0        0    10767 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__containers.py
+-rw-r--r--   0        0        0     2451 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__equals.py
+-rw-r--r--   0        0        0     3613 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__float_approx.py
+-rw-r--r--   0        0        0      993 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__init__.py
+-rw-r--r--   0        0        0     2610 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__jestspectation_base.py
+-rw-r--r--   0        0        0     2861 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__py_diffs.py
+-rw-r--r--   0        0        0     1304 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__containing.py
+-rw-r--r--   0        0        0      292 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__init__.py
+-rw-r--r--   0        0        0     4741 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__lines_like.py
+-rw-r--r--   0        0        0     1360 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__matching_regex.py
+-rw-r--r--   0        0        0     2547 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__strings/__text_like.py
+-rw-r--r--   0        0        0     3699 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/__util.py
+-rw-r--r--   0        0        0     1670 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__and.py
+-rw-r--r--   0        0        0      242 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__init__.py
+-rw-r--r--   0        0        0     1279 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__not.py
+-rw-r--r--   0        0        0     1612 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__or.py
+-rw-r--r--   0        0        0     2162 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/logicals/__xor.py
+-rw-r--r--   0        0        0        0 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/py.typed
+-rw-r--r--   0        0        0      719 2023-04-22 18:13:30.788580 jestspectation-1.0.0/jestspectation/pytest.py
+-rw-r--r--   0        0        0     1408 2023-04-22 18:13:30.788580 jestspectation-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 jestspectation-1.0.0/PKG-INFO
```

### Comparing `Jestspectation-0.9.1/Jestspectation.egg-info/PKG-INFO` & `jestspectation-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
-Name: Jestspectation
-Version: 0.9.1
-Summary: Pattern matching helper classes designed to allow for testing of complex data structures in a readable and logical format.
+Name: jestspectation
+Version: 1.0.0
+Summary: Pattern matching helper classes designed to allow for testing of complex data structures in a readable and logical format
 Home-page: https://github.com/MiguelGuthridge/Jestspectation
+License: MIT
+Keywords: jest,pattern,matching,pytest,equality
 Author: Miguel Guthridge
 Author-email: hdsq@outlook.com.au
-Project-URL: Online Documentation, https://github.com/MiguelGuthridge/Jestspectation
-Project-URL: Bug Tracker, https://github.com/MiguelGuthridge/Jestspectation/issues
-Keywords: jest,pattern,matching,pytest,equality
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Framework :: Pytest
-Requires-Python: >=3.9.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
+Project-URL: Bug Tracker, https://github.com/MiguelGuthridge/Jestspectation/issues
+Project-URL: Documentation, https://miguelguthridge.github.io/Jestspectation
+Project-URL: Online Documentation, https://github.com/MiguelGuthridge/Jestspectation
+Project-URL: Repository, https://github.com/MiguelGuthridge/Jestspectation
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Jestspectation
 
 Pattern matching helper classes designed to allow for testing of complex data
 structures in a readable and logical format.
 
 The design is inspired by the `expect` system from JavaScript's Jest testing
@@ -48,34 +55,28 @@
 ```
 
 ## Usage with Pytest
 
 The library can be used as a pytest plugin, which can give access to much more
 detailed error messages when assertions fail.
 
-You can enable it by adding the following lines to your `conftest.py`
-
-```py
-pytest_plugins = ("jestspectation.pytest",)
-```
-
 This should result in output similar to the following
 
-```
+```txt
     def test_goodbye():
 >       assert 1 == expect.Any(float)
 E       assert Type mismatch
 E         Expected any object of type float
 E         Received 1 (int)
 ```
 
 These advanced completions can also be used for most standard Python objects
 by wrapping the expected values in an `Equals`. For example:
 
-```
+```txt
     def test_lists():
 >       assert expect.Equals([1, 2, 3, 4]) == [1, 2, 3, 5, 6]
 E       assert [1, 2, 3, 4] == [1, 2, 3, 5, 6]
 E         !! [3] 4 == 5
 E            Value mismatch
 E            Expected 4
 E            Received 5
@@ -86,7 +87,8 @@
 Jestspectation.
 
 ```py
 import jestspectation
 
 jestspectation.configure().pytest_all_diffs = True
 ```
+
```

### Comparing `Jestspectation-0.9.1/LICENSE` & `jestspectation-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/PKG-INFO` & `jestspectation-1.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: Jestspectation
-Version: 0.9.1
-Summary: Pattern matching helper classes designed to allow for testing of complex data structures in a readable and logical format.
-Home-page: https://github.com/MiguelGuthridge/Jestspectation
-Author: Miguel Guthridge
-Author-email: hdsq@outlook.com.au
-Project-URL: Online Documentation, https://github.com/MiguelGuthridge/Jestspectation
-Project-URL: Bug Tracker, https://github.com/MiguelGuthridge/Jestspectation/issues
-Keywords: jest,pattern,matching,pytest,equality
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Other Environment
-Classifier: Framework :: Pytest
-Requires-Python: >=3.9.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Jestspectation
 
 Pattern matching helper classes designed to allow for testing of complex data
 structures in a readable and logical format.
 
 The design is inspired by the `expect` system from JavaScript's Jest testing
 framework.
@@ -48,34 +27,28 @@
 ```
 
 ## Usage with Pytest
 
 The library can be used as a pytest plugin, which can give access to much more
 detailed error messages when assertions fail.
 
-You can enable it by adding the following lines to your `conftest.py`
-
-```py
-pytest_plugins = ("jestspectation.pytest",)
-```
-
 This should result in output similar to the following
 
-```
+```txt
     def test_goodbye():
 >       assert 1 == expect.Any(float)
 E       assert Type mismatch
 E         Expected any object of type float
 E         Received 1 (int)
 ```
 
 These advanced completions can also be used for most standard Python objects
 by wrapping the expected values in an `Equals`. For example:
 
-```
+```txt
     def test_lists():
 >       assert expect.Equals([1, 2, 3, 4]) == [1, 2, 3, 5, 6]
 E       assert [1, 2, 3, 4] == [1, 2, 3, 5, 6]
 E         !! [3] 4 == 5
 E            Value mismatch
 E            Expected 4
 E            Received 5
```

### Comparing `Jestspectation-0.9.1/jestspectation/__any.py` & `jestspectation-1.0.0/jestspectation/__any.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/__config/__config.py` & `jestspectation-1.0.0/jestspectation/__config/__config.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/__containers.py` & `jestspectation-1.0.0/jestspectation/__containers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Matchers for specific container types
 """
 
 from abc import abstractmethod
 from collections.abc import Iterable, ItemsView
-from typing import TypeGuard, TypeVar, Generic
+from typing import TypeVar, Generic
+from typing_extensions import TypeGuard
 from .__jestspectation_base import JestspectationBase
 from .__util import get_object_type_name, safe_diff_wrapper, sub_diff_delegate
 
 
 T = TypeVar('T', bound=Iterable)
 
 
@@ -335,7 +336,40 @@
         else:
             eq_expr = f"   {self_repr} == {other_repr}"
         return [eq_expr] + diff
 
     def _format_missing_item(self, item: object) -> str:
         # Format like dict keys
         return f"{repr(item[0])}: {repr(item[1])}"  # type: ignore
+
+
+class ListOfLength(JestspectationBase):
+    """
+    Matches any list of the given length
+    """
+
+    def __init__(self, length: int) -> None:
+        if length < 0:
+            raise ValueError("List length cannot be < 0")
+        self.__length = length
+
+    def __eq__(self, other: object) -> bool:
+        if not isinstance(other, list):
+            return False
+        return len(other) == self.__length
+
+    def __repr__(self) -> str:
+        return f"ListOfLength({self.__length})"
+
+    def get_diff(self, other: object, other_is_lhs: bool) -> list[str]:
+        if not isinstance(other, list):
+            return [
+                "Type mismatch",
+                f"Expected object of type list ({repr(self)})",
+                f"Received object of type {type(other).__name__} ({other})",
+            ]
+
+        return [
+            "Length failed to match",
+            f"Expected list of length {self.__length}",
+            f"Received list of length {len(other)} ({other})",
+        ]
```

### Comparing `Jestspectation-0.9.1/jestspectation/__equals.py` & `jestspectation-1.0.0/jestspectation/__equals.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/__float_approx.py` & `jestspectation-1.0.0/jestspectation/__float_approx.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/__init__.py` & `jestspectation-1.0.0/jestspectation/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .__any import Any, Anything
 from .__containers import (
     DictContainingKeys,
     DictContainingValues,
     DictContainingItems,
     ListContaining,
     SetContaining,
+    ListOfLength,
 )
 from .__float_approx import FloatApprox
 from .__equals import Equals, Is
 from .logicals import And, Not, Or, Xor
 from .__strings import (
     StringMatchingRegex,
     StringContaining,
@@ -35,14 +36,15 @@
     'DictContainingValues',
     'DictContainingItems',
     'Equals',
     'FloatApprox',
     'Is',
     'LinesLike',
     'ListContaining',
+    'ListOfLength',
     'Not',
     'Or',
     'SetContaining',
     'StringContaining',
     'StringMatchingRegex',
     'TextLike',
     'Xor',
```

### Comparing `Jestspectation-0.9.1/jestspectation/__jestspectation_base.py` & `jestspectation-1.0.0/jestspectation/__jestspectation_base.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/__py_diffs.py` & `jestspectation-1.0.0/jestspectation/__py_diffs.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/__strings/__containing.py` & `jestspectation-1.0.0/jestspectation/__strings/__containing.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/__strings/__lines_like.py` & `jestspectation-1.0.0/jestspectation/__strings/__lines_like.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Matches text similar to the given text, but with better diffs for
 multi-line text
 """
 from itertools import zip_longest
-from typing import overload, Optional, Iterable
+from typing import Union, overload, Optional, Iterable
 
 from .__text_like import TextLike
 from ..__jestspectation_base import JestspectationBase
 from ..__util import sub_diff_delegate, safe_diff_wrapper
 
 
 class LinesLike(JestspectationBase):
@@ -64,15 +64,15 @@
         ignored_sequences: Optional[Iterable[str]] = None,
         strip_lines: bool = False,
     ) -> None:
         ...
 
     def __init__(
         self,
-        lines: list[str] | str,
+        lines: Union[list[str], str],
         /,
         ignore_case: bool = True,
         ignored_sequences: Optional[Iterable[str]] = None,
         strip_lines: bool = False,
     ) -> None:
         """
         Matches text similar to the given text, but can display diffs of
```

### Comparing `Jestspectation-0.9.1/jestspectation/__strings/__matching_regex.py` & `jestspectation-1.0.0/jestspectation/__strings/__matching_regex.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/__strings/__text_like.py` & `jestspectation-1.0.0/jestspectation/__strings/__text_like.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/__util.py` & `jestspectation-1.0.0/jestspectation/__util.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/logicals/__and.py` & `jestspectation-1.0.0/jestspectation/logicals/__and.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/logicals/__not.py` & `jestspectation-1.0.0/jestspectation/logicals/__not.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/logicals/__or.py` & `jestspectation-1.0.0/jestspectation/logicals/__or.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/logicals/__xor.py` & `jestspectation-1.0.0/jestspectation/logicals/__xor.py`

 * *Files identical despite different names*

### Comparing `Jestspectation-0.9.1/jestspectation/pytest.py` & `jestspectation-1.0.0/jestspectation/pytest.py`

 * *Files identical despite different names*

