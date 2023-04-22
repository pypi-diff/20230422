# Comparing `tmp/bus_burgos-0.0.0.tar.gz` & `tmp/bus_burgos-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_burgos-0.0.0.tar", max compression
+gzip compressed data, was "bus_burgos-0.1.0.tar", max compression
```

## Comparing `bus_burgos-0.0.0.tar` & `bus_burgos-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      238 2023-04-22 11:04:43.035687 bus_burgos-0.0.0/README.md
--rw-r--r--   0        0        0     3231 2023-04-22 12:24:11.737970 bus_burgos-0.0.0/bus_burgos/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-22 11:01:56.346317 bus_burgos-0.0.0/pyproject.toml
--rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 bus_burgos-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      238 2023-04-22 14:33:16.796371 bus_burgos-0.1.0/README.md
+-rw-r--r--   0        0        0     3232 2023-04-22 14:33:16.796371 bus_burgos-0.1.0/bus_burgos/__init__.py
+-rw-r--r--   0        0        0     1088 2023-04-22 14:33:48.780585 bus_burgos-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 bus_burgos-0.1.0/PKG-INFO
```

### Comparing `bus_burgos-0.0.0/bus_burgos/__init__.py` & `bus_burgos-0.1.0/bus_burgos/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     times: List[BusTime]
 
     def get_times_by_line(self, line: str):
         return next(x for x in self.times if x.line == line).estimations
 
     def get_next_bus(self, line: str):
         estimations = self.get_times_by_line(line)
-        return sorted(estimations, key=lambda x: x.seconds, reverse=True)[0]
+        return sorted(estimations, key=lambda x: x.seconds, reverse=False)[0]
 
     @staticmethod
     def from_json(item):
         return BusStopWithEstimations(
             times=list(map(BusTime.from_json, item["routeEstimationByNode"])),
         )
```

### Comparing `bus_burgos-0.0.0/pyproject.toml` & `bus_burgos-0.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bus_burgos"
-version = "0.0.0"
+version = "0.1.0"
 description = "Asynchronous Python client for getting bus stops information in Burgos"
 authors = ["ricveal <ricveal@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ricveal/bus_burgos"
 repository = "https://github.com/ricveal/bus_burgos"
 keywords = ["bus", "burgos", "transit", "api", "async", "client"]
```

### Comparing `bus_burgos-0.0.0/PKG-INFO` & `bus_burgos-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus-burgos
-Version: 0.0.0
+Version: 0.1.0
 Summary: Asynchronous Python client for getting bus stops information in Burgos
 Home-page: https://github.com/ricveal/bus_burgos
 License: MIT
 Keywords: bus,burgos,transit,api,async,client
 Author: ricveal
 Author-email: ricveal@gmail.com
 Requires-Python: >=3.7,<4.0
```

