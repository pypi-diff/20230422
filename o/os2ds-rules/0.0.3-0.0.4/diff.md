# Comparing `tmp/os2ds-rules-0.0.3.tar.gz` & `tmp/os2ds-rules-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2ds-rules-0.0.3.tar", last modified: Sat Apr 15 10:09:14 2023, max compression
+gzip compressed data, was "os2ds-rules-0.0.4.tar", last modified: Sat Apr 22 12:41:50 2023, max compression
```

## Comparing `os2ds-rules-0.0.3.tar` & `os2ds-rules-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.489535 os2ds-rules-0.0.3/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/include/cpr-detector.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/lib/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/lib/cpr-detector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/lib/name_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.489535 os2ds-rules-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/src/os2ds_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/src/os2ds_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/src/os2ds_rules/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/src/os2ds_rules/cpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-15 10:09:02.000000 os2ds-rules-0.0.3/src/os2ds_rules/name_rule.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 10:09:14.493536 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-15 10:09:14.000000 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-15 10:09:14.000000 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 10:09:14.000000 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-15 10:09:14.000000 os2ds-rules-0.0.3/src/os2ds_rules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:41:50.174703 os2ds-rules-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-22 12:41:50.174703 os2ds-rules-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:41:50.170704 os2ds-rules-0.0.4/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/include/cpr-detector.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:41:50.170704 os2ds-rules-0.0.4/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/lib/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/lib/cpr-detector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/lib/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/lib/wordlist_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 12:41:50.174703 os2ds-rules-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:41:50.170704 os2ds-rules-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:41:50.174703 os2ds-rules-0.0.4/src/os2ds_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/src/os2ds_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/src/os2ds_rules/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/src/os2ds_rules/cpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/src/os2ds_rules/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-22 12:41:38.000000 os2ds-rules-0.0.4/src/os2ds_rules/wordlist_rule.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 12:41:50.174703 os2ds-rules-0.0.4/src/os2ds_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-04-22 12:41:50.000000 os2ds-rules-0.0.4/src/os2ds_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-22 12:41:50.000000 os2ds-rules-0.0.4/src/os2ds_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 12:41:50.000000 os2ds-rules-0.0.4/src/os2ds_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-22 12:41:50.000000 os2ds-rules-0.0.4/src/os2ds_rules.egg-info/top_level.txt
```

### Comparing `os2ds-rules-0.0.3/LICENSE` & `os2ds-rules-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.3/PKG-INFO` & `os2ds-rules-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.3
+Version: 0.0.4
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `os2ds-rules-0.0.3/README.md` & `os2ds-rules-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.3/include/cpr-detector.hpp` & `os2ds-rules-0.0.4/include/cpr-detector.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -11,43 +11,26 @@
 #include <string_view>
 #include <vector>
 
 namespace OS2DSRules {
 
 namespace CPRDetector {
 
-using Predicate = std::function<bool(char)>;
-
-template <typename T>
-  requires std::same_as<T, char>
-constexpr auto make_predicate(T d) noexcept {
-  return [d](T c) { return c == d; };
-}
-
-template <typename T, typename... Args>
-constexpr auto make_predicate(T d, Args... ds) noexcept {
-  if constexpr (sizeof...(ds) > 0) {
-    return [d, ds...](T c) {
-      return make_predicate(d)(c) || make_predicate(ds...)(c);
-    };
-  } else
-    return make_predicate(d);
-}
-
 constexpr bool is_nonzero_digit(char c) noexcept { return '0' < c && c <= '9'; }
 
 constexpr bool is_digit(char c) noexcept { return '0' <= c && c <= '9'; }
 
 const auto is_separator = make_predicate(' ', '-', '/');
 
 const auto is_previous_ok = make_predicate(char(0), ' ', '\n', '\t', '\0');
 
 constexpr bool is_space(const char c) noexcept { return c == ' '; }
 
-const std::array<int, 10> modulus11_factors = {4, 3, 2, 7, 6, 5, 4, 3, 2, 1};
+static constexpr std::array<int, 10> modulus11_factors = {4, 3, 2, 7, 6,
+                                                          5, 4, 3, 2, 1};
 
 class CPRDetector {
 private:
   enum class CPRDetectorState : unsigned char {
     Empty,
     First,
     Second,
```

### Comparing `os2ds-rules-0.0.3/lib/address_rule.cpp` & `os2ds-rules-0.0.4/lib/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.3/lib/cpr-detector.cpp` & `os2ds-rules-0.0.4/lib/cpr-detector.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.3/lib/name_rule.cpp` & `os2ds-rules-0.0.4/lib/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.3/pyproject.toml` & `os2ds-rules-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "os2ds-rules"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="HackTheOxidation", email="tomas.hagenau@protonmail.ch" },
 ]
 description = "Text processing tool for detecting Danish CPR-numbers."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `os2ds-rules-0.0.3/setup.py` & `os2ds-rules-0.0.4/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from setuptools import Extension, setup
 
 
-CXX_FLAGS = ("/O3", "/std:c++20") if os.name == "nt" else ("-O3", "-std=c++20")
+CXX_FLAGS = ["/std:c++20"] if os.name == "nt" else ["-std=c++20", "-O3"]
 
 CPR_SOURCES = (
     "src/os2ds_rules/cpr.cpp",
     "lib/cpr-detector.cpp",
     )
 
 NAMERULE_SOURCES = (
@@ -15,32 +15,44 @@
     )
 
 ADDRESSRULE_SOURCES = (
     "src/os2ds_rules/address_rule.cpp",
     "lib/address_rule.cpp",
     )
 
+WORDLISTRULE_SOURCES = (
+    "src/os2ds_rules/wordlist_rule.cpp",
+    "lib/wordlist_rule.cpp",
+    )
+
 cpr_detector = Extension(name="os2ds_rules.cpr_detector",
                          language="c++",
                          include_dirs=["include/"],
                          sources=[*CPR_SOURCES],
-                         extra_compile_args=[*CXX_FLAGS])
+                         extra_compile_args=CXX_FLAGS)
 
 name_rule = Extension(name="os2ds_rules.name_rule",
                       language="c++",
                       include_dirs=["include/"],
                       sources=[*NAMERULE_SOURCES],
-                      extra_compile_args=[*CXX_FLAGS])
+                      extra_compile_args=CXX_FLAGS)
 
 address_rule = Extension(name="os2ds_rules.address_rule",
                          language="c++",
                          include_dirs=["include/"],
                          sources=[*ADDRESSRULE_SOURCES],
-                         extra_compile_args=[*CXX_FLAGS])
+                         extra_compile_args=CXX_FLAGS)
+
+wordlist_rule = Extension(name="os2ds_rules.wordlist_rule",
+                          language="c++",
+                          include_dirs=["include/"],
+                          sources=[*WORDLISTRULE_SOURCES],
+                          extra_compile_args=CXX_FLAGS)
 
 setup(
     ext_modules=[
         cpr_detector,
         name_rule,
         address_rule,
+        wordlist_rule,
       ]
     )
```

### Comparing `os2ds-rules-0.0.3/src/os2ds_rules/__init__.py` & `os2ds-rules-0.0.4/src/os2ds_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.3/src/os2ds_rules/address_rule.cpp` & `os2ds-rules-0.0.4/src/os2ds_rules/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.3/src/os2ds_rules/cpr.cpp` & `os2ds-rules-0.0.4/src/os2ds_rules/cpr.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.3/src/os2ds_rules/name_rule.cpp` & `os2ds-rules-0.0.4/src/os2ds_rules/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.3/src/os2ds_rules.egg-info/PKG-INFO` & `os2ds-rules-0.0.4/src/os2ds_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.3
+Version: 0.0.4
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

