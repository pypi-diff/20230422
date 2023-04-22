# Comparing `tmp/wbpFilebrowser-0.1.4.tar.gz` & `tmp/wbpFilebrowser-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpFilebrowser-0.1.4.tar", last modified: Sun Feb 12 14:58:07 2023, max compression
+gzip compressed data, was "wbpFilebrowser-0.1.6.tar", last modified: Sat Apr 22 14:54:06 2023, max compression
```

## Comparing `wbpFilebrowser-0.1.4.tar` & `wbpFilebrowser-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-12 14:58:07.973469 wbpFilebrowser-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-02-12 14:58:06.000000 wbpFilebrowser-0.1.4/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-12 14:58:07.969468 wbpFilebrowser-0.1.4/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-12 14:58:07.971469 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser/
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-02-12 14:58:06.000000 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6619 2023-02-12 14:58:06.000000 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser/dirtreewindow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-12 14:58:07.973469 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1696 2023-02-12 14:58:07.000000 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      357 2023-02-12 14:58:07.000000 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-12 14:58:07.000000 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-02-12 14:58:07.000000 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-12 14:58:07.000000 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-02-12 14:58:07.000000 wbpFilebrowser-0.1.4/Lib/wbpFilebrowser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1696 2023-02-12 14:58:07.973469 wbpFilebrowser-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-02-12 14:58:06.000000 wbpFilebrowser-0.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2112 2023-02-12 14:58:07.974469 wbpFilebrowser-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-02-12 14:58:06.000000 wbpFilebrowser-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 14:54:06.207555 wbpFilebrowser-0.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 14:54:06.202555 wbpFilebrowser-0.1.6/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 14:54:06.204555 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser/
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6619 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser/dirtreewindow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 14:54:06.206555 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-22 14:54:06.000000 wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-04-22 14:54:06.207555 wbpFilebrowser-0.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2138 2023-04-22 14:54:06.208555 wbpFilebrowser-0.1.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-22 14:54:04.000000 wbpFilebrowser-0.1.6/setup.py
```

### Comparing `wbpFilebrowser-0.1.4/LICENSE` & `wbpFilebrowser-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpFilebrowser-0.1.4/Lib/wbpFilebrowser/dirtreewindow.py` & `wbpFilebrowser-0.1.6/Lib/wbpFilebrowser/dirtreewindow.py`

 * *Files identical despite different names*

### Comparing `wbpFilebrowser-0.1.4/Lib/wbpFilebrowser.egg-info/PKG-INFO` & `wbpFilebrowser-0.1.6/Lib/wbpFilebrowser.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wbpFilebrowser
-Version: 0.1.4
-Summary: Log list panel panel for Workbench applications.
+Version: 0.1.6
+Summary: File browser panel panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
-Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpFilebrowser/
+Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfilebrowser/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
 Classifier: Development Status :: 3 - Alpha
@@ -18,31 +18,42 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpFilebrowser
 
-Filebrowser plugin for Workbench applications
+Filebrowser plugin for [Workbench](https://pypi.org/project/wbBase/) applications
 
 ## Installation
 
 ```shell
 pip install wbpFilebrowser
 ```
 
+Installing this plugin registers an entry point 
+in the group "*wbbase.plugin*" named "*filebrowser*".
+
+To use the plugin in your application, 
+add it to your *application.yml* file as follows:
+```yaml
+AppName: myApp
+Plugins:
+- Name: filebrowser
+```
+
 ## Documentation
 
 For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpfilebrowser/).
```

### Comparing `wbpFilebrowser-0.1.4/PKG-INFO` & `wbpFilebrowser-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: wbpFilebrowser
-Version: 0.1.4
-Summary: Log list panel panel for Workbench applications.
+Version: 0.1.6
+Summary: File browser panel panel for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
-Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpFilebrowser/
+Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpfilebrowser/
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser/-/issues
 Keywords: workbench,wxPython,GUI
 Platform: WIN32
 Platform: WIN64
 Platform: OSX
 Platform: POSIX
 Classifier: Development Status :: 3 - Alpha
@@ -18,31 +18,42 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Environment :: MacOS X :: Cocoa
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wbpFilebrowser
 
-Filebrowser plugin for Workbench applications
+Filebrowser plugin for [Workbench](https://pypi.org/project/wbBase/) applications
 
 ## Installation
 
 ```shell
 pip install wbpFilebrowser
 ```
 
+Installing this plugin registers an entry point 
+in the group "*wbbase.plugin*" named "*filebrowser*".
+
+To use the plugin in your application, 
+add it to your *application.yml* file as follows:
+```yaml
+AppName: myApp
+Plugins:
+- Name: filebrowser
+```
+
 ## Documentation
 
 For details read the [Documentation](https://workbench2.gitlab.io/workbench-plugins/wbpfilebrowser/).
```

### Comparing `wbpFilebrowser-0.1.4/setup.cfg` & `wbpFilebrowser-0.1.6/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [bumpversion]
-current_version = 0.1.4
+current_version = 0.1.6
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
 
 [metadata]
 name = wbpFilebrowser
 version = attr: wbpFilebrowser.__version__
 author = Andreas Eigendorf
-description = Log list panel panel for Workbench applications.
+description = File browser panel panel for Workbench applications.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_files = LICENSE
 url = https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
 project_urls = 
 	Source = https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser
-	Documentation = https://workbench2.gitlab.io/workbench-plugins/wbpFilebrowser/
+	Documentation = https://workbench2.gitlab.io/workbench-plugins/wbpfilebrowser/
 	Tracker = https://gitlab.com/workbench2/workbench-plugins/wbpFilebrowser/-/issues
 platforms = 
 	WIN32
 	WIN64
 	OSX
 	POSIX
 keywords = 
@@ -36,44 +36,43 @@
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Environment :: MacOS X :: Cocoa
 	Environment :: Win32 (MS Windows)
 	Environment :: X11 Applications :: GTK
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: Implementation :: CPython
 	Intended Audience :: Developers
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: User Interfaces
 
 [options]
 package_dir = 
 	=Lib
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8,<3.11
 install_requires = 
-	wbBase>=0.1.46
+	wbBase>=0.1.53
 
 [options.packages.find]
 where = Lib
 
 [options.entry_points]
 wbbase.plugin = filebrowser = wbpFilebrowser
 
 [bumpversion:file:Lib/wbpFilebrowser/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
 
 [tox:tox]
-min_version = 4.3
+min_version = 4.4
 env_list = 
-	py37
 	py38
 	py39
 	py310
 
 [testenv]
 deps = 
 	pytest
```

