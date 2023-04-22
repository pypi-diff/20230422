# Comparing `tmp/tomlize-0.0.2.tar.gz` & `tmp/tomlize-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomlize-0.0.2.tar", last modified: Fri Apr 21 19:39:47 2023, max compression
+gzip compressed data, was "tomlize-0.1.0.tar", last modified: Sat Apr 22 21:49:03 2023, max compression
```

## Comparing `tomlize-0.0.2.tar` & `tomlize-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-21 19:39:46.995435 tomlize-0.0.2/
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      721 2023-04-21 19:39:46.995435 tomlize-0.0.2/PKG-INFO
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      405 2023-04-21 19:39:01.000000 tomlize-0.0.2/README.md
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      486 2023-04-21 19:39:19.000000 tomlize-0.0.2/pyproject.toml
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       38 2023-04-21 19:39:46.995435 tomlize-0.0.2/setup.cfg
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-21 19:39:46.985435 tomlize-0.0.2/src/
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-21 19:39:46.995435 tomlize-0.0.2/src/tomlize/
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       63 2023-04-19 11:25:03.000000 tomlize-0.0.2/src/tomlize/__init__.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       62 2023-04-19 16:49:30.000000 tomlize-0.0.2/src/tomlize/__main__.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      247 2023-04-19 16:51:24.000000 tomlize-0.0.2/src/tomlize/cli.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      205 2023-04-19 20:42:21.000000 tomlize-0.0.2/src/tomlize/exceptions.py
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-21 19:39:46.995435 tomlize-0.0.2/src/tomlize/loaders/
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       54 2023-04-19 20:44:26.000000 tomlize-0.0.2/src/tomlize/loaders/__init__.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     4783 2023-04-20 03:17:42.000000 tomlize-0.0.2/src/tomlize/loaders/setup_py.py
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      617 2023-04-19 21:02:37.000000 tomlize-0.0.2/src/tomlize/main.py
-drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-21 19:39:46.995435 tomlize-0.0.2/src/tomlize.egg-info/
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      721 2023-04-21 19:39:46.000000 tomlize-0.0.2/src/tomlize.egg-info/PKG-INFO
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      375 2023-04-21 19:39:46.000000 tomlize-0.0.2/src/tomlize.egg-info/SOURCES.txt
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)        1 2023-04-21 19:39:46.000000 tomlize-0.0.2/src/tomlize.egg-info/dependency_links.txt
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       17 2023-04-21 19:39:46.000000 tomlize-0.0.2/src/tomlize.egg-info/requires.txt
--rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)        8 2023-04-21 19:39:46.000000 tomlize-0.0.2/src/tomlize.egg-info/top_level.txt
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:49:03.952408 tomlize-0.1.0/
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     1299 2023-04-22 21:49:03.952408 tomlize-0.1.0/PKG-INFO
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      829 2023-04-22 21:32:48.000000 tomlize-0.1.0/README.md
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      625 2023-04-22 21:48:55.000000 tomlize-0.1.0/pyproject.toml
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       38 2023-04-22 21:49:03.952408 tomlize-0.1.0/setup.cfg
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:49:03.952408 tomlize-0.1.0/src/
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:49:03.952408 tomlize-0.1.0/src/tomlize/
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       63 2023-04-19 11:25:03.000000 tomlize-0.1.0/src/tomlize/__init__.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       62 2023-04-19 16:49:30.000000 tomlize-0.1.0/src/tomlize/__main__.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      247 2023-04-19 16:51:24.000000 tomlize-0.1.0/src/tomlize/cli.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      205 2023-04-19 20:42:21.000000 tomlize-0.1.0/src/tomlize/exceptions.py
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:49:03.952408 tomlize-0.1.0/src/tomlize/loaders/
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       54 2023-04-19 20:44:26.000000 tomlize-0.1.0/src/tomlize/loaders/__init__.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     5577 2023-04-22 21:31:11.000000 tomlize-0.1.0/src/tomlize/loaders/setup_py.py
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      617 2023-04-19 21:02:37.000000 tomlize-0.1.0/src/tomlize/main.py
+drwxr-xr-x   0 mcorcherojim  (1000) mcorcherojim  (1000)        0 2023-04-22 21:49:03.952408 tomlize-0.1.0/src/tomlize.egg-info/
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)     1299 2023-04-22 21:49:03.000000 tomlize-0.1.0/src/tomlize.egg-info/PKG-INFO
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)      375 2023-04-22 21:49:03.000000 tomlize-0.1.0/src/tomlize.egg-info/SOURCES.txt
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)        1 2023-04-22 21:49:03.000000 tomlize-0.1.0/src/tomlize.egg-info/dependency_links.txt
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)       17 2023-04-22 21:49:03.000000 tomlize-0.1.0/src/tomlize.egg-info/requires.txt
+-rw-r--r--   0 mcorcherojim  (1000) mcorcherojim  (1000)        8 2023-04-22 21:49:03.000000 tomlize-0.1.0/src/tomlize.egg-info/top_level.txt
```

### Comparing `tomlize-0.0.2/src/tomlize/loaders/setup_py.py` & `tomlize-0.1.0/src/tomlize/loaders/setup_py.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,53 +22,60 @@
     data = _extract_setup_args(setup_path)
     ret = {}
 
     ## Pending fields
     # ext_modules
     # ext_package
     # package_data
-    # license
     # entry_points
 
     ### Ignored fields ###
     for field in [
         "zip_safe",  # Deprecated
     ]:
         data.pop(field, None)
 
     ### metadata fields ###
     metadata = {}
     for attr in [
         "name",
         "version",
         "description",
-        "url",
         "download_url",
         "classifiers",
         "keywords",
     ]:
         moveif(data, metadata, attr)
     for orig_attr, dst_attr in [
         ("python_requires", "requires-python"),
         ("install_requires", "dependencies"),
         ("extras_require", "optional-dependencies"),
+        ("project_urls", "urls"),
     ]:
         moveif(data, metadata, orig_attr, dst_attr)
     if "author" in data or "author_email" in data:
         metadata["authors"] = [{}]
         if name := data.pop("author", None):
             metadata["authors"][0]["name"] = name
         if email := data.pop("author_email", None):
             metadata["authors"][0]["email"] = email
     if "maintainer" in data or "maintainer_email" in data:
         metadata["maintainers"] = [{}]
         if name := data.pop("maintainer", None):
             metadata["maintainers"][0]["name"] = name
         if email := data.pop("maintainer_email", None):
             metadata["maintainers"][0]["email"] = email
+    if url := data.pop("url", None):
+        if "urls" not in metadata:
+            metadata["urls"] = {}
+        metadata["urls"]["Home-page"] = url
+    if license_text := data.pop("license", None):
+        metadata["license"] = {"text": license_text}
+    if license_file := data.pop("license_file", None):
+        metadata["license"] = {"file": license_file}
 
     ### build system fields ###
     build_system = {
         "build-backend": "setuptools.build_meta",
         "requires": [],
     }
     for req_str in data.pop("setup_requires", []):
@@ -87,20 +94,27 @@
     ):
         build_system["requires"].append(
             f"setuptools >= {MIN_SETUPTOOLS_VERSION}",
         )
     ret["build-system"] = build_system
 
     ### setuptools specific fields ###
+    setuptools_specific = {}
+
     if data.get("package_dir", {}).get("") == "src":
+        # TODO: Properly figure out if we can default to automatic discovery
         # standard src layout, default to automatic discovery
         data.pop("package_dir")
         data.pop("packages", None)
         data.pop("py_modules", None)
-    setuptools_specific = {}
+    else:
+        moveif(data, setuptools_specific, "packages")
+        moveif(data, setuptools_specific, "py_modules")
+        moveif(data, setuptools_specific, "package_dir", "package-dir")
+
     for attr in [
         "platform",
         "packages",
     ]:
         moveif(data, setuptools_specific, attr)
     for orig_attr, dst_attr in [
         ("scripts", "script-files"),
@@ -114,33 +128,34 @@
     ### Enhancements ###
     project_root = setup_path.parent
     for name in ["README.rst", "README.md"]:
         if project_root.joinpath(name).exists():
             metadata["readme"] = name
             data.pop("long_description", None)
             data.pop("long_description_content_type", None)
+    if isinstance(metadata.get("keywords"), str):
+        metadata["keywords"] = metadata["keywords"].split(", ")
+    # TODO: Find and use license-file (glob)
 
     ### Warn on remaining fields ###
     for field in data:
         logging.warning("Unexpected field found: %s", field)
 
     if metadata:
         ret["project"] = metadata
     if setuptools_specific:
-        ret["tool.setuptools"] = setuptools_specific
+        ret["tool"] = {"setuptools": setuptools_specific}
     return ret
 
 
 def _run_setup_py(setup_path: pathlib.Path):
     try:
         exec(
             setup_path.read_text(),
-            {
-                "__name__": "__main__",
-            },
+            {"__name__": "__main__", "__file__": "setup.py"},
         )
     except FileNotFoundError:
         raise exceptions.FailedToParseError(setup_path, "File not found")
     except ImportError as e:
         raise exceptions.FailedToParseError(
             setup_path, f"Unable to import {e.name!r}, are you missing a dependency?"
         )
```

### Comparing `tomlize-0.0.2/src/tomlize/main.py` & `tomlize-0.1.0/src/tomlize/main.py`

 * *Files identical despite different names*

