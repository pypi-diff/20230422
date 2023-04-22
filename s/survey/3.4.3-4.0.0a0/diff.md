# Comparing `tmp/survey-3.4.3.tar.gz` & `tmp/survey-4.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survey-3.4.3.tar", last modified: Fri Apr 23 18:49:18 2021, max compression
+gzip compressed data, was "survey-4.0.0a0.tar", last modified: Sat Apr 22 16:24:32 2023, max compression
```

## Comparing `survey-3.4.3.tar` & `survey-4.0.0a0.tar`

### file list

```diff
@@ -1,22 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-23 18:49:18.309480 survey-3.4.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2021-04-23 18:49:18.309480 survey-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      829 2021-04-23 18:49:09.000000 survey-3.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-23 18:49:18.313480 survey-3.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      643 2021-04-23 18:49:09.000000 survey-3.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-23 18:49:18.309480 survey-3.4.3/survey/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-04-23 18:49:09.000000 survey-3.4.3/survey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8737 2021-04-23 18:49:09.000000 survey-3.4.3/survey/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    26995 2021-04-23 18:49:09.000000 survey-3.4.3/survey/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3664 2021-04-23 18:49:09.000000 survey-3.4.3/survey/cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5115 2021-04-23 18:49:09.000000 survey-3.4.3/survey/display.py
--rw-r--r--   0 runner    (1001) docker     (121)     8642 2021-04-23 18:49:09.000000 survey-3.4.3/survey/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3654 2021-04-23 18:49:09.000000 survey-3.4.3/survey/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2021-04-23 18:49:09.000000 survey-3.4.3/survey/machines.py
--rw-r--r--   0 runner    (1001) docker     (121)      827 2021-04-23 18:49:09.000000 survey-3.4.3/survey/theme.py
--rw-r--r--   0 runner    (1001) docker     (121)    27136 2021-04-23 18:49:09.000000 survey-3.4.3/survey/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-23 18:49:18.309480 survey-3.4.3/survey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2021-04-23 18:49:18.000000 survey-3.4.3/survey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-04-23 18:49:18.000000 survey-3.4.3/survey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-23 18:49:18.000000 survey-3.4.3/survey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-04-23 18:49:18.000000 survey-3.4.3/survey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-23 18:49:18.000000 survey-3.4.3/survey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:24:32.496133 survey-4.0.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-22 16:24:17.000000 survey-4.0.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-22 16:24:32.496133 survey-4.0.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-22 16:24:17.000000 survey-4.0.0a0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 16:24:32.496133 survey-4.0.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-22 16:24:17.000000 survey-4.0.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:24:32.492133 survey-4.0.0a0/survey/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_controls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:24:32.496133 survey-4.0.0a0/survey/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_io_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_io_os_nt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_io_os_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_core/_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30907 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_funnels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18288 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_mutates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_printers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16758 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_searches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58488 2023-04-22 16:24:17.000000 survey-4.0.0a0/survey/_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 16:24:32.492133 survey-4.0.0a0/survey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-22 16:24:32.000000 survey-4.0.0a0/survey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-22 16:24:32.000000 survey-4.0.0a0/survey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 16:24:32.000000 survey-4.0.0a0/survey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-22 16:24:32.000000 survey-4.0.0a0/survey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-22 16:24:32.000000 survey-4.0.0a0/survey.egg-info/top_level.txt
```

### Comparing `survey-3.4.3/PKG-INFO` & `survey-4.0.0a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 3.4.3
+Version: 4.0.0a0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
-Description: ✨ A simple library for creating beautiful interactive prompts.
-        
-        .. image:: https://github.com/Exahilosys/survey/raw/master/images/showcase.gif
-        
-        Features
-        --------
-        
-        - **Pythonic**: Friendly interface wrapped around simple functions.
-        - **Lightweight**: Independent of any other prompt or visual libraries.
-        - **Adaptable**: Works with any string formatting and window size.
-        - **Extensive**: Packed with tweaks and features for any situation.
-        - **Complete**: Supports Windows 10 (Anniversary Update and up).
-        
-        Installing
-        ----------
-        
-        .. code-block::
-        
-            pip3 install survey
-        
-        Links
-        -----
-        
-        - Check out the `Quickstart <https://survey.readthedocs.io/quickstart.html>`_ guide for more.
-        - Greatly inspired by `AlecAivazis's GoLang <https://github.com/AlecAivazis/survey>`_ library.
-        
-        Suggestions and contributions are greatly appreciated!
-        
-Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.11
 Provides-Extra: docs
+License-File: LICENSE
+
+✨ A simple library for creating beautiful interactive prompts.
+
+.. image:: https://github.com/Exahilosys/survey/blob/main/docs/_static/images/showcase-1.gif?raw=true
+
+Features
+--------
+
+- **Pythonic**: Friendly interface built around simple functions.
+- **Lightweight**: No external depencencies for any operating system.
+- **Adaptable**: Works with any string formatting and window size.
+- **Extensive**: Packed with tweaks and features for any situation.
+- **Complete**: Supports Windows 10 (Anniversary Update and up).
+
+Installing
+----------
+
+.. code-block::
+
+    pip3 install survey
+
+Links
+-----
+
+- Check out the `Quickstart <https://survey.readthedocs.io/reference.html>`_ guide for more.
+- Greatly inspired by `AlecAivazis's GoLang <https://github.com/AlecAivazis/survey>`_ library.
+
+Suggestions and contributions are greatly appreciated!
```

### Comparing `survey-3.4.3/README.rst` & `survey-4.0.0a0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ✨ A simple library for creating beautiful interactive prompts.
 
-.. image:: https://github.com/Exahilosys/survey/raw/master/images/showcase.gif
+.. image:: https://github.com/Exahilosys/survey/blob/main/docs/_static/images/showcase-1.gif?raw=true
 
 Features
 --------
 
-- **Pythonic**: Friendly interface wrapped around simple functions.
-- **Lightweight**: Independent of any other prompt or visual libraries.
+- **Pythonic**: Friendly interface built around simple functions.
+- **Lightweight**: No external depencencies for any operating system.
 - **Adaptable**: Works with any string formatting and window size.
 - **Extensive**: Packed with tweaks and features for any situation.
 - **Complete**: Supports Windows 10 (Anniversary Update and up).
 
 Installing
 ----------
 
 .. code-block::
 
     pip3 install survey
 
 Links
 -----
 
-- Check out the `Quickstart <https://survey.readthedocs.io/quickstart.html>`_ guide for more.
+- Check out the `Quickstart <https://survey.readthedocs.io/reference.html>`_ guide for more.
 - Greatly inspired by `AlecAivazis's GoLang <https://github.com/AlecAivazis/survey>`_ library.
 
 Suggestions and contributions are greatly appreciated!
```

### Comparing `survey-3.4.3/setup.py` & `survey-4.0.0a0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import setuptools
 
 with open('README.rst') as file:
     readme = file.read()
 
-name = 'survey'
-
-version = '3.4.3'
-
 author = 'Exahilosys'
+project = 'survey'
+version = '4.0.0-alpha'
 
-url = 'https://github.com/{0}/{1}'.format(author, name)
+url = 'https://github.com/{0}/{1}'.format(author, project)
 
 setuptools.setup(
-    name = name,
-    python_requires = '>=3.5',
+    name = project,
+    python_requires = '>=3.11',
     version = version,
     url = url,
     packages = setuptools.find_packages(),
     license = 'MIT',
     description = 'A simple library for creating beautiful interactive prompts.',
     long_description = readme,
-    install_requires = [
-        'wrapio>=1.0.0'
-    ],
     extras_require = {
         'docs': [
             'sphinx',
-            'sphinx_rtd_theme'
+            'sphinx-rtd-theme',
+            'sphinx-paramlinks',
+            'sphinx-autodoc-typehints'
         ]
     }
-)
+)
```

### Comparing `survey-3.4.3/survey/io.py` & `survey-4.0.0a0/survey/_core/_io_os_nt.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,206 +1,129 @@
-import os
+import msvcrt
+import ctypes
+import ctypes.wintypes
 
-from . import helpers
+from . import _constants
+from . import _io_os
 
 
 __all__ = ('IO',)
 
 
-class BaseIO:
+_LINESEP = _constants.linesep.encode()
 
-    __slots__ = ('_i', '_o', '_buffer')
 
-    def __init__(self, i, o):
+def _recv_linesep(text):
 
-        self._i = i
-        self._o = o
+    return _LINESEP
 
-        self._buffer = []
 
-    def feed(self, data):
+def _recv_interrupt(text):
 
-        self._buffer.extend(data)
+    raise KeyboardInterrupt
 
-    def _send(self, value):
 
-        raise NotImplementedError()
+class IO(_io_os.StreamIO):
 
-    def send(self, value):
-
-        self._send(value)
-
-    def _recv(self):
-
-        raise NotImplementedError()
-
-    def recv(self):
-
-        try:
-            rune = self._buffer.pop(0)
-        except IndexError:
-            rune = self._recv()
-
-        return rune
-
-    def ring(self):
-
-
-        self._send('\a')
-
-
-class ModeIO(BaseIO):
-
-    __slots__ = ('_atomic', '_i_save', '_i_mode')
+    __slots__ = ('_i_fh', '_o_fh', '_o_save')
 
     def __init__(self, *args, **kwargs):
 
         super().__init__(*args, **kwargs)
 
-        self._atomic = helpers.Atomic(self.start, self.stop)
+        i_fd = self._i.fileno()
+        self._i_fh = msvcrt.get_osfhandle(i_fd)
 
-    @property
-    def atomic(self):
+        o_fd = self._o.fileno()
+        self._o_fh = msvcrt.get_osfhandle(o_fd)
 
-        return self._atomic
+    def _wait(self, mode, switch):
 
-    def _init(self):
-
-        raise NotImplementedError()
-
-    def _swap(self, mode):
-
-        raise NotImplementedError()
-
-    def start(self):
-
-        (self._i_save, mode) = self._init()
-
-        self._swap(mode)
+        bit = 2
 
-        self._i_mode = mode
+        if switch:
+            # - ENABLE_LINE_INPUT
+            mode &= ~ bit
+        else:
+            # + ENABLE_LINE_INPUT
+            mode |= bit
 
-    def stop(self):
+        return mode
 
-        self._swap(self._i_save)
+    @staticmethod
+    def _getm(fh):
 
-        self._i_save = None
+        c_mode = ctypes.wintypes.DWORD()
 
+        ctypes.windll.kernel32.GetConsoleMode(fh, ctypes.byref(c_mode))
 
-class StreamModeIO(ModeIO):
-
-    __slots__ = ()
-
-    def _send(self, value):
-
-        self._o.write(value)
-        self._o.flush()
-
-    def _recv(self):
-
-        rune = self._i.read(1)
+        mode = c_mode.value
 
-        return rune
+        return mode
 
-    def setup(self):
-
-        pass
-
-    def reset(self):
-
-        pass
-
-
-if os.name == 'nt':
-
-    import msvcrt
-    import ctypes
-    import ctypes.wintypes
-
-    _kernel32 = ctypes.windll.kernel32
-
-    class IO(StreamModeIO):
-
-        __slots__ = ('_i_fh', '_o_fh', '_o_save')
-
-        def __init__(self, *args, **kwargs):
-
-            super().__init__(*args, **kwargs)
-
-            i_fd = self._i.fileno()
-            self._i_fh = msvcrt.get_osfhandle(i_fd)
-
-            o_fd = self._o.fileno()
-            self._o_fh = msvcrt.get_osfhandle(o_fd)
-
-        def _getm(self, fh):
-
-            c_mode = ctypes.wintypes.DWORD()
-
-            _kernel32.GetConsoleMode(fh, ctypes.byref(c_mode))
-
-            mode = c_mode.value
-
-            return mode
-
-        def _init(self):
-
-            save = self._getm(self._i_fh)
-
-            mode = save &~ (2 | 4 | 32) | 512
-            # - (ENABLE_LINE_INPUT + ENABLE_ECHO_INPUT + ENABLE_INSERT_MODE)
-            # + ENABLE_VIRTUAL_TERMINAL_INPUT
-
-            return (save, mode)
-
-        def _setm(self, fh, mode):
+    def _init(self):
 
-            c_mode = ctypes.wintypes.DWORD(mode)
+        save = self._getm(self._i_fh)
 
-            _kernel32.SetConsoleMode(fh, c_mode)
+        # - ENABLE_PROCESSED_INPUT
+        # - ENABLE_ECHO_INPUT
+        # - ENABLE_INSERT_MODE
+        # + ENABLE_VIRTUAL_TERMINAL_INPUT
+        mode = save &~ (1 | 4 | 32) | 512
 
-        def _swap(self, mode):
+        return (save, mode)
 
-            self._setm(self._i_fh, mode)
+    @staticmethod
+    def _setm(fh, mode):
 
-        def setup(self):
+        c_mode = ctypes.wintypes.DWORD(mode)
 
-            mode = self._o_save = self._getm(self._o_fh)
+        ctypes.windll.kernel32.SetConsoleMode(fh, c_mode)
 
-            mode = mode | 1 | 4
-            # + ENABLE_PROCESSED_OUTPUT + ENABLE_VIRTUAL_TERMINAL_PROCESSING
+    def _set(self, mode):
 
-            self._setm(self._o_fh, mode)
+        self._setm(self._i_fh, mode)
 
-        def reset(self):
+    def _setup(self):
 
-            self._setm(self._o_fh, self._o_save)
+        mode = self._o_save = self._getm(self._o_fh)
 
-else:
+        # + ENABLE_PROCESSED_OUTPUT
+        # + ENABLE_VIRTUAL_TERMINAL_PROCESSING
+        mode = mode | 1 | 4
 
-    import termios
+        self._setm(self._o_fh, mode)
 
-    class IO(StreamModeIO):
+    def _reset(self):
 
-        __slots__ = ('_i_fd',)
+        self._setm(self._o_fh, self._o_save)
 
-        def __init__(self, *args, **kwargs):
+    _recv_replace = {
+        b'\r': _recv_linesep,
+        b'\x03': _recv_interrupt
+    }
 
-            super().__init__(*args, **kwargs)
+    def _recv(self):
 
-            self._i_fd = self._i.fileno()
+        text = super()._recv()
 
-        def _init(self):
+        while True:
+            try:
+                function = self._recv_replace[text]
+            except KeyError:
+                break
+            else:
+                text = function(text)
+        
+        return text
 
-            save = termios.tcgetattr(self._i_fd)
+    def __enter__(self, *args):
 
-            mode = termios.tcgetattr(self._i_fd)
+        self._setup()
 
-            mode[3] &= ~(termios.ECHO | termios.ECHONL | termios.ICANON)
-            mode[6][termios.VTIME] = 0
-            mode[6][termios.VMIN] = 1
+        return super().__enter__(*args)
 
-            return (save, mode)
+    def __exit__(self, *args):
 
-        def _swap(self, mode):
+        self._reset()
 
-            termios.tcsetattr(self._i_fd, termios.TCSAFLUSH, mode)
+        return super().__exit__(*args)
```

### Comparing `survey-3.4.3/survey.egg-info/PKG-INFO` & `survey-4.0.0a0/survey.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: survey
-Version: 3.4.3
+Version: 4.0.0a0
 Summary: A simple library for creating beautiful interactive prompts.
 Home-page: https://github.com/Exahilosys/survey
 License: MIT
-Description: ✨ A simple library for creating beautiful interactive prompts.
-        
-        .. image:: https://github.com/Exahilosys/survey/raw/master/images/showcase.gif
-        
-        Features
-        --------
-        
-        - **Pythonic**: Friendly interface wrapped around simple functions.
-        - **Lightweight**: Independent of any other prompt or visual libraries.
-        - **Adaptable**: Works with any string formatting and window size.
-        - **Extensive**: Packed with tweaks and features for any situation.
-        - **Complete**: Supports Windows 10 (Anniversary Update and up).
-        
-        Installing
-        ----------
-        
-        .. code-block::
-        
-            pip3 install survey
-        
-        Links
-        -----
-        
-        - Check out the `Quickstart <https://survey.readthedocs.io/quickstart.html>`_ guide for more.
-        - Greatly inspired by `AlecAivazis's GoLang <https://github.com/AlecAivazis/survey>`_ library.
-        
-        Suggestions and contributions are greatly appreciated!
-        
-Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.11
 Provides-Extra: docs
+License-File: LICENSE
+
+✨ A simple library for creating beautiful interactive prompts.
+
+.. image:: https://github.com/Exahilosys/survey/blob/main/docs/_static/images/showcase-1.gif?raw=true
+
+Features
+--------
+
+- **Pythonic**: Friendly interface built around simple functions.
+- **Lightweight**: No external depencencies for any operating system.
+- **Adaptable**: Works with any string formatting and window size.
+- **Extensive**: Packed with tweaks and features for any situation.
+- **Complete**: Supports Windows 10 (Anniversary Update and up).
+
+Installing
+----------
+
+.. code-block::
+
+    pip3 install survey
+
+Links
+-----
+
+- Check out the `Quickstart <https://survey.readthedocs.io/reference.html>`_ guide for more.
+- Greatly inspired by `AlecAivazis's GoLang <https://github.com/AlecAivazis/survey>`_ library.
+
+Suggestions and contributions are greatly appreciated!
```

