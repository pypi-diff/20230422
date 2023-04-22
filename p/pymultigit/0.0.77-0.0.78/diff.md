# Comparing `tmp/pymultigit-0.0.77.tar.gz` & `tmp/pymultigit-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultigit-0.0.77.tar", last modified: Tue Nov  1 13:25:00 2022, max compression
+gzip compressed data, was "pymultigit-0.0.78.tar", last modified: Sat Apr 22 12:29:23 2023, max compression
```

## Comparing `pymultigit-0.0.77.tar` & `pymultigit-0.0.78.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-11-01 13:25:00.950497 pymultigit-0.0.77/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2022-11-01 13:24:51.000000 pymultigit-0.0.77/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1395 2022-11-01 13:25:00.950497 pymultigit-0.0.77/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      421 2022-11-01 13:24:49.000000 pymultigit-0.0.77/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-11-01 13:25:00.950497 pymultigit-0.0.77/pymultigit/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-06-13 04:34:03.000000 pymultigit-0.0.77/pymultigit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2193 2022-10-29 11:23:32.000000 pymultigit-0.0.77/pymultigit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     9128 2022-11-01 13:24:24.000000 pymultigit-0.0.77/pymultigit/core.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5084 2022-10-18 09:51:06.000000 pymultigit-0.0.77/pymultigit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      196 2022-11-01 13:24:49.000000 pymultigit-0.0.77/pymultigit/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-11-01 13:25:00.950497 pymultigit-0.0.77/pymultigit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1395 2022-11-01 13:25:00.000000 pymultigit-0.0.77/pymultigit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      347 2022-11-01 13:25:00.000000 pymultigit-0.0.77/pymultigit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-11-01 13:25:00.000000 pymultigit-0.0.77/pymultigit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       53 2022-11-01 13:25:00.000000 pymultigit-0.0.77/pymultigit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       47 2022-11-01 13:25:00.000000 pymultigit-0.0.77/pymultigit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       11 2022-11-01 13:25:00.000000 pymultigit-0.0.77/pymultigit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2022-11-01 13:25:00.950497 pymultigit-0.0.77/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1612 2022-11-01 13:24:49.000000 pymultigit-0.0.77/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-22 12:29:23.590953 pymultigit-0.0.78/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-22 12:29:16.000000 pymultigit-0.0.78/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1399 2023-04-22 12:29:23.590953 pymultigit-0.0.78/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      427 2023-04-22 12:29:16.000000 pymultigit-0.0.78/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-22 12:29:23.589953 pymultigit-0.0.78/pymultigit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:38:18.000000 pymultigit-0.0.78/pymultigit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2338 2023-04-22 12:29:03.000000 pymultigit-0.0.78/pymultigit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     9277 2023-04-22 12:28:30.000000 pymultigit-0.0.78/pymultigit/core.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5084 2022-10-17 03:51:11.000000 pymultigit-0.0.78/pymultigit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      196 2023-04-22 12:29:16.000000 pymultigit-0.0.78/pymultigit/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-22 12:29:23.590953 pymultigit-0.0.78/pymultigit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1399 2023-04-22 12:29:23.000000 pymultigit-0.0.78/pymultigit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      347 2023-04-22 12:29:23.000000 pymultigit-0.0.78/pymultigit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-22 12:29:23.000000 pymultigit-0.0.78/pymultigit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       52 2023-04-22 12:29:23.000000 pymultigit-0.0.78/pymultigit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       47 2023-04-22 12:29:23.000000 pymultigit-0.0.78/pymultigit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       11 2023-04-22 12:29:23.000000 pymultigit-0.0.78/pymultigit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-22 12:29:23.590953 pymultigit-0.0.78/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1612 2023-04-22 12:29:16.000000 pymultigit-0.0.78/setup.py
```

### Comparing `pymultigit-0.0.77/LICENSE` & `pymultigit-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.77/PKG-INFO` & `pymultigit-0.0.78/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pymultigit
-Version: 0.0.77
+Version: 0.0.78
 Summary: Help you deal with multiple git repositories
 Home-page: https://veltzer.github.io/pymultigit
+Download-URL: https://github.com/veltzer/pymultigit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pymultigit
 Keywords: git,python,repositories,multiple
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -35,12 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pymultigit
 
 author: Mark Veltzer
 
-version: 0.0.77
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022
-
+version: 0.0.78
 
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pymultigit-0.0.77/pymultigit/configs.py` & `pymultigit-0.0.78/pymultigit/configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         help_string="what list of folders to use?",
         default=[],
     )
     stop = ParamCreator.create_bool(
         help_string="Stop when failing?",
         default=True,
     )
+    print_no_projects = ParamCreator.create_bool(
+        help_string="Print a message when no projects are found?",
+        default=True,
+    )
 
 
 class ConfigGrep(Config):
     """
     Parameters for the grep command
     """
```

### Comparing `pymultigit-0.0.77/pymultigit/core.py` & `pymultigit-0.0.78/pymultigit/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,24 +87,28 @@
 
 def print_projects_that_return_data(fnc) -> None:
     """
     In this function we are sure that the directories we get a real git folders
     since we get them from the `projects` function. There is no need to check this.
     """
     orig_dir = os.getcwd()
+    have_projects = False
     for project_dir in projects(sort=ConfigMain.sort):
+        have_projects = True
         os.chdir(project_dir)
         data = fnc()
         if data is not None:
             if ConfigOutput.terse:
                 print(project_dir)
             else:
                 print(f"project [{project_dir}]...")
                 print(data, end="")
         os.chdir(orig_dir)
+    if ConfigMain.print_no_projects and not have_projects:
+        print("no projects found")
 
 
 def is_dirty(repo) -> bool:
     return repo.is_dirty()
 
 
 def has_untracked_files(repo) -> bool:
```

### Comparing `pymultigit-0.0.77/pymultigit/main.py` & `pymultigit-0.0.78/pymultigit/main.py`

 * *Files identical despite different names*

### Comparing `pymultigit-0.0.77/pymultigit.egg-info/PKG-INFO` & `pymultigit-0.0.78/pymultigit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pymultigit
-Version: 0.0.77
+Version: 0.0.78
 Summary: Help you deal with multiple git repositories
 Home-page: https://veltzer.github.io/pymultigit
+Download-URL: https://github.com/veltzer/pymultigit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
-Download-URL: https://github.com/veltzer/pymultigit
 Keywords: git,python,repositories,multiple
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -35,12 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pymultigit
 
 author: Mark Veltzer
 
-version: 0.0.77
-
-	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022
-
+version: 0.0.78
 
+	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pymultigit-0.0.77/setup.py` & `pymultigit-0.0.78/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,55 +5,55 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pymultigit",
-    version="0.0.77",
+    version="0.0.78",
     packages=[
-        'pymultigit',
+        "pymultigit",
     ],
     # from here all is optional
     description="Help you deal with multiple git repositories",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
     author="Mark Veltzer",
     author_email="mark.veltzer@gmail.com",
     maintainer="Mark Veltzer",
     maintainer_email="mark.veltzer@gmail.com",
     keywords=[
-        'git',
-        'python',
-        'repositories',
-        'multiple',
+        "git",
+        "python",
+        "repositories",
+        "multiple",
     ],
     url="https://veltzer.github.io/pymultigit",
     download_url="https://github.com/veltzer/pymultigit",
     license="MIT",
     platforms=[
-        'python3',
+        "python3",
     ],
     install_requires=[
-        'gitpython',
-        'pyfakeuse',
-        'pytconf',
-        'pylogconf',
-        'venv-run',
+        "gitpython",
+        "pyfakeuse",
+        "pytconf",
+        "pylogconf",
+        "venv-run",
     ],
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Environment :: Console',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Topic :: Utilities',
-        'License :: OSI Approved :: MIT License',
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Utilities",
+        "License :: OSI Approved :: MIT License",
     ],
     entry_points={"console_scripts": [
-        'pymultigit=pymultigit.main:main',
+        "pymultigit=pymultigit.main:main",
     ]},
 )
```

