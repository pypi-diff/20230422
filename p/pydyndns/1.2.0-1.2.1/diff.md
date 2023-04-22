# Comparing `tmp/pydyndns-1.2.0.tar.gz` & `tmp/pydyndns-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydyndns-1.2.0.tar", last modified: Wed Nov 10 05:56:26 2021, max compression
+gzip compressed data, was "pydyndns-1.2.1.tar", last modified: Sat Apr 22 07:23:45 2023, max compression
```

## Comparing `pydyndns-1.2.0.tar` & `pydyndns-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2021-11-10 05:56:26.224682 pydyndns-1.2.0/
--rw-r--r--   0 chead     (1000) chead     (1000)       44 2020-08-25 15:53:56.000000 pydyndns-1.2.0/.gitignore
--rw-r--r--   0 chead     (1000) chead     (1000)     1073 2016-11-12 01:01:11.000000 pydyndns-1.2.0/LICENSE.txt
--rw-r--r--   0 chead     (1000) chead     (1000)       15 2020-08-25 15:53:56.000000 pydyndns-1.2.0/MANIFEST.in
--rw-r--r--   0 chead     (1000) chead     (1000)     6140 2021-11-10 05:56:26.224682 pydyndns-1.2.0/PKG-INFO
--rw-r--r--   0 chead     (1000) chead     (1000)     5491 2020-08-25 15:53:56.000000 pydyndns-1.2.0/README.md
--rwxr-xr-x   0 chead     (1000) chead     (1000)      387 2020-08-25 15:53:56.000000 pydyndns-1.2.0/build-sdist
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2021-11-10 05:56:26.221683 pydyndns-1.2.0/examples/
--rw-r--r--   0 chead     (1000) chead     (1000)      188 2020-08-25 15:53:56.000000 pydyndns-1.2.0/examples/dhcpcd-hook
--rw-r--r--   0 chead     (1000) chead     (1000)      409 2020-08-25 15:53:56.000000 pydyndns-1.2.0/examples/pydyndns.conf.sample
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2021-11-10 05:56:26.222683 pydyndns-1.2.0/examples/tasksched/
--rw-r--r--   0 chead     (1000) chead     (1000)     3050 2020-08-25 15:53:56.000000 pydyndns-1.2.0/examples/tasksched/Force.xml
--rw-r--r--   0 chead     (1000) chead     (1000)     3368 2020-08-25 15:53:56.000000 pydyndns-1.2.0/examples/tasksched/Normal.xml
--rw-r--r--   0 chead     (1000) chead     (1000)       95 2020-08-25 15:53:56.000000 pydyndns-1.2.0/pyproject.toml
--rw-r--r--   0 chead     (1000) chead     (1000)     1203 2021-11-10 05:56:26.226683 pydyndns-1.2.0/setup.cfg
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2021-11-10 05:56:26.219683 pydyndns-1.2.0/src/
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2021-11-10 05:56:26.222683 pydyndns-1.2.0/src/pydyndns/
--rw-r--r--   0 chead     (1000) chead     (1000)    17468 2021-11-10 05:39:22.000000 pydyndns-1.2.0/src/pydyndns/__init__.py
-drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2021-11-10 05:56:26.224682 pydyndns-1.2.0/src/pydyndns.egg-info/
--rw-r--r--   0 chead     (1000) chead     (1000)     6140 2021-11-10 05:56:26.000000 pydyndns-1.2.0/src/pydyndns.egg-info/PKG-INFO
--rw-r--r--   0 chead     (1000) chead     (1000)      465 2021-11-10 05:56:26.000000 pydyndns-1.2.0/src/pydyndns.egg-info/SOURCES.txt
--rw-r--r--   0 chead     (1000) chead     (1000)        1 2021-11-10 05:56:26.000000 pydyndns-1.2.0/src/pydyndns.egg-info/dependency_links.txt
--rw-r--r--   0 chead     (1000) chead     (1000)       44 2021-11-10 05:56:26.000000 pydyndns-1.2.0/src/pydyndns.egg-info/entry_points.txt
--rw-r--r--   0 chead     (1000) chead     (1000)       19 2021-11-10 05:56:26.000000 pydyndns-1.2.0/src/pydyndns.egg-info/requires.txt
--rw-r--r--   0 chead     (1000) chead     (1000)        9 2021-11-10 05:56:26.000000 pydyndns-1.2.0/src/pydyndns.egg-info/top_level.txt
--rw-r--r--   0 chead     (1000) chead     (1000)        1 2021-10-29 05:18:04.000000 pydyndns-1.2.0/src/pydyndns.egg-info/zip-safe
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-04-22 07:23:45.592956 pydyndns-1.2.1/
+-rw-r--r--   0 chead     (1000) chead     (1000)     1073 2016-11-12 01:01:11.000000 pydyndns-1.2.1/LICENSE.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)       15 2020-08-25 15:53:56.000000 pydyndns-1.2.1/MANIFEST.in
+-rw-r--r--   0 chead     (1000) chead     (1000)     6100 2023-04-22 07:23:45.592956 pydyndns-1.2.1/PKG-INFO
+-rw-r--r--   0 chead     (1000) chead     (1000)     5488 2021-11-10 06:14:51.000000 pydyndns-1.2.1/README.md
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-04-22 07:23:45.558956 pydyndns-1.2.1/examples/
+-rw-r--r--   0 chead     (1000) chead     (1000)      188 2020-08-25 15:53:56.000000 pydyndns-1.2.1/examples/dhcpcd-hook
+-rw-r--r--   0 chead     (1000) chead     (1000)      409 2020-08-25 15:53:56.000000 pydyndns-1.2.1/examples/pydyndns.conf.sample
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-04-22 07:23:45.584956 pydyndns-1.2.1/examples/tasksched/
+-rw-r--r--   0 chead     (1000) chead     (1000)     3050 2020-08-25 15:53:56.000000 pydyndns-1.2.1/examples/tasksched/Force.xml
+-rw-r--r--   0 chead     (1000) chead     (1000)     3368 2020-08-25 15:53:56.000000 pydyndns-1.2.1/examples/tasksched/Normal.xml
+-rw-r--r--   0 chead     (1000) chead     (1000)       95 2020-08-25 15:53:56.000000 pydyndns-1.2.1/pyproject.toml
+-rw-r--r--   0 chead     (1000) chead     (1000)     1203 2023-04-22 07:23:45.594956 pydyndns-1.2.1/setup.cfg
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-04-22 07:23:45.556956 pydyndns-1.2.1/src/
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-04-22 07:23:45.591956 pydyndns-1.2.1/src/pydyndns/
+-rw-r--r--   0 chead     (1000) chead     (1000)    17488 2023-04-22 07:20:35.000000 pydyndns-1.2.1/src/pydyndns/__init__.py
+drwxr-xr-x   0 chead     (1000) chead     (1000)        0 2023-04-22 07:23:45.592956 pydyndns-1.2.1/src/pydyndns.egg-info/
+-rw-r--r--   0 chead     (1000) chead     (1000)     6100 2023-04-22 07:23:45.000000 pydyndns-1.2.1/src/pydyndns.egg-info/PKG-INFO
+-rw-r--r--   0 chead     (1000) chead     (1000)      442 2023-04-22 07:23:45.000000 pydyndns-1.2.1/src/pydyndns.egg-info/SOURCES.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)        1 2023-04-22 07:23:45.000000 pydyndns-1.2.1/src/pydyndns.egg-info/dependency_links.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)       43 2023-04-22 07:23:45.000000 pydyndns-1.2.1/src/pydyndns.egg-info/entry_points.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)       19 2023-04-22 07:23:45.000000 pydyndns-1.2.1/src/pydyndns.egg-info/requires.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)        9 2023-04-22 07:23:45.000000 pydyndns-1.2.1/src/pydyndns.egg-info/top_level.txt
+-rw-r--r--   0 chead     (1000) chead     (1000)        1 2023-04-22 07:23:45.000000 pydyndns-1.2.1/src/pydyndns.egg-info/zip-safe
```

### Comparing `pydyndns-1.2.0/LICENSE.txt` & `pydyndns-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydyndns-1.2.0/PKG-INFO` & `pydyndns-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pydyndns
-Version: 1.2.0
+Version: 1.2.1
 Summary: Sends dynamic DNS updates to a DNS server.
 Home-page: https://gitlab.com/Hawk777/pydyndns
 Author: Christopher Head
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: Name Service (DNS)
@@ -37,15 +35,15 @@
 
 
 Dependencies
 ============
 
 PyDynDNS requires the following packages, all of which are available via `pip`:
 * dnspython
-* netifaces
+* ifaddr
 
 
 
 Usage
 =====
 
 PyDynDNS can be invoked from the command line. It uses standard command-line
@@ -170,9 +168,7 @@
 	},
 	"root": {
 		"level": "WARNING",
 		"handlers": ["eventlog"]
 	}
 }
 ```
-
-
```

### Comparing `pydyndns-1.2.0/README.md` & `pydyndns-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 Dependencies
 ============
 
 PyDynDNS requires the following packages, all of which are available via `pip`:
 * dnspython
-* netifaces
+* ifaddr
 
 
 
 Usage
 =====
 
 PyDynDNS can be invoked from the command line. It uses standard command-line
```

### Comparing `pydyndns-1.2.0/examples/tasksched/Force.xml` & `pydyndns-1.2.1/examples/tasksched/Force.xml`

 * *Files identical despite different names*

### Comparing `pydyndns-1.2.0/examples/tasksched/Normal.xml` & `pydyndns-1.2.1/examples/tasksched/Normal.xml`

 * *Files identical despite different names*

### Comparing `pydyndns-1.2.0/setup.cfg` & `pydyndns-1.2.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydyndns
-version = 1.2.0
+version = 1.2.1
 url = https://gitlab.com/Hawk777/pydyndns
 author = Christopher Head
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: No Input/Output (Daemon)
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: MIT License
```

### Comparing `pydyndns-1.2.0/src/pydyndns/__init__.py` & `pydyndns-1.2.1/src/pydyndns/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,7 +451,8 @@
     # Run the program.
     try:
         run(platform, args, config, logging.getLogger("pydyndns"))
     except (KeyboardInterrupt, SystemExit):
         raise
     except:
         logging.getLogger("pydyndns").error("Unhandled exception", exc_info=True)
+        sys.exit(1)
```

### Comparing `pydyndns-1.2.0/src/pydyndns.egg-info/PKG-INFO` & `pydyndns-1.2.1/src/pydyndns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 Metadata-Version: 2.1
 Name: pydyndns
-Version: 1.2.0
+Version: 1.2.1
 Summary: Sends dynamic DNS updates to a DNS server.
 Home-page: https://gitlab.com/Hawk777/pydyndns
 Author: Christopher Head
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Internet :: Name Service (DNS)
@@ -37,15 +35,15 @@
 
 
 Dependencies
 ============
 
 PyDynDNS requires the following packages, all of which are available via `pip`:
 * dnspython
-* netifaces
+* ifaddr
 
 
 
 Usage
 =====
 
 PyDynDNS can be invoked from the command line. It uses standard command-line
@@ -170,9 +168,7 @@
 	},
 	"root": {
 		"level": "WARNING",
 		"handlers": ["eventlog"]
 	}
 }
 ```
-
-
```

