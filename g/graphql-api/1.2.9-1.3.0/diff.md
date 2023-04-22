# Comparing `tmp/graphql-api-1.2.9.tar.gz` & `tmp/graphql-api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-api-1.2.9.tar", last modified: Thu Sep 22 17:17:08 2022, max compression
+gzip compressed data, was "graphql-api-1.3.0.tar", last modified: Sat Apr 22 10:50:39 2023, max compression
```

## Comparing `graphql-api-1.2.9.tar` & `graphql-api-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 17:17:08.619816 graphql-api-1.2.9/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2022-09-22 17:16:58.000000 graphql-api-1.2.9/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       73 2022-09-22 17:16:58.000000 graphql-api-1.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1945 2022-09-22 17:17:08.619816 graphql-api-1.2.9/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1269 2022-09-22 17:16:58.000000 graphql-api-1.2.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)        7 2022-09-22 17:17:08.000000 graphql-api-1.2.9/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 17:17:08.617816 graphql-api-1.2.9/graphql_api/
--rwxrwxrwx   0 root         (0) root         (0)      286 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6728 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/api.py
--rwxrwxrwx   0 root         (0) root         (0)      560 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/context.py
--rwxrwxrwx   0 root         (0) root         (0)     3166 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/dataclass_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)      592 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/error.py
--rwxrwxrwx   0 root         (0) root         (0)       52 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     4686 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/executor.py
--rwxrwxrwx   0 root         (0) root         (0)    22758 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)     2093 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/middleware.py
--rwxrwxrwx   0 root         (0) root         (0)     6915 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/reduce.py
--rwxrwxrwx   0 root         (0) root         (0)     3122 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/relay.py
--rwxrwxrwx   0 root         (0) root         (0)    33657 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/remote.py
--rwxrwxrwx   0 root         (0) root         (0)     2648 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/types.py
--rwxrwxrwx   0 root         (0) root         (0)     5618 2022-09-22 17:16:58.000000 graphql-api-1.2.9/graphql_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-22 17:17:08.619816 graphql-api-1.2.9/graphql_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1945 2022-09-22 17:17:08.000000 graphql-api-1.2.9/graphql_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2022-09-22 17:17:08.000000 graphql-api-1.2.9/graphql_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-22 17:17:08.000000 graphql-api-1.2.9/graphql_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2022-09-22 17:17:08.000000 graphql-api-1.2.9/graphql_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2022-09-22 17:17:08.000000 graphql-api-1.2.9/graphql_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2022-09-22 17:17:08.619816 graphql-api-1.2.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1442 2022-09-22 17:16:58.000000 graphql-api-1.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:50:39.418552 graphql-api-1.3.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-22 10:50:30.000000 graphql-api-1.3.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-22 10:50:30.000000 graphql-api-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-04-22 10:50:39.418552 graphql-api-1.3.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1269 2023-04-22 10:50:30.000000 graphql-api-1.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-22 10:50:38.000000 graphql-api-1.3.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:50:39.413557 graphql-api-1.3.0/graphql_api/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     8046 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      560 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/context.py
+-rwxrwxrwx   0 root         (0) root         (0)     3693 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/dataclass_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)      592 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/error.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     6166 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/executor.py
+-rwxrwxrwx   0 root         (0) root         (0)    24401 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3073 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/middleware.py
+-rwxrwxrwx   0 root         (0) root         (0)     6915 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/reduce.py
+-rwxrwxrwx   0 root         (0) root         (0)     3161 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    34111 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/remote.py
+-rwxrwxrwx   0 root         (0) root         (0)     3492 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5635 2023-04-22 10:50:30.000000 graphql-api-1.3.0/graphql_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:50:39.414556 graphql-api-1.3.0/graphql_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      806 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-22 10:50:39.000000 graphql-api-1.3.0/graphql_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-22 10:50:39.418552 graphql-api-1.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1483 2023-04-22 10:50:30.000000 graphql-api-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-22 10:50:39.418552 graphql-api-1.3.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5443 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_custom_types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5766 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_docstrings.py
+-rwxrwxrwx   0 root         (0) root         (0)     3128 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     7401 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_filtering.py
+-rwxrwxrwx   0 root         (0) root         (0)    36924 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_graphql.py
+-rwxrwxrwx   0 root         (0) root         (0)     4347 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    19028 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3722 2023-04-22 10:50:30.000000 graphql-api-1.3.0/tests/test_subscriptions.py
```

### Comparing `graphql-api-1.2.9/LICENSE` & `graphql-api-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-api-1.2.9/PKG-INFO` & `graphql-api-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.2.9
+Version: 1.3.0
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.2.9/graphql-api-v1.2.9.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.0/graphql-api-v1.3.0.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.2.9/README.md` & `graphql-api-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `graphql-api-1.2.9/graphql_api/api.py` & `graphql-api-1.3.0/graphql_api/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
     def __init__(self, args, info):
         self.args = args
         self.info = info
 
 
 def decorate(
-    func: Callable,
-    _type: str,
-    schema: "GraphQLAPI" = None,
-    meta: Dict = None
+        func: Callable,
+        _type: str,
+        schema: "GraphQLAPI" = None,
+        meta: Dict = None
 ):
     func.graphql = True
     func.defined_on = func
 
     if not meta:
         meta = {}
 
@@ -85,29 +85,43 @@
         func=_func,
         _type=_type,
         schema=schema,
         meta=meta
     )
 
 
+class GraphQLRootTypeDelegate:
+    infer_subclass_fields = True
+
+    @classmethod
+    def validate_graphql_schema(cls, schema: GraphQLSchema) -> GraphQLSchema:
+        """
+        This method is called whenever a schema is created with this
+        class as the root type.
+        :param schema: The GraphQL schema that is generated by
+        :return:schema: The validated and updated GraphQL schema.
+        """
+        return schema
+
+
 class GraphQLAPI(GraphQLBaseExecutor):
 
     def field(self=None, meta=None, mutable=False):
         _type = "query"
         if mutable:
             _type = "mutation"
 
         return decorator(self, meta, _type=_type)
 
     def type(
-        self=None,
-        meta=None,
-        abstract=False,
-        interface=False,
-        root=False
+            self=None,
+            meta=None,
+            abstract=False,
+            interface=False,
+            root=False
     ):
         _type = "object"
         if interface:
             _type = "interface"
         elif abstract:
             _type = "abstract"
         elif root:
@@ -116,28 +130,30 @@
         return decorator(self, meta, _type=_type)
 
     def set_root(self, root_type):
         self.root_type = root_type
         return root_type
 
     def __init__(
-        self,
-        root: Type = None,
-        middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
-        filters: List[GraphQLFilter] = None
+            self,
+            root: Type = None,
+            middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
+            filters: List[GraphQLFilter] = None,
+            error_protection=True
     ):
         super().__init__()
         if middleware is None:
             middleware = []
 
         self.root_type = root
         self.middleware = middleware
         self.filters = filters
         self.query_mapper = None
         self.mutation_mapper = None
+        self.error_protection = error_protection
 
     def graphql_schema(self) -> Tuple[GraphQLSchema, Dict]:
         schema_args = {}
         meta = {}
 
         if self.root_type:
             # Create the root query
@@ -211,39 +227,57 @@
             schema_args['query'] = GraphQLObjectType(
                 name='PlaceholderQuery',
                 fields={'placeholder': placeholder}
             )
 
         schema = GraphQLSchema(**schema_args)
 
+        if self.root_type and issubclass(
+                self.root_type,
+                GraphQLRootTypeDelegate
+        ):
+            schema = self.root_type.validate_graphql_schema(schema)
+
         return schema, meta
 
     def execute(
         self,
         query,
         variables=None,
-        operation_name=None
+        operation_name=None,
+        root_value: Any = None,
+        middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
+        middleware_on_introspection: bool = False,
+        error_protection: bool = None
     ) -> ExecutionResult:
-        return self.executor().execute(
+        return self.executor(
+            root_value=root_value,
+            middleware=middleware,
+            middleware_on_introspection=middleware_on_introspection,
+            error_protection=error_protection
+        ).execute(
             query=query,
             variables=variables,
-            operation_name=operation_name
+            operation_name=operation_name,
         )
 
     def executor(
         self,
         root_value: Any = None,
         middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
-        middleware_on_introspection: bool = False
+        middleware_on_introspection: bool = False,
+        error_protection: bool = None
     ) -> GraphQLExecutor:
         schema, meta = self.graphql_schema()
 
         if callable(self.root_type) and root_value is None:
             root_value = self.root_type()
 
         return GraphQLExecutor(
             schema=schema,
             meta=meta,
             root_value=root_value,
             middleware=middleware,
-            middleware_on_introspection=middleware_on_introspection
+            middleware_on_introspection=middleware_on_introspection,
+            error_protection=error_protection if error_protection is not None
+            else self.error_protection
         )
```

### Comparing `graphql-api-1.2.9/graphql_api/context.py` & `graphql-api-1.3.0/graphql_api/context.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.2.9/graphql_api/dataclass_mapping.py` & `graphql-api-1.3.0/graphql_api/dataclass_mapping.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Type, get_type_hints
 import typing_inspect
+from docstring_parser import parse_from_object
 
 from graphql.type.definition import \
     GraphQLType, \
     GraphQLObjectType, \
     GraphQLField, \
     GraphQLInputField, \
     GraphQLNonNull
@@ -20,14 +21,15 @@
         return is_dataclass(_class)
 
 
 def type_from_dataclass(_class: Type, mapper) -> GraphQLType:
     dataclass_fields = dict(_class.__dataclass_fields__)
     dataclass_types = get_type_hints(_class)
     base_type: GraphQLObjectType = mapper.map(_class, use_graphql_type=False)
+    docstrings = parse_from_object(_class)
 
     # Remove any modifiers
     while hasattr(base_type, 'of_type'):
         base_type = base_type.of_type
 
     if mapper.as_input:
         return base_type
@@ -63,14 +65,20 @@
                         context=None,
                         *args,
                         **kwargs
                     ):
                         return getattr(self, local_prop_name)
                     return resolver
 
+                description = None
+
+                for docstring_param in docstrings.params:
+                    if docstring_param.arg_name == prop_name:
+                        description = docstring_param.description
+
                 type_: GraphQLType = local_mapper.map(type_=field_type)
 
                 nullable = False
 
                 if typing_inspect.is_union_type(field_type):
                     union_args = typing_inspect.get_args(
                         field_type,
@@ -79,17 +87,24 @@
                     if type(None) in union_args:
                         nullable = True
 
                 if not nullable:
                     type_: GraphQLType = GraphQLNonNull(type_)
 
                 if local_mapper.as_input:
-                    field = GraphQLInputField(type_=type_)
+                    field = GraphQLInputField(
+                        type_=type_,
+                        description=description
+                    )
                 else:
-                    field = GraphQLField(type_=type_, resolve=local_resolver())
+                    field = GraphQLField(
+                        type_=type_,
+                        resolve=local_resolver(),
+                        description=description
+                    )
 
                 local_fields[to_camel_case(prop_name)] = field
 
             if local_type_fields:
                 try:
                     fields_ = local_type_fields()
                     for name, field in fields_.items():
```

### Comparing `graphql-api-1.2.9/graphql_api/error.py` & `graphql-api-1.3.0/graphql_api/error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.2.9/graphql_api/executor.py` & `graphql-api-1.3.0/graphql_api/executor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,120 @@
 import inspect
 
 from typing import Any, List, Dict, Callable
 
-from graphql import graphql, graphql_sync
+from graphql import graphql, graphql_sync, ExecutionContext, GraphQLError, \
+    GraphQLOutputType
 
 from graphql.execution import ExecutionResult
 from graphql.type.schema import GraphQLSchema
 
 from graphql_api.context import GraphQLContext
 from graphql_api.middleware import \
     middleware_field_context, \
     middleware_request_context, \
     middleware_local_proxy, \
-    middleware_adapt_enum
+    middleware_adapt_enum, middleware_catch_exception
 
 
 class GraphQLBaseExecutor:
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.validate()
 
     def validate(self):
         pass
 
     def execute(
-        self,
-        query,
-        variables=None,
-        operation_name=None
+            self,
+            query,
+            variables=None,
+            operation_name=None
     ) -> ExecutionResult:
         pass
 
     async def execute_async(
-        self,
-        query,
-        variables=None,
-        operation_name=None
+            self,
+            query,
+            variables=None,
+            operation_name=None
     ) -> ExecutionResult:
         pass
 
 
+class ErrorProtectionExecutionContext(ExecutionContext):
+    default_error_protection = True
+
+    error_protection = "ERROR_PROTECTION"
+
+    def handle_field_error(
+            self,
+            error: GraphQLError,
+            return_type: GraphQLOutputType,
+    ) -> None:
+
+        error_protection = self.default_error_protection
+        original_error = error.original_error
+        if hasattr(error, self.error_protection):
+            error_protection = getattr(error, self.error_protection)
+
+        elif hasattr(original_error, self.error_protection):
+            error_protection = getattr(original_error, self.error_protection)
+
+        if not error_protection:
+            raise error.original_error
+
+        return super().handle_field_error(error=error, return_type=return_type)
+
+
+class NoErrorProtectionExecutionContext(ErrorProtectionExecutionContext):
+    default_error_protection = False
+
+
 class GraphQLExecutor(GraphQLBaseExecutor):
 
     def __init__(
-        self,
-        schema: GraphQLSchema,
-        meta: Dict = None,
-        root_value: Any = None,
-        middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
-        middleware_on_introspection: bool = False
+            self,
+            schema: GraphQLSchema,
+            meta: Dict = None,
+            root_value: Any = None,
+            middleware: List[Callable[[Callable, GraphQLContext], Any]] = None,
+            middleware_on_introspection: bool = False,
+            error_protection: bool = True
     ):
         super().__init__()
 
         if meta is None:
             meta = {}
 
         if middleware is None:
             middleware = []
 
+        middleware.insert(0, middleware_catch_exception)
         middleware.insert(0, middleware_field_context)
         middleware.insert(0, middleware_request_context)
         middleware.insert(0, middleware_local_proxy)
         middleware.insert(0, middleware_adapt_enum)
 
         self.meta = meta
         self.schema = schema
         self.middleware = middleware
         self.root_value = root_value
         self.middleware_on_introspection = middleware_on_introspection
+        self.execution_context_class = ErrorProtectionExecutionContext \
+            if error_protection else NoErrorProtectionExecutionContext
 
     def execute(
-        self,
-        query,
-        variables=None,
-        operation_name=None,
-        root_value=None,
-        context=None
+            self,
+            query,
+            variables=None,
+            operation_name=None,
+            root_value=None,
+            context=None
     ) -> ExecutionResult:
 
         context = GraphQLContext(
             schema=self.schema,
             meta=self.meta,
             executor=self
         )
@@ -91,25 +125,26 @@
         value = graphql_sync(
             self.schema,
             query,
             context_value=context,
             variable_values=variables,
             operation_name=operation_name,
             middleware=self.adapt_middleware(self.middleware),
-            root_value=root_value
+            root_value=root_value,
+            execution_context_class=self.execution_context_class
         )
         return value
 
     async def execute_async(
-        self,
-        query,
-        variables=None,
-        operation_name=None,
-        root_value=None,
-        context=None
+            self,
+            query,
+            variables=None,
+            operation_name=None,
+            root_value=None,
+            context=None
     ) -> ExecutionResult:
 
         context = GraphQLContext(
             schema=self.schema,
             meta=self.meta,
             executor=self
         )
@@ -120,22 +155,23 @@
         value = await graphql(
             self.schema,
             query,
             context_value=context,
             variable_values=variables,
             operation_name=operation_name,
             middleware=self.adapt_middleware(self.middleware),
-            root_value=root_value
+            root_value=root_value,
+            execution_context_class=self.execution_context_class
         )
         return value
 
     @staticmethod
     def adapt_middleware(
-        middleware,
-        middleware_on_introspection: bool = False
+            middleware,
+            middleware_on_introspection: bool = False
     ):
 
         def simplify(_middleware: Callable[[Callable, GraphQLContext], Any]):
             def graphql_middleware(next, root, info, **args):
                 kwargs = {}
                 if "context" in inspect.signature(_middleware).parameters:
                     context: GraphQLContext = info.context
```

### Comparing `graphql-api-1.2.9/graphql_api/mapper.py` & `graphql-api-1.3.0/graphql_api/mapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from graphql.pyutils import Undefined, UndefinedType
 
 from graphql_api.context import GraphQLContext
 from graphql_api.types import (
     GraphQLBytes,
     GraphQLUUID,
     GraphQLDateTime,
-    GraphQLJSON
+    GraphQLJSON, JsonType, GraphQLMappedEnumType
 )
 
 from graphql_api.utils import to_camel_case, to_snake_case, to_input_value
 from graphql_api.exception import GraphQLBaseException
 from graphql_api.dataclass_mapping import \
     type_is_dataclass, \
     type_from_dataclass
@@ -82,48 +82,49 @@
         pass
 
 
 class GraphQLMetaKey(enum.Enum):
     resolve_to_mutable = "RESOLVE_TO_MUTABLE"
     resolve_to_self = "RESOLVE_TO_SELF"
     native_middleware = "NATIVE_MIDDLEWARE"
+    error_protection = "ERROR_PROTECTION"
 
 
 class GraphQLMutableField(GraphQLField):
     pass
 
 
 class GraphQLTypeMapper:
 
     def __init__(
-        self,
-        as_mutable=False,
-        as_input=False,
-        registry=None,
-        reverse_registry=None,
-        suffix="",
-        schema=None
+            self,
+            as_mutable=False,
+            as_input=False,
+            registry=None,
+            reverse_registry=None,
+            suffix="",
+            schema=None
     ):
         self.as_mutable = as_mutable
         self.as_input = as_input
         self.registry = registry or {}
         self.reverse_registry = reverse_registry or {}
         self.suffix = suffix
         self.meta = {}
         self.input_type_mapper = None
         self.schema = schema
 
     def types(self) -> Set[GraphQLType]:
         return set(self.registry.values())
 
     def map_to_field(
-        self,
-        function_type: Callable,
-        name="",
-        key=""
+            self,
+            function_type: Callable,
+            name="",
+            key=""
     ) -> GraphQLField:
         type_hints = typing.get_type_hints(function_type)
         description = inspect.getdoc(function_type)
 
         return_type = type_hints.pop('return', None)
 
         if not return_type:
@@ -197,52 +198,45 @@
                 arg_type = GraphQLNonNull(arg_type)
 
             arguments[to_camel_case(key)] = GraphQLArgument(
                 type_=arg_type,
                 default_value=default_args.get(key, Undefined)
             )
 
-        def resolve(self, info=None, context=None, *args, **kwargs):
-            _args = {to_snake_case(key): arg for key, arg in kwargs.items()}
-
-            if enum_arguments:
-                enum_keys = list(enum_arguments.keys())
-                _args = {
-                    key: enum_arguments[key](arg)
-                    if key in enum_keys else arg
-                    for key, arg in _args.items()
-                }
+        # noinspection PyUnusedLocal
+        def resolve(_self, info=None, context=None, *args, **kwargs):
+            _args = {to_snake_case(_key): arg for _key, arg in kwargs.items()}
 
             if include_context:
                 _args['context'] = info.context
 
             function_name = function_type.__name__
-            parent_type = self.__class__
+            parent_type = _self.__class__
             class_attribute = getattr(parent_type, function_name, None)
             is_property = isinstance(class_attribute, property)
             response = None
 
             if is_property:
                 if _args:
                     if len(_args) > 1:
                         raise KeyError(
                             f"{function_name} on type {parent_type} is a"
                             f" property, and cannot have multiple arguments."
                         )
                     else:
-                        response = function_type(self, **_args)
+                        response = function_type(_self, **_args)
                 else:
-                    response = getattr(self, function_name, None)
+                    response = getattr(_self, function_name, None)
             else:
-                function_type_override = getattr(self, function_name, None)
+                function_type_override = getattr(_self, function_name, None)
 
                 if function_type_override is not None:
                     response = function_type_override(**_args)
                 else:
-                    response = function_type(self, **_args)
+                    response = function_type(_self, **_args)
 
             if enum_return:
                 if isinstance(response, enum.Enum):
                     response = response.value
 
             return response
 
@@ -266,25 +260,27 @@
             for arg in union_args if arg and arg != none_type
         }
 
         if len(union_map) == 1:
             _, mapped_type = union_map.popitem()
             return mapped_type
 
+        # noinspection PyUnusedLocal
         def resolve_type(value, info, _type):
             from graphql_api.remote import GraphQLRemoteObject
 
             value_type = type(value)
 
             if isinstance(value, GraphQLRemoteObject):
                 value_type = value.python_type
 
-            for arg, mapped_type in union_map.items():
-                if issubclass(value_type, arg):
-                    return mapped_type.name
+            for arg, _mapped_type in union_map.items():
+                if issubclass(value_type, arg) \
+                        and hasattr(_mapped_type, 'name'):
+                    return _mapped_type.name
 
         names = [arg.__name__ for arg in union_args]
         name = f"{''.join(names)}{self.suffix}Union"
 
         return GraphQLUnionType(
             name,
             types=[*union_map.values()],
@@ -294,35 +290,45 @@
     def map_to_list(self, type_: List) -> GraphQLList:
         list_subtype = typing_inspect.get_args(type_)[0]
 
         list_type = GraphQLList(type_=self.map(list_subtype))
 
         return list_type
 
+    def map_to_literal(self, type__) -> GraphQLType:
+        literal_args = typing_inspect.get_args(type__, evaluate=True)
+        _type = type(literal_args[0])
+        if not all(isinstance(x, _type) for x in literal_args):
+            raise TypeError("Literals must all be of the same type")
+
+        return self.map(_type)
+
+    # noinspection PyMethodMayBeStatic
     def map_to_enum(self, type_: Type[enum.Enum]) -> GraphQLEnumType:
         enum_type = type_
         name = f"{type_.__name__}Enum"
-        # Enums dont include a suffix as they are immutable
+        # Enums don't include a suffix as they are immutable
 
         description = inspect.getdoc(enum_type)
 
-        enum_type = GraphQLEnumType(
+        enum_type = GraphQLMappedEnumType(
             name=name,
             values=enum_type,
             description=description
         )
 
         enum_type.enum_type = type_
 
-        def serialize(self, value) -> Union[str, None, UndefinedType]:
+        def serialize(_self, value) -> Union[str, None, UndefinedType]:
             if value and isinstance(value, collections.abc.Hashable):
                 if isinstance(value, enum.Enum):
                     value = value.value
 
-                lookup_value = self._value_lookup.get(value)
+                # noinspection PyProtectedMember
+                lookup_value = _self._value_lookup.get(value)
                 if lookup_value:
                     return lookup_value
                 else:
                     return Undefined
 
             return None
 
@@ -367,16 +373,19 @@
 
         interface_name = f"{name}{self.suffix}Interface"
         description = inspect.getdoc(class_type)
 
         def local_resolve_type():
             local_self = self
 
+            # noinspection PyUnusedLocal
             def resolve_type(value, info, _type):
-                return local_self.map(type(value)).name
+                value = local_self.map(type(value))
+                if hasattr(value, 'name'):
+                    return value.name
             return resolve_type
 
         def local_fields():
             local_self = self
             local_class_funcs = class_funcs
             local_class_type = class_type
             local_name = name
@@ -407,14 +416,15 @@
 
         if hasattr(class_type, 'graphql_from_input'):
             creator = class_type.graphql_from_input
             func = creator
 
         else:
             creator = class_type
+            # noinspection PyTypeChecker
             func = class_type.__init__
 
         description = inspect.getdoc(func) or inspect.getdoc(class_type)
 
         try:
             type_hints = typing.get_type_hints(func)
         except Exception as err:
@@ -445,24 +455,25 @@
 
                 for key, hint in local_type_hints.items():
 
                     input_arg_type = local_self.map(hint)
 
                     nullable = key in local_default_args
                     if not nullable:
+                        # noinspection PyTypeChecker
                         input_arg_type = GraphQLNonNull(input_arg_type)
 
                     default_value = local_default_args.get(key, None)
 
                     if default_value is not None:
                         try:
                             default_value = to_input_value(default_value)
-                        except ValueError as err:
+                        except ValueError as _err:
                             raise ValueError(
-                                f"Unable to map {local_name}.{key}, {err}."
+                                f"Unable to map {local_name}.{key}, {_err}."
                             )
 
                     arguments[to_camel_case(key)] = GraphQLInputField(
                         type_=input_arg_type,
                         default_value=default_value
                     )
                 return arguments
@@ -506,15 +517,18 @@
 
             def interfaces():
                 _interfaces = []
                 superclasses = inspect.getmro(local_class_type)[1:]
 
                 for superclass in superclasses:
                     if is_interface(superclass, local_self.schema):
-                        _interfaces.append(local_self.map(superclass))
+                        value = local_self.map(superclass)
+                        if isinstance(value, GraphQLInterfaceType):
+                            interface: GraphQLInterfaceType = value
+                            _interfaces.append(interface)
 
                 return _interfaces
 
             return interfaces
 
         def local_fields():
             local_self = self
@@ -553,24 +567,30 @@
 
         return self.reverse_registry.get(graphql_type)
 
     def map(self, type_, use_graphql_type=True) -> GraphQLType:
 
         def _map(type__) -> GraphQLType:
 
+            if type_ == JsonType:
+                return GraphQLJSON
+
             if use_graphql_type and inspect.isclass(type__):
                 if issubclass(type__, GraphQLTypeWrapper):
                     return type__.graphql_type(mapper=self)
 
                 if type_is_dataclass(type__):
                     return type_from_dataclass(type__, mapper=self)
 
             if typing_inspect.is_union_type(type__):
                 return self.map_to_union(type__)
 
+            if typing_inspect.is_literal_type(type__):
+                return self.map_to_literal(type__)
+
             origin_type = get_origin(type__)
 
             if inspect.isclass(origin_type) and \
                     issubclass(get_origin(type__), (List, Set)):
                 return self.map_to_list(type__)
 
             if inspect.isclass(type__):
@@ -631,42 +651,47 @@
         if isinstance(type_, GraphQLNonNull):
             type_ = type_.of_type
 
         if self.as_input and not is_input_type(type_):
             return False
 
         if isinstance(type_, GraphQLObjectType):
+            # noinspection PyProtectedMember
             if evaluate:
                 try:
                     if len(type_.fields) == 0:
                         return False
                 except AssertionError:
                     return False
 
             elif not callable(type_._fields) and len(type_._fields) == 0:
                 return False
 
         return True
 
 
 def get_class_funcs(
-    class_type,
-    schema,
-    mutable=False
+        class_type,
+        schema,
+        mutable=False
 ) -> List[Tuple[Any, Any]]:
-    members = [(key, member) for key, member in inspect.getmembers(class_type)]
+    members = []
+    for _class_type in class_type.mro():
+        for key, member in inspect.getmembers(_class_type):
+            if not (key.startswith("__") and key.endswith("__")):
+                members.append((key, member))
 
     if hasattr(class_type, 'graphql_fields'):
         members += [
             (func.__name__, func)
             for func in class_type.graphql_fields()
         ]
     func_members = []
 
-    for key, member in members:
+    for key, member in reversed(members):
         if isinstance(member, property):
             getter = member.fget
             if getter:
                 func_members.append((key, getter))
             setter = member.fset
 
             if setter:
@@ -676,15 +701,27 @@
 
     def matches_criterion(func):
         func_type = get_value(func, schema, 'type')
         return func_type == "query" or (mutable and func_type == "mutation")
 
     callable_funcs = []
 
+    inherited_fields = {}
     for key, member in func_members:
+        if getattr(member, 'graphql', None) and key != "test_property":
+            inherited_fields[key] = {**member.__dict__}
+        elif key in inherited_fields:
+            member.__dict__ = {
+                **inherited_fields[key],
+                'defined_on': member
+            }
+
+    done = []
+
+    for key, member in reversed(func_members):
         if is_graphql(member, schema=schema) and matches_criterion(member):
             if not callable(member):
                 type_hints = typing.get_type_hints(member)
                 return_type = type_hints.pop('return', None)
 
                 def local_func():
                     local_key = key
@@ -707,28 +744,29 @@
                     return func
 
                 func = local_func()
 
             else:
                 func = member
 
-            callable_funcs.append((key, func))
+            if key not in done:
+                done.append(key)
+                callable_funcs.append((key, func))
 
     return callable_funcs
 
 
 def get_value(type_, schema, key):
     if is_graphql(type_, schema):
         return type_.schemas.get(schema, type_.schemas.get(None)).get(key)
 
 
 def is_graphql(type_, schema):
     graphql = getattr(type_, 'graphql', None)
     schemas = getattr(type_, 'schemas', {})
-
     valid_schema = schema in schemas.keys() or None in schemas.keys()
 
     return graphql and schemas and valid_schema
 
 
 def is_interface(type_, schema):
     if is_graphql(type_, schema):
```

### Comparing `graphql-api-1.2.9/graphql_api/middleware.py` & `graphql-api-1.3.0/graphql_api/middleware.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,54 @@
 import enum
+import sys
+import traceback
 
-from graphql import GraphQLObjectType, GraphQLNonNull
+from graphql import GraphQLObjectType, GraphQLNonNull, GraphQLResolveInfo
+
+from graphql_api.mapper import GraphQLMetaKey
 
 from graphql_api.context import GraphQLContext
 from graphql_api.utils import to_snake_case
 
 
+def middleware_catch_exception(next, context: GraphQLContext):
+    try:
+        value = next()
+    except Exception as err:
+        from graphql_api.executor import ErrorProtectionExecutionContext
+        info: GraphQLResolveInfo = context.resolve_args.get("info")
+
+        field_meta = context.field.meta
+        if field_meta.get(GraphQLMetaKey.error_protection) is not None:
+            setattr(
+                err,
+                ErrorProtectionExecutionContext.error_protection,
+                field_meta.get(GraphQLMetaKey.error_protection)
+            )
+
+        return_type = info.return_type
+        ignored = isinstance(return_type, GraphQLNonNull)
+
+        print(
+            f"GraphQLField '{info.field_name}' on '{info.parent_type.name}' "
+            f"resolver {'(ignored) ' if ignored else ''}Exception: {err} ",
+            file=sys.stderr
+        )
+        traceback.print_exc()
+        raise err
+
+    return value
+
+
 def middleware_local_proxy(next):
     value = next()
 
     # Compatibility with LocalProxy from Werkzeug
-    try:
-        if hasattr(value, '_get_current_object'):
-            value = value._get_current_object()
-
-    except Exception:
-        pass
+    if hasattr(value, '_get_current_object'):
+        value = value._get_current_object()
 
     if isinstance(value, Exception):
         raise value
 
     return value
```

### Comparing `graphql-api-1.2.9/graphql_api/reduce.py` & `graphql-api-1.3.0/graphql_api/reduce.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.2.9/graphql_api/relay.py` & `graphql-api-1.3.0/graphql_api/relay.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 @GraphQLAPI.type(interface=True)
 class Node:
     """
     The `Node` Interface type represents a Relay Node.
     `https://facebook.github.io/relay/graphql/objectidentification.htm`
     """
 
+    # noinspection PyShadowingBuiltins
     def __init__(self, id: UUID = None, *args, **kwargs):
         if id is None:
             id = uuid4()
 
         self.id = id
         super().__init__(*args, **kwargs)
```

### Comparing `graphql-api-1.2.9/graphql_api/remote.py` & `graphql-api-1.3.0/graphql_api/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,33 +31,34 @@
     is_enum_type
 )
 
 from graphql_api.error import GraphQLError
 from graphql_api.executor import GraphQLBaseExecutor
 from graphql_api.mapper import GraphQLTypeMapper, GraphQLMetaKey
 from graphql_api.api import GraphQLAPI
+from graphql_api.types import serialize_bytes
 from graphql_api.utils import \
     to_camel_case, \
     url_to_ast, \
     to_snake_case, \
     http_query
 
 
 class GraphQLRemoteExecutor(GraphQLBaseExecutor, GraphQLObjectType):
 
     def __init__(
-        self,
-        url,
-        name="Remote",
-        description=None,
-        http_method="GET",
-        http_headers=None,
-        http_timeout=None,
-        verify=True,
-        ignore_unsupported=True
+            self,
+            url,
+            name="Remote",
+            description=None,
+            http_method="GET",
+            http_headers=None,
+            http_timeout=None,
+            verify=True,
+            ignore_unsupported=True
     ):
 
         if not description:
             description = f'The `{name}` object type forwards all ' \
                           f'requests to the GraphQL executor at {url}'
 
         if http_headers is None:
@@ -135,19 +136,19 @@
                     f"a remote executor '{self.url}'."
                 )
 
         # noinspection PyProtectedMember
         return ast_schema.query_type.fields
 
     async def execute_async(
-        self,
-        query,
-        variable_values=None,
-        operation_name=None,
-        http_headers=None
+            self,
+            query,
+            variable_values=None,
+            operation_name=None,
+            http_headers=None
     ) -> ExecutionResult:
 
         if http_headers is None:
             http_headers = self.http_headers
         else:
             http_headers = {**self.http_headers, **http_headers}
 
@@ -174,19 +175,19 @@
 
         return ExecutionResult(
             data=json_.get('data'),
             errors=json_.get('errors')
         )
 
     def execute(
-        self,
-        query,
-        variable_values=None,
-        operation_name=None,
-        http_headers=None
+            self,
+            query,
+            variable_values=None,
+            operation_name=None,
+            http_headers=None
     ) -> ExecutionResult:
 
         if http_headers is None:
             http_headers = self.http_headers
         else:
             http_headers = {**self.http_headers, **http_headers}
 
@@ -216,39 +217,31 @@
             errors=json_.get('errors')
         )
 
 
 class GraphQLMappers:
 
     def __init__(
-        self,
-        query_mapper: GraphQLTypeMapper,
-        mutable_mapper: GraphQLTypeMapper
+            self,
+            query_mapper: GraphQLTypeMapper,
+            mutable_mapper: GraphQLTypeMapper
     ):
         self.query_mapper = query_mapper
         self.mutable_mapper = mutable_mapper
 
     def map(self, type, reverse=False):
-        query_type = None
-        try:
-            if reverse:
-                query_type = self.query_mapper.rmap(type)
-            else:
-                query_type = self.query_mapper.map(type)
-        except Exception:
-            pass
+        if reverse:
+            query_type = self.query_mapper.rmap(type)
+        else:
+            query_type = self.query_mapper.map(type)
 
-        mutable_type = None
-        try:
-            if reverse:
-                mutable_type = self.mutable_mapper.rmap(type)
-            else:
-                mutable_type = self.mutable_mapper.map(type)
-        except Exception:
-            pass
+        if reverse:
+            mutable_type = self.mutable_mapper.rmap(type)
+        else:
+            mutable_type = self.mutable_mapper.map(type)
 
         if reverse:
             return query_type or mutable_type
 
         return query_type, mutable_type
 
 
@@ -273,32 +266,32 @@
 class GraphQLRemoteObject:
 
     def get_labels(self) -> List[str]:
         return self.python_type.get_labels()
 
     @classmethod
     def from_url(
-        cls,
-        url: str,
-        api: GraphQLAPI,
-        http_method: str = "GET"
+            cls,
+            url: str,
+            api: GraphQLAPI,
+            http_method: str = "GET"
     ) -> 'GraphQLRemoteObject':
         executor = GraphQLRemoteExecutor(url=url, http_method=http_method)
 
         return GraphQLRemoteObject(executor=executor, api=api)
 
     # noinspection PyProtectedMember
     def __init__(
-        self,
-        executor: GraphQLBaseExecutor,
-        api: GraphQLAPI = None,
-        mappers: GraphQLMappers = None,
-        python_type: Type = None,
-        call_history: List[Tuple['GraphQLRemoteField', Dict]] = None,
-        delay_mapping: bool = True
+            self,
+            executor: GraphQLBaseExecutor,
+            api: GraphQLAPI = None,
+            mappers: GraphQLMappers = None,
+            python_type: Type = None,
+            call_history: List[Tuple['GraphQLRemoteField', Dict]] = None,
+            delay_mapping: bool = True
     ):
         if not call_history:
             call_history = []
 
         if not api and python_type:
             api = GraphQLAPI(root=python_type)
 
@@ -347,16 +340,16 @@
             field_value = field_values.get(to_camel_case(field.name))
 
             arg_hash = self.hash(args)
 
             self.values[(field, arg_hash)] = field_value
 
     async def fetch_async(
-        self,
-        fields: List[Tuple['GraphQLRemoteField', Dict]] = None
+            self,
+            fields: List[Tuple['GraphQLRemoteField', Dict]] = None
     ):
         if fields is None:
             fields = self._fields()
 
         field_values = await self._fetch_async(fields=fields)
 
         for field, args in fields:
@@ -398,16 +391,16 @@
         query = self._fetch_build_query(fields=fields)
 
         result = self.executor.execute(query=query)
 
         return self._fetch_process(query, result, fields)
 
     async def _fetch_async(
-        self,
-        fields: List[Tuple['GraphQLRemoteField', Dict]] = None
+            self,
+            fields: List[Tuple['GraphQLRemoteField', Dict]] = None
     ):
         """
         Load all the scalar values for this object into the values dictionary
         :return:
         """
         if fields is None:
             fields = self._fields()
@@ -415,16 +408,16 @@
         query = self._fetch_build_query(fields=fields)
 
         result = await self.executor.execute_async(query=query)
 
         return self._fetch_process(query, result, fields)
 
     def _fetch_build_query(
-        self,
-        fields: List[Tuple['GraphQLRemoteField', Dict]]
+            self,
+            fields: List[Tuple['GraphQLRemoteField', Dict]]
     ):
         self._map()
 
         mutable = any([
             field.mutable
             for field, args in self.call_history + fields])
 
@@ -434,25 +427,25 @@
             mappers=self.mappers,
             mutable=mutable
         )
 
         return query_builder.build()
 
     def _fetch_process(
-        self,
-        query,
-        result: ExecutionResult,
-        fields: List[Tuple['GraphQLRemoteField', Dict]]
+            self,
+            query,
+            result: ExecutionResult,
+            fields: List[Tuple['GraphQLRemoteField', Dict]]
     ):
 
         if result.errors:
             raise GraphQLRemoteError(
                 query=query,
                 result=result,
-                message=result.errors[0]['message']
+                message=result.errors[0]["message"]
             )
 
         field_values = result.data
         for field, args in self.call_history:
             camel_name = to_camel_case(field.name)
 
             if isinstance(field_values, list):
@@ -493,29 +486,34 @@
                 return None
 
             if not is_scalar(field_type):
                 raise TypeError(
                     f"Unable to parse non-scalar type {field_type}"
                 )
 
-            ast_value = to_ast_value(value, field_type)
+            def _to_value(value):
+                ast_value = to_ast_value(value, field_type)
 
-            if hasattr(field_type, 'parse_literal'):
-                value = field_type.parse_literal(ast_value)
+                if hasattr(field_type, 'parse_literal'):
+                    value = field_type.parse_literal(ast_value)
 
-                if is_enum_type(field_type) and \
-                        hasattr(field_type, 'enum_type'):
-                    enum_type = field_type.enum_type
-                    value = enum_type(value)
+                    if is_enum_type(field_type) and \
+                            hasattr(field_type, 'enum_type'):
+                        enum_type = field_type.enum_type
+                        value = enum_type(value)
 
-                return value
+                    return value
 
-            raise TypeError(
-                f"Scalar type {field_type} missing 'parse_literal' attribute"
-            )
+            if field.list:
+                values = []
+                for _value in value:
+                    values.append(_to_value(value))
+                return value
+            else:
+                return _to_value(value)
 
         if isinstance(field_values, list):
             field_values = [
                 {
                     key: parse_field(key, value)
                     for key, value in field_values_list_item.items()
                 }
@@ -763,14 +761,15 @@
         self._map()
 
         attribute_type = getattr(self.python_type, name, None)
 
         is_dataclass_field = False
 
         try:
+            # noinspection PyUnresolvedReferences
             from dataclasses import fields, is_dataclass
 
             if is_dataclass(self.python_type):
                 # noinspection PyDataclass
                 field_names = [
                     field.name
                     for field in fields(self.python_type)
@@ -784,14 +783,15 @@
         is_property = isinstance(attribute_type, property)
         is_callable = callable(attribute_type)
 
         auto_call = is_dataclass_field or is_property
 
         if not auto_call:
             try:
+                # noinspection PyPackageRequirements
                 from sqlalchemy.orm.attributes import InstrumentedAttribute
                 auto_call = isinstance(attribute_type, InstrumentedAttribute)
             except ImportError:
                 pass
 
         try:
             field = self.get_field(name)
@@ -831,19 +831,19 @@
                f"at {hex(id(self))}>"
 
 
 class GraphQLRemoteField:
 
     # noinspection PyProtectedMember
     def __init__(
-        self,
-        name: str,
-        mutable: bool,
-        graphql_field: GraphQLField,
-        parent: GraphQLRemoteObject
+            self,
+            name: str,
+            mutable: bool,
+            graphql_field: GraphQLField,
+            parent: GraphQLRemoteObject
     ):
         self.name = name
         self.mutable = mutable
         self.graphql_field = graphql_field
         self.parent = parent
         self.nullable = is_nullable(self.graphql_field.type)
         self.scalar = is_scalar(self.graphql_field.type)
@@ -895,19 +895,19 @@
             if other.parent == self.parent and other.name == self.name:
                 return True
 
 
 class GraphQLRemoteQueryBuilder:
 
     def __init__(
-        self,
-        call_stack: List[Tuple['GraphQLRemoteField', Dict]],
-        fields: List[Tuple['GraphQLRemoteField', Dict]],
-        mappers: GraphQLMappers,
-        mutable=False
+            self,
+            call_stack: List[Tuple['GraphQLRemoteField', Dict]],
+            fields: List[Tuple['GraphQLRemoteField', Dict]],
+            mappers: GraphQLMappers,
+            mutable=False
     ):
         self.call_stack = call_stack
         self.fields = fields
         self.mappers = mappers
         self.mutable = mutable
 
     def build(self):
@@ -949,18 +949,18 @@
         query += "{" + ",".join(field_calls) + "}"
         query += "}" * len(self.call_stack)
 
         return query
 
     # noinspection PyMethodMayBeStatic
     def map_to_input_value(
-        self,
-        value,
-        mappers: GraphQLMappers,
-        expected_graphql_type=None
+            self,
+            value,
+            mappers: GraphQLMappers,
+            expected_graphql_type=None
     ):
         from graphql_api.mapper import is_scalar
 
         if value is None:
             return None
 
         python_type = type(value)
@@ -979,14 +979,16 @@
 
             if isinstance(value, str):
                 return json.dumps(value)
             if isinstance(value, bool):
                 return 'true' if value else 'false'
             if isinstance(value, (float, int)):
                 return str(value)
+            if isinstance(value, bytes):
+                return '"' + serialize_bytes(value) + '"'
             else:
                 return '"' + str(value) + '"'
 
         if isinstance(value, enum.Enum):
             return str(value.value)
 
         if isinstance(value, object):
```

### Comparing `graphql-api-1.2.9/graphql_api/types.py` & `graphql-api-1.3.0/graphql_api/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,33 @@
+import binascii
 import datetime
 import json
 import uuid
+from typing import Dict, Union, List
 
-from typing import Dict
-
-from graphql import GraphQLScalarType, StringValueNode
+from graphql import GraphQLScalarType, StringValueNode, Undefined, \
+    GraphQLEnumType
 from graphql.language import ast
 
 
+class GraphQLMappedEnumType(GraphQLEnumType):
+
+    def parse_literal(self, *args, **kwargs):
+        result = super().parse_literal(*args, **kwargs)
+
+        return self.enum_type(result) \
+            if hasattr(self, 'enum_type') else result
+
+
 def parse_uuid_literal(ast):
     if isinstance(ast, StringValueNode):
         try:
             return uuid.UUID(ast.value)
         except ValueError:
-            pass
+            return Undefined
 
 
 GraphQLUUID = GraphQLScalarType(
     name='UUID',
     description='The `UUID` scalar type represents a unique identifer.',
     serialize=str,
     parse_value=str,
@@ -54,51 +64,65 @@
     description='The `DateTime` scalar type represents a datetime, '
                 'the datetime should be in the format `2018-01-22 17:46:32`',
     serialize=serialize_datetime,
     parse_value=parse_datetime_value,
     parse_literal=parse_datetime_literal)
 
 
-def serialize_json(data: Dict) -> str:
+JsonType = Union[None, int, float, str, bool, List, Dict]
+
+
+def serialize_json(data: JsonType) -> str:
     return json.dumps(data)
 
 
-def parse_json_value(value: str) -> Dict:
+def parse_json_value(value: str) -> JsonType:
     return json.loads(value)
 
 
-def parse_json_literal(node) -> Dict:
+def parse_json_literal(node) -> JsonType:
     if isinstance(node, ast.StringValueNode):
         return parse_json_value(node.value)
+    if isinstance(node, ast.BooleanValueNode):
+        return node.value
+    if isinstance(node, ast.FloatValueNode):
+        return node.value
 
 
 GraphQLJSON = GraphQLScalarType(
     name='JSON',
     description='The `JSON` scalar type represents JSON values as specified by'
                 ' [ECMA-404](http://www.ecma-international.org/'
                 'publications/files/ECMA-ST/ECMA-404.pdf).',
     serialize=serialize_json,
     parse_value=parse_json_value,
     parse_literal=parse_json_literal)
 
 
 def serialize_bytes(bytes: bytes) -> str:
-    return bytes.decode("utf-8")
+    try:
+        data = bytes.decode('utf-8')
+    except (binascii.Error, UnicodeDecodeError, Exception):
+        data = "UTF-8 ENCODED PREVIEW: " + \
+               bytes.decode('utf-8', errors="ignore")
+    return data
 
 
 def parse_bytes_value(value: str) -> bytes:
-    return value.encode("utf-8")
+    data = bytes(value, 'utf-8')
+    return data
 
 
 def parse_bytes_literal(node):
     if isinstance(node, ast.StringValueNode):
         return parse_bytes_value(node.value)
 
 
 GraphQLBytes = GraphQLScalarType(
     name='Bytes',
-    description='The `Bytes` scalar type represents a '
-                'Byte array datatype in UTF-8 string format.',
+    description='The `Bytes` scalar type expects and returns a '
+                'Byte array in UTF-8 string format that represents the Bytes. '
+                'If the data is not UTF-encodable the erros will be ignored',
     serialize=serialize_bytes,
     parse_value=parse_bytes_value,
     parse_literal=parse_bytes_literal
 )
```

### Comparing `graphql-api-1.2.9/graphql_api/utils.py` & `graphql-api-1.3.0/graphql_api/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,14 +193,14 @@
                 timeout=ClientTimeout(total=http_timeout)
             )
 
         else:
             raise AttributeError(f"Invalid HTTP method {http_method}")
 
         try:
-            json = await r.json()
+            json = await r.json(content_type=None)
         except JSONDecodeError as e:
             raise ValueError(
                 f"{e}, unable to decode JSON"
             )
 
     return json
```

### Comparing `graphql-api-1.2.9/graphql_api.egg-info/PKG-INFO` & `graphql-api-1.3.0/graphql_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.2.9
+Version: 1.3.0
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.2.9/graphql-api-v1.2.9.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.0/graphql-api-v1.3.0.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.2.9/setup.py` & `graphql-api-1.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,31 +15,33 @@
     version=version,
     license='MIT',
     packages=find_packages(),
     include_package_data=True,
     author='Robert Parker',
     author_email='rob@parob.com',
     url='https://gitlab.com/parob/graphql-api',
-    download_url=f'https://gitlab.com/parob/graphql/-/archive/v{version}/graphql-api-v{version}.tar.gz',
+    download_url=f'https://gitlab.com/parob/graphql/-/archive/v{version}'
+                 f'/graphql-api-v{version}.tar.gz',
     keywords=['GraphQL', 'GraphQL-API', 'GraphQLAPI', 'Server'],
     description='A framework for building Python GraphQL APIs.',
     long_description=readme,
     long_description_content_type='text/markdown',
     install_requires=[
-        'graphql-core>=3.1.2',
-        'requests>=2.24.0',
-        'typing-inspect>=0.6.0',
-        'aiohttp>=3.8.0'
+        'graphql-core~=3.1',
+        'requests~=2.24',
+        'typing-inspect~=0.6',
+        'aiohttp~=3.8',
+        'docstring-parser~=0.15'
     ],
     extras_require={
         'dev': [
-            'pytest>=5.4.3',
-            'pytest-cov>=2.10.0',
-            'coverage>=5.2',
-            'faker>=4.1.1'
+            'pytest~=5.4',
+            'pytest-cov~=2.10',
+            'coverage~=5.2',
+            'faker~=4.1'
         ]
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

