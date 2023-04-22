# Comparing `tmp/graphql_http_server-1.4.0.tar.gz` & `tmp/graphql_http_server-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_http_server-1.4.0.tar", last modified: Sat Apr 22 11:47:56 2023, max compression
+gzip compressed data, was "graphql_http_server-1.4.1.tar", last modified: Sat Apr 22 18:09:14 2023, max compression
```

## Comparing `graphql_http_server-1.4.0.tar` & `graphql_http_server-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.753238 graphql_http_server-1.4.0/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-22 11:47:56.753238 graphql_http_server-1.4.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       90 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.749238 graphql_http_server-1.4.0/graphql_http_server/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.751238 graphql_http_server-1.4.0/graphql_http_server/graphiql/
--rw-rw-rw-   0 root         (0) root         (0)     3103 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/graphiql/index.html
--rw-rw-rw-   0 root         (0) root         (0)     6785 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     9135 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/graphql_http_server/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.751238 graphql_http_server-1.4.0/graphql_http_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-22 11:47:56.000000 graphql_http_server-1.4.0/graphql_http_server.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-22 11:47:56.753238 graphql_http_server-1.4.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 11:47:56.753238 graphql_http_server-1.4.0/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/app.py
--rwxrwxrwx   0 root         (0) root         (0)      476 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)     1984 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/test_app.py
--rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-22 11:47:46.000000 graphql_http_server-1.4.0/tests/test_graphql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 18:09:14.117907 graphql_http_server-1.4.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-22 18:09:14.118823 graphql_http_server-1.4.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       90 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-22 18:09:13.000000 graphql_http_server-1.4.1/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 18:09:14.115157 graphql_http_server-1.4.1/graphql_http_server/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/graphql_http_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/graphql_http_server/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 18:09:14.116990 graphql_http_server-1.4.1/graphql_http_server/graphiql/
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/graphql_http_server/graphiql/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     6785 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/graphql_http_server/helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9135 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/graphql_http_server/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 18:09:14.116990 graphql_http_server-1.4.1/graphql_http_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-22 18:09:14.000000 graphql_http_server-1.4.1/graphql_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-22 18:09:14.000000 graphql_http_server-1.4.1/graphql_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 18:09:14.000000 graphql_http_server-1.4.1/graphql_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-04-22 18:09:14.000000 graphql_http_server-1.4.1/graphql_http_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-22 18:09:14.000000 graphql_http_server-1.4.1/graphql_http_server.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-22 18:09:14.118823 graphql_http_server-1.4.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1330 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 18:09:14.117907 graphql_http_server-1.4.1/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/tests/app.py
+-rwxrwxrwx   0 root         (0) root         (0)      476 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/tests/conftest.py
+-rwxrwxrwx   0 root         (0) root         (0)     1984 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/tests/test_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     2771 2023-04-22 18:09:04.000000 graphql_http_server-1.4.1/tests/test_graphql_api.py
```

### Comparing `graphql_http_server-1.4.0/LICENSE` & `graphql_http_server-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.0/PKG-INFO` & `graphql_http_server-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_http_server
-Version: 1.4.0
+Version: 1.4.1
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.0.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.1.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.0/graphql_http_server/error.py` & `graphql_http_server-1.4.1/graphql_http_server/error.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.0/graphql_http_server/graphiql/index.html` & `graphql_http_server-1.4.1/graphql_http_server/graphiql/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,14 @@
         });
         return React.createElement(GraphiQL, {
             fetcher: GraphiQL.createFetcher({
                 url: fetchURL,
             }),
             defaultEditorToolsVisibility: true,
             plugins: [explorerPlugin],
-            visiblePlugin: explorerPlugin,
             query: query,
             onEditQuery: setQuery,
             schemaDescription: "test"
         });
     }
 
     ReactDOM.render(
```

### Comparing `graphql_http_server-1.4.0/graphql_http_server/helpers.py` & `graphql_http_server-1.4.1/graphql_http_server/helpers.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.0/graphql_http_server/server.py` & `graphql_http_server-1.4.1/graphql_http_server/server.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.0/graphql_http_server.egg-info/PKG-INFO` & `graphql_http_server-1.4.1/graphql_http_server.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-http-server
-Version: 1.4.0
+Version: 1.4.1
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.0.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.1.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.0/graphql_http_server.egg-info/SOURCES.txt` & `graphql_http_server-1.4.1/graphql_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.0/setup.py` & `graphql_http_server-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.0/tests/test_app.py` & `graphql_http_server-1.4.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.0/tests/test_graphql_api.py` & `graphql_http_server-1.4.1/tests/test_graphql_api.py`

 * *Files identical despite different names*

