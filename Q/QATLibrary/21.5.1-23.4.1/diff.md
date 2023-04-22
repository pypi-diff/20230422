# Comparing `tmp/QATLibrary-21.5.1.tar.gz` & `tmp/QATLibrary-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QATLibrary-21.5.1.tar", last modified: Fri Apr 30 19:05:13 2021, max compression
+gzip compressed data, was "QATLibrary-23.4.1.tar", last modified: Sat Apr 22 00:18:10 2023, max compression
```

## Comparing `QATLibrary-21.5.1.tar` & `QATLibrary-23.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 19:05:13.627740 QATLibrary-21.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-04-30 19:04:57.000000 QATLibrary-21.5.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     7763 2021-04-30 19:05:13.627740 QATLibrary-21.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5565 2021-04-30 19:04:57.000000 QATLibrary-21.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2021-04-30 19:05:13.631740 QATLibrary-21.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-30 19:04:57.000000 QATLibrary-21.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 19:05:13.627740 QATLibrary-21.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 19:05:13.627740 QATLibrary-21.5.1/src/QATLibrary/
--rw-r--r--   0 runner    (1001) docker     (121)    17048 2021-04-30 19:04:57.000000 QATLibrary-21.5.1/src/QATLibrary/QATLibrary.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-04-30 19:04:57.000000 QATLibrary-21.5.1/src/QATLibrary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-04-30 19:04:57.000000 QATLibrary-21.5.1/src/QATLibrary/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6367 2021-04-30 19:04:57.000000 QATLibrary-21.5.1/src/QATLibrary/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    12033 2021-04-30 19:04:57.000000 QATLibrary-21.5.1/src/QATLibrary/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-04-30 19:04:57.000000 QATLibrary-21.5.1/src/QATLibrary/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-30 19:05:13.627740 QATLibrary-21.5.1/src/QATLibrary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7763 2021-04-30 19:05:13.000000 QATLibrary-21.5.1/src/QATLibrary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      465 2021-04-30 19:05:13.000000 QATLibrary-21.5.1/src/QATLibrary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-30 19:05:13.000000 QATLibrary-21.5.1/src/QATLibrary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-04-30 19:05:13.000000 QATLibrary-21.5.1/src/QATLibrary.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-30 19:05:13.000000 QATLibrary-21.5.1/src/QATLibrary.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-04-30 19:05:13.000000 QATLibrary-21.5.1/src/QATLibrary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-04-30 19:05:13.000000 QATLibrary-21.5.1/src/QATLibrary.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:10.107556 QATLibrary-23.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/src/QATLibrary/
+-rw-r--r--   0 runner    (1001) docker     (123)    17056 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/QATLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12033 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-22 00:17:50.000000 QATLibrary-23.4.1/src/QATLibrary/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:18:10.111556 QATLibrary-23.4.1/src/QATLibrary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 00:18:10.000000 QATLibrary-23.4.1/src/QATLibrary.egg-info/top_level.txt
```

### Comparing `QATLibrary-21.5.1/LICENSE.md` & `QATLibrary-23.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `QATLibrary-21.5.1/PKG-INFO` & `QATLibrary-23.4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,160 +1,163 @@
 Metadata-Version: 2.1
 Name: QATLibrary
-Version: 21.5.1
+Version: 23.4.1
 Summary: Data/Configuration Driven REST API Test Automation Library. Can be used as a Robot Framework Library or as standalone CLI tool.
 Home-page: https://github.com/sharif314/QATLibrary
 Author: Sharif Rahman
 Author-email: shrif.sbu@gmail.com
 License: MIT
 Project-URL: Docs, https://github.com/sharif314/QATLibrary/README.md
 Project-URL: Issue Tracker, https://github.com/sharif314/QATLibrary/issues
-Description: # QATLibrary 
-        ![gh ci](https://github.com/sharif314/QATLibrary/workflows/QATLibrary%20CI/badge.svg)
-        ![gh tests](https://github.com/sharif314/QATLibrary/workflows/Test/badge.svg)
-        [![PyPI version](https://badge.fury.io/py/QATLibrary.svg)](https://badge.fury.io/py/QATLibrary)
-        [![Maintenance](https://img.shields.io/badge/Maintained%3F-Yes-blue.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-        
-        
-        QAT (Quick API Tests) Library is a Data/Configuration Driven REST API Test Automation Library. 
-        Can be used as a Robot Framework Library or as standalone tool (CLI). This tool does not solve complex 
-        REST API automation scenarios, rather, provides a simple, lightweight and data-driven approach to create 
-        automated REST API tests quickly. For complex flows, it is recommended to use the library with Robot 
-        Framework. 
-        
-        ## Features
-        * No coding required. Quick and easy implementation for REST API Tests. 
-        * Initialize sample config and Test Data with a single command. 
-        * Run from CLI (CI/CD friendly).
-        * Store Test Data, Documentation and Assertions in CSV File. 
-        * Authorization: Basic, Digest, OAuth1
-        * Run as a Robot Framework Library with Dynamic Test Generation Support. 
-        * Supports all HTTP Methods, SSL Certificates, Proxy Server, Stream, Redirection, Request Timeout etc.
-        * Robot Framework based execution, reports and logs (CLI or Library). 
-        
-        ### Built-in Assertions
-        * Status Code
-        * JSON Schema
-        * Response Body 
-        * Response Headers
-        * Response Time/SLA
-        * Server Certificate
-        
-        ## Install QATLibrary
-        ``QATLibrary`` is available in [PyPI](https://pypi.org/project/QATLibrary/). You can install using [Pip](https://pip.pypa.io/en/stable/):
-        ```shell 
-        pip install qatlibrary
-        ```
-        
-        ## Execution 
-        #### Getting started from scratch is only a few commands away. Follow - 
-        1. Generate Sample Test Data CSV and Config YAML from CLI run _(Skip this step if you already have Test Data and Config files)_:
-            ```shell 
-            qat init
-            ```
-        2. Execute Tests Using CLI _(standalone)_:
-            ```shell
-            qat run -c config.yaml -f TestCases.csv
-            ```
-        3. Delete report files (*.html and *.xml) in current directory:
-            ```shell
-            qat clean
-            ```
-            or to clean a specific report directory:
-            ```shell
-            qat clean -d path/to/dir
-            ```
-        
-        4. For CLI Help (shows all required and optional args, usage etc):
-            ```shell
-            qat --help
-            ```
-        
-        ## Use as Robot Framework Library
-        Example:
-        
-        ```robot
-        *** Settings ***
-        Library          QATLibrary
-        Suite Setup      QAT Dynamic Tests Setup        csvFile=${csvData}
-        Variables        config.yaml        # Or can be a robot framework variable (Test/Suite/Variablefile etc.)
-        
-        *** Variables ***
-        ${host}          httpbin.org
-        ${csvData}       Tests.csv
-        
-        *** Test Cases ***
-        Place Holder Test
-            [Documentation]  Placeholder Test Required by Robot Framework Suite Runner.  
-            No Operaiton 
-        
-        ```
-        
-        ## Configurations and Test Data
-        QATLibrary requires a CSV file with required data to drive the tests. Config yaml or .py files can inject your desired
-        configurations during execution. 
-        
-        Generating Sample Test Data CSV and Config YAML is easy. Simply run:
-        
-        ```shell 
-        qat init
-        ```
-        
-        This command should generate two sample files like below - 
-        1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
-        Test cases gets generated based on this file's content using Robot Framework. 
-        
-        2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
-        for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
-            ```yaml
-            host: httpbin.org           # Required
-            
-            #optional args
-            timeout: 5                  # Default 5 seconds
-            allow_redirects:            # Allow Redirects. Default True. 
-            stream:                     # True/False. 
-            http_proxy:                 # HTTP Proxy. Default None. 
-            https_proxy:                # HTTPS Proxy. Default None.
-            
-            verify_server_cert: True    # True/False or path to CA Bundle. Default False. 
-            certificate:                # .pem format certificate. Default None
-            private_key:                # .pem format private key (unencrypted). Default None
-            
-            # Required if using Basic/Digest Auth (Default None)
-            authUser:             
-            authPass:
-            
-            # Required if using OAuth1 auth (Default None)
-            oauth1_app_key:
-            oauth1_app_secret:
-            oauth1_user_token:
-            oauth1_user_token_secret:
-            ```
-        
-        Once the files are generated, you can rename them according to your test suites or requirements.  
-        
-        ## Contributing
-        This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
-        a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done 
-        quickly for your projects without coding and powerful assertion methods out of the box. 
-        
-        QATLibrary is on [GitHub](https://github.com/sharif314/QATLibrary). 
-        Get in touch, via GitHub or otherwise, if you've got something to contribute, it'd be most welcome! 
-        Please follow the [CONTRIBUTING.md](https://github.com/sharif314/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
-        
-        ## License 
-        QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md](https://github.com/sharif314/QATLibrary/blob/main/LICENSE.md) for more details. 
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# QATLibrary 
+![gh ci](https://github.com/sharif314/QATLibrary/workflows/QATLibrary%20CI/badge.svg)
+![gh tests](https://github.com/sharif314/QATLibrary/workflows/Test/badge.svg)
+[![PyPI version](https://badge.fury.io/py/QATLibrary.svg)](https://badge.fury.io/py/QATLibrary)
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-Yes-blue.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+
+QAT (Quick API Tests) Library is a Data/Configuration Driven REST API Test Automation Library. 
+Can be used as a Robot Framework Library or as standalone tool (CLI). This tool does not solve complex 
+REST API automation scenarios, rather, provides a simple, lightweight and data-driven approach to create 
+automated REST API tests quickly. For complex flows, it is recommended to use the library with Robot 
+Framework. 
+
+## Features
+* No coding required. Quick and easy implementation for REST API Tests. 
+* Initialize sample config and Test Data with a single command. 
+* Run from CLI (CI/CD friendly).
+* Store Test Data, Documentation and Assertions in CSV File. 
+* Authorization: Basic, Digest, OAuth1
+* Run as a Robot Framework Library with Dynamic Test Generation Support. 
+* Supports all HTTP Methods, SSL Certificates, Proxy Server, Stream, Redirection, Request Timeout etc.
+* Robot Framework based execution, reports and logs (CLI or Library). 
+
+### Built-in Assertions
+* Status Code
+* JSON Schema
+* Response Body 
+* Response Headers
+* Response Time/SLA
+* Server Certificate
+
+## Install QATLibrary
+``QATLibrary`` is available in [PyPI](https://pypi.org/project/QATLibrary/). You can install using [Pip](https://pip.pypa.io/en/stable/):
+```shell 
+pip install qatlibrary
+```
+
+## Execution 
+#### Getting started from scratch is only a few commands away. Follow - 
+1. Generate Sample Test Data CSV and Config YAML from CLI run _(Skip this step if you already have Test Data and Config files)_:
+    ```shell 
+    qat init
+    ```
+2. Execute Tests Using CLI _(standalone)_:
+    ```shell
+    qat run -c config.yaml -f TestCases.csv
+    ```
+3. Delete report files (*.html and *.xml) in current directory:
+    ```shell
+    qat clean
+    ```
+    or to clean a specific report directory:
+    ```shell
+    qat clean -d path/to/dir
+    ```
+
+4. For CLI Help (shows all required and optional args, usage etc):
+    ```shell
+    qat --help
+    ```
+
+## Use as Robot Framework Library
+Example:
+
+```robot
+*** Settings ***
+Library          QATLibrary
+Suite Setup      QAT Dynamic Tests Setup        csvFile=${csvData}
+Variables        config.yaml        # Or can be a robot framework variable (Test/Suite/Variablefile etc.)
+
+*** Variables ***
+${host}          httpbin.org
+${csvData}       Tests.csv
+
+*** Test Cases ***
+Place Holder Test
+    [Documentation]  Placeholder Test Required by Robot Framework Suite Runner.  
+    No Operaiton 
+
+```
+
+## Configurations and Test Data
+QATLibrary requires a CSV file with required data to drive the tests. Config yaml or .py files can inject your desired
+configurations during execution. 
+
+Generating Sample Test Data CSV and Config YAML is easy. Simply run:
+
+```shell 
+qat init
+```
+
+This command should generate two sample files like below - 
+1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
+Test cases gets generated based on this file's content using Robot Framework. 
+
+2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
+for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
+    ```yaml
+    host: httpbin.org           # Required
+    
+    #optional args
+    timeout: 5                  # Default 5 seconds
+    allow_redirects:            # Allow Redirects. Default True. 
+    stream:                     # True/False. 
+    http_proxy:                 # HTTP Proxy. Default None. 
+    https_proxy:                # HTTPS Proxy. Default None.
+    
+    verify_server_cert: True    # True/False or path to CA Bundle. Default False. 
+    certificate:                # .pem format certificate. Default None
+    private_key:                # .pem format private key (unencrypted). Default None
+    
+    # Required if using Basic/Digest Auth (Default None)
+    authUser:             
+    authPass:
+    
+    # Required if using OAuth1 auth (Default None)
+    oauth1_app_key:
+    oauth1_app_secret:
+    oauth1_user_token:
+    oauth1_user_token_secret:
+    ```
+
+Once the files are generated, you can rename them according to your test suites or requirements.  
+
+## Contributing
+This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
+a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done 
+quickly for your projects without coding and powerful assertion methods out of the box. 
+
+QATLibrary is on [GitHub](https://github.com/sharif314/QATLibrary). 
+Get in touch, via GitHub or otherwise, if you've got something to contribute, it'd be most welcome! 
+Please follow the [CONTRIBUTING.md](https://github.com/sharif314/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
+
+## License 
+QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md](https://github.com/sharif314/QATLibrary/blob/main/LICENSE.md) for more details. 
+
+
```

### Comparing `QATLibrary-21.5.1/README.md` & `QATLibrary-23.4.1/README.md`

 * *Files identical despite different names*

### Comparing `QATLibrary-21.5.1/setup.cfg` & `QATLibrary-23.4.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,22 @@
 zip_safe = False
 include_package_data = True
 package_dir = 
 	=src
 packages = find:
 setup_requires = 
 	requests>2
-	robotframework<4
+	robotframework>4
 	requests_oauthlib>1
 	pyyaml>5
 	jsonschema>3
 	termcolor>1.0
 install_requires = 
 	requests>2
-	robotframework<4
+	robotframework>4
 	requests_oauthlib>1
 	pyyaml>5
 	jsonschema>3
 	termcolor>1.0
 
 [options.packages.find]
 where = src
```

### Comparing `QATLibrary-21.5.1/src/QATLibrary/QATLibrary.py` & `QATLibrary-23.4.1/src/QATLibrary/QATLibrary.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,19 +48,19 @@
 
         try:
             for testCase in data:
                 if testCase['execute'] not in ['N', 'False', 'false']:
                     tc = self.current_suite.tests.create(name=testCase['testName'] or 'Untitled Test',
                                                          tags=self.__setup_test_tags(testCase),
                                                          doc=self.__setup_test_documentation(testCase))
-                    tc.keywords.create(name='Data Driven HTTP Request',
+                    tc.body.create_keyword(name='Data Driven HTTP Request',
                                        args=[testCase])
 
                     if kwname is not None:
-                        tc.keywords.create(name=kwname, args=args)
+                        tc.body.create_keyword(name=kwname, args=args)
             logger.info('Dynamic Tests Creation Successful!')
         except Exception as e:
             logger.error(e)
             raise Exception('Dynamic Tests creation failed!')
 
     @keyword('Data Driven HTTP Request')
     def qat_data_driven_http_request(self, data):
```

### Comparing `QATLibrary-21.5.1/src/QATLibrary/cli.py` & `QATLibrary-23.4.1/src/QATLibrary/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 def _create_test_suite(args):
     print_qat_cli_intro(args)
     suite = TestSuite(name=args.file.split('/')[-1] + ' | ' + 'QAT ',
                       doc='Runs (Quick) API Tests from Input CSV Data')
     suite.resource.imports.library('QATLibrary')
 
-    suite.keywords.create('QAT Dynamic Tests Setup', args=[args.file, args.encoding], type='setup')
+    suite.setup.config(name='QAT Dynamic Tests Setup', args=[args.file, args.encoding])
     settings = RobotSettings(output=args.output,
                              report=args.report,
                              loglevel=args.loglevel,
                              log=args.log,
                              variablefile=args.config)
 
     with pyloggingconf.robot_handler_enabled(settings.log_level):
```

### Comparing `QATLibrary-21.5.1/src/QATLibrary/templates.py` & `QATLibrary-23.4.1/src/QATLibrary/templates.py`

 * *Files identical despite different names*

### Comparing `QATLibrary-21.5.1/src/QATLibrary.egg-info/PKG-INFO` & `QATLibrary-23.4.1/src/QATLibrary.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,160 +1,163 @@
 Metadata-Version: 2.1
 Name: QATLibrary
-Version: 21.5.1
+Version: 23.4.1
 Summary: Data/Configuration Driven REST API Test Automation Library. Can be used as a Robot Framework Library or as standalone CLI tool.
 Home-page: https://github.com/sharif314/QATLibrary
 Author: Sharif Rahman
 Author-email: shrif.sbu@gmail.com
 License: MIT
 Project-URL: Docs, https://github.com/sharif314/QATLibrary/README.md
 Project-URL: Issue Tracker, https://github.com/sharif314/QATLibrary/issues
-Description: # QATLibrary 
-        ![gh ci](https://github.com/sharif314/QATLibrary/workflows/QATLibrary%20CI/badge.svg)
-        ![gh tests](https://github.com/sharif314/QATLibrary/workflows/Test/badge.svg)
-        [![PyPI version](https://badge.fury.io/py/QATLibrary.svg)](https://badge.fury.io/py/QATLibrary)
-        [![Maintenance](https://img.shields.io/badge/Maintained%3F-Yes-blue.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
-        [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-        
-        
-        QAT (Quick API Tests) Library is a Data/Configuration Driven REST API Test Automation Library. 
-        Can be used as a Robot Framework Library or as standalone tool (CLI). This tool does not solve complex 
-        REST API automation scenarios, rather, provides a simple, lightweight and data-driven approach to create 
-        automated REST API tests quickly. For complex flows, it is recommended to use the library with Robot 
-        Framework. 
-        
-        ## Features
-        * No coding required. Quick and easy implementation for REST API Tests. 
-        * Initialize sample config and Test Data with a single command. 
-        * Run from CLI (CI/CD friendly).
-        * Store Test Data, Documentation and Assertions in CSV File. 
-        * Authorization: Basic, Digest, OAuth1
-        * Run as a Robot Framework Library with Dynamic Test Generation Support. 
-        * Supports all HTTP Methods, SSL Certificates, Proxy Server, Stream, Redirection, Request Timeout etc.
-        * Robot Framework based execution, reports and logs (CLI or Library). 
-        
-        ### Built-in Assertions
-        * Status Code
-        * JSON Schema
-        * Response Body 
-        * Response Headers
-        * Response Time/SLA
-        * Server Certificate
-        
-        ## Install QATLibrary
-        ``QATLibrary`` is available in [PyPI](https://pypi.org/project/QATLibrary/). You can install using [Pip](https://pip.pypa.io/en/stable/):
-        ```shell 
-        pip install qatlibrary
-        ```
-        
-        ## Execution 
-        #### Getting started from scratch is only a few commands away. Follow - 
-        1. Generate Sample Test Data CSV and Config YAML from CLI run _(Skip this step if you already have Test Data and Config files)_:
-            ```shell 
-            qat init
-            ```
-        2. Execute Tests Using CLI _(standalone)_:
-            ```shell
-            qat run -c config.yaml -f TestCases.csv
-            ```
-        3. Delete report files (*.html and *.xml) in current directory:
-            ```shell
-            qat clean
-            ```
-            or to clean a specific report directory:
-            ```shell
-            qat clean -d path/to/dir
-            ```
-        
-        4. For CLI Help (shows all required and optional args, usage etc):
-            ```shell
-            qat --help
-            ```
-        
-        ## Use as Robot Framework Library
-        Example:
-        
-        ```robot
-        *** Settings ***
-        Library          QATLibrary
-        Suite Setup      QAT Dynamic Tests Setup        csvFile=${csvData}
-        Variables        config.yaml        # Or can be a robot framework variable (Test/Suite/Variablefile etc.)
-        
-        *** Variables ***
-        ${host}          httpbin.org
-        ${csvData}       Tests.csv
-        
-        *** Test Cases ***
-        Place Holder Test
-            [Documentation]  Placeholder Test Required by Robot Framework Suite Runner.  
-            No Operaiton 
-        
-        ```
-        
-        ## Configurations and Test Data
-        QATLibrary requires a CSV file with required data to drive the tests. Config yaml or .py files can inject your desired
-        configurations during execution. 
-        
-        Generating Sample Test Data CSV and Config YAML is easy. Simply run:
-        
-        ```shell 
-        qat init
-        ```
-        
-        This command should generate two sample files like below - 
-        1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
-        Test cases gets generated based on this file's content using Robot Framework. 
-        
-        2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
-        for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
-            ```yaml
-            host: httpbin.org           # Required
-            
-            #optional args
-            timeout: 5                  # Default 5 seconds
-            allow_redirects:            # Allow Redirects. Default True. 
-            stream:                     # True/False. 
-            http_proxy:                 # HTTP Proxy. Default None. 
-            https_proxy:                # HTTPS Proxy. Default None.
-            
-            verify_server_cert: True    # True/False or path to CA Bundle. Default False. 
-            certificate:                # .pem format certificate. Default None
-            private_key:                # .pem format private key (unencrypted). Default None
-            
-            # Required if using Basic/Digest Auth (Default None)
-            authUser:             
-            authPass:
-            
-            # Required if using OAuth1 auth (Default None)
-            oauth1_app_key:
-            oauth1_app_secret:
-            oauth1_user_token:
-            oauth1_user_token_secret:
-            ```
-        
-        Once the files are generated, you can rename them according to your test suites or requirements.  
-        
-        ## Contributing
-        This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
-        a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done 
-        quickly for your projects without coding and powerful assertion methods out of the box. 
-        
-        QATLibrary is on [GitHub](https://github.com/sharif314/QATLibrary). 
-        Get in touch, via GitHub or otherwise, if you've got something to contribute, it'd be most welcome! 
-        Please follow the [CONTRIBUTING.md](https://github.com/sharif314/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
-        
-        ## License 
-        QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md](https://github.com/sharif314/QATLibrary/blob/main/LICENSE.md) for more details. 
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# QATLibrary 
+![gh ci](https://github.com/sharif314/QATLibrary/workflows/QATLibrary%20CI/badge.svg)
+![gh tests](https://github.com/sharif314/QATLibrary/workflows/Test/badge.svg)
+[![PyPI version](https://badge.fury.io/py/QATLibrary.svg)](https://badge.fury.io/py/QATLibrary)
+[![Maintenance](https://img.shields.io/badge/Maintained%3F-Yes-blue.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
+
+
+QAT (Quick API Tests) Library is a Data/Configuration Driven REST API Test Automation Library. 
+Can be used as a Robot Framework Library or as standalone tool (CLI). This tool does not solve complex 
+REST API automation scenarios, rather, provides a simple, lightweight and data-driven approach to create 
+automated REST API tests quickly. For complex flows, it is recommended to use the library with Robot 
+Framework. 
+
+## Features
+* No coding required. Quick and easy implementation for REST API Tests. 
+* Initialize sample config and Test Data with a single command. 
+* Run from CLI (CI/CD friendly).
+* Store Test Data, Documentation and Assertions in CSV File. 
+* Authorization: Basic, Digest, OAuth1
+* Run as a Robot Framework Library with Dynamic Test Generation Support. 
+* Supports all HTTP Methods, SSL Certificates, Proxy Server, Stream, Redirection, Request Timeout etc.
+* Robot Framework based execution, reports and logs (CLI or Library). 
+
+### Built-in Assertions
+* Status Code
+* JSON Schema
+* Response Body 
+* Response Headers
+* Response Time/SLA
+* Server Certificate
+
+## Install QATLibrary
+``QATLibrary`` is available in [PyPI](https://pypi.org/project/QATLibrary/). You can install using [Pip](https://pip.pypa.io/en/stable/):
+```shell 
+pip install qatlibrary
+```
+
+## Execution 
+#### Getting started from scratch is only a few commands away. Follow - 
+1. Generate Sample Test Data CSV and Config YAML from CLI run _(Skip this step if you already have Test Data and Config files)_:
+    ```shell 
+    qat init
+    ```
+2. Execute Tests Using CLI _(standalone)_:
+    ```shell
+    qat run -c config.yaml -f TestCases.csv
+    ```
+3. Delete report files (*.html and *.xml) in current directory:
+    ```shell
+    qat clean
+    ```
+    or to clean a specific report directory:
+    ```shell
+    qat clean -d path/to/dir
+    ```
+
+4. For CLI Help (shows all required and optional args, usage etc):
+    ```shell
+    qat --help
+    ```
+
+## Use as Robot Framework Library
+Example:
+
+```robot
+*** Settings ***
+Library          QATLibrary
+Suite Setup      QAT Dynamic Tests Setup        csvFile=${csvData}
+Variables        config.yaml        # Or can be a robot framework variable (Test/Suite/Variablefile etc.)
+
+*** Variables ***
+${host}          httpbin.org
+${csvData}       Tests.csv
+
+*** Test Cases ***
+Place Holder Test
+    [Documentation]  Placeholder Test Required by Robot Framework Suite Runner.  
+    No Operaiton 
+
+```
+
+## Configurations and Test Data
+QATLibrary requires a CSV file with required data to drive the tests. Config yaml or .py files can inject your desired
+configurations during execution. 
+
+Generating Sample Test Data CSV and Config YAML is easy. Simply run:
+
+```shell 
+qat init
+```
+
+This command should generate two sample files like below - 
+1. [Sample CSV Test Data](https://github.com/sharif314/QATLibrary/blob/main/sample/TestCases.csv): Test Cases or Data file. 
+Test cases gets generated based on this file's content using Robot Framework. 
+
+2. [Sample Config YAML](https://github.com/sharif314/QATLibrary/blob/main/sample/config.yaml): This file contains various runtime configurations 
+for tests. Can be utilize to accommodate various CI or Test environments. Please follow the inline comments for more details -  
+    ```yaml
+    host: httpbin.org           # Required
+    
+    #optional args
+    timeout: 5                  # Default 5 seconds
+    allow_redirects:            # Allow Redirects. Default True. 
+    stream:                     # True/False. 
+    http_proxy:                 # HTTP Proxy. Default None. 
+    https_proxy:                # HTTPS Proxy. Default None.
+    
+    verify_server_cert: True    # True/False or path to CA Bundle. Default False. 
+    certificate:                # .pem format certificate. Default None
+    private_key:                # .pem format private key (unencrypted). Default None
+    
+    # Required if using Basic/Digest Auth (Default None)
+    authUser:             
+    authPass:
+    
+    # Required if using OAuth1 auth (Default None)
+    oauth1_app_key:
+    oauth1_app_secret:
+    oauth1_user_token:
+    oauth1_user_token_secret:
+    ```
+
+Once the files are generated, you can rename them according to your test suites or requirements.  
+
+## Contributing
+This is [Sharif](https://www.linkedin.com/in/sharif-rahman/). I started this project basically to make my life 
+a bit easier around simple REST API tests. This project is ideal for you if want to get some automated tests done 
+quickly for your projects without coding and powerful assertion methods out of the box. 
+
+QATLibrary is on [GitHub](https://github.com/sharif314/QATLibrary). 
+Get in touch, via GitHub or otherwise, if you've got something to contribute, it'd be most welcome! 
+Please follow the [CONTRIBUTING.md](https://github.com/sharif314/QATLibrary/blob/main/CONTRIBUTING.md) for detailed guidelines.
+
+## License 
+QATLibrary is open source software provided under the MIT License. Please follow [LICENSE.md](https://github.com/sharif314/QATLibrary/blob/main/LICENSE.md) for more details. 
+
+
```

