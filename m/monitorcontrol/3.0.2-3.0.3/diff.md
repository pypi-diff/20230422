# Comparing `tmp/monitorcontrol-3.0.2.tar.gz` & `tmp/monitorcontrol-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monitorcontrol-3.0.2.tar", max compression
+gzip compressed data, was "monitorcontrol-3.0.3.tar", max compression
```

## Comparing `monitorcontrol-3.0.2.tar` & `monitorcontrol-3.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1077 2022-11-05 16:40:44.839724 monitorcontrol-3.0.2/LICENSE
--rw-r--r--   0        0        0     1387 2022-11-05 16:40:44.839724 monitorcontrol-3.0.2/README.rst
--rw-r--r--   0        0        0      213 2022-11-05 16:40:44.839724 monitorcontrol-3.0.2/monitorcontrol/__init__.py
--rw-r--r--   0        0        0     5639 2022-11-05 16:40:44.843724 monitorcontrol-3.0.2/monitorcontrol/__main__.py
--rw-r--r--   0        0        0    17388 2022-11-05 16:40:44.843724 monitorcontrol-3.0.2/monitorcontrol/monitorcontrol.py
--rw-r--r--   0        0        0      328 2022-11-05 16:40:44.843724 monitorcontrol-3.0.2/monitorcontrol/vcp/__init__.py
--rw-r--r--   0        0        0     1385 2022-11-05 16:40:44.843724 monitorcontrol-3.0.2/monitorcontrol/vcp/vcp_abc.py
--rw-r--r--   0        0        0     2702 2022-11-05 16:40:44.843724 monitorcontrol-3.0.2/monitorcontrol/vcp/vcp_codes.py
--rw-r--r--   0        0        0    11735 2022-11-05 16:40:44.843724 monitorcontrol-3.0.2/monitorcontrol/vcp/vcp_linux.py
--rw-r--r--   0        0        0     6182 2022-11-05 16:40:44.843724 monitorcontrol-3.0.2/monitorcontrol/vcp/vcp_windows.py
--rw-r--r--   0        0        0      893 2022-11-05 16:40:44.843724 monitorcontrol-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     2266 2022-11-05 16:41:20.208320 monitorcontrol-3.0.2/setup.py
--rw-r--r--   0        0        0     2123 2022-11-05 16:41:20.208579 monitorcontrol-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/LICENSE
+-rw-r--r--   0        0        0     1419 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/README.rst
+-rw-r--r--   0        0        0      213 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/monitorcontrol/__init__.py
+-rw-r--r--   0        0        0     5639 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/monitorcontrol/__main__.py
+-rw-r--r--   0        0        0    17388 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/monitorcontrol/monitorcontrol.py
+-rw-r--r--   0        0        0      328 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/monitorcontrol/vcp/__init__.py
+-rw-r--r--   0        0        0     1385 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/monitorcontrol/vcp/vcp_abc.py
+-rw-r--r--   0        0        0     2702 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/monitorcontrol/vcp/vcp_codes.py
+-rw-r--r--   0        0        0    12039 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/monitorcontrol/vcp/vcp_linux.py
+-rw-r--r--   0        0        0     6182 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/monitorcontrol/vcp/vcp_windows.py
+-rw-r--r--   0        0        0      975 2023-04-22 19:22:27.026720 monitorcontrol-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2207 1970-01-01 00:00:00.000000 monitorcontrol-3.0.3/PKG-INFO
```

### Comparing `monitorcontrol-3.0.2/LICENSE` & `monitorcontrol-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `monitorcontrol-3.0.2/README.rst` & `monitorcontrol-3.0.3/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 -  Windows (tested with Windows 10)
 
 Windows Install
 ***************
 
 .. code-block:: bash
 
-   py -3.8 -m pip install monitorcontrol
+   py -3 -m pip install monitorcontrol
 
 Linux Install
 *************
 
 .. code-block:: bash
 
-   python3.8 -m pip install monitorcontrol
+   python3 -m pip install monitorcontrol
 
 Documentation
 *************
 
 Full documentation including examples are avaliable in the `docs <https://newam.github.io/monitorcontrol>`__.
 
 .. |PyPi Version| image:: https://badge.fury.io/py/monitorcontrol.svg
    :target: https://badge.fury.io/py/monitorcontrol
-.. |Build Status| image:: https://travis-ci.com/newAM/monitorcontrol.svg?branch=master
-   :target: https://travis-ci.com/newAM/monitorcontrol
+.. |Build Status| image:: https://github.com/newAM/monitorcontrol/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/newAM/monitorcontrol/actions/workflows/ci.yml
 .. |Coverage Status| image:: https://coveralls.io/repos/github/newAM/monitorcontrol/badge.svg?branch=master
    :target: https://coveralls.io/github/newAM/monitorcontrol?branch=master
 .. |Documentation Status| image:: https://img.shields.io/badge/docs-latest-blue
    :target: https://newam.github.io/monitorcontrol
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
```

### Comparing `monitorcontrol-3.0.2/monitorcontrol/__main__.py` & `monitorcontrol-3.0.3/monitorcontrol/__main__.py`

 * *Files identical despite different names*

### Comparing `monitorcontrol-3.0.2/monitorcontrol/monitorcontrol.py` & `monitorcontrol-3.0.3/monitorcontrol/monitorcontrol.py`

 * *Files identical despite different names*

### Comparing `monitorcontrol-3.0.2/monitorcontrol/vcp/vcp_abc.py` & `monitorcontrol-3.0.3/monitorcontrol/vcp/vcp_abc.py`

 * *Files identical despite different names*

### Comparing `monitorcontrol-3.0.2/monitorcontrol/vcp/vcp_codes.py` & `monitorcontrol-3.0.3/monitorcontrol/vcp/vcp_codes.py`

 * *Files identical despite different names*

### Comparing `monitorcontrol-3.0.2/monitorcontrol/vcp/vcp_linux.py` & `monitorcontrol-3.0.3/monitorcontrol/vcp/vcp_linux.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,28 +52,39 @@
         """
         Args:
             bus_number: I2C bus number.
         """
         self.logger = logging.getLogger(__name__)
         self.bus_number = bus_number
         self.fd: Optional[str] = None
-        self.fp = None
+        self.fp: str = f"/dev/i2c-{self.bus_number}"
         # time of last feature set call
         self.last_set: Optional[float] = None
 
     def __enter__(self):
+        def cleanup(fd: Optional[int]):
+            if fd is not None:
+                try:
+                    os.close(self.fd)
+                except OSError:
+                    pass
+
         try:
-            self.fp = f"/dev/i2c-{self.bus_number}"
             self.fd = os.open(self.fp, os.O_RDWR)
             fcntl.ioctl(self.fd, self.I2C_SLAVE, self.DDCCI_ADDR)
             self.read_bytes(1)
         except PermissionError as e:
+            cleanup(self.fd)
             raise VCPPermissionError(f"permission error for {self.fp}") from e
         except OSError as e:
+            cleanup(self.fd)
             raise VCPIOError(f"unable to open VCP at {self.fp}") from e
+        except Exception as e:
+            cleanup(self.fd)
+            raise e
         return self
 
     def __exit__(
         self,
         exception_type: Optional[Type[BaseException]],
         exception_value: Optional[BaseException],
         exception_traceback: Optional[TracebackType],
```

### Comparing `monitorcontrol-3.0.2/monitorcontrol/vcp/vcp_windows.py` & `monitorcontrol-3.0.3/monitorcontrol/vcp/vcp_windows.py`

 * *Files identical despite different names*

### Comparing `monitorcontrol-3.0.2/pyproject.toml` & `monitorcontrol-3.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.black]
 line-length = 79
 target-version = ["py36", "py37", "py38"]
 
 [tool.poetry]
 name = "monitorcontrol"
 description = "Monitor controls using MCCS over DDC-CI."
-version = "3.0.2"
+version = "3.0.3"
 authors = ["Alex Martens <alex@thinglab.org>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/newAM/monitorcontrol"
 documentation = "https://newam.github.io/monitorcontrol"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyudev = { version = ">=0.23,<0.25", markers = "sys_platform != 'win32'" }
 
 [tool.poetry.dev-dependencies]
-black = "22.10.0"
+black = "23.3.0"
 coveralls = "^3"
-flake8 = "^5"
-flake8-bugbear = "^22"
+flake8 = { version = "^6", python = ">=3.8.1,<4.0" }
+flake8-bugbear = { version = "^23.3.23", python = ">=3.8.1,<4.0" }
 pep8-naming = "~0.13"
 pytest = "^7"
 pytest-cov = "^4"
-sphinx = "^5.3"
+sphinx = "^6.1"
 sphinx-rtd-theme = "^1"
 toml = "~0.10"
 voluptuous = "~0.13"
 
 [tool.poetry.scripts]
 monitorcontrol = "monitorcontrol.__main__:main"
```

### Comparing `monitorcontrol-3.0.2/setup.py` & `monitorcontrol-3.0.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,63 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: monitorcontrol
+Version: 3.0.3
+Summary: Monitor controls using MCCS over DDC-CI.
+Home-page: https://github.com/newAM/monitorcontrol
+License: MIT
+Author: Alex Martens
+Author-email: alex@thinglab.org
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyudev (>=0.23,<0.25) ; sys_platform != "win32"
+Project-URL: Documentation, https://newam.github.io/monitorcontrol
+Project-URL: Repository, https://github.com/newAM/monitorcontrol
+Description-Content-Type: text/x-rst
+
+monitorcontrol
+##############
+
+|PyPi Version| |Build Status| |Documentation Status| |Coverage Status| |Black|
+
+Python monitor control using the VESA Monitor Control Command Set (MCCS)
+over the Display Data Channel Command Interface Standard (DDC-CI).
+
+Supported Platforms
+*******************
+-  Linux (tested with NixOS)
+-  Windows (tested with Windows 10)
+
+Windows Install
+***************
+
+.. code-block:: bash
+
+   py -3 -m pip install monitorcontrol
+
+Linux Install
+*************
+
+.. code-block:: bash
+
+   python3 -m pip install monitorcontrol
+
+Documentation
+*************
+
+Full documentation including examples are avaliable in the `docs <https://newam.github.io/monitorcontrol>`__.
+
+.. |PyPi Version| image:: https://badge.fury.io/py/monitorcontrol.svg
+   :target: https://badge.fury.io/py/monitorcontrol
+.. |Build Status| image:: https://github.com/newAM/monitorcontrol/actions/workflows/ci.yml/badge.svg
+   :target: https://github.com/newAM/monitorcontrol/actions/workflows/ci.yml
+.. |Coverage Status| image:: https://coveralls.io/repos/github/newAM/monitorcontrol/badge.svg?branch=master
+   :target: https://coveralls.io/github/newAM/monitorcontrol?branch=master
+.. |Documentation Status| image:: https://img.shields.io/badge/docs-latest-blue
+   :target: https://newam.github.io/monitorcontrol
+.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
 
-packages = \
-['monitorcontrol', 'monitorcontrol.vcp']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{':sys_platform != "win32"': ['pyudev>=0.23,<0.25']}
-
-entry_points = \
-{'console_scripts': ['monitorcontrol = monitorcontrol.__main__:main']}
-
-setup_kwargs = {
-    'name': 'monitorcontrol',
-    'version': '3.0.2',
-    'description': 'Monitor controls using MCCS over DDC-CI.',
-    'long_description': 'monitorcontrol\n##############\n\n|PyPi Version| |Build Status| |Documentation Status| |Coverage Status| |Black|\n\nPython monitor control using the VESA Monitor Control Command Set (MCCS)\nover the Display Data Channel Command Interface Standard (DDC-CI).\n\nSupported Platforms\n*******************\n-  Linux (tested with NixOS)\n-  Windows (tested with Windows 10)\n\nWindows Install\n***************\n\n.. code-block:: bash\n\n   py -3.8 -m pip install monitorcontrol\n\nLinux Install\n*************\n\n.. code-block:: bash\n\n   python3.8 -m pip install monitorcontrol\n\nDocumentation\n*************\n\nFull documentation including examples are avaliable in the `docs <https://newam.github.io/monitorcontrol>`__.\n\n.. |PyPi Version| image:: https://badge.fury.io/py/monitorcontrol.svg\n   :target: https://badge.fury.io/py/monitorcontrol\n.. |Build Status| image:: https://travis-ci.com/newAM/monitorcontrol.svg?branch=master\n   :target: https://travis-ci.com/newAM/monitorcontrol\n.. |Coverage Status| image:: https://coveralls.io/repos/github/newAM/monitorcontrol/badge.svg?branch=master\n   :target: https://coveralls.io/github/newAM/monitorcontrol?branch=master\n.. |Documentation Status| image:: https://img.shields.io/badge/docs-latest-blue\n   :target: https://newam.github.io/monitorcontrol\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n',
-    'author': 'Alex Martens',
-    'author_email': 'alex@thinglab.org',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/newAM/monitorcontrol',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

