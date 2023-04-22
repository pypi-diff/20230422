# Comparing `tmp/armaqdl-0.6.1.tar.gz` & `tmp/armaqdl-0.7.0.tar.gz`

## Comparing `armaqdl-0.6.1.tar` & `armaqdl-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.6.1/.editorconfig
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.6.1/.flake8
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.6.1/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.6.1/armaqdl/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.6.1/armaqdl/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 armaqdl-0.6.1/armaqdl/_version.py
--rw-r--r--   0        0        0    14851 2020-02-02 00:00:00.000000 armaqdl-0.6.1/armaqdl/armaqdl.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 armaqdl-0.6.1/armaqdl/config.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 armaqdl-0.6.1/armaqdl/const.py
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 armaqdl-0.6.1/armaqdl/update.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 armaqdl-0.6.1/config/settings.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 armaqdl-0.6.1/tests/test_commands.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.6.1/tests/test_config.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.6.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.6.1/LICENSE
--rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 armaqdl-0.6.1/README.md
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 armaqdl-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 armaqdl-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 armaqdl-0.7.0/.editorconfig
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 armaqdl-0.7.0/.flake8
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 armaqdl-0.7.0/.gitattributes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/_version.py
+-rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/armaqdl.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/config.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/const.py
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 armaqdl-0.7.0/armaqdl/update.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 armaqdl-0.7.0/config/settings.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 armaqdl-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 armaqdl-0.7.0/tests/test_commands.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 armaqdl-0.7.0/tests/test_config.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 armaqdl-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 armaqdl-0.7.0/LICENSE
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 armaqdl-0.7.0/README.md
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 armaqdl-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 armaqdl-0.7.0/PKG-INFO
```

### Comparing `armaqdl-0.6.1/armaqdl/armaqdl.py` & `armaqdl-0.7.0/armaqdl/armaqdl.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,19 +59,22 @@
         last_rpt = max(rpt_list, key=os.path.getctime)
         if not DRY:
             os.startfile(last_rpt)
     else:
         print("Warning! Opening last log only implemented for Windows.")
 
 
-def build_mod(path, tool):
+def build_mod(path, tool, launch_type=""):
     for build_tool in SETTINGS.get("build", {}):
         req_file = SETTINGS["build"][build_tool]["presence"]
         cmd = SETTINGS["build"][build_tool]["command"]
 
+        if launch_type and cmd[0] == "hemtt":
+            cmd[1] = launch_type
+
         if (tool == "b" or tool.lower() == build_tool.lower()) and (path / req_file).exists():
             print(f"=> Building [{build_tool}] ...")
 
             if not DRY:
                 try:
                     subprocess.run(cmd, cwd=path, shell=True, check=True)
                 except subprocess.CalledProcessError:
@@ -105,16 +108,15 @@
         # Path
         cli_mod = mod
         separators = cli_mod.count(":")
         if separators == 1:
             location, mod = cli_mod.split(":")
         elif separators > 1:
             location, mod, marks = cli_mod.split(":", 2)
-            if isinstance(marks, str):
-                marks = [marks]
+            marks = marks.split(":")
             marks = [x.lower() for x in marks]
 
         if location not in SETTINGS.get("locations", {}).keys():
             # Absolute path
             mod = f"{location}:{mod}"
             location = "abs"
             location_path = ""
@@ -122,14 +124,15 @@
             # Predefined path
             location_path = SETTINGS.get("locations", {}).get(location, {}).get('path')
             if location_path is None:
                 print(f"Invalid location: {location}")
                 continue
 
         path = Path(location_path) / mod
+        path_build = path
 
         # Split wildcard (add to the end)
         if "*" in mod:
             mods_wildcard = [f"{location}:{str(mod_wildcard)[len(location_path) + 1:]}"
                              for mod_wildcard in path.parent.glob("*") if mod_wildcard.is_dir()]
             mods.extend(mods_wildcard)
             ignores += 1
@@ -150,35 +153,58 @@
 
         # Skip mod found in wildcard
         if path in skips:
             print(f"(skip) {cli_mod}  [{path}]")
             ignores += 1
             continue
 
+        # Get just identifiers (first letters) of each mark
+        marks_identifiers = [x[0] for x in marks]
+
+        # HEMTT launch type argument
+        launch_type = ""  # Empty is path itself (non-HEMTT)
+        if (path / ".hemttout").exists():
+            launch_type = SETTINGS.get("locations", {}).get(location, {}).get("type", "dev")
+
+        if "t" in marks_identifiers:
+            launch_type_index = marks_identifiers.index("t")
+            launch_type = marks[launch_type_index][1:]
+
+            if launch_type not in ["", "dev", "build", "release"]:
+                print(f"Invalid launch type: {launch_type} (HEMTT)  [{location}:{mod}]")
+                continue
+
+        if launch_type:
+            path = path / ".hemttout" / launch_type
+
         # Local build argument
         build_tool = ""
-        marks_build = [x[0] for x in marks]
-        if "b" in marks_build:
-            mark_build_index = marks_build.index("b")
+        if "b" in marks_identifiers:
+            mark_build_index = marks_identifiers.index("b")
             build_tool = marks[mark_build_index][1:]
 
             if not build_tool:
                 build_tool = "b"
 
         # Global build argument
         if not build_tool and build_dev_tool is not None and (location == "abs" or SETTINGS["locations"][location].get("build", False)):
             build_tool = build_dev_tool
 
         print(f"{cli_mod}  [{path}]")
 
         # Build
         if build_tool:
-            if not build_mod(path, build_tool):
+            if not build_mod(path_build, build_tool, launch_type=launch_type):
                 continue
 
+        # Check path existance after build, as HEMTT output does not exist if no build has been performed yet
+        if not path.exists():
+            print(f"Invalid mod path: {path}")
+            continue
+
         paths.append(path)  # Marks success
 
     # Some mods are invalid (return at the end to show all invalid locations/paths)
     if VERBOSE:
         print(f"Paths: {len(paths)} processed vs. {len(mods) - ignores} input ({len(mods)} mods - {ignores} ignores)")
 
     if len(paths) != len(mods) - ignores:
@@ -358,15 +384,15 @@
 
     # Parse arguments
     parser = argparse.ArgumentParser(
         prog=PACKAGE,
         description=f"Quick development Arma 3 launcher v{__version__}",
         formatter_class=argparse.RawTextHelpFormatter)
 
-    parser.add_argument("mods", metavar="loc:mod[:b[tool]][:s|:skip] ...", type=str, nargs="*", help="paths to mods or 'none' for no mods")
+    parser.add_argument("mods", metavar="loc:mod[:b[tool]][:s|:skip][:t[type]] ...", type=str, nargs="*", help="paths to mods or 'none' for no mods")
     parser.add_argument("-m", "--mission", default="", type=str, help="mission to load")
 
     parser.add_argument("-s", "--server", action="store_true", help="start server")
     parser.add_argument("-j", "--join-server", nargs="?", const="", type=str, help="join server")
     parser.add_argument("-hc", "--headless", action="store_true", help="start headess client")
 
     parser.add_argument("-p", "--profile", default="", type=str, help="profile name")
```

### Comparing `armaqdl-0.6.1/armaqdl/config.py` & `armaqdl-0.7.0/armaqdl/config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.6.1/armaqdl/update.py` & `armaqdl-0.7.0/armaqdl/update.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.6.1/config/settings.toml` & `armaqdl-0.7.0/config/settings.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Default profile to use with ArmaQDL
 profile = "Dev"
 
 # Predefined locations of mods to be used with CLI as `location:@mod`
 # Alternatively use full absolute paths to `@mod` folders with the CLI
 [locations]
   # Every location contains a path and a build flag determining if mods from that folder should be rebuild with the `-b` CLI flag
-  # Use forward slahes `/` in paths
+  # Every location may contain a type ("dev" [default], "build" or "release") determining the HEMTT build to load by default
+  #   HEMTT builds will automatically load if `.hemttout` folder is present and non-HEMTT build is not forced
+  # Use forward slashes `/` in paths
 
   [locations.main]
     path = "C:/Program Files (x86)/Steam/steamapps/common/Arma 3"
     build = false
 
   [locations.workshop]
     path = "C:/Program Files (x86)/Steam/steamapps/common/Arma 3/!Workshop"
@@ -18,23 +20,24 @@
   [locations.dev]
     path = "C:/Arma 3/Mods"
     build = true
 
   [locations.p]
     path = "P:/"
     build = true
+    type = "build"  # Load HEMTT build from `.hemttout/build/` by default instead, if available, otherwise from `addons/`
 
 # Build tools and their instructions
 [build]
   # Every build tool contains presence marker (a file) determining if a tool can be used and the invocation command
   # Order defines priority if project supports multiple build tools
 
   [build.hemtt]
-    presence = "hemtt.toml"
-    command = ["hemtt", "build"]
+    presence = ".hemtt/project.toml"
+    command = ["hemtt", "dev"]
 
   [build.mikero]
     presence = "tools/build.py"
     command = ["python", "tools/build.py"]
 
   [build.make]
     presence = "Makefile"
```

### Comparing `armaqdl-0.6.1/tests/test_commands.py` & `armaqdl-0.7.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.6.1/tests/test_config.py` & `armaqdl-0.7.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `armaqdl-0.6.1/.gitignore` & `armaqdl-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `armaqdl-0.6.1/LICENSE` & `armaqdl-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `armaqdl-0.6.1/README.md` & `armaqdl-0.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: ArmaQDL
+Version: 0.7.0
+Summary: Python program for quick launching various mod development configurations for Arma through a simple CLI.
+Project-URL: Homepage, https://github.com/jonpas/Arma-QDL
+Project-URL: Bug Tracker, https://github.com/jonpas/Arma-QDL/issues
+Author-email: Jonpas <jonpas33@gmail.com>
+License-Expression: MIT
+License-File: LICENSE
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Python: >=3.7
+Requires-Dist: platformdirs
+Requires-Dist: toml
+Description-Content-Type: text/markdown
+
 # ArmaQDL
 
 [![CI - Test](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml)
 [![CI - Build](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/ArmaQDL.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/ArmaQDL)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ArmaQDL.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/ArmaQDL)
 
@@ -105,40 +129,63 @@
 ArmaQDL is a CLI script, view all the options with the `--help` flag.
 
 ```sh
 $ armaqdl -h
 ```
 _Note: All examples use `armaqdl` to launch ArmaQDL, replace it appropriately depending on your install._
 
-**Example 1:**
+**Example 1:** _(launching and building mods)_
 
 Launches Arma with CBA from main location, ACE3 from Workshop install and ACRE2 from local development folder. Additionally builds ACRE2 mod and opens the latest log file. Loads Arma directly into the editor using the specified mission from the "Soldier" profile.
 
 ```sh
-$ armaqdl main:x\cba workshop:@ace dev:acre2:b -m Soldier:test.vr
+$ armaqdl main:cba workshop:@ace dev:acre2:b -m Soldier:test.vr
 ```
 
 Specific build tool can also be specified, such as HEMTT.
 
 ```sh
-$ armaqdl main:x\cba workshop:@ace dev:acre2:bhemtt -m Soldier:test.vr
+$ armaqdl main:cba workshop:@ace dev:acre2:bhemtt -m Soldier:test.vr
 ```
 
-**Example 2:**
+**Example 2:** _(server and mission handling)_
 
 Launches Arma Server with CBA from local development folder and loads specified mission from default profile's missions folder, copying it to the server in the process.
 
 ```sh
-$ armaqdl dev:x\cba -m test.vr -s
+$ armaqdl dev:cba -m test.vr -s
 ```
 
 Launches Arma with CBA from local development folder and connects to the given server with the given password (`-j` defaults to the settings file).
 
 ```sh
-$ armaqdl dev:x\cba -j 192.168.1.1:2302:test
+$ armaqdl dev:cba -j 192.168.1.1:2302:test
+```
+
+**Example 3:** _(glob and skipping)_
+
+Launches Arma with all mods in a folder `modpack` from main location, skipping ACE3 in the same folder and instead loading ACE3 from a local development folder. This is useful for replacing a subset of mods from a bigger modpack.
+
+```sh
+$ armaqdl main:modpack\* main:modpack\ace:s dev:ace
+```
+
+**Example 4:** _(launch types)_
+
+Launches Arma with mods from local development folder, CBA using HEMTT release build, ACE3 using automatic launch type determination and ACRE2 using non-HEMTT build. Available launch types are `dev`, `build`, `release` for HEMTT or none for non-HEMTT `addons/`. Automatic determination uses HEMTT if `.hemttout` folder exists with launch type as specified in settings file, or `dev` if not specified.
+
+
+```sh
+$ armaqdl dev:cba:trelease dev:ace dev:acre2:t
+```
+
+Build type for HEMTT can also be specified using the same flag in addition to build flag.
+
+```sh
+$ armaqdl dev:cba:bhemtt:trelease dev:ace:b:tbuild
 ```
 
 
 ## Development
 
 ArmaQDL uses [Hatchling](https://hatch.pypa.io/latest/) as a build backend and [flake8](https://flake8.pycqa.org/en/latest/) as a style guide.
```

### Comparing `armaqdl-0.6.1/pyproject.toml` & `armaqdl-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armaqdl-0.6.1/PKG-INFO` & `armaqdl-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: ArmaQDL
-Version: 0.6.1
-Summary: Python program for quick launching various mod development configurations for Arma through a simple CLI.
-Project-URL: Homepage, https://github.com/jonpas/Arma-QDL
-Project-URL: Bug Tracker, https://github.com/jonpas/Arma-QDL/issues
-Author-email: Jonpas <jonpas33@gmail.com>
-License-Expression: MIT
-License-File: LICENSE
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.7
-Requires-Dist: platformdirs
-Requires-Dist: toml
-Description-Content-Type: text/markdown
-
 # ArmaQDL
 
 [![CI - Test](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/test.yml)
 [![CI - Build](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml/badge.svg)](https://github.com/jonpas/ArmaQDL/actions/workflows/build.yml)
 [![PyPI - Version](https://img.shields.io/pypi/v/ArmaQDL.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/ArmaQDL)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ArmaQDL.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/ArmaQDL)
 
@@ -129,40 +105,63 @@
 ArmaQDL is a CLI script, view all the options with the `--help` flag.
 
 ```sh
 $ armaqdl -h
 ```
 _Note: All examples use `armaqdl` to launch ArmaQDL, replace it appropriately depending on your install._
 
-**Example 1:**
+**Example 1:** _(launching and building mods)_
 
 Launches Arma with CBA from main location, ACE3 from Workshop install and ACRE2 from local development folder. Additionally builds ACRE2 mod and opens the latest log file. Loads Arma directly into the editor using the specified mission from the "Soldier" profile.
 
 ```sh
-$ armaqdl main:x\cba workshop:@ace dev:acre2:b -m Soldier:test.vr
+$ armaqdl main:cba workshop:@ace dev:acre2:b -m Soldier:test.vr
 ```
 
 Specific build tool can also be specified, such as HEMTT.
 
 ```sh
-$ armaqdl main:x\cba workshop:@ace dev:acre2:bhemtt -m Soldier:test.vr
+$ armaqdl main:cba workshop:@ace dev:acre2:bhemtt -m Soldier:test.vr
 ```
 
-**Example 2:**
+**Example 2:** _(server and mission handling)_
 
 Launches Arma Server with CBA from local development folder and loads specified mission from default profile's missions folder, copying it to the server in the process.
 
 ```sh
-$ armaqdl dev:x\cba -m test.vr -s
+$ armaqdl dev:cba -m test.vr -s
 ```
 
 Launches Arma with CBA from local development folder and connects to the given server with the given password (`-j` defaults to the settings file).
 
 ```sh
-$ armaqdl dev:x\cba -j 192.168.1.1:2302:test
+$ armaqdl dev:cba -j 192.168.1.1:2302:test
+```
+
+**Example 3:** _(glob and skipping)_
+
+Launches Arma with all mods in a folder `modpack` from main location, skipping ACE3 in the same folder and instead loading ACE3 from a local development folder. This is useful for replacing a subset of mods from a bigger modpack.
+
+```sh
+$ armaqdl main:modpack\* main:modpack\ace:s dev:ace
+```
+
+**Example 4:** _(launch types)_
+
+Launches Arma with mods from local development folder, CBA using HEMTT release build, ACE3 using automatic launch type determination and ACRE2 using non-HEMTT build. Available launch types are `dev`, `build`, `release` for HEMTT or none for non-HEMTT `addons/`. Automatic determination uses HEMTT if `.hemttout` folder exists with launch type as specified in settings file, or `dev` if not specified.
+
+
+```sh
+$ armaqdl dev:cba:trelease dev:ace dev:acre2:t
+```
+
+Build type for HEMTT can also be specified using the same flag in addition to build flag.
+
+```sh
+$ armaqdl dev:cba:bhemtt:trelease dev:ace:b:tbuild
 ```
 
 
 ## Development
 
 ArmaQDL uses [Hatchling](https://hatch.pypa.io/latest/) as a build backend and [flake8](https://flake8.pycqa.org/en/latest/) as a style guide.
```

