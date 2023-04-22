# Comparing `tmp/dbterd-1.1.0b1.tar.gz` & `tmp/dbterd-1.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbterd-1.1.0b1.tar", max compression
+gzip compressed data, was "dbterd-1.1.0b2.tar", max compression
```

## Comparing `dbterd-1.1.0b1.tar` & `dbterd-1.1.0b2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     1067 2023-04-16 06:29:54.505994 dbterd-1.1.0b1/LICENSE
--rw-r--r--   0        0        0     4504 2023-04-16 06:29:54.505994 dbterd-1.1.0b1/README.md
--rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/__init__.py
--rw-r--r--   0        0        0       37 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/__main__.py
--rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/algos/__init__.py
--rw-r--r--   0        0        0      648 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/algos/meta.py
--rw-r--r--   0        0        0     5833 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/algos/test_relationship.py
--rw-r--r--   0        0        0     1997 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/base.py
--rw-r--r--   0        0        0      344 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/factory.py
--rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/__init__.py
--rw-r--r--   0        0        0      132 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/constants.py
--rw-r--r--   0        0        0      304 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/dbml/__init__.py
--rw-r--r--   0        0        0      978 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/dbml/dbml_test_relationship.py
--rw-r--r--   0        0        0       49 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/default.py
--rw-r--r--   0        0        0      316 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/mermaid/__init__.py
--rw-r--r--   0        0        0     1190 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
--rw-r--r--   0        0        0      198 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/adapters/worker.py
--rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/cli/__init__.py
--rw-r--r--   0        0        0     1732 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/cli/main.py
--rw-r--r--   0        0        0     2200 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/cli/params.py
--rw-r--r--   0        0        0      284 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/default.py
--rw-r--r--   0        0        0        0 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/__init__.py
--rw-r--r--   0        0        0      721 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/cli_messaging.py
--rw-r--r--   0        0        0      877 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/dict.py
--rw-r--r--   0        0        0     4076 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/file.py
--rw-r--r--   0        0        0     1022 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/jsonify.py
--rw-r--r--   0        0        0      976 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/log.py
--rw-r--r--   0        0        0     1605 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/helpers/yaml.py
--rw-r--r--   0        0        0       94 2023-04-16 06:29:54.509994 dbterd-1.1.0b1/dbterd/main.py
--rw-r--r--   0        0        0     2133 2023-04-16 06:30:10.730031 dbterd-1.1.0b1/pyproject.toml
--rw-r--r--   0        0        0     5594 1970-01-01 00:00:00.000000 dbterd-1.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-22 06:27:30.683149 dbterd-1.1.0b2/LICENSE
+-rw-r--r--   0        0        0     4504 2023-04-22 06:27:30.683149 dbterd-1.1.0b2/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/__init__.py
+-rw-r--r--   0        0        0     4465 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/base.py
+-rw-r--r--   0        0        0     3157 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/filter.py
+-rw-r--r--   0        0        0      545 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/meta.py
+-rw-r--r--   0        0        0     2505 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/algos/test_relationship.py
+-rw-r--r--   0        0        0     2561 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/base.py
+-rw-r--r--   0        0        0      560 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/factory.py
+-rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/constants.py
+-rw-r--r--   0        0        0      304 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/dbml/__init__.py
+-rw-r--r--   0        0        0     1373 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/dbml/dbml_test_relationship.py
+-rw-r--r--   0        0        0      168 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/default.py
+-rw-r--r--   0        0        0      316 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/mermaid/__init__.py
+-rw-r--r--   0        0        0     1597 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py
+-rw-r--r--   0        0        0      222 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/adapters/worker.py
+-rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/cli/__init__.py
+-rw-r--r--   0        0        0     2026 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/cli/main.py
+-rw-r--r--   0        0        0     1928 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/cli/params.py
+-rw-r--r--   0        0        0      284 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/default.py
+-rw-r--r--   0        0        0        0 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/__init__.py
+-rw-r--r--   0        0        0      721 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/cli_messaging.py
+-rw-r--r--   0        0        0      877 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/dict.py
+-rw-r--r--   0        0        0     4494 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/file.py
+-rw-r--r--   0        0        0     1022 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/jsonify.py
+-rw-r--r--   0        0        0      976 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/log.py
+-rw-r--r--   0        0        0     1605 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/helpers/yaml.py
+-rw-r--r--   0        0        0       94 2023-04-22 06:27:30.691150 dbterd-1.1.0b2/dbterd/main.py
+-rw-r--r--   0        0        0     2113 2023-04-22 06:27:48.171863 dbterd-1.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     5553 1970-01-01 00:00:00.000000 dbterd-1.1.0b2/PKG-INFO
```

### Comparing `dbterd-1.1.0b1/LICENSE` & `dbterd-1.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b1/README.md` & `dbterd-1.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b1/dbterd/adapters/algos/meta.py` & `dbterd-1.1.0b2/dbterd/adapters/algos/meta.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 from dataclasses import dataclass
 from typing import List, Optional, Tuple
 
 
 @dataclass
 class Column:
-    """
-    Sample DBML: id varchar [primary key]
-    """
+    """Parsed Column object"""
 
     name: str = "unknown"
     data_type: str = "unknown"
 
 
 @dataclass
 class Table:
-    """
-    Sample DBML:
-    Table posts {
-        id varchar [primary key]
-    }
-    """
+    """Parsed Table object"""
 
     name: str
     database: str
     schema: str
     columns: Optional[List[Column]] = None
     raw_sql: Optional[str] = None
     resource_type: str = "model"
 
 
 @dataclass
 class Ref:
-    """Sample DBML: Ref: posts.user_id > users.id"""
+    """Parsed Relationship object"""
 
     name: str
     table_map: Tuple[str, str]
     column_map: Tuple[str, str]
```

### Comparing `dbterd-1.1.0b1/dbterd/adapters/algos/test_relationship.py` & `dbterd-1.1.0b2/dbterd/adapters/algos/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,170 +1,142 @@
-from dbterd.adapters.algos.meta import Column, Ref, Table
+import copy
 
-
-def parse(manifest, catalog, **kwargs):
-    # Parse Table
-    tables = get_tables(manifest, catalog)
-    # Apply selection
-    select_rule = (kwargs.get("select") or "").lower().split(":")
-    resource_types = kwargs.get("resource_type") or ""
-
-    def filter_table_select(table):
-        if select_rule[0].startswith("schema"):
-            schema = f"{table.database}.{table.schema}"
-            return schema.startswith(select_rule[-1]) or table.schema.startswith(
-                select_rule[-1]
-            )
-        else:
-            return table.name.startswith(select_rule[-1])
-
-    tables = [table for table in tables if filter_table_select(table)]
-    tables = [table for table in tables if table.resource_type in resource_types]
-
-    # -- apply exclusion (take care of name only)
-
-    exclude_rule = kwargs.get("exclude")
-    if exclude_rule:
-        tables = [table for table in tables if not table.name.startswith(exclude_rule)]
-
-    # Parse Ref
-    relationships = get_relationships(manifest)
-    table_names = [x.name for x in tables]
-    relationships = [
-        x
-        for x in relationships
-        if x.table_map[0] in table_names and x.table_map[1] in table_names
-    ]
-
-    # Fullfill columns in Tables (due to `select *`)
-    for relationship in relationships:
-        for table in tables:
-            table_columns = [x.name.lower() for x in table.columns]
-            if (
-                table.name == relationship.table_map[0]
-                and relationship.column_map[0].lower() not in table_columns
-            ):
-                table.columns.append(Column(name=relationship.column_map[0]))
-            if (
-                table.name == relationship.table_map[1]
-                and relationship.column_map[1].lower() not in table_columns
-            ):
-                table.columns.append(Column(name=relationship.column_map[1]))
-
-    return (tables, relationships)
+from dbterd.adapters.algos.meta import Column, Table
 
 
 def get_tables(manifest, catalog):
-    """Extract tables from dbt artifacts"""
-
-    def create_table_and_columns(table_name, resource, catalog_resource=None):
-        table = Table(
-            name=table_name,
-            raw_sql=get_compiled_sql(resource),
-            database=resource.database.lower(),
-            schema=resource.schema_.lower(),
-            columns=[],
-            resource_type=table_name.split(".")[0],
-        )
-
-        if catalog_resource:
-            for column, metadata in catalog_resource.columns.items():
-                table.columns.append(
-                    Column(
-                        name=str(column).lower(),
-                        data_type=str(metadata.type).lower(),
-                    )
-                )
-
-        for column_name, column_metadata in resource.columns.items():
-            column_name = column_name.strip('"')
-            if not any(c.name.lower() == column_name.lower() for c in table.columns):
-                table.columns.append(
-                    Column(
-                        name=column_name.lower(),
-                        data_type=str(column_metadata.data_type or "unknown").lower(),
-                    )
-                )
-
-        if not table.columns:
-            table.columns.append(Column())
-
-        return table
+    """Extract tables from dbt artifacts
 
+    Args:
+        manifest (dict): dbt manifest json
+        catalog (dict): dbt catalog json
+
+    Returns:
+        List[Table]: All tables parsed from dbt artifacts
+    """
     tables = []
 
     if hasattr(manifest, "nodes"):
         for table_name, node in manifest.nodes.items():
             if (
                 table_name.startswith("model.")
                 or table_name.startswith("seed.")
                 or table_name.startswith("snapshot.")
             ):
                 catalog_node = catalog.nodes.get(table_name)
-                table = create_table_and_columns(table_name, node, catalog_node)
+                table = get_table(
+                    table_name=table_name, manifest_node=node, catalog_node=catalog_node
+                )
                 tables.append(table)
 
     if hasattr(manifest, "sources"):
         for table_name, source in manifest.sources.items():
             if table_name.startswith("source"):
                 catalog_source = catalog.sources.get(table_name)
-                table = create_table_and_columns(table_name, source, catalog_source)
+                table = get_table(
+                    table_name=table_name,
+                    manifest_node=source,
+                    catalog_node=catalog_source,
+                )
                 tables.append(table)
 
     return tables
 
 
-def get_relationships(manifest):
-    """Extract relationships from dbt artifacts based on test relationship"""
-    refs = [
-        Ref(
-            name=x,
-            table_map=manifest.parent_map[x],
-            column_map=[
-                str(
-                    manifest.nodes[x].test_metadata.kwargs.get("field", "unknown")
-                ).lower(),
-                str(
-                    manifest.nodes[x].test_metadata.kwargs.get("column_name", "unknown")
-                ).lower(),
-            ],
-        )
-        for x in manifest.nodes
-        if (
-            x.startswith("test")
-            and "relationship" in x.lower()
-            and manifest.nodes[x].meta.get("ignore_in_erd", "0") == "0"
-        )
-    ]
+def enrich_tables_from_relationships(tables, relationships):
+    """Fullfill columns in Table due to `select *`
+
+    Args:
+        tables (List[Table]): List of Tables
+        relationships (List[Ref]): List of Relationships between Tables
+
+    Returns:
+        List[Table]: Enriched tables
+    """
+    copied_tables = copy.deepcopy(tables)
+    for relationship in relationships:
+        for table in copied_tables:
+            table_columns = [x.name.lower() for x in table.columns]
+            if (
+                table.name == relationship.table_map[0]
+                and relationship.column_map[0].lower() not in table_columns
+            ):
+                table.columns.append(Column(name=relationship.column_map[0]))
+            if (
+                table.name == relationship.table_map[1]
+                and relationship.column_map[1].lower() not in table_columns
+            ):
+                table.columns.append(Column(name=relationship.column_map[1]))
+    return copied_tables
 
-    # remove duplicates
-    if refs:
-        distinct_list = [refs[0]]
-        for ref in refs:
-            distinct_maps = [str((x.table_map, x.column_map)) for x in distinct_list]
-            if str((ref.table_map, ref.column_map)) not in distinct_maps:
-                distinct_list.append(ref)
 
-        return distinct_list
+def get_table(table_name, manifest_node, catalog_node=None):
+    """Construct a single Table object
 
-    return []
+    Args:
+        table_name (str): Table name
+        manifest_node (dict): Manifest node
+        catalog_node (dict, optional): Catalog node. Defaults to None.
+
+    Returns:
+        Table: Parsed table
+    """
+    table = Table(
+        name=table_name,
+        raw_sql=get_compiled_sql(manifest_node),
+        database=manifest_node.database.lower(),
+        schema=manifest_node.schema_.lower(),
+        columns=[],
+        resource_type=table_name.split(".")[0],
+    )
+
+    if catalog_node:
+        for column, metadata in catalog_node.columns.items():
+            table.columns.append(
+                Column(
+                    name=str(column).lower(),
+                    data_type=str(metadata.type).lower(),
+                )
+            )
+
+    for column_name, column_metadata in manifest_node.columns.items():
+        column_name = column_name.strip('"')
+        if not any(c.name.lower() == column_name.lower() for c in table.columns):
+            table.columns.append(
+                Column(
+                    name=column_name.lower(),
+                    data_type=str(column_metadata.data_type or "unknown").lower(),
+                )
+            )
+
+    if not table.columns:
+        table.columns.append(Column())
+
+    return table
 
 
 def get_compiled_sql(manifest_node):
+    """Retrieve compiled SQL from manifest node
+
+    Args:
+        manifest_node (dict): Manifest node
+
+    Returns:
+        str: Compiled SQL
+    """
     if hasattr(manifest_node, "compiled_sql"):  # up to v6
         return manifest_node.compiled_sql
 
     if hasattr(manifest_node, "compiled_code"):  # from v7
         return manifest_node.compiled_code
 
     if hasattr(
         manifest_node, "columns"
     ):  # nodes having no compiled but just list of columns
         return """select
             {columns}
-        from {table}
-        """.format(
+        from {table}""".format(
             columns=",\n".join([f"{x}" for x in manifest_node.columns]),
             table=f"{manifest_node.database}.{manifest_node.schema}.undefined",
         )
 
     return manifest_node.raw_sql  # fallback to raw dbt code
```

### Comparing `dbterd-1.1.0b1/dbterd/adapters/base.py` & `dbterd-1.1.0b2/dbterd/adapters/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,63 @@
 import abc
-from asyncio.log import logger
 
 import click
 
 from dbterd.adapters import factory
 from dbterd.helpers import cli_messaging
 from dbterd.helpers import file as file_handlers
+from dbterd.helpers.log import logger
 
 
 class Executor(abc.ABC):
+    """Base executor"""
+
     ctx: click.Context
 
     def __init__(self, ctx) -> None:
         super().__init__()
         self.ctx = ctx
         self.filename_manifest = "manifest.json"
         self.filename_catalog = "catalog.json"
 
     @abc.abstractmethod
     def run(self, **kwargs):
+        """Main function helps to run by the target strategy"""
         self.__run_by_strategy(**kwargs)
 
     def __read_manifest(self, mp: str, mv: int = None):
+        """Read the Manifest content
+
+        Args:
+            mp (str): manifest.json json file path
+            mv (int, optional): Manifest version. Defaults to None.
+
+        Returns:
+            dict: Manifest dict
+        """
         cli_messaging.check_existence(mp, self.filename_manifest)
         conditional = f" or provided version {mv} is incorrect" if mv else ""
         with cli_messaging.handle_read_errors(self.filename_manifest, conditional):
             return file_handlers.read_manifest(mp, mv)
 
     def __read_catalog(self, cp: str):
+        """Read the Catalog content
+
+        Args:
+            cp (str): catalog.json file path
+
+        Returns:
+            dict: Catalog dict
+        """
         cli_messaging.check_existence(cp, self.filename_catalog)
         with cli_messaging.handle_read_errors(self.filename_catalog):
             return file_handlers.read_catalog(cp)
 
     def __run_by_strategy(self, **kwargs):
+        """Read artifacts and export the diagram file following the target"""
         target = factory.load_executor(name=kwargs["target"])  # import {target}
         run_operation_dispatcher = getattr(target, "run_operation_dispatcher")
         operation_default = getattr(target, "run_operation_default")
         operation = run_operation_dispatcher.get(
             f"{kwargs['target']}_{kwargs['algo']}",
             operation_default,
         )
```

### Comparing `dbterd-1.1.0b1/dbterd/adapters/targets/dbml/dbml_test_relationship.py` & `dbterd-1.1.0b2/dbterd/adapters/targets/dbml/dbml_test_relationship.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 from dbterd.adapters.algos import test_relationship
 
 
 def run(manifest, catalog, **kwargs):
+    """Parse dbt artifacts and export DBML file
+
+    Args:
+        manifest (dict): Manifest json
+        catalog (dict): Catalog json
+
+    Returns:
+        Tuple(str, str): File name and the DBML content
+    """
     return ("output.dbml", parse(manifest, catalog, **kwargs))
 
 
 def parse(manifest, catalog, **kwargs):
+    """Get the DBML content from dbt artifacts
+
+    Args:
+        manifest (dict): Manifest json
+        catalog (dict): Catalog json
+
+    Returns:
+        str: DBML content
+    """
     tables, relationships = test_relationship.parse(
         manifest=manifest, catalog=catalog, **kwargs
     )
 
     # Build DBML content
     dbml = "//Tables (based on the selection criteria)\n"
     for table in tables:
```

### Comparing `dbterd-1.1.0b1/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py` & `dbterd-1.1.0b2/dbterd/adapters/targets/mermaid/mermaid_test_relationship.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,33 @@
 from dbterd.adapters.algos import test_relationship
 
 
 def run(manifest, catalog, **kwargs):
+    """Parse dbt artifacts and export Mermaid file
+
+    Args:
+        manifest (dict): Manifest json
+        catalog (dict): Catalog json
+
+    Returns:
+        Tuple(str, str): File name and the Mermaid content
+    """
     return ("output.md", parse(manifest, catalog, **kwargs))
 
 
 def parse(manifest, catalog, **kwargs):
+    """Get the Mermaid content from dbt artifacts
+
+    Args:
+        manifest (dict): Manifest json
+        catalog (dict): Catalog json
+
+    Returns:
+        str: Mermaid content
+    """
     tables, relationships = test_relationship.parse(
         manifest=manifest, catalog=catalog, **kwargs
     )
 
     # Build Mermaid content
     # https://mermaid.js.org/syntax/entityRelationshipDiagram.html
     mermaid = "erDiagram\n"
```

### Comparing `dbterd-1.1.0b1/dbterd/cli/main.py` & `dbterd-1.1.0b2/dbterd/cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,18 +9,29 @@
 from dbterd.helpers.log import logger
 
 __version__ = importlib.metadata.version("dbterd")
 
 
 # Programmatic invocation
 class dbterdRunner:
+    """Support runner for the programatic call"""
+
     def __init__(self) -> None:
         pass
 
     def invoke(self, args: List[str]):
+        """Invoke a command of dbterd programatically
+
+        Args:
+            args (List[str]): dbterd arguments
+
+        Raises:
+            Exception: Unhandled exception
+            Exception: Not Supported command exception
+        """
         try:
             dbt_ctx = dbterd.make_context(dbterd.name, args)
             return dbterd.invoke(dbt_ctx)
         except click.exceptions.Exit as e:
             # 0 exit code, expected for --version early exit
             if str(e) == "0":
                 return [], True
```

### Comparing `dbterd-1.1.0b1/dbterd/cli/params.py` & `dbterd-1.1.0b2/dbterd/cli/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,40 +11,35 @@
         "-ad",
         help="Specified the full path to dbt artifacts path which known as /target directory",
         default=default.default_artifact_path(),
         show_default=True,
         type=click.STRING,
     )
     @click.option(
-        "--manifest-path",
-        "-mp",
-        help="__DEPRECATED_WARNING__: Specified the full directory path to dbt manifest.json file. Use --artifacts-dir instead.",
-        default=None,
-        type=click.STRING,
-    )
-    @click.option(
         "--output",
         "-o",
         help="Output the result file. Default to the same target dir",
         default=default.default_output_path(),
         show_default=True,
         type=click.STRING,
     )
     @click.option(
         "--select",
         "-s",
-        help="Selecttion criteria. Support 'starts with' a string",
-        default=None,
+        help="Selecttion criteria",
+        default=[],
+        multiple=True,
         type=click.STRING,
     )
     @click.option(
         "--exclude",
         "-ns",
-        help="Exclusion criteria. Support 'not starts with' a string",
-        default=None,
+        help="Exclusion criteria",
+        default=[],
+        multiple=True,
         type=click.STRING,
     )
     @click.option(
         "--target",
         "-t",
         help="Target to the diagram-as-code platform",
         default=default.default_target(),
```

### Comparing `dbterd-1.1.0b1/dbterd/helpers/cli_messaging.py` & `dbterd-1.1.0b2/dbterd/helpers/cli_messaging.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b1/dbterd/helpers/dict.py` & `dbterd-1.1.0b2/dbterd/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b1/dbterd/helpers/file.py` & `dbterd-1.1.0b2/dbterd/helpers/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,17 +29,22 @@
 
 def open_json(fp):
     """Json loading utility, leveraging long path fixes"""
     return json.loads(load_file_contents(fp))
 
 
 def convert_path(path: str) -> str:
-    """Convert a path which might be >260 characters long, to one
-    that will be writable/readable on Windows.
+    """Convert a path which might be >260 characters long, to one that will be writable/readable on Windows.
     On other platforms, this is a no-op.
+
+    Args:
+        path (str): Path string
+
+    Returns:
+        str: Converted path string
     """
     # some parts of python seem to append '\*.*' to strings, better safe than
     # sorry.
     if len(path) < 250:
         return path
     if supports_long_paths():
         return path
@@ -76,17 +81,15 @@
             return False  # pragma: no cover
         # tell windows we want to get back a single unsigned byte (a bool).
         dll.RtlAreLongPathsEnabled.restype = c_bool
         return dll.RtlAreLongPathsEnabled()
 
 
 def win_prepare_path(path: str) -> str:  # pragma: no cover
-    """Given a windows path, prepare it for use by making sure it is absolute
-    and normalized.
-    """
+    """Given a windows path, prepare it for use by making sure it is absolute and normalized."""
     path = os.path.normpath(path)
 
     # if a path starts with '\', splitdrive() on it will return '' for the
     # drive, but the prefix requires a drive letter. So let's add the drive
     # letter back in.
     # Unless it starts with '\\'. In that case, the path is a UNC mount point
     # and splitdrive will be fine.
@@ -101,20 +104,36 @@
     if not os.path.splitdrive(path)[0]:
         path = os.path.join(os.getcwd(), path)
 
     return path
 
 
 def read_manifest(path: str, version: int = None):
-    """Reads in the manifest.json file, with optional version specification"""
+    """Reads in the manifest.json file, with optional version specification
+
+    Args:
+        path (str): manifest.json file path
+        version (int, optional): Manifest version. Defaults to None.
+
+    Returns:
+        dict: Manifest dict
+    """
     _dict = open_json(f"{path}/manifest.json")
     parser_version = f"parse_manifest_v{version}" if version else "parse_manifest"
     parse_func = getattr(parser, parser_version)
     return parse_func(manifest=_dict)
 
 
 def read_catalog(path: str, version: int = None):
-    """Reads in the catalog.json file, with optional version specification"""
+    """Reads in the catalog.json file, with optional version specification
+
+    Args:
+        path (str): catalog.json file path
+        version (int, optional): Catalog version. Defaults to None.
+
+    Returns:
+        dict: Catalog dict
+    """
     _dict = open_json(f"{path}/catalog.json")
     parser_version = f"parse_catalog_v{version}" if version else "parse_catalog"
     parse_func = getattr(parser, parser_version)
     return parse_func(catalog=_dict)
```

### Comparing `dbterd-1.1.0b1/dbterd/helpers/jsonify.py` & `dbterd-1.1.0b2/dbterd/helpers/jsonify.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b1/dbterd/helpers/log.py` & `dbterd-1.1.0b2/dbterd/helpers/log.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b1/dbterd/helpers/yaml.py` & `dbterd-1.1.0b2/dbterd/helpers/yaml.py`

 * *Files identical despite different names*

### Comparing `dbterd-1.1.0b1/pyproject.toml` & `dbterd-1.1.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbterd"
-version = "1.1.0b1"
+version = "1.1.0b2"
 description = "dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file"
 authors = ["Dat Nguyen <datnguyen.it09@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/datnguye/dbterd"
 repository = "https://github.com/datnguye/dbterd"
 keywords = ["flake8", "markdown", "lint"]
@@ -26,15 +26,14 @@
 [tool.poetry.scripts]
 dbterd = "dbterd.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 dbt-artifacts-parser = "^0.2.3"
-sqlparse = "^0.4.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-sugar = "^0.9.6"
 black = "^22.10.0"
 coverage = {version = "^6.5.0", extras = ["toml"]}
 poethepoet = "^0.16.4"
```

### Comparing `dbterd-1.1.0b1/PKG-INFO` & `dbterd-1.1.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbterd
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: dbterd is a Command Line Interface (CLI) to convert dbt manifest.json file to diagram file
 Home-page: https://github.com/datnguye/dbterd
 License: MIT
 Keywords: flake8,markdown,lint
 Author: Dat Nguyen
 Author-email: datnguyen.it09@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dbt-artifacts-parser (>=0.2.3,<0.3.0)
-Requires-Dist: sqlparse (>=0.4.3,<0.5.0)
 Project-URL: Repository, https://github.com/datnguye/dbterd
 Description-Content-Type: text/markdown
 
 # dbterd
 CLI to generate Diagram-as-a-code file ([DBML](https://dbdiagram.io/d), [Mermaid](https://mermaid-js.github.io/mermaid-live-editor/)) from dbt artifact files (required: `manifest.json`, `catalog.json`)
 > Version 0.1: only required `manifest.json`
```

