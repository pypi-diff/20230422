# Comparing `tmp/pyudev-0.8.tar.gz` & `tmp/pyudev-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyudev-0.8.tar", last modified: Sat Jan  8 01:09:07 2011, max compression
+gzip compressed data, was "dist/pyudev-0.9.tar", last modified: Wed Mar  9 11:15:15 2011, max compression
```

## Comparing `pyudev-0.8.tar` & `pyudev-0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-01-08 01:09:07.000000 pyudev-0.8/
--rw-r--r--   0 lunar     (1000) lunar     (1000)     4690 2011-01-08 00:57:55.000000 pyudev-0.8/CHANGES.rst
--rwxr-xr-x   0 lunar     (1000) lunar     (1000)    11514 2011-01-08 00:46:45.000000 pyudev-0.8/bootstrap_native_bindings.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     3266 2011-01-08 01:09:07.000000 pyudev-0.8/PKG-INFO
-drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-01-08 01:09:07.000000 pyudev-0.8/tests/
--rw-r--r--   0 lunar     (1000) lunar     (1000)    13429 2011-01-08 00:57:52.000000 pyudev-0.8/tests/conftest.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     3267 2011-01-08 00:57:52.000000 pyudev-0.8/tests/test_libudev.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     9900 2011-01-08 00:57:52.000000 pyudev-0.8/tests/test_monitor.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     1572 2011-01-08 00:57:52.000000 pyudev-0.8/tests/test_core.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)    10492 2011-01-08 00:57:52.000000 pyudev-0.8/tests/test_device.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     3121 2011-01-08 00:57:52.000000 pyudev-0.8/tests/test_util.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     7369 2011-01-08 00:46:45.000000 pyudev-0.8/tests/test_observer.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     3799 2011-01-08 00:57:52.000000 pyudev-0.8/tests/test_enumerate.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     2062 2011-01-08 00:57:52.000000 pyudev-0.8/README.rst
--rw-r--r--   0 lunar     (1000) lunar     (1000)     2144 2011-01-08 01:00:02.000000 pyudev-0.8/setup.py
-drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-01-08 01:09:07.000000 pyudev-0.8/pyudev/
--rw-r--r--   0 lunar     (1000) lunar     (1000)     2900 2011-01-08 00:57:52.000000 pyudev-0.8/pyudev/pyside.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     9786 2011-01-08 00:57:52.000000 pyudev-0.8/pyudev/monitor.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     2918 2011-01-08 00:57:52.000000 pyudev-0.8/pyudev/pyqt4.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     2058 2011-01-08 00:46:45.000000 pyudev-0.8/pyudev/_qt_base.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     5863 2011-01-08 01:07:41.000000 pyudev-0.8/pyudev/__init__.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     3584 2011-01-08 00:57:52.000000 pyudev-0.8/pyudev/glib.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)    32881 2011-01-08 00:57:52.000000 pyudev-0.8/pyudev/core.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     3372 2011-01-08 00:57:52.000000 pyudev-0.8/pyudev/_util.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)     6735 2011-01-08 00:57:52.000000 pyudev-0.8/pyudev/_libudev.py
-drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-01-08 01:09:07.000000 pyudev-0.8/pyudev.egg-info/
--rw-r--r--   0 lunar     (1000) lunar     (1000)     3266 2011-01-08 01:09:05.000000 pyudev-0.8/pyudev.egg-info/PKG-INFO
--rw-r--r--   0 lunar     (1000) lunar     (1000)        1 2011-01-08 01:09:05.000000 pyudev-0.8/pyudev.egg-info/dependency_links.txt
--rw-r--r--   0 lunar     (1000) lunar     (1000)        7 2011-01-08 01:09:05.000000 pyudev-0.8/pyudev.egg-info/top_level.txt
--rw-r--r--   0 lunar     (1000) lunar     (1000)      746 2011-01-08 01:09:05.000000 pyudev-0.8/pyudev.egg-info/SOURCES.txt
--rw-r--r--   0 lunar     (1000) lunar     (1000)      143 2011-01-08 01:09:07.000000 pyudev-0.8/setup.cfg
-drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-01-08 01:09:07.000000 pyudev-0.8/doc/
-drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-01-08 01:09:07.000000 pyudev-0.8/doc/api/
--rw-r--r--   0 lunar     (1000) lunar     (1000)      554 2011-01-08 00:57:52.000000 pyudev-0.8/doc/api/context.rst
--rw-r--r--   0 lunar     (1000) lunar     (1000)      528 2011-01-08 00:57:52.000000 pyudev-0.8/doc/api/monitor.rst
--rw-r--r--   0 lunar     (1000) lunar     (1000)     4794 2011-01-08 00:57:52.000000 pyudev-0.8/doc/api/toolkit.rst
--rw-r--r--   0 lunar     (1000) lunar     (1000)     1525 2011-01-08 00:57:52.000000 pyudev-0.8/doc/api/device.rst
--rw-r--r--   0 lunar     (1000) lunar     (1000)      831 2011-01-08 00:57:52.000000 pyudev-0.8/doc/api/index.rst
--rw-r--r--   0 lunar     (1000) lunar     (1000)     2410 2011-01-08 00:57:52.000000 pyudev-0.8/doc/conf.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)       49 2011-01-06 14:34:35.000000 pyudev-0.8/doc/changes.rst
--rw-r--r--   0 lunar     (1000) lunar     (1000)     4569 2011-01-06 14:34:35.000000 pyudev-0.8/doc/Makefile
--rw-r--r--   0 lunar     (1000) lunar     (1000)     3733 2011-01-08 00:57:52.000000 pyudev-0.8/doc/index.rst
--rw-r--r--   0 lunar     (1000) lunar     (1000)       52 2011-01-06 14:34:35.000000 pyudev-0.8/doc/licencing.rst
--rw-r--r--   0 lunar     (1000) lunar     (1000)    15757 2011-01-06 14:34:35.000000 pyudev-0.8/distribute_setup.py
--rw-r--r--   0 lunar     (1000) lunar     (1000)      174 2011-01-06 14:34:35.000000 pyudev-0.8/MANIFEST.in
--rw-r--r--   0 lunar     (1000) lunar     (1000)    26432 2011-01-06 14:34:35.000000 pyudev-0.8/COPYING
--rwxr-xr-x   0 lunar     (1000) lunar     (1000)     2181 2011-01-08 00:46:45.000000 pyudev-0.8/library_path_wrapper.py
+drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-03-09 11:15:15.000000 pyudev-0.9/
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     4954 2011-03-09 11:09:57.000000 pyudev-0.9/CHANGES.rst
+-rwxr-xr-x   0 lunar     (1000) lunar     (1000)    11841 2011-03-08 15:44:52.000000 pyudev-0.9/bootstrap_native_bindings.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     3266 2011-03-09 11:15:15.000000 pyudev-0.9/PKG-INFO
+drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-03-09 11:15:15.000000 pyudev-0.9/tests/
+-rw-r--r--   0 lunar     (1000) lunar     (1000)    14759 2011-03-08 16:30:20.000000 pyudev-0.9/tests/conftest.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     3314 2011-03-08 16:13:48.000000 pyudev-0.9/tests/test_libudev.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)    11112 2011-03-08 16:20:12.000000 pyudev-0.9/tests/test_monitor.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     2887 2011-03-08 16:13:48.000000 pyudev-0.9/tests/test_core.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)    13531 2011-03-08 16:19:37.000000 pyudev-0.9/tests/test_device.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     4054 2011-03-08 16:20:27.000000 pyudev-0.9/tests/test_util.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     7369 2011-03-08 16:13:48.000000 pyudev-0.9/tests/test_observer.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     6289 2011-03-08 16:19:51.000000 pyudev-0.9/tests/test_enumerate.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     2062 2011-01-08 00:57:52.000000 pyudev-0.9/README.rst
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     2144 2011-01-08 01:00:02.000000 pyudev-0.9/setup.py
+drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-03-09 11:15:15.000000 pyudev-0.9/pyudev/
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     2899 2011-03-09 11:04:18.000000 pyudev-0.9/pyudev/pyside.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)    10564 2011-02-19 20:28:21.000000 pyudev-0.9/pyudev/monitor.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     2917 2011-03-09 11:04:15.000000 pyudev-0.9/pyudev/pyqt4.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     2058 2011-01-08 00:46:45.000000 pyudev-0.9/pyudev/_qt_base.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     5854 2011-01-30 16:14:46.000000 pyudev-0.9/pyudev/__init__.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     3584 2011-01-08 00:57:52.000000 pyudev-0.9/pyudev/glib.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)    35120 2011-03-09 11:04:07.000000 pyudev-0.9/pyudev/core.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     3401 2011-03-09 11:03:59.000000 pyudev-0.9/pyudev/_util.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     7299 2011-03-08 16:55:39.000000 pyudev-0.9/pyudev/_libudev.py
+drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-03-09 11:15:15.000000 pyudev-0.9/pyudev.egg-info/
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     3266 2011-03-09 11:15:13.000000 pyudev-0.9/pyudev.egg-info/PKG-INFO
+-rw-r--r--   0 lunar     (1000) lunar     (1000)        1 2011-03-09 11:15:13.000000 pyudev-0.9/pyudev.egg-info/dependency_links.txt
+-rw-r--r--   0 lunar     (1000) lunar     (1000)        7 2011-03-09 11:15:13.000000 pyudev-0.9/pyudev.egg-info/top_level.txt
+-rw-r--r--   0 lunar     (1000) lunar     (1000)      746 2011-03-09 11:15:14.000000 pyudev-0.9/pyudev.egg-info/SOURCES.txt
+-rw-r--r--   0 lunar     (1000) lunar     (1000)      143 2011-03-09 11:15:15.000000 pyudev-0.9/setup.cfg
+drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-03-09 11:15:15.000000 pyudev-0.9/doc/
+drwxr-xr-x   0 lunar     (1000) lunar     (1000)        0 2011-03-09 11:15:15.000000 pyudev-0.9/doc/api/
+-rw-r--r--   0 lunar     (1000) lunar     (1000)      590 2011-02-23 19:54:45.000000 pyudev-0.9/doc/api/context.rst
+-rw-r--r--   0 lunar     (1000) lunar     (1000)      562 2011-02-19 20:28:21.000000 pyudev-0.9/doc/api/monitor.rst
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     4794 2011-01-08 00:57:52.000000 pyudev-0.9/doc/api/toolkit.rst
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     1557 2011-02-12 17:30:00.000000 pyudev-0.9/doc/api/device.rst
+-rw-r--r--   0 lunar     (1000) lunar     (1000)      831 2011-01-08 00:57:52.000000 pyudev-0.9/doc/api/index.rst
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     2372 2011-01-30 16:16:39.000000 pyudev-0.9/doc/conf.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)       49 2011-01-06 14:34:35.000000 pyudev-0.9/doc/changes.rst
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     4569 2011-01-06 14:34:35.000000 pyudev-0.9/doc/Makefile
+-rw-r--r--   0 lunar     (1000) lunar     (1000)     3733 2011-01-08 00:57:52.000000 pyudev-0.9/doc/index.rst
+-rw-r--r--   0 lunar     (1000) lunar     (1000)       52 2011-01-06 14:34:35.000000 pyudev-0.9/doc/licencing.rst
+-rw-r--r--   0 lunar     (1000) lunar     (1000)    15757 2011-01-06 14:34:35.000000 pyudev-0.9/distribute_setup.py
+-rw-r--r--   0 lunar     (1000) lunar     (1000)      174 2011-01-06 14:34:35.000000 pyudev-0.9/MANIFEST.in
+-rw-r--r--   0 lunar     (1000) lunar     (1000)    26432 2011-01-06 14:34:35.000000 pyudev-0.9/COPYING
+-rwxr-xr-x   0 lunar     (1000) lunar     (1000)     2181 2011-01-08 00:46:45.000000 pyudev-0.9/library_path_wrapper.py
```

### Comparing `pyudev-0.8/CHANGES.rst` & `pyudev-0.9/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+0.9 (Mar 09, 2011)
+==================
+
+- #21: Added :meth:`pyudev.Device.find_parent`
+- #22: Added :meth:`pyudev.Monitor.filter_by_tag`
+- Added :attr:`pyudev.Context.log_priority` to control internal UDev logging
+- Improve error reporting, if libudev is missing
+
+
 0.8 (Jan 08, 2011)
 ==================
 
 New features
 ------------
 
 - #16: Added :meth:`pyudev.Enumerator.match` to simplify device filtering
```

### Comparing `pyudev-0.8/bootstrap_native_bindings.py` & `pyudev-0.9/bootstrap_native_bindings.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,31 +193,31 @@
         cmd.extend(self.configure_options)
         self._check_call(cmd, cwd=self.build_directory)
 
 
 RIVERBANK_DOWNLOAD_URL = 'http://www.riverbankcomputing.com/static/Downloads/{0}'
 
 PYQT4_SOURCES = [
-    SourcePackage('sip', '4.12', SipBuild,
+    SourcePackage('sip', '4.12.1', SipBuild,
                   RIVERBANK_DOWNLOAD_URL.format(
                       'sip4/{name}-{version}.tar.gz')),
-    SourcePackage('PyQt-x11-gpl', '4.8.2', PyQtBuild,
+    SourcePackage('PyQt-x11-gpl', '4.8.3', PyQtBuild,
                   RIVERBANK_DOWNLOAD_URL.format(
                       'PyQt4/{name}-{version}.tar.gz'))]
 
 PYSIDE_DOWNLOAD_URL = 'http://www.pyside.org/files/{0}'
 
 PYSIDE_SOURCES = [
-    SourcePackage('apiextractor', '0.9.1', CMakeBuild,
+    SourcePackage('apiextractor', '0.10.0', CMakeBuild,
                   PYSIDE_DOWNLOAD_URL.format('{name}-{version}.tar.bz2')),
-    SourcePackage('generatorrunner', '0.6.3', CMakeBuild,
+    SourcePackage('generatorrunner', '0.6.7', CMakeBuild,
                   PYSIDE_DOWNLOAD_URL.format('{name}-{version}.tar.bz2')),
-    SourcePackage('shiboken', '1.0.0~beta2', CMakeBuild,
+    SourcePackage('shiboken', '1.0.0', CMakeBuild,
                   PYSIDE_DOWNLOAD_URL.format('{name}-{version}.tar.bz2')),
-    SourcePackage('pyside', 'qt4.7+1.0.0~beta2', PySideBuild,
+    SourcePackage('pyside', 'qt4.7+1.0.0', PySideBuild,
                   PYSIDE_DOWNLOAD_URL.format('{name}-{version}.tar.bz2')),
     ]
 
 GNOME_DOWNLOAD_URL = 'http://ftp.gnome.org/pub/GNOME/sources/{0}'
 
 GOBJECT_SOURCES = [
     SourcePackage('pygobject', '2.27.0', AutotoolsBuild,
@@ -271,19 +271,22 @@
                  expected_version, QtCore.PYQT_VERSION_STR)
         return QtCore.PYQT_VERSION_STR == expected_version
     except ImportError:
         log.exception('QtCore not found')
         return False
 
 
-def have_pyside_qtcore():
+def have_pyside_qtcore(expected_version):
     log = logging.getLogger('pyside')
     try:
         import_string('PySide.QtCore')
-        return True
+        PySide = import_string('PySide')
+        log.info('excepted version %s, actual version %s',
+                 expected_version, PySide.__version__)
+        return PySide.__version__ == expected_version
     except ImportError:
         log.exception('QtCore not found')
         return False
 
 
 def have_gobject(expected_version):
     log = logging.getLogger('pygobject')
@@ -311,24 +314,27 @@
                       const=logging.INFO)
     parser.set_defaults(loglevel=logging.WARN)
     opts, args = parser.parse_args()
     if len(args) != 2:
         parser.error('missing arguments')
     logging.basicConfig(level=opts.loglevel)
 
-    download_directory, build_directory = args
-    ensuredirs(download_directory, build_directory)
-
-    if not have_pyqt4_qtcore(PYQT4_SOURCES[1].version):
-        build_all(PYQT4_SOURCES, download_directory, build_directory)
+    try:
+        download_directory, build_directory = args
+        ensuredirs(download_directory, build_directory)
 
-    if sys.version_info[0] < 3:
-        # pyside and pygobject are not available for python 3 yet
-        if not have_pyside_qtcore():
-            build_all(PYSIDE_SOURCES, download_directory, build_directory)
+        if not have_pyqt4_qtcore(PYQT4_SOURCES[1].version):
+            build_all(PYQT4_SOURCES, download_directory, build_directory)
 
-        if not have_gobject(GOBJECT_SOURCES[0].version):
-            build_all(GOBJECT_SOURCES, download_directory, build_directory)
+        if sys.version_info[0] < 3:
+            # pyside and pygobject are not available for python 3 yet
+            if not have_pyside_qtcore(PYSIDE_SOURCES[3].version.split('+')[1]):
+                build_all(PYSIDE_SOURCES, download_directory, build_directory)
+
+            if not have_gobject(GOBJECT_SOURCES[0].version):
+                build_all(GOBJECT_SOURCES, download_directory, build_directory)
+    except KeyboardInterrupt:
+        pass
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pyudev-0.8/PKG-INFO` & `pyudev-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pyudev
-Version: 0.8
+Version: 0.9
 Summary: A libudev binding
 Home-page: http://packages.python.org/pyudev
 Author: Sebastian Wiesner
 Author-email: lunaryorn@googlemail.com
 License: MIT/X11
 Description: ######
         pyudev
```

### Comparing `pyudev-0.8/tests/conftest.py` & `pyudev-0.9/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,61 @@
 import re
 import random
 import subprocess
 import socket
 from functools import wraps
 from contextlib import contextmanager
 from subprocess import check_call
+if sys.version_info[:2] < (3, 2):
+    from contextlib import nested
 
 import mock
 import pytest
 
 import pyudev
 
 
+if sys.version_info[:2] >= (3, 2):
+    @contextmanager
+    def nested(*managers):
+        """
+        Copy of contextlib.nested from python 2.7 with slight adaptions to
+        Python 3.2 to use nested() on python 3.2 and thus retain backwards
+        compatibility with Python 2.6 (with doesn't support the new nesting
+        syntax), while being able to run the test suite on Python 3.2 as
+        well (which doesn't provide contextlib.nested anymore).
+        """
+        exits = []
+        vars = []
+        exc = None
+        try:
+            for mgr in managers:
+                exit = mgr.__exit__
+                enter = mgr.__enter__
+                vars.append(enter())
+                exits.append(exit)
+            yield vars
+        except BaseException as e:
+            exc = e
+        finally:
+            while exits:
+                exit = exits.pop()
+                try:
+                    if exc:
+                        args = (type(exc), exc, exc.__traceback__)
+                    else:
+                        args = (None, None, None)
+                    if exit(*args):
+                        exc = None
+                except BaseException as e:
+                    exc = e
+            if exc:
+                raise exc
+
+
 class FakeMonitor(object):
     """
     A dummy pyudev.Monitor class, which allows clients to trigger arbitrary
     events, emitting clearly defined device objects.
     """
 
     def __init__(self, device_to_emit):
@@ -225,15 +265,15 @@
     reason = 'udev version mismatch: {0} required, {1} found'.format(
         version_spec, actual_version)
     return pytest.mark.skipif(str(expr), reason=reason)
 
 
 def pytest_namespace():
     return dict((func.__name__, func) for func in
-                (get_device_sample, patch_libudev, load_dummy,
+                (get_device_sample, patch_libudev, load_dummy, nested,
                  unload_dummy, is_unicode_string, check_udev_version))
 
 
 def pytest_addoption(parser):
     parser.addoption('--all-devices', action='store_true',
                      help='Run device tests against *all* devices in the '
                      'database.  By default, only a random sample will be '
```

### Comparing `pyudev-0.8/tests/test_libudev.py` & `pyudev-0.9/tests/test_libudev.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 libudev = binding.libudev
 
 
 # new functions added in specific libudev versions
 UDEV_ADDITIONS = {
     152: ['udev_new_from_environment'],
     154: ['udev_device_get_tags_list_entry',
-          'udev_enumerate_add_match_tag'],
+          'udev_enumerate_add_match_tag',
+          'udev_monitor_filter_add_match_tag'],
     165: ['udev_device_get_is_initialized',
           'udev_device_get_usec_since_initialized',
           'udev_enumerate_add_match_is_initialized']
     }
 
 
 def pytest_generate_tests(metafunc):
```

### Comparing `pyudev-0.8/tests/test_monitor.py` & `pyudev-0.9/tests/test_monitor.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,20 +41,21 @@
         Monitor.from_netlink(context, source='invalid_source')
     message = ('Invalid source: {0!r}. Must be one of "udev" '
                'or "kernel"'.format('invalid_source'))
     assert str(exc_info.value) == message
 
 
 def _assert_from_netlink_called(context, *args):
-    with pytest.patch_libudev('udev_monitor_new_from_netlink') as func:
+    new_from_netlink = 'udev_monitor_new_from_netlink'
+    with pytest.patch_libudev(new_from_netlink) as new_from_netlink:
         source = args[0].encode('ascii') if args else b'udev'
-        func.return_value = mock.sentinel.pointer
+        new_from_netlink.return_value = mock.sentinel.pointer
         monitor = Monitor.from_netlink(context, *args)
-        func.assert_called_with(context._context, source)
-        assert isinstance(func.call_args[0][1], bytes)
+        new_from_netlink.assert_called_with(context._context, source)
+        assert isinstance(new_from_netlink.call_args[0][1], bytes)
         assert monitor._monitor is mock.sentinel.pointer
 
 
 def test_from_netlink_source_udev(context):
     monitor = Monitor.from_netlink(context)
     assert monitor._monitor
     monitor = Monitor.from_netlink(context, source='udev')
@@ -77,72 +78,94 @@
 
 def test_from_socket(context, socket_path):
     monitor = Monitor.from_socket(context, str(socket_path))
     assert monitor._monitor
 
 
 def test_from_socket_mock(context, socket_path):
-    with pytest.patch_libudev('udev_monitor_new_from_socket') as func:
-        func.return_value = mock.sentinel.pointer
-        monitor = Monitor.from_socket(context, str(socket_path))
-        func.assert_called_with(context._context, str(socket_path).encode(
-            sys.getfilesystemencoding()))
+    socket_path = str(socket_path)
+    new_from_socket = 'udev_monitor_new_from_socket'
+    with pytest.patch_libudev(new_from_socket) as new_from_socket:
+        new_from_socket.return_value = mock.sentinel.pointer
+        monitor = Monitor.from_socket(context, socket_path)
+        new_from_socket.assert_called_with(
+            context._context, socket_path.encode(sys.getfilesystemencoding()))
         assert monitor._monitor is mock.sentinel.pointer
         Monitor.from_socket(context, 'foobar')
-        func.assert_called_with(context._context, b'foobar')
-        assert isinstance(func.call_args[0][1], bytes)
+        new_from_socket.assert_called_with(context._context, b'foobar')
+        assert isinstance(new_from_socket.call_args[0][1], bytes)
 
 
 def test_fileno(monitor):
     # we can't do more than check that no exception is thrown
     monitor.fileno()
 
 
 def test_fileno_mock(monitor):
-    with pytest.patch_libudev('udev_monitor_get_fd') as func:
-        func.return_value = mock.sentinel.fileno
+    get_fd = 'udev_monitor_get_fd'
+    with pytest.patch_libudev(get_fd) as get_fd:
+        get_fd.return_value = mock.sentinel.fileno
         assert monitor.fileno() is mock.sentinel.fileno
-        func.assert_called_with(monitor._monitor)
+        get_fd.assert_called_with(monitor._monitor)
 
 
 def test_filter_by_no_subsystem(monitor):
     with pytest.raises(AttributeError):
         monitor.filter_by(None)
 
 
 def test_filter_by_subsystem_no_dev_type(monitor):
     monitor.filter_by(b'input')
     monitor.filter_by('input')
 
 
 def test_filter_by_subsystem_no_dev_type_mock(monitor):
-    epic_func_name = 'udev_monitor_filter_add_match_subsystem_devtype'
-    with pytest.patch_libudev(epic_func_name) as func:
-        func.return_value = 0
+    add_match = 'udev_monitor_filter_add_match_subsystem_devtype'
+    with pytest.patch_libudev(add_match) as add_match:
+        add_match.return_value = 0
         monitor.filter_by(b'input')
-        func.assert_called_with(monitor._monitor, b'input', None)
+        add_match.assert_called_with(monitor._monitor, b'input', None)
         monitor.filter_by('input')
-        func.assert_called_with(monitor._monitor, b'input', None)
-        assert isinstance(func.call_args[0][1], bytes)
+        add_match.assert_called_with(monitor._monitor, b'input', None)
+        assert isinstance(add_match.call_args[0][1], bytes)
 
 
 def test_filter_by_subsystem_dev_type(monitor):
     monitor.filter_by('input', b'usb_interface')
     monitor.filter_by('input', 'usb_interface')
 
 
 def test_filter_by_subsystem_dev_type_mock(monitor):
-    epic_func_name = 'udev_monitor_filter_add_match_subsystem_devtype'
-    with pytest.patch_libudev(epic_func_name) as func:
-        func.return_value = 0
+    add_match = 'udev_monitor_filter_add_match_subsystem_devtype'
+    with pytest.patch_libudev(add_match) as add_match:
+        add_match.return_value = 0
         monitor.filter_by(b'input', b'usb_interface')
-        func.assert_called_with(monitor._monitor, b'input', b'usb_interface')
+        add_match.assert_called_with(
+            monitor._monitor, b'input', b'usb_interface')
         monitor.filter_by('input', 'usb_interface')
-        func.assert_called_with(monitor._monitor, b'input', b'usb_interface')
-        assert isinstance(func.call_args[0][2], bytes)
+        add_match.assert_called_with(
+            monitor._monitor, b'input', b'usb_interface')
+        assert isinstance(add_match.call_args[0][2], bytes)
+
+
+@pytest.check_udev_version('>= 154')
+def test_filter_by_tag(monitor):
+    monitor.filter_by_tag('spam')
+
+
+@pytest.check_udev_version('>= 154')
+def test_pytest_filter_by_tag_mock(monitor):
+    match_tag = 'udev_monitor_filter_add_match_tag'
+    with pytest.patch_libudev(match_tag) as match_tag:
+        match_tag.return_value = 0
+        monitor.filter_by_tag(b'spam')
+        match_tag.assert_called_with(monitor._monitor, b'spam')
+        monitor.filter_by_tag('eggs')
+        match_tag.assert_called_with(monitor._monitor, b'eggs')
+        assert isinstance(match_tag.call_args[0][1], bytes)
 
 
 def test_enable_receiving_netlink_kernel_source(context):
     monitor = Monitor.from_netlink(context, source='kernel')
     monitor.enable_receiving()
 
 
@@ -173,18 +196,20 @@
     with pytest.patch_libudev('udev_monitor_enable_receiving') as func:
         func.return_value = 0
         monitor.enable_receiving()
         func.assert_called_with(monitor._monitor)
 
 
 def test_enable_receiving_error_mock(context, monitor, socket_path):
-    with pytest.patch_libudev('udev_monitor_enable_receiving') as func:
-        with mock.patch('pyudev.monitor.get_libudev_errno') as get_errno:
+    enable_receiving = 'udev_monitor_enable_receiving'
+    get_errno = 'pyudev.monitor.get_libudev_errno'
+    with pytest.nested(pytest.patch_libudev(enable_receiving),
+                       mock.patch(get_errno)) as (enable_receiving, get_errno):
             get_errno.return_value = errno.ENOENT
-            func.return_value = 1
+            enable_receiving.return_value = 1
             with pytest.raises(EnvironmentError) as exc_info:
                 monitor.enable_receiving()
             error = exc_info.value
             assert error.errno == errno.ENOENT
             assert error.strerror == os.strerror(errno.ENOENT)
 
             monitor = Monitor.from_socket(context, str(socket_path))
@@ -211,42 +236,47 @@
     action, device = monitor.receive_device()
     assert action == 'remove'
     assert device.subsystem == 'net'
     assert device.device_path == '/devices/virtual/net/dummy0'
 
 
 def test_receive_device_mock(monitor):
-    with pytest.patch_libudev('udev_monitor_receive_device') as func:
-        with pytest.patch_libudev('udev_device_get_action') as actfunc:
-            func.return_value = mock.sentinel.pointer
-            actfunc.return_value = b'action'
-            action, device = monitor.receive_device()
-            assert action == 'action'
-            assert pytest.is_unicode_string(action)
-            assert isinstance(device, Device)
-            assert device.context is monitor.context
-            assert device._device is mock.sentinel.pointer
-            actfunc.assert_called_with(mock.sentinel.pointer)
-            func.assert_called_with(monitor._monitor)
+    receive_device = 'udev_monitor_receive_device'
+    get_action = 'udev_device_get_action'
+    with pytest.nested(pytest.patch_libudev(receive_device),
+                       pytest.patch_libudev(get_action)) as (receive_device,
+                                                             get_action):
+        receive_device.return_value = mock.sentinel.pointer
+        get_action.return_value = b'action'
+        action, device = monitor.receive_device()
+        assert action == 'action'
+        assert pytest.is_unicode_string(action)
+        assert isinstance(device, Device)
+        assert device.context is monitor.context
+        assert device._device is mock.sentinel.pointer
+        get_action.assert_called_with(mock.sentinel.pointer)
+        receive_device.assert_called_with(monitor._monitor)
 
 
 def test_receive_device_error_mock(monitor):
-    with pytest.patch_libudev('udev_monitor_receive_device') as func:
-        with mock.patch('pyudev.monitor.get_libudev_errno') as errorfunc:
-            func.return_value = None
-            errorfunc.return_value = 0
-            with pytest.raises(EnvironmentError) as exc_info:
-                monitor.receive_device()
-            assert str(exc_info.value) == 'Could not receive device'
-            errorfunc.return_value = errno.ENOENT
-            with pytest.raises(EnvironmentError) as exc_info:
-                monitor.receive_device()
-            error = exc_info.value
-            assert error.errno == errno.ENOENT
-            assert error.strerror == os.strerror(errno.ENOENT)
+    get_errno = 'pyudev.monitor.get_libudev_errno'
+    receive_device = 'udev_monitor_receive_device'
+    with pytest.nested(pytest.patch_libudev(receive_device),
+                       mock.patch(get_errno)) as (receive_device, get_errno):
+        receive_device.return_value = None
+        get_errno.return_value = 0
+        with pytest.raises(EnvironmentError) as exc_info:
+            monitor.receive_device()
+        assert str(exc_info.value) == 'Could not receive device'
+        get_errno.return_value = errno.ENOENT
+        with pytest.raises(EnvironmentError) as exc_info:
+            monitor.receive_device()
+        error = exc_info.value
+        assert error.errno == errno.ENOENT
+        assert error.strerror == os.strerror(errno.ENOENT)
 
 
 @pytest.mark.privileged
 def test_iter(monitor):
     pytest.unload_dummy()
     monitor.filter_by('net')
     monitor.enable_receiving()
```

### Comparing `pyudev-0.8/tests/test_device.py` & `pyudev-0.9/tests/test_device.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,17 +22,20 @@
 import os
 import operator
 import sys
 from itertools import count
 from datetime import timedelta
 
 import pytest
+import mock
 
 from pyudev import (Device,
-                    DeviceNotFoundAtPathError, DeviceNotFoundByNameError)
+                    DeviceNotFoundAtPathError,
+                    DeviceNotFoundByNameError,
+                    DeviceNotFoundInEnvironmentError)
 
 
 def pytest_generate_tests(metafunc):
     args = metafunc.funcargnames
     if 'device_path' in args or 'device' in args:
         devices = pytest.get_device_sample(metafunc.config)
         for device_path in devices:
@@ -96,59 +99,55 @@
     assert error.sys_name == 'foobar'
     assert str(error) == 'No device {0!r} in {1!r}'.format(
         error.sys_name, error.subsystem)
 
 
 @pytest.check_udev_version('>= 152')
 def test_device_from_environment(context):
-    raise NotImplementedError()
+    # there is no device in a standard environment
+    with pytest.raises(DeviceNotFoundInEnvironmentError):
+        Device.from_environment(context)
 
 
 @pytest.mark.properties
 def test_device_properties(device, properties):
-    properties.pop('DEVNAME', None)
-    for n, property in enumerate(properties, start=1):
-        assert device[property] == properties[property]
-    assert n > 0
+    assert all(device[p] == properties[p] for p in properties)
 
 
 @pytest.mark.properties
 def test_device_asint(device, properties):
-    for n, property in enumerate(properties, start=1):
+    for property in properties:
         value = properties[property]
         try:
             value = int(value)
         except ValueError:
             with pytest.raises(ValueError):
                 device.asint(property)
         else:
             assert device.asint(property) == value
-    assert n > 0
 
 
 @pytest.mark.properties
 def test_device_asbool(device, properties):
-    for n, property in enumerate(properties, start=1):
+    for property in properties:
         value = properties[property]
         if value == '1':
             assert device.asbool(property)
         elif value == '0':
             assert not device.asbool(property)
         else:
             with pytest.raises(ValueError) as exc_info:
                 device.asbool(property)
             message = 'Not a boolean value: {0!r}'
             assert str(exc_info.value) == message.format(value)
-    assert n > 0
 
 
 def test_attributes_iter(device, attributes):
     device_attributes = set(device.attributes)
-    for attribute in attributes:
-        assert attribute in device_attributes
+    assert all(a in device_attributes for a in attributes)
     assert all(pytest.is_unicode_string(a) for a in device_attributes)
 
 
 def test_attributes_len(device):
     counter = count()
     for _ in device.attributes:
         next(counter)
@@ -156,26 +155,24 @@
 
 
 def test_attributes_contains(device, attributes):
     assert all(a in device.attributes for a in attributes)
 
 
 def test_attributes_getitem(device, attributes):
-    for attribute, value in attributes.items():
-        # device attributes *must* be bytes.
-        assert isinstance(device.attributes[attribute], bytes)
-        value = value.encode(sys.getfilesystemencoding())
-        assert device.attributes[attribute] == value
+    assert all(isinstance(device.attributes[a], bytes) for a in attributes)
+    assert all(device.attributes[a] == v.encode(sys.getfilesystemencoding())
+               for a, v in attributes.items())
 
 
 def test_attributes_asstring(device, attributes):
-    for attribute, value in attributes.items():
-        assert pytest.is_unicode_string(
-            device.attributes.asstring(attribute))
-        assert device.attributes.asstring(attribute) == value
+    assert all(pytest.is_unicode_string(device.attributes.asstring(a))
+               for a in attributes)
+    assert all(device.attributes.asstring(a) == v
+               for a, v in attributes.items())
 
 
 def test_attributes_asint(device, attributes):
     for attribute, value in attributes.items():
         try:
             value = int(value)
         except ValueError:
@@ -196,19 +193,18 @@
                 device.attributes.asbool(attribute)
             message = 'Not a boolean value: {0!r}'
             assert str(exc_info.value) == message.format(value)
 
 
 @pytest.mark.properties
 def test_device_devname(context, device, all_properties):
-    if 'DEVNAME' not in device:
+    if 'DEVNAME' not in all_properties:
         pytest.xfail('%r has no DEVNAME' % device)
-    assert device['DEVNAME'].startswith(context.device_path)
-    assert device['DEVNAME'] == os.path.join(context.device_path,
-                                             all_properties['DEVNAME'])
+    assert os.path.join(context.device_path, device['DEVNAME']) == \
+           os.path.join(context.device_path, all_properties['DEVNAME'])
 
 
 @pytest.mark.properties
 def test_device_subsystem(device, properties):
     assert device.subsystem == properties['SUBSYSTEM']
     assert pytest.is_unicode_string(device.subsystem)
 
@@ -236,31 +232,64 @@
     assert all(pytest.is_unicode_string(l) for l in device.device_links)
 
 
 @pytest.check_udev_version('>= 165')
 @pytest.mark.properties
 def test_device_is_initialized(device):
     assert isinstance(device.is_initialized, bool)
-    with pytest.patch_libudev('udev_device_get_is_initialized') as func:
-        func.return_value = True
+    get_is_initialized = 'udev_device_get_is_initialized'
+    with pytest.patch_libudev(get_is_initialized) as get_is_initialized:
+        get_is_initialized.return_value = True
         assert device.is_initialized
-        assert func.called
+        get_is_initialized.assert_called_with(device._device)
 
 
 @pytest.check_udev_version('>= 165')
 @pytest.mark.properties
 def test_device_time_since_initialized(device):
     assert isinstance(device.time_since_initialized, timedelta)
-    funcname = 'udev_device_get_usec_since_initialized'
-    with pytest.patch_libudev(funcname) as func:
-        func.return_value = 100
+    usec_since_init = 'udev_device_get_usec_since_initialized'
+    with pytest.patch_libudev(usec_since_init) as usec_since_init:
+        usec_since_init.return_value = 100
         assert device.time_since_initialized.microseconds == 100
-        assert func.called
+        usec_since_init.assert_called_with(device._device)
+
+
+@pytest.check_udev_version('>= 154')
+def test_device_tags_mock(device):
+    tags_list = iter([b'spam', b'eggs', b'foo', b'bar'])
 
+    def next_entry(entry):
+        try:
+            return next(tags_list)
+        except StopIteration:
+            return None
+    def name(entry):
+        if entry:
+            return entry
+        else:
+            pytest.fail('empty entry!')
+
+    get_tags_list_entry = 'udev_device_get_tags_list_entry'
+    get_next = 'udev_list_entry_get_next'
+    get_name = 'udev_list_entry_get_name'
+    with pytest.nested(pytest.patch_libudev(get_tags_list_entry),
+                       pytest.patch_libudev(get_name),
+                       pytest.patch_libudev(get_next)) as (get_tags_list_entry,
+                                                           get_name, get_next):
+        get_tags_list_entry.return_value = next(tags_list)
+        get_name.side_effect = name
+        get_next.side_effect = next_entry
+
+        device_tags = list(device.tags)
+        assert device_tags == ['spam', 'eggs', 'foo', 'bar']
+        assert all(pytest.is_unicode_string(t) for t in device_tags)
 
+
+@pytest.mark.xfail(reason='Not implemented')
 @pytest.check_udev_version('>= 154')
 def test_device_tags():
     raise NotImplementedError()
 
 
 @pytest.mark.properties
 def test_device_driver(device, properties):
@@ -280,14 +309,54 @@
     child = device
     for parent in device.traverse():
         assert parent == child.parent
         assert child in parent.children
         child = parent
 
 
+def test_device_find_parent(device):
+    parent = device.find_parent(device.subsystem)
+    if not parent:
+        pytest.xfail('no parent within the same subsystem')
+    assert parent.subsystem == device.subsystem
+    assert parent in device.traverse()
+    assert device in parent.children
+
+
+def test_device_find_parent_no_devtype_mock(device):
+    get_parent = 'udev_device_get_parent_with_subsystem_devtype'
+    ref = 'udev_device_ref'
+    with pytest.nested(pytest.patch_libudev(get_parent),
+                       pytest.patch_libudev(ref)) as (get_parent, ref):
+        get_parent.return_value = mock.sentinel.device
+        ref.return_value = mock.sentinel.referenced_device
+        parent = device.find_parent('subsystem')
+        get_parent.assert_called_with(device._device, b'subsystem', None)
+        ref.assert_called_with(mock.sentinel.device)
+        assert isinstance(get_parent.call_args[0][1], bytes)
+        assert isinstance(parent, Device)
+        assert parent._device is mock.sentinel.referenced_device
+
+
+def test_device_find_parent_with_devtype_mock(device):
+    get_parent = 'udev_device_get_parent_with_subsystem_devtype'
+    ref = 'udev_device_ref'
+    with pytest.nested(pytest.patch_libudev(get_parent),
+                       pytest.patch_libudev(ref)) as (get_parent, ref):
+        get_parent.return_value = mock.sentinel.device
+        ref.return_value = mock.sentinel.referenced_device
+        parent = device.find_parent('subsystem', 'devtype')
+        get_parent.assert_called_with(device._device, b'subsystem', b'devtype')
+        ref.assert_called_with(mock.sentinel.device)
+        args = get_parent.call_args[0][1:]
+        assert all(isinstance(a, bytes) for a in args)
+        assert isinstance(parent, Device)
+        assert parent._device is mock.sentinel.referenced_device
+
+
 @pytest.mark.operator
 def test_device_eq(device):
     assert device == device.device_path
     assert device == device
     assert device.parent == device.parent
     assert not (device == device.parent)
```

### Comparing `pyudev-0.8/tests/test_util.py` & `pyudev-0.9/tests/test_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,39 +22,40 @@
 
 import pytest
 
 from pyudev import _util
 
 
 @pytest.mark.conversion
-def test_assert_bytes():
-    assert isinstance(_util.assert_bytes('hello world'), bytes)
-    assert _util.assert_bytes('hello world') == b'hello world'
+def test_ensure_byte_string():
+    assert isinstance(_util.ensure_byte_string('hello world'), bytes)
+    assert _util.ensure_byte_string('hello world') == b'hello world'
     hello = b'hello world'
-    assert _util.assert_bytes(hello) is hello
+    assert _util.ensure_byte_string(hello) is hello
 
 
 @pytest.mark.conversion
-def test_assert_bytes_none():
+def test_ensure_byte_string_none():
     with pytest.raises(AttributeError):
-        _util.assert_bytes(None)
+        _util.ensure_byte_string(None)
 
 
 @pytest.mark.conversion
-def test_assert_unicode():
-    assert pytest.is_unicode_string(_util.assert_unicode(b'hello world'))
-    assert _util.assert_unicode(b'hello world') == 'hello world'
+def test_ensure_unicode_string():
+    assert pytest.is_unicode_string(
+        _util.ensure_unicode_string(b'hello world'))
+    assert _util.ensure_unicode_string(b'hello world') == 'hello world'
     hello = 'hello world'
-    assert _util.assert_unicode(hello) is hello
+    assert _util.ensure_unicode_string(hello) is hello
 
 
 @pytest.mark.conversion
-def test_assert_unicode_none():
+def test_ensure_unicode_string_none():
     with pytest.raises(AttributeError):
-        _util.assert_unicode(None)
+        _util.ensure_unicode_string(None)
 
 
 @pytest.mark.conversion
 def test_property_value_to_bytes_string():
     hello = 'hello world'.encode(sys.getfilesystemencoding())
     assert _util.property_value_to_bytes(hello) is hello
     assert isinstance(_util.property_value_to_bytes('hello world'), bytes)
@@ -85,7 +86,35 @@
     assert not _util.string_to_bool('0')
 
 @pytest.mark.conversion
 def test_string_to_bool_invalid_value():
     with pytest.raises(ValueError) as exc_info:
         _util.string_to_bool('foo')
     assert str(exc_info.value) == 'Not a boolean value: {0!r}'.format('foo')
+
+
+def test_udev_list_iterate_no_entry():
+    assert not list(_util.udev_list_iterate(None))
+
+
+def test_udev_list_iterate_mock():
+    test_list = iter(['spam', 'eggs', 'foo', 'bar'])
+
+    def next_entry(entry):
+        try:
+            return next(test_list)
+        except StopIteration:
+            return None
+    def name(entry):
+        if entry:
+            return entry
+        else:
+            pytest.fail('empty entry!')
+
+    get_next = 'udev_list_entry_get_next'
+    get_name = 'udev_list_entry_get_name'
+    with pytest.nested(pytest.patch_libudev(get_name),
+                       pytest.patch_libudev(get_next)) as (get_name, get_next):
+        get_name.side_effect = name
+        get_next.side_effect = next_entry
+        items = list(_util.udev_list_iterate(next(test_list)))
+        assert items == ['spam', 'eggs', 'foo', 'bar']
```

### Comparing `pyudev-0.8/tests/test_observer.py` & `pyudev-0.9/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/README.rst` & `pyudev-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/setup.py` & `pyudev-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/pyudev/pyside.py` & `pyudev-0.9/pyudev/pyside.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     #: emitted, if a device was removed
     deviceRemoved = Signal(Device)
     #: emitted, if a device was changed
     deviceChanged = Signal(Device)
     #: emitted, if a device was moved
     deviceMoved = Signal(Device)
 
-
     def __init__(self, monitor, parent=None):
         """
         Observe the given ``monitor`` (a :class:`~pyudev.Monitor`):
 
         ``parent`` is the parent :class:`~PySide.QtCore.QObject` of this
         object.  It is passed unchanged to the inherited constructor of
         :class:`~PySide.QtCore.QObject`.
```

### Comparing `pyudev-0.8/pyudev/monitor.py` & `pyudev-0.9/pyudev/monitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                         absolute_import)
 
 import os
 import select
 from contextlib import closing
 
 from pyudev._libudev import libudev, get_libudev_errno
-from pyudev._util import assert_bytes, assert_unicode
+from pyudev._util import ensure_byte_string, ensure_unicode_string
 
 from pyudev.core import Device
 
 
 __all__ = ['Monitor']
 
 
@@ -104,41 +104,40 @@
         source has been specified.  Raise
         :exc:`~exceptions.EnvironmentError`, if the creation of the monitor
         failed.
         """
         if source not in ('kernel', 'udev'):
             raise ValueError('Invalid source: {0!r}. Must be one of "udev" '
                              'or "kernel"'.format(source))
-        source = assert_bytes(source)
+        source = ensure_byte_string(source)
         monitor = libudev.udev_monitor_new_from_netlink(
             context._context, source)
         if not monitor:
             raise EnvironmentError('Could not create udev monitor')
         return cls(context, monitor)
 
     @classmethod
     def from_socket(cls, context, socket_path):
         """
         Connect to an arbitrary udev daemon using the given ``socket_path``.
 
-        ``context`` is the :class:`Context` to use. ``socket_path`` is a
-        byte or unicode string, pointing to an existing socket.  If the path
-        starts with a @, use an abstract namespace socket.  If
-        ``socket_path`` does not exist, fall back to an abstract namespace
-        socket.
+        ``context`` is the :class:`Context` to use. ``socket_path`` is a byte
+        or unicode string, pointing to an existing socket.  If the path starts
+        with a ``@``, use an abstract namespace socket.  If ``socket_path``
+        does not exist, fall back to an abstract namespace socket.
 
         The caller is responsible for permissions and cleanup of the socket
         file.
 
-        Return a new :class:`Monitor` object, which is connected to the
-        given socket.  Raise :exc:`~exceptions.EnvironmentError`, if the
-        creation of the monitor failed.
+        Return a new :class:`Monitor` object, which is connected to the given
+        socket.  Raise :exc:`~exceptions.EnvironmentError`, if the creation of
+        the monitor failed.
         """
         monitor = libudev.udev_monitor_new_from_socket(
-            context._context, assert_bytes(socket_path))
+            context._context, ensure_byte_string(socket_path))
         if not monitor:
             raise EnvironmentError('Could not create monitor for socket: '
                                    '{0!r}'.format(socket_path))
         return cls(context, monitor, socket_path=socket_path)
 
     def fileno(self):
         """
@@ -164,20 +163,41 @@
 
         These filters are executed inside the kernel, and client processes
         will usually not be woken up for device, that do not match these
         filters.
 
         This method must be called *before* :meth:`enable_receiving`.
         """
-        subsystem = assert_bytes(subsystem)
+        subsystem = ensure_byte_string(subsystem)
         if device_type:
-            device_type = assert_bytes(device_type)
+            device_type = ensure_byte_string(device_type)
         libudev.udev_monitor_filter_add_match_subsystem_devtype(
             self._monitor, subsystem, device_type)
 
+    def filter_by_tag(self, tag):
+        """
+        Filter incoming events by the given ``tag``.
+
+        ``tag`` is a byte or unicode string with the name of a tag.  Only
+        events for devices which have this tag attached pass the filter and are
+        handed to the caller.
+
+        Like with :meth:`filter_by` this filter is also executed inside the
+        kernel, so that client processes are usually not woken up for devices
+        without the given ``tag``.
+
+        This method must be called *before* :meth:`enable_receiving`.
+
+        .. udevminversion:: 154
+
+        .. versionadded:: 0.9
+        """
+        libudev.udev_monitor_filter_add_match_tag(
+            self._monitor, ensure_byte_string(tag))
+
     def enable_receiving(self):
         """
         Switch the monitor into listing mode.
 
         Connect to the event source and receive incoming events.  Only after
         calling this method, the monitor listens for incoming events.
 
@@ -222,15 +242,16 @@
         device_p = libudev.udev_monitor_receive_device(self._monitor)
         if not device_p:
             errno = get_libudev_errno()
             if errno == 0:
                 raise EnvironmentError('Could not receive device')
             else:
                 raise EnvironmentError(errno, os.strerror(errno))
-        action = assert_unicode(libudev.udev_device_get_action(device_p))
+        action = ensure_unicode_string(
+            libudev.udev_device_get_action(device_p))
         return action, Device(self.context, device_p)
 
     def __iter__(self):
         """
         Wait for incoming events and receive them upon arrival.
 
         This methods implicitly calls :meth:`enable_receiving`, and starts
```

### Comparing `pyudev-0.8/pyudev/pyqt4.py` & `pyudev-0.9/pyudev/pyqt4.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     #: emitted, if a device was removed
     deviceRemoved = pyqtSignal(Device)
     #: emitted, if a device was changed
     deviceChanged = pyqtSignal(Device)
     #: emitted, if a device was moved
     deviceMoved = pyqtSignal(Device)
 
-
     def __init__(self, monitor, parent=None):
         """
         Observe the given ``monitor`` (a :class:`~pyudev.Monitor`):
 
         ``parent`` is the parent :class:`~PyQt4.QtCore.QObject` of this
         object.  It is passed unchanged to the inherited constructor of
         :class:`~PyQt4.QtCore.QObject`.
```

### Comparing `pyudev-0.8/pyudev/_qt_base.py` & `pyudev-0.9/pyudev/_qt_base.py`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/pyudev/__init__.py` & `pyudev-0.9/pyudev/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,30 +59,30 @@
     You can filter the devices by specific subsystems or properties.  For
     instance, the following code only matches all mouse devices:
 
     >>> devices = context.list_devices(subsystem='input', ID_INPUT_MOUSE=True)
 
     In both cases ``devices`` is an instance of :class:`Enumerator`.  When
     iterated over, this class yields :class:`Device` objects, representing
-    those devices, which match the filters.  :class:`Device` provide various
-    attributes to access information:
+    those devices, which match the filters.  :class:`Device` objects provide
+    various attributes to access information:
 
     >>> for device in devices:
     ...     if device.sys_name.startswith('event'):
     ...         device.parent['NAME']
     ...
     u'"Logitech USB-PS/2 Optical Mouse"'
     u'"Broadcom Corp"'
     u'"PS/2 Mouse"'
 
     Monitoring devices
     ^^^^^^^^^^^^^^^^^^
 
-    Alternatively you can monitor the device tree for changes instead of
-    listing all devices using the :class:`Monitor` class:
+    Instead of listing devices, you can monitor the device tree for changes
+    using the :class:`Monitor` class:
 
     >>> monitor = pyudev.Monitor.from_netlink(context)
     >>> monitor.filter_by(subsystem='input')
     >>> for action, device in monitor:
     ...     if action == 'add':
     ...         print('{0!r} added'.format(device))
 
@@ -161,13 +161,13 @@
     .. moduleauthor::  Sebastian Wiesner  <lunaryorn@googlemail.com>
 """
 
 from __future__ import (print_function, division, unicode_literals,
                         absolute_import)
 
 
-__version__ = '0.8'
+__version__ = '0.9'
 __all__ = ['Context', 'Device']
 
 
 from pyudev.core import *
 from pyudev.monitor import *
```

### Comparing `pyudev-0.8/pyudev/glib.py` & `pyudev-0.9/pyudev/glib.py`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/pyudev/core.py` & `pyudev-0.9/pyudev/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,17 @@
 import os
 from subprocess import Popen, PIPE, CalledProcessError
 from itertools import count
 from collections import Mapping
 from datetime import timedelta
 
 from pyudev._libudev import libudev
-from pyudev._util import (assert_unicode, assert_bytes, udev_list_iterate,
-                          property_value_to_bytes, string_to_bool)
+from pyudev._util import (ensure_unicode_string, ensure_byte_string,
+                          udev_list_iterate, property_value_to_bytes,
+                          string_to_bool)
 
 
 __all__ = [
     'udev_version', 'Context', 'Enumerator', 'Device', 'Attributes',
     'DeviceNotFoundError', 'DeviceNotFoundAtPathError',
     'DeviceNotFoundByNameError', 'DeviceNotFoundInEnvironmentError']
 
@@ -68,15 +69,15 @@
     not be executed.  Raise :exc:`subprocess.CalledProcessError`, if
     ``udevadm`` returned a non-zero exit code.
 
     .. versionadded:: 0.8
     """
     command = ['udevadm', '--version']
     udevadm = Popen(command, stdout=PIPE)
-    stdout = assert_unicode(udevadm.communicate()[0]).strip()
+    stdout = ensure_unicode_string(udevadm.communicate()[0]).strip()
     if udevadm.returncode != 0:
         raise CalledProcessError(0, command)
     return int(stdout)
 
 
 class Context(object):
     """
@@ -101,24 +102,45 @@
     def sys_path(self):
         """
         The ``sysfs`` mount point defaulting to ``/sys'`` as unicode string.
 
         The mount point can be overwritten using the environment variable
         :envvar:`SYSFS_PATH`.  Use this for testing purposes.
         """
-        return assert_unicode(libudev.udev_get_sys_path(self._context))
+        return ensure_unicode_string(libudev.udev_get_sys_path(self._context))
 
     @property
     def device_path(self):
         """
         The device directory path defaulting to ``/dev`` as unicode string.
 
         This can be overridden in the udev configuration.
         """
-        return assert_unicode(libudev.udev_get_dev_path(self._context))
+        return ensure_unicode_string(libudev.udev_get_dev_path(self._context))
+
+    @property
+    def log_priority(self):
+        """
+        The logging priority of the interal logging facitility of udev as
+        integer with a standard :mod:`syslog` priority.  Assign to this
+        property to change the logging priority.
+
+        UDev uses the standard :mod:`syslog` priorities.  Constants for these
+        priorities are defined in the :mod:`syslog` module in the standard
+        library:
+
+        >>> import syslog
+        >>> context = pyudev.Context()
+        >>> context.log_priority = syslog.LOG_DEBUG
+        """
+        return libudev.udev_get_log_priority(self._context)
+
+    @log_priority.setter
+    def log_priority(self, value):
+        libudev.udev_set_log_priority(self._context, value)
 
     def list_devices(self, **kwargs):
         """
         List all available devices.
 
         The arguments of this method are the same as for
         :meth:`Enumerator.match()`.  In fact, the arguments are simply passed
@@ -218,29 +240,29 @@
 
         ``subsystem`` is either a unicode string or a byte string,
         containing the name of the subsystem.
 
         Return the instance again.
         """
         libudev.udev_enumerate_add_match_subsystem(
-            self._enumerator, assert_bytes(subsystem))
+            self._enumerator, ensure_byte_string(subsystem))
         return self
 
     def match_sys_name(self, sys_name):
         """
         Include all devices with the given name.
 
         ``sys_name`` is a byte or unicode string containing the device name.
 
         Return the instance again.
 
         .. versionadded:: 0.8
         """
         libudev.udev_enumerate_add_match_sysname(self._enumerator,
-                                                 assert_bytes(sys_name))
+                                                 ensure_byte_string(sys_name))
         return self
 
     def match_property(self, property, value):
         """
         Include all devices, whose ``property`` has the given ``value``.
 
         ``property`` is either a unicode string or a byte string, containing
@@ -251,15 +273,15 @@
         - :func:`bool`
         - A unicode or byte string
         - Anything convertable to a byte string
 
         Return the instance again.
         """
         libudev.udev_enumerate_add_match_property(
-            self._enumerator, assert_bytes(property),
+            self._enumerator, ensure_byte_string(property),
             property_value_to_bytes(value))
         return self
 
     def match_tag(self, tag):
         """
         Include all devices, which have the given ``tag`` attached.
 
@@ -268,15 +290,15 @@
         Return the instance again.
 
         .. versionadded:: 0.6
 
         .. udevminversion:: 154
         """
         libudev.udev_enumerate_add_match_tag(self._enumerator,
-                                             assert_bytes(tag))
+                                             ensure_byte_string(tag))
         return self
 
     def match_is_initialized(self):
         """
         Include only devices, which are initialized.
 
         Initialized devices have properly set device node permissions and
@@ -450,25 +472,26 @@
         Device(u'/sys/devices/platform')
 
         ``context`` is the :class:`Context` in which to search the device.
         ``sys_path`` is a unicode or byte string containing the path of the
         device inside ``sysfs`` with the mount point included.
 
         Return a :class:`Device` object for the device.  Raise
-        :exc:`DeviceNotFoundAtPathError`, if no device was found for ``sys_path``.
+        :exc:`DeviceNotFoundAtPathError`, if no device was found for
+        ``sys_path``.
 
         .. versionchanged:: 0.4
            Raise :exc:`NoSuchDeviceError` instead of returning ``None``, if
            no device was found for ``sys_path``
         .. versionchanged:: 0.5
            Raise :exc:`DeviceNotFoundAtPathError` instead of
            :exc:`NoSuchDeviceError`
         """
         device = libudev.udev_device_new_from_syspath(
-            context._context, assert_bytes(sys_path))
+            context._context, ensure_byte_string(sys_path))
         if not device:
             raise DeviceNotFoundAtPathError(sys_path)
         return cls(context, device)
 
     @classmethod
     def from_name(cls, context, subsystem, sys_name):
         """
@@ -488,16 +511,16 @@
         Return a :class:`Device` object for the device.  Raise
         :exc:`DeviceNotFoundByNameError`, if no device was found with the given
         name.
 
         .. versionadded:: 0.5
         """
         device = libudev.udev_device_new_from_subsystem_sysname(
-            context._context, assert_bytes(subsystem),
-            assert_bytes(sys_name))
+            context._context, ensure_byte_string(subsystem),
+            ensure_byte_string(sys_name))
         if not device:
             raise DeviceNotFoundByNameError(subsystem, sys_name)
         return cls(context, device)
 
     @classmethod
     def from_environment(cls, context):
         """
@@ -561,14 +584,42 @@
 
         Return an iterable yielding a :class:`Device` object for each direct
         child of this device.
         """
         for device in self.context.list_devices().match_children(self):
             yield device
 
+    def find_parent(self, subsystem, device_type=None):
+        """
+        Find the parent device with the given ``subsystem`` and
+        ``device_type``.
+
+        ``subsystem`` is a byte or unicode string containing the name of the
+        subsystem, in which to search for the parent.  ``device_type`` is a
+        byte or unicode string holding the expected device type of the parent.
+        It can be ``None`` (the default), which means, that no specific device
+        type is expected.
+
+        Return a parent :class:`Device` within the given ``subsystem`` and – if
+        ``device_type`` is not ``None`` – with the given ``device_type``, or
+        ``None``, if this device has no parent device matching these
+        constraints.
+
+        .. versionadded:: 0.9
+        """
+        subsystem = ensure_byte_string(subsystem)
+        if device_type is not None:
+            device_type = ensure_byte_string(device_type)
+        parent = libudev.udev_device_get_parent_with_subsystem_devtype(
+            self._device, subsystem, device_type)
+        if not parent:
+            return None
+        # parent device is not referenced, thus forcibly acquire a reference
+        return Device(self.context, libudev.udev_device_ref(parent))
+
     def traverse(self):
         """
         Traverse all parent devices of this device from bottom to top.
 
         Return an iterable yielding all parent devices as :class:`Device`
         objects, *not* including the current device.  The last yielded
         :class:`Device` is the top of the device hierarchy.
@@ -580,53 +631,57 @@
 
     @property
     def sys_path(self):
         """
         Absolute path of this device in ``sysfs`` including the ``sysfs``
         mount point as unicode string.
         """
-        return assert_unicode(libudev.udev_device_get_syspath(self._device))
+        return ensure_unicode_string(
+            libudev.udev_device_get_syspath(self._device))
 
     @property
     def device_path(self):
         """
         Kernel device path as unicode string.  This path uniquely identifies
         a single device.
 
         Unlike :attr:`sys_path`, this path does not contain the ``sysfs``
         mount point.  However, the path is absolute and starts with a slash
         ``'/'``.
         """
-        return assert_unicode(libudev.udev_device_get_devpath(self._device))
+        return ensure_unicode_string(
+            libudev.udev_device_get_devpath(self._device))
 
     @property
     def subsystem(self):
         """
         Name of the subsystem this device is part of as unicode string.
         """
-        return assert_unicode(libudev.udev_device_get_subsystem(self._device))
+        return ensure_unicode_string(
+            libudev.udev_device_get_subsystem(self._device))
 
     @property
     def sys_name(self):
         """
         Device file name inside ``sysfs`` as unicode string.
         """
-        return assert_unicode(libudev.udev_device_get_sysname(self._device))
+        return ensure_unicode_string(
+            libudev.udev_device_get_sysname(self._device))
 
     @property
     def driver(self):
         """
         The driver name as unicode string, or ``None``, if there is no
         driver for this device.
 
         .. versionadded:: 0.5
         """
         driver = libudev.udev_device_get_driver(self._device)
         if driver:
-            return assert_unicode(driver)
+            return ensure_unicode_string(driver)
 
     @property
     def device_node(self):
         """
         Absolute path to the device node of this device as unicode string or
         ``None``, if this device doesn't have a device node.  The path
         includes the device directory (see :attr:`Context.device_path`).
@@ -634,15 +689,15 @@
         This path always points to the actual device node associated with
         this device, and never to any symbolic links to this device node.
         See :attr:`device_links` to get a list of symbolic links to this
         device node.
         """
         node = libudev.udev_device_get_devnode(self._device)
         if node:
-            return assert_unicode(node)
+            return ensure_unicode_string(node)
 
     @property
     def is_initialized(self):
         """
         ``True``, if the device is initialized, ``False`` otherwise.
 
         A device is initialized, if udev has already handled this device and
@@ -696,15 +751,15 @@
         removeable media, which technically do not have a constant device
         node, or to map a single device into multiple device hierarchies.
         The property provides access to all such symbolic links, which were
         created by UDev for this device.
         """
         entry = libudev.udev_device_get_devlinks_list_entry(self._device)
         for name in udev_list_iterate(entry):
-            yield assert_unicode(name)
+            yield ensure_unicode_string(name)
 
     @property
     def attributes(self):
         """
         The system attributes of this device as read-only
         :class:`Attributes` mapping.
 
@@ -728,26 +783,26 @@
 
         .. versionadded:: 0.6
 
         .. udevminversion:: 154
         """
         entry = libudev.udev_device_get_tags_list_entry(self._device)
         for tag in udev_list_iterate(entry):
-            yield assert_unicode(tag)
+            yield ensure_unicode_string(tag)
 
     def __iter__(self):
         """
         Iterate over the names of all properties defined for this device.
 
         Return a generator yielding the names of all properties of this
         device as unicode strings.
         """
         entry = libudev.udev_device_get_properties_list_entry(self._device)
         for name in udev_list_iterate(entry):
-            yield assert_unicode(name)
+            yield ensure_unicode_string(name)
 
     def __len__(self):
         """
         Return the amount of properties defined for this device as integer.
         """
         entry = libudev.udev_device_get_properties_list_entry(self._device)
         counter = count()
@@ -763,18 +818,18 @@
         property.
 
         Return the property value as unicode string, or raise a
         :exc:`~exceptions.KeyError`, if the given property is not defined
         for this device.
         """
         value = libudev.udev_device_get_property_value(
-            self._device, assert_bytes(property))
+            self._device, ensure_byte_string(property))
         if value is None:
             raise KeyError('No such property: {0}'.format(property))
-        return assert_unicode(value)
+        return ensure_unicode_string(value)
 
     def asint(self, property):
         """
         Get the given ``property`` from this device as integer.
 
         ``property`` is a unicode or byte string containing the name of the
         property.
@@ -884,29 +939,29 @@
 
         Yield each attribute name as unicode string.
         """
         return iter(self._attribute_files)
 
     def __contains__(self, attribute):
         return libudev.udev_device_get_sysattr_value(
-            self.device._device, assert_bytes(attribute)) is not None
+            self.device._device, ensure_byte_string(attribute)) is not None
 
     def __getitem__(self, attribute):
         """
         Get the given system ``attribute`` for the device.
 
         ``attribute`` is a unicode or byte string containing the name of the
         system attribute.
 
         Return the attribute value as byte string, or raise a
         :exc:`~exceptions.KeyError`, if the given attribute is not defined
         for this device.
         """
         value = libudev.udev_device_get_sysattr_value(
-            self.device._device, assert_bytes(attribute))
+            self.device._device, ensure_byte_string(attribute))
         if value is None:
             raise KeyError('No such attribute: {0}'.format(attribute))
         return value
 
     def asstring(self, attribute):
         """
         Get the given ``atribute`` for the device as unicode string.
@@ -918,15 +973,15 @@
         attribute.
 
         Return the attribute value as byte string.  Raise a
         :exc:`~exceptions.KeyError`, if the given attribute is not defined
         for this device, or :exc:`~exceptions.UnicodeDecodeError`, if the
         content of the attribute cannot be decoded into a unicode string.
         """
-        return assert_unicode(self[attribute])
+        return ensure_unicode_string(self[attribute])
 
     def asint(self, attribute):
         """
         Get the given ``attribute`` as integer.
 
         ``attribute`` is a unicode or byte string containing the name of the
         attribute.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyudev-0.8/pyudev/_util.py` & `pyudev-0.9/pyudev/_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,28 +30,28 @@
                         absolute_import)
 
 import sys
 
 from pyudev._libudev import libudev
 
 
-def assert_bytes(value):
+def ensure_byte_string(value):
     """
     Return the given ``value`` as bytestring.
 
     If the given ``value`` is not a byte string, but a real unicode string, it
     is encoded with the filesystem encoding (as in
     :func:`sys.getfilesystemencoding()`).
     """
     if not isinstance(value, bytes):
         value = value.encode(sys.getfilesystemencoding())
     return value
 
 
-def assert_unicode(value):
+def ensure_unicode_string(value):
     """
     Return the given ``value`` as unicode string.
 
     If the given ``value`` is not a unicode string, but a byte string, it is
     decoded with the filesystem encoding (as in
     :func:`sys.getfilesystemencoding()`).
     """
@@ -64,24 +64,25 @@
     """
     Return a byte string, which represents the given ``value`` in a way
     suitable as raw value of an udev property.
 
     If ``value`` is a boolean object, it is converted to ``'1'`` or ``'0'``,
     depending on whether ``value`` is ``True`` or ``False``.  If ``value`` is a
     byte string already, it is returned unchanged.  Anything else is simply
-    converted to a unicode string, and then passed to :func:`assert_bytes`.
+    converted to a unicode string, and then passed to
+    :func:`ensure_byte_string`.
     """
     # udev represents boolean values as 1 or 0, therefore an explicit
     # conversion to int is required for boolean values
     if isinstance(value, bool):
         value = int(value)
     if isinstance(value, bytes):
         return value
     else:
-        return assert_bytes(unicode(value))
+        return ensure_byte_string(unicode(value))
 
 
 def string_to_bool(value):
     """
     Convert the given unicode string ``value`` to a boolean object.
 
     If ``value`` is ``'1'``, ``True`` is returned.  If ``value`` is ``'0'``,
```

### Comparing `pyudev-0.8/pyudev/_libudev.py` & `pyudev-0.9/pyudev/_libudev.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,15 +81,17 @@
 SIGNATURES = {
     # context
     'udev': dict(
         new=(None, udev_p),
         unref=([udev_p], None),
         ref=([udev_p], udev_p),
         get_sys_path=([udev_p], c_char_p),
-        get_dev_path=([udev_p], c_char_p)),
+        get_dev_path=([udev_p], c_char_p),
+        get_log_priority=([udev_p], c_int),
+        set_log_priority=([udev_p, c_int], None)),
     # enumeration
     'udev_enumerate': dict(
         new=([udev_p], udev_enumerate_p),
         ref=([udev_enumerate_p], udev_enumerate_p),
         unref=([udev_enumerate_p], None),
         add_match_subsystem=([udev_enumerate_p, c_char_p], c_int),
         add_match_property=([udev_enumerate_p, c_char_p, c_char_p], c_int),
@@ -108,14 +110,16 @@
         ref=([udev_device_p], udev_device_p),
         unref=([udev_device_p], None),
         new_from_syspath=([udev_p, c_char_p], udev_device_p),
         new_from_subsystem_sysname=([udev_p, c_char_p, c_char_p],
                                     udev_device_p),
         new_from_environment=([udev_p], udev_device_p),
         get_parent=([udev_device_p], udev_device_p),
+        get_parent_with_subsystem_devtype=([udev_device_p, c_char_p, c_char_p],
+                                           udev_device_p),
         get_devpath=([udev_device_p], c_char_p),
         get_subsystem=([udev_device_p], c_char_p),
         get_syspath=([udev_device_p], c_char_p),
         get_sysname=([udev_device_p], c_char_p),
         get_driver=([udev_device_p], c_char_p),
         get_devnode=([udev_device_p], c_char_p),
         get_property_value=([udev_device_p, c_char_p], c_char_p),
@@ -132,15 +136,16 @@
         unref=([udev_monitor_p], None),
         new_from_netlink=([udev_p, c_char_p], udev_monitor_p),
         new_from_socket=([udev_p, c_char_p], udev_monitor_p),
         enable_receiving=([udev_monitor_p], c_int),
         get_fd=([udev_monitor_p], c_int),
         receive_device=([udev_monitor_p], udev_device_p),
         filter_add_match_subsystem_devtype=(
-            [udev_monitor_p, c_char_p, c_char_p], c_int))
+            [udev_monitor_p, c_char_p, c_char_p], c_int),
+        filter_add_match_tag=([udev_monitor_p, c_char_p], c_int))
     }
 
 
 def check_negative_errorcode(result, func, *args):
     """
     Check if ``result`` is ``0``.  If so, return normally.  Otherwise interpret
     ``result`` as negative error code, and raise
@@ -158,26 +163,32 @@
 
 ERROR_CHECKERS = dict(
     udev_enumerate_add_match_subsystem=check_negative_errorcode,
     udev_enumerate_add_match_property=check_negative_errorcode,
     udev_enumerate_add_match_tag=check_negative_errorcode,
     udev_enumerate_add_match_sysname=check_negative_errorcode,
     udev_enumerate_add_match_is_initialized=check_negative_errorcode,
-    udev_monitor_filter_add_match_subsystem_devtype=check_negative_errorcode)
+    udev_monitor_filter_add_match_subsystem_devtype=check_negative_errorcode,
+    udev_monitor_filter_add_match_tag=check_negative_errorcode)
 
 
 def load_udev_library():
     """
     Load the ``udev`` library and return a :class:`ctypes.CDLL` object for
     it.  The library has errno handling enabled.
 
     Important functions are given proper signatures and return types to
     support type checking and argument conversion.
+
+    Raise :exc:`~exceptions.ImportError`, if the udev library was not found.
     """
-    libudev = CDLL(find_library('udev'), use_errno=True)
+    udev_library_name = find_library('udev')
+    if not udev_library_name:
+        raise ImportError('No library named udev')
+    libudev = CDLL(udev_library_name, use_errno=True)
     # context function signature
     for namespace, members in SIGNATURES.items():
         for funcname in members:
             fullname = '{0}_{1}'.format(namespace, funcname)
             func = getattr(libudev, fullname, None)
             if func:
                 argtypes, restype = members[funcname]
```

### Comparing `pyudev-0.8/pyudev.egg-info/PKG-INFO` & `pyudev-0.9/pyudev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: pyudev
-Version: 0.8
+Version: 0.9
 Summary: A libudev binding
 Home-page: http://packages.python.org/pyudev
 Author: Sebastian Wiesner
 Author-email: lunaryorn@googlemail.com
 License: MIT/X11
 Description: ######
         pyudev
```

### Comparing `pyudev-0.8/pyudev.egg-info/SOURCES.txt` & `pyudev-0.9/pyudev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/doc/api/context.rst` & `pyudev-0.9/doc/api/context.rst`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
    .. automethod:: __init__
 
    .. autoattribute:: sys_path
 
    .. autoattribute:: device_path
 
+   .. autoattribute:: log_priority
+
    .. automethod:: list_devices
 
 .. autoclass:: Enumerator()
 
    .. automethod:: match
 
    .. automethod:: match_subsystem
```

### Comparing `pyudev-0.8/doc/api/monitor.rst` & `pyudev-0.9/doc/api/monitor.rst`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
       .. versionadded:: 0.5
 
    .. automethod:: fileno
 
    .. automethod:: filter_by
 
+   .. automethod:: filter_by_tag
+
    .. automethod:: enable_receiving
 
    .. method:: start
 
       Alias for :meth:`enable_receiving`
 
    .. automethod:: receive_device
```

### Comparing `pyudev-0.8/doc/api/toolkit.rst` & `pyudev-0.9/doc/api/toolkit.rst`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/doc/api/device.rst` & `pyudev-0.9/doc/api/device.rst`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 
    .. autoattribute:: parent
 
    .. autoattribute:: children
 
    .. automethod:: traverse
 
+   .. automethod:: find_parent
+
    .. automethod:: __iter__
 
    .. automethod:: __len__
 
    .. automethod:: __getitem__
 
    .. automethod:: asint
```

### Comparing `pyudev-0.8/doc/api/index.rst` & `pyudev-0.9/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/doc/conf.py` & `pyudev-0.9/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 project = u'pyudev'
 copyright = u'2010, 2011 Sebastian Wiesner'
 version = '.'.join(pyudev.__version__.split('.')[:2])
 release = pyudev.__version__
 
 html_theme = 'default'
 html_static_path = []
-html_domain_indices = ['py-modindex']
 
 intersphinx_mapping = {'python': ('http://docs.python.org/', None)}
 
 issuetracker = 'github'
 issuetracker_user = 'lunaryorn'
```

### Comparing `pyudev-0.8/doc/Makefile` & `pyudev-0.9/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/doc/index.rst` & `pyudev-0.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/distribute_setup.py` & `pyudev-0.9/distribute_setup.py`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/COPYING` & `pyudev-0.9/COPYING`

 * *Files identical despite different names*

### Comparing `pyudev-0.8/library_path_wrapper.py` & `pyudev-0.9/library_path_wrapper.py`

 * *Files identical despite different names*

