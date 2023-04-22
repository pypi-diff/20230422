# Comparing `tmp/ord-schema-0.3.48.tar.gz` & `tmp/ord-schema-0.3.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ord-schema-0.3.48.tar", last modified: Thu Apr 20 08:27:56 2023, max compression
+gzip compressed data, was "ord-schema-0.3.49.tar", last modified: Sat Apr 22 00:32:09 2023, max compression
```

## Comparing `ord-schema-0.3.48.tar` & `ord-schema-0.3.49.tar`

### file list

```diff
@@ -1,67 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.341699 ord-schema-0.3.48/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-20 08:27:33.000000 ord-schema-0.3.48/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-20 08:27:33.000000 ord-schema-0.3.48/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-20 08:27:56.341699 ord-schema-0.3.48/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-20 08:27:33.000000 ord-schema-0.3.48/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.333698 ord-schema-0.3.48/ord_schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/frozen_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/frozen_message_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.333698 ord-schema-0.3.48/ord_schema/macros/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/macros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/macros/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/macros/solutions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/macros/workups.py
--rw-r--r--   0 runner    (1001) docker     (123)    35625 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/message_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/message_helpers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.337698 ord-schema-0.3.48/ord_schema/orm/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/add_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/add_datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/mappers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/rdkit_mappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/orm/rdkit_mappers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.337698 ord-schema-0.3.48/ord_schema/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/dataset_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/dataset_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    77919 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/reaction_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/reaction_pb2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/proto/test_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/resolvers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.341699 ord-schema-0.3.48/ord_schema/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/build_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/check_pb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/check_pb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/enumerate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/enumerate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/parse_uspto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/process_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/process_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/validate_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/scripts/validate_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/templating_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/units_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    45244 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/validations.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-20 08:27:34.000000 ord-schema-0.3.48/ord_schema/validations_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 08:27:56.333698 ord-schema-0.3.48/ord_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 08:27:56.000000 ord-schema-0.3.48/ord_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-20 08:27:34.000000 ord-schema-0.3.48/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 08:27:56.341699 ord-schema-0.3.48/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-20 08:27:37.000000 ord-schema-0.3.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:32:09.200247 ord-schema-0.3.49/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-22 00:31:40.000000 ord-schema-0.3.49/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-22 00:31:40.000000 ord-schema-0.3.49/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-22 00:31:40.000000 ord-schema-0.3.49/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-22 00:32:09.200247 ord-schema-0.3.49/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-22 00:31:40.000000 ord-schema-0.3.49/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:32:09.196247 ord-schema-0.3.49/ord_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/frozen_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/frozen_message_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:32:09.196247 ord-schema-0.3.49/ord_schema/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/macros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/macros/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/macros/solutions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/macros/workups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35625 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/message_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27021 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/message_helpers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:32:09.200247 ord-schema-0.3.49/ord_schema/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/add_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/add_datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/mappers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/rdkit_mappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/orm/rdkit_mappers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:32:09.200247 ord-schema-0.3.49/ord_schema/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/proto/dataset_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/proto/dataset_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77919 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/proto/reaction_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/proto/reaction_pb2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/proto/test_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/resolvers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:32:09.200247 ord-schema-0.3.49/ord_schema/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/build_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/check_pb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/check_pb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/enumerate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/enumerate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22653 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/parse_uspto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/process_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21286 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/process_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/validate_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/scripts/validate_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/templating_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/units_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45244 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/validations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-22 00:31:40.000000 ord-schema-0.3.49/ord_schema/validations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:32:09.196247 ord-schema-0.3.49/ord_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-22 00:32:09.000000 ord-schema-0.3.49/ord_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-22 00:32:09.000000 ord-schema-0.3.49/ord_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 00:32:09.000000 ord-schema-0.3.49/ord_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-22 00:32:09.000000 ord-schema-0.3.49/ord_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 00:32:09.000000 ord-schema-0.3.49/ord_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 00:32:09.200247 ord-schema-0.3.49/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-22 00:31:40.000000 ord-schema-0.3.49/proto/dataset.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    46054 2023-04-22 00:31:40.000000 ord-schema-0.3.49/proto/reaction.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-22 00:31:40.000000 ord-schema-0.3.49/proto/test.proto
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-22 00:31:40.000000 ord-schema-0.3.49/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 00:32:09.200247 ord-schema-0.3.49/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-22 00:31:48.000000 ord-schema-0.3.49/setup.py
```

### Comparing `ord-schema-0.3.48/LICENSE` & `ord-schema-0.3.49/LICENSE`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/PKG-INFO` & `ord-schema-0.3.49/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.48
+Version: 0.3.49
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.48/README.md` & `ord-schema-0.3.49/README.md`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/__init__.py` & `ord-schema-0.3.49/ord_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/frozen_message.py` & `ord-schema-0.3.49/ord_schema/frozen_message.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/frozen_message_test.py` & `ord-schema-0.3.49/ord_schema/frozen_message_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/logging.py` & `ord-schema-0.3.49/ord_schema/logging.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/macros/__init__.py` & `ord-schema-0.3.49/ord_schema/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/macros/solutions.py` & `ord-schema-0.3.49/ord_schema/macros/solutions.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/macros/solutions_test.py` & `ord-schema-0.3.49/ord_schema/macros/solutions_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/macros/workups.py` & `ord-schema-0.3.49/ord_schema/macros/workups.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/message_helpers.py` & `ord-schema-0.3.49/ord_schema/message_helpers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/message_helpers_test.py` & `ord-schema-0.3.49/ord_schema/message_helpers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/__init__.py` & `ord-schema-0.3.49/ord_schema/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/add_datasets.py` & `ord-schema-0.3.49/ord_schema/orm/add_datasets.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/add_datasets_test.py` & `ord-schema-0.3.49/ord_schema/orm/add_datasets_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/conftest.py` & `ord-schema-0.3.49/ord_schema/orm/conftest.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/database.py` & `ord-schema-0.3.49/ord_schema/orm/database.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/database_test.py` & `ord-schema-0.3.49/ord_schema/orm/database_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/mappers.py` & `ord-schema-0.3.49/ord_schema/orm/mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/mappers_test.py` & `ord-schema-0.3.49/ord_schema/orm/mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/rdkit_mappers.py` & `ord-schema-0.3.49/ord_schema/orm/rdkit_mappers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/orm/rdkit_mappers_test.py` & `ord-schema-0.3.49/ord_schema/orm/rdkit_mappers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/proto/__init__.py` & `ord-schema-0.3.49/ord_schema/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/proto/dataset_pb2.py` & `ord-schema-0.3.49/ord_schema/proto/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/proto/dataset_pb2_test.py` & `ord-schema-0.3.49/ord_schema/proto/dataset_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/proto/reaction_pb2.py` & `ord-schema-0.3.49/ord_schema/proto/reaction_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/proto/reaction_pb2_test.py` & `ord-schema-0.3.49/ord_schema/proto/reaction_pb2_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/proto/test_pb2.py` & `ord-schema-0.3.49/ord_schema/proto/test_pb2.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/resolvers.py` & `ord-schema-0.3.49/ord_schema/resolvers.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/resolvers_test.py` & `ord-schema-0.3.49/ord_schema/resolvers_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/__init__.py` & `ord-schema-0.3.49/ord_schema/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/build_dataset.py` & `ord-schema-0.3.49/ord_schema/scripts/build_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/build_dataset_test.py` & `ord-schema-0.3.49/ord_schema/scripts/build_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/check_pb.py` & `ord-schema-0.3.49/ord_schema/scripts/check_pb.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/check_pb_test.py` & `ord-schema-0.3.49/ord_schema/scripts/check_pb_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/enumerate_dataset.py` & `ord-schema-0.3.49/ord_schema/scripts/enumerate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/enumerate_dataset_test.py` & `ord-schema-0.3.49/ord_schema/scripts/enumerate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/parse_uspto.py` & `ord-schema-0.3.49/ord_schema/scripts/parse_uspto.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/process_dataset.py` & `ord-schema-0.3.49/ord_schema/scripts/process_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/process_dataset_test.py` & `ord-schema-0.3.49/ord_schema/scripts/process_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/validate_dataset.py` & `ord-schema-0.3.49/ord_schema/scripts/validate_dataset.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/scripts/validate_dataset_test.py` & `ord-schema-0.3.49/ord_schema/scripts/validate_dataset_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/templating.py` & `ord-schema-0.3.49/ord_schema/templating.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/templating_test.py` & `ord-schema-0.3.49/ord_schema/templating_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/units.py` & `ord-schema-0.3.49/ord_schema/units.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/units_test.py` & `ord-schema-0.3.49/ord_schema/units_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/updates.py` & `ord-schema-0.3.49/ord_schema/updates.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/updates_test.py` & `ord-schema-0.3.49/ord_schema/updates_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/validations.py` & `ord-schema-0.3.49/ord_schema/validations.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema/validations_test.py` & `ord-schema-0.3.49/ord_schema/validations_test.py`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/ord_schema.egg-info/PKG-INFO` & `ord-schema-0.3.49/ord_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ord-schema
-Version: 0.3.48
+Version: 0.3.49
 Summary: Schema for the Open Reaction Database
 Home-page: https://github.com/Open-Reaction-Database/ord-schema
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `ord-schema-0.3.48/ord_schema.egg-info/SOURCES.txt` & `ord-schema-0.3.49/ord_schema.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 AUTHORS
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 ord_schema/__init__.py
 ord_schema/frozen_message.py
 ord_schema/frozen_message_test.py
 ord_schema/logging.py
@@ -51,8 +52,11 @@
 ord_schema/scripts/check_pb_test.py
 ord_schema/scripts/enumerate_dataset.py
 ord_schema/scripts/enumerate_dataset_test.py
 ord_schema/scripts/parse_uspto.py
 ord_schema/scripts/process_dataset.py
 ord_schema/scripts/process_dataset_test.py
 ord_schema/scripts/validate_dataset.py
-ord_schema/scripts/validate_dataset_test.py
+ord_schema/scripts/validate_dataset_test.py
+proto/dataset.proto
+proto/reaction.proto
+proto/test.proto
```

### Comparing `ord-schema-0.3.48/ord_schema.egg-info/requires.txt` & `ord-schema-0.3.49/ord_schema.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ord-schema-0.3.48/setup.py` & `ord-schema-0.3.49/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,32 +17,25 @@
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="ord-schema",
-    version="0.3.48",
+    version="0.3.49",
     description="Schema for the Open Reaction Database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Reaction-Database/ord-schema",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
-    package_data={
-        "ord_schema.proto": [
-            "dataset.proto",
-            "reaction.proto",
-            "test.proto",
-        ],
-    },
     python_requires=">=3.10",
     install_requires=[
         "docopt>=0.6.2",
         "flask>=1.1.2",
         "inflection>=0.5.1",
         "jinja2>=2.0.0",
         "joblib>=1.0.0",
```

