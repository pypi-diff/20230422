# Comparing `tmp/cli2-2.5.4.tar.gz` & `tmp/cli2-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cli2-2.5.4.tar", last modified: Wed Jul 27 21:54:12 2022, max compression
+gzip compressed data, was "cli2-2.6.0.tar", last modified: Fri Apr 21 22:28:26 2023, max compression
```

## Comparing `cli2-2.5.4.tar` & `cli2-2.6.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 21:54:12.539699 cli2-2.5.4/
--rw-rw-rw-   0 root         (0) root         (0)      161 2022-07-27 21:45:20.000000 cli2-2.5.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2965 2022-07-27 21:54:12.539699 cli2-2.5.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2134 2022-07-27 21:45:20.000000 cli2-2.5.4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      303 2022-07-27 21:45:20.000000 cli2-2.5.4/classifiers.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 21:54:12.536366 cli2-2.5.4/cli2/
--rw-rw-rw-   0 root         (0) root         (0)      213 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11550 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/argument.py
--rw-rw-rw-   0 root         (0) root         (0)     1118 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/colors.py
--rw-rw-rw-   0 root         (0) root         (0)     5840 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/command.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     1546 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/entry_point.py
--rw-rw-rw-   0 root         (0) root         (0)     5653 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/group.py
--rw-rw-rw-   0 root         (0) root         (0)     2697 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/node.py
--rw-rw-rw-   0 root         (0) root         (0)     4855 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/table.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/test.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    11396 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/test_command.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/test_entrypoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/test_group.py
--rw-rw-rw-   0 root         (0) root         (0)     2551 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2589 2022-07-27 21:45:20.000000 cli2-2.5.4/cli2/test_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-27 21:54:12.539699 cli2-2.5.4/cli2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2965 2022-07-27 21:54:12.000000 cli2-2.5.4/cli2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      529 2022-07-27 21:54:12.000000 cli2-2.5.4/cli2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-27 21:54:12.000000 cli2-2.5.4/cli2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2022-07-27 21:54:12.000000 cli2-2.5.4/cli2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       60 2022-07-27 21:54:12.000000 cli2-2.5.4/cli2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-07-27 21:54:12.000000 cli2-2.5.4/cli2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-27 21:54:12.539699 cli2-2.5.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      607 2022-07-27 21:54:11.000000 cli2-2.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 22:28:26.778579 cli2-2.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-21 18:09:22.000000 cli2-2.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-04-21 22:28:26.778579 cli2-2.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2023-04-21 18:09:22.000000 cli2-2.6.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-04-21 18:09:22.000000 cli2-2.6.0/classifiers.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 22:28:26.775245 cli2-2.6.0/cli2/
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11933 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/argument.py
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5840 2023-04-21 19:16:37.000000 cli2-2.6.0/cli2/command.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1554 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/entry_point.py
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/group.py
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/node.py
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    11376 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/test_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test_entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2023-04-21 21:55:13.000000 cli2-2.6.0/cli2/test_inject.py
+-rw-rw-rw-   0 root         (0) root         (0)     2551 2023-04-21 18:09:22.000000 cli2-2.6.0/cli2/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-04-21 21:56:13.000000 cli2-2.6.0/cli2/test_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 22:28:26.778579 cli2-2.6.0/cli2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      549 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-21 22:28:26.000000 cli2-2.6.0/cli2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 22:28:26.778579 cli2-2.6.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      607 2023-04-21 22:28:26.000000 cli2-2.6.0/setup.py
```

### Comparing `cli2-2.5.4/PKG-INFO` & `cli2-2.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 Metadata-Version: 2.1
 Name: cli2
-Version: 2.5.4
+Version: 2.6.0
 Summary: image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
 Home-page: https://yourlabs.io/oss/cli2
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
-Description: .. image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
-           :target: https://yourlabs.io/oss/cli2/pipelines
-        .. image:: https://codecov.io/gh/yourlabs/cli2/branch/master/graph/badge.svg
-          :target: https://codecov.io/gh/yourlabs/cli2
-        .. image:: https://img.shields.io/pypi/v/cli2.svg
-           :target: https://pypi.python.org/pypi/cli2
-        
-        cli2: Dynamic CLI for Python 3
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Expose Python functions or objects with a minimalist argument typing style, or
-        building your own command try during runtime.
-        
-        `Documentation available on RTFD
-        <https://cli2.rtfd.io>`_.
-        
-        Demo
-        ====
-        
-        cli2 is a little library to build CLIs, which documentation is `available on
-        RTFD <https://cli2.readthedocs.io/en/latest/>`_, but it comes with its own demo
-        command that may as well be useful to explore Python libraries and call
-        functions on the fly.
-        
-        Because, initially, cli2 was supposed to just bring Python callables on the CLI
-        without even a single line of code::
-        
-            cli2 path.to.your.callable arg1 kwarg1=value
-        
-        This command was implemented again in this 10th rewrite of the CLI engine
-        extracted from Playlabs, however this implementation features something pretty
-        funny: cli2 is a Group subclass which overrides the default Group
-        implementation based on the first argument passed on the command line.
-        
-        Basically, when you call ``cli2 path.to.module``, it will load a Group of name
-        ``path.to.module`` which whill load one Command per callable in
-        ``path.to.module``.
-        
-        When you call ``cli2 path.to.function`` it will execute the function.
-        
-        As a result, these three commands are strictly equivalent::
-        
-            cli2 cli2.test_node.example_function foo=bar
-            cli2 cli2.test_node example_function foo=bar
-        
-        That is because cli2 generates a group with every member of the previous group!
-        
-        See for yourself with::
-        
-            cli2 help cli2.test_node
-        
-        Or just::
-        
-            cli2 cli2.test_node
-        
-        Because cli2.test_node is not a callable but a module, cli2's cli2 CLI created
-        a command Group on the fly with the module and added every callable member as
-        command.
-        
-        When you call a group on the command line, it displays help by default to drive
-        the user.
 Keywords: cli
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: test
+
+.. image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
+   :target: https://yourlabs.io/oss/cli2/pipelines
+.. image:: https://codecov.io/gh/yourlabs/cli2/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/yourlabs/cli2
+.. image:: https://img.shields.io/pypi/v/cli2.svg
+   :target: https://pypi.python.org/pypi/cli2
+
+cli2: Dynamic CLI for Python 3
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Expose Python functions or objects with a minimalist argument typing style, or
+building your own command try during runtime.
+
+`Documentation available on RTFD
+<https://cli2.rtfd.io>`_.
+
+Demo
+====
+
+cli2 is a little library to build CLIs, which documentation is `available on
+RTFD <https://cli2.readthedocs.io/en/latest/>`_, but it comes with its own demo
+command that may as well be useful to explore Python libraries and call
+functions on the fly.
+
+Because, initially, cli2 was supposed to just bring Python callables on the CLI
+without even a single line of code::
+
+    cli2 path.to.your.callable arg1 kwarg1=value
+
+This command was implemented again in this 10th rewrite of the CLI engine
+extracted from Playlabs, however this implementation features something pretty
+funny: cli2 is a Group subclass which overrides the default Group
+implementation based on the first argument passed on the command line.
+
+Basically, when you call ``cli2 path.to.module``, it will load a Group of name
+``path.to.module`` which whill load one Command per callable in
+``path.to.module``.
+
+When you call ``cli2 path.to.function`` it will execute the function.
+
+As a result, these three commands are strictly equivalent::
+
+    cli2 cli2.test_node.example_function foo=bar
+    cli2 cli2.test_node example_function foo=bar
+
+That is because cli2 generates a group with every member of the previous group!
+
+See for yourself with::
+
+    cli2 help cli2.test_node
+
+Or just::
+
+    cli2 cli2.test_node
+
+Because cli2.test_node is not a callable but a module, cli2's cli2 CLI created
+a command Group on the fly with the module and added every callable member as
+command.
+
+When you call a group on the command line, it displays help by default to drive
+the user.
```

### Comparing `cli2-2.5.4/README.rst` & `cli2-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `cli2-2.5.4/cli2/argument.py` & `cli2-2.6.0/cli2/argument.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 
 class Argument:
     """
     Class representing a bound parameter and command line argument.
     """
     # TODO: why not split this into a bunch of simpler sub-classes now that
     # it's pretty featureful ?
-    def __init__(self, cmd, param, doc=None, color=None, default=None):
+    def __init__(self, cmd, param, doc=None, color=None, **kwargs):
         self.cmd = cmd
         self.param = param
         self.color = color
-        self.default = default
+        # Let default be set to None :)
+        self.default = kwargs.pop('default', param.default)
 
         self.doc = doc or ''
         if not doc:
             for _param in cmd.parsed.params:
                 if _param.arg_name == self.param.name:
                     self.doc = _param.description.replace('\n', ' ')
                     break
@@ -163,15 +164,18 @@
             out = ''
             for negate in self.negates:
                 out += colors.orange + negate + colors.reset
                 out += colors.reset
                 out += ' '
             self.cmd.print(out)
 
-        if self.default or self.param.default != self.param.empty:
+        if (
+            self.default != self.param.empty
+            or self.param.default != self.param.empty
+        ):
             self.cmd.print(
                 'Default: '
                 + colors.blue3
                 + str(self.default or self.param.default)
                 + colors.reset
             )
 
@@ -222,19 +226,27 @@
                 self.param.VAR_KEYWORD,
             )
         )
 
     @property
     def value(self):
         """Return the value bound to this argument."""
-        return self.cmd.bound.arguments[self.param.name]
+        try:
+            return self.cmd.bound.arguments[self.param.name]
+        except KeyError:
+            if self.default != self.param.empty:
+                return self.default
+            raise
 
     @value.setter
     def value(self, value):
-        if self.param.kind == self.param.VAR_POSITIONAL:
+        if value == self.param.empty:
+            # the getter will return the default or raise
+            return
+        elif self.param.kind == self.param.VAR_POSITIONAL:
             self.cmd.bound.arguments.setdefault(self.param.name, [])
             self.cmd.bound.arguments[self.param.name].append(value)
         elif self.param.kind == self.param.VAR_KEYWORD:
             self.cmd.bound.arguments.setdefault(self.param.name, {})
             parts = value.split('=')
             name = parts[0]
             if self.cmd.posix:
```

### Comparing `cli2-2.5.4/cli2/cli.py` & `cli2-2.6.0/cli2/cli.py`

 * *Files identical despite different names*

### Comparing `cli2-2.5.4/cli2/colors.py` & `cli2-2.6.0/cli2/colors.py`

 * *Files identical despite different names*

### Comparing `cli2-2.5.4/cli2/command.py` & `cli2-2.6.0/cli2/command.py`

 * *Files identical despite different names*

### Comparing `cli2-2.5.4/cli2/entry_point.py` & `cli2-2.6.0/cli2/entry_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             )
 
         result = self(*args[1:])
         if result is not None:
             if isinstance(result, (list, tuple)):
                 try:
                     table = Table.factory(*result)
-                except:
+                except:  # noqa
                     print(result)
                 else:
                     table.print()
             else:
                 print(result)
         sys.exit(self.exit_code)
```

### Comparing `cli2-2.5.4/cli2/group.py` & `cli2-2.6.0/cli2/group.py`

 * *Files identical despite different names*

### Comparing `cli2-2.5.4/cli2/node.py` & `cli2-2.6.0/cli2/node.py`

 * *Files identical despite different names*

### Comparing `cli2-2.5.4/cli2/table.py` & `cli2-2.6.0/cli2/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Table module for cli2.
 
 This Table module behaves like a list, and is pretty simple. Its purpose is to
-tabulate data and it's going to brute force output sizes until it finds a match.
+tabulate data and it's going to brute force output sizes until it finds a
+match.
 
 As such, it's not a good module to display really a lot of data because it
 sacrifies performance for human readability.
 """
 
 import os
 import textwrap
@@ -33,15 +34,14 @@
     def __init__(self, *args):
         super().__init__(args)
 
     @classmethod
     def factory(cls, *items):
         self = cls()
         first = True
-        keys = None
         kind = None
         for item in items:
             if not kind:
                 kind = type(item)
             elif kind != type(item):
                 raise Exception('Data contains different types')
 
@@ -65,20 +65,20 @@
                     columns.append(column)
                 else:
                     column = columns[colnum]
 
                 data = item
 
                 if isinstance(data, (list, tuple)):
-                    color = data[0]
                     data = data[1]
                 else:
-                    color = ''
                     data = item
 
+                data = str(data)
+
                 minlength = max(
                     [len(word) for word in data.split(' ')]
                 )
                 if minlength > column.minlength:
                     column.minlength = minlength
 
                 length = len(data)
@@ -103,15 +103,15 @@
         return columns
 
     def print(self, print_function=None, termsize=None):
         print_function = print_function or print
         if not termsize:
             try:
                 termsize = os.get_terminal_size().columns
-            except:
+            except:  # noqa
                 termsize = 80
         columns = self.calculate_columns(termsize=termsize)
 
         # separate columns with 2 spaces if possible
         if sumsize(columns) + (len(columns) - 1) * 2 <= termsize:
             numspaces = 2
         else:
@@ -126,14 +126,15 @@
                 data = row[colnum]
                 if isinstance(data, (list, tuple)):
                     color = data[0]
                     data = data[1]
                 else:
                     color = ''
                     data = row[colnum]
+                data = str(data)
 
                 wrapped = textwrap.wrap(data, column.maxlength)
                 words = wrapped[0] if wrapped else ''
                 if words == '=':
                     words = '=' * column.maxlength
                 line.append(words)
                 if colnum + 1 < len(columns):
```

### Comparing `cli2-2.5.4/cli2/test.py` & `cli2-2.6.0/cli2/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     if proc.stderr:
         fixture += '\n'.join([
             'stderr:',
             proc.stderr.decode('utf8'),
         ])
 
     for r in ignore or []:
-        fixture = re.compile(r).sub(f'redacted', fixture)
+        fixture = re.compile(r).sub('redacted', fixture)
 
     exists = os.path.exists(path)
     if REWRITE and exists:
         os.unlink(path)
         exists = False
 
     if not exists:
```

### Comparing `cli2-2.5.4/cli2/test_cli.py` & `cli2-2.6.0/cli2/test_cli.py`

 * *Files identical despite different names*

### Comparing `cli2-2.5.4/cli2/test_command.py` & `cli2-2.6.0/cli2/test_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,15 @@
 
 def test_keyword_only():
     def foo(*one, two=None): return (one, two)
     cmd = Command(foo)
 
     cmd.parse('x')
     assert cmd['one'].value == ['x']
-    with pytest.raises(KeyError):
-        cmd['two'].value
+    assert cmd['two'].value is None
 
 
 def test_bool():
     def foo(one: bool): return one
     cmd = Command(foo)
 
     cmd.parse('yes')
@@ -259,15 +258,15 @@
     cmd = Command(foo)
     cmd.parse('a=b=x')
     assert cmd['a'].value == 'b=x'
     assert cmd('a=b=x') == ('b=x', None)
 
 
 class Foo:
-    def __call__(self, a: int, b: list, c : bool = False, *d, e=None, **f):
+    def __call__(self, a: int, b: list, c: bool = False, *d, e=None, **f):
         self.a = a
         self.b = b
         self.c = c
         self.d = d
         self.e = e
         self.f = f
 
@@ -307,15 +306,15 @@
     cmd = Command(foo)
     cmd.parse('foo=bar')
     with pytest.raises(KeyError):
         cmd['missing'].value
 
 
 def test_kwargs_find_their_values():
-    def foo(*a, b: str='', c: str='', **d):
+    def foo(*a, b: str = '', c: str = '', **d):
         """docstring"""
     cmd = Command(foo)
     cmd.parse('c=3', 'e=5', '1', 'b=2')
     assert cmd['a'].value == ['1']
     assert cmd['b'].value == '2'
     assert cmd['c'].value == '3'
     assert cmd['d'].value == dict(e='5')
```

### Comparing `cli2-2.5.4/cli2/test_decorators.py` & `cli2-2.6.0/cli2/test_decorators.py`

 * *Files identical despite different names*

### Comparing `cli2-2.5.4/cli2/test_group.py` & `cli2-2.6.0/cli2/test_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,26 +95,26 @@
         """foodoc"""
     group = Group(posix=True)
     group.add(foo)
     assert group.posix
     assert group['foo'].posix
 
 
-class TestCmd(Command):
+class CommandSubject(Command):
     pass
 
 
 def example():
     pass
 
 
 def test_cmd_cls():
     group = Group()
-    group.cmd(cls=TestCmd)(example)
-    assert isinstance(group['example'], TestCmd)
+    group.cmd(cls=CommandSubject)(example)
+    assert isinstance(group['example'], CommandSubject)
 
 
 def test_group_cmdclass():
-    group = Group(cmdclass=TestCmd)
+    group = Group(cmdclass=CommandSubject)
     group.cmd()(example)
-    assert isinstance(group['example'], TestCmd)
-    assert not isinstance(group['help'], TestCmd)
+    assert isinstance(group['example'], CommandSubject)
+    assert not isinstance(group['help'], CommandSubject)
```

### Comparing `cli2-2.5.4/cli2/test_node.py` & `cli2-2.6.0/cli2/test_node.py`

 * *Files identical despite different names*

### Comparing `cli2-2.5.4/cli2/test_table.py` & `cli2-2.6.0/cli2/test_table.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import cli2
-import pytest
 import textwrap
 
 
 def test_calculate_columns():
-    table = cli2.Table(
+    table = cli2.Table(  # noqa
         ['a', 'b'],
         ['foo test', 'bar'],
     )
 
     # large term
-    columns =    table.calculate_columns(termsize=80)
+    columns = table.calculate_columns(termsize=80)
     assert columns[0].minlength == 4
     assert columns[0].maxlength == 8
     assert columns[1].minlength == 3
     assert columns[1].maxlength == 3
 
     # small term
     columns = table.calculate_columns(termsize=8)
@@ -116,7 +115,16 @@
     )
     assert_table_output(table, 18, '''
         a  b
         =  =
         1  2
         2  3
     ''')
+
+
+def test_nonstring():
+    table = cli2.Table(
+        [1, False],
+    )
+    assert_table_output(table, 9, '''
+        1  False
+    ''')
```

### Comparing `cli2-2.5.4/cli2.egg-info/PKG-INFO` & `cli2-2.6.0/cli2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 Metadata-Version: 2.1
 Name: cli2
-Version: 2.5.4
+Version: 2.6.0
 Summary: image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
 Home-page: https://yourlabs.io/oss/cli2
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
-Description: .. image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
-           :target: https://yourlabs.io/oss/cli2/pipelines
-        .. image:: https://codecov.io/gh/yourlabs/cli2/branch/master/graph/badge.svg
-          :target: https://codecov.io/gh/yourlabs/cli2
-        .. image:: https://img.shields.io/pypi/v/cli2.svg
-           :target: https://pypi.python.org/pypi/cli2
-        
-        cli2: Dynamic CLI for Python 3
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        Expose Python functions or objects with a minimalist argument typing style, or
-        building your own command try during runtime.
-        
-        `Documentation available on RTFD
-        <https://cli2.rtfd.io>`_.
-        
-        Demo
-        ====
-        
-        cli2 is a little library to build CLIs, which documentation is `available on
-        RTFD <https://cli2.readthedocs.io/en/latest/>`_, but it comes with its own demo
-        command that may as well be useful to explore Python libraries and call
-        functions on the fly.
-        
-        Because, initially, cli2 was supposed to just bring Python callables on the CLI
-        without even a single line of code::
-        
-            cli2 path.to.your.callable arg1 kwarg1=value
-        
-        This command was implemented again in this 10th rewrite of the CLI engine
-        extracted from Playlabs, however this implementation features something pretty
-        funny: cli2 is a Group subclass which overrides the default Group
-        implementation based on the first argument passed on the command line.
-        
-        Basically, when you call ``cli2 path.to.module``, it will load a Group of name
-        ``path.to.module`` which whill load one Command per callable in
-        ``path.to.module``.
-        
-        When you call ``cli2 path.to.function`` it will execute the function.
-        
-        As a result, these three commands are strictly equivalent::
-        
-            cli2 cli2.test_node.example_function foo=bar
-            cli2 cli2.test_node example_function foo=bar
-        
-        That is because cli2 generates a group with every member of the previous group!
-        
-        See for yourself with::
-        
-            cli2 help cli2.test_node
-        
-        Or just::
-        
-            cli2 cli2.test_node
-        
-        Because cli2.test_node is not a callable but a module, cli2's cli2 CLI created
-        a command Group on the fly with the module and added every callable member as
-        command.
-        
-        When you call a group on the command line, it displays help by default to drive
-        the user.
 Keywords: cli
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: test
+
+.. image:: https://yourlabs.io/oss/cli2/badges/master/pipeline.svg
+   :target: https://yourlabs.io/oss/cli2/pipelines
+.. image:: https://codecov.io/gh/yourlabs/cli2/branch/master/graph/badge.svg
+  :target: https://codecov.io/gh/yourlabs/cli2
+.. image:: https://img.shields.io/pypi/v/cli2.svg
+   :target: https://pypi.python.org/pypi/cli2
+
+cli2: Dynamic CLI for Python 3
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Expose Python functions or objects with a minimalist argument typing style, or
+building your own command try during runtime.
+
+`Documentation available on RTFD
+<https://cli2.rtfd.io>`_.
+
+Demo
+====
+
+cli2 is a little library to build CLIs, which documentation is `available on
+RTFD <https://cli2.readthedocs.io/en/latest/>`_, but it comes with its own demo
+command that may as well be useful to explore Python libraries and call
+functions on the fly.
+
+Because, initially, cli2 was supposed to just bring Python callables on the CLI
+without even a single line of code::
+
+    cli2 path.to.your.callable arg1 kwarg1=value
+
+This command was implemented again in this 10th rewrite of the CLI engine
+extracted from Playlabs, however this implementation features something pretty
+funny: cli2 is a Group subclass which overrides the default Group
+implementation based on the first argument passed on the command line.
+
+Basically, when you call ``cli2 path.to.module``, it will load a Group of name
+``path.to.module`` which whill load one Command per callable in
+``path.to.module``.
+
+When you call ``cli2 path.to.function`` it will execute the function.
+
+As a result, these three commands are strictly equivalent::
+
+    cli2 cli2.test_node.example_function foo=bar
+    cli2 cli2.test_node example_function foo=bar
+
+That is because cli2 generates a group with every member of the previous group!
+
+See for yourself with::
+
+    cli2 help cli2.test_node
+
+Or just::
+
+    cli2 cli2.test_node
+
+Because cli2.test_node is not a callable but a module, cli2's cli2 CLI created
+a command Group on the fly with the module and added every callable member as
+command.
+
+When you call a group on the command line, it displays help by default to drive
+the user.
```

### Comparing `cli2-2.5.4/cli2.egg-info/SOURCES.txt` & `cli2-2.6.0/cli2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 cli2/table.py
 cli2/test.py
 cli2/test_cli.py
 cli2/test_command.py
 cli2/test_decorators.py
 cli2/test_entrypoint.py
 cli2/test_group.py
+cli2/test_inject.py
 cli2/test_node.py
 cli2/test_table.py
 cli2.egg-info/PKG-INFO
 cli2.egg-info/SOURCES.txt
 cli2.egg-info/dependency_links.txt
 cli2.egg-info/entry_points.txt
 cli2.egg-info/requires.txt
```

### Comparing `cli2-2.5.4/setup.py` & `cli2-2.6.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='cli2',
-    version='2.5.4',
+    version='2.6.0',
     setup_requires='setupmeta',
     install_requires=['docstring_parser==0.7.1'],
     extras_require=dict(
         test=[
             'freezegun',
             'pytest',
             'pytest-cov',
```

