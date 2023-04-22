# Comparing `tmp/humanreadable-0.2.0.tar.gz` & `tmp/humanreadable-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanreadable-0.2.0.tar", last modified: Sat Feb 11 17:02:45 2023, max compression
+gzip compressed data, was "humanreadable-0.3.0.tar", last modified: Sat Apr 22 17:38:07 2023, max compression
```

## Comparing `humanreadable-0.2.0.tar` & `humanreadable-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-11 17:02:45.051149 humanreadable-0.2.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:00.000000 humanreadable-0.2.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      179 2021-03-20 04:14:00.000000 humanreadable-0.2.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     6922 2023-02-11 17:02:45.051149 humanreadable-0.2.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     5395 2023-02-11 15:56:30.000000 humanreadable-0.2.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-11 17:02:45.041149 humanreadable-0.2.0/humanreadable/
--rw-r--r--   0 toor      (1000) toor      (1000)      199 2021-03-20 04:14:00.000000 humanreadable-0.2.0/humanreadable/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-02-11 16:08:49.000000 humanreadable-0.2.0/humanreadable/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3816 2023-02-11 16:56:40.000000 humanreadable-0.2.0/humanreadable/_base.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7899 2023-02-11 15:13:25.000000 humanreadable-0.2.0/humanreadable/_persec.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6854 2023-02-11 15:15:27.000000 humanreadable-0.2.0/humanreadable/_time.py
--rw-r--r--   0 toor      (1000) toor      (1000)   109604 2023-02-11 16:54:11.000000 humanreadable-0.2.0/humanreadable/_typing.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1416 2023-02-11 06:36:23.000000 humanreadable-0.2.0/humanreadable/error.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-02-11 15:16:58.000000 humanreadable-0.2.0/humanreadable/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-11 17:02:45.041149 humanreadable-0.2.0/humanreadable.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     6922 2023-02-11 17:02:44.000000 humanreadable-0.2.0/humanreadable.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      546 2023-02-11 17:02:45.000000 humanreadable-0.2.0/humanreadable.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-02-11 17:02:44.000000 humanreadable-0.2.0/humanreadable.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       54 2023-02-11 17:02:44.000000 humanreadable-0.2.0/humanreadable.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       14 2023-02-11 17:02:44.000000 humanreadable-0.2.0/humanreadable.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1187 2023-02-11 16:54:38.000000 humanreadable-0.2.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-11 17:02:45.051149 humanreadable-0.2.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       17 2021-07-17 12:51:45.000000 humanreadable-0.2.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-02-11 06:14:30.000000 humanreadable-0.2.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-02-11 17:02:45.051149 humanreadable-0.2.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2692 2023-02-11 16:44:47.000000 humanreadable-0.2.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-11 17:02:45.051149 humanreadable-0.2.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)     9253 2023-02-11 06:36:23.000000 humanreadable-0.2.0/test/test_persec.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5326 2021-03-20 04:14:00.000000 humanreadable-0.2.0/test/test_time.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1057 2023-02-11 16:55:07.000000 humanreadable-0.2.0/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-04-22 17:37:50.000000 humanreadable-0.3.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      179 2023-04-22 17:37:50.000000 humanreadable-0.3.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     7460 2023-04-22 17:38:07.723380 humanreadable-0.3.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     5940 2023-04-22 17:37:50.000000 humanreadable-0.3.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/humanreadable/
+-rw-r--r--   0 toor      (1000) toor      (1000)      430 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3952 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8273 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/_persec.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9298 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/_time.py
+-rw-r--r--   0 toor      (1000) toor      (1000)   109604 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/_typing.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1416 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-04-22 17:37:50.000000 humanreadable-0.3.0/humanreadable/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/humanreadable.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     7460 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      546 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       54 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       14 2023-04-22 17:38:07.000000 humanreadable-0.3.0/humanreadable.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1230 2023-04-22 17:37:50.000000 humanreadable-0.3.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)       17 2023-04-22 17:37:50.000000 humanreadable-0.3.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-04-22 17:37:50.000000 humanreadable-0.3.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-04-22 17:38:07.723380 humanreadable-0.3.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2730 2023-04-22 17:37:50.000000 humanreadable-0.3.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-04-22 17:38:07.723380 humanreadable-0.3.0/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)     9861 2023-04-22 17:37:50.000000 humanreadable-0.3.0/test/test_persec.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6658 2023-04-22 17:37:50.000000 humanreadable-0.3.0/test/test_time.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1055 2023-04-22 17:37:50.000000 humanreadable-0.3.0/tox.ini
```

### Comparing `humanreadable-0.2.0/LICENSE` & `humanreadable-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `humanreadable-0.2.0/PKG-INFO` & `humanreadable-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: humanreadable
-Version: 0.2.0
-Summary: humanreadable is a Python library to convert from human-readable values to Python values.
+Version: 0.3.0
+Summary: humanreadable is a Python library to convert human-readable values to other units.
 Home-page: https://github.com/thombashi/humanreadable
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/humanreadable
 Project-URL: Tracker, https://github.com/thombashi/humanreadable/issues
 Keywords: human-readable,converter
@@ -67,44 +67,62 @@
 - time (days, hours, minutes, seconds, etc.)
 - bits per second
 
 
 Usage
 ============================================
 
-Basic usages
--------------------------------------------
+Convert a human-readable value to another unit
+----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import humanreadable as hr
 
         print("\n[Examples: humanreadable.Time]")
         value = "120 sec"
         print("'{}' to msecs -> {}".format(value, hr.Time(value).milliseconds))
         print("'{}' to minutes -> {}".format(value, hr.Time(value).minutes))
 
-        print("\n[Examples: humanreadable.BitPerSecond]")
+        value = "12 min 40 sec"
+        print("'{}' to seconds -> {}".format(value, hr.Time(value).seconds))
+
+        print("\n[Examples: humanreadable.BitsPerSecond]")
         value = "1 Gbps"
-        print("'{}' to Mbps -> {}".format(value, hr.BitPerSecond(value).mega_bps))
-        print("'{}' to Kbps -> {}".format(value, hr.BitPerSecond(value).kilo_bps))
-        print("'{}' to Kibps -> {}".format(value, hr.BitPerSecond(value).kibi_bps))
+        print("'{}' to Mbps -> {}".format(value, hr.BitsPerSecond(value).mega_bps))
+        print("'{}' to Kbps -> {}".format(value, hr.BitsPerSecond(value).kilo_bps))
+        print("'{}' to Kibps -> {}".format(value, hr.BitsPerSecond(value).kibi_bps))
 
 :Output:
     .. code-block::
 
         [Examples: humanreadable.Time]
         '120 sec' to msecs -> 120000.0
         '120 sec' to minutes -> 2.0
+        '12 minutes 40 seconds' to seconds -> 760.0
 
-        [Examples: humanreadable.BitPerSecond]
+        [Examples: humanreadable.BitsPerSecond]
         '1 Gbps' to Mbps -> 1000.0
         '1 Gbps' to Kbps -> 1000000.0
-        '1 Gbps' to Kibps -> 953674.31640625
+        '1 Gbps' to Kibps -> 976562.5
+
+
+Convert a value to a human readable string
+----------------------------------------------
+:Sample Code:
+    .. code-block:: python
+
+        import humanreadable as hr
+
+        hr.Time("400", default_unit=hr.Time.Unit.SECOND).to_humanreadable()
+
+:Output:
+    .. code-block::
 
+        6 minutes 40 seconds
 
 Set default unit
 -------------------------------------------
 Unit for an instance is determined by input value.
 If a valid unit is not found, ``default_unit`` will be used for the instance (defaults to ``None``).
 
 :Sample Code:
@@ -136,37 +154,37 @@
     |seconds     |``s``/``sec``/``secs``/``second``/``seconds``             |
     +------------+----------------------------------------------------------+
     |milliseconds|``ms``/``msec``/``msecs``/``millisecond``/``milliseconds``|
     +------------+----------------------------------------------------------+
     |microseconds|``us``/``usec``/``usecs``/``microsecond``/``microseconds``|
     +------------+----------------------------------------------------------+
 
-.. table:: Available units for ``humanreadable.BitPerSecond``
+.. table:: Available units for ``humanreadable.BitsPerSecond``
 
-    +-----+---------------------------+
-    |Unit |Available specifiers (str) |
-    +=====+===========================+
-    |bps  |``bps``/``bit/s``          |
-    +-----+---------------------------+
-    |Kbps |``[kK]bps``/``[kK]bit/s``  |
-    +-----+---------------------------+
-    |Kibps|``[kK]ibps``/``[kK]ibit/s``|
-    +-----+---------------------------+
-    |Mbps |``[mM]bps``/``[mM]bit/s``  |
-    +-----+---------------------------+
-    |Mibps|``[mM]ibps``/``[mM]ibit/s``|
-    +-----+---------------------------+
-    |Gbps |``[gG]bps``/``[gG]bit/s``  |
-    +-----+---------------------------+
-    |Gibps|``[gG]ibps``/``[gG]ibit/s``|
-    +-----+---------------------------+
-    |Tbps |``[tT]bps``/``[tT]bit/s``  |
-    +-----+---------------------------+
-    |Tibps|``[tT]ibps``/``[tT]ibit/s``|
-    +-----+---------------------------+
+    +-----+-----------------------------+
+    |Unit |Available specifiers (str)   |
+    +=====+=============================+
+    |bps  |``bps``/``bits?/s``          |
+    +-----+-----------------------------+
+    |Kbps |``[kK]bps``/``[kK]bits?/s``  |
+    +-----+-----------------------------+
+    |Kibps|``[kK]ibps``/``[kK]ibits?/s``|
+    +-----+-----------------------------+
+    |Mbps |``[mM]bps``/``[mM]bits?/s``  |
+    +-----+-----------------------------+
+    |Mibps|``[mM]ibps``/``[mM]ibits?/s``|
+    +-----+-----------------------------+
+    |Gbps |``[gG]bps``/``[gG]bits?/s``  |
+    +-----+-----------------------------+
+    |Gibps|``[gG]ibps``/``[gG]ibits?/s``|
+    +-----+-----------------------------+
+    |Tbps |``[tT]bps``/``[tT]bits?/s``  |
+    +-----+-----------------------------+
+    |Tibps|``[tT]ibps``/``[tT]ibits?/s``|
+    +-----+-----------------------------+
 
 
 Installation
 ============================================
 Installation: pip
 ------------------------------
 ::
@@ -180,9 +198,9 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-humanreadable
 
 
 Dependencies
 ============================================
-- Python 3.7+
+- Python 3.6+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/humanreadable/network/dependencies>`__
```

### Comparing `humanreadable-0.2.0/README.rst` & `humanreadable-0.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -33,44 +33,62 @@
 - time (days, hours, minutes, seconds, etc.)
 - bits per second
 
 
 Usage
 ============================================
 
-Basic usages
--------------------------------------------
+Convert a human-readable value to another unit
+----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import humanreadable as hr
 
         print("\n[Examples: humanreadable.Time]")
         value = "120 sec"
         print("'{}' to msecs -> {}".format(value, hr.Time(value).milliseconds))
         print("'{}' to minutes -> {}".format(value, hr.Time(value).minutes))
 
-        print("\n[Examples: humanreadable.BitPerSecond]")
+        value = "12 min 40 sec"
+        print("'{}' to seconds -> {}".format(value, hr.Time(value).seconds))
+
+        print("\n[Examples: humanreadable.BitsPerSecond]")
         value = "1 Gbps"
-        print("'{}' to Mbps -> {}".format(value, hr.BitPerSecond(value).mega_bps))
-        print("'{}' to Kbps -> {}".format(value, hr.BitPerSecond(value).kilo_bps))
-        print("'{}' to Kibps -> {}".format(value, hr.BitPerSecond(value).kibi_bps))
+        print("'{}' to Mbps -> {}".format(value, hr.BitsPerSecond(value).mega_bps))
+        print("'{}' to Kbps -> {}".format(value, hr.BitsPerSecond(value).kilo_bps))
+        print("'{}' to Kibps -> {}".format(value, hr.BitsPerSecond(value).kibi_bps))
 
 :Output:
     .. code-block::
 
         [Examples: humanreadable.Time]
         '120 sec' to msecs -> 120000.0
         '120 sec' to minutes -> 2.0
+        '12 minutes 40 seconds' to seconds -> 760.0
 
-        [Examples: humanreadable.BitPerSecond]
+        [Examples: humanreadable.BitsPerSecond]
         '1 Gbps' to Mbps -> 1000.0
         '1 Gbps' to Kbps -> 1000000.0
-        '1 Gbps' to Kibps -> 953674.31640625
+        '1 Gbps' to Kibps -> 976562.5
+
+
+Convert a value to a human readable string
+----------------------------------------------
+:Sample Code:
+    .. code-block:: python
+
+        import humanreadable as hr
+
+        hr.Time("400", default_unit=hr.Time.Unit.SECOND).to_humanreadable()
+
+:Output:
+    .. code-block::
 
+        6 minutes 40 seconds
 
 Set default unit
 -------------------------------------------
 Unit for an instance is determined by input value.
 If a valid unit is not found, ``default_unit`` will be used for the instance (defaults to ``None``).
 
 :Sample Code:
@@ -102,37 +120,37 @@
     |seconds     |``s``/``sec``/``secs``/``second``/``seconds``             |
     +------------+----------------------------------------------------------+
     |milliseconds|``ms``/``msec``/``msecs``/``millisecond``/``milliseconds``|
     +------------+----------------------------------------------------------+
     |microseconds|``us``/``usec``/``usecs``/``microsecond``/``microseconds``|
     +------------+----------------------------------------------------------+
 
-.. table:: Available units for ``humanreadable.BitPerSecond``
+.. table:: Available units for ``humanreadable.BitsPerSecond``
 
-    +-----+---------------------------+
-    |Unit |Available specifiers (str) |
-    +=====+===========================+
-    |bps  |``bps``/``bit/s``          |
-    +-----+---------------------------+
-    |Kbps |``[kK]bps``/``[kK]bit/s``  |
-    +-----+---------------------------+
-    |Kibps|``[kK]ibps``/``[kK]ibit/s``|
-    +-----+---------------------------+
-    |Mbps |``[mM]bps``/``[mM]bit/s``  |
-    +-----+---------------------------+
-    |Mibps|``[mM]ibps``/``[mM]ibit/s``|
-    +-----+---------------------------+
-    |Gbps |``[gG]bps``/``[gG]bit/s``  |
-    +-----+---------------------------+
-    |Gibps|``[gG]ibps``/``[gG]ibit/s``|
-    +-----+---------------------------+
-    |Tbps |``[tT]bps``/``[tT]bit/s``  |
-    +-----+---------------------------+
-    |Tibps|``[tT]ibps``/``[tT]ibit/s``|
-    +-----+---------------------------+
+    +-----+-----------------------------+
+    |Unit |Available specifiers (str)   |
+    +=====+=============================+
+    |bps  |``bps``/``bits?/s``          |
+    +-----+-----------------------------+
+    |Kbps |``[kK]bps``/``[kK]bits?/s``  |
+    +-----+-----------------------------+
+    |Kibps|``[kK]ibps``/``[kK]ibits?/s``|
+    +-----+-----------------------------+
+    |Mbps |``[mM]bps``/``[mM]bits?/s``  |
+    +-----+-----------------------------+
+    |Mibps|``[mM]ibps``/``[mM]ibits?/s``|
+    +-----+-----------------------------+
+    |Gbps |``[gG]bps``/``[gG]bits?/s``  |
+    +-----+-----------------------------+
+    |Gibps|``[gG]ibps``/``[gG]ibits?/s``|
+    +-----+-----------------------------+
+    |Tbps |``[tT]bps``/``[tT]bits?/s``  |
+    +-----+-----------------------------+
+    |Tibps|``[tT]ibps``/``[tT]ibits?/s``|
+    +-----+-----------------------------+
 
 
 Installation
 ============================================
 Installation: pip
 ------------------------------
 ::
@@ -146,9 +164,9 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-humanreadable
 
 
 Dependencies
 ============================================
-- Python 3.7+
+- Python 3.6+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/humanreadable/network/dependencies>`__
```

### Comparing `humanreadable-0.2.0/humanreadable/_base.py` & `humanreadable-0.3.0/humanreadable/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 
 from typepy import RealNumber, String
 
 from .error import ParameterError, UnitNotFoundError
 
 
 try:
-    from typing import Protocol
+    from typing import Final, Protocol
 except ImportError:
-    # typing.Protocol is only available starting from Python 3.8.
-    from ._typing import Protocol  # type: ignore
+    # typing.Final and typing.Protocol are only available starting from Python 3.8.
+    from ._typing import Final, Protocol  # type: ignore
 
 
 class SupportsUnit(Protocol):
     @property
-    def name(self) -> str:
+    def name(self) -> str:  # pragma: no cover
         ...
 
     @property
-    def regexp(self) -> Pattern:
+    def regexp(self) -> Pattern:  # pragma: no cover
         ...
 
 
 Units = List[str]
 TextUnitsMap = Dict[SupportsUnit, Units]
 
 
-_RE_NUMBER = re.compile(r"^[-\+]?[0-9\.]+$")
+_RE_NUMBER: Final[Pattern] = re.compile(r"^[-\+]?[0-9\.]+$")
 
 
 def _get_unit_msg(text_units: TextUnitsMap) -> str:
     return ", ".join([", ".join(values) for values in text_units.values()])
 
 
 class HumanReadableValue(metaclass=abc.ABCMeta):
@@ -49,15 +49,17 @@
     def _units(self) -> List[SupportsUnit]:  # pragma: no cover
         pass
 
     @abc.abstractmethod
     def get_as(self, unit: Union[str, SupportsUnit]) -> float:  # pragma: no cover
         pass
 
-    def __init__(self, readable_value: str, default_unit=None) -> None:
+    def __init__(
+        self, readable_value: str, default_unit: Union[str, SupportsUnit, None] = None
+    ) -> None:
         self._default_unit = self._normalize_unit(default_unit)
         self._number, self._from_unit = self.__preprocess(readable_value)
 
     def __repr__(self) -> str:
         items = [str(self._number)]
         if self._from_unit.name:
             items.append(self._from_unit.name)
```

### Comparing `humanreadable-0.2.0/humanreadable/_persec.py` & `humanreadable-0.3.0/humanreadable/_persec.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 from decimal import Decimal
 from typing import Dict, List, NamedTuple, Optional, Pattern, Union, cast
 
 from ._base import HumanReadableValue, SupportsUnit, TextUnitsMap
 
 
 _PATTERN_TEMPLETE = r"\s?{}$"
+_BPS_PATTERN = r"bits?(/|\s?per\s?)(s|sec|second)"
 
-_BPS_STR_UNITS = ["bps", "bit/s"]
-_KBPS_STR_UNITS = ["[kK]bps", "[kK]bit/s"]
-_KIBPS_STR_UNITS = ["[kK]ibps", "[kK]ibit/s"]
-_MBPS_STR_UNITS = ["[mM]bps", "[mM]bit/s"]
-_MIBPS_STR_UNITS = ["[mM]ibps", "[mM]ibit/s"]
-_GBPS_STR_UNITS = ["[gG]bps", "[gG]bit/s"]
-_GIBPS_STR_UNITS = ["[gG]ibps", "[gG]ibit/s"]
-_TBPS_STR_UNITS = ["[tT]bps", "[tT]bit/s"]
-_TIBPS_STR_UNITS = ["[tT]ibps", "[tT]ibit/s"]
+_BPS_STR_UNITS = ["bps", _BPS_PATTERN]
+_KBPS_STR_UNITS = ["[kK]bps", "[kK]" + _BPS_PATTERN]
+_KIBPS_STR_UNITS = ["[kK]ibps", "[kK]i" + _BPS_PATTERN]
+_MBPS_STR_UNITS = ["[mM]bps", "[mM]" + _BPS_PATTERN]
+_MIBPS_STR_UNITS = ["[mM]ibps", "[mM]i" + _BPS_PATTERN]
+_GBPS_STR_UNITS = ["[gG]bps", "[gG]" + _BPS_PATTERN]
+_GIBPS_STR_UNITS = ["[gG]ibps", "[gG]i" + _BPS_PATTERN]
+_TBPS_STR_UNITS = ["[tT]bps", "[tT]" + _BPS_PATTERN]
+_TIBPS_STR_UNITS = ["[tT]ibps", "[tT]i" + _BPS_PATTERN]
 
 
 class ByteUnit(NamedTuple):
     name: str
     regexp: Pattern
     kilo_size: int
     factor: int
@@ -235,14 +236,18 @@
 
     def __gt__(self, other) -> bool:
         return self.bps > other.bps
 
     def __ge__(self, other) -> bool:
         return self.bps >= other.bps
 
+    def __add__(self, other: "BitPerSecond") -> "BitPerSecond":
+        number = self._number + Decimal(other.get_as(self._from_unit))
+        return BitPerSecond(str(number), default_unit=self._from_unit)
+
     def get_as(self, unit: Union[str, SupportsUnit]) -> float:
         unit_maps: Dict[SupportsUnit, str] = {
             self.Unit.BPS: "bps",
             self.Unit.KBPS: "kilo_bps",
             self.Unit.KIBPS: "kibi_bps",
             self.Unit.MBPS: "mega_bps",
             self.Unit.MIBPS: "mebi_bps",
@@ -266,7 +271,10 @@
         from_unit_bu = cast(ByteUnit, from_unit)
         if from_unit_bu.kilo_size == to_unit.kilo_size:
             return Decimal(from_unit_bu.kilo_size ** (from_unit_bu.factor - to_unit.factor))
 
         return Decimal(from_unit_bu.kilo_size**from_unit_bu.factor) / Decimal(
             to_unit.kilo_size**to_unit.factor
         )
+
+
+BitsPerSecond = BitPerSecond
```

### Comparing `humanreadable-0.2.0/humanreadable/_time.py` & `humanreadable-0.3.0/humanreadable/_time.py`

 * *Files 22% similar despite different names*

```diff
@@ -140,14 +140,29 @@
             self.Unit.HOUR,
             self.Unit.MINUTE,
             self.Unit.SECOND,
             self.Unit.MILLISECOND,
             self.Unit.MICROSECOND,
         ]
 
+    def __init__(
+        self, readable_value: str, default_unit: Union[str, SupportsUnit, None] = None
+    ) -> None:
+        values = re.findall(r"\d+\s*[a-zA-Z]+", readable_value)
+        if len(values) <= 1:
+            super().__init__(readable_value, default_unit)
+            return
+
+        t = _parse(readable_value, default_unit)
+        self._default_unit = t._default_unit
+        self._number = t._number
+        self._from_unit = t._from_unit
+
+        assert self._default_unit
+
     def __eq__(self, other) -> bool:
         return self.microseconds == other.microseconds
 
     def __ne__(self, other) -> bool:
         return self.microseconds != other.microseconds
 
     def __lt__(self, other) -> bool:
@@ -158,14 +173,18 @@
 
     def __gt__(self, other) -> bool:
         return self.microseconds > other.microseconds
 
     def __ge__(self, other) -> bool:
         return self.microseconds >= other.microseconds
 
+    def __add__(self, other: "Time") -> "Time":
+        number = self._number + Decimal(other.get_as(self._from_unit))
+        return Time(str(number), default_unit=self._from_unit)
+
     def validate(self, min_value=None, max_value=None):
         if min_value is not None:
             if not isinstance(min_value, Time):
                 min_value = Time(min_value)
 
             if self < min_value:
                 raise ParameterError(
@@ -195,20 +214,74 @@
             self.Unit.MICROSECOND: "microseconds",
         }
         norm_unit = self._normalize_unit(unit)
         assert norm_unit
 
         return getattr(self, unit_maps[norm_unit])
 
+    def to_humanreadable(self, style: str = "full") -> str:
+        def _to_unit_str(unit, style: str) -> str:
+            if style in ("short", "abbr"):
+                return unit.name[0]
+
+            if style == "full":
+                return f" {unit.name}"
+
+            return unit.name
+
+        style = style.strip().lower()
+        items = []
+
+        if self.days >= 1:
+            items.append(f"{self.days:d}{_to_unit_str(self.Unit.DAY, style)}")
+        if self.hours % 24 >= 1:
+            items.append(f"{int(self.hours) % 24:d}{_to_unit_str(self.Unit.HOUR, style)}")
+        if self.minutes % 60 >= 1:
+            items.append(f"{int(self.minutes) % 60:d}{_to_unit_str(self.Unit.MINUTE, style)}")
+        if self.seconds % 60 >= 1:
+            items.append(f"{int(self.seconds) % 60:d}{_to_unit_str(self.Unit.SECOND, style)}")
+        if self.milliseconds % 1000 >= 1:
+            items.append(
+                f"{int(self.milliseconds) % 1000:d}{_to_unit_str(self.Unit.MILLISECOND, style)}"
+            )
+        if self.microseconds % 1000 >= 1:
+            items.append(
+                f"{int(self.microseconds) % 1000:d}{_to_unit_str(self.Unit.MICROSECOND, style)}"
+            )
+
+        if not items:
+            assert self._default_unit
+            return f"0 {self._default_unit.name}"
+
+        return " ".join(items)
+
     def _normalize_unit(self, unit: Union[str, SupportsUnit, None]) -> Optional[SupportsUnit]:
         if isinstance(unit, TimeUnit):
             return unit
 
         return super()._normalize_unit(unit)
 
     def __calc_coef(self, from_unit: SupportsUnit, to_unit: TimeUnit) -> Decimal:
         from_unit_tu = cast(TimeUnit, from_unit)
         thousand_coef = Decimal(1000 ** (to_unit.thousand_factor - from_unit_tu.thousand_factor))
         sixty_coef = Decimal(60 ** (to_unit.sixty_factor - from_unit_tu.sixty_factor))
         day_coef = Decimal(24 ** (to_unit.day_factor - from_unit_tu.day_factor))
 
         return day_coef * sixty_coef * thousand_coef
+
+
+def _parse(value: Union[str, Time], default_unit: Union[str, SupportsUnit, None] = None) -> Time:
+    if isinstance(value, Time):
+        return value
+
+    sum: Optional[Time] = None
+
+    for item in reversed(re.findall(r"\d+\s*[a-zA-Z]+", value)):
+        t = Time(item, default_unit=default_unit)
+        if sum is None:
+            sum = t
+        else:
+            sum += t
+
+    assert sum is not None
+
+    return sum
```

### Comparing `humanreadable-0.2.0/humanreadable/_typing.py` & `humanreadable-0.3.0/humanreadable/_typing.py`

 * *Files identical despite different names*

### Comparing `humanreadable-0.2.0/humanreadable/error.py` & `humanreadable-0.3.0/humanreadable/error.py`

 * *Files identical despite different names*

### Comparing `humanreadable-0.2.0/humanreadable.egg-info/PKG-INFO` & `humanreadable-0.3.0/humanreadable.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: humanreadable
-Version: 0.2.0
-Summary: humanreadable is a Python library to convert from human-readable values to Python values.
+Version: 0.3.0
+Summary: humanreadable is a Python library to convert human-readable values to other units.
 Home-page: https://github.com/thombashi/humanreadable
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/humanreadable
 Project-URL: Tracker, https://github.com/thombashi/humanreadable/issues
 Keywords: human-readable,converter
@@ -67,44 +67,62 @@
 - time (days, hours, minutes, seconds, etc.)
 - bits per second
 
 
 Usage
 ============================================
 
-Basic usages
--------------------------------------------
+Convert a human-readable value to another unit
+----------------------------------------------
 :Sample Code:
     .. code-block:: python
 
         import humanreadable as hr
 
         print("\n[Examples: humanreadable.Time]")
         value = "120 sec"
         print("'{}' to msecs -> {}".format(value, hr.Time(value).milliseconds))
         print("'{}' to minutes -> {}".format(value, hr.Time(value).minutes))
 
-        print("\n[Examples: humanreadable.BitPerSecond]")
+        value = "12 min 40 sec"
+        print("'{}' to seconds -> {}".format(value, hr.Time(value).seconds))
+
+        print("\n[Examples: humanreadable.BitsPerSecond]")
         value = "1 Gbps"
-        print("'{}' to Mbps -> {}".format(value, hr.BitPerSecond(value).mega_bps))
-        print("'{}' to Kbps -> {}".format(value, hr.BitPerSecond(value).kilo_bps))
-        print("'{}' to Kibps -> {}".format(value, hr.BitPerSecond(value).kibi_bps))
+        print("'{}' to Mbps -> {}".format(value, hr.BitsPerSecond(value).mega_bps))
+        print("'{}' to Kbps -> {}".format(value, hr.BitsPerSecond(value).kilo_bps))
+        print("'{}' to Kibps -> {}".format(value, hr.BitsPerSecond(value).kibi_bps))
 
 :Output:
     .. code-block::
 
         [Examples: humanreadable.Time]
         '120 sec' to msecs -> 120000.0
         '120 sec' to minutes -> 2.0
+        '12 minutes 40 seconds' to seconds -> 760.0
 
-        [Examples: humanreadable.BitPerSecond]
+        [Examples: humanreadable.BitsPerSecond]
         '1 Gbps' to Mbps -> 1000.0
         '1 Gbps' to Kbps -> 1000000.0
-        '1 Gbps' to Kibps -> 953674.31640625
+        '1 Gbps' to Kibps -> 976562.5
+
+
+Convert a value to a human readable string
+----------------------------------------------
+:Sample Code:
+    .. code-block:: python
+
+        import humanreadable as hr
+
+        hr.Time("400", default_unit=hr.Time.Unit.SECOND).to_humanreadable()
+
+:Output:
+    .. code-block::
 
+        6 minutes 40 seconds
 
 Set default unit
 -------------------------------------------
 Unit for an instance is determined by input value.
 If a valid unit is not found, ``default_unit`` will be used for the instance (defaults to ``None``).
 
 :Sample Code:
@@ -136,37 +154,37 @@
     |seconds     |``s``/``sec``/``secs``/``second``/``seconds``             |
     +------------+----------------------------------------------------------+
     |milliseconds|``ms``/``msec``/``msecs``/``millisecond``/``milliseconds``|
     +------------+----------------------------------------------------------+
     |microseconds|``us``/``usec``/``usecs``/``microsecond``/``microseconds``|
     +------------+----------------------------------------------------------+
 
-.. table:: Available units for ``humanreadable.BitPerSecond``
+.. table:: Available units for ``humanreadable.BitsPerSecond``
 
-    +-----+---------------------------+
-    |Unit |Available specifiers (str) |
-    +=====+===========================+
-    |bps  |``bps``/``bit/s``          |
-    +-----+---------------------------+
-    |Kbps |``[kK]bps``/``[kK]bit/s``  |
-    +-----+---------------------------+
-    |Kibps|``[kK]ibps``/``[kK]ibit/s``|
-    +-----+---------------------------+
-    |Mbps |``[mM]bps``/``[mM]bit/s``  |
-    +-----+---------------------------+
-    |Mibps|``[mM]ibps``/``[mM]ibit/s``|
-    +-----+---------------------------+
-    |Gbps |``[gG]bps``/``[gG]bit/s``  |
-    +-----+---------------------------+
-    |Gibps|``[gG]ibps``/``[gG]ibit/s``|
-    +-----+---------------------------+
-    |Tbps |``[tT]bps``/``[tT]bit/s``  |
-    +-----+---------------------------+
-    |Tibps|``[tT]ibps``/``[tT]ibit/s``|
-    +-----+---------------------------+
+    +-----+-----------------------------+
+    |Unit |Available specifiers (str)   |
+    +=====+=============================+
+    |bps  |``bps``/``bits?/s``          |
+    +-----+-----------------------------+
+    |Kbps |``[kK]bps``/``[kK]bits?/s``  |
+    +-----+-----------------------------+
+    |Kibps|``[kK]ibps``/``[kK]ibits?/s``|
+    +-----+-----------------------------+
+    |Mbps |``[mM]bps``/``[mM]bits?/s``  |
+    +-----+-----------------------------+
+    |Mibps|``[mM]ibps``/``[mM]ibits?/s``|
+    +-----+-----------------------------+
+    |Gbps |``[gG]bps``/``[gG]bits?/s``  |
+    +-----+-----------------------------+
+    |Gibps|``[gG]ibps``/``[gG]ibits?/s``|
+    +-----+-----------------------------+
+    |Tbps |``[tT]bps``/``[tT]bits?/s``  |
+    +-----+-----------------------------+
+    |Tibps|``[tT]ibps``/``[tT]ibits?/s``|
+    +-----+-----------------------------+
 
 
 Installation
 ============================================
 Installation: pip
 ------------------------------
 ::
@@ -180,9 +198,9 @@
     sudo add-apt-repository ppa:thombashi/ppa
     sudo apt update
     sudo apt install python3-humanreadable
 
 
 Dependencies
 ============================================
-- Python 3.7+
+- Python 3.6+
 - `Python package dependencies (automatically installed) <https://github.com/thombashi/humanreadable/network/dependencies>`__
```

### Comparing `humanreadable-0.2.0/humanreadable.egg-info/SOURCES.txt` & `humanreadable-0.3.0/humanreadable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `humanreadable-0.2.0/pyproject.toml` & `humanreadable-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     'pass',
     'ABCmeta',
     'abstractmethod',
     'abstractproperty',
     'abstractclassmethod',
     'warnings.warn',
 ]
+omit = [
+    'humanreadable/_typing.py',
+]
 
 [tool.isort]
 known_third_party = [
     'pytest'
 ]
 include_trailing_comma = true
 line_length = 100
@@ -52,15 +55,15 @@
     '*/.pytype/*',
     '*/.tox/*',
     'humanreadable/_typing.py',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.6
+python_version = 3.8
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 warn_unused_configs = true
```

### Comparing `humanreadable-0.2.0/setup.py` & `humanreadable-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "humanreadable"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class():
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -37,15 +37,15 @@
 setuptools.setup(
     name=MODULE_NAME,
     version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
     description=(
-        "humanreadable is a Python library to convert from human-readable values to Python values."
+        "humanreadable is a Python library to convert human-readable values to other units."
     ),
     include_package_data=True,
     keywords=["human-readable", "converter"],
     license=pkg_info["__license__"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
```

### Comparing `humanreadable-0.2.0/test/test_persec.py` & `humanreadable-0.3.0/test/test_persec.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import sys
 from decimal import Decimal
 
 import pytest
 
-from humanreadable import BitPerSecond, ParameterError, UnitNotFoundError
+from humanreadable import BitPerSecond, BitsPerSecond, ParameterError, UnitNotFoundError
 
 
 KILO = Decimal(1000**1)
 MEGA = Decimal(1000**2)
 GIGA = Decimal(1000**3)
 TERA = Decimal(1000**4)
 KIBI = Decimal(1024**1)
@@ -40,32 +40,58 @@
     )
     def test_exception(self, value, exception):
         with pytest.raises(exception):
             BitPerSecond(value).bps
 
 
 class Test_BitPerSecond_repr:
-    @pytest.mark.parametrize(["value", "expected"], [["2 Kbps", "2 Kbps"]])
+    @pytest.mark.parametrize(
+        ["value", "expected"],
+        [
+            ["2 Kbps", "2 Kbps"],
+        ],
+    )
     def test_exception(self, value, expected):
         assert str(BitPerSecond(value)) == expected
 
 
-class Test_eq:
+class Test_BitPerSecond_eq:
     @pytest.mark.parametrize(
         ["lhs", "rhs", "expected"],
-        [["5 bps", "5.0 bit/s", True], ["60000bps", "60 Kbps", True], ["1 bps", "2 bps", False]],
+        [
+            ["5 bps", "5.0 bit/s", True],
+            ["5.0 bit/s", "5 bits/sec", True],
+            ["60000bps", "60 Kbps", True],
+            ["1 bps", "2 bps", False],
+        ],
     )
     def test_exception(self, lhs, rhs, expected):
         assert (BitPerSecond(lhs) == BitPerSecond(rhs)) is expected
+        assert (BitPerSecond(lhs) == BitsPerSecond(rhs)) is expected
 
 
-class Test_less_than:
+class Test_BitPerSecond_add:
     @pytest.mark.parametrize(
         ["lhs", "rhs", "expected"],
-        [["20 Gbps", "32Gbps", True], ["20 Gibps", "32Gbps", True], ["40 Gibps", "32Gbps", False]],
+        [
+            ["1Kbps", "1 Kbits/sec", "2 Kbps"],
+        ],
+    )
+    def test_exception(self, lhs, rhs, expected):
+        assert (BitPerSecond(lhs) + BitPerSecond(rhs)) == BitPerSecond(expected)
+
+
+class Test_BitPerSecond_less_than:
+    @pytest.mark.parametrize(
+        ["lhs", "rhs", "expected"],
+        [
+            ["20 Gbps", "32Gbps", True],
+            ["20 Gibps", "32Gbps", True],
+            ["40 Gibps", "32Gbps", False],
+        ],
     )
     def test_exception(self, lhs, rhs, expected):
         lhs = BitPerSecond(lhs)
         rhs = BitPerSecond(rhs)
 
         print(f"lhs={lhs.mega_bps}Mbps, rhs={rhs.mega_bps}Mbps", file=sys.stderr)
 
@@ -267,15 +293,15 @@
     )
     def test_normal_gibi(self, value, expected):
         value = BitPerSecond(value)
         assert value.tebi_bps == expected
         assert value.tebi_byte_per_sec == value.tebi_bps / 8
 
 
-class Test_Time_get_as:
+class Test_BitPerSecond_get_as:
     @pytest.mark.parametrize(
         ["value", "default_unit", "expected"],
         [
             ["2bps", BitPerSecond.Unit.BPS, 2],
             ["2Kbps", BitPerSecond.Unit.KBPS, 2],
             ["2Kibps", BitPerSecond.Unit.KIBPS, 2],
             ["2Mbps", BitPerSecond.Unit.MBPS, 2],
```

### Comparing `humanreadable-0.2.0/test/test_time.py` & `humanreadable-0.3.0/test/test_time.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import pytest
 
 from humanreadable import ParameterError, Time
 
 
-class Test_constructor:
+class Test_Time_constructor:
     @pytest.mark.parametrize(
         ["value", "exception"],
         [
             [None, TypeError],
             [True, TypeError],
             [float("nan"), TypeError],
             ["", ParameterError],
@@ -23,47 +23,87 @@
         ],
     )
     def test_exception(self, value, exception):
         with pytest.raises(exception):
             Time(value)
 
 
-class Test_repr:
-    @pytest.mark.parametrize(["value", "expected"], [["5seconds", "5 seconds"]])
+class Test_Time_repr:
+    @pytest.mark.parametrize(
+        ["value", "expected"],
+        [
+            ["5seconds", "5 seconds"],
+        ],
+    )
     def test_exception(self, value, expected):
         assert str(Time(value)) == expected
 
 
-class Test_eq:
+class Test_Time_eq:
     @pytest.mark.parametrize(
         ["lhs", "rhs", "expected"],
-        [["5seconds", "5.0 sec", True], ["60000ms", "1min", True], ["1 sec", "2 sec", False]],
+        [
+            ["5seconds", "5.0 sec", True],
+            ["60000ms", "1min", True],
+            ["1 sec", "2 sec", False],
+        ],
     )
     def test_exception(self, lhs, rhs, expected):
         assert (Time(lhs) == Time(rhs)) is expected
 
 
+class Test_Time_add:
+    @pytest.mark.parametrize(
+        ["lhs", "rhs", "expected"],
+        [
+            ["1s", "1seconds", "2 sec"],
+            ["1s", "1000ms", "2 sec"],
+        ],
+    )
+    def test_exception(self, lhs, rhs, expected):
+        assert (Time(lhs) + Time(rhs)) == Time(expected)
+
+
 class Test_Time_days:
-    @pytest.mark.parametrize(["value", "expected"], [["12hours", 0.5], ["1day", 1], ["3 days", 3]])
+    @pytest.mark.parametrize(
+        ["value", "expected"],
+        [
+            ["12hours", 0.5],
+            ["1day", 1],
+            ["3 days", 3],
+        ],
+    )
     def test_normal(self, value, expected):
         assert Time(value).days == expected
 
 
 class Test_Time_hours:
     @pytest.mark.parametrize(
         ["value", "expected"],
-        [["3600 seconds", 1], ["30minutes", 0.5], ["2hours", 2], ["1day", 24], ["3 days", 72]],
+        [
+            ["3600 seconds", 1],
+            ["30minutes", 0.5],
+            ["2hours", 2],
+            ["1day", 24],
+            ["3 days", 72],
+        ],
     )
     def test_normal(self, value, expected):
         assert Time(value).hours == expected
 
 
 class Test_Time_minutes:
     @pytest.mark.parametrize(
-        ["value", "expected"], [["30 seconds", 0.5], ["60000ms", 1], ["1m", 1], ["2hour", 120]]
+        ["value", "expected"],
+        [
+            ["30 seconds", 0.5],
+            ["60000ms", 1],
+            ["1m", 1],
+            ["2hour", 120],
+        ],
     )
     def test_normal(self, value, expected):
         assert Time(value).minutes == expected
 
 
 class Test_Time_seconds:
     @pytest.mark.parametrize(
@@ -72,14 +112,19 @@
             ["1s", 1],
             ["123 seconds", 123],
             ["1000ms", 1],
             ["123000 MSEC", 123],
             ["123000000 usecs", 123],
             ["1m", 60],
             ["2hour", 7200],
+            ["12m40s", 760],
+            ["12m 40s", 760],
+            ["12min 40sec", 760],
+            ["12 minutes 40 seconds", 760],
+            ["1 hour 12 minutes 40 seconds", 4360],
         ],
     )
     def test_normal(self, value, expected):
         assert Time(value).seconds == expected
 
     @pytest.mark.parametrize(
         ["value", "default_unit", "expected"],
@@ -173,7 +218,20 @@
             ["2", Time.Unit.SECOND, 2],
             ["2", Time.Unit.MILLISECOND, 2],
             ["2", Time.Unit.MICROSECOND, 2],
         ],
     )
     def test_normal_default_unit(self, value, default_unit, expected):
         assert Time(value, default_unit=default_unit).get_as(default_unit) == expected
+
+
+class Test_Time_to_humanreadable:
+    @pytest.mark.parametrize(
+        ["value", "default_unit", "style", "expected"],
+        [
+            ["0", Time.Unit.SECOND, "full", "0 seconds"],
+            ["4000", Time.Unit.SECOND, "full", "1 hours 6 minutes 40 seconds"],
+            ["4000", Time.Unit.SECOND, "short", "1h 6m 40s"],
+        ],
+    )
+    def test_normal_default_unit(self, value, default_unit, style, expected):
+        assert Time(value, default_unit=default_unit).to_humanreadable(style=style) == expected
```

### Comparing `humanreadable-0.2.0/tox.ini` & `humanreadable-0.3.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:fmt]
 skip_install = true
 deps =
-    autoflake>=1.4
+    autoflake>=2
     black[jupyter]>=23.1
     isort>=5
 commands =
     black setup.py examples test humanreadable
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
```

