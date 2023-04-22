# Comparing `tmp/scrape_schema-0.0.3.tar.gz` & `tmp/scrape_schema-0.0.4.tar.gz`

## Comparing `scrape_schema-0.0.3.tar` & `scrape_schema-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/__init__.py
--rw-r--r--   0        0        0    18312 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/base.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/callbacks/__init__.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/callbacks/slax.py
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/callbacks/soup.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/factory/__init__.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/__init__.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/nested.py
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/regex.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/slax.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/scrape_schema/fields/soup.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/LICENSE
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/README.md
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/__init__.py
+-rw-r--r--   0        0        0    18521 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/base.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/callbacks/__init__.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/callbacks/slax.py
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/callbacks/soup.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/factory/__init__.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/fields/__init__.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/fields/nested.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/fields/regex.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/fields/slax.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/scrape_schema/fields/soup.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/README.md
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 scrape_schema-0.0.4/PKG-INFO
```

### Comparing `scrape_schema-0.0.3/scrape_schema/base.py` & `scrape_schema-0.0.4/scrape_schema/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,15 +547,21 @@
         return value
 
     def dict(self) -> dict[str, Any]:
         """convert schema object to python dict"""
         return {
             k: self._to_dict(v)
             for k, v in self.__dict__.items()
-            if not k.startswith("__") and k != "Config"
+            if not k.startswith("_") and k != "Config"
         }
 
+    def __repr_args__(self) -> list[str]:
+        return [
+            f"{k}={repr(v)}"
+            if isinstance(v, BaseSchema)
+            else f"{k}:{type(v).__name__}={repr(v)}"
+            for k, v in self.__dict__.items()
+            if not k.startswith("_") and k != "Config"
+        ]
+
     def __repr__(self):
-        return (
-            f"{self.__class__.__name__}("
-            f"{', '.join(f'{k}: {type(v).__name__} = {v}' for k, v in self.dict().items())})"
-        )
+        return f'{self.__class__.__name__}({", ".join(self.__repr_args__())})'
```

### Comparing `scrape_schema-0.0.3/scrape_schema/callbacks/slax.py` & `scrape_schema-0.0.4/scrape_schema/callbacks/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/scrape_schema/callbacks/soup.py` & `scrape_schema-0.0.4/scrape_schema/callbacks/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/scrape_schema/fields/nested.py` & `scrape_schema-0.0.4/scrape_schema/fields/nested.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/scrape_schema/fields/regex.py` & `scrape_schema-0.0.4/scrape_schema/fields/regex.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/scrape_schema/fields/slax.py` & `scrape_schema-0.0.4/scrape_schema/fields/slax.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/scrape_schema/fields/soup.py` & `scrape_schema-0.0.4/scrape_schema/fields/soup.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/.gitignore` & `scrape_schema-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/LICENSE` & `scrape_schema-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/README.md` & `scrape_schema-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/pyproject.toml` & `scrape_schema-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.0.3/PKG-INFO` & `scrape_schema-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
```

