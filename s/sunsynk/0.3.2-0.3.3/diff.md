# Comparing `tmp/sunsynk-0.3.2.tar.gz` & `tmp/sunsynk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunsynk-0.3.2.tar", last modified: Thu Apr 20 20:06:59 2023, max compression
+gzip compressed data, was "sunsynk-0.3.3.tar", last modified: Sat Apr 22 20:28:34 2023, max compression
```

## Comparing `sunsynk-0.3.2.tar` & `sunsynk-0.3.3.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.554793 sunsynk-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 20:06:50.000000 sunsynk-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-20 20:06:50.000000 sunsynk-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-20 20:06:59.554793 sunsynk-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-20 20:06:50.000000 sunsynk-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-20 20:06:59.554793 sunsynk-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-20 20:06:50.000000 sunsynk-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.550792 sunsynk-0.3.2/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12513 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/pysunsynk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6273 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-20 20:06:50.000000 sunsynk-0.3.2/sunsynk/usunsynk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.550792 sunsynk-0.3.2/sunsynk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 20:06:59.000000 sunsynk-0.3.2/sunsynk.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.550792 sunsynk-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk-dev.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.550792 sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/hass-addon-sunsynk.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:59.554793 sunsynk-0.3.2/tests/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 20:06:50.000000 sunsynk-0.3.2/tests/sunsynk/test_sunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.037470 sunsynk-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-22 20:28:24.000000 sunsynk-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 20:28:24.000000 sunsynk-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-22 20:28:34.037470 sunsynk-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-22 20:28:24.000000 sunsynk-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-22 20:28:34.037470 sunsynk-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 20:28:24.000000 sunsynk-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.033470 sunsynk-0.3.3/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12614 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/pysunsynk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8050 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.033470 sunsynk-0.3.3/sunsynk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:28:33.000000 sunsynk-0.3.3/sunsynk.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.033470 sunsynk-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass-addon-sunsynk-dev.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass-addon-sunsynk.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.037470 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.037470 sunsynk-0.3.3/tests/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_pysunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_usunsynk.py
```

### Comparing `sunsynk-0.3.2/LICENSE` & `sunsynk-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/PKG-INFO` & `sunsynk-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.2/README.md` & `sunsynk-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/setup.cfg` & `sunsynk-0.3.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 description = Library to interface Deye/Sunsynk Hybrid Inverters
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://kellerza.github.io/sunsynk/
 author = Johann Kellerman
 author_email = kellerza@gmail.com
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.9
```

### Comparing `sunsynk-0.3.2/sunsynk/definitions.py` & `sunsynk-0.3.3/sunsynk/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 """Sunsynk 5kW&8kW hybrid inverter sensor definitions."""
 from sunsynk import AMPS, CELSIUS, KWH, VOLT, WATT
-from sunsynk.rwsensors import NumberRWSensor, SelectRWSensor, TimeRWSensor
+from sunsynk.rwsensors import (
+    NumberRWSensor,
+    SelectRWSensor,
+    SystemTimeRWSensor,
+    TimeRWSensor,
+)
 from sunsynk.sensors import (
     FaultSensor,
     InverterStateSensor,
     MathSensor,
     SDStatusSensor,
     Sensor,
     SensorDefinitions,
@@ -131,14 +136,15 @@
     FaultSensor((103, 104, 105, 106), "Fault"),
     InverterStateSensor(59, "Overall state"),
     SDStatusSensor(92, "SD Status", ""),  # type: ignore
     TempSensor(90, "DC transformer temperature", CELSIUS, 0.1),
     TempSensor(95, "Environment temperature", CELSIUS, 0.1),
     TempSensor(91, "Radiator temperature", CELSIUS, 0.1),
     Sensor(194, "Grid Connected Status"),
+    SystemTimeRWSensor((22, 23, 24), "Date Time", unit=""),
 )
 ###########
 # Settings
 ###########
 SENSORS += (
     Sensor(200, "Control Mode"),
     Sensor(232, "Grid Charge enabled", "", -1),
```

### Comparing `sunsynk-0.3.2/sunsynk/definitions3ph.py` & `sunsynk-0.3.3/sunsynk/definitions3ph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 """Sunsynk 5kW&8kW hybrid 3-phase inverter sensor definitions."""
 # pylint: disable=duplicate-code
 from sunsynk import AMPS, CELSIUS, KWH, VOLT, WATT
-from sunsynk.rwsensors import NumberRWSensor, SelectRWSensor, TimeRWSensor
+from sunsynk.rwsensors import (
+    NumberRWSensor,
+    SelectRWSensor,
+    SwitchRWSensor,
+    TimeRWSensor,
+)
 from sunsynk.sensors import (
     FaultSensor,
     InverterStateSensor,
     MathSensor,
     SDStatusSensor,
     Sensor,
     SensorDefinitions,
@@ -155,17 +160,17 @@
 
 
 ###########
 # Settings
 ###########
 SENSORS += (
     NumberRWSensor(128, "Grid Charge Battery current", AMPS, max=210),
-    SelectRWSensor(130, "Grid Charge enabled", switch=(0, 1)),
-    SelectRWSensor(146, "Use Timer", switch=(0, 255)),
-    SelectRWSensor(145, "Solar Export", switch=(0, 1)),
+    SwitchRWSensor(130, "Grid Charge enabled"),
+    SwitchRWSensor(146, "Use Timer", on=255),
+    SwitchRWSensor(145, "Solar Export"),
     NumberRWSensor(143, "Export Limit power", WATT, max=RATED_POWER),
     NumberRWSensor(108, "Battery Max Charge current", AMPS, max=210),
     NumberRWSensor(109, "Battery Max Discharge current", AMPS, max=210),
     NumberRWSensor(102, "Battery Capacity current", AMPS, max=2000),
 )
 
 # Additional optional sensors
```

### Comparing `sunsynk-0.3.2/sunsynk/helpers.py` & `sunsynk-0.3.3/sunsynk/helpers.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/sunsynk/pysunsynk.py` & `sunsynk-0.3.3/sunsynk/pysunsynk.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,79 @@
 """Sunsync Modbus interface."""
 import asyncio
 import logging
 from typing import Sequence
 from urllib.parse import urlparse
 
-import attr
+import attrs
 from pymodbus import version
 from pymodbus.client import (
     AsyncModbusSerialClient,
     AsyncModbusTcpClient,
     ModbusBaseClient,
 )
 
 from sunsynk.sunsynk import Sunsynk
 
 _LOGGER = logging.getLogger(__name__)
 
 
-@attr.define
+@attrs.define
 class pySunsynk(Sunsynk):  # pylint: disable=invalid-name
     """Sunsync Modbus class."""
 
-    port: str = attr.ib(default="/dev/tty0")
-    client: ModbusBaseClient = attr.ib(default=None)
+    client: ModbusBaseClient = None  # type:ignore
 
-    async def connect(self) -> None:
-        """Connect.
-
-        https://pymodbus.readthedocs.io/en/latest/source/example/async_asyncio_serial_client.html
-
-        """
-        if self.client and self.client.async_connected:
-            return
+    def _new_client(self) -> ModbusBaseClient:
+        """Create a new client."""
         url = urlparse(f"{self.port}")
+        if url.hostname:
+            host, port = url.hostname, url.port or 502
+            _LOGGER.info("PyModbus %s TCP: %s:%s", version.short(), host, port)
+            return AsyncModbusTcpClient(host=host, port=port)
+
+        _LOGGER.info("PyModbus %s Serial: %s", version.short(), self.port)
+        return AsyncModbusSerialClient(
+            port=self.port,
+            baudrate=self.baudrate,
+            # method="rtu",
+            stopbits=1,
+            bytesize=8,
+        )
 
-        if not url.netloc:
-            # Cannot run from a coroutine currently
-            # https://github.com/riptideio/pymodbus/pull/658/files#r718775308
-            _LOGGER.debug("Port: %s pymodbus %s", self.port, version.short())
-
-            self.client = AsyncModbusSerialClient(
-                port=self.port,
-                baudrate=self.baudrate,
-                # method="rtu",
-                stopbits=1,
-                bytesize=8,
-            )
-            # _loop, client = msc  # pylint: disable=unpacking-non-sequence
-
-            # Alternative interim...
-            # client = AsyncioModbusSerialClient(
-            #     port=self.port,
-            #     protocol_class=ModbusClientProtocol,
-            #     framer=AsyncModbusSerialClient._framer(method="rtu"),
-            #     loop=asyncio.get_running_loop(),
-            #     baudrate=self.baudrate,
-            #     stopbits=STOPBITS_ONE,
-            #     bytesize=8,
-            # )
-        else:
-            _LOGGER.debug(
-                "Host: %s : %s pymodbus %s", url.hostname, url.port, version.short()
-            )
-            self.client = AsyncModbusTcpClient(
-                host=url.hostname,
-                port=url.port or 502,
-                # protocol_class=ModbusClientProtocol,
-                # loop=asyncio.get_running_loop(),
-            )
+    async def connect(self) -> None:
+        """Connect. Will create a new client if required."""
+        if not self.client:
+            self.client = self._new_client()
 
-        await self.client.connect()
+        if not self.client.async_connected:
+            await self.client.connect()
 
         if not self.client.async_connected:
             raise ConnectionError
 
-        # try:
-        #     client.protocol._timeout = self.timeout
-        # except AttributeError as err:
-        #     _LOGGER.warning("%s", err)
-
-        # self.client = client. .protocol
-
     async def write_register(self, *, address: int, value: int) -> bool:
         """Write to a register - Sunsynk supports modbus function 0x10."""
+        await self.connect()
         try:
-            w_r = await self.client.write_registers(
-                address=address, values=(value,), slave=self.server_id
+            res = await self.client.write_registers(  # type:ignore
+                address=address, values=[value], slave=self.server_id
             )
-            if w_r.function_code < 0x80:  # test that we are not an error
+            if res.function_code < 0x80:  # test that we are not an error
                 return True
             _LOGGER.error("failed to write register %s=%s", address, value)
         except asyncio.TimeoutError:
             _LOGGER.error("timeout writing register %s=%s", address, value)
         self.timeouts += 1
         return False
 
     async def read_holding_registers(self, start: int, length: int) -> Sequence[int]:
         """Read a holding register."""
-        res = await self.client.read_holding_registers(
+        await self.connect()
+        res = await self.client.read_holding_registers(  # type:ignore
             address=start, count=length, slave=self.server_id
         )
         if res.function_code >= 0x80:  # test that we are not an error
-            raise Exception(  # pylint: disable=broad-exception-raised
+            raise IOError(
                 f"failed to read register {start} - function code: {res.function_code}"
             )
         return res.registers
```

### Comparing `sunsynk-0.3.2/sunsynk/rwsensors.py` & `sunsynk-0.3.3/sunsynk/rwsensors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Sensor classes represent modbus registers for an inverter."""
 from __future__ import annotations
 
 import logging
+import re
 from typing import Callable, Generator, Optional, Union
 
-import attr
+import attrs
 
 from sunsynk.helpers import NumType, RegType, SSTime, ValType, as_num
 from sunsynk.sensors import Sensor
 
 _LOGGER = logging.getLogger(__name__)
 ResolveType = Optional[Callable[[Sensor, ValType], ValType]]
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
 class RWSensor(Sensor):
     """Read & write sensor."""
 
     def reg(self, *regs: int, msg: str = "") -> RegType:
         """Check the registers are within the bitmask."""
         if self.bitmask and regs[0] != (regs[0] & self.bitmask):
             _LOGGER.error(
@@ -48,53 +49,52 @@
 
     @property
     def dependencies(self) -> list[Sensor]:
         """Dependencies."""
         return []
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
 class NumberRWSensor(RWSensor):
     """Numeric sensor which can be read and written."""
 
-    min: int | float | Sensor = attr.field(default=0)
-    max: int | float | Sensor = attr.field(default=100)
+    min: int | float | Sensor = attrs.field(default=0)
+    max: int | float | Sensor = attrs.field(default=100)
 
     @property
     def dependencies(self) -> list[Sensor]:
         """Get a list of sensors upon which this sensor depends."""
         return [s for s in (self.min, self.max) if isinstance(s, Sensor)]
 
     def value_to_reg(self, value: ValType, resolve: ResolveType) -> RegType:
         """Get the reg value from a display value, or the current reg value if out of range."""
-        if value is None or isinstance(value, str):
-            raise TypeError
+        fval = float(value)  # type:ignore
         minv = resolve_num(resolve, self.min, 0)
         maxv = resolve_num(resolve, self.max, 100)
-        val = int(max(minv, min(maxv, value / abs(self.factor))))
+        val = int(max(minv, min(maxv, fval / abs(self.factor))))
         if len(self.address) == 1:
             return self.reg(val)
         if len(self.address) == 2:
             return self.reg(val & 0xFFFF, int(val >> 16))
         raise NotImplementedError
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
 class SelectRWSensor(RWSensor):
     """Sensor with a set of options to select from."""
 
-    options: dict[int, str] = attr.field(factory=dict)
-    switch: Optional[tuple] = attr.field(default=None)
+    options: dict[int, str] = attrs.field(factory=dict)
+    # switch: Optional[tuple[int, int]] = attrs.field(default=None)
 
-    def __attrs_post_init__(self) -> None:
-        """Ensure correct parameters."""
-        if self.switch:
-            assert self.options == {}
-            assert len(self.switch) == 2
-            self.options = {self.switch[0]: "OFF", self.switch[1]: "ON"}
+    # def __attrs_post_init__(self) -> None:
+    #     """Ensure correct parameters."""
+    #     if self.switch:
+    #         assert not self.options
+    #         assert len(self.switch) == 2
+    #         self.options = {self.switch[0]: "OFF", self.switch[1]: "ON"}
 
     def available_values(self) -> list[str]:
         """Get the available values for this sensor."""
         return list(self.options.values())
 
     def value_to_reg(self, value: ValType, resolve: ResolveType) -> RegType:
         """Get the reg value from a display value, or the current reg value if out of range."""
@@ -111,20 +111,71 @@
         regsm = self.masked(regs)
         res = self.options.get(regsm[0])
         if res is None:
             _LOGGER.warning("%s: Unknown register value %s", self.id, regsm[0])
         return res
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
+class SwitchRWSensor(SelectRWSensor):
+    """Sensor with a set of options to select from."""
+
+    on: int = attrs.field(default=1)  # pylint: disable=invalid-name
+    off: int = attrs.field(default=0)
+
+    def __attrs_post_init__(self) -> None:
+        """Ensure correct parameters."""
+        assert not self.options
+        assert self.on != self.off
+        self.options = {self.off: "OFF", self.on: "ON"}
+
+
+@attrs.define(slots=True, eq=False)
+class SystemTimeRWSensor(RWSensor):
+    """Read & write time sensor."""
+
+    _path = "text"
+
+    def value_to_reg(self, value: ValType, resolve: ResolveType) -> RegType:
+        """Get the reg value from a display value."""
+        # pylint: disable=invalid-name
+        redt = re.compile(r"(2\d{3})-(\d{2})-(\d{2}) (\d{2}):(\d{2}):(\d{2})")
+        match = redt.fullmatch(str(value).strip())
+        if not match:
+            raise ValueError("Invalid datetime {value}")
+        y, m, d = int(match.group(1)) - 2000, int(match.group(2)), int(match.group(3))
+        h, mn, s = int(match.group(4)), int(match.group(5)), int(match.group(6))
+        regs = (
+            (y << 8) + m,
+            (d << 8) + h,
+            (mn << 8) + s,
+        )
+        msg = f"{y}-{m:02}-{d:02} {h}:{mn:02}:{s:02} ==> {regs}"
+        assert len(regs) == len(self.address)
+        _LOGGER.debug(msg)
+        return regs
+
+    def reg_to_value(self, regs: RegType) -> ValType:
+        """Decode the register."""
+        # pylint: disable=invalid-name
+        y = ((regs[0] & 0xFF00) >> 8) + 2000
+        m = regs[0] & 0xFF
+        d = (regs[1] & 0xFF00) >> 8
+        h = regs[1] & 0xFF
+        mn = (regs[2] & 0xFF00) >> 8
+        s = regs[2] & 0xFF
+        return f"{y}-{m:02}-{d:02} {h}:{mn:02}:{s:02}"
+
+
+@attrs.define(slots=True, eq=False)
 class TimeRWSensor(RWSensor):
     """Extract the time."""
 
-    min: TimeRWSensor = attr.field(default=None)
-    max: TimeRWSensor = attr.field(default=None)
+    min: TimeRWSensor = attrs.field(default=None)
+    max: TimeRWSensor = attrs.field(default=None)
 
     def available_values(
         self, step_minutes: int, resolve: Callable[[Sensor, ValType], ValType]
     ) -> list[str]:
         """Get the available values for this sensor."""
         full_day = 24 * 60
```

### Comparing `sunsynk-0.3.2/sunsynk/sensors.py` & `sunsynk-0.3.3/sunsynk/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 """Sensor classes represent modbus registers for an inverter."""
 from __future__ import annotations
 
 import logging
 from typing import Union
 
-import attr
+import attrs
 
 from sunsynk.helpers import (
     NumType,
     RegType,
     ValType,
     ensure_tuple,
     int_round,
     signed,
     slug,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
-@attr.define(slots=True)
+@attrs.define(slots=True)
 class Sensor:
     """Sunsynk sensor."""
 
     # pylint: disable=too-many-instance-attributes
-    address: RegType = attr.field(converter=ensure_tuple)
-    name: str = attr.field()
-    unit: str = attr.field(default="")
-    factor: float = attr.field(default=1)
-    bitmask: int = attr.field(default=0)
+    address: RegType = attrs.field(converter=ensure_tuple)
+    name: str = attrs.field()
+    unit: str = attrs.field(default="")
+    factor: float = attrs.field(default=1)
+    bitmask: int = attrs.field(default=0)
 
     @property
     def id(self) -> str:  # pylint: disable=invalid-name
         """Get the sensor ID."""
         return slug(self.name)
 
     def reg_to_value(self, regs: RegType) -> ValType:
@@ -60,20 +60,20 @@
     def __eq__(self, other: object) -> bool:
         """Sensor equality is based on the ID only."""
         if not isinstance(other, Sensor):
             raise TypeError
         return self.id == other.id
 
 
-@attr.define(slots=True)
+@attrs.define(slots=True)
 class SensorDefinitions:
     """Definitions."""
 
-    all: dict[str, Sensor] = attr.field(factory=dict)
-    deprecated: dict[str, Sensor] = attr.field(factory=dict)
+    all: dict[str, Sensor] = attrs.field(factory=dict)
+    deprecated: dict[str, Sensor] = attrs.field(factory=dict)
 
     @property
     def serial(self) -> Sensor:
         """Get the serial sensor."""
         return self.all["serial"]
 
     @property
@@ -90,21 +90,21 @@
             return self
         if isinstance(item, (tuple, list)):
             for itm in item:
                 self.all[itm.id] = itm
         return self
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
 class MathSensor(Sensor):
     """Math sensor, add multiple registers."""
 
-    factors: tuple[float, ...] = attr.field(default=None, converter=ensure_tuple)
-    no_negative: bool = attr.field(default=False)
-    absolute: bool = attr.field(default=False)
+    factors: tuple[float, ...] = attrs.field(default=None, converter=ensure_tuple)
+    no_negative: bool = attrs.field(default=False)
+    absolute: bool = attrs.field(default=False)
 
     def reg_to_value(self, regs: RegType) -> ValType:
         """Calculate the math value."""
         val = int_round(sum(signed(i) * s for i, s in zip(regs, self.factors)))
         if self.absolute and val < 0:
             val = -val
         if self.no_negative and val < 0:
@@ -112,65 +112,65 @@
         return val
 
     def __attrs_post_init__(self) -> None:
         """Ensure correct parameters."""
         assert len(self.address) == len(self.factors)
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
 class TempSensor(Sensor):
     """Offset by 100 for temperature."""
 
     def reg_to_value(self, regs: RegType) -> ValType:
         """Decode the temperature (offset by 100)."""
         try:
             val = regs[0]
             return int_round((float(val) * abs(self.factor)) - 100)  # type: ignore
         except (TypeError, ValueError) as err:
             _LOGGER.error("Could not decode temperature: %s", err)
         return None
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
 class SDStatusSensor(Sensor):
     """SD card status."""
 
     def reg_to_value(self, regs: RegType) -> ValType:
         """Decode the SD card status."""
         return {
             1000: "fault",
             2000: "ok",
         }.get(regs[0]) or f"unknown {regs[0]}"
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
 class InverterStateSensor(Sensor):
     """Inverter status."""
 
     def reg_to_value(self, regs: RegType) -> ValType:
         """Decode the inverter status."""
         if regs[0] == 2:
             return "ok"
         return f"unknown {regs[0]}"
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
 class SerialSensor(Sensor):
     """Decode the inverter serial number."""
 
     def reg_to_value(self, regs: RegType) -> ValType:
         """Decode the inverter serial number."""
         val = ""
         for b16 in regs:
             val += chr(b16 >> 8)
             val += chr(b16 & 0xFF)
         return val
 
 
-@attr.define(slots=True, eq=False)
+@attrs.define(slots=True, eq=False)
 class FaultSensor(Sensor):
     """Decode Inverter faults."""
 
     def reg_to_value(self, regs: RegType) -> ValType:
         """Decode Inverter faults."""
         faults = {
             13: "Working mode change",
```

### Comparing `sunsynk-0.3.2/sunsynk/state.py` & `sunsynk-0.3.3/sunsynk/state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/sunsynk/sunsynk.py` & `sunsynk-0.3.3/sunsynk/sunsynk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """Sunsync Modbus interface."""
 import asyncio
 import logging
 from typing import Iterable, Sequence
 
-import attr
+import attrs
 
 from sunsynk.helpers import patch_bitmask
 from sunsynk.rwsensors import RWSensor
 from sunsynk.sensors import Sensor, ValType
 from sunsynk.state import InverterState, group_sensors, register_map
 
 _LOGGER = logging.getLogger(__name__)
 
 
-@attr.define
+@attrs.define
 class Sunsynk:
     """Sunsync Modbus class."""
 
-    state: InverterState = attr.field(factory=InverterState)
-    port: str = attr.ib(default="/dev/tty0")
-    baudrate: int = attr.ib(default=9600)
-    server_id: int = attr.ib(default=1)
-    timeout: int = attr.ib(default=10)
-    read_sensors_batch_size: int = attr.field(default=60)
+    state: InverterState = attrs.field(factory=InverterState)
+    port: str = attrs.field(default="/dev/tty0")
+    baudrate: int = attrs.field(default=9600)
+    server_id: int = attrs.field(default=1)
+    timeout: int = attrs.field(default=10)
+    read_sensors_batch_size: int = attrs.field(default=60)
     timeouts: int = 0
 
     async def connect(self) -> None:
         """Connect."""
         raise NotImplementedError
 
     async def write_register(self, *, address: int, value: int) -> bool:
```

### Comparing `sunsynk-0.3.2/sunsynk/usunsynk.py` & `sunsynk-0.3.3/sunsynk/usunsynk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """Sunsynk lib using umodbus."""
 import asyncio
 import logging
 from typing import Sequence
 from urllib import parse
 
-import attr
+import attrs
 from async_modbus import AsyncClient, modbus_for_url
 from connio import SERIAL_SCHEMES, SOCKET_SCHEMES
 
 from sunsynk.sunsynk import Sunsynk
 
 _LOGGER = logging.getLogger(__name__)
 
 
-@attr.define
+@attrs.define
 class uSunsynk(Sunsynk):  # pylint: disable=invalid-name
     """Sunsynk class using umodbus."""
 
-    client: AsyncClient = attr.field(default=None)
+    client: AsyncClient = None
 
     async def connect(self) -> None:
         """Connect."""
         url_result = parse.urlparse(self.port)
         scheme = url_result.scheme
         if scheme not in SOCKET_SCHEMES and scheme not in SERIAL_SCHEMES:
             sks = [f"{s}://" for s in SOCKET_SCHEMES]
```

### Comparing `sunsynk-0.3.2/sunsynk.egg-info/PKG-INFO` & `sunsynk-0.3.3/sunsynk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sunsynk-0.3.2/tests/conftest.py` & `sunsynk-0.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/tests/hass-addon-sunsynk-dev.zip` & `sunsynk-0.3.3/tests/hass-addon-sunsynk-dev.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/test_filter.py` & `sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,19 @@
-"""Optionally test filters."""
+"""Optionally test filter."""
 import logging
 from itertools import repeat
-from pathlib import Path
-from typing import Any, Callable, List
-
-import pytest
+from typing import Any, List
 
 from sunsynk.definitions import SENSORS
 from sunsynk.rwsensors import RWSensor
-from tests.conftest import import_module
+from tests.hass_addon_sunsynk_multi import filter
 
 _LOGGER = logging.getLogger(__name__)
 
 
-@pytest.fixture
-def mod_folder() -> str:
-    """Return the folder from __init__."""
-    init = import_module("__init__", Path(__file__).parent)
-    return init.MOD_FOLDER
-
-
-@pytest.fixture
-def filters(mod_folder) -> Callable:
-    """Import & return the getfilter function."""
-    return import_module("filter", mod_folder)
-
-
 def assert_sequence(fut, updates: List[Any], counts=None):
     upd_cnt, i_cnt = 0, 0
     try:
         for upd in updates:
             i_cnt += 1
             if upd is None:
                 assert not fut.should_update()
@@ -60,37 +44,37 @@
     yield val0
     for val in vals:
         # an interval is represented as None
         yield from repeat(None, count)
         yield val
 
 
-def test_last(filters):
+def test_last():
     """Last filter."""
-    fut = filters.getfilter("last", None)
+    fut = filter.getfilter("last", None)
 
     assert_sequence(fut, add_intervals(59, *[(55, 55), (44, 44), (43, 43)]))
 
 
-def test_min(filters):
+def test_min():
     """Min filter."""
-    fut = filters.getfilter("min", None)
+    fut = filter.getfilter("min", None)
 
     sq0 = (50, 50)
     sq1 = [44, 100, 100, 100, 100, (100, 44)]
     sq2 = [100, 100, 100, 55, 100, (100, 55)]
 
     assert_sequence(fut, add_intervals(9, sq0, sq1, sq2))
 
     assert fut.should_update() is False
 
 
-def test_mean(filters):
+def test_mean():
     """Mean filter."""
-    fut = filters.getfilter("mean", None)
+    fut = filter.getfilter("mean", None)
 
     assert_sequence(
         fut,
         add_intervals(9, *[(50, 50), 50, 50, 50, 100, 100, (100, 75)]),
         counts=(61, 7),
     )
 
@@ -103,56 +87,56 @@
     assert_sequence(
         fut,
         add_intervals(9, *[50, 100, 50, 50, 100, (100, 75)]),
         counts=(51, 6),
     )
 
 
-def test_step(filters):
+def test_step():
     """Step filter."""
-    fut = filters.getfilter("", None)
+    fut = filter.getfilter("", None)
     assert_sequence(
         fut,
         [(20, 20), 20, 20, 20, (120, 120), 140, 140],
     )
 
-    fut = filters.getfilter("step:100", None)
+    fut = filter.getfilter("step:100", None)
     assert_sequence(
         fut,
         [(90, 90)] + [90] * 58 + [(90, 90)],
     )
 
-    fut = filters.getfilter("step:100", None)
+    fut = filter.getfilter("step:100", None)
     sq0 = [(10, 10)]
     sq0 += [21] * 58 + [(50, 21.3)]
     sq0 += [(150, 150), (20, 20)]
     sq0 += [21] * 58 + [(50, 21.5)]
     sq0 += [20] * 58 + [(50, 20.5)]
     sq0 += [20] * 58 + [(50, 20.5)]
     sq0 += [(1000, 1000)] + [950] * 58 + [(950, 950.8)]
 
     assert_sequence(fut, sq0)
 
 
-def test_step_text(filters):
+def test_step_text():
     """Step filter."""
-    fut = filters.getfilter("step", None)
+    fut = filter.getfilter("step", None)
     assert_sequence(
         fut,
         [("a", "a"), ("b", "b")],
     )
 
 
-def test_rr(filters):
+def test_rr():
     """Test round robin."""
-    RROBIN = filters.RROBIN
+    RROBIN = filter.RROBIN
     RROBIN.tick()
 
-    sen = [filters.Sensor(1, "a"), filters.Sensor(2, "b"), filters.Sensor(3, "c")]
-    fil = [filters.getfilter("round_robin", s) for s in sen]
+    sen = [filter.Sensor(1, "a"), filter.Sensor(2, "b"), filter.Sensor(3, "c")]
+    fil = [filter.getfilter("round_robin", s) for s in sen]
 
     for idx in range(2):
         assert fil[idx].sensor_name is sen[idx].name
     assert RROBIN.list == list(fil)
 
     assert [RROBIN.idx, RROBIN.active] == [-1, []]
     RROBIN.tick()
@@ -164,16 +148,16 @@
     assert [f.should_update() for f in fil] == [False, True, False]
     RROBIN.tick()
     assert [f.should_update() for f in fil] == [False, False, True]
     RROBIN.tick()
     assert [f.should_update() for f in fil] == [True, False, False]
 
 
-def test_suggest(filters):
-    assert filters.suggested_filter(SENSORS.all["environment_temperature"]) == "avg"
-    assert filters.suggested_filter(SENSORS.all["day_battery_charge"]) == "last"
-    # assert filters.suggested_filter(SENSORS.all["grid_ct_load"]) == "step"
-    assert filters.suggested_filter(SENSORS.all["sd_status"]) == "last"
+def test_suggest():
+    assert filter.suggested_filter(SENSORS.all["environment_temperature"]) == "avg"
+    assert filter.suggested_filter(SENSORS.all["day_battery_charge"]) == "last"
+    # assert filter.suggested_filter(SENSORS.all["grid_ct_load"]) == "step"
+    assert filter.suggested_filter(SENSORS.all["sd_status"]) == "last"
 
     rw_sensors = [s for s in SENSORS.all.values() if isinstance(s, RWSensor)]
     for s in rw_sensors:
-        assert filters.suggested_filter(s) == "round_robin"
+        assert filter.suggested_filter(s) == "round_robin"
```

### Comparing `sunsynk-0.3.2/tests/hass-addon-sunsynk-multi/test_run.py` & `sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_run.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,71 +3,56 @@
 import re
 from pathlib import Path
 from types import ModuleType
 
 import pytest
 
 from tests.conftest import import_module
+from tests.hass_addon_sunsynk_multi import MOD_FOLDER
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @pytest.fixture
-def mod_folder() -> str:
-    """Return the folder from __init__."""
-    init = import_module("__init__", Path(__file__).parent)
-    return init.MOD_FOLDER
-
-
-@pytest.fixture
-def run(mod_folder) -> ModuleType:
+def run() -> ModuleType:
     """Import the module."""
-    return import_module("run", mod_folder)
+    return import_module("run", MOD_FOLDER)
 
 
 def test_run(run):
     """Test Run."""
     assert not run.STATES
     assert not run.OPT.mqtt_host
 
-    # testargs = ["run.py", "host1", "passw"]
-    # with patch.object(run.sys, "argv", testargs):
-    #     run.startup()
-    # assert run.STATES
-    # assert run.OPT.mqtt_host == "host1"
-    # assert run.OPT.mqtt_password == "passw"
-
-    # run.STATES.clear()
-    # run.OPT.mqtt_host = ""
-
 
-def test_versions(run, mod_folder):
+def test_versions(run):
     """Test versions.
 
     config.json - contains the HASS addon version
     Dockerfile  - installs the specific sunsynk library from pypi
     setup.py    - sunsynk library on pypi
     """
 
     def _get_version(filename, regex):
         txt = Path(filename).read_text()
         res = re.compile(regex).search(txt)
         assert res, f"version not found in {filename}"
+        _LOGGER.warning("\t%s\t%s", res.group(1), filename)
         return res.group(1)
 
     v_setup = _get_version(
         filename="sunsynk/__init__.py",
         regex=r'VERSION = "(.+)"',
     )
 
     v_docker = _get_version(
-        filename=f"{mod_folder}/Dockerfile",
+        filename=f"{MOD_FOLDER}/Dockerfile",
         regex=r"sunsynk(?:\[[^\]]+\])?==([0-9.]+)",
     )
 
     v_config = _get_version(
-        filename=f"{mod_folder}/config.yaml",
+        filename=f"{MOD_FOLDER}/config.yaml",
         regex=r"version: .+-(.+)",
     )
 
     assert v_setup == v_docker
     assert v_setup == v_config
```

### Comparing `sunsynk-0.3.2/tests/hass-addon-sunsynk.zip` & `sunsynk-0.3.3/tests/hass-addon-sunsynk.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/tests/sunsynk/test_helpers.py` & `sunsynk-0.3.3/tests/sunsynk/test_helpers.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/tests/sunsynk/test_register.py` & `sunsynk-0.3.3/tests/sunsynk/test_register.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/tests/sunsynk/test_rwsensors.py` & `sunsynk-0.3.3/tests/sunsynk/test_rwsensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 
 from sunsynk.rwsensors import (
     NumberRWSensor,
     RWSensor,
     SelectRWSensor,
     Sensor,
+    SwitchRWSensor,
     TimeRWSensor,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def test_bitmask(caplog, state) -> None:
@@ -35,15 +36,15 @@
     reg = s.reg(*reg, msg=f"value was {val}")
 
     assert reg == (1,)
     assert "outside" in caplog.text
 
 
 def test_bitmask2(caplog, state) -> None:
-    s = SelectRWSensor(1, "", switch=(0, 4), bitmask=0x4)
+    s = SwitchRWSensor(1, "", on=4, bitmask=0x4)
     state.track(s)
 
     assert state[s] is None
     state.update({1: 0x1})
 
     assert state[s] == "OFF"
     assert "outside" not in caplog.text
```

### Comparing `sunsynk-0.3.2/tests/sunsynk/test_sensors.py` & `sunsynk-0.3.3/tests/sunsynk/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.2/tests/sunsynk/test_sunsynk.py` & `sunsynk-0.3.3/tests/sunsynk/test_sunsynk.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,22 @@
 """Test sunsynk library."""
 import logging
-import os
-from unittest.mock import AsyncMock, MagicMock, call, patch
+from unittest.mock import MagicMock, call, patch
 
 import pytest
 
 # from sunsynk.definitions import serial
 from sunsynk import Sunsynk
-from sunsynk.pysunsynk import pySunsynk
 from sunsynk.rwsensors import NumberRWSensor
 from sunsynk.state import InverterState
-from sunsynk.usunsynk import uSunsynk
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @pytest.mark.asyncio
-async def test_pyss():
-    ss = pySunsynk()
-    with pytest.raises(ConnectionError):
-        await ss.connect()
-
-
-@pytest.mark.asyncio
-async def test_uss_schemes():
-    """Test url schemes for usunsynk.
-
-    umodbus only connects on read.
-    """
-    for port in ("serial:///dev/usb1", "tcp://127.0.0.1:502"):
-        ss = uSunsynk(port=port)
-        try:
-            await ss.connect()
-        except ModuleNotFoundError as err:  # not working on windows
-            _LOGGER.error("usunsynk could not connect to %s: %s", port, err)
-            if os.name == "posix":
-                raise
-
-    for port in ("127.0.0.1:502", "xxx", "localhost"):
-        ss = uSunsynk(port=port)
-        with pytest.raises(ValueError):
-            await ss.connect()
-
-
-@pytest.mark.asyncio
-async def test_uss_sensor():
-    ss = uSunsynk(port="tcp://127.0.0.1:502")
-    await ss.connect()
-
-    rhr = ss.client.read_holding_registers = AsyncMock()
-
-    _LOGGER.warning("%s", dir(ss.client))
-    assert not rhr.called
-    await ss.read_holding_registers(1, 2)
-    assert rhr.called
-
-    wrr = ss.client.write_registers = AsyncMock()
-    assert not wrr.called
-    await ss.write_register(address=1, value=2)
-    assert wrr.called
-
-
-@pytest.mark.asyncio
 async def test_ss_NotImplemented():
     ss = Sunsynk()
     with pytest.raises(NotImplementedError):
         await ss.connect()
     with pytest.raises(NotImplementedError):
         await ss.write_register(address=1, value=1)
     with pytest.raises(NotImplementedError):
```

