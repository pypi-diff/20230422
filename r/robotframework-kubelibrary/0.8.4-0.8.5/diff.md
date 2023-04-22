# Comparing `tmp/robotframework-kubelibrary-0.8.4.tar.gz` & `tmp/robotframework-kubelibrary-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-kubelibrary-0.8.4.tar", last modified: Mon Apr 10 17:43:06 2023, max compression
+gzip compressed data, was "robotframework-kubelibrary-0.8.5.tar", last modified: Sat Apr 22 07:04:23 2023, max compression
```

## Comparing `robotframework-kubelibrary-0.8.4.tar` & `robotframework-kubelibrary-0.8.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6213 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/src/KubeLibrary/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    60866 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/src/KubeLibrary/KubeLibrary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/src/KubeLibrary/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/src/KubeLibrary/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/src/KubeLibrary/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-10 17:43:06.000000 robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-10 17:43:06.643914 robotframework-kubelibrary-0.8.4/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42996 2023-04-10 17:43:00.000000 robotframework-kubelibrary-0.8.4/test/test_KubeLibrary.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6213 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1211 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/src/KubeLibrary/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    61132 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/src/KubeLibrary/KubeLibrary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/src/KubeLibrary/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/src/KubeLibrary/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/src/KubeLibrary/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6871 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-04-22 07:04:23.000000 robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-22 07:04:23.181756 robotframework-kubelibrary-0.8.5/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42996 2023-04-22 07:04:17.000000 robotframework-kubelibrary-0.8.5/test/test_KubeLibrary.py
```

### Comparing `robotframework-kubelibrary-0.8.4/LICENSE` & `robotframework-kubelibrary-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-kubelibrary-0.8.4/PKG-INFO` & `robotframework-kubelibrary-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-kubelibrary
-Version: 0.8.4
+Version: 0.8.5
 Summary: Kubernetes library for Robot Framework
 Home-page: https://github.com/devopsspiral/KubeLibrary
 Author: Michał Wcisło
 Author-email: mwcislo999@gmail.com
 License: MIT
 Keywords: robotframework testing test automation kubernetes
 Platform: UNKNOWN
```

### Comparing `robotframework-kubelibrary-0.8.4/README.md` & `robotframework-kubelibrary-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-kubelibrary-0.8.4/setup.py` & `robotframework-kubelibrary-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-kubelibrary-0.8.4/src/KubeLibrary/KubeLibrary.py` & `robotframework-kubelibrary-0.8.5/src/KubeLibrary/KubeLibrary.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,18 @@
                            ca_cert=ca_cert, incluster=incluster, cert_validation=cert_validation)
 
     @staticmethod
     def get_proxy():
         return environ.get('https_proxy') or environ.get('HTTPS_PROXY') or environ.get('http_proxy') or environ.get('HTTP_PROXY')
 
     @staticmethod
+    def get_no_proxy():
+        return environ.get('no_proxy') or environ.get('NO_PROXY')
+
+    @staticmethod
     def generate_alphanumeric_str(size):
         """Generates a random alphanumeric string with given size.
 
         Returns a string.
 
         - ``size``:
           Desired size of the output string
@@ -248,23 +252,25 @@
                 logger.error('Are you sure tests are executed from within k8s cluster?')
                 raise e
         elif api_url and bearer_token:
             if bearer_token.startswith('Bearer '):
                 raise BearerTokenWithPrefixException
             configuration = client.Configuration()
             configuration._default.proxy = KubeLibrary.get_proxy()
+            configuration._default.no_proxy = KubeLibrary.get_no_proxy()
             configuration.api_key["authorization"] = bearer_token
             configuration.api_key_prefix['authorization'] = 'Bearer'
             configuration.host = api_url
             configuration.ssl_ca_cert = ca_cert
             self.api_client = client.ApiClient(configuration)
         else:
             try:
                 config.load_kube_config(kube_config, context)
                 client.Configuration._default.proxy = KubeLibrary.get_proxy()
+                client.Configuration._default.no_proxy = KubeLibrary.get_no_proxy()
             except TypeError:
                 logger.error('Neither KUBECONFIG nor ~/.kube/config available.')
 
         if not self.api_client:
             self.api_client = client.ApiClient(configuration=client.Configuration().get_default_copy())
 
         self._add_api('v1', client.CoreV1Api)
```

### Comparing `robotframework-kubelibrary-0.8.4/src/robotframework_kubelibrary.egg-info/PKG-INFO` & `robotframework-kubelibrary-0.8.5/src/robotframework_kubelibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-kubelibrary
-Version: 0.8.4
+Version: 0.8.5
 Summary: Kubernetes library for Robot Framework
 Home-page: https://github.com/devopsspiral/KubeLibrary
 Author: Michał Wcisło
 Author-email: mwcislo999@gmail.com
 License: MIT
 Keywords: robotframework testing test automation kubernetes
 Platform: UNKNOWN
```

### Comparing `robotframework-kubelibrary-0.8.4/test/test_KubeLibrary.py` & `robotframework-kubelibrary-0.8.5/test/test_KubeLibrary.py`

 * *Files identical despite different names*

