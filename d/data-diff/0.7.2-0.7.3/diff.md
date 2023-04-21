# Comparing `tmp/data_diff-0.7.2.tar.gz` & `tmp/data_diff-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.7.2.tar", max compression
+gzip compressed data, was "data_diff-0.7.3.tar", max compression
```

## Comparing `data_diff-0.7.2.tar` & `data_diff-0.7.3.tar`

### file list

```diff
@@ -1,40 +1,72 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.2/LICENSE
--rw-r--r--   0        0        0     4773 2023-04-14 15:23:33.906410 data_diff-0.7.2/README.md
--rw-r--r--   0        0        0     8419 2023-04-03 18:06:26.931396 data_diff-0.7.2/data_diff/__init__.py
--rw-r--r--   0        0        0    15796 2023-04-03 18:06:26.931499 data_diff-0.7.2/data_diff/__main__.py
--rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.2/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0     9235 2023-04-14 15:23:33.906694 data_diff-0.7.2/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0     8746 2023-04-14 15:23:33.906807 data_diff-0.7.2/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.2/data_diff/config.py
--rw-r--r--   0        0        0      483 2023-04-03 18:06:26.931645 data_diff-0.7.2/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1343 2023-04-03 18:06:26.931693 data_diff-0.7.2/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      164 2023-04-03 18:06:26.931735 data_diff-0.7.2/data_diff/databases/base.py
--rw-r--r--   0        0        0      247 2023-04-03 18:06:26.931779 data_diff-0.7.2/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      261 2023-04-03 18:06:26.931823 data_diff-0.7.2/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      261 2023-04-03 18:06:26.931868 data_diff-0.7.2/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      233 2023-04-03 18:06:26.931912 data_diff-0.7.2/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      226 2023-04-03 18:06:26.931970 data_diff-0.7.2/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      233 2023-04-03 18:06:26.932016 data_diff-0.7.2/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      265 2023-04-03 18:06:26.932063 data_diff-0.7.2/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      233 2023-04-03 18:06:26.932105 data_diff-0.7.2/data_diff/databases/presto.py
--rw-r--r--   0        0        0      247 2023-04-03 18:06:26.932150 data_diff-0.7.2/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      254 2023-04-03 18:06:26.932199 data_diff-0.7.2/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      226 2023-04-03 18:06:26.932247 data_diff-0.7.2/data_diff/databases/trino.py
--rw-r--r--   0        0        0      240 2023-04-03 18:06:26.932292 data_diff-0.7.2/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    13473 2023-04-14 23:37:25.350943 data_diff-0.7.2/data_diff/dbt.py
--rw-r--r--   0        0        0    13346 2023-04-18 20:40:59.490092 data_diff-0.7.2/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14366 2023-04-03 18:06:26.932528 data_diff-0.7.2/data_diff/diff_tables.py
--rw-r--r--   0        0        0     8557 2023-04-03 18:06:26.932606 data_diff-0.7.2/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.2/data_diff/info_tree.py
--rw-r--r--   0        0        0    14718 2023-04-03 18:06:26.932755 data_diff-0.7.2/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.2/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.2/data_diff/parse_time.py
--rw-r--r--   0        0        0     1384 2023-04-03 18:06:26.932946 data_diff-0.7.2/data_diff/query_utils.py
--rw-r--r--   0        0        0     1818 2023-04-03 18:06:26.933026 data_diff-0.7.2/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0    10834 2023-04-03 18:06:26.933122 data_diff-0.7.2/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.2/data_diff/thread_utils.py
--rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.2/data_diff/tracking.py
--rw-r--r--   0        0        0     4306 2023-04-14 15:23:33.907379 data_diff-0.7.2/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-04-18 20:40:59.490257 data_diff-0.7.2/data_diff/version.py
--rwxr-xr-x   0        0        0     2708 2023-04-18 20:40:59.490498 data_diff-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 data_diff-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4773 2023-04-14 15:23:33.906410 data_diff-0.7.3/README.md
+-rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.3/data_diff/__init__.py
+-rw-r--r--   0        0        0    15816 2023-04-21 21:58:08.194100 data_diff-0.7.3/data_diff/__main__.py
+-rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.3/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.3/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0     9253 2023-04-21 21:58:08.194472 data_diff-0.7.3/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.3/data_diff/config.py
+-rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.3/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.3/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.3/data_diff/databases/base.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.3/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.3/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.3/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.3/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.3/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.3/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.3/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.3/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.3/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.3/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.3/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.3/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    14002 2023-04-21 21:58:08.196463 data_diff-0.7.3/data_diff/dbt.py
+-rw-r--r--   0        0        0    13759 2023-04-21 21:58:08.196614 data_diff-0.7.3/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.3/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     8567 2023-04-21 21:58:08.196909 data_diff-0.7.3/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.3/data_diff/info_tree.py
+-rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.3/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.3/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.3/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.3/data_diff/query_utils.py
+-rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.3/data_diff/sqeleton/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.3/data_diff/sqeleton/__main__.py
+-rw-r--r--   0        0        0      254 2023-04-21 21:58:08.197672 data_diff-0.7.3/data_diff/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.3/data_diff/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    10339 2023-04-21 21:58:08.197842 data_diff-0.7.3/data_diff/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     5909 2023-04-21 21:58:08.197929 data_diff-0.7.3/data_diff/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.3/data_diff/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.3/data_diff/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9131 2023-04-21 21:58:08.198249 data_diff-0.7.3/data_diff/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    19920 2023-04-21 21:58:08.198404 data_diff-0.7.3/data_diff/sqeleton/databases/base.py
+-rw-r--r--   0        0        0     7140 2023-04-21 21:58:08.198520 data_diff-0.7.3/data_diff/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.3/data_diff/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.3/data_diff/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.3/data_diff/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.3/data_diff/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.3/data_diff/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6523 2023-04-21 21:58:08.199025 data_diff-0.7.3/data_diff/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5430 2023-04-21 21:58:08.199106 data_diff-0.7.3/data_diff/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.3/data_diff/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     4844 2023-04-21 21:58:08.199284 data_diff-0.7.3/data_diff/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.3/data_diff/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.3/data_diff/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.3/data_diff/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.3/data_diff/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.3/data_diff/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    30646 2023-04-21 21:58:08.199945 data_diff-0.7.3/data_diff/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.3/data_diff/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.3/data_diff/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.3/data_diff/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.3/data_diff/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.3/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.3/data_diff/sqeleton/schema.py
+-rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.3/data_diff/sqeleton/utils.py
+-rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.3/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.3/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.3/data_diff/tracking.py
+-rw-r--r--   0        0        0     4306 2023-04-14 15:23:33.907379 data_diff-0.7.3/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-04-21 21:58:08.200716 data_diff-0.7.3/data_diff/version.py
+-rwxr-xr-x   0        0        0     2865 2023-04-21 21:58:08.202087 data_diff-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     7387 1970-01-01 00:00:00.000000 data_diff-0.7.3/PKG-INFO
```

### Comparing `data_diff-0.7.2/LICENSE` & `data_diff-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.2/README.md` & `data_diff-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.2/data_diff/__init__.py` & `data_diff-0.7.3/data_diff/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Sequence, Tuple, Iterator, Optional, Union
 
-from sqeleton.abcs import DbTime, DbPath
+from data_diff.sqeleton.abcs import DbTime, DbPath
 
 from .tracking import disable_tracking
 from .databases import connect
 from .diff_tables import Algorithm
 from .hashdiff_tables import HashDiffer, DEFAULT_BISECTION_THRESHOLD, DEFAULT_BISECTION_FACTOR
 from .joindiff_tables import JoinDiffer, TABLE_WRITE_LIMIT
 from .table_segment import TableSegment
```

### Comparing `data_diff-0.7.2/data_diff/__main__.py` & `data_diff-0.7.3/data_diff/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import logging
 from itertools import islice
 from typing import Optional
 
 import rich
 import click
 
-from sqeleton.schema import create_schema
-from sqeleton.queries.api import current_timestamp
+from data_diff.sqeleton.schema import create_schema
+from data_diff.sqeleton.queries.api import current_timestamp
 
 from .dbt import dbt_diff
 from .utils import eval_name_template, remove_password_from_url, safezip, match_like
 from .diff_tables import Algorithm
 from .hashdiff_tables import HashDiffer, DEFAULT_BISECTION_THRESHOLD, DEFAULT_BISECTION_FACTOR
 from .joindiff_tables import TABLE_WRITE_LIMIT, JoinDiffer
 from .table_segment import TableSegment
```

### Comparing `data_diff-0.7.2/data_diff/cloud/data_source.py` & `data_diff-0.7.3/data_diff/cloud/data_source.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import time
 from typing import List, Optional, Union, overload
 
 import pydantic
 import rich
 from rich.table import Table
 from rich.prompt import Confirm, Prompt, FloatPrompt, IntPrompt, InvalidResponse
@@ -46,22 +47,41 @@
 
 
 def _validate_temp_schema(temp_schema: str):
     if len(temp_schema.split(".")) != 2:
         raise ValueError("Temporary schema should have a format <database>.<schema>")
 
 
+def _get_temp_schema(dbt_parser: DbtParser, db_type: str) -> Optional[str]:
+    diff_vars = dbt_parser.get_datadiff_variables()
+    config_prod_database = diff_vars.get("prod_database")
+    config_prod_schema = diff_vars.get("prod_schema")
+    if config_prod_database is not None and config_prod_schema is not None:
+        temp_schema = f"{config_prod_database}.{config_prod_schema}"
+        if db_type == "snowflake":
+            return temp_schema.upper()
+        elif db_type in {"pg", "postgres_aurora", "postgres_aws_rds", "redshift"}:
+            return temp_schema.lower()
+        return temp_schema
+    return
+
+
 def create_ds_config(
     ds_config: TCloudApiDataSourceConfigSchema,
     data_source_name: str,
     dbt_parser: Optional[DbtParser] = None,
 ) -> TDsConfig:
     options = _parse_ds_credentials(ds_config=ds_config, only_basic_settings=True, dbt_parser=dbt_parser)
 
-    temp_schema = TemporarySchemaPrompt.ask("Temporary schema (<database>.<schema>)")
+    temp_schema = _get_temp_schema(dbt_parser=dbt_parser, db_type=ds_config.db_type) if dbt_parser else None
+    if temp_schema:
+        temp_schema = TemporarySchemaPrompt.ask("Temporary schema", default=temp_schema)
+    else:
+        temp_schema = TemporarySchemaPrompt.ask("Temporary schema (<database>.<schema>)")
+
     float_tolerance = FloatPrompt.ask("Float tolerance", default=0.000001)
 
     return TDsConfig(
         name=data_source_name,
         type=ds_config.db_type,
         temp_schema=temp_schema,
         float_tolerance=float_tolerance,
@@ -88,23 +108,55 @@
     if type_ == "integer":
         return int(value)
     elif type_ == "boolean":
         return bool(value)
     return value
 
 
+def _get_data_from_bigquery_json(path: str):
+    with open(path, "r") as file:
+        return json.load(file)
+
+
+def _align_dbt_cred_params_with_datafold_params(dbt_creds: dict) -> dict:
+    db_type = dbt_creds["type"]
+    if db_type == "bigquery":
+        method = dbt_creds["method"]
+        if method == "service-account":
+            data = _get_data_from_bigquery_json(path=dbt_creds["keyfile"])
+            dbt_creds["jsonKeyFile"] = json.dumps(data)
+        elif method == "service-account-json":
+            dbt_creds["jsonKeyFile"] = json.dumps(dbt_creds["keyfile_json"])
+        else:
+            rich.print(
+                f'[red]Cannot extract bigquery credentials from dbt_project.yml for "{method}" type. '
+                f"If you want to provide credentials via dbt_project.yml, "
+                f'please, use "service-account" or "service-account-json" '
+                f"(more in docs: https://docs.getdbt.com/reference/warehouse-setups/bigquery-setup). "
+                f"Otherwise, you can provide a path to a json key file or a json key file data as an input."
+            )
+        dbt_creds["projectId"] = dbt_creds["project"]
+    elif db_type == "snowflake":
+        dbt_creds["default_db"] = dbt_creds["database"]
+    elif db_type == "databricks":
+        dbt_creds["http_password"] = dbt_creds["token"]
+        dbt_creds["database"] = dbt_creds.get("catalog")
+    return dbt_creds
+
+
 def _parse_ds_credentials(
     ds_config: TCloudApiDataSourceConfigSchema, only_basic_settings: bool = True, dbt_parser: Optional[DbtParser] = None
 ):
     creds = {}
     use_dbt_data = False
     if dbt_parser is not None:
         use_dbt_data = Confirm.ask("Would you like to extract database credentials from dbt profiles.yml?")
         try:
             creds = dbt_parser.get_connection_creds()[0]
+            creds = _align_dbt_cred_params_with_datafold_params(dbt_creds=creds)
         except Exception as e:
             rich.print(f"[red]Cannot parse database credentials from dbt profiles.yml. Reason: {e}")
 
     ds_options = {}
     basic_required_fields = set(ds_config.config_schema.required)
     for param_name, param_data in ds_config.config_schema.properties.items():
         if only_basic_settings and param_name not in basic_required_fields:
```

### Comparing `data_diff-0.7.2/data_diff/cloud/datafold_api.py` & `data_diff-0.7.3/data_diff/cloud/datafold_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import base64
 import dataclasses
 import enum
 import time
 from typing import Any, Dict, List, Optional, Type, TypeVar, Tuple
 
 import pydantic
 import requests
 
+from ..utils import getLogger
+
+logger = getLogger(__name__)
 
 Self = TypeVar("Self", bound=pydantic.BaseModel)
 
 
 class TestDataSourceStatus(str, enum.Enum):
     SUCCESS = "ok"
     FAILED = "error"
@@ -93,14 +97,16 @@
 
 class TCloudApiDataDiff(pydantic.BaseModel):
     data_source1_id: int
     data_source2_id: int
     table1: List[str]
     table2: List[str]
     pk_columns: List[str]
+    filter1: Optional[str] = None
+    filter2: Optional[str] = None
 
 
 class TSummaryResultPrimaryKeyStats(pydantic.BaseModel):
     total_rows: Tuple[int, int]
     nulls: Tuple[int, int]
     dupes: Tuple[int, int]
     exclusives: Tuple[int, int]
@@ -155,15 +161,15 @@
     message: str
     outcome: str
 
 
 class TCloudApiDataSourceTestResult(pydantic.BaseModel):
     name: str
     status: str
-    result: TCloudDataSourceTestResult
+    result: Optional[TCloudDataSourceTestResult]
 
 
 @dataclasses.dataclass
 class DatafoldAPI:
     api_key: str
     host: str = "https://app.datafold.com"
     timeout: int = 30
@@ -187,15 +193,19 @@
 
     def get_data_sources(self) -> List[TCloudApiDataSource]:
         rv = self.make_get_request(url="api/v1/data_sources")
         rv.raise_for_status()
         return [TCloudApiDataSource(**item) for item in rv.json()]
 
     def create_data_source(self, config: TDsConfig) -> TCloudApiDataSource:
-        rv = self.make_post_request(url="api/v1/data_sources", payload=config.dict())
+        payload = config.dict()
+        if config.type == "bigquery":
+            json_string = payload["options"]["jsonKeyFile"].encode("utf-8")
+            payload["options"]["jsonKeyFile"] = base64.b64encode(json_string).decode("utf-8")
+        rv = self.make_post_request(url="api/v1/data_sources", payload=payload)
         return TCloudApiDataSource(**rv.json())
 
     def get_data_source_schema_config(
         self,
         only_important_properties: bool = False,
     ) -> List[TCloudApiDataSourceConfigSchema]:
         rv = self.make_get_request(url="api/v1/data_sources/types")
@@ -212,19 +222,20 @@
         rv = self.make_post_request(url="api/v1/datadiffs", payload=payload.dict())
         return rv.json()["id"]
 
     def poll_data_diff_results(self, diff_id: int) -> TCloudApiDataDiffSummaryResult:
         summary_results = None
         start_time = time.monotonic()
         sleep_interval = 5  # starts at 5 sec
-        max_sleep_interval = 60
+        max_sleep_interval = 30
         max_wait_time = 300
 
         diff_url = f"{self.host}/datadiffs/{diff_id}/overview"
         while not summary_results:
+            logger.debug(f"Polling: {diff_url}")
             response = self.make_get_request(url=f"api/v1/datadiffs/{diff_id}/summary_results")
             response_json = response.json()
             if response_json["status"] == "success":
                 summary_results = response_json
             elif response_json["status"] == "failed":
                 raise Exception(f"Diff failed: {str(response_json)}")
 
@@ -246,11 +257,13 @@
             TCloudApiDataSourceTestResult(
                 name=item["step"],
                 status=item["status"],
                 result=TCloudDataSourceTestResult(
                     status=item["result"]["code"].lower(),
                     message=item["result"]["message"],
                     outcome=item["result"]["outcome"],
-                ),
+                )
+                if item["result"] is not None
+                else None,
             )
             for item in rv.json()["results"]
         ]
```

### Comparing `data_diff-0.7.2/data_diff/config.py` & `data_diff-0.7.3/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.2/data_diff/databases/_connect.py` & `data_diff-0.7.3/data_diff/databases/_connect.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from sqeleton.databases import Connect
+from data_diff.sqeleton.databases import Connect
 
 from .postgresql import PostgreSQL
 from .mysql import MySQL
 from .oracle import Oracle
 from .snowflake import Snowflake
 from .bigquery import BigQuery
 from .redshift import Redshift
```

### Comparing `data_diff-0.7.2/data_diff/dbt.py` & `data_diff-0.7.3/data_diff/dbt.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 @dataclass
 class DiffVars:
     dev_path: List[str]
     prod_path: List[str]
     primary_keys: List[str]
     connection: Dict[str, str]
     threads: Optional[int]
+    where_filter: Optional[str] = None
 
 
 def dbt_diff(
     profiles_dir_override: Optional[str] = None, project_dir_override: Optional[str] = None, is_cloud: bool = False
 ) -> None:
     diff_threads = []
     set_entrypoint_name("CLI-dbt")
@@ -114,14 +115,15 @@
                     "https://docs.datafold.com/os_diff/dbt_integration/#configure-a-data-source\n"
                 )
             else:
                 raise ValueError(
                     "Datasource ID not found, include it as a dbt variable in the dbt_project.yml. "
                     "\nvars:\n data_diff:\n   datasource_id: 1234"
                 )
+        rich.print("[green][bold]\nDiffs in progress...[/][/]\n")
 
     else:
         dbt_parser.set_connection()
 
     if config_prod_database is None:
         raise ValueError(
             "Expected a value for prod_database: OR prod_database: AND prod_schema: under \nvars:\n  data_diff: "
@@ -186,15 +188,24 @@
         dev_qualified_list = [x.upper() for x in [dev_database, dev_schema, model.alias]]
         prod_qualified_list = [x.upper() for x in [prod_database, prod_schema, model.alias]]
         primary_keys = [x.upper() for x in primary_keys]
     else:
         dev_qualified_list = [dev_database, dev_schema, model.alias]
         prod_qualified_list = [prod_database, prod_schema, model.alias]
 
-    return DiffVars(dev_qualified_list, prod_qualified_list, primary_keys, dbt_parser.connection, dbt_parser.threads)
+    where_filter = None
+    if model.meta:
+        try:
+            where_filter = model.meta["datafold"]["datadiff"]["filter"]
+        except KeyError:
+            pass
+
+    return DiffVars(
+        dev_qualified_list, prod_qualified_list, primary_keys, dbt_parser.connection, dbt_parser.threads, where_filter
+    )
 
 
 def _local_diff(diff_vars: DiffVars) -> None:
     column_diffs_str = ""
     dev_qualified_str = ".".join(diff_vars.dev_path)
     prod_qualified_str = ".".join(diff_vars.prod_path)
     diff_output_str = _diff_output_base(dev_qualified_str, prod_qualified_str)
@@ -223,15 +234,22 @@
 
     if table2_set_diff:
         column_diffs_str += "Column(s) removed: " + str(table2_set_diff) + "\n"
 
     mutual_set = mutual_set - set(diff_vars.primary_keys)
     extra_columns = tuple(mutual_set)
 
-    diff = diff_tables(table1, table2, threaded=True, algorithm=Algorithm.JOINDIFF, extra_columns=extra_columns)
+    diff = diff_tables(
+        table1,
+        table2,
+        threaded=True,
+        algorithm=Algorithm.JOINDIFF,
+        extra_columns=extra_columns,
+        where=diff_vars.where_filter,
+    )
 
     if list(diff):
         diff_output_str += f"{column_diffs_str}{diff.get_stats_string(is_dbt=True)} \n"
         rich.print(diff_output_str)
     else:
         diff_output_str += f"{column_diffs_str}[bold][green]No row differences[/][/] \n"
         rich.print(diff_output_str)
@@ -272,34 +290,36 @@
     diff_output_str = _diff_output_base(".".join(diff_vars.dev_path), ".".join(diff_vars.prod_path))
     payload = TCloudApiDataDiff(
         data_source1_id=datasource_id,
         data_source2_id=datasource_id,
         table1=diff_vars.prod_path,
         table2=diff_vars.dev_path,
         pk_columns=diff_vars.primary_keys,
+        filter1=diff_vars.where_filter,
+        filter2=diff_vars.where_filter,
     )
 
     if is_tracking_enabled():
         event_json = create_start_event_json({"is_cloud": True, "datasource_id": datasource_id})
         run_as_daemon(send_event_json, event_json)
 
     start = time.monotonic()
     error = None
     diff_id = None
     diff_url = None
     try:
         diff_id = api.create_data_diff(payload=payload)
+        diff_url = f"{api.host}/datadiffs/{diff_id}/overview"
+        rich.print(f"{diff_vars.dev_path[2]}: {diff_url}")
 
         if diff_id is None:
             raise Exception(f"Api response did not contain a diff_id")
 
         diff_results = api.poll_data_diff_results(diff_id)
 
-        diff_url = f"{api.host}/datadiffs/{diff_id}/overview"
-
         rows_added_count = diff_results.pks.exclusives[1]
         rows_removed_count = diff_results.pks.exclusives[0]
 
         rows_updated = diff_results.values.rows_with_differences
         total_rows = diff_results.values.total_rows
         rows_unchanged = int(total_rows) - int(rows_updated)
         diff_percent_list = {
@@ -348,8 +368,8 @@
             if diff_id:
                 diff_url = f"{api.host}/datadiffs/{diff_id}/overview"
                 rich.print(f"{diff_url} \n")
             logger.error(error)
 
 
 def _diff_output_base(dev_path: str, prod_path: str) -> str:
-    return f"[green]{prod_path} <> {dev_path}[/] \n"
+    return f"\n[green]{prod_path} <> {dev_path}[/] \n"
```

### Comparing `data_diff-0.7.2/data_diff/dbt_parser.py` & `data_diff-0.7.3/data_diff/dbt_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 RUN_RESULTS_PATH = "target/run_results.json"
 MANIFEST_PATH = "target/manifest.json"
 PROJECT_FILE = "dbt_project.yml"
 PROFILES_FILE = "profiles.yml"
 LOWER_DBT_V = "1.0.0"
-UPPER_DBT_V = "1.4.6"
+UPPER_DBT_V = "1.4.7"
 
 
 # https://github.com/dbt-labs/dbt-core/blob/c952d44ec5c2506995fbad75320acbae49125d3d/core/dbt/cli/resolvers.py#L6
 def default_project_dir() -> Path:
     paths = list(Path.cwd().parents)
     paths.insert(0, Path.cwd())
     return next((x for x in paths if (x / PROJECT_FILE).exists()), Path.cwd())
@@ -64,49 +64,55 @@
 
     def get_datadiff_variables(self) -> dict:
         vars = get_from_dict_with_raise(self.project_dict, "vars", f"No vars: found in dbt_project.yml.")
         return get_from_dict_with_raise(vars, "data_diff", f"data_diff: section not found in dbt_project.yml vars:.")
 
     def get_models(self):
         with open(self.project_dir / RUN_RESULTS_PATH) as run_results:
+            logger.info(f"Parsing file {RUN_RESULTS_PATH}")
             run_results_dict = json.load(run_results)
             run_results_obj = self.parse_run_results(run_results=run_results_dict)
 
         dbt_version = parse_version(run_results_obj.metadata.dbt_version)
 
         if dbt_version < parse_version("1.3.0"):
             self.profiles_dir = legacy_profiles_dir()
 
-        if dbt_version < parse_version(LOWER_DBT_V) or dbt_version >= parse_version(UPPER_DBT_V):
+        if dbt_version < parse_version(LOWER_DBT_V):
             raise Exception(
-                f"Found dbt: v{dbt_version} Expected the dbt project's version to be >= {LOWER_DBT_V} and < {UPPER_DBT_V}"
+                f"Found dbt: v{dbt_version} Expected the dbt project's version to be >= {LOWER_DBT_V}"
             )
+        elif dbt_version >= parse_version(UPPER_DBT_V):
+            logger.warning(f"{dbt_version} is a recent version of dbt and may not be fully tested with data-diff! \nPlease report any issues to https://github.com/datafold/data-diff/issues")
 
         success_models = [x.unique_id for x in run_results_obj.results if x.status.name == "success"]
         models = [self.manifest_obj.nodes.get(x) for x in success_models]
         if not models:
             raise ValueError("Expected > 0 successful models runs from the last dbt command.")
 
         print(f"Running with data-diff={__version__}\n")
         return models
 
     def get_manifest_obj(self):
         with open(self.project_dir / MANIFEST_PATH) as manifest:
+            logger.info(f"Parsing file {MANIFEST_PATH}")
             manifest_dict = json.load(manifest)
             manifest_obj = self.parse_manifest(manifest=manifest_dict)
         return manifest_obj
 
     def get_project_dict(self):
         with open(self.project_dir / PROJECT_FILE) as project:
+            logger.info(f"Parsing file {PROJECT_FILE}")
             project_dict = self.yaml.safe_load(project)
         return project_dict
 
     def get_connection_creds(self) -> Tuple[Dict[str, str], str]:
         profiles_path = self.profiles_dir / PROFILES_FILE
         with open(profiles_path) as profiles:
+            logger.info(f"Parsing file {profiles_path}")
             profiles = self.yaml.safe_load(profiles)
 
         dbt_profile_var = self.project_dict.get("profile")
 
         profile = get_from_dict_with_raise(
             profiles, dbt_profile_var, f"No profile '{dbt_profile_var}' found in '{profiles_path}'."
         )
@@ -141,15 +147,15 @@
                 "user": credentials.get("user"),
                 "account": credentials.get("account"),
                 "database": credentials.get("database"),
                 "warehouse": credentials.get("warehouse"),
                 "role": credentials.get("role"),
                 "schema": credentials.get("schema"),
                 "insecure_mode": credentials.get("insecure_mode", False),
-                "client_session_keep_alive": credentials.get("client_session_keep_alive", False)
+                "client_session_keep_alive": credentials.get("client_session_keep_alive", False),
             }
             self.threads = credentials.get("threads")
             self.requires_upper = True
 
             if credentials.get("private_key_path") is not None:
                 if credentials.get("password") is not None:
                     raise Exception("Cannot use password and key at the same time")
```

### Comparing `data_diff-0.7.2/data_diff/diff_tables.py` & `data_diff-0.7.3/data_diff/diff_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from data_diff.info_tree import InfoTree, SegmentInfo
 
 from .utils import dbt_diff_string_template, run_as_daemon, safezip, getLogger, truncate_error, Vector
 from .thread_utils import ThreadedYielder
 from .table_segment import TableSegment, create_mesh_from_points
 from .tracking import create_end_event_json, create_start_event_json, send_event_json, is_tracking_enabled
-from sqeleton.abcs import IKey
+from data_diff.sqeleton.abcs import IKey
 
 logger = getLogger(__name__)
 
 
 class Algorithm(Enum):
     AUTO = "auto"
     JOINDIFF = "joindiff"
```

### Comparing `data_diff-0.7.2/data_diff/hashdiff_tables.py` & `data_diff-0.7.3/data_diff/hashdiff_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from collections import defaultdict
 from typing import Iterator
 from operator import attrgetter
 
 from runtype import dataclass
 
-from sqeleton.abcs import ColType_UUID, NumericType, PrecisionType, StringType, Boolean
+from data_diff.sqeleton.abcs import ColType_UUID, NumericType, PrecisionType, StringType, Boolean
 
 from .info_tree import InfoTree
 from .utils import safezip
 from .thread_utils import ThreadedYielder
 from .table_segment import TableSegment
 
 from .diff_tables import TableDiffer
```

### Comparing `data_diff-0.7.2/data_diff/info_tree.py` & `data_diff-0.7.3/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.2/data_diff/joindiff_tables.py` & `data_diff-0.7.3/data_diff/joindiff_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 from functools import partial
 import logging
 from typing import List
 from itertools import chain
 
 from runtype import dataclass
 
-from sqeleton.databases import Database, MySQL, BigQuery, Presto, Oracle, Snowflake, DbPath
-from sqeleton.abcs import NumericType
-from sqeleton.queries import (
+from data_diff.sqeleton.databases import Database, MySQL, BigQuery, Presto, Oracle, Snowflake, DbPath
+from data_diff.sqeleton.abcs import NumericType
+from data_diff.sqeleton.queries import (
     table,
     sum_,
     min_,
     max_,
     avg,
     and_,
     if_,
     or_,
     outerjoin,
     leftjoin,
     rightjoin,
     this,
     Compiler,
 )
-from sqeleton.queries.ast_classes import Concat, Count, Expr, Random, TablePath, Code, ITable
-from sqeleton.queries.extras import NormalizeAsString
+from data_diff.sqeleton.queries.ast_classes import Concat, Count, Expr, Random, TablePath, Code, ITable
+from data_diff.sqeleton.queries.extras import NormalizeAsString
 
 from .info_tree import InfoTree
 
 from .query_utils import append_to_table, drop_table
 from .utils import safezip
 from .table_segment import TableSegment
 from .diff_tables import TableDiffer, DiffResult
```

### Comparing `data_diff-0.7.2/data_diff/lexicographic_space.py` & `data_diff-0.7.3/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.2/data_diff/parse_time.py` & `data_diff-0.7.3/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.2/data_diff/query_utils.py` & `data_diff-0.7.3/data_diff/query_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 "Module for query utilities that didn't make it into the query-builder (yet)"
 
 from contextlib import suppress
 
-from sqeleton.databases import DbPath, QueryError, Oracle
-from sqeleton.queries import table, commit, Expr
+from data_diff.sqeleton.databases import DbPath, QueryError, Oracle
+from data_diff.sqeleton.queries import table, commit, Expr
 
 
 def _drop_table_oracle(name: DbPath):
     t = table(name)
     # Experience shows double drop is necessary
     with suppress(QueryError):
         yield t.drop()
```

### Comparing `data_diff-0.7.2/data_diff/sqeleton/repl.py` & `data_diff-0.7.3/data_diff/sqeleton/repl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import rich.table
 import logging
 
 # logging.basicConfig(level=logging.DEBUG)
 
 from . import connect
-from .queries import table
 
 import sys
 
 
 def print_table(rows, schema, table_name=""):
     # Print rows in a rich table
     t = rich.table.Table(title=table_name, caption=f"{len(rows)} rows")
@@ -23,43 +22,53 @@
     rich.print("Commands:")
     rich.print("  ?mytable - shows schema of table 'mytable'")
     rich.print("  * - shows list of all tables")
     rich.print("  *pattern - shows list of all tables with name like pattern")
     rich.print("Otherwise, runs regular SQL query")
 
 
-def main(uri):
+def repl(uri):
     db = connect(uri)
     db_name = db.name
 
     while True:
-        q = input(f"{db_name}> ").strip()
+        try:
+            q = input(f"{db_name}> ").strip()
+        except EOFError:
+            return
         if not q:
             continue
         if q.startswith("*"):
             pattern = q[1:]
             names = db.query(db.dialect.list_tables(db.default_schema, like=f"%{pattern}%" if pattern else None))
             print_table(names, ["name"], "List of tables")
         elif q.startswith("?"):
             table_name = q[1:]
             if not table_name:
                 help()
                 continue
             try:
-                schema = db.query_table_schema((table_name,))
+                path = db.parse_table_name(table_name)
+                print("->", path)
+                schema = db.query_table_schema(path)
             except Exception as e:
                 logging.error(e)
             else:
                 print_table([(k, v[1]) for k, v in schema.items()], ["name", "type"], f"Table '{table_name}'")
         else:
+            # Normal SQL query
             try:
                 res = db.query(q)
             except Exception as e:
                 logging.error(e)
             else:
                 if res:
-                    print_table(res, [str(i) for i in range(len(res[0]))], q)
+                    print_table(res.rows, res.columns, None)
 
 
-if __name__ == "__main__":
+def main():
     uri = sys.argv[1]
+    return repl(uri)
+
+
+if __name__ == "__main__":
     main()
```

### Comparing `data_diff-0.7.2/data_diff/table_segment.py` & `data_diff-0.7.3/data_diff/table_segment.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from typing import List, Tuple
 import logging
 from itertools import product
 
 from runtype import dataclass
 
 from .utils import safezip, Vector
-from sqeleton.utils import ArithString, split_space
-from sqeleton.databases import Database, DbPath, DbKey, DbTime
-from sqeleton.schema import Schema, create_schema
-from sqeleton.queries import Count, Checksum, SKIP, table, this, Expr, min_, max_, Code
-from sqeleton.queries.extras import ApplyFuncAndNormalizeAsString, NormalizeAsString
+from data_diff.sqeleton.utils import ArithString, split_space
+from data_diff.sqeleton.databases import Database, DbPath, DbKey, DbTime
+from data_diff.sqeleton.schema import Schema, create_schema
+from data_diff.sqeleton.queries import Count, Checksum, SKIP, table, this, Expr, min_, max_, Code
+from data_diff.sqeleton.queries.extras import ApplyFuncAndNormalizeAsString, NormalizeAsString
 
 logger = logging.getLogger("table_segment")
 
 RECOMMENDED_CHECKSUM_DURATION = 20
 
 
 def split_key_space(min_key: DbKey, max_key: DbKey, count: int) -> List[DbKey]:
```

### Comparing `data_diff-0.7.2/data_diff/thread_utils.py` & `data_diff-0.7.3/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.2/data_diff/tracking.py` & `data_diff-0.7.3/data_diff/tracking.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.2/data_diff/utils.py` & `data_diff-0.7.3/data_diff/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.2/pyproject.toml` & `data_diff-0.7.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.7.2"
+version = "0.7.3"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
@@ -28,27 +28,29 @@
 dsnparse = [
     { version = "<0.2.0", markers = "python_version < '3.8.0'" },
     { version = "*", markers = "python_version >= '3.8.0'" }
 ]
 click = "^8.1"
 rich = "*"
 toml = "^0.10.2"
-sqeleton = "0.0.8"
 mysql-connector-python = {version="8.0.29", optional=true}
 psycopg2 = {version="*", optional=true}
 snowflake-connector-python = {version="^2.7.2", optional=true}
 cryptography = {version="*", optional=true}
 trino = {version="^0.314.0", optional=true}
 presto-python-client = {version="*", optional=true}
 clickhouse-driver = {version="*", optional=true}
 duckdb = {version="^0.7.0", optional=true}
 dbt-artifacts-parser = {version="^0.2.5", optional=true}
 dbt-core = {version="^1.0.0", optional=true}
 keyring = "*"
 tabulate = "^0.9.0"
+preql = {version="^0.2.19", optional=true}
+cx_Oracle = {version="*", optional=true}
+vertica-python = {version="*", optional=true}
 
 [tool.poetry.dev-dependencies]
 parameterized = "*"
 unittest-parallel = "*"
 preql = "^0.2.19"
 mysql-connector-python = "*"
 psycopg2 = "*"
@@ -81,10 +83,11 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 data-diff = 'data_diff.__main__:main'
+sqeleton = 'data_diff.sqeleton.__main__:main'
 
 [tool.black]
 line-length = 120
```

### Comparing `data_diff-0.7.2/PKG-INFO` & `data_diff-0.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-diff
-Version: 0.7.2
+Version: 0.7.3
 Summary: Command-line tool and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff
 License: MIT
 Author: Datafold
 Author-email: data-diff@datafold.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -35,30 +35,32 @@
 Provides-Extra: presto
 Provides-Extra: snowflake
 Provides-Extra: trino
 Provides-Extra: vertica
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: clickhouse-driver ; extra == "clickhouse"
 Requires-Dist: cryptography ; extra == "snowflake"
+Requires-Dist: cx_Oracle ; extra == "oracle"
 Requires-Dist: dbt-artifacts-parser (>=0.2.5,<0.3.0) ; extra == "dbt"
 Requires-Dist: dbt-core (>=1.0.0,<2.0.0) ; extra == "dbt"
 Requires-Dist: dsnparse (<0.2.0) ; python_version < "3.8.0"
 Requires-Dist: dsnparse ; python_version >= "3.8.0"
 Requires-Dist: duckdb (>=0.7.0,<0.8.0) ; extra == "duckdb"
 Requires-Dist: keyring
 Requires-Dist: mysql-connector-python (==8.0.29) ; extra == "mysql"
+Requires-Dist: preql (>=0.2.19,<0.3.0) ; extra == "preql"
 Requires-Dist: presto-python-client ; extra == "presto"
 Requires-Dist: psycopg2 ; extra == "postgresql"
 Requires-Dist: rich
 Requires-Dist: runtype (>=0.2.6,<0.3.0)
 Requires-Dist: snowflake-connector-python (>=2.7.2,<3.0.0) ; extra == "snowflake"
-Requires-Dist: sqeleton (==0.0.8)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: trino (>=0.314.0,<0.315.0) ; extra == "trino"
+Requires-Dist: vertica-python ; extra == "vertica"
 Project-URL: Repository, https://github.com/datafold/data-diff
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img alt="Datafold" src="https://user-images.githubusercontent.com/1799931/196497110-d3de1113-a97f-4322-b531-026d859b867a.png" width="50%" />
 </p>
```

