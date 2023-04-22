# Comparing `tmp/transon-0.0.6.tar.gz` & `tmp/transon-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transon-0.0.6.tar", max compression
+gzip compressed data, was "transon-0.0.7.tar", max compression
```

## Comparing `transon-0.0.6.tar` & `transon-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     4444 2023-04-21 07:39:47.969963 transon-0.0.6/README.md
--rw-r--r--   0        0        0      881 2023-04-21 07:39:47.969963 transon-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      174 2023-04-21 07:39:47.969963 transon-0.0.6/transon/__init__.py
--rw-r--r--   0        0        0     3186 2023-04-21 07:39:47.969963 transon-0.0.6/transon/docs.py
--rw-r--r--   0        0        0      173 2023-04-21 07:39:47.969963 transon-0.0.6/transon/functions.py
--rw-r--r--   0        0        0     1455 2023-04-21 07:39:47.969963 transon-0.0.6/transon/operators.py
--rw-r--r--   0        0        0    16737 2023-04-21 07:39:47.969963 transon-0.0.6/transon/rules.py
--rw-r--r--   0        0        0        0 2023-04-21 07:39:47.969963 transon-0.0.6/transon/tests/__init__.py
--rw-r--r--   0        0        0     1448 2023-04-21 07:39:47.969963 transon-0.0.6/transon/tests/base.py
--rw-r--r--   0        0        0      347 2023-04-21 07:39:47.969963 transon-0.0.6/transon/tests/base_attr.py
--rw-r--r--   0        0        0      763 2023-04-21 07:39:47.969963 transon-0.0.6/transon/tests/base_join.py
--rw-r--r--   0        0        0       68 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/conftest.py
--rw-r--r--   0        0        0     4339 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_attr.py
--rw-r--r--   0        0        0     1080 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_chain.py
--rw-r--r--   0        0        0      984 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_convert.py
--rw-r--r--   0        0        0     4225 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_expr.py
--rw-r--r--   0        0        0     1981 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_file.py
--rw-r--r--   0        0        0     2248 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_filter.py
--rw-r--r--   0        0        0     2102 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_format.py
--rw-r--r--   0        0        0      604 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_include.py
--rw-r--r--   0        0        0     2890 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_join.py
--rw-r--r--   0        0        0     3866 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_map.py
--rw-r--r--   0        0        0     2952 2023-04-21 07:39:47.973963 transon-0.0.6/transon/tests/test_no_content.py
--rw-r--r--   0        0        0     8130 2023-04-21 07:39:47.973963 transon-0.0.6/transon/transformers.py
--rw-r--r--   0        0        0     5391 1970-01-01 00:00:00.000000 transon-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     4444 2023-04-22 11:40:18.703710 transon-0.0.7/README.md
+-rw-r--r--   0        0        0      883 2023-04-22 11:40:18.703710 transon-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-04-22 11:40:18.707710 transon-0.0.7/transon/__init__.py
+-rw-r--r--   0        0        0     3901 2023-04-22 11:40:18.707710 transon-0.0.7/transon/docs.py
+-rw-r--r--   0        0        0      173 2023-04-22 11:40:18.707710 transon-0.0.7/transon/functions.py
+-rw-r--r--   0        0        0     1455 2023-04-22 11:40:18.707710 transon-0.0.7/transon/operators.py
+-rw-r--r--   0        0        0    16744 2023-04-22 11:40:18.707710 transon-0.0.7/transon/rules.py
+-rw-r--r--   0        0        0        0 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/__init__.py
+-rw-r--r--   0        0        0     1448 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/base.py
+-rw-r--r--   0        0        0      347 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/base_attr.py
+-rw-r--r--   0        0        0      763 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/base_join.py
+-rw-r--r--   0        0        0       68 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/conftest.py
+-rw-r--r--   0        0        0     4807 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_attr.py
+-rw-r--r--   0        0        0     1080 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_chain.py
+-rw-r--r--   0        0        0      984 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_convert.py
+-rw-r--r--   0        0        0     4225 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_expr.py
+-rw-r--r--   0        0        0     1981 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_file.py
+-rw-r--r--   0        0        0     1809 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_filter.py
+-rw-r--r--   0        0        0     2102 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_format.py
+-rw-r--r--   0        0        0      996 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_include.py
+-rw-r--r--   0        0        0      670 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_invalid_value.py
+-rw-r--r--   0        0        0     2890 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_join.py
+-rw-r--r--   0        0        0     3565 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_map.py
+-rw-r--r--   0        0        0     2952 2023-04-22 11:40:18.707710 transon-0.0.7/transon/tests/test_no_content.py
+-rw-r--r--   0        0        0     8225 2023-04-22 11:40:18.707710 transon-0.0.7/transon/transformers.py
+-rw-r--r--   0        0        0     5455 1970-01-01 00:00:00.000000 transon-0.0.7/PKG-INFO
```

### Comparing `transon-0.0.6/README.md` & `transon-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/pyproject.toml` & `transon-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "transon"
-version = "0.0.6"
+version = "0.0.7"
 description = "Homogenous JSON template engine"
 authors = ["Eugene Chernyshov <chernyshov.eugene@gmail.com>"]
 readme = "README.md"
-homepage = "https://github.com/transon-org/transon"
+repository = "https://github.com/transon-org/transon"
 documentation = "https://transon-org.github.io/"
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `transon-0.0.6/transon/docs.py` & `transon-0.0.7/transon/docs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,46 @@
-import os.path
+import importlib
 import inspect
+import pkgutil
 
-import unittest
 from functools import lru_cache
+from types import ModuleType
 
 try:  # pragma: no cover
     from importlib.metadata import version
 except ImportError:  # pragma: no cover
     # noinspection PyUnresolvedReferences
     from importlib_metadata import version
 
-import transon
 from transon import Transformer
 
 
+def import_submodules(package: ModuleType | str, recursive=True):
+    if isinstance(package, str):
+        try:
+            package = importlib.import_module(package)
+        except Exception:
+            return {}
+    results = {}
+    for loader, name, is_pkg in pkgutil.walk_packages(package.__path__):
+        full_name = package.__name__ + '.' + name
+        try:
+            results[full_name] = importlib.import_module(full_name)
+        except Exception:
+            pass
+        else:
+            if recursive and is_pkg:
+                results.update(import_submodules(full_name))
+    return results
+
+
 @lru_cache(maxsize=None)
 def get_test_cases():
     from transon.tests.base import TableDataBaseCase
-    project_root = os.path.dirname(os.path.dirname(transon.__file__))
-    unittest.defaultTestLoader.discover(project_root)
+    import_submodules('transon.tests')
     return list(TableDataBaseCase.iterate_valid_cases())
 
 
 @lru_cache(maxsize=None)
 def get_test_cases_by_tag(tag: str):
     return [
         case
@@ -120,7 +138,12 @@
         ]
     }
 
 
 if __name__ == '__main__':  # pragma: no cover
     import json
     print(json.dumps(get_all_docs(), indent=4))
+    for case in get_test_cases():
+        doc = inspect.getdoc(case)
+        if 'TBD' in doc:
+            print(f'no doc in {case}: {doc}')
+    print(len(get_test_cases()))
```

### Comparing `transon-0.0.6/transon/operators.py` & `transon-0.0.7/transon/operators.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/transon/rules.py` & `transon-0.0.7/transon/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,15 +508,15 @@
         return pattern.format(**value)
     else:
         return pattern.format(value)
 
 
 @Transformer.register_rule(
     'include',
-    name="Name or path to template. Can be dynamic. Meaning of this depends of provided template loader.",
+    name="Name or path to template. Can be dynamic. Meaning of this `name` depends on provided template loader.",
 )
 def rule_include(t: Transformer, template, context: Context):
     t_name = t.require(template, 'name')
     name = t.walk(t_name, context)
     sub_transformer = t.template_loader(name)
     result = sub_transformer.transform(context.this)
     return t.NO_CONTENT if result is sub_transformer.NO_CONTENT else result
```

### Comparing `transon-0.0.6/transon/tests/base.py` & `transon-0.0.7/transon/tests/base.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/transon/tests/base_join.py` & `transon-0.0.7/transon/tests/base_join.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/transon/tests/test_attr.py` & `transon-0.0.7/transon/tests/test_attr.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,19 @@
     data = {
         'a': 1
     }
     result = None
 
 
 class AttrSimplePathDoesNotExist1(base.TableDataBaseCase):
+    """
+    Tries to get a value from nested input structure of `dicts` with paths defined in different attribute of input data.
+    Actual path is not correct at its second component.
+    Template results with no value.
+    """
     tags = []
     template = {
         '$': 'attr',
         'names': ['a', 'x', 'c'],
     }
     data = {
         'a': {
@@ -45,14 +50,19 @@
             }
         }
     }
     result = None
 
 
 class AttrSimplePathDoesNotExist2(base.TableDataBaseCase):
+    """
+    Tries to get a value from nested input structure of `lists` with paths defined in different attribute of input data.
+    Actual path is not correct at its second component.
+    Template results with no value.
+    """
     tags = []
     template = {
         '$': 'attr',
         'names': [0, 1, 0],
     }
     data = [[[1]]]
     result = None
@@ -100,15 +110,15 @@
         'name': 'b',
     }
     result = 2
 
 
 class AttrSimpleFixedNames(base.TableDataBaseCase):
     """
-    Gets a list of values with 4 elements discovered in nested input structure of dicts with paths defined in template.
+    Gets a `list` of values with 4 elements discovered in nested input structure of `dicts` with paths defined in template.
     """
     tags = ['attr:names']
     template = [
         {'$': 'attr', 'names': ['a', 'b', 'c']},
         {'$': 'attr', 'names': ['a', 'b', 'd']},
         {'$': 'attr', 'names': ['a', 'e', 'f']},
         {'$': 'attr', 'names': ['a', 'e', 'g']},
@@ -126,15 +136,15 @@
         },
     }
     result = [1, 2, 3, 4]
 
 
 class AttrDynamicReferenceNames(base.TableDataBaseCase):
     """
-    Gets value from nested input structure of dicts with paths defined in different attribute of input data.
+    Gets value from nested input structure of `dicts` with paths defined in different attribute of input data.
     """
     tags = ['attr:names']
     template = {
         '$': 'attr',
         'names': {'$': 'attr', 'name': 'path'},
     }
     data = {
@@ -151,15 +161,15 @@
         'path': ['a', 'e', 'f']
     }
     result = 3
 
 
 class AttrDynamicReferenceMultipleNames(base.TableDataBaseCase):
     """
-    Gets a list of values discovered in nested input structure of dicts with paths defined in input data.
+    Gets a `list` of values discovered in nested input structure of `dicts` with paths defined in input data.
     List of paths may include any number of paths of any depth.
     """
     tags = ['attr:names', 'chain', 'set', 'get', 'map:item']
     template = {
         '$': 'chain',
         'funcs': [
             {'$': 'set', 'name': 'root'},
```

### Comparing `transon-0.0.6/transon/tests/test_chain.py` & `transon-0.0.7/transon/tests/test_chain.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/transon/tests/test_convert.py` & `transon-0.0.7/transon/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/transon/tests/test_expr.py` & `transon-0.0.7/transon/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/transon/tests/test_file.py` & `transon-0.0.7/transon/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/transon/tests/test_filter.py` & `transon-0.0.7/transon/tests/test_format.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,83 @@
-import pytest
-
 from . import base
-from transon import (
-    TransformationError,
-    Transformer,
-)
 
 
-class FilterDict(base.TableDataBaseCase):
+class FormatFromSingleValue(base.TableDataBaseCase):
     """
-    Iterates over input `dict` and filters out items with even value.
+    Iterates list with floats and produces list of strings by formatting each item.
     """
-    tags = ['filter', 'expr']
+    tags = ['map:item', 'format']
     template = {
-        '$': 'filter',
-        'cond': {
-            '$': 'expr',
-            'op': 'mod',
-            'values': [
-                {'$': 'value'},
-                2,
-            ]
+        '$': 'map',
+        'item': {
+            '$': 'format',
+            'pattern': '{:.03f}'
         }
     }
-    data = {
-        'a': 1,
-        'b': 2,
-        'c': 3,
-        'd': 4,
-        'e': 5,
-        'f': 6,
-    }
-    result = {
-        'a': 1,
-        'c': 3,
-        'e': 5,
-    }
+    data = [1 / i for i in range(2, 10)]
+    result = ['0.500', '0.333', '0.250', '0.200', '0.167', '0.143', '0.125', '0.111']
 
 
-class FilterList(base.TableDataBaseCase):
+class FormatFromDict(base.TableDataBaseCase):
     """
-    Iterates over input `list` and filters out items with even value.
+    Iterates over list of dicts and produces list of string using items for filling pattern slots.
     """
-    tags = ['filter', 'expr']
+    tags = ['map:item', 'format']
     template = {
-        '$': 'filter',
-        'cond': {
-            '$': 'expr',
-            'op': 'mod',
-            'values': [
-                {'$': 'item'},
-                2,
-            ]
+        '$': 'map',
+        'item': {
+            '$': 'format',
+            'pattern': '{name}-{index}'
         }
     }
-    data = [1, 2, 3, 4, 5, 6]
-    result = [1, 3, 5]
+    data = [
+        {'name': 'a', 'index': 1},
+        {'name': 'b', 'index': 2},
+        {'name': 'c', 'index': 3},
+    ]
+    result = ['a-1', 'b-2', 'c-3']
 
 
-class FilterListNoContent(base.TableDataBaseCase):
+class FormatFromList(base.TableDataBaseCase):
     """
-    Sets some names to context, one with `true` value and one with `false`.
-    Iterates over input `list` of string and filters out items with name that is not set to `true` in the context.
+    Iterates over list of lists and produces list of string using items for filling pattern slots.
     """
-    tags = ['chain', 'filter', 'set', 'get']
+    tags = ['map:item', 'format']
     template = {
-        '$': 'chain',
-        'funcs': [
-            {'$': 'set', 'name': 'current'},
-            True,
-            {'$': 'set', 'name': 'a'},
-            False,
-            {'$': 'set', 'name': 'b'},
-            {'$': 'get', 'name': 'current'},
-            {
-                '$': 'filter',
-                'cond': {
-                    '$': 'get',
-                    'name': {'$': 'item'},
-                }
-            }
-        ]
+        '$': 'map',
+        'item': {
+            '$': 'format',
+            'pattern': '{0}-{1}'
+        }
     }
-    data = ['a', 'b', 'c']
-    result = ['a']
+    data = [
+        ['a', 1],
+        ['b', 2],
+        ['c', 3],
+    ]
+    result = ['a-1', 'b-2', 'c-3']
 
 
-def test_invalid_value():
+class FormatWithValue(base.TableDataBaseCase):
+    """
+    Iterates over list of values.
+    For formatting value creates dict with dynamically calculated values.
+    Produces list of strings using formatting.
+    """
+    tags = ['map:item', 'format:value', 'index', 'expr:values']
     template = {
-        '$': 'filter',
-        'cond': {
-            '$': 'expr',
-            'op': 'mod',
-            'values': [
-                {'$': 'item'},
-                2,
-            ]
+        '$': 'map',
+        'item': {
+            '$': 'format',
+            'pattern': '{x}-{y}',
+            'value': {
+                'x': {'$': 'this'},
+                'y': {
+                    '$': 'expr',
+                    'op': '+',
+                    'values': [{'$': 'index'}, 1]
+                }
+            }
         }
     }
-    transformer = Transformer(template)
-    with pytest.raises(TransformationError):
-        transformer.transform(1)
+    data = ['a', 'b', 'c']
+    result = ['a-1', 'b-2', 'c-3']
```

### Comparing `transon-0.0.6/transon/tests/test_join.py` & `transon-0.0.7/transon/tests/test_join.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/transon/tests/test_map.py` & `transon-0.0.7/transon/tests/test_map.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-import pytest
-
 from . import base
-from transon import (
-    Transformer,
-    TransformationError,
-)
 
 
 class MapListToList(base.TableDataBaseCase):
     """
     Maps two lists obtained from different attributes of input.
     Then joins two obtained lists into single resulting list.
     """
@@ -122,24 +116,14 @@
     result = [
         'a', 1,
         'b', 2,
         'c', 3,
     ]
 
 
-def test_invalid_value():
-    template = {
-        '$': 'map',
-        'item': {'$': 'item'},
-    }
-    transformer = Transformer(template)
-    with pytest.raises(TransformationError):
-        transformer.transform(1)
-
-
 class MapListsToDict(base.TableDataBaseCase):
     """
     Zips two lists containing keys and values together into pairs.
     Then iterates over list of pairs and produces resulting dict.
     """
     tags = ['chain', 'zip', 'map:key', 'map:value', 'attr:name']
     template = {
```

### Comparing `transon-0.0.6/transon/tests/test_no_content.py` & `transon-0.0.7/transon/tests/test_no_content.py`

 * *Files identical despite different names*

### Comparing `transon-0.0.6/transon/transformers.py` & `transon-0.0.7/transon/transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,26 +78,34 @@
 # noinspection PyUnusedLocal
 def no_template_loader(name: str) -> 'Transformer':   # pragma: no cover
     raise RuntimeError(f'template with name `{name}` was not found')
 
 
 class Transformer:
     """
+    ## Usage
+
     `Transformer` class interpolates template with input data.
     Format of output is defined by template.
     Input is used to fill values into template placeholders.
 
     ```python
+    from transon import Transformer
+
     transformer = Transformer(template)
     output_data = transformer.transform(input_data)
     ```
 
+    ## Templates
+
     Template could be any JSON structure. It will be reflected as-is in output, except of `rules` structures.
     Rules are json objects with special attribute named `$` (this is called marker and can be changed).
-    If the rule has nested template the same applies to it as well. For example
+    If the rule has nested template the same applies to it as well.
+
+    Example template:
 
     ```json
     {
         "test": {
             "$": "map",
             "item": [
                 {
@@ -111,28 +119,31 @@
     ```
 
     At the top level output will just copy template `{"test": ...}`.
     Then the `map` rule will be applied to the input executing sub-template, defined by `item` attribute,
     for each item in input collection.
     Let's assume that our input is `[1, 2, 3]`.
     Inner template contains another rule `{"$": "item"}` which points to value of items of the input.
+
     So the final result will be:
 
     ```json
-        {
+    {
         "test": [
             [{"x": 1}],
             [{"x": 2}],
             [{"x": 3}],
         ]
     }
     ```
 
     Note that each item preserves its template definition (including list around object).
 
+    ## Extending
+
     All rules are pluggable. There is a list of rules available out of the box.
     However, you can easily add your own rules with their own attributes.
 
     ```python
     @Transformer.register_rule('my_rule')
     def my_rule(t: Transformer, template, context: Context):
         ...
```

### Comparing `transon-0.0.6/PKG-INFO` & `transon-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transon
-Version: 0.0.6
+Version: 0.0.7
 Summary: Homogenous JSON template engine
 Home-page: https://github.com/transon-org/transon
 License: MIT
 Author: Eugene Chernyshov
 Author-email: chernyshov.eugene@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: importlib-metadata (>=6.5.0,<7.0.0) ; python_version == "3.7"
 Project-URL: Bug Tracker, https://github.com/transon-org/transon/issues
 Project-URL: Documentation, https://transon-org.github.io/
+Project-URL: Repository, https://github.com/transon-org/transon
 Description-Content-Type: text/markdown
 
 # transon
 
 ![PyPI](https://img.shields.io/pypi/v/transon)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/transon)
 ![Codecov](https://img.shields.io/codecov/c/github/transon-org/transon)
```

