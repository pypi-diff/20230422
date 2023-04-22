# Comparing `tmp/argcomplete-3.0.5.tar.gz` & `tmp/argcomplete-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argcomplete-3.0.5.tar", last modified: Sun Mar 26 05:56:51 2023, max compression
+gzip compressed data, was "argcomplete-3.0.6.tar", last modified: Sat Apr 22 14:30:58 2023, max compression
```

## Comparing `argcomplete-3.0.5.tar` & `argcomplete-3.0.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-03-26 05:56:51.589738 argcomplete-3.0.5/
--rw-r--r--   0 kislyuk    (501) staff       (20)       35 2016-06-14 14:20:26.000000 argcomplete-3.0.5/Authors.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    12020 2023-03-26 05:56:32.000000 argcomplete-3.0.5/Changes.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)    10174 2016-06-14 14:20:26.000000 argcomplete-3.0.5/LICENSE.rst
--rw-r--r--   0 kislyuk    (501) staff       (20)       79 2022-08-21 15:59:43.000000 argcomplete-3.0.5/MANIFEST.in
--rw-r--r--   0 kislyuk    (501) staff       (20)      387 2023-03-21 02:49:58.000000 argcomplete-3.0.5/NOTICE
--rw-r--r--   0 kislyuk    (501) staff       (20)    17221 2023-03-26 05:56:51.589819 argcomplete-3.0.5/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)    15614 2023-03-26 05:56:01.000000 argcomplete-3.0.5/README.rst
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-03-26 05:56:51.586981 argcomplete-3.0.5/argcomplete/
--rw-r--r--   0 kislyuk    (501) staff       (20)      693 2023-03-21 02:49:58.000000 argcomplete-3.0.5/argcomplete/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2140 2023-03-05 19:47:13.000000 argcomplete-3.0.5/argcomplete/_check_console_script.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2600 2023-03-18 19:32:22.000000 argcomplete-3.0.5/argcomplete/_check_module.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-03-26 05:56:51.587785 argcomplete-3.0.5/argcomplete/bash_completion.d/
--rw-r--r--   0 kislyuk    (501) staff       (20)     5422 2023-03-26 00:26:25.000000 argcomplete-3.0.5/argcomplete/bash_completion.d/python-argcomplete
--rw-r--r--   0 kislyuk    (501) staff       (20)     3980 2023-03-26 05:10:17.000000 argcomplete-3.0.5/argcomplete/completers.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      112 2023-03-19 18:35:55.000000 argcomplete-3.0.5/argcomplete/exceptions.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    26975 2023-03-26 04:57:44.000000 argcomplete-3.0.5/argcomplete/finders.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      866 2023-03-19 18:46:34.000000 argcomplete-3.0.5/argcomplete/io.py
--rw-r--r--   0 kislyuk    (501) staff       (20)     2131 2023-03-21 02:49:58.000000 argcomplete-3.0.5/argcomplete/lexers.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-03-26 05:56:51.588077 argcomplete-3.0.5/argcomplete/packages/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-19 10:11:13.000000 argcomplete-3.0.5/argcomplete/packages/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    15846 2023-03-19 18:59:55.000000 argcomplete-3.0.5/argcomplete/packages/_argparse.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    12766 2023-03-18 19:32:22.000000 argcomplete-3.0.5/argcomplete/packages/_shlex.py
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-18 19:32:22.000000 argcomplete-3.0.5/argcomplete/py.typed
--rw-r--r--   0 kislyuk    (501) staff       (20)     6965 2023-03-20 05:09:51.000000 argcomplete-3.0.5/argcomplete/shell_integration.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-03-26 05:56:51.587672 argcomplete-3.0.5/argcomplete.egg-info/
--rw-r--r--   0 kislyuk    (501) staff       (20)    17221 2023-03-26 05:56:51.000000 argcomplete-3.0.5/argcomplete.egg-info/PKG-INFO
--rw-r--r--   0 kislyuk    (501) staff       (20)     1091 2023-03-26 05:56:51.000000 argcomplete-3.0.5/argcomplete.egg-info/SOURCES.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-03-26 05:56:51.000000 argcomplete-3.0.5/argcomplete.egg-info/dependency_links.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-03-26 05:56:42.000000 argcomplete-3.0.5/argcomplete.egg-info/not-zip-safe
--rw-r--r--   0 kislyuk    (501) staff       (20)      153 2023-03-26 05:56:51.000000 argcomplete-3.0.5/argcomplete.egg-info/requires.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)       12 2023-03-26 05:56:51.000000 argcomplete-3.0.5/argcomplete.egg-info/top_level.txt
--rw-r--r--   0 kislyuk    (501) staff       (20)      371 2023-03-26 00:37:29.000000 argcomplete-3.0.5/pyproject.toml
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-03-26 05:56:51.588411 argcomplete-3.0.5/scripts/
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     3374 2023-03-26 00:26:25.000000 argcomplete-3.0.5/scripts/activate-global-python-argcomplete
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2609 2023-03-19 01:09:49.000000 argcomplete-3.0.5/scripts/python-argcomplete-check-easy-install-script
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1957 2023-03-19 08:36:11.000000 argcomplete-3.0.5/scripts/register-python-argcomplete
--rw-r--r--   0 kislyuk    (501) staff       (20)      143 2023-03-26 05:56:51.590349 argcomplete-3.0.5/setup.cfg
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     2403 2023-03-26 05:56:11.000000 argcomplete-3.0.5/setup.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-03-26 05:56:51.589233 argcomplete-3.0.5/test/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-06-14 14:20:26.000000 argcomplete-3.0.5/test/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      139 2016-06-16 15:02:13.000000 argcomplete-3.0.5/test/__init__.pyc
--rw-r--r--   0 kislyuk    (501) staff       (20)       31 2023-03-05 19:47:13.000000 argcomplete-3.0.5/test/inputrc
--rwxr-xr-x   0 kislyuk    (501) staff       (20)     1765 2022-09-14 03:21:59.000000 argcomplete-3.0.5/test/prog
--rwxr-xr-x   0 kislyuk    (501) staff       (20)    56755 2023-03-26 05:56:05.000000 argcomplete-3.0.5/test/test.py
--rw-r--r--   0 kislyuk    (501) staff       (20)    31570 2016-10-16 02:47:39.000000 argcomplete-3.0.5/test/test.pyc
--rw-r--r--   0 kislyuk    (501) staff       (20)     3183 2023-03-18 19:32:22.000000 argcomplete-3.0.5/test/test_contrib_shells.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-03-26 05:56:51.589535 argcomplete-3.0.5/test/test_package/
--rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-05 19:47:13.000000 argcomplete-3.0.5/test/test_package/__init__.py
--rw-r--r--   0 kislyuk    (501) staff       (20)      299 2022-09-14 03:21:59.000000 argcomplete-3.0.5/test/test_package/setup.py
--rw-r--r--   0 kislyuk    (501) staff       (20)       94 2022-09-14 03:21:59.000000 argcomplete-3.0.5/test/test_package/test_module.py
-drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-03-26 05:56:51.589639 argcomplete-3.0.5/test/test_package/test_package/
--rw-r--r--   0 kislyuk    (501) staff       (20)      289 2022-09-14 03:21:59.000000 argcomplete-3.0.5/test/test_package/test_package/__init__.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.418194 argcomplete-3.0.6/
+-rw-r--r--   0 kislyuk    (501) staff       (20)       35 2016-06-14 14:20:26.000000 argcomplete-3.0.6/Authors.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)    12286 2023-04-22 14:30:41.000000 argcomplete-3.0.6/Changes.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)    10174 2016-06-14 14:20:26.000000 argcomplete-3.0.6/LICENSE.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)       79 2022-08-21 15:59:43.000000 argcomplete-3.0.6/MANIFEST.in
+-rw-r--r--   0 kislyuk    (501) staff       (20)      387 2023-03-21 02:49:58.000000 argcomplete-3.0.6/NOTICE
+-rw-r--r--   0 kislyuk    (501) staff       (20)    16463 2023-04-22 14:30:58.418271 argcomplete-3.0.6/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)    14856 2023-04-22 14:28:37.000000 argcomplete-3.0.6/README.rst
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.413428 argcomplete-3.0.6/argcomplete/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      693 2023-03-21 02:49:58.000000 argcomplete-3.0.6/argcomplete/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2140 2023-03-05 19:47:13.000000 argcomplete-3.0.6/argcomplete/_check_console_script.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2600 2023-03-18 19:32:22.000000 argcomplete-3.0.6/argcomplete/_check_module.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.414283 argcomplete-3.0.6/argcomplete/bash_completion.d/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     5422 2023-03-26 00:26:25.000000 argcomplete-3.0.6/argcomplete/bash_completion.d/python-argcomplete
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3980 2023-03-26 15:30:13.000000 argcomplete-3.0.6/argcomplete/completers.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      112 2023-03-19 18:35:55.000000 argcomplete-3.0.6/argcomplete/exceptions.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    26975 2023-03-26 15:30:13.000000 argcomplete-3.0.6/argcomplete/finders.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      866 2023-03-19 18:46:34.000000 argcomplete-3.0.6/argcomplete/io.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2131 2023-03-21 02:49:58.000000 argcomplete-3.0.6/argcomplete/lexers.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.414998 argcomplete-3.0.6/argcomplete/packages/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-19 10:11:13.000000 argcomplete-3.0.6/argcomplete/packages/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    15846 2023-03-19 18:59:55.000000 argcomplete-3.0.6/argcomplete/packages/_argparse.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    12766 2023-03-18 19:32:22.000000 argcomplete-3.0.6/argcomplete/packages/_shlex.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-18 19:32:22.000000 argcomplete-3.0.6/argcomplete/py.typed
+-rw-r--r--   0 kislyuk    (501) staff       (20)     7012 2023-04-22 14:28:37.000000 argcomplete-3.0.6/argcomplete/shell_integration.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.414176 argcomplete-3.0.6/argcomplete.egg-info/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    16463 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1091 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-22 14:30:49.000000 argcomplete-3.0.6/argcomplete.egg-info/not-zip-safe
+-rw-r--r--   0 kislyuk    (501) staff       (20)      153 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/requires.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)       12 2023-04-22 14:30:58.000000 argcomplete-3.0.6/argcomplete.egg-info/top_level.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)      371 2023-03-26 00:37:29.000000 argcomplete-3.0.6/pyproject.toml
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.415741 argcomplete-3.0.6/scripts/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     3374 2023-03-26 00:26:25.000000 argcomplete-3.0.6/scripts/activate-global-python-argcomplete
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     2609 2023-03-19 01:09:49.000000 argcomplete-3.0.6/scripts/python-argcomplete-check-easy-install-script
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1997 2023-04-22 14:28:37.000000 argcomplete-3.0.6/scripts/register-python-argcomplete
+-rw-r--r--   0 kislyuk    (501) staff       (20)      143 2023-04-22 14:30:58.418541 argcomplete-3.0.6/setup.cfg
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     2403 2023-04-22 14:29:05.000000 argcomplete-3.0.6/setup.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.417409 argcomplete-3.0.6/test/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2016-06-14 14:20:26.000000 argcomplete-3.0.6/test/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      139 2016-06-16 15:02:13.000000 argcomplete-3.0.6/test/__init__.pyc
+-rw-r--r--   0 kislyuk    (501) staff       (20)       31 2023-03-05 19:47:13.000000 argcomplete-3.0.6/test/inputrc
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1765 2022-09-14 03:21:59.000000 argcomplete-3.0.6/test/prog
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)    59328 2023-04-22 14:28:37.000000 argcomplete-3.0.6/test/test.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    31570 2016-10-16 02:47:39.000000 argcomplete-3.0.6/test/test.pyc
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3183 2023-03-18 19:32:22.000000 argcomplete-3.0.6/test/test_contrib_shells.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.417895 argcomplete-3.0.6/test/test_package/
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2023-03-05 19:47:13.000000 argcomplete-3.0.6/test/test_package/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      299 2022-09-14 03:21:59.000000 argcomplete-3.0.6/test/test_package/setup.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)       94 2022-09-14 03:21:59.000000 argcomplete-3.0.6/test/test_package/test_module.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-22 14:30:58.418068 argcomplete-3.0.6/test/test_package/test_package/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      289 2022-09-14 03:21:59.000000 argcomplete-3.0.6/test/test_package/test_package/__init__.py
```

### Comparing `argcomplete-3.0.5/Changes.rst` & `argcomplete-3.0.6/Changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Changes for v3.0.6 (2023-04-22)
+===============================
+
+-  Allow importlib-metadata 6.x; skip test failures on Python 3.7 (#420,
+   #424)
+
+-  Note completers can return iterables of strings, not just lists
+   (#422)
+
+-  Documentation and test improvements
+
 Changes for v3.0.5 (2023-03-25)
 ===============================
 
 -  Call \_default as fallback in zsh global completion hook
 
 -  Begin support for mapping-emitting completers
```

### Comparing `argcomplete-3.0.5/LICENSE.rst` & `argcomplete-3.0.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/PKG-INFO` & `argcomplete-3.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.0.5
+Version: 3.0.6
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
@@ -56,15 +56,15 @@
 ::
 
     pip install argcomplete
     activate-global-python-argcomplete
 
 On Linux, you will need to run the second command with ``sudo``. See `Activating global completion`_ below for details.
 
-Refresh your shell environment (start a new shell or ``source /etc/profile``).
+Refresh your shell environment (start a new shell).
 
 Synopsis
 --------
 Add the ``PYTHON_ARGCOMPLETE_OK`` marker and a call to ``argcomplete.autocomplete()`` to your Python application as
 follows:
 
 .. code-block:: python
@@ -116,16 +116,17 @@
 * ``prefix``: The prefix text of the last word before the cursor on the command line.
   For dynamic completers, this can be used to reduce the work required to generate possible completions.
 * ``action``: The ``argparse.Action`` instance that this completer was called for.
 * ``parser``: The ``argparse.ArgumentParser`` instance that the action was taken by.
 * ``parsed_args``: The result of argument parsing so far (the ``argparse.Namespace`` args object normally returned by
   ``ArgumentParser.parse_args()``).
 
-Completers should return their completions as a list of strings. An example completer for names of environment
-variables might look like this:
+Completers can return their completions as an iterable of strings or a mapping (dict) of strings to their
+descriptions (zsh will display the descriptions as context help alongside completions). An example completer for names
+of environment variables might look like this:
 
 .. code-block:: python
 
     def EnvironCompleter(**kwargs):
         return os.environ
 
 To specify a completer for an argument or option, set the ``completer`` attribute of its associated action. An easy
@@ -284,34 +285,23 @@
 Zsh Support
 -----------
 Argcomplete supports zsh. On top of plain completions like in bash, zsh allows you to see argparse help strings as
 completion descriptions. All shellcode included with argcomplete is compatible with both bash and zsh, so the same
 completer commands ``activate-global-python-argcomplete`` and ``eval "$(register-python-argcomplete my-python-app)"``
 work for zsh as well.
 
-External argcomplete script
----------------------------
-To register an argcomplete script for an arbitrary name, the ``--external-argcomplete-script`` argument of the ``register-python-argcomplete`` script can be used::
-
-    eval "$(register-python-argcomplete --external-argcomplete-script /path/to/script arbitrary-name)"
-
-This allows, for example, to use the auto completion functionality of argcomplete for an application not written in Python. 
-The command line interface of this program must be additionally implemented in a Python script with argparse and argcomplete and whenever the application is called the registered external argcomplete script is used for auto completion.
-
-This option can also be used in combination with the other supported shells.
-
 Python Support
 --------------
 Argcomplete requires Python 3.7+.
 
 Support for other shells
 ------------------------
 Argcomplete maintainers provide support only for the bash and zsh shells on Linux and MacOS. For resources related to
-other shells and platforms, please see the `contrib <https://github.com/kislyuk/argcomplete/tree/develop/contrib>`_
-directory.
+other shells and platforms, including fish, tcsh, xonsh, powershell, and Windows, please see the
+`contrib <https://github.com/kislyuk/argcomplete/tree/develop/contrib>`_ directory.
 
 Common Problems
 ---------------
 If global completion is not completing your script, bash may have registered a default completion function::
 
     $ complete | grep my-python-app
     complete -F _minimal my-python-app
@@ -332,15 +322,14 @@
 
 Links
 -----
 * `Project home page (GitHub) <https://github.com/kislyuk/argcomplete>`_
 * `Documentation <https://kislyuk.github.io/argcomplete/>`_
 * `Package distribution (PyPI) <https://pypi.python.org/pypi/argcomplete>`_
 * `Change log <https://github.com/kislyuk/argcomplete/blob/master/Changes.rst>`_
-* `xontrib-argcomplete <https://github.com/anki-code/xontrib-argcomplete>`_ - support argcomplete in `xonsh <https://github.com/xonsh/xonsh>`_ shell
 
 Bugs
 ~~~~
 Please report bugs, issues, feature requests, etc. on `GitHub <https://github.com/kislyuk/argcomplete/issues>`_.
 
 License
 -------
```

### Comparing `argcomplete-3.0.5/README.rst` & `argcomplete-3.0.6/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ::
 
     pip install argcomplete
     activate-global-python-argcomplete
 
 On Linux, you will need to run the second command with ``sudo``. See `Activating global completion`_ below for details.
 
-Refresh your shell environment (start a new shell or ``source /etc/profile``).
+Refresh your shell environment (start a new shell).
 
 Synopsis
 --------
 Add the ``PYTHON_ARGCOMPLETE_OK`` marker and a call to ``argcomplete.autocomplete()`` to your Python application as
 follows:
 
 .. code-block:: python
@@ -78,16 +78,17 @@
 * ``prefix``: The prefix text of the last word before the cursor on the command line.
   For dynamic completers, this can be used to reduce the work required to generate possible completions.
 * ``action``: The ``argparse.Action`` instance that this completer was called for.
 * ``parser``: The ``argparse.ArgumentParser`` instance that the action was taken by.
 * ``parsed_args``: The result of argument parsing so far (the ``argparse.Namespace`` args object normally returned by
   ``ArgumentParser.parse_args()``).
 
-Completers should return their completions as a list of strings. An example completer for names of environment
-variables might look like this:
+Completers can return their completions as an iterable of strings or a mapping (dict) of strings to their
+descriptions (zsh will display the descriptions as context help alongside completions). An example completer for names
+of environment variables might look like this:
 
 .. code-block:: python
 
     def EnvironCompleter(**kwargs):
         return os.environ
 
 To specify a completer for an argument or option, set the ``completer`` attribute of its associated action. An easy
@@ -246,34 +247,23 @@
 Zsh Support
 -----------
 Argcomplete supports zsh. On top of plain completions like in bash, zsh allows you to see argparse help strings as
 completion descriptions. All shellcode included with argcomplete is compatible with both bash and zsh, so the same
 completer commands ``activate-global-python-argcomplete`` and ``eval "$(register-python-argcomplete my-python-app)"``
 work for zsh as well.
 
-External argcomplete script
----------------------------
-To register an argcomplete script for an arbitrary name, the ``--external-argcomplete-script`` argument of the ``register-python-argcomplete`` script can be used::
-
-    eval "$(register-python-argcomplete --external-argcomplete-script /path/to/script arbitrary-name)"
-
-This allows, for example, to use the auto completion functionality of argcomplete for an application not written in Python. 
-The command line interface of this program must be additionally implemented in a Python script with argparse and argcomplete and whenever the application is called the registered external argcomplete script is used for auto completion.
-
-This option can also be used in combination with the other supported shells.
-
 Python Support
 --------------
 Argcomplete requires Python 3.7+.
 
 Support for other shells
 ------------------------
 Argcomplete maintainers provide support only for the bash and zsh shells on Linux and MacOS. For resources related to
-other shells and platforms, please see the `contrib <https://github.com/kislyuk/argcomplete/tree/develop/contrib>`_
-directory.
+other shells and platforms, including fish, tcsh, xonsh, powershell, and Windows, please see the
+`contrib <https://github.com/kislyuk/argcomplete/tree/develop/contrib>`_ directory.
 
 Common Problems
 ---------------
 If global completion is not completing your script, bash may have registered a default completion function::
 
     $ complete | grep my-python-app
     complete -F _minimal my-python-app
@@ -294,15 +284,14 @@
 
 Links
 -----
 * `Project home page (GitHub) <https://github.com/kislyuk/argcomplete>`_
 * `Documentation <https://kislyuk.github.io/argcomplete/>`_
 * `Package distribution (PyPI) <https://pypi.python.org/pypi/argcomplete>`_
 * `Change log <https://github.com/kislyuk/argcomplete/blob/master/Changes.rst>`_
-* `xontrib-argcomplete <https://github.com/anki-code/xontrib-argcomplete>`_ - support argcomplete in `xonsh <https://github.com/xonsh/xonsh>`_ shell
 
 Bugs
 ~~~~
 Please report bugs, issues, feature requests, etc. on `GitHub <https://github.com/kislyuk/argcomplete/issues>`_.
 
 License
 -------
```

### Comparing `argcomplete-3.0.5/argcomplete/__init__.py` & `argcomplete-3.0.6/argcomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/_check_console_script.py` & `argcomplete-3.0.6/argcomplete/_check_console_script.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/_check_module.py` & `argcomplete-3.0.6/argcomplete/_check_module.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/bash_completion.d/python-argcomplete` & `argcomplete-3.0.6/argcomplete/bash_completion.d/python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/completers.py` & `argcomplete-3.0.6/argcomplete/completers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/finders.py` & `argcomplete-3.0.6/argcomplete/finders.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/io.py` & `argcomplete-3.0.6/argcomplete/io.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/lexers.py` & `argcomplete-3.0.6/argcomplete/lexers.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/packages/_argparse.py` & `argcomplete-3.0.6/argcomplete/packages/_argparse.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/packages/_shlex.py` & `argcomplete-3.0.6/argcomplete/packages/_shlex.py`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/argcomplete/shell_integration.py` & `argcomplete-3.0.6/argcomplete/shell_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,17 +119,18 @@
 
 
 def shellcode(executables, use_defaults=True, shell="bash", complete_arguments=None, argcomplete_script=None):
     """
     Provide the shell code required to register a python executable for use with the argcomplete module.
 
     :param list(str) executables: Executables to be completed (when invoked exactly with this name)
-    :param bool use_defaults: Whether to fallback to readline's default completion when no matches are generated.
+    :param bool use_defaults: Whether to fallback to readline's default completion when no matches are generated
+        (affects bash only)
     :param str shell: Name of the shell to output code for
-    :param complete_arguments: Arguments to call complete with
+    :param complete_arguments: Arguments to call complete with (affects bash only)
     :type complete_arguments: list(str) or None
     :param argcomplete_script: Script to call complete with, if not the executable to complete.
         If supplied, will be used to complete *all* passed executables.
     :type argcomplete_script: str or None
     """
 
     if complete_arguments is None:
```

### Comparing `argcomplete-3.0.5/argcomplete.egg-info/PKG-INFO` & `argcomplete-3.0.6/argcomplete.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argcomplete
-Version: 3.0.5
+Version: 3.0.6
 Summary: Bash tab completion for argparse
 Home-page: https://github.com/kislyuk/argcomplete
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Project-URL: Documentation, https://kislyuk.github.io/argcomplete
 Project-URL: Source Code, https://github.com/kislyuk/argcomplete
@@ -56,15 +56,15 @@
 ::
 
     pip install argcomplete
     activate-global-python-argcomplete
 
 On Linux, you will need to run the second command with ``sudo``. See `Activating global completion`_ below for details.
 
-Refresh your shell environment (start a new shell or ``source /etc/profile``).
+Refresh your shell environment (start a new shell).
 
 Synopsis
 --------
 Add the ``PYTHON_ARGCOMPLETE_OK`` marker and a call to ``argcomplete.autocomplete()`` to your Python application as
 follows:
 
 .. code-block:: python
@@ -116,16 +116,17 @@
 * ``prefix``: The prefix text of the last word before the cursor on the command line.
   For dynamic completers, this can be used to reduce the work required to generate possible completions.
 * ``action``: The ``argparse.Action`` instance that this completer was called for.
 * ``parser``: The ``argparse.ArgumentParser`` instance that the action was taken by.
 * ``parsed_args``: The result of argument parsing so far (the ``argparse.Namespace`` args object normally returned by
   ``ArgumentParser.parse_args()``).
 
-Completers should return their completions as a list of strings. An example completer for names of environment
-variables might look like this:
+Completers can return their completions as an iterable of strings or a mapping (dict) of strings to their
+descriptions (zsh will display the descriptions as context help alongside completions). An example completer for names
+of environment variables might look like this:
 
 .. code-block:: python
 
     def EnvironCompleter(**kwargs):
         return os.environ
 
 To specify a completer for an argument or option, set the ``completer`` attribute of its associated action. An easy
@@ -284,34 +285,23 @@
 Zsh Support
 -----------
 Argcomplete supports zsh. On top of plain completions like in bash, zsh allows you to see argparse help strings as
 completion descriptions. All shellcode included with argcomplete is compatible with both bash and zsh, so the same
 completer commands ``activate-global-python-argcomplete`` and ``eval "$(register-python-argcomplete my-python-app)"``
 work for zsh as well.
 
-External argcomplete script
----------------------------
-To register an argcomplete script for an arbitrary name, the ``--external-argcomplete-script`` argument of the ``register-python-argcomplete`` script can be used::
-
-    eval "$(register-python-argcomplete --external-argcomplete-script /path/to/script arbitrary-name)"
-
-This allows, for example, to use the auto completion functionality of argcomplete for an application not written in Python. 
-The command line interface of this program must be additionally implemented in a Python script with argparse and argcomplete and whenever the application is called the registered external argcomplete script is used for auto completion.
-
-This option can also be used in combination with the other supported shells.
-
 Python Support
 --------------
 Argcomplete requires Python 3.7+.
 
 Support for other shells
 ------------------------
 Argcomplete maintainers provide support only for the bash and zsh shells on Linux and MacOS. For resources related to
-other shells and platforms, please see the `contrib <https://github.com/kislyuk/argcomplete/tree/develop/contrib>`_
-directory.
+other shells and platforms, including fish, tcsh, xonsh, powershell, and Windows, please see the
+`contrib <https://github.com/kislyuk/argcomplete/tree/develop/contrib>`_ directory.
 
 Common Problems
 ---------------
 If global completion is not completing your script, bash may have registered a default completion function::
 
     $ complete | grep my-python-app
     complete -F _minimal my-python-app
@@ -332,15 +322,14 @@
 
 Links
 -----
 * `Project home page (GitHub) <https://github.com/kislyuk/argcomplete>`_
 * `Documentation <https://kislyuk.github.io/argcomplete/>`_
 * `Package distribution (PyPI) <https://pypi.python.org/pypi/argcomplete>`_
 * `Change log <https://github.com/kislyuk/argcomplete/blob/master/Changes.rst>`_
-* `xontrib-argcomplete <https://github.com/anki-code/xontrib-argcomplete>`_ - support argcomplete in `xonsh <https://github.com/xonsh/xonsh>`_ shell
 
 Bugs
 ~~~~
 Please report bugs, issues, feature requests, etc. on `GitHub <https://github.com/kislyuk/argcomplete/issues>`_.
 
 License
 -------
```

### Comparing `argcomplete-3.0.5/argcomplete.egg-info/SOURCES.txt` & `argcomplete-3.0.6/argcomplete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/scripts/activate-global-python-argcomplete` & `argcomplete-3.0.6/scripts/activate-global-python-argcomplete`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/scripts/python-argcomplete-check-easy-install-script` & `argcomplete-3.0.6/scripts/python-argcomplete-check-easy-install-script`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/scripts/register-python-argcomplete` & `argcomplete-3.0.6/scripts/register-python-argcomplete`

 * *Files 7% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 parser = argparse.ArgumentParser(description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter)
 
 parser.add_argument(
     "--no-defaults",
     dest="use_defaults",
     action="store_false",
     default=True,
-    help="When no matches are generated, do not fallback to readline's default completion",
+    help="when no matches are generated, do not fallback to readline's default completion (affects bash only)",
 )
 parser.add_argument(
     "--complete-arguments",
     nargs=argparse.REMAINDER,
-    help="arguments to call complete with; use of this option discards default options",
+    help="arguments to call complete with; use of this option discards default options (affects bash only)",
 )
 parser.add_argument(
     "-s",
     "--shell",
     choices=("bash", "zsh", "tcsh", "fish", "powershell"),
     default="bash",
     help="output code for the specified shell",
```

### Comparing `argcomplete-3.0.5/setup.py` & `argcomplete-3.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import glob
 
 from setuptools import find_packages, setup
 
 install_requires = []
 tests_require = ["coverage", "pexpect", "wheel", "ruff", "mypy"]
-importlib_backport_requires = ["importlib-metadata >= 0.23, < 6"]
+importlib_backport_requires = ["importlib-metadata >= 0.23, < 7"]
 
 setup(
     name="argcomplete",
-    version="3.0.5",
+    version="3.0.6",
     url="https://github.com/kislyuk/argcomplete",
     project_urls={
         "Documentation": "https://kislyuk.github.io/argcomplete",
         "Source Code": "https://github.com/kislyuk/argcomplete",
         "Issue Tracker": "https://github.com/kislyuk/argcomplete/issues",
         "Change Log": "https://github.com/kislyuk/argcomplete/blob/master/Changes.rst",
     },
```

### Comparing `argcomplete-3.0.5/test/prog` & `argcomplete-3.0.6/test/prog`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/test/test.py` & `argcomplete-3.0.6/test/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import subprocess
 import sys
 import unittest
 from io import StringIO
 from tempfile import NamedTemporaryFile, TemporaryFile, mkdtemp
 
 import pexpect
-import pexpect.replwrap
+from pexpect.replwrap import REPLWrapper, PEXPECT_PROMPT, PEXPECT_CONTINUATION_PROMPT
 
 TEST_DIR = os.path.abspath(os.path.dirname(__file__))
 BASE_DIR = os.path.dirname(TEST_DIR)
 sys.path.insert(0, BASE_DIR)
 
 from argparse import SUPPRESS, ArgumentParser  # noqa: E402
 
@@ -35,19 +35,55 @@
 IFS = "\013"
 COMP_WORDBREAKS = " \t\n\"'><=;|&(:"
 
 BASH_VERSION = subprocess.check_output(["bash", "-c", "echo $BASH_VERSION"]).decode()
 BASH_MAJOR_VERSION = int(BASH_VERSION.split(".")[0])
 
 
+class ArgcompleteREPLWrapper(REPLWrapper):
+    def run_command(self, command, **kwargs):
+        if "\n" in command:
+            raise Exception("newlines not supported in REPL input")
+        res = super().run_command(command, **kwargs)
+        if self.child.command.split("/")[-1] == "zsh":
+            if "\n" not in res:
+                raise Exception("Expected to see a newline in command response")
+            echo_cmd, actual_res = res.split("\n", 1)
+            actual_res = actual_res.replace("\x1b[0m\x1b[23m\x1b[24m\x1b[J", "")
+            return actual_res
+        else:
+            return res
+
+
+def _repl_sh(command, args, non_printable_insert):
+    os.environ["PS1"] = "$"
+    child = pexpect.spawn(command, args, echo=False, encoding="utf-8")
+    ps1 = PEXPECT_PROMPT[:5] + non_printable_insert + PEXPECT_PROMPT[5:]
+    ps2 = PEXPECT_CONTINUATION_PROMPT[:5] + non_printable_insert + PEXPECT_CONTINUATION_PROMPT[5:]
+    prompt_change = f"PS1='{ps1}' PS2='{ps2}' PROMPT_COMMAND=''"
+    return ArgcompleteREPLWrapper(child, "\\$", prompt_change, extra_init_cmd="export PAGER=cat")
+
+
+def bash_repl(command="bash"):
+    bashrc = os.path.join(os.path.dirname(pexpect.__file__), "replwrap", "bashrc.sh")
+    sh = _repl_sh(command, ["--rcfile", bashrc], non_printable_insert="\\[\\]")
+    return sh
+
+
+def zsh_repl(command="zsh"):
+    sh = _repl_sh(command, ["--no-rcs", "-V"], non_printable_insert="%(!..)")
+    sh.run_command("autoload compinit; compinit -u")
+    return sh
+
+
 def setUpModule():
-    os.environ['INPUTRC'] = os.path.join(os.path.dirname(__file__), 'inputrc')
+    os.environ["INPUTRC"] = os.path.join(os.path.dirname(__file__), "inputrc")
 
 
-class TempDir(object):
+class TempDir:
     """
     Temporary directory for testing FilesCompletion
 
     Usage:
 
         with TempDir(prefix="temp_fc") as t:
             print("tempdir", t)
@@ -1058,15 +1094,15 @@
             _check_module.find("module.bad")
         self.assertNotIn("module", sys.modules)
 
     def _mkfile(self, path):
         open(path, "w").close()
 
 
-class TestShellBase(object):
+class TestShellBase:
     """
     Contains tests which should work in any shell using argcomplete.
 
     Tests use the test program in this directory named ``prog``.
     All commands are expected to input one of the valid choices
     which is then printed and collected by the shell wrapper.
 
@@ -1197,42 +1233,48 @@
         self.assertEqual(self.sh.run_command("export POINT=1"), "")
         self.assertEqual(self.sh.run_command("prog point hi\t"), "13\r\n")
         self.assertEqual(self.sh.run_command("prog point hi \t"), "14\r\n")
         self.assertEqual(self.sh.run_command("prog point 你好嘚瑟\t"), "15\r\n")
         self.assertEqual(self.sh.run_command("prog point 你好嘚瑟 \t"), "16\r\n")
 
 
-class TestBash(TestShellBase, unittest.TestCase):
-    expected_failures = [
-        "test_parse_special_characters_dollar",
-        "test_exclamation_in_double_quotes",
-    ]
-    if BASH_MAJOR_VERSION < 4:
-        # This requires compopt which is not available in 3.x.
-        expected_failures.append("test_quoted_exact")
-
+class TestBashZshBase(TestShellBase):
     # 'dummy' argument unused; checks multi-command registration works
     # by passing 'prog' as the second argument.
     install_cmd = 'eval "$(register-python-argcomplete dummy prog)"'
 
     def setUp(self):
-        sh = pexpect.replwrap.bash()
+        sh = self.repl_provider()
         path = ":".join([os.path.join(BASE_DIR, "scripts"), TEST_DIR, "$PATH"])
         sh.run_command("export PATH={0}".format(path))
         sh.run_command("export PYTHONPATH={0}".format(BASE_DIR))
-        # Disable the "python" module provided by bash-completion
-        sh.run_command("complete -r python python2 python3")
+        if self.repl_provider == bash_repl:
+            # Disable the "python" module provided by bash-completion
+            sh.run_command("complete -r python python2 python3")
         output = sh.run_command(self.install_cmd)
         self.assertEqual(output, "")
         # Register a dummy completion with an external argcomplete script
         # to ensure this doesn't overwrite our previous registration.
         output = sh.run_command('eval "$(register-python-argcomplete dummy --external-argcomplete-script dummy)"')
         self.assertEqual(output, "")
         self.sh = sh
 
+
+class TestBash(TestBashZshBase, unittest.TestCase):
+    expected_failures = [
+        "test_parse_special_characters_dollar",
+        "test_exclamation_in_double_quotes",
+    ]
+    if BASH_MAJOR_VERSION < 4:
+        # This requires compopt which is not available in 3.x.
+        expected_failures.append("test_quoted_exact")
+
+    def repl_provider(self):
+        return bash_repl()
+
     def test_one_space_after_exact(self):
         """Test exactly one space is appended after an exact match."""
         # Actual command run is 'echo "prog basic foo "'.
         result = self.sh.run_command('prog basic f\t"\1echo "')
         self.assertEqual(result, "prog basic foo \r\n")
 
     def test_debug_output(self):
@@ -1252,14 +1294,30 @@
         self.assertIn("Using output file ", output)
 
     def test_nounset(self):
         self.sh.run_command("set -o nounset")
         self.test_simple_completion()
 
 
+class TestZsh(TestBashZshBase, unittest.TestCase):
+    expected_failures = [
+        "test_parse_special_characters_dollar",
+        "test_comp_point",  # FIXME
+        "test_completion_environment",  # FIXME
+        "test_continuation",  # FIXME
+        "test_wordbreak_chars",  # FIXME
+    ]
+
+    def test_parse_special_characters(self):
+        pass  # FIXME: test crashes in teardown
+
+    def repl_provider(self):
+        return zsh_repl()
+
+
 @unittest.skipIf(BASH_MAJOR_VERSION < 4, "complete -D not supported")
 class TestBashGlobal(TestBash):
     install_cmd = 'eval "$(activate-global-python-argcomplete --dest=-)"'
 
     def test_python_completion(self):
         self.sh.run_command("cd " + TEST_DIR)
         self.assertEqual(self.sh.run_command("python3 ./prog basic f\t"), "foo\r\n")
@@ -1307,35 +1365,39 @@
             command = "test-module"
             if package:
                 command = "test-package"
             command += " a\t"
             self.assertEqual(self.sh.run_command(command), "arg\r\n")
 
     @unittest.skipIf(os.uname()[0] == "Darwin", "Skip test that fails on MacOS")
+    @unittest.skipIf(sys.version_info < (3, 8), "Skip test that fails on Python 3.7 with importlib_metadata > 4")
     def test_console_script_module(self):
         """Test completing a console_script for a module."""
         self._test_console_script()
 
     @unittest.skipIf(os.uname()[0] == "Darwin", "Skip test that fails on MacOS")
+    @unittest.skipIf(sys.version_info < (3, 8), "Skip test that fails on Python 3.7 with importlib_metadata > 4")
     def test_console_script_package(self):
         """Test completing a console_script for a package."""
         self._test_console_script(package=True)
 
     @unittest.skipIf(os.uname()[0] == "Darwin", "Skip test that fails on MacOS")
+    @unittest.skipIf(sys.version_info < (3, 8), "Skip test that fails on Python 3.7 with importlib_metadata > 4")
     def test_console_script_module_wheel(self):
         """Test completing a console_script for a module from a wheel."""
         self._test_console_script(wheel=True)
 
     @unittest.skipIf(os.uname()[0] == "Darwin", "Skip test that fails on MacOS")
+    @unittest.skipIf(sys.version_info < (3, 8), "Skip test that fails on Python 3.7 with importlib_metadata > 4")
     def test_console_script_package_wheel(self):
         """Test completing a console_script for a package from a wheel."""
         self._test_console_script(package=True, wheel=True)
 
 
-class Shell(object):
+class Shell:
     def __init__(self, shell):
         self.child = pexpect.spawn(shell, encoding="utf-8")
 
     def run_command(self, command):
         try:
             self.child.sendline(r"echo -n \#\#\#; {0}; echo -n \#\#\#".format(command))
             self.child.expect_exact("###", timeout=5)
```

### Comparing `argcomplete-3.0.5/test/test.pyc` & `argcomplete-3.0.6/test/test.pyc`

 * *Files identical despite different names*

### Comparing `argcomplete-3.0.5/test/test_contrib_shells.py` & `argcomplete-3.0.6/test/test_contrib_shells.py`

 * *Files identical despite different names*

