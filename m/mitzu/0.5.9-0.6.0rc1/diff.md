# Comparing `tmp/mitzu-0.5.9.tar.gz` & `tmp/mitzu-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.5.9.tar", max compression
+gzip compressed data, was "mitzu-0.6.0rc1.tar", max compression
```

## Comparing `mitzu-0.5.9.tar` & `mitzu-0.6.0rc1.tar`

### file list

```diff
@@ -1,120 +1,123 @@
--rw-r--r--   0        0        0     1082 2023-03-24 13:47:41.090671 mitzu-0.5.9/LICENSE.txt
--rw-r--r--   0        0        0     7200 2023-03-24 13:47:41.090671 mitzu-0.5.9/README.md
--rw-r--r--   0        0        0     6148 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/.DS_Store
--rw-r--r--   0        0        0      860 2023-03-24 13:48:44.543592 mitzu-0.5.9/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1606 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5234 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6072 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2563 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      723 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     3208 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39380 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     5009 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6687 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1760 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/helper.py
--rw-r--r--   0        0        0    52530 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     5347 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2068 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11435 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     7124 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1367 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7547 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5372 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1261 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-03-24 13:47:41.486677 mitzu-0.5.9/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    10321 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    15067 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1963 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     6202 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2966 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     2349 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     2805 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4833 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8014 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/model.py
--rw-r--r--   0        0        0     2434 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     6444 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0     7561 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/admin_page.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    15549 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4199 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    21143 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9803 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/dashboards.py
--rw-r--r--   0        0        0    15455 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5299 2023-03-24 13:47:41.490677 mitzu-0.5.9/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    16185 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10086 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    11681 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1290 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1401 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1712 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     4123 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     3932 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1319 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0     9839 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    12020 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0    10009 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1733 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35869 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9231 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     4900 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3308 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2065 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     4710 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0     9534 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/storage.py
--rw-r--r--   0        0        0      666 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/toast.py
--rw-r--r--   0        0        0     3248 2023-03-24 13:47:41.494677 mitzu-0.5.9/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     2922 2023-03-24 13:48:44.539592 mitzu-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     9611 1970-01-01 00:00:00.000000 mitzu-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-22 19:42:35.921651 mitzu-0.6.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-04-22 19:42:35.921651 mitzu-0.6.0rc1/README.md
+-rw-r--r--   0        0        0     6148 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/.DS_Store
+-rw-r--r--   0        0        0      865 2023-04-22 19:43:38.102597 mitzu-0.6.0rc1/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1762 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5234 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6072 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2563 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      723 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     4085 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3344 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      660 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-04-22 19:42:36.317656 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0      672 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    39389 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     5009 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     6687 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1760 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/helper.py
+-rw-r--r--   0        0        0    54541 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6818 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     5424 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2086 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11435 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     7124 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1854 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7547 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5372 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3339 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1261 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    10321 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-04-22 19:42:36.321657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    14499 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1963 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7392 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2966 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     2595 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     3382 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4833 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8355 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      408 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     6460 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    15406 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4195 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    21143 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9799 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards.py
+-rw-r--r--   0        0        0    15447 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5299 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    16412 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10152 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    11669 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9783 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1401 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1708 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     4123 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     3928 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1315 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10034 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11710 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0    10013 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1733 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    35869 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9231 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     4901 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3304 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2172 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     5366 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0     2105 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     4710 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    19970 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25909 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0      666 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/toast.py
+-rw-r--r--   0        0        0     4266 2023-04-22 19:42:36.325657 mitzu-0.6.0rc1/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     2965 2023-04-22 19:43:38.098597 mitzu-0.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc1/PKG-INFO
```

### Comparing `mitzu-0.5.9/LICENSE.txt` & `mitzu-0.6.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/.DS_Store` & `mitzu-0.6.0rc1/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/__init__.py` & `mitzu-0.6.0rc1/mitzu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.5.9"
+__version__ = "0.6.0-rc.1"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.5.9/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.0rc1/mitzu/adapters/adapter_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,18 @@
         from mitzu.adapters.mysql_adapter import MySQLAdapter
 
         res = MySQLAdapter(project)
     elif con_type == M.ConnectionType.POSTGRESQL:
         from mitzu.adapters.postgresql_adapter import PostgresqlAdapter
 
         res = PostgresqlAdapter(project)
+    elif con_type == M.ConnectionType.REDSHIFT:
+        from mitzu.adapters.redshift_adapter import RedshiftAdapter
+
+        res = RedshiftAdapter(project)
     elif con_type == M.ConnectionType.TRINO:
         from mitzu.adapters.trino_adapter import TrinoAdapter
 
         res = TrinoAdapter(project)
     elif con_type == M.ConnectionType.DATABRICKS:
         from mitzu.adapters.databricks_adapter import DatabricksAdapter
```

### Comparing `mitzu-0.5.9/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/file_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/helper.py` & `mitzu-0.6.0rc1/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/snowflake_adapter.py`

 * *Files 19% similar despite different names*

```diff
@@ -63,14 +63,17 @@
         df = super()._get_column_values_df(event_data_table, fields, event_specific)
         for field in df.columns:
             df[field] = df[field].apply(
                 lambda val: ast.literal_eval(val) if val is not None else None
             )
         return df
 
+    def _get_distinct_array_agg_func(self, field_ref: FieldReference) -> Any:
+        return SA.func.array_agg(SA.distinct(field_ref))
+
     def _get_conv_aggregation(
         self, metric: M.Metric, cte: EXP.CTE, first_cte: EXP.CTE
     ) -> Any:
         if metric._agg_type == M.AggType.PERCENTILE_TIME_TO_CONV:
             if metric._agg_param is None or 0 < metric._agg_param > 100:
                 raise ValueError(
                     "Conversion percentile parameter must be between 0 and 100"
```

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/__init__.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
         port_str = "" if con.port is None else ":" + str(con.port)
         schema_str = "" if con.schema is None else f"/{con.schema}"
         url_params_str = "" if con.url_params is None else con.url_params
         if url_params_str != "" and url_params_str[0] != "?":
             url_params_str = "?" + url_params_str
         catalog_str = "" if con.catalog is None else f"/{con.catalog}"
 
-        protocol = con.connection_type.value.lower()
+        protocol = con.connection_type.get_protocol().lower()
         res = f"{protocol}://{user_name}{password}{host_str}{port_str}{catalog_str}{schema_str}{url_params_str}"
         return res
 
     def _get_distinct_array_agg_func(self, field_ref: FieldReference) -> Any:
         return SA.func.cast(SA.func.array_agg(SA.distinct(field_ref)), SA.JSON)
 
     def _column_index_support(self):
```

### Comparing `mitzu-0.5.9/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.0rc1/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/helper.py` & `mitzu-0.6.0rc1/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/model.py` & `mitzu-0.6.0rc1/mitzu/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,35 +256,57 @@
 class AttributionMode(Enum):
     FIRST_EVENT = 1
     LAST_EVENT = 2
     ALL_EVENTS = 3
 
 
 class ConnectionType(Enum):
-    FILE = "file"
-    ATHENA = "athena"
-    TRINO = "trino"
-    POSTGRESQL = "postgresql+psycopg2"
-    MYSQL = "mysql+mysqlconnector"
-    SQLITE = "sqlite"
-    DATABRICKS = "databricks"
-    SNOWFLAKE = "snowflake"
+    FILE = auto()
+    ATHENA = auto()
+    TRINO = auto()
+    POSTGRESQL = auto()
+    REDSHIFT = auto()
+    MYSQL = auto()
+    SQLITE = auto()
+    DATABRICKS = auto()
+    SNOWFLAKE = auto()
 
     @classmethod
     def parse(cls, val: str | ConnectionType) -> ConnectionType:
         if type(val) == str:
             val = val.upper()
             return ConnectionType[val]
         elif type(val) == ConnectionType:
             return val
         else:
             raise ValueError(
                 f"Invalid argument type for ConnectionType parse: {type(val)}"
             )
 
+    def get_protocol(self) -> str:
+        if self == ConnectionType.FILE:
+            return "file"
+        if self == ConnectionType.ATHENA:
+            return "athena"
+        if self == ConnectionType.TRINO:
+            return "trino"
+        if self == ConnectionType.POSTGRESQL:
+            return "postgresql+psycopg2"
+        if self == ConnectionType.REDSHIFT:
+            return "postgresql+psycopg2"
+        if self == ConnectionType.MYSQL:
+            return "mysql+mysqlconnector"
+        if self == ConnectionType.SQLITE:
+            return "sqlite"
+        if self == ConnectionType.DATABRICKS:
+            return "databricks"
+        if self == ConnectionType.SNOWFLAKE:
+            return "snowflake"
+        raise ValueError(f"No protocol for: {self}")
+
 
 @dataclass(frozen=True)
 class TimeWindow:
     value: int = 1
     period: TimeGroup = TimeGroup.DAY
 
     @classmethod
@@ -363,20 +385,32 @@
     If the Connection or Project objects are reused we don't want to store them in the DB
     multiple times. The reference protected _id must be the id of the object
     """
 
     _value_state: State[ID]
     _id: Optional[str]
 
-    def __init__(self, value: Optional[ID]):
+    def __init__(self, id: Optional[str], value: Optional[ID]):
         self._value_state = State(value)
-        if value is None:
-            self._id = None
+        self._id = id
+        if id is None:
+            if value is None:
+                raise ValueError("Both id and value are None")
+            else:
+                self._id = value.get_id()
         else:
-            self._id = value.get_id()
+            self._id = id
+
+    @classmethod
+    def create_from_value(cls, value: ID) -> Reference:
+        return Reference(id=value.get_id(), value=value)
+
+    @classmethod
+    def create_from_id(cls, id: str) -> Reference:
+        return Reference(id=id, value=None)
 
     def get_id(self) -> Optional[str]:
         return self._id
 
     def get_value(self) -> Optional[ID]:
         return self._value_state.get_value()
 
@@ -397,15 +431,15 @@
 
     def restore_value(self, value: Optional[ID]):
         if self._id is None:
             raise InvalidReferenceException("Restoring reference without ID.")
         self._value_state.set_value(value)
         if value is not None and value.get_id() != self._id:
             raise InvalidReferenceException(
-                "Restored reference value has different ID."
+                f"Restored reference value has different ID. Original: {self._id}, New: {value.get_id()}"
             )
 
 
 class SecretResolver(ABC):
     """
     Abstract base class for all secret resolvers
     """
@@ -513,14 +547,15 @@
 
     def get_id(self) -> str:
         return self.id
 
 
 @dataclass(frozen=True)
 class DiscoverySettings:
+    id: str = field(default_factory=helper.create_unique_id)
     max_enum_cardinality: int = 300
     max_map_key_cardinality: int = 1000
 
     end_dt: Optional[datetime] = None
     property_sample_rate: int = 0
 
     lookback_days: int = 14
@@ -529,17 +564,33 @@
 
 class WebappEndDateConfig(Enum):
     CUSTOM_DATE = auto()
     NOW = auto()
     START_OF_CURRENT_DAY = auto()
     END_OF_CURRENT_DAY = auto()
 
+    @classmethod
+    def parse(cls, val: str | WebappEndDateConfig) -> WebappEndDateConfig:
+        if type(val) == str:
+            val = val.upper()
+            return WebappEndDateConfig[val]
+        elif type(val) == WebappEndDateConfig:
+            return val
+        else:
+            raise ValueError(
+                f"Invalid argument type for WebappEndDateConfig parse: {type(val)}"
+            )
+
+    def __str__(self) -> str:
+        return self.name.lower()
+
 
 @dataclass(frozen=True)
 class WebappSettings:
+    id: str = field(default_factory=helper.create_unique_id)
     lookback_window: TimeWindow = TimeWindow(30, TimeGroup.DAY)
     auto_refresh_enabled: bool = True
     end_date_config: WebappEndDateConfig = WebappEndDateConfig.START_OF_CURRENT_DAY
     custom_end_date: Optional[datetime] = None
 
 
 class InvalidEventDataTableError(Exception):
@@ -558,28 +609,22 @@
 
     id: str = field(default_factory=helper.create_unique_id)
     schema: Optional[str] = None
     catalog: Optional[str] = None
     event_name_field: Optional[Field] = None
     date_partition_field: Optional[Field] = None
     event_name_alias: Optional[str] = None
-
-    # TBD change to Field type
     ignored_fields: List[Field] = field(default_factory=lambda: [])
-
-    # TBD change to Field type
     event_specific_fields: Optional[List[Field]] = None
 
     # TBD remove
     description: Optional[str] = None
 
     discovery_settings: Optional[DiscoverySettings] = None
-    project_reference: Reference[Project] = field(
-        default_factory=lambda: Reference(None)
-    )
+    project_reference: Optional[Reference[Project]] = None
 
     @classmethod
     def create(
         cls,
         table_name: str,
         event_time_field: Union[str, Field],
         user_id_field: Union[str, Field],
@@ -788,21 +833,25 @@
             if field_to_validate._get_name().lower() not in available_fields:
                 raise InvalidEventDataTableError(
                     f"Event data table '{self.table_name}' does not have '{field_to_validate._get_name()}' field"
                 )
 
     @property
     def project(self) -> Project:
+        if self.project_reference is None:
+            raise InvalidReferenceException(
+                "EventDataTable doesn't have a ProjectReference"
+            )
         res = self.project_reference.get_value()
         if res is None:
             raise InvalidReferenceException("EventDataTable doesn't have a Project")
         return res
 
     def set_project(self, project: Project):
-        self.project_reference = Reference(project)
+        self.project_reference = Reference.create_from_value(project)
 
 
 class InvalidProjectError(Exception):
     pass
 
 
 @dataclass(init=False)
@@ -832,14 +881,17 @@
         event_data_tables: List[EventDataTable],
         project_name: str,
         project_id: Optional[str] = None,
         description: Optional[str] = None,
         discovery_settings: Optional[DiscoverySettings] = None,
         webapp_settings: Optional[WebappSettings] = None,
     ):
+        if project_id is None:
+            project_id = helper.create_unique_id()
+
         object.__setattr__(self, "id", project_id)
         edt_with_discovery_settings = []
         if discovery_settings is None:
             discovery_settings = DiscoverySettings()
         for edt in event_data_tables:
             edt.set_project(self)
             if edt.discovery_settings is None:
@@ -848,23 +900,22 @@
                 )
             else:
                 edt_with_discovery_settings.append(edt)
 
         if webapp_settings is None:
             webapp_settings = WebappSettings()
 
-        if project_id is None:
-            project_id = helper.create_unique_id()
-
         object.__setattr__(self, "event_data_tables", edt_with_discovery_settings)
         object.__setattr__(self, "discovery_settings", discovery_settings)
         object.__setattr__(self, "webapp_settings", webapp_settings)
         object.__setattr__(self, "project_name", project_name)
         object.__setattr__(self, "description", description)
-        object.__setattr__(self, "_connection_ref", Reference(connection))
+        object.__setattr__(
+            self, "_connection_ref", Reference.create_from_value(connection)
+        )
         object.__setattr__(self, "_adapter_cache", State())
         object.__setattr__(self, "_discovered_project", State())
 
     def get_adapter(self) -> GA.GenericDatasetAdapter:
         val = self._adapter_cache.get_value()
         if val is None:
             adp = factory.create_adapter(self)
@@ -1034,21 +1085,23 @@
     )
 
     def __init__(
         self,
         _name: str,
         _type: DataType,
         _sub_fields: Optional[Tuple[Field, ...]] = None,
+        _parent: Optional[Field] = None,
     ):
         object.__setattr__(self, "_name", _name)
         object.__setattr__(self, "_type", _type)
         object.__setattr__(self, "_sub_fields", _sub_fields)
         if _sub_fields is not None:
             for sf in _sub_fields:
                 object.__setattr__(sf, "_parent", self)
+        object.__setattr__(self, "_parent", _parent)
 
     def has_sub_field(self, field: Field) -> bool:
         if self._sub_fields is None:
             return False
         curr = field
         while curr._parent is not None:
             curr = curr._parent
@@ -1085,25 +1138,27 @@
     @property
     def _project(self) -> Project:
         return self._event_data_table.project
 
 
 @dataclass(frozen=True)
 class EventDef(Identifiable):
+
     _event_name: str
     _fields: Dict[Field, EventFieldDef]
     _event_data_table: EventDataTable
     _description: Optional[str] = ""
+    _id: str = field(default_factory=helper.create_unique_id)
 
     @property
     def _project(self) -> Project:
         return self._event_data_table.project
 
     def get_id(self) -> str:
-        return self._event_data_table.id + f"_{self._event_name}"
+        return self._id
 
 
 # =========================================== Metric definitions ===========================================
 
 DEF_MAX_GROUP_COUNT = 10
 DEF_LOOK_BACK_DAYS = TimeWindow(30, TimeGroup.DAY)
 DEF_CONV_WINDOW = TimeWindow(1, TimeGroup.DAY)
```

### Comparing `mitzu-0.5.9/mitzu/notebook/model_loader.py` & `mitzu-0.6.0rc1/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/project_discovery.py` & `mitzu-0.6.0rc1/mitzu/project_discovery.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             }
 
             new_def = M.EventDef(
                 _event_data_table=event_data_table,
                 _event_name=evt_name,
                 _fields={**spec_evt_def._fields, **copied_gen_fields},
             )
-            res[evt_name] = M.Reference(new_def)
+            res[evt_name] = M.Reference.create_from_value(new_def)
 
         return res
 
     def discover_project(self, progress_bar: bool = False) -> M.DiscoveredProject:
         definitions: Dict[M.EventDataTable, Dict[str, M.Reference[M.EventDef]]] = {}
 
         self.project.validate()
@@ -113,18 +113,22 @@
                 specific_fields = self._get_specific_fields(ed_table, fields)
 
                 generic_fields = [c for c in fields if c not in specific_fields]
                 generic_field_values = self._get_field_values(
                     ed_table, generic_fields, False
                 )
                 if M.ANY_EVENT_NAME not in generic_field_values.keys():
-                    raise ProjectDiscoveryError(
-                        f"Can't find any data to determine the generic field values in table '{ed_table.table_name}'"
+                    any_event_field_values = M.EventDef(
+                        _event_name=M.ANY_EVENT_NAME,
+                        _fields={},
+                        _event_data_table=ed_table,
                     )
-                any_event_field_values = generic_field_values[M.ANY_EVENT_NAME]
+                else:
+                    any_event_field_values = generic_field_values[M.ANY_EVENT_NAME]
+
                 event_specific_field_values = self._get_field_values(
                     ed_table, specific_fields, True
                 )
                 defs = self._merge_generic_and_specific_definitions(
                     ed_table,
                     any_event_field_values,
                     event_specific_field_values,
```

### Comparing `mitzu-0.5.9/mitzu/project_serialization.py` & `mitzu-0.6.0rc1/mitzu/project_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,11 +61,11 @@
         edt.set_project(project)
     project.set_connection(res[CONNECTION])
 
     definitions = {}
     for edt, defs in res[DEFS].items():
         edt_def: Dict[str, M.Reference[M.EventDef]] = {}
         for evt_name, evt_def in defs.items():
-            edt_def[evt_name] = M.Reference(evt_def)
+            edt_def[evt_name] = M.Reference.create_from_value(evt_def)
         definitions[edt] = edt_def
 
     return M.DiscoveredProject(definitions=definitions, project=project)
```

### Comparing `mitzu-0.5.9/mitzu/samples/__init__.py` & `mitzu-0.6.0rc1/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/samples/data_ingestion.py` & `mitzu-0.6.0rc1/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.0rc1/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/serialization.py` & `mitzu-0.6.0rc1/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/visualization/charts.py` & `mitzu-0.6.0rc1/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/visualization/common.py` & `mitzu-0.6.0rc1/mitzu/visualization/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,7 +47,23 @@
     yaxis_ticksuffix: str
     hover_mode: str
     chart_type: M.SimpleChartType
     dataframe: pd.DataFrame
     x_axis_labels_func: Optional[Callable[[Any, M.Metric], Any]] = None
     y_axis_labels_func: Optional[Callable[[Any, M.Metric], Any]] = None
     color_labels_func: Optional[Callable[[Any, M.Metric], Any]] = None
+
+    def __eq__(self, value: object) -> bool:
+        if not isinstance(value, SimpleChart):
+            return False
+
+        value_dict = value.__dict__
+        for key, value in self.__dict__.items():
+            if key not in [
+                "dataframe",
+                "x_axis_labels_func",
+                "y_axis_labels_func",
+                "color_labels_func",
+            ]:
+                if value != value_dict[key]:
+                    return False
+        return True
```

### Comparing `mitzu-0.5.9/mitzu/visualization/labels.py` & `mitzu-0.6.0rc1/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/visualization/plot.py` & `mitzu-0.6.0rc1/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/visualization/titles.py` & `mitzu-0.6.0rc1/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/visualization/tooltips.py` & `mitzu-0.6.0rc1/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/visualization/transform_conv.py` & `mitzu-0.6.0rc1/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/visualization/transform_retention.py` & `mitzu-0.6.0rc1/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/.DS_Store` & `mitzu-0.6.0rc1/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.0rc1/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.0rc1/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/logo.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.0rc1/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.0rc1/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.0rc1/mitzu/webapp/auth/authorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,121 +239,111 @@
                 return None
 
             return user_email
         except Exception as e:
             LOGGER.warning(f"Failed to validate token: {str(e)}")
             return None
 
-    def setup_authorizer(self, server: flask.Flask):
-        @server.before_request
-        def authorize_request():
-            request = flask.request
+    def authorize_request(
+        self, request: flask.Request
+    ) -> Optional[werkzeug.wrappers.response.Response]:
+        if self._config.oauth and request.path == P.REDIRECT_TO_LOGIN_URL:
+            resp = self._redirect(self._config.oauth.sign_in_url)
+            return resp
 
-            if self._config.oauth and request.path == P.REDIRECT_TO_LOGIN_URL:
-                resp = self._redirect(self._config.oauth.sign_in_url)
-                return resp
+        if self._config.oauth and request.path == P.OAUTH_CODE_URL:
+            code = self._get_oauth_code()
+            if code is not None:
+                LOGGER.debug(f"Redirected with code={code}")
+                try:
+                    id_token = self._get_identity_token(code)
+                    redirect_url = flask.request.cookies.get(
+                        self._config.redirect_cookie_name, MITZU_WEBAPP_URL
+                    )
 
-            if self._config.oauth and request.path == P.OAUTH_CODE_URL:
-                code = self._get_oauth_code()
-                if code is not None:
-                    LOGGER.debug(f"Redirected with code={code}")
-                    try:
-                        id_token = self._get_identity_token(code)
-                        redirect_url = flask.request.cookies.get(
-                            self._config.redirect_cookie_name, MITZU_WEBAPP_URL
+                    user_email = self._validate_foreign_token(id_token)
+                    if not user_email:
+                        raise Exception("Unauthorized (Invalid jwt token)")
+
+                    if (
+                        self._config.allowed_email_domain is not None
+                        and not user_email.endswith(self._config.allowed_email_domain)
+                    ):
+                        raise Exception(
+                            f"User tried to login with not allowed email address: {user_email}"
                         )
 
-                        user_email = self._validate_foreign_token(id_token)
-                        if not user_email:
-                            raise Exception("Unauthorized (Invalid jwt token)")
-
-                        if (
-                            self._config.allowed_email_domain is not None
-                            and not user_email.endswith(
-                                self._config.allowed_email_domain
-                            )
-                        ):
+                    user_role = WM.Role.MEMBER
+                    token_identity = user_email
+                    if (
+                        configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS
+                        and self._config.user_service is not None
+                    ):
+                        user = self._config.user_service.get_user_by_email(user_email)
+                        if user is None:
                             raise Exception(
-                                f"User tried to login with not allowed email address: {user_email}"
-                            )
-
-                        user_role = WM.Role.MEMBER
-                        token_identity = user_email
-                        if (
-                            configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS
-                            and self._config.user_service is not None
-                        ):
-                            user = self._config.user_service.get_user_by_email(
-                                user_email
+                                f"User tried to login without having a local user: {user_email}"
                             )
-                            if user is None:
-                                raise Exception(
-                                    f"User tried to login without having a local user: {user_email}"
-                                )
-                            user_role = user.role
-                            token_identity = user.id
+                        user_role = user.role
+                        token_identity = user.id
 
-                        token = self._generate_new_token_for_identity(
-                            token_identity, role=user_role
-                        )
+                    token = self._generate_new_token_for_identity(
+                        token_identity, role=user_role
+                    )
 
-                        resp = self._redirect(redirect_url)
-                        resp.set_cookie(self._config.token_cookie_name, token)
-                        resp.set_cookie(
-                            self._config.redirect_cookie_name, "", expires=0
-                        )
+                    resp = self._redirect(redirect_url)
+                    resp.set_cookie(self._config.token_cookie_name, token)
+                    resp.set_cookie(self._config.redirect_cookie_name, "", expires=0)
+                    return resp
+                except Exception as exc:
+                    traceback.print_exception(type(exc), exc, exc.__traceback__)
+                    LOGGER.warning(f"Failed to authenticate: {str(exc)}")
+                    if self._config.oauth and self._config.oauth.sign_out_url:
+                        resp = self._redirect(self._config.oauth.sign_out_url)
+                        resp.set_cookie(self._config.token_cookie_name, "", expires=0)
                         return resp
-                    except Exception as exc:
-                        traceback.print_exception(type(exc), exc, exc.__traceback__)
-                        LOGGER.warning(f"Failed to authenticate: {str(exc)}")
-                        if self._config.oauth and self._config.oauth.sign_out_url:
-                            resp = self._redirect(self._config.oauth.sign_out_url)
-                            resp.set_cookie(
-                                self._config.token_cookie_name, "", expires=0
-                            )
-                            return resp
-                        return self._get_unauthenticated_response()
-
-            auth_token = flask.request.cookies.get(self._config.token_cookie_name)
+                    return self._get_unauthenticated_response()
 
-            if request.path == P.SIGN_OUT_URL:
-                if self._config.oauth and self._config.oauth.sign_out_url:
-                    resp = self._redirect(self._config.oauth.sign_out_url)
-                    resp.set_cookie(self._config.token_cookie_name, "", expires=0)
-                    return resp
-                return self._get_unauthenticated_response()
+        auth_token = flask.request.cookies.get(self._config.token_cookie_name)
 
-            for prefix in self._authorized_url_prefixes:
-                if request.path.startswith(prefix):
-                    return None
+        if request.path == P.SIGN_OUT_URL:
+            if self._config.oauth and self._config.oauth.sign_out_url:
+                resp = self._redirect(self._config.oauth.sign_out_url)
+                resp.set_cookie(self._config.token_cookie_name, "", expires=0)
+                return resp
+            return self._get_unauthenticated_response()
 
-            if auth_token and self._validate_token(auth_token) is not None:
+        for prefix in self._authorized_url_prefixes:
+            if request.path.startswith(prefix):
                 return None
 
-            redirect_url = request.path
-            if len(request.query_string) > 0:
-                redirect_url += "?" + request.query_string.decode("utf-8")
-            return self._get_unauthenticated_response(redirect_url)
-
-        @server.after_request
-        def after_request(resp: flask.Response):
-            request = flask.request
-            for prefix in self._ignore_token_refresh_prefixes:
-                if request.path.startswith(prefix):
-                    return resp
+        if auth_token and self._validate_token(auth_token) is not None:
+            return None
 
-            auth_token = flask.request.cookies.get(self._config.token_cookie_name)
-            if auth_token is not None:
-                identity = self._validate_token(auth_token)
-                if identity is not None:
-                    new_token = self._generate_new_token_for_identity(
-                        identity["sub"], role=identity[JWT_CLAIM_ROLE]
-                    )
-                    resp.set_cookie(self._config.token_cookie_name, new_token)
-            return resp
+        redirect_url = request.path
+        if len(request.query_string) > 0:
+            redirect_url += "?" + request.query_string.decode("utf-8")
+        return self._get_unauthenticated_response(redirect_url)
+
+    def refresh_auth_token(
+        self, request: flask.Request, resp: flask.Response
+    ) -> werkzeug.wrappers.response.Response:
+        for prefix in self._ignore_token_refresh_prefixes:
+            if request.path.startswith(prefix):
+                return resp
+
+        auth_token = flask.request.cookies.get(self._config.token_cookie_name)
+        if auth_token is not None:
+            identity = self._validate_token(auth_token)
+            if identity is not None:
+                new_token = self._generate_new_token_for_identity(
+                    identity["sub"], role=identity[JWT_CLAIM_ROLE]
+                )
+                resp.set_cookie(self._config.token_cookie_name, new_token)
+        return resp
 
     def is_request_authorized(self, request: flask.Request) -> bool:
         auth_token = request.cookies.get(self._config.token_cookie_name)
         return auth_token is not None and self._validate_token(auth_token) is not None
 
     def get_current_user_role(self, request: flask.Request) -> Optional[WM.Role]:
         auth_token = request.cookies.get(self._config.token_cookie_name)
```

### Comparing `mitzu-0.5.9/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.0rc1/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.0rc1/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/auth/google.py` & `mitzu-0.6.0rc1/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/cache.py` & `mitzu-0.6.0rc1/mitzu/webapp/cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,51 +39,70 @@
         raise NotImplementedError()
 
 
 @dataclass(frozen=True, init=False)
 class DiskMitzuCache(MitzuCache):
 
     _disk_cache: diskcache.Cache
+    _global_prefix: Optional[str] = None
 
-    def __init__(self, name: str) -> None:
+    def __init__(self, name: str, global_prefix: Optional[str] = None) -> None:
         super().__init__()
         object.__setattr__(
             self,
             "_disk_cache",
             diskcache.Cache(timeout=10, directory=f"{configs.DISK_CACHE_PATH}/{name}"),
         )
+        object.__setattr__(
+            self,
+            "_global_prefix",
+            global_prefix,
+        )
 
     def __post_init__(self):
         H.LOGGER.info("Vacuuming disk cache")
         self._disk_cache._sql("vacuum")
 
+    def _get_key(self, key: str) -> str:
+        if self._global_prefix:
+            return f"{self._global_prefix}.{key}"
+        return key
+
     def put(self, key: str, val: Any, expire: Optional[float] = None):
+        key = self._get_key(key)
         self.clear(key)
         if val is not None:
             H.LOGGER.debug(f"PUT: {key}: {type(val)}")
             self._disk_cache.add(key, value=val, expire=expire)
         else:
             H.LOGGER.debug(f"PUT: {key}: None")
 
     def get(self, key: str, default: Optional[Any] = None) -> Any:
+        key = self._get_key(key)
         res = self._disk_cache.get(key)
         if res is not None:
             H.LOGGER.debug(f"GET: {key}: {type(res)}")
             return res
         else:
             H.LOGGER.debug(f"GET: {key}: None")
             return default
 
     def clear(self, key: str) -> None:
+        key = self._get_key(key)
         H.LOGGER.debug(f"Clear {key}")
         self._disk_cache.pop(key)
 
     def list_keys(
         self, prefix: Optional[str] = None, strip_prefix: bool = True
     ) -> List[str]:
+        if prefix is None:
+            prefix = self._global_prefix
+        else:
+            prefix = self._get_key(prefix)
+
         keys = self._disk_cache.iterkeys()
         start_pos = len(prefix) if strip_prefix and prefix is not None else 0
         res = [k[start_pos:] for k in keys if prefix is None or k.startswith(prefix)]
         if H.LOGGER.getEffectiveLevel() == H.logging.DEBUG:
             H.LOGGER.debug(f"LIST {prefix}: {res}")
         return res
 
@@ -132,62 +151,81 @@
     pass
 
 
 @dataclass(init=False, frozen=True)
 class RedisMitzuCache(MitzuCache):
 
     _redis: redis.Redis
+    _global_prefix: Optional[str] = None
 
-    def __init__(self, redis_cache: Optional[redis.Redis] = None) -> None:
+    def __init__(
+        self,
+        redis_cache: Optional[redis.Redis] = None,
+        global_prefix: Optional[str] = None,
+    ) -> None:
         super().__init__()
 
         if redis_cache is not None:
             object.__setattr__(self, "_redis", redis_cache)
+            object.__setattr__(self, "_global_prefix", global_prefix)
         else:
             if configs.STORAGE_REDIS_HOST is None:
                 raise ValueError(
                     "STORAGE_REDIS_HOST env variable is not set, can't create redis cache."
                 )
             object.__setattr__(
                 self,
                 "_redis",
                 redis.Redis(
                     host=configs.STORAGE_REDIS_HOST,
                     port=configs.STORAGE_REDIS_PORT,
                     password=configs.STORAGE_REDIS_PASSWORD,
                 ),
             )
+            object.__setattr__(self, "_global_prefix", global_prefix)
+
+    def _get_key(self, key: str) -> str:
+        if self._global_prefix:
+            return f"{self._global_prefix}.{key}"
+        return key
 
     def put(self, key: str, val: Any, expire: Optional[float] = None):
+        key = self._get_key(key)
         pickled_value = pickle.dumps(val)
         if H.LOGGER.getEffectiveLevel() == H.logging.DEBUG:
             H.LOGGER.debug(f"PUT: {key}: {len(pickled_value)}")
         res = self._redis.set(name=key, value=pickled_value, ex=expire)
         if not res:
             raise RedisException(f"Couldn't set {key}")
 
     def get(self, key: str, default: Optional[Any] = None) -> Any:
+        key = self._get_key(key)
         res = self._redis.get(name=key)
         if res is None:
             H.LOGGER.debug(f"GET: {key}: None")
             if default is not None:
                 return default
             return None
         if H.LOGGER.getEffectiveLevel() == H.logging.DEBUG:
             H.LOGGER.debug(f"GET: {key}: {len(res)}")
         return pickle.loads(res)
 
     def clear(self, key: str) -> None:
+        key = self._get_key(key)
         H.LOGGER.debug(f"CLEAR: {key}")
         self._redis.delete(key)
 
     def list_keys(
         self, prefix: Optional[str] = None, strip_prefix: bool = True
     ) -> List[str]:
-        if not prefix:
+        if prefix:
+            prefix = self._get_key(prefix)
+        elif self._global_prefix is not None:
+            prefix = self._global_prefix
+        else:
             prefix = ""
         keys = self._redis.keys(f"{prefix}*")
         start_pos = len(prefix) if strip_prefix else 0
         res = [k.decode()[start_pos:] for k in keys]
         if H.LOGGER.getEffectiveLevel() == H.logging.DEBUG:
             H.LOGGER.debug(f"LIST prefix={prefix}: {res}")
         return res
```

### Comparing `mitzu-0.5.9/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.0rc1/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/configs.py` & `mitzu-0.6.0rc1/mitzu/webapp/configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 AUTH_SSO_ONLY_FOR_LOCAL_USERS = bool(os.getenv("AUTH_SSO_ONLY_FOR_LOCAL_USERS", False))
 AUTH_ROOT_PASSWORD = os.getenv("AUTH_ROOT_PASSWORD", "test")
 AUTH_ROOT_USER_EMAIL = os.getenv("AUTH_ROOT_USER_EMAIL", "root@local")
 
 
 # cache
 CACHE_EXPIRATION = int(os.getenv("CACHE_EXPIRATION", "600"))
+CACHE_PREFIX = os.getenv("CACHE_PREFIX")
 
 # redis cache
 QUEUE_REDIS_HOST = os.getenv("QUEUE_REDIS_HOST")
 QUEUE_REDIS_PORT = int(os.getenv("QUEUE_REDIS_PORT", 6379))
 QUEUE_REDIS_DB = os.getenv("STORAGE_REDIS_DB")
 QUEUE_REDIS_USERNAME = os.getenv("QUEUE_REDIS_USERNAME")
 QUEUE_REDIS_PASSWORD = os.getenv("QUEUE_REDIS_PASSWORD")
@@ -50,14 +51,20 @@
 DISK_CACHE_PATH = os.getenv("DISK_CACHE_PATH", "./storage")
 
 # storage
 SETUP_SAMPLE_PROJECT = bool(
     os.getenv("SETUP_SAMPLE_PROJECT", "false").lower() != "false"
 )
 
+SECRET_ENCRYPTION_KEY = os.getenv("SECRET_ENCRYPTION_KEY", None)
+STORAGE_CONNECTION_STRING = os.getenv(
+    "STORAGE_CONNECTION_STRING",
+    "sqlite:///storage.db?cache=shared&check_same_thread=False",
+)
+
 
 KALEIDO_CONFIGS = os.getenv("KALEIDO_CONFIGS", "--disable-gpu-*,--single-process")
 
 
 def get_kaleido_configs() -> Optional[Tuple[str, ...]]:
     if KALEIDO_CONFIGS:
         return tuple(KALEIDO_CONFIGS.split(","))
```

### Comparing `mitzu-0.5.9/mitzu/webapp/dependencies.py` & `mitzu-0.6.0rc1/mitzu/webapp/dependencies.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,68 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
 
-from flask import Flask
 
 import mitzu.webapp.auth.authorizer as A
 import mitzu.webapp.cache as C
 import mitzu.webapp.configs as configs
 import mitzu.webapp.storage as S
 import mitzu.webapp.service.user_service as U
+import mitzu.webapp.service.navbar_service as NB
 import mitzu.webapp.service.events_service as E
+import mitzu.webapp.service.secret_service as SS
 
 CONFIG_KEY = "dependencies"
 
 
 @dataclass(frozen=True)
 class Dependencies:
 
     authorizer: Optional[A.OAuthAuthorizer]
     storage: S.MitzuStorage
     queue: C.MitzuCache
     cache: C.MitzuCache
     events_service: E.EventsService
+    navbar_service: NB.NavbarService
+    secret_service: SS.SecretService
     user_service: Optional[U.UserService] = None
 
     @classmethod
-    def from_configs(cls, server: Flask) -> Dependencies:
+    def from_configs(cls) -> Dependencies:
         delegate_cache: C.MitzuCache
         if configs.STORAGE_REDIS_HOST is not None:
-            delegate_cache = C.RedisMitzuCache()
+            delegate_cache = C.RedisMitzuCache(global_prefix=configs.CACHE_PREFIX)
         else:
-            delegate_cache = C.DiskMitzuCache("cache")
+            delegate_cache = C.DiskMitzuCache(
+                "cache", global_prefix=configs.CACHE_PREFIX
+            )
         cache = C.RequestCache(delegate_cache)
-        storage = S.MitzuStorage(cache)
+        storage = S.MitzuStorage(connection_string=configs.STORAGE_CONNECTION_STRING)
 
         authorizer = None
         oauth_config = None
         user_service = None
+        create_user_service = False
         if configs.AUTH_BACKEND == "cognito":
             from mitzu.webapp.auth.cognito import Cognito
 
             oauth_config = Cognito.get_config()
+            create_user_service = configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS
         elif configs.AUTH_BACKEND == "google":
             from mitzu.webapp.auth.google import GoogleOAuth
 
             oauth_config = GoogleOAuth.get_config()
+            create_user_service = configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS
+
+        elif configs.AUTH_BACKEND == "local":
+            create_user_service = True
 
-        elif configs.AUTH_BACKEND == "local" or configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
+        if create_user_service:
             user_service = U.UserService(
                 storage, root_password=configs.AUTH_ROOT_PASSWORD
             )
 
         if oauth_config or user_service:
             auth_config = A.AuthConfig(
                 oauth=oauth_config,
@@ -62,26 +73,29 @@
                 else None,
                 allowed_email_domain=configs.AUTH_ALLOWED_EMAIL_DOMAIN,
                 token_signing_key=configs.AUTH_JWT_SECRET,
                 session_timeout=configs.AUTH_SESSION_TIMEOUT,
                 user_service=user_service,
             )
             authorizer = A.OAuthAuthorizer.create(auth_config)
-            authorizer.setup_authorizer(server)
 
         queue: C.MitzuCache
         if configs.QUEUE_REDIS_HOST is not None:
             queue = C.RedisMitzuCache()
         else:
             queue = C.DiskMitzuCache("queue")
 
         # Adding cache layer over storage
         events_service = E.EventsService(storage)
 
+        secret_service = SS.SecretService()
+
         return Dependencies(
             authorizer=authorizer,
             cache=cache,
             storage=storage,
             queue=queue,
             user_service=user_service,
+            navbar_service=NB.NavbarService(),
             events_service=events_service,
+            secret_service=secret_service,
         )
```

### Comparing `mitzu-0.5.9/mitzu/webapp/helper.py` & `mitzu-0.6.0rc1/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/model.py` & `mitzu-0.6.0rc1/mitzu/webapp/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,39 +49,43 @@
         project: M.Project,
         metric_json: Optional[str] = None,
         metric: Optional[M.Metric] = None,
         owner: Optional[str] = None,
         description: Optional[str] = None,
         created_at: Optional[datetime] = None,
         id: Optional[str] = None,
+        last_updated_at: Optional[datetime] = None,
     ):
         if created_at is None:
             created_at = datetime.now()
 
         if metric_json is None:
             if metric is not None:
                 metric_json = SE.to_compressed_string(metric)
             else:
                 raise ValueError(
                     "Either metric or metric_json needs to be defined as an argument"
                 )
 
         if id is None:
             id = create_unique_id()
+
+        if last_updated_at is None:
+            last_updated_at = datetime.now()
         object.__setattr__(self, "chart", chart)
         object.__setattr__(self, "name", name)
         object.__setattr__(self, "description", description if description else "")
         object.__setattr__(self, "image_base64", image_base64)
         object.__setattr__(self, "small_base64", small_base64)
         object.__setattr__(self, "created_at", created_at)
-        object.__setattr__(self, "last_updated_at", datetime.now())
+        object.__setattr__(self, "last_updated_at", last_updated_at)
         object.__setattr__(self, "metric_json", metric_json)
         object.__setattr__(self, "owner", owner)
         object.__setattr__(self, "id", id)
-        object.__setattr__(self, "_project_ref", M.Reference(project))
+        object.__setattr__(self, "_project_ref", M.Reference.create_from_value(project))
         object.__setattr__(self, "_metric_state", M.State(metric))
 
     @property
     def project(self) -> Optional[M.Project]:
         return self._project_ref.get_value()
 
     @property
@@ -163,28 +167,35 @@
     """
 
     x: int
     y: int
     width: int
     height: int
     _saved_metric_ref: M.Reference[SavedMetric]
+    id: str
 
     def __init__(
         self,
         saved_metric: SavedMetric,
         x: int = 0,
         y: int = 0,
         width: int = 2,
         height: int = 8,
+        id: Optional[str] = None,
     ):
+        if id is None:
+            id = str(uuid4())[-12:]
+        object.__setattr__(self, "id", id)
         object.__setattr__(self, "x", x)
         object.__setattr__(self, "y", y)
         object.__setattr__(self, "width", width)
         object.__setattr__(self, "height", height)
-        object.__setattr__(self, "_saved_metric_ref", M.Reference(saved_metric))
+        object.__setattr__(
+            self, "_saved_metric_ref", M.Reference.create_from_value(saved_metric)
+        )
 
     @property
     def saved_metric(self) -> Optional[SavedMetric]:
         return self._saved_metric_ref.get_value()
 
     def restore_saved_metric(self, saved_metric: SavedMetric):
         self._saved_metric_ref.restore_value(saved_metric)
```

### Comparing `mitzu-0.5.9/mitzu/webapp/offcanvas.py` & `mitzu-0.6.0rc1/mitzu/webapp/offcanvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import dash_bootstrap_components as dbc
 from dash import callback, ctx, html, dcc
 from dash.dependencies import ALL, Input, Output
 from mitzu import __version__ as version
 
 import mitzu.webapp.configs as configs
 import mitzu.webapp.dependencies as DEPS
-import mitzu.webapp.navbar as NB
+import mitzu.webapp.service.navbar_service as NB
 import mitzu.webapp.pages.paths as P
 from mitzu.webapp.auth.decorator import restricted
 
 OFF_CANVAS = "off-canvas-id"
 BUTTON_COLOR = "light"
 
 CLOSE_BUTTON = "close-button"
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import dash_bootstrap_components as dbc
 import dash_mantine_components as dmc
 from dash import Input, Output, State, callback, ctx, html, no_update, ALL, dcc
 
 import mitzu.model as M
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.pages.paths as P
-import mitzu.webapp.configs as CO
 from mitzu.helper import value_to_label
 from mitzu.webapp.auth.decorator import restricted
 from mitzu.webapp.helper import MITZU_LOCATION, create_form_property_input
 import traceback
 
 EXTRA_PROPERTY_CONTAINER = "extra_property_container"
 CONNECTION_DELETE_BUTTON = "connection_delete_button"
@@ -39,26 +38,30 @@
 PROP_ROLE = "role"
 PROP_HTTP_PATH = "http_path"
 PROP_PORT = "port"
 PROP_HOST = "host"
 PROP_USERNAME = "username"
 PROP_PASSWORD = "password"
 NOT_REQUIRED_PROPERTIES = [PROP_CATALOG, PROP_PORT, PROP_PASSWORD, PROP_USERNAME]
-CON_TYPE_BLACKLIST = [M.ConnectionType.FILE, M.ConnectionType.SQLITE]
+CON_TYPE_BLACKLIST = [M.ConnectionType.FILE]
 
 
 MIN_LENGTH = 4
 MAX_LENGTH = 100
 
 
 def create_url_param(values: Dict[str, Any], property: str) -> str:
     return f"{property}={values[property]}"
 
 
 def create_connection_from_values(values: Dict[str, Any]) -> M.Connection:
+    deps: DEPS.Dependencies = cast(
+        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
+    )
+
     con_type = M.ConnectionType.parse(values[PROP_CONNECTION_TYPE])
     url_params = ""
     extra_configs = {}
     if con_type == M.ConnectionType.ATHENA:
         url_params = "&".join(
             [
                 create_url_param(values, PROP_S3_STAGING_DIR),
@@ -78,15 +81,15 @@
         connection_name=values[PROP_CONNECTION_NAME],
         connection_type=con_type,
         host=values[PROP_HOST],
         port=values[PROP_PORT],
         id=values[PROP_CONNECTION_ID],
         catalog=values[PROP_CATALOG],
         user_name=values[PROP_USERNAME],
-        secret_resolver=M.ConstSecretResolver(values[PROP_PASSWORD]),
+        secret_resolver=deps.secret_service.get_secret_resolver(values[PROP_PASSWORD]),
         url_params=url_params,
         extra_configs=extra_configs,
     )
 
 
 def create_connection_extra_inputs(
     con_type: Optional[M.ConnectionType], con: Optional[M.Connection]
@@ -201,21 +204,14 @@
     con: Optional[M.Connection],
 ) -> bc.Component:
     con_type_opts = [
         {"label": ct.name.title(), "value": ct.name}
         for ct in M.ConnectionType
         if ct not in CON_TYPE_BLACKLIST
     ]
-    if CO.SETUP_SAMPLE_PROJECT:
-        con_type_opts.append(
-            {
-                "label": M.ConnectionType.SQLITE.name.title(),
-                "value": M.ConnectionType.SQLITE.name,
-            }
-        )
     def_con_type = M.ConnectionType.SNOWFLAKE
     return html.Div(
         [
             html.Div(
                 create_form_property_input(
                     index_type=INDEX_TYPE,
                     property=PROP_CONNECTION_ID,
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/connections_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     connections: List[M.Connection] = []
     for con_id in connection_ids:
         con = depenednecies.storage.get_connection(con_id)
         connections.append(con)
 
     return html.Div(
         [
-            NB.create_mitzu_navbar("explore-navbar", []),
+            NB.create_mitzu_navbar("explore-navbar"),
             dbc.Container(
                 children=[
                     html.H4("Choose from connections:", className="card-title"),
                     html.Hr(),
                     create_connections_container(connections),
                     html.Hr(),
                     dbc.Row(
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/dashboards.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/dashboards.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
     ).storage
     d_ids = storage.list_dashboards()
     dashboards = [storage.get_dashboard(d_id) for d_id in d_ids]
 
     return html.Div(
         [
-            NB.create_mitzu_navbar("dashboard-navbar", []),
+            NB.create_mitzu_navbar("dashboard-navbar"),
             dbc.Container(
                 children=[
                     dbc.Row(
                         [
                             dbc.Col(
                                 html.H4("Select a Dashboard", className="card-title"),
                                 width="auto",
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/edit_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         )
     else:
         user = None
 
     if user is None and user_id != "new":
         return html.Div(
             [
-                NB.create_mitzu_navbar("users_edit", []),
+                NB.create_mitzu_navbar("users_edit"),
                 dbc.Container(
                     [
                         html.H4("Users not found"),
                         html.Hr(),
                         dbc.Button(
                             [html.B(className="bi bi-x"), " Close"],
                             color="secondary",
@@ -101,15 +101,15 @@
                     ]
                 ),
             ]
         )
 
     return html.Div(
         [
-            NB.create_mitzu_navbar("users_management_page", []),
+            NB.create_mitzu_navbar("users_management_page"),
             dbc.Container(
                 [
                     html.H4("User"),
                     html.Hr(),
                     create_form_property_input(
                         index_type=INDEX_TYPE,
                         property=PROP_EMAIL,
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/explore_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,37 +75,52 @@
         TH.CHART_TYPE_DD: Input(TH.CHART_TYPE_DD, "value"),
         TH.GRAPH_CONTENT_TYPE: Input(TH.GRAPH_CONTENT_TYPE, "value"),
         MTH.METRIC_TYPE_DROPDOWN: Input(MTH.METRIC_TYPE_DROPDOWN, "value"),
     }
 }
 
 
-def create_navbar(
-    metric: Optional[M.Metric],
-    saved_metric: Optional[WM.SavedMetric],
-    project: M.Project,
-    notebook_mode: bool,
-) -> dbc.Navbar:
-    navbar_children = [
-        MTH.from_metric_type(MTH.MetricType.from_metric(metric)),
-        dmc.TextInput(
-            id=METRIC_NAME_INPUT,
-            debounce=700,
-            placeholder="Name your metric",
-            value=saved_metric.name if saved_metric is not None else None,
+def metric_type_navbar_provider(
+    id: str, show_metric_type: bool = False, metric: Optional[M.Metric] = None, **kwargs
+) -> Optional[bc.Component]:
+    if not show_metric_type:
+        return None
+    return MTH.from_metric_type(MTH.MetricType.from_metric(metric))
+
+
+def metric_name_navbar_provider(
+    id: str,
+    show_metric_name: bool = False,
+    saved_metric: Optional[WM.SavedMetric] = None,
+    **kwargs,
+) -> Optional[bc.Component]:
+    if not show_metric_name:
+        return None
+
+    return dmc.TextInput(
+        id=METRIC_NAME_INPUT,
+        debounce=700,
+        placeholder="Name your metric",
+        value=saved_metric.name if saved_metric is not None else None,
+        size="xs",
+        icon=DashIconify(icon="material-symbols:star", color="dark"),
+        rightSection=dmc.Loader(
             size="xs",
-            icon=DashIconify(icon="material-symbols:star", color="dark"),
-            rightSection=dmc.Loader(
-                size="xs",
-                color="dark",
-                className="d-none",
-                id=METRIC_NAME_PROGRESS,
-            ),
-            style={"width": "200px"},
+            color="dark",
+            className="d-none",
+            id=METRIC_NAME_PROGRESS,
         ),
+        style={"width": "200px"},
+    )
+
+
+def share_button_navbar_provider(
+    id: str, notebook_mode: bool = True, **kwargs
+) -> Optional[bc.Component]:
+    return (
         dbc.Button(
             [
                 html.B(className="bi bi-link-45deg"),
                 " Share",
                 dcc.Clipboard(
                     id=CLIPBOARD,
                     content="",
@@ -114,21 +129,14 @@
             ],
             id=SHARE_BUTTON,
             className="position-relative top-0 start-0 text-nowrap",
             color="light",
             size="sm",
             style={"display": "none" if notebook_mode else "inline-block"},
         ),
-    ]
-
-    return NB.create_mitzu_navbar(
-        id=NAVBAR_ID,
-        children=navbar_children,
-        off_canvas_toggler_visible=not notebook_mode,
-        project_name=project.project_name,
     )
 
 
 def create_explore_page(
     query_params: Dict[str, str],
     discovered_project: M.DiscoveredProject,
     storage: S.MitzuStorage,
@@ -144,18 +152,20 @@
         saved_metric = storage.get_saved_metric(
             query_params[P.PROJECTS_EXPLORE_SAVED_METRIC_QUERY]
         )
         metric = saved_metric.metric
 
     metric_segments_div = MS.from_metric(metric, discovered_project)
     graph_container = create_graph_container(metric, discovered_project.project)
-    navbar = create_navbar(
+    navbar = NB.create_mitzu_navbar(
+        id=NAVBAR_ID,
+        show_metric_type=True,
+        show_metric_name=True,
         metric=metric,
         saved_metric=saved_metric,
-        project=discovered_project.project,
         notebook_mode=notebook_mode,
     )
 
     metric_id = H.create_unique_id() if saved_metric is None else saved_metric.id
     res = html.Div(
         children=[
             navbar,
@@ -225,16 +235,16 @@
     if len(group_by_paths) >= 1 and not (
         metric_type == MTH.MetricType.RETENTION
         and metric_config.time_group != M.TimeGroup.TOTAL
     ):
         gp = group_by_paths[0].get(CS.COMPLEX_SEGMENT_GROUP_BY)
         group_by = find_event_field_def(gp, discovered_project) if gp else None
         if group_by is not None:
-            group_by._event_data_table.project_reference.restore_value(
-                discovered_project.project
+            group_by._event_data_table.project_reference = (
+                M.Reference.create_from_value(discovered_project.project)
             )
     return group_by
 
 
 def create_metric_from_all_inputs(
     all_inputs: Dict[str, Any],
     discovered_project: M.DiscoveredProject,
@@ -413,18 +423,17 @@
 )
 @restricted
 def handle_metric_name_changed(
     metric_name: str,
     metric_id: str,
     href: str,
 ) -> str:
-    storage = cast(
-        DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-    ).storage
-
+    deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
+    storage = deps.storage
+    mitzu_cache = deps.cache
     parse_result = urlparse(href)
     sm = storage.get_saved_metric(metric_id)
     if sm is not None and sm.project is not None:
         storage.clear_saved_metric(metric_id)
         if metric_name:
             storage.set_saved_metric(metric_id, sm.rename(metric_name))
     else:
@@ -433,15 +442,15 @@
             P.PROJECTS_EXPLORE_PATH, parse_result.path, P.PROJECT_ID_PATH_PART
         )
         project = storage.get_project(project_id)
         metric_v64 = parse_qs(parse_result.query).get(P.PROJECTS_EXPLORE_METRIC_QUERY)
         if metric_v64 is not None:
             metric = SE.from_compressed_string(metric_v64[0], project)
             hash_key = GH.create_metric_hash_key(metric)
-            result_df = GH.get_metric_result_df(hash_key, metric, storage)
+            result_df = GH.get_metric_result_df(hash_key, metric, mitzu_cache)
             simple_chart = CHRT.get_simple_chart(metric, result_df)
             GH.store_rendered_saved_metric(
                 metric_name=metric_name,
                 metric=metric,
                 simple_chart=simple_chart,
                 project=project,
                 storage=storage,
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import dash_bootstrap_components as dbc
 import mitzu.model as M
 import mitzu.webapp.pages.explore.toolbar_handler as TH
 import mitzu.webapp.pages.explore.explore_page as EXP
 import mitzu.webapp.configs as configs
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.storage as S
+import mitzu.webapp.cache as C
 import mitzu.visualization.common as CO
 import flask
 import mitzu.webapp.pages.paths as P
 import mitzu.webapp.model as WM
 import mitzu.serialization as SE
 from mitzu.webapp.helper import MITZU_LOCATION
 
@@ -79,20 +80,20 @@
     metric_dict["co"]["cat"] = None
     metric_dict["id"] = None
 
     return hashlib.md5(json.dumps(metric_dict).encode("ascii")).hexdigest()
 
 
 def get_metric_result_df(
-    hash_key: str, metric: M.Metric, storage: S.MitzuStorage
+    hash_key: str, metric: M.Metric, mitzu_cache: C.MitzuCache
 ) -> pd.DataFrame:
-    result_df = storage.get_query_result_dataframe(hash_key)
+    result_df = mitzu_cache.get(hash_key)
     if result_df is None:
         result_df = metric.get_df()
-        storage.set_query_result_dataframe(hash_key, result_df)
+        mitzu_cache.put(hash_key, result_df, expire=configs.CACHE_EXPIRATION)
     return result_df
 
 
 def create_graph(
     metric: Optional[M.Metric],
     simple_chart: CO.SimpleChart,
 ) -> Optional[dcc.Graph]:
@@ -112,20 +113,20 @@
     fig = PLT.plot_chart(simple_chart, metric)
     return dcc.Graph(
         id=GRAPH, className="w-100", figure=fig, config={"displayModeBar": False}
     )
 
 
 def create_table(
-    metric: Optional[M.Metric], hash_key: str, storage: S.MitzuStorage
+    metric: Optional[M.Metric], hash_key: str, mitzu_cache: C.MitzuCache
 ) -> Optional[dbc.Table]:
     if metric is None:
         return None
 
-    result_df = get_metric_result_df(hash_key, metric, storage)
+    result_df = get_metric_result_df(hash_key, metric, mitzu_cache)
     result_df = result_df.sort_values(by=[result_df.columns[0], result_df.columns[1]])
     result_df.columns = [col[1:].replace("_", " ").title() for col in result_df.columns]
     table = dash_table.DataTable(
         id=TABLE,
         columns=[
             {"name": i, "id": i, "deletable": False, "selectable": False}
             for i in result_df.columns
@@ -219,17 +220,20 @@
         metric_id: str,
     ) -> bc.Component:
         try:
             parse_result = urlparse(href)
             project_id = P.get_path_value(
                 P.PROJECTS_EXPLORE_PATH, parse_result.path, P.PROJECT_ID_PATH_PART
             )
-            storage = cast(
+            deps = cast(
                 DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
-            ).storage
+            )
+            storage = deps.storage
+            mitzu_cache = deps.cache
+
             project = storage.get_project(project_id)
             if project is None:
                 return no_update
             all_inputs = get_final_all_inputs(all_inputs, ctx.inputs_list)
             all_inputs[EXP.METRIC_ID_VALUE] = metric_id
             all_inputs[EXP.METRIC_NAME_INPUT] = metric_name
             all_inputs[EXP.MITZU_LOCATION] = parse_result.query
@@ -256,33 +260,33 @@
                 return html.Div("Select an event", id=GRAPH, className=MESSAGE)
 
             should_save_metrics = all_inputs[EXP.METRIC_NAME_INPUT] is not None
             simple_chart: CO.SimpleChart
 
             hash_key = create_metric_hash_key(metric)
             if ctx.triggered_id in (TH.GRAPH_REFRESH_BUTTON, TH.GRAPH_RUN_QUERY_BUTTON):
-                storage.clear_query_result_dataframe(hash_key)
+                mitzu_cache.clear(hash_key)
 
             if (
                 not project.webapp_settings.auto_refresh_enabled
                 and ctx.triggered_id != TH.GRAPH_RUN_QUERY_BUTTON
-                and storage.get_query_result_dataframe(hash_key) is None
+                and mitzu_cache.get(hash_key) is None
             ):
                 return html.Div(
                     "Click run to execute the query", id=GRAPH, className=MESSAGE
                 )
 
             if graph_content_type == TH.CHART_VAL or should_save_metrics:
-                result_df = get_metric_result_df(hash_key, metric, storage)
+                result_df = get_metric_result_df(hash_key, metric, mitzu_cache)
                 simple_chart = CHRT.get_simple_chart(metric, result_df)
 
             if graph_content_type == TH.CHART_VAL:
                 res = create_graph(metric, simple_chart)  # noqa
             if graph_content_type == TH.TABLE_VAL:
-                res = create_table(metric, hash_key, storage)
+                res = create_table(metric, hash_key, mitzu_cache)
             elif graph_content_type == TH.SQL_VAL:
                 res = create_sql_area(metric)
 
             if should_save_metrics and metric_name is not None:
                 store_rendered_saved_metric(
                     metric_name=metric_name,
                     metric=metric,
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,20 +275,20 @@
         agg_type, agg_param = M.AggType.parse_agg_str(agg_type_val)
 
     if ctx.triggered_id == MTH.METRIC_TYPE_DROPDOWN:
         start_dt = None
         end_dt = None
         if metric_type == MTH.MetricType.RETENTION:
             time_group = M.TimeGroup.WEEK
-            resolution = M.Resolution.ONE_USER_EVENT_PER_HOUR
+            resolution = M.Resolution.ONE_USER_EVENT_PER_MINUTE
             lookback_days = M.TimeWindow(2, M.TimeGroup.MONTH)
             time_window = M.TimeWindow(1, M.TimeGroup.WEEK)
         elif metric_type == MTH.MetricType.CONVERSION:
             time_group = M.TimeGroup.DAY
-            resolution = M.Resolution.ONE_USER_EVENT_PER_MINUTE
+            resolution = M.Resolution.EVERY_EVENT
             lookback_days = M.TimeWindow(1, M.TimeGroup.MONTH)
             time_window = M.TimeWindow(1, M.TimeGroup.DAY)
         else:
             time_group = M.TimeGroup.DAY
             resolution = M.Resolution.EVERY_EVENT
             lookback_days = M.TimeWindow(1, M.TimeGroup.MONTH)
             time_window = M.TimeWindow(1, M.TimeGroup.DAY)
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,19 @@
 METRIC_TYPE_DROPDOWN = "metric-type-dropdown"
 
 
 class MetricType(Enum):
     SEGMENTATION = auto()
     CONVERSION = auto()
     RETENTION = auto()
-    JOURNEY = auto()
+    USER_JOURNEYS = auto()
+    REVENUE = auto()
+    AB_TEST_ANALYSIS = auto()
+    COHORTS = auto()
+    CHURN_ANALYSIS = auto()
 
     @classmethod
     def from_metric(cls, metric: Optional[M.Metric]) -> MetricType:
         if isinstance(metric, M.ConversionMetric):
             return MetricType.CONVERSION
         elif isinstance(metric, M.RetentionMetric):
             return MetricType.RETENTION
@@ -31,17 +35,22 @@
         return MetricType[val_str.upper()]
 
 
 def from_metric_type(metric_type: MetricType) -> bc.Component:
     return dmc.Select(
         data=[
             {
-                "label": m_type.name.upper(),
+                "label": m_type.name.upper().replace("_", " "),
                 "value": m_type.name.upper(),
-                "disabled": m_type == MetricType.JOURNEY,
+                "disabled": m_type
+                not in (
+                    MetricType.SEGMENTATION,
+                    MetricType.RETENTION,
+                    MetricType.CONVERSION,
+                ),
             }
             for m_type in MetricType
         ],
         id=METRIC_TYPE_DROPDOWN,
         clearable=False,
         value=metric_type.name.upper(),
         size="xs",
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/home.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/home.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 
 @restricted_layout
 def layout(**query_params):
     return html.Div(
         [
-            NB.create_mitzu_navbar("home-navbar", []),
+            NB.create_mitzu_navbar("home-navbar"),
             dbc.Container(
                 children=[
                     dbc.Row(
                         [
                             html.Img(
                                 src=configs.DASH_LOGO_PATH,
                                 height="100px",
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/login.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/login.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         )
         connection = depenednecies.storage.get_connection(connection_id)
 
     title = "Create new connection" if connection is None else "Manage connection"
 
     return dbc.Form(
         [
-            NB.create_mitzu_navbar("create-connection-navbar", []),
+            NB.create_mitzu_navbar("create-connection-navbar"),
             dbc.Container(
                 children=[
                     html.H4(title),
                     html.Hr(),
                     MCC.create_manage_connection_component(connection),
                     html.Hr(),
                     html.Div(
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         depenednecies: DEPS.Dependencies = cast(
             DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
         )
         dashboard = depenednecies.storage.get_dashboard(dashboard_id)
 
     return html.Div(
         [
-            NB.create_mitzu_navbar("create-dashboard-navbar", []),
+            NB.create_mitzu_navbar("create-dashboard-navbar"),
             MDC.create_manage_dashboard_container(dashboard),
         ]
     )
 
 
 register_page(
     __name__ + "_create",
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_event_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,20 @@
         ]
     )
 
 
 def create_event_table_component(project: Optional[M.Project]) -> bc.Component:
     rows = []
     if project is not None:
-        dp = project._discovered_project.get_value()
+        dp = project._discovered_project.get_value_if_exsits()
+        events_service = cast(
+            DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
+        ).events_service
+        events_service.populate_discovered_project(dp)
+
         if dp is not None:
             for edt, df in dp.definitions.items():
                 for evt_df in df.values():
                     rows.append(create_table_row(edt, evt_df))
 
     return dbc.Table(
         children=[
@@ -101,15 +106,15 @@
             selected_project = p
             break
 
     options = [{"label": p.project_name, "value": p.id} for p in projects]
 
     return html.Div(
         [
-            NB.create_mitzu_navbar("events-navbar", []),
+            NB.create_mitzu_navbar("events-navbar"),
             dbc.Container(
                 [
                     html.H4("Discovered events and properties"),
                     html.Hr(),
                     dbc.Row(
                         [
                             dbc.Col("Select project:", className="lead", width="auto"),
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         "Create new project"
         if project is None
         else f"{H.value_to_label(project.project_name)}"
     )
 
     return html.Div(
         [
-            NB.create_mitzu_navbar("create-project-navbar", []),
+            NB.create_mitzu_navbar("create-project-navbar"),
             dbc.Container(
                 children=[
                     dbc.Row(
                         [
                             dbc.Col(
                                 html.H4(
                                     title, id=PROJECT_TITLE, className="card-title"
@@ -183,15 +183,15 @@
                         class_name="d-inline-block me-3 mb-1",
                         href=(
                             P.create_path(
                                 P.EVENTS_AND_PROPERTIES_PROJECT_PATH,
                                 project_id=project_id,
                             )
                             if project_id is not None
-                            else P.EVENTS_AND_PROPERTIES_PROJECT_PATH
+                            else P.EVENTS_AND_PROPERTIES_PATH
                         ),
                     ),
                     html.Div(
                         children="",
                         className="mb-3 lead",
                         id=MANAGE_PROJECT_INFO,
                     ),
@@ -230,19 +230,14 @@
         project_id = P.get_path_value(
             P.PROJECTS_MANAGE_PATH, pathname, P.PROJECT_ID_PATH_PART
         )
         depenednecies = cast(
             DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
         )
         try:
-            project = depenednecies.storage.get_project(project_id=project_id)
-            for edt in project.event_data_tables:
-                depenednecies.storage.delete_event_data_table_definition(
-                    project_id=project_id, edt_full_name=edt.get_full_name()
-                )
             depenednecies.storage.delete_project(project_id)
         except Exception:
             # TBD: Toaster
             traceback.print_exc()
 
     return no_update
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 def layout(**query_params) -> bc.Component:
     storage = cast(
         DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY)
     ).storage
 
     return html.Div(
         [
-            NB.create_mitzu_navbar("saved_metrics_navbar", [], storage),
+            NB.create_mitzu_navbar("saved_metrics_navbar", storage=storage),
             dbc.Container(
                 [
                     html.H4("Saved metrics"),
                     html.Hr(),
                     html.Div("", id=SAVED_METRICS_INFO, className="lead"),
                     dbc.Row(
                         list_saved_metrics(storage),
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/paths.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/projects_page.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 @restricted_layout
 def layout(**query_params) -> bc.Component:
     projects = create_projects_children()
 
     return html.Div(
         [
-            NB.create_mitzu_navbar("explore-navbar", []),
+            NB.create_mitzu_navbar("explore-navbar"),
             dbc.Container(
                 children=[
                     dbc.Row(
                         [
                             dbc.Col(
                                 html.H4(
                                     "Select a project for exploration",
@@ -94,15 +94,15 @@
 
 
 def create_project_selector(project_id: str, deps: DEPS.Dependencies) -> bc.Component:
     project = deps.storage.get_project(project_id)
     discovered_project = project._discovered_project.get_value()
 
     tables = len(project.event_data_tables)
-    events = len(discovered_project.get_all_events()) if discovered_project else 0
+    events = len(discovered_project.get_all_event_names()) if discovered_project else 0
     project_jumbotron = dbc.Col(
         dbc.Card(
             dbc.CardBody(
                 [
                     html.H4(
                         project.project_name,
                         className="card-title",
```

### Comparing `mitzu-0.5.9/mitzu/webapp/pages/users.py` & `mitzu-0.6.0rc1/mitzu/webapp/pages/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
     is_admin = authorizer.get_current_user_role(flask.request) == WM.Role.ADMIN
 
     table = create_users_table(user_service)
 
     return html.Div(
         [
-            NB.create_mitzu_navbar("users_list", []),
+            NB.create_mitzu_navbar("users_list"),
             dbc.Container(
                 [
                     html.H4("Registered Users"),
                     html.Hr(),
                     table,
                 ]
                 + (
```

### Comparing `mitzu-0.5.9/mitzu/webapp/service/events_service.py` & `mitzu-0.6.0rc1/mitzu/webapp/service/events_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,20 +15,23 @@
 
     def list_all_projects(self) -> List[M.Project]:
         project_ids = self.storage.list_projects()
         return [
             self.storage.get_project(pid) for pid in project_ids
         ]  # todo move this logic to storage
 
+    def populate_discovered_project(self, discovered_project: M.DiscoveredProject):
+        self.storage.populate_discovered_project(discovered_project)
+
     def get_project_definition(
         self, project_id: str
     ) -> Dict[M.EventDataTable, Dict[str, M.Reference[M.EventDef]]]:
-        dp = self.storage.get_project(project_id)._discovered_project.get_value()
-        if dp is None:
-            raise EventServiceException(f"Missing discovered project for {project_id}")
+        project = self.storage.get_project(project_id)
+        dp = project._discovered_project.get_value_if_exsits()
+        self.storage.populate_discovered_project(dp)
         return dp.definitions
 
     def discover_project(
         self,
         project_id: str,
         callback: Callable[
             [
@@ -48,15 +51,15 @@
         def edt_callback(
             edt: M.EventDataTable,
             defs: Dict[str, M.Reference[M.EventDef]],
             exc: Optional[Exception],
         ):
             if exc is None:
                 self.storage.set_event_data_table_definition(
-                    project_id, edt_full_name=edt.get_full_name(), definitions=defs
+                    event_data_table=edt, definitions=defs
                 )
             edts.append(edt)
             callback(edt, defs, exc, len(edts), edt_count)
 
         discovered_project = project.discover_project(False, edt_callback)
         self.storage.set_project(
             project_id=discovered_project.project.id,
```

### Comparing `mitzu-0.5.9/mitzu/webapp/service/user_service.py` & `mitzu-0.6.0rc1/mitzu/webapp/service/user_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/toast.py` & `mitzu-0.6.0rc1/mitzu/webapp/toast.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.5.9/mitzu/webapp/webapp.py` & `mitzu-0.6.0rc1/mitzu/webapp/webapp.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dash import CeleryManager, Dash, DiskcacheManager, dcc, html, page_container
 from dash.long_callback.managers import BaseLongCallbackManager
 
 import mitzu.webapp.configs as configs
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.storage as S
 import mitzu.webapp.offcanvas as OC
+import mitzu.webapp.pages.explore.explore_page as EXP
 from mitzu.helper import LOGGER
 
 from mitzu.webapp.helper import MITZU_LOCATION
 
 MAIN = "main"
 
 MDB_CSS = "https://cdnjs.cloudflare.com/ajax/libs/mdb-ui-kit/6.0.1/mdb.min.css"
@@ -56,21 +57,51 @@
             expire=configs.CACHE_EXPIRATION,
         )
 
 
 def create_dash_app(dependencies: Optional[DEPS.Dependencies] = None) -> Dash:
     server = flask.Flask(__name__)
     if dependencies is None:
-        dependencies = DEPS.Dependencies.from_configs(server)
+        dependencies = DEPS.Dependencies.from_configs()
+
+    if dependencies.authorizer is not None:
+
+        @server.before_request
+        def before_request():
+            request = flask.request
+            return dependencies.authorizer.authorize_request(request)
+
+        @server.after_request
+        def after_request(response: flask.Response):
+            request = flask.request
+            if dependencies is not None and dependencies.authorizer is not None:
+                return dependencies.authorizer.refresh_auth_token(request, response)
+            return response
 
     with server.app_context():
         flask.current_app.config[DEPS.CONFIG_KEY] = dependencies
         if configs.SETUP_SAMPLE_PROJECT:
             S.setup_sample_project(dependencies.storage)
 
+    dependencies.navbar_service.register_navbar_item_provider(
+        "left",
+        EXP.metric_type_navbar_provider,
+        priority=20,
+    )
+    dependencies.navbar_service.register_navbar_item_provider(
+        "left",
+        EXP.metric_name_navbar_provider,
+        priority=30,
+    )
+    dependencies.navbar_service.register_navbar_item_provider(
+        "left",
+        EXP.share_button_navbar_provider,
+        priority=40,
+    )
+
     app = Dash(
         __name__,
         compress=configs.DASH_COMPRESS_RESPONSES,
         server=server,
         external_stylesheets=[
             MDB_CSS,
             dbc.icons.BOOTSTRAP,
```

### Comparing `mitzu-0.5.9/pyproject.toml` & `mitzu-0.6.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.5.9"
+version = "0.6.0-rc.1"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
@@ -15,40 +15,41 @@
 pandas = "~1.3.5"
 plotly = "~5.5.0"
 sqlalchemy = {version="~1.4.31", extras=["asyncio"]}
 pyarrow = "~8.0.0"
 fastparquet = "~0.8.0"
 sqlparse = "^0.4.2"
 tqdm = "^4.64.1"
-cryptography= ">=38.0.4,<39.1.0"
+cryptography= "==38.0.4"
 requests = "^2.28.2"
 
 # Adapter extras
 psycopg2 = {version = "~2.9.3", optional=true}
 mysql-connector-python = {version = "~8.0.28", optional=true}
 trino = { version = "~0.313.0", optional=true, extras=["sqlalchemy"] }
 databricks-sql-connector = { version = "^2.0.2", optional=true}
 PyAthena = { version="^2.13.0", optional=true}
 snowflake-sqlalchemy = {version = "^1.4.3", optional=true}
 snowflake-connector-python = {version = "~=2.8.3", optional=true}
 
 # Webapp Extras
-dash = {version="^2.6.0", optional=true, extras=["diskcache", "celery", "compress"]}
+dash = {version="~2.8.1", optional=true, extras=["diskcache", "celery", "compress"]}
 dash-bootstrap-components = { version="^1.2.0", optional=true}
 dash-mantine-components =  { version= "^0.11.1", optional=true}
 orjson = {version="^3.7.11", optional=true}
 PyJWT = { version="^2.4.0", extras=["crypto"], optional=true}
 gunicorn = {version= "^20.1.0", optional=true}
 redis =  { version= "^4.4.0", optional=true}
 kaleido = {version = "==0.2.1", optional=true}
 dash-iconify = {version ="^0.1.2", optional=true}
 dash-draggable = {version="^0.1.2", optional=true}
 
 [tool.poetry.extras]
 postgres = ["psycopg2"]
+redshift= ["psycopg2"]
 mysql = ["mysql-connector-python"]
 trinodwh = ["trino"]
 databricks = ["databricks-sql-connector"]
 athena = ["PyAthena"]
 snowflake = ["snowflake-sqlalchemy","snowflake-connector-python"]
 webapp = [
     "orjson", 
@@ -74,14 +75,15 @@
 apig-wsgi = "^2.14.0"
 types-python-dateutil = "^2.8.18"
 flake8 = "^5.0.4"
 autoflake = "^1.4"
 types-requests = "^2.28.8"
 freezegun = "^1.2.2"
 pyclean = "^2.2.0"
+hypothesis = "^6.71.0"
 
 # Docs
 sphinx = "^5.3.0"
 sphinx-autodoc-typehints = "^1.19.5"
 
 
 [tool.poetry.group.dev.dependencies]
```

