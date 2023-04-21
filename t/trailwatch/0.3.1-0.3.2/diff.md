# Comparing `tmp/trailwatch-0.3.1.tar.gz` & `tmp/trailwatch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailwatch-0.3.1.tar", max compression
+gzip compressed data, was "trailwatch-0.3.2.tar", max compression
```

## Comparing `trailwatch-0.3.1.tar` & `trailwatch-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-04-20 15:40:39.231816 trailwatch-0.3.1/LICENSE
--rw-r--r--   0        0        0     7527 2023-04-20 15:40:39.231816 trailwatch-0.3.1/README.md
--rw-r--r--   0        0        0     2026 2023-04-20 15:40:39.235816 trailwatch-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3634 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/__init__.py
--rw-r--r--   0        0        0     6071 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/config.py
--rw-r--r--   0        0        0        0 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/__init__.py
--rw-r--r--   0        0        0       85 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/aws/__init__.py
--rw-r--r--   0        0        0     8308 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/aws/api.py
--rw-r--r--   0        0        0     3912 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/aws/connector.py
--rw-r--r--   0        0        0      809 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/aws/handler.py
--rw-r--r--   0        0        0     1081 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/base.py
--rw-r--r--   0        0        0      306 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/salesforce/__init__.py
--rw-r--r--   0        0        0     6116 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/connectors/salesforce/connector.py
--rw-r--r--   0        0        0     7103 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/context.py
--rw-r--r--   0        0        0      414 2023-04-20 15:40:39.235816 trailwatch-0.3.1/src/trailwatch/exceptions.py
--rw-r--r--   0        0        0     8253 1970-01-01 00:00:00.000000 trailwatch-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-20 22:42:40.840035 trailwatch-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7527 2023-04-20 22:42:40.840035 trailwatch-0.3.2/README.md
+-rw-r--r--   0        0        0     2026 2023-04-20 22:42:40.844035 trailwatch-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3634 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/__init__.py
+-rw-r--r--   0        0        0     6071 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/config.py
+-rw-r--r--   0        0        0        0 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/connectors/__init__.py
+-rw-r--r--   0        0        0       85 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/connectors/aws/__init__.py
+-rw-r--r--   0        0        0     8308 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/connectors/aws/api.py
+-rw-r--r--   0        0        0     3912 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/connectors/aws/connector.py
+-rw-r--r--   0        0        0      809 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/connectors/aws/handler.py
+-rw-r--r--   0        0        0     1081 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/connectors/base.py
+-rw-r--r--   0        0        0      306 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/connectors/salesforce/__init__.py
+-rw-r--r--   0        0        0     6461 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/connectors/salesforce/connector.py
+-rw-r--r--   0        0        0     7103 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/context.py
+-rw-r--r--   0        0        0      414 2023-04-20 22:42:40.844035 trailwatch-0.3.2/src/trailwatch/exceptions.py
+-rw-r--r--   0        0        0     8253 1970-01-01 00:00:00.000000 trailwatch-0.3.2/PKG-INFO
```

### Comparing `trailwatch-0.3.1/LICENSE` & `trailwatch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.1/README.md` & `trailwatch-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.1/pyproject.toml` & `trailwatch-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trailwatch"
-version = "0.3.1"
+version = "0.3.2"
 description = "Python SDK for TrailWatch by Kicksaw"
 license = "Apache-2.0"
 authors = ["George Bocharov <george@kicksaw.com>"]
 readme = "README.md"
 homepage = "https://www.kicksaw.com/"
 repository = "https://github.com/Kicksaw-Consulting/trailwatch-python-sdk"
 packages = [
```

### Comparing `trailwatch-0.3.1/src/trailwatch/__init__.py` & `trailwatch-0.3.2/src/trailwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.1/src/trailwatch/config.py` & `trailwatch-0.3.2/src/trailwatch/config.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.1/src/trailwatch/connectors/aws/api.py` & `trailwatch-0.3.2/src/trailwatch/connectors/aws/api.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.1/src/trailwatch/connectors/aws/connector.py` & `trailwatch-0.3.2/src/trailwatch/connectors/aws/connector.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.1/src/trailwatch/connectors/aws/handler.py` & `trailwatch-0.3.2/src/trailwatch/connectors/aws/handler.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.1/src/trailwatch/connectors/base.py` & `trailwatch-0.3.2/src/trailwatch/connectors/base.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.1/src/trailwatch/connectors/salesforce/connector.py` & `trailwatch-0.3.2/src/trailwatch/connectors/salesforce/connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,18 @@
             return
 
         try:
             # Create integration
             response = self.salesforce.query_all(
                 format_soql(
                     (
-                        f"SELECT Id FROM {NAMESPACE}{INTEGRATION} "  # nosec
+                        f"SELECT Id "
+                        f"FROM {NAMESPACE}{INTEGRATION} "  # nosec
                         f"WHERE Name = {{name}}"
+                        f"ORDER BY LastModifiedDate ASC"
                     ),
                     name=self.config.job,
                 )
             )
             if len(response["records"]) == 0:
                 response = getattr(
                     self.salesforce,
@@ -68,16 +70,21 @@
                     {
                         "Name": self.config.job,
                         f"{NAMESPACE}LambdaName__c": None,
                     }
                 )
                 self.integration_object_id = response["id"]
             else:
-                assert len(response["records"]) == 1
                 self.integration_object_id = response["records"][0]["Id"]
+                if len(response["records"]) > 1:
+                    warnings.warn(
+                        f"Found multiple Salesforce integration objects "
+                        f"for '{self.config.job}', using the oldest one: "
+                        f"'{self.integration_object_id}'"
+                    )
 
             # Create execution
             response = getattr(
                 self.salesforce,
                 f"{NAMESPACE}{EXECUTION}",
             ).create(
                 {
```

### Comparing `trailwatch-0.3.1/src/trailwatch/context.py` & `trailwatch-0.3.2/src/trailwatch/context.py`

 * *Files identical despite different names*

### Comparing `trailwatch-0.3.1/PKG-INFO` & `trailwatch-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trailwatch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python SDK for TrailWatch by Kicksaw
 Home-page: https://www.kicksaw.com/
 License: Apache-2.0
 Author: George Bocharov
 Author-email: george@kicksaw.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

