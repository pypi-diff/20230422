# Comparing `tmp/feast-0.9.8.tar.gz` & `tmp/feast-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feast-0.9.8.tar", last modified: Thu Jun  9 04:29:59 2022, max compression
+gzip compressed data, was "feast-0.9.9.tar", last modified: Thu Jul 14 02:37:20 2022, max compression
```

## Comparing `feast-0.9.8.tar` & `feast-0.9.9.tar`

### file list

```diff
@@ -1,250 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.049041 feast-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-06-09 04:28:25.000000 feast-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    12154 2022-06-09 04:29:59.049041 feast-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.025039 feast-0.9.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-06-09 04:28:25.000000 feast-0.9.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     5430 2022-06-09 04:28:25.000000 feast-0.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-06-09 04:28:25.000000 feast-0.9.8/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.029039 feast-0.9.8/docs/source/
--rw-r--r--   0 runner    (1001) docker     (121)     5430 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.contrib.rst
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.contrib.validation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2914 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.core.rst
--rw-r--r--   0 runner    (1001) docker     (121)      804 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.loaders.rst
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.pyspark.launchers.aws.rst
--rw-r--r--   0 runner    (1001) docker     (121)      442 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.pyspark.launchers.gcloud.rst
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.pyspark.launchers.k8s.rst
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.pyspark.launchers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.pyspark.launchers.standalone.rst
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.pyspark.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2514 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.rst
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.serving.rst
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.staging.rst
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.storage.rst
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.third_party.grpc.health.rst
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.third_party.grpc.health.v1.rst
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.third_party.grpc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.third_party.rst
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/feast.types.rst
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-06-09 04:28:25.000000 feast-0.9.8/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.029039 feast-0.9.8/feast/
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-06-09 04:28:25.000000 feast-0.9.8/feast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13037 2022-06-09 04:28:25.000000 feast-0.9.8/feast/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    48327 2022-06-09 04:28:25.000000 feast-0.9.8/feast/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     6784 2022-06-09 04:28:25.000000 feast-0.9.8/feast/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8673 2022-06-09 04:28:25.000000 feast-0.9.8/feast/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.029039 feast-0.9.8/feast/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.029039 feast-0.9.8/feast/contrib/validation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/contrib/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-06-09 04:28:25.000000 feast-0.9.8/feast/contrib/validation/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6822 2022-06-09 04:28:25.000000 feast-0.9.8/feast/contrib/validation/ge.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.033039 feast-0.9.8/feast/core/
--rw-r--r--   0 runner    (1001) docker     (121)    67988 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/CoreService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    21424 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/CoreService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    27134 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/CoreService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9142 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/DataFormat_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3227 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/DataFormat_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/DataFormat_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    20067 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/DataSource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7664 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/DataSource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/DataSource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9995 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/Entity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3672 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/Entity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/Entity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    13450 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/FeatureTable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5156 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/FeatureTable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/FeatureTable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5531 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/Feature_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/Feature_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/Feature_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    44707 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/JobService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14674 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/JobService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11486 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/JobService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    19308 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/Store_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7457 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/Store_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/Store_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3748 2022-06-09 04:28:25.000000 feast-0.9.8/feast/data_format.py
--rw-r--r--   0 runner    (1001) docker     (121)    22924 2022-06-09 04:28:25.000000 feast-0.9.8/feast/data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     8342 2022-06-09 04:28:25.000000 feast-0.9.8/feast/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     5405 2022-06-09 04:28:25.000000 feast-0.9.8/feast/feature.py
--rw-r--r--   0 runner    (1001) docker     (121)    12576 2022-06-09 04:28:25.000000 feast-0.9.8/feast/feature_table.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.033039 feast-0.9.8/feast/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8942 2022-06-09 04:28:25.000000 feast-0.9.8/feast/grpc/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-06-09 04:28:25.000000 feast-0.9.8/feast/grpc/grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    13162 2022-06-09 04:28:25.000000 feast-0.9.8/feast/job_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.033039 feast-0.9.8/feast/loaders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6979 2022-06-09 04:28:25.000000 feast-0.9.8/feast/loaders/abstract_producer.py
--rw-r--r--   0 runner    (1001) docker     (121)     5120 2022-06-09 04:28:25.000000 feast-0.9.8/feast/loaders/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     7802 2022-06-09 04:28:25.000000 feast-0.9.8/feast/loaders/ingest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-06-09 04:28:25.000000 feast-0.9.8/feast/loaders/yaml.py
--rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-06-09 04:28:25.000000 feast-0.9.8/feast/online_response.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.025039 feast-0.9.8/feast/protos/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.025039 feast-0.9.8/feast/protos/feast/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.037040 feast-0.9.8/feast/protos/feast/core/
--rw-r--r--   0 runner    (1001) docker     (121)    68096 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/CoreService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    21424 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/CoreService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    27156 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/CoreService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     9180 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/DataFormat_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3227 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/DataFormat_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/DataFormat_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    20589 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/DataSource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7795 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/DataSource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/DataSource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    10507 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Entity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3801 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Entity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Entity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    13979 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/FeatureTable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     5285 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/FeatureTable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/FeatureTable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    12739 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/FeatureView_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4775 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/FeatureView_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/FeatureView_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Feature_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Feature_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Feature_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     5918 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Registry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Registry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Registry_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    18548 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Store_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7070 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Store_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/core/Store_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.037040 feast-0.9.8/feast/protos/feast/serving/
--rw-r--r--   0 runner    (1001) docker     (121)    27682 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/serving/ServingService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9406 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/serving/ServingService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4661 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/serving/ServingService_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.037040 feast-0.9.8/feast/protos/feast/storage/
--rw-r--r--   0 runner    (1001) docker     (121)     3710 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/storage/Redis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/storage/Redis_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/storage/Redis_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/protos/feast/types/
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/types/EntityKey_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/types/EntityKey_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/types/EntityKey_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2963 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/types/Field_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/types/Field_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/types/Field_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    24401 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/types/Value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9033 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/types/Value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-09 04:28:25.000000 feast-0.9.8/feast/protos/feast/types/Value_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/pyspark/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18519 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)    28492 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/historical_feature_retrieval_job.py
--rw-r--r--   0 runner    (1001) docker     (121)    13094 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/pyspark/launchers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/pyspark/launchers/aws/
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12919 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/aws/emr.py
--rw-r--r--   0 runner    (1001) docker     (121)    11421 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/aws/emr_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/pyspark/launchers/gcloud/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/gcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16888 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/gcloud/dataproc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/pyspark/launchers/k8s/
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14164 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/k8s/k8s.py
--rw-r--r--   0 runner    (1001) docker     (121)     8866 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/k8s/k8s_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/pyspark/launchers/standalone/
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/standalone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11725 2022-06-09 04:28:25.000000 feast-0.9.8/feast/pyspark/launchers/standalone/local.py
--rw-r--r--   0 runner    (1001) docker     (121)     6786 2022-06-09 04:28:25.000000 feast-0.9.8/feast/remote_job.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/serving/
--rw-r--r--   0 runner    (1001) docker     (121)    27622 2022-06-09 04:28:25.000000 feast-0.9.8/feast/serving/ServingService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9406 2022-06-09 04:28:25.000000 feast-0.9.8/feast/serving/ServingService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4639 2022-06-09 04:28:25.000000 feast-0.9.8/feast/serving/ServingService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/serving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/staging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-06-09 04:28:25.000000 feast-0.9.8/feast/staging/entities.py
--rw-r--r--   0 runner    (1001) docker     (121)    17709 2022-06-09 04:28:25.000000 feast-0.9.8/feast/staging/storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/storage/
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-06-09 04:28:25.000000 feast-0.9.8/feast/storage/Redis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-06-09 04:28:25.000000 feast-0.9.8/feast/storage/Redis_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-06-09 04:28:25.000000 feast-0.9.8/feast/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/third_party/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/third_party/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/third_party/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/third_party/grpc/health/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/third_party/grpc/health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.041040 feast-0.9.8/feast/third_party/grpc/health/v1/
--rw-r--r--   0 runner    (1001) docker     (121)     5835 2022-06-09 04:28:25.000000 feast-0.9.8/feast/third_party/grpc/health/v1/HealthService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-06-09 04:28:25.000000 feast-0.9.8/feast/third_party/grpc/health/v1/HealthService_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2867 2022-06-09 04:28:25.000000 feast-0.9.8/feast/third_party/grpc/health/v1/HealthService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/third_party/grpc/health/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16331 2022-06-09 04:28:25.000000 feast-0.9.8/feast/type_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.045040 feast-0.9.8/feast/types/
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-06-09 04:28:25.000000 feast-0.9.8/feast/types/Field_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-06-09 04:28:25.000000 feast-0.9.8/feast/types/Field_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    24363 2022-06-09 04:28:25.000000 feast-0.9.8/feast/types/Value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9033 2022-06-09 04:28:25.000000 feast-0.9.8/feast/types/Value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/feast/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-06-09 04:28:25.000000 feast-0.9.8/feast/value_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-06-09 04:28:25.000000 feast-0.9.8/feast/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.029039 feast-0.9.8/feast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    12154 2022-06-09 04:29:58.000000 feast-0.9.8/feast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6878 2022-06-09 04:29:58.000000 feast-0.9.8/feast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 04:29:58.000000 feast-0.9.8/feast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-09 04:29:58.000000 feast-0.9.8/feast.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-06-09 04:29:58.000000 feast-0.9.8/feast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-06-09 04:29:58.000000 feast-0.9.8/feast.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-06-09 04:28:25.000000 feast-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-06-09 04:28:25.000000 feast-0.9.8/requirements-ci.txt
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-06-09 04:28:25.000000 feast-0.9.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-06-09 04:29:59.049041 feast-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-06-09 04:28:25.000000 feast-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.045040 feast-0.9.8/telemetry_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-06-09 04:28:25.000000 feast-0.9.8/telemetry_tests/test_telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.045040 feast-0.9.8/tensorflow_metadata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/tensorflow_metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.045040 feast-0.9.8/tensorflow_metadata/proto/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/tensorflow_metadata/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.045040 feast-0.9.8/tensorflow_metadata/proto/v0/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/tensorflow_metadata/proto/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-06-09 04:28:25.000000 feast-0.9.8/tensorflow_metadata/proto/v0/path_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-06-09 04:28:25.000000 feast-0.9.8/tensorflow_metadata/proto/v0/path_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)   107849 2022-06-09 04:28:25.000000 feast-0.9.8/tensorflow_metadata/proto/v0/schema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    42974 2022-06-09 04:28:25.000000 feast-0.9.8/tensorflow_metadata/proto/v0/schema_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    87532 2022-06-09 04:28:25.000000 feast-0.9.8/tensorflow_metadata/proto/v0/statistics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    32249 2022-06-09 04:28:25.000000 feast-0.9.8/tensorflow_metadata/proto/v0/statistics_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.045040 feast-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-06-09 04:28:25.000000 feast-0.9.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.049041 feast-0.9.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)     7059 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/austin_bikeshare.bikeshare_stations.avro
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/bookings.csv
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/column_mapping_test_entity.csv
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/column_mapping_test_feature.csv
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/customer_driver_pairs.csv
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/customers.csv
--rw-r--r--   0 runner    (1001) docker     (121)     7939 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/dev_featuretable.csv
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/driver_features.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/localhost.crt
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/localhost.key
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/localhost.pem
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.049041 feast-0.9.8/tests/data/tensorflow_metadata/
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/tensorflow_metadata/bikeshare_feature_set.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/tensorflow_metadata/bikeshare_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-06-09 04:28:25.000000 feast-0.9.8/tests/data/transactions.csv
--rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-06-09 04:28:25.000000 feast-0.9.8/tests/dataframes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-06-09 04:28:25.000000 feast-0.9.8/tests/feast_core_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-06-09 04:28:25.000000 feast-0.9.8/tests/feast_serving_server.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.049041 feast-0.9.8/tests/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)     5872 2022-06-09 04:28:25.000000 feast-0.9.8/tests/grpc/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 04:29:59.049041 feast-0.9.8/tests/loaders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 04:28:25.000000 feast-0.9.8/tests/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-06-09 04:28:25.000000 feast-0.9.8/tests/loaders/test_file.py
--rw-r--r--   0 runner    (1001) docker     (121)    26658 2022-06-09 04:28:25.000000 feast-0.9.8/tests/test_as_of_join.py
--rw-r--r--   0 runner    (1001) docker     (121)    33588 2022-06-09 04:28:25.000000 feast-0.9.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5203 2022-06-09 04:28:25.000000 feast-0.9.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2767 2022-06-09 04:28:25.000000 feast-0.9.8/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-06-09 04:28:25.000000 feast-0.9.8/tests/test_feature_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    17523 2022-06-09 04:28:25.000000 feast-0.9.8/tests/test_historical_feature_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-06-09 04:28:25.000000 feast-0.9.8/tests/test_remote_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     6859 2022-06-09 04:28:25.000000 feast-0.9.8/tests/test_streaming_control_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.538276 feast-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-07-14 02:36:03.000000 feast-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    12154 2022-07-14 02:37:20.538276 feast-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.518276 feast-0.9.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-07-14 02:36:03.000000 feast-0.9.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     5430 2022-07-14 02:36:03.000000 feast-0.9.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-14 02:36:03.000000 feast-0.9.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.522276 feast-0.9.9/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (121)     5430 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.contrib.validation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2914 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.core.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.pyspark.launchers.aws.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      442 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.pyspark.launchers.gcloud.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.pyspark.launchers.k8s.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.pyspark.launchers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.pyspark.launchers.standalone.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.pyspark.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2514 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.serving.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.staging.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.storage.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.third_party.grpc.health.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.third_party.grpc.health.v1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.third_party.grpc.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.third_party.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/feast.types.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-07-14 02:36:03.000000 feast-0.9.9/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.522276 feast-0.9.9/feast/
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-07-14 02:36:03.000000 feast-0.9.9/feast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13037 2022-07-14 02:36:03.000000 feast-0.9.9/feast/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49798 2022-07-14 02:36:03.000000 feast-0.9.9/feast/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6766 2022-07-14 02:36:03.000000 feast-0.9.9/feast/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8671 2022-07-14 02:36:03.000000 feast-0.9.9/feast/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.522276 feast-0.9.9/feast/contrib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.522276 feast-0.9.9/feast/contrib/validation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/contrib/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-07-14 02:36:03.000000 feast-0.9.9/feast/contrib/validation/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6822 2022-07-14 02:36:03.000000 feast-0.9.9/feast/contrib/validation/ge.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.526276 feast-0.9.9/feast/core/
+-rw-r--r--   0 runner    (1001) docker     (121)    84314 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/CoreService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28802 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/CoreService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    34146 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/CoreService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9142 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/DataFormat_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3653 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/DataFormat_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/DataFormat_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20067 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/DataSource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8548 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/DataSource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/DataSource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9995 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/Entity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4205 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/Entity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/Entity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14873 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/FeatureTable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/FeatureTable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/FeatureTable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5531 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/Feature_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/Feature_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/Feature_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44707 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/JobService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15567 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/JobService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    11486 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/JobService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4646 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/OnlineStore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/OnlineStore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/OnlineStore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19308 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/Store_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8306 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/Store_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/Store_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3748 2022-07-14 02:36:03.000000 feast-0.9.9/feast/data_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22924 2022-07-14 02:36:03.000000 feast-0.9.9/feast/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8342 2022-07-14 02:36:03.000000 feast-0.9.9/feast/entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5403 2022-07-14 02:36:03.000000 feast-0.9.9/feast/feature.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13506 2022-07-14 02:36:03.000000 feast-0.9.9/feast/feature_table.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.526276 feast-0.9.9/feast/grpc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8960 2022-07-14 02:36:03.000000 feast-0.9.9/feast/grpc/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-07-14 02:36:03.000000 feast-0.9.9/feast/grpc/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13162 2022-07-14 02:36:03.000000 feast-0.9.9/feast/job_service.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.526276 feast-0.9.9/feast/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6979 2022-07-14 02:36:03.000000 feast-0.9.9/feast/loaders/abstract_producer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5120 2022-07-14 02:36:03.000000 feast-0.9.9/feast/loaders/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7802 2022-07-14 02:36:03.000000 feast-0.9.9/feast/loaders/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-07-14 02:36:03.000000 feast-0.9.9/feast/loaders/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-07-14 02:36:03.000000 feast-0.9.9/feast/online_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3429 2022-07-14 02:36:03.000000 feast-0.9.9/feast/online_store.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.518276 feast-0.9.9/feast/protos/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.518276 feast-0.9.9/feast/protos/feast/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/protos/feast/core/
+-rw-r--r--   0 runner    (1001) docker     (121)    68096 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/CoreService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21424 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/CoreService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    27156 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/CoreService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9180 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/DataFormat_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3227 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/DataFormat_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/DataFormat_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20589 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/DataSource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7795 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/DataSource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/DataSource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10507 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Entity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3801 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Entity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Entity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13979 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/FeatureTable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5285 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/FeatureTable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/FeatureTable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12739 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/FeatureView_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4775 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/FeatureView_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/FeatureView_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5581 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Feature_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Feature_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Feature_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5918 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Registry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Registry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Registry_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18548 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Store_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7070 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Store_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/core/Store_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/protos/feast/serving/
+-rw-r--r--   0 runner    (1001) docker     (121)    27682 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/serving/ServingService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9406 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/serving/ServingService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     4661 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/serving/ServingService_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/protos/feast/storage/
+-rw-r--r--   0 runner    (1001) docker     (121)     3710 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/storage/Redis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1313 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/storage/Redis_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/storage/Redis_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/protos/feast/types/
+-rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/types/EntityKey_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/types/EntityKey_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/types/EntityKey_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2963 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/types/Field_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/types/Field_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/types/Field_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24401 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/types/Value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9033 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/types/Value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-07-14 02:36:03.000000 feast-0.9.9/feast/protos/feast/types/Value_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/pyspark/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18519 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28492 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/historical_feature_retrieval_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13094 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/pyspark/launchers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/pyspark/launchers/aws/
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12919 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/aws/emr.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11419 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/aws/emr_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/pyspark/launchers/gcloud/
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/gcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16888 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/gcloud/dataproc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/pyspark/launchers/k8s/
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14162 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/k8s/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8862 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/k8s/k8s_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/pyspark/launchers/standalone/
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/standalone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11725 2022-07-14 02:36:03.000000 feast-0.9.9/feast/pyspark/launchers/standalone/local.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6786 2022-07-14 02:36:03.000000 feast-0.9.9/feast/remote_job.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/serving/
+-rw-r--r--   0 runner    (1001) docker     (121)    35691 2022-07-14 02:36:03.000000 feast-0.9.9/feast/serving/ServingService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13543 2022-07-14 02:36:03.000000 feast-0.9.9/feast/serving/ServingService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6459 2022-07-14 02:36:03.000000 feast-0.9.9/feast/serving/ServingService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/serving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/staging/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4765 2022-07-14 02:36:03.000000 feast-0.9.9/feast/staging/entities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17695 2022-07-14 02:36:03.000000 feast-0.9.9/feast/staging/storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/storage/
+-rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-07-14 02:36:03.000000 feast-0.9.9/feast/storage/Redis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-07-14 02:36:03.000000 feast-0.9.9/feast/storage/Redis_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-07-14 02:36:03.000000 feast-0.9.9/feast/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.530276 feast-0.9.9/feast/third_party/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.534276 feast-0.9.9/feast/third_party/grpc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/third_party/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.534276 feast-0.9.9/feast/third_party/grpc/health/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/third_party/grpc/health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.534276 feast-0.9.9/feast/third_party/grpc/health/v1/
+-rw-r--r--   0 runner    (1001) docker     (121)     5835 2022-07-14 02:36:03.000000 feast-0.9.9/feast/third_party/grpc/health/v1/HealthService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-07-14 02:36:03.000000 feast-0.9.9/feast/third_party/grpc/health/v1/HealthService_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     2867 2022-07-14 02:36:03.000000 feast-0.9.9/feast/third_party/grpc/health/v1/HealthService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/third_party/grpc/health/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16331 2022-07-14 02:36:03.000000 feast-0.9.9/feast/type_map.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.534276 feast-0.9.9/feast/types/
+-rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-07-14 02:36:03.000000 feast-0.9.9/feast/types/Field_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-07-14 02:36:03.000000 feast-0.9.9/feast/types/Field_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    24363 2022-07-14 02:36:03.000000 feast-0.9.9/feast/types/Value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9934 2022-07-14 02:36:03.000000 feast-0.9.9/feast/types/Value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/feast/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-07-14 02:36:03.000000 feast-0.9.9/feast/value_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-07-14 02:36:03.000000 feast-0.9.9/feast/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.522276 feast-0.9.9/feast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    12154 2022-07-14 02:37:20.000000 feast-0.9.9/feast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6996 2022-07-14 02:37:20.000000 feast-0.9.9/feast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 02:37:20.000000 feast-0.9.9/feast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-07-14 02:37:20.000000 feast-0.9.9/feast.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-07-14 02:37:20.000000 feast-0.9.9/feast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-07-14 02:37:20.000000 feast-0.9.9/feast.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-07-14 02:36:03.000000 feast-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-07-14 02:36:03.000000 feast-0.9.9/requirements-ci.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-07-14 02:36:03.000000 feast-0.9.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2022-07-14 02:37:20.538276 feast-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-07-14 02:36:03.000000 feast-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.534276 feast-0.9.9/telemetry_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     2627 2022-07-14 02:36:03.000000 feast-0.9.9/telemetry_tests/test_telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.534276 feast-0.9.9/tensorflow_metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/tensorflow_metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.534276 feast-0.9.9/tensorflow_metadata/proto/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/tensorflow_metadata/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.534276 feast-0.9.9/tensorflow_metadata/proto/v0/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/tensorflow_metadata/proto/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-07-14 02:36:03.000000 feast-0.9.9/tensorflow_metadata/proto/v0/path_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-07-14 02:36:03.000000 feast-0.9.9/tensorflow_metadata/proto/v0/path_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)   107849 2022-07-14 02:36:03.000000 feast-0.9.9/tensorflow_metadata/proto/v0/schema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41992 2022-07-14 02:36:03.000000 feast-0.9.9/tensorflow_metadata/proto/v0/schema_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    87532 2022-07-14 02:36:03.000000 feast-0.9.9/tensorflow_metadata/proto/v0/statistics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31328 2022-07-14 02:36:03.000000 feast-0.9.9/tensorflow_metadata/proto/v0/statistics_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.534276 feast-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      813 2022-07-14 02:36:03.000000 feast-0.9.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.538276 feast-0.9.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     7059 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/austin_bikeshare.bikeshare_stations.avro
+-rw-r--r--   0 runner    (1001) docker     (121)      348 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/bookings.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/column_mapping_test_entity.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      338 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/column_mapping_test_feature.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/customer_driver_pairs.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/customers.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     7939 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/dev_featuretable.csv
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/driver_features.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/localhost.crt
+-rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/localhost.key
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/localhost.pem
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.538276 feast-0.9.9/tests/data/tensorflow_metadata/
+-rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/tensorflow_metadata/bikeshare_feature_set.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/tensorflow_metadata/bikeshare_schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2022-07-14 02:36:03.000000 feast-0.9.9/tests/data/transactions.csv
+-rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-07-14 02:36:03.000000 feast-0.9.9/tests/dataframes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5496 2022-07-14 02:36:03.000000 feast-0.9.9/tests/feast_core_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-07-14 02:36:03.000000 feast-0.9.9/tests/feast_serving_server.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.538276 feast-0.9.9/tests/grpc/
+-rw-r--r--   0 runner    (1001) docker     (121)     5872 2022-07-14 02:36:03.000000 feast-0.9.9/tests/grpc/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 02:37:20.538276 feast-0.9.9/tests/loaders/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 02:36:03.000000 feast-0.9.9/tests/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-07-14 02:36:03.000000 feast-0.9.9/tests/loaders/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26658 2022-07-14 02:36:03.000000 feast-0.9.9/tests/test_as_of_join.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33588 2022-07-14 02:36:03.000000 feast-0.9.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5203 2022-07-14 02:36:03.000000 feast-0.9.9/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2767 2022-07-14 02:36:03.000000 feast-0.9.9/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-07-14 02:36:03.000000 feast-0.9.9/tests/test_feature_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17523 2022-07-14 02:36:03.000000 feast-0.9.9/tests/test_historical_feature_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2270 2022-07-14 02:36:03.000000 feast-0.9.9/tests/test_remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6857 2022-07-14 02:36:03.000000 feast-0.9.9/tests/test_streaming_control_loop.py
```

### Comparing `feast-0.9.8/.gitignore` & `feast-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/PKG-INFO` & `feast-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feast
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python SDK for Feast
 Home-page: https://github.com/feast-dev/feast
 Author: Feast
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: feast Version: 0.9.8 Summary: Python SDK for Feast
+Metadata-Version: 2.1 Name: feast Version: 0.9.9 Summary: Python SDK for Feast
 Home-page: https://github.com/feast-dev/feast Author: Feast License: Apache
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
 validation
                          [docs/assets/feast_logo.png]
```

### Comparing `feast-0.9.8/docs/Makefile` & `feast-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/conf.py` & `feast-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/index.rst` & `feast-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/conf.py` & `feast-0.9.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.contrib.validation.rst` & `feast-0.9.9/docs/source/feast.contrib.validation.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.core.rst` & `feast-0.9.9/docs/source/feast.core.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.loaders.rst` & `feast-0.9.9/docs/source/feast.loaders.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.pyspark.launchers.aws.rst` & `feast-0.9.9/docs/source/feast.pyspark.launchers.aws.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.pyspark.launchers.k8s.rst` & `feast-0.9.9/docs/source/feast.pyspark.launchers.k8s.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.pyspark.rst` & `feast-0.9.9/docs/source/feast.pyspark.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.rst` & `feast-0.9.9/docs/source/feast.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.serving.rst` & `feast-0.9.9/docs/source/feast.serving.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.staging.rst` & `feast-0.9.9/docs/source/feast.staging.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/feast.third_party.grpc.health.v1.rst` & `feast-0.9.9/docs/source/feast.third_party.grpc.health.v1.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/docs/source/index.rst` & `feast-0.9.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/__init__.py` & `feast-0.9.9/feast/__init__.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/cli.py` & `feast-0.9.9/feast/cli.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/client.py` & `feast-0.9.9/feast/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,32 +28,36 @@
 from feast.config import Config
 from feast.constants import ConfigOptions as opt
 from feast.core.CoreService_pb2 import (
     ApplyEntityRequest,
     ApplyEntityResponse,
     ApplyFeatureTableRequest,
     ApplyFeatureTableResponse,
+    ArchiveOnlineStoreRequest,
+    ArchiveOnlineStoreResponse,
     ArchiveProjectRequest,
-    ArchiveProjectResponse,
     CreateProjectRequest,
-    CreateProjectResponse,
     DeleteFeatureTableRequest,
     GetEntityRequest,
     GetEntityResponse,
     GetFeastCoreVersionRequest,
     GetFeatureTableRequest,
     GetFeatureTableResponse,
+    GetOnlineStoreRequest,
     ListEntitiesRequest,
     ListEntitiesResponse,
     ListFeaturesRequest,
     ListFeaturesResponse,
     ListFeatureTablesRequest,
     ListFeatureTablesResponse,
+    ListOnlineStoresRequest,
     ListProjectsRequest,
     ListProjectsResponse,
+    RegisterOnlineStoreRequest,
+    RegisterOnlineStoreResponse,
 )
 from feast.core.CoreService_pb2_grpc import CoreServiceStub
 from feast.core.JobService_pb2 import (
     GetHistoricalFeaturesRequest,
     GetJobRequest,
     ListJobsRequest,
     StartOfflineToOnlineIngestionJobRequest,
@@ -72,14 +76,15 @@
     _read_table_from_source,
     _upload_to_bq_source,
     _upload_to_file_source,
     _write_non_partitioned_table_from_source,
     _write_partitioned_table_from_source,
 )
 from feast.online_response import OnlineResponse, _infer_online_entity_rows
+from feast.online_store import OnlineStore
 from feast.pyspark.abc import RetrievalJob, SparkJob
 from feast.pyspark.launcher import (
     get_job_by_id,
     list_jobs,
     stage_dataframe,
     start_historical_feature_retrieval_job,
     start_historical_feature_retrieval_spark_session,
@@ -454,15 +459,15 @@
             project: Name of project
         """
 
         self._core_service.CreateProject(
             CreateProjectRequest(name=project),
             timeout=self._config.getint(opt.GRPC_CONNECTION_TIMEOUT),
             metadata=self._get_grpc_metadata(),
-        )  # type: CreateProjectResponse
+        )
 
     def archive_project(self, project):
         """
         Archives a project. Project will still continue to function for
         ingestion and retrieval, but will be in a read-only state. It will
         also not be visible from the Core API for management purposes.
 
@@ -471,15 +476,15 @@
         """
 
         try:
             self._core_service_stub.ArchiveProject(
                 ArchiveProjectRequest(name=project),
                 timeout=self._config.getint(opt.GRPC_CONNECTION_TIMEOUT),
                 metadata=self._get_grpc_metadata(),
-            )  # type: ArchiveProjectResponse
+            )
         except grpc.RpcError as e:
             raise grpc.RpcError(e.details())
 
         # revert to the default project
         if self._project == project:
             self._project = opt().PROJECT
 
@@ -1294,7 +1299,45 @@
                 self._job_service, self._extra_grpc_params, response.job
             )
 
     def stage_dataframe(
         self, df: pd.DataFrame, event_timestamp_column: str,
     ) -> FileSource:
         return stage_dataframe(df, event_timestamp_column, self._config)
+
+    def register_online_store(
+        self, online_store: OnlineStore
+    ) -> RegisterOnlineStoreResponse:
+        try:
+            response = self._core_service.RegisterOnlineStore(
+                RegisterOnlineStoreRequest(online_store=online_store.to_proto())
+            )
+        except grpc.RpcError as e:
+            raise grpc.RpcError(e.details())
+        return response
+
+    def list_online_stores(self) -> List[OnlineStore]:
+        try:
+            response = self._core_service.ListOnlineStores(ListOnlineStoresRequest())
+        except grpc.RpcError as e:
+            raise grpc.RpcError(e.details())
+
+        return [OnlineStore.from_proto(proto) for proto in response.online_store]
+
+    def get_online_store(self, name: str) -> OnlineStore:
+        try:
+            response = self._core_service.GetOnlineStore(
+                GetOnlineStoreRequest(name=name)
+            )
+        except grpc.RpcError as e:
+            raise grpc.RpcError(e.details())
+
+        return OnlineStore.from_proto(response.online_store)
+
+    def archive_online_store(self, name: str) -> ArchiveOnlineStoreResponse:
+        try:
+            response = self._core_service.ArchiveOnlineStore(
+                ArchiveOnlineStoreRequest(name=name)
+            )
+        except grpc.RpcError as e:
+            raise grpc.RpcError(e.details())
+        return response
```

### Comparing `feast-0.9.8/feast/config.py` & `feast-0.9.9/feast/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,49 +135,49 @@
         Returns: String option that is returned
 
         """
         return self._get(option, default, self._config.get)
 
     def getboolean(self, option, default=_UNSET):
         """
-         Returns a single configuration option as a boolean
+        Returns a single configuration option as a boolean
 
-         Args:
-             option: Name of the option
-             default: Default value to return if option is not found
+        Args:
+            option: Name of the option
+            default: Default value to return if option is not found
 
-         Returns: Boolean option value that is returned
+        Returns: Boolean option value that is returned
 
-         """
+        """
         return self._get(option, default, self._config.getboolean)
 
     def getint(self, option, default=_UNSET):
         """
-         Returns a single configuration option as an integer
+        Returns a single configuration option as an integer
 
-         Args:
-             option: Name of the option
-             default: Default value to return if option is not found
+        Args:
+            option: Name of the option
+            default: Default value to return if option is not found
 
-         Returns: Integer option value that is returned
+        Returns: Integer option value that is returned
 
-         """
+        """
         return self._get(option, default, self._config.getint)
 
     def getfloat(self, option, default=_UNSET):
         """
-         Returns a single configuration option as an integer
+        Returns a single configuration option as an integer
 
-         Args:
-             option: Name of the option
-             default: Default value to return if option is not found
+        Args:
+            option: Name of the option
+            default: Default value to return if option is not found
 
-         Returns: Float option value that is returned
+        Returns: Float option value that is returned
 
-         """
+        """
         return self._get(option, default, self._config.getfloat)
 
     def set(self, option, value):
         """
         Sets a configuration option. Must be serializable to string
         Args:
             option: Option name to use as key
```

### Comparing `feast-0.9.8/feast/constants.py` & `feast-0.9.9/feast/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 CONFIG_FILE_SECTION: str = "general"
 
 # Maximum interval(secs) to wait between retries for retry function
 MAX_WAIT_INTERVAL: str = "60"
 
 
 class ConfigOptions(metaclass=ConfigMeta):
-    """ Feast Configuration Options """
+    """Feast Configuration Options"""
 
     #: Feast project namespace to use
     PROJECT: str = "default"
 
     #: Default Feast Core URL
     CORE_URL: str = "localhost:6565"
```

### Comparing `feast-0.9.8/feast/contrib/validation/ge.py` & `feast-0.9.9/feast/contrib/validation/ge.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/CoreService_pb2.py` & `feast-0.9.9/feast/protos/feast/core/CoreService_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: feast/core/CoreService.proto
-
+"""Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from tensorflow_metadata.proto.v0 import statistics_pb2 as tensorflow__metadata_dot_proto_dot_v0_dot_statistics__pb2
-from feast.core import Entity_pb2 as feast_dot_core_dot_Entity__pb2
-from feast.core import Feature_pb2 as feast_dot_core_dot_Feature__pb2
-from feast.core import FeatureTable_pb2 as feast_dot_core_dot_FeatureTable__pb2
-from feast.core import Store_pb2 as feast_dot_core_dot_Store__pb2
 
+from feast.protos.feast.core import Entity_pb2 as feast_dot_core_dot_Entity__pb2
+from feast.protos.feast.core import Feature_pb2 as feast_dot_core_dot_Feature__pb2
+from feast.protos.feast.core import (
+    FeatureTable_pb2 as feast_dot_core_dot_FeatureTable__pb2,
+)
+from feast.protos.feast.core import Store_pb2 as feast_dot_core_dot_Store__pb2
+from tensorflow_metadata.proto.v0 import (
+    statistics_pb2 as tensorflow__metadata_dot_proto_dot_v0_dot_statistics__pb2,
+)
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='feast/core/CoreService.proto',
   package='feast.core',
   syntax='proto3',
   serialized_options=b'\n\020feast.proto.coreB\020CoreServiceProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/core',
   create_key=_descriptor._internal_create_key,
```

### Comparing `feast-0.9.8/feast/core/CoreService_pb2.pyi` & `feast-0.9.9/feast/protos/feast/core/CoreService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/CoreService_pb2_grpc.py` & `feast-0.9.9/feast/protos/feast/core/CoreService_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from feast.core import CoreService_pb2 as feast_dot_core_dot_CoreService__pb2
+from feast.protos.feast.core import (
+    CoreService_pb2 as feast_dot_core_dot_CoreService__pb2,
+)
 
 
 class CoreServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `feast-0.9.8/feast/core/DataFormat_pb2.py` & `feast-0.9.9/feast/core/DataFormat_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/DataFormat_pb2.pyi` & `feast-0.9.9/feast/protos/feast/core/DataFormat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/DataSource_pb2.py` & `feast-0.9.9/feast/core/DataSource_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/DataSource_pb2.pyi` & `feast-0.9.9/feast/protos/feast/core/DataSource_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -60,21 +60,24 @@
             ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal[u"file_format",b"file_format"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal[u"file_format",b"file_format",u"file_url",b"file_url"]) -> None: ...
 
     class BigQueryOptions(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         TABLE_REF_FIELD_NUMBER: builtins.int
+        QUERY_FIELD_NUMBER: builtins.int
         table_ref: typing.Text = ...
+        query: typing.Text = ...
 
         def __init__(self,
             *,
             table_ref : typing.Text = ...,
+            query : typing.Text = ...,
             ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"table_ref",b"table_ref"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal[u"query",b"query",u"table_ref",b"table_ref"]) -> None: ...
 
     class KafkaOptions(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         BOOTSTRAP_SERVERS_FIELD_NUMBER: builtins.int
         TOPIC_FIELD_NUMBER: builtins.int
         MESSAGE_FORMAT_FIELD_NUMBER: builtins.int
         bootstrap_servers: typing.Text = ...
```

### Comparing `feast-0.9.8/feast/core/Entity_pb2.py` & `feast-0.9.9/feast/core/Entity_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/Entity_pb2.pyi` & `feast-0.9.9/feast/protos/feast/core/Entity_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -46,32 +46,35 @@
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
     VALUE_TYPE_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     LABELS_FIELD_NUMBER: builtins.int
     name: typing.Text = ...
+    project: typing.Text = ...
     value_type: feast.types.Value_pb2.ValueType.Enum.V = ...
     description: typing.Text = ...
 
     @property
     def labels(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
 
     def __init__(self,
         *,
         name : typing.Text = ...,
+        project : typing.Text = ...,
         value_type : feast.types.Value_pb2.ValueType.Enum.V = ...,
         description : typing.Text = ...,
         labels : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"description",b"description",u"labels",b"labels",u"name",b"name",u"value_type",b"value_type"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal[u"description",b"description",u"labels",b"labels",u"name",b"name",u"project",b"project",u"value_type",b"value_type"]) -> None: ...
 global___EntitySpecV2 = EntitySpecV2
 
 class EntityMeta(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     CREATED_TIMESTAMP_FIELD_NUMBER: builtins.int
     LAST_UPDATED_TIMESTAMP_FIELD_NUMBER: builtins.int
```

### Comparing `feast-0.9.8/feast/core/FeatureTable_pb2.py` & `feast-0.9.9/feast/protos/feast/core/FeatureTable_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: feast/core/FeatureTable.proto
-
+"""Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
+
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from feast.core import DataSource_pb2 as feast_dot_core_dot_DataSource__pb2
-from feast.core import Feature_pb2 as feast_dot_core_dot_Feature__pb2
 
+from feast.protos.feast.core import DataSource_pb2 as feast_dot_core_dot_DataSource__pb2
+from feast.protos.feast.core import Feature_pb2 as feast_dot_core_dot_Feature__pb2
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='feast/core/FeatureTable.proto',
   package='feast.core',
   syntax='proto3',
   serialized_options=b'\n\020feast.proto.coreB\021FeatureTableProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/core',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1d\x66\x65\x61st/core/FeatureTable.proto\x12\nfeast.core\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1b\x66\x65\x61st/core/DataSource.proto\x1a\x18\x66\x65\x61st/core/Feature.proto\"f\n\x0c\x46\x65\x61tureTable\x12*\n\x04spec\x18\x01 \x01(\x0b\x32\x1c.feast.core.FeatureTableSpec\x12*\n\x04meta\x18\x02 \x01(\x0b\x32\x1c.feast.core.FeatureTableMeta\"\xd1\x02\n\x10\x46\x65\x61tureTableSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x65ntities\x18\x03 \x03(\t\x12+\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32\x19.feast.core.FeatureSpecV2\x12\x38\n\x06labels\x18\x05 \x03(\x0b\x32(.feast.core.FeatureTableSpec.LabelsEntry\x12*\n\x07max_age\x18\x06 \x01(\x0b\x32\x19.google.protobuf.Duration\x12,\n\x0c\x62\x61tch_source\x18\x07 \x01(\x0b\x32\x16.feast.core.DataSource\x12-\n\rstream_source\x18\x08 \x01(\x0b\x32\x16.feast.core.DataSource\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa5\x01\n\x10\x46\x65\x61tureTableMeta\x12\x35\n\x11\x63reated_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_updated_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08revision\x18\x03 \x01(\x03\x12\x0c\n\x04hash\x18\x04 \x01(\tBZ\n\x10\x66\x65\x61st.proto.coreB\x11\x46\x65\x61tureTableProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/coreb\x06proto3'
+  serialized_pb=b'\n\x1d\x66\x65\x61st/core/FeatureTable.proto\x12\nfeast.core\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1b\x66\x65\x61st/core/DataSource.proto\x1a\x18\x66\x65\x61st/core/Feature.proto\"f\n\x0c\x46\x65\x61tureTable\x12*\n\x04spec\x18\x01 \x01(\x0b\x32\x1c.feast.core.FeatureTableSpec\x12*\n\x04meta\x18\x02 \x01(\x0b\x32\x1c.feast.core.FeatureTableMeta\"\xe2\x02\n\x10\x46\x65\x61tureTableSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07project\x18\t \x01(\t\x12\x10\n\x08\x65ntities\x18\x03 \x03(\t\x12+\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32\x19.feast.core.FeatureSpecV2\x12\x38\n\x06labels\x18\x05 \x03(\x0b\x32(.feast.core.FeatureTableSpec.LabelsEntry\x12*\n\x07max_age\x18\x06 \x01(\x0b\x32\x19.google.protobuf.Duration\x12,\n\x0c\x62\x61tch_source\x18\x07 \x01(\x0b\x32\x16.feast.core.DataSource\x12-\n\rstream_source\x18\x08 \x01(\x0b\x32\x16.feast.core.DataSource\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa5\x01\n\x10\x46\x65\x61tureTableMeta\x12\x35\n\x11\x63reated_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_updated_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08revision\x18\x03 \x01(\x03\x12\x0c\n\x04hash\x18\x04 \x01(\tBZ\n\x10\x66\x65\x61st.proto.coreB\x11\x46\x65\x61tureTableProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/coreb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,feast_dot_core_dot_DataSource__pb2.DESCRIPTOR,feast_dot_core_dot_Feature__pb2.DESCRIPTOR,])
 
 
 
 
 _FEATURETABLE = _descriptor.Descriptor(
@@ -99,16 +100,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=562,
-  serialized_end=607,
+  serialized_start=579,
+  serialized_end=624,
 )
 
 _FEATURETABLESPEC = _descriptor.Descriptor(
   name='FeatureTableSpec',
   full_name='feast.core.FeatureTableSpec',
   filename=None,
   file=DESCRIPTOR,
@@ -119,50 +120,57 @@
       name='name', full_name='feast.core.FeatureTableSpec.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='entities', full_name='feast.core.FeatureTableSpec.entities', index=1,
+      name='project', full_name='feast.core.FeatureTableSpec.project', index=1,
+      number=9, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='entities', full_name='feast.core.FeatureTableSpec.entities', index=2,
       number=3, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='features', full_name='feast.core.FeatureTableSpec.features', index=2,
+      name='features', full_name='feast.core.FeatureTableSpec.features', index=3,
       number=4, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='labels', full_name='feast.core.FeatureTableSpec.labels', index=3,
+      name='labels', full_name='feast.core.FeatureTableSpec.labels', index=4,
       number=5, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='max_age', full_name='feast.core.FeatureTableSpec.max_age', index=4,
+      name='max_age', full_name='feast.core.FeatureTableSpec.max_age', index=5,
       number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='batch_source', full_name='feast.core.FeatureTableSpec.batch_source', index=5,
+      name='batch_source', full_name='feast.core.FeatureTableSpec.batch_source', index=6,
       number=7, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='stream_source', full_name='feast.core.FeatureTableSpec.stream_source', index=6,
+      name='stream_source', full_name='feast.core.FeatureTableSpec.stream_source', index=7,
       number=8, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
@@ -173,15 +181,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=270,
-  serialized_end=607,
+  serialized_end=624,
 )
 
 
 _FEATURETABLEMETA = _descriptor.Descriptor(
   name='FeatureTableMeta',
   full_name='feast.core.FeatureTableMeta',
   filename=None,
@@ -225,16 +233,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=610,
-  serialized_end=775,
+  serialized_start=627,
+  serialized_end=792,
 )
 
 _FEATURETABLE.fields_by_name['spec'].message_type = _FEATURETABLESPEC
 _FEATURETABLE.fields_by_name['meta'].message_type = _FEATURETABLEMETA
 _FEATURETABLESPEC_LABELSENTRY.containing_type = _FEATURETABLESPEC
 _FEATURETABLESPEC.fields_by_name['features'].message_type = feast_dot_core_dot_Feature__pb2._FEATURESPECV2
 _FEATURETABLESPEC.fields_by_name['labels'].message_type = _FEATURETABLESPEC_LABELSENTRY
```

### Comparing `feast-0.9.8/feast/core/FeatureTable_pb2.pyi` & `feast-0.9.9/feast/protos/feast/core/FeatureTable_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -48,21 +48,23 @@
             *,
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
     ENTITIES_FIELD_NUMBER: builtins.int
     FEATURES_FIELD_NUMBER: builtins.int
     LABELS_FIELD_NUMBER: builtins.int
     MAX_AGE_FIELD_NUMBER: builtins.int
     BATCH_SOURCE_FIELD_NUMBER: builtins.int
     STREAM_SOURCE_FIELD_NUMBER: builtins.int
     name: typing.Text = ...
+    project: typing.Text = ...
     entities: google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text] = ...
 
     @property
     def features(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[feast.core.Feature_pb2.FeatureSpecV2]: ...
 
     @property
     def labels(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
@@ -75,23 +77,24 @@
 
     @property
     def stream_source(self) -> feast.core.DataSource_pb2.DataSource: ...
 
     def __init__(self,
         *,
         name : typing.Text = ...,
+        project : typing.Text = ...,
         entities : typing.Optional[typing.Iterable[typing.Text]] = ...,
         features : typing.Optional[typing.Iterable[feast.core.Feature_pb2.FeatureSpecV2]] = ...,
         labels : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
         max_age : typing.Optional[google.protobuf.duration_pb2.Duration] = ...,
         batch_source : typing.Optional[feast.core.DataSource_pb2.DataSource] = ...,
         stream_source : typing.Optional[feast.core.DataSource_pb2.DataSource] = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal[u"batch_source",b"batch_source",u"max_age",b"max_age",u"stream_source",b"stream_source"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"batch_source",b"batch_source",u"entities",b"entities",u"features",b"features",u"labels",b"labels",u"max_age",b"max_age",u"name",b"name",u"stream_source",b"stream_source"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal[u"batch_source",b"batch_source",u"entities",b"entities",u"features",b"features",u"labels",b"labels",u"max_age",b"max_age",u"name",b"name",u"project",b"project",u"stream_source",b"stream_source"]) -> None: ...
 global___FeatureTableSpec = FeatureTableSpec
 
 class FeatureTableMeta(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     CREATED_TIMESTAMP_FIELD_NUMBER: builtins.int
     LAST_UPDATED_TIMESTAMP_FIELD_NUMBER: builtins.int
     REVISION_FIELD_NUMBER: builtins.int
```

### Comparing `feast-0.9.8/feast/core/Feature_pb2.py` & `feast-0.9.9/feast/core/Feature_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/Feature_pb2.pyi` & `feast-0.9.9/feast/protos/feast/core/Feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/JobService_pb2.py` & `feast-0.9.9/feast/core/JobService_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/JobService_pb2_grpc.py` & `feast-0.9.9/feast/core/JobService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/Store_pb2.py` & `feast-0.9.9/feast/core/Store_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/core/Store_pb2.pyi` & `feast-0.9.9/feast/protos/feast/core/Store_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
-import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
@@ -71,41 +70,35 @@
         INITIAL_BACKOFF_MS_FIELD_NUMBER: builtins.int
         MAX_RETRIES_FIELD_NUMBER: builtins.int
         FLUSH_FREQUENCY_SECONDS_FIELD_NUMBER: builtins.int
         KEY_PREFIX_FIELD_NUMBER: builtins.int
         ENABLE_FALLBACK_FIELD_NUMBER: builtins.int
         FALLBACK_PREFIX_FIELD_NUMBER: builtins.int
         READ_FROM_FIELD_NUMBER: builtins.int
-        TIMEOUT_FIELD_NUMBER: builtins.int
         connection_string: typing.Text = ...
         initial_backoff_ms: builtins.int = ...
         max_retries: builtins.int = ...
         flush_frequency_seconds: builtins.int = ...
         key_prefix: typing.Text = ...
         enable_fallback: builtins.bool = ...
         fallback_prefix: typing.Text = ...
         read_from: global___Store.RedisClusterConfig.ReadFrom.V = ...
 
-        @property
-        def timeout(self) -> google.protobuf.duration_pb2.Duration: ...
-
         def __init__(self,
             *,
             connection_string : typing.Text = ...,
             initial_backoff_ms : builtins.int = ...,
             max_retries : builtins.int = ...,
             flush_frequency_seconds : builtins.int = ...,
             key_prefix : typing.Text = ...,
             enable_fallback : builtins.bool = ...,
             fallback_prefix : typing.Text = ...,
             read_from : global___Store.RedisClusterConfig.ReadFrom.V = ...,
-            timeout : typing.Optional[google.protobuf.duration_pb2.Duration] = ...,
             ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal[u"timeout",b"timeout"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"connection_string",b"connection_string",u"enable_fallback",b"enable_fallback",u"fallback_prefix",b"fallback_prefix",u"flush_frequency_seconds",b"flush_frequency_seconds",u"initial_backoff_ms",b"initial_backoff_ms",u"key_prefix",b"key_prefix",u"max_retries",b"max_retries",u"read_from",b"read_from",u"timeout",b"timeout"]) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal[u"connection_string",b"connection_string",u"enable_fallback",b"enable_fallback",u"fallback_prefix",b"fallback_prefix",u"flush_frequency_seconds",b"flush_frequency_seconds",u"initial_backoff_ms",b"initial_backoff_ms",u"key_prefix",b"key_prefix",u"max_retries",b"max_retries",u"read_from",b"read_from"]) -> None: ...
 
     class Subscription(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         PROJECT_FIELD_NUMBER: builtins.int
         NAME_FIELD_NUMBER: builtins.int
         EXCLUDE_FIELD_NUMBER: builtins.int
         project: typing.Text = ...
```

### Comparing `feast-0.9.8/feast/data_format.py` & `feast-0.9.9/feast/data_format.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/data_source.py` & `feast-0.9.9/feast/data_source.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/entity.py` & `feast-0.9.9/feast/entity.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/feature.py` & `feast-0.9.9/feast/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             labels=feature_proto.labels,
         )
 
         return feature
 
 
 class FeatureRef:
-    """ Feature Reference represents a reference to a specific feature. """
+    """Feature Reference represents a reference to a specific feature."""
 
     def __init__(self, name: str, feature_table: str = None):
         self.proto = FeatureRefProto(name=name, feature_table=feature_table)
 
     @classmethod
     def from_proto(cls, proto: FeatureRefProto):
         """
```

### Comparing `feast-0.9.8/feast/feature_table.py` & `feast-0.9.9/feast/feature_table.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, List, MutableMapping, Optional, Union
 
 import yaml
 from google.protobuf import json_format
-from google.protobuf.duration_pb2 import Duration
+from google.protobuf.internal.well_known_types import Duration, Timestamp
 from google.protobuf.json_format import MessageToDict, MessageToJson
-from google.protobuf.timestamp_pb2 import Timestamp
 
 from feast.core.FeatureTable_pb2 import FeatureTable as FeatureTableProto
 from feast.core.FeatureTable_pb2 import FeatureTableMeta as FeatureTableMetaProto
 from feast.core.FeatureTable_pb2 import FeatureTableSpec as FeatureTableSpecProto
 from feast.data_source import (
     BigQuerySource,
     DataSource,
     FileSource,
     KafkaSource,
     KinesisSource,
 )
 from feast.feature import Feature
 from feast.loaders import yaml as feast_yaml
+from feast.online_store import OnlineStore
 from feast.value_type import ValueType
 
 
 class FeatureTable:
     """
     Represents a collection of features and associated metadata.
     """
@@ -45,28 +45,30 @@
         name: str,
         entities: List[str],
         features: List[Feature],
         batch_source: Union[BigQuerySource, FileSource] = None,
         stream_source: Optional[Union[KafkaSource, KinesisSource]] = None,
         max_age: Optional[Duration] = None,
         labels: Optional[MutableMapping[str, str]] = None,
+        online_store: Optional[OnlineStore] = None,
     ):
         self._name = name
         self._entities = entities
         self._features = features
         self._batch_source = batch_source
         self._stream_source = stream_source
         if labels is None:
             self._labels = dict()  # type: MutableMapping[str, str]
         else:
             self._labels = labels
 
         self._max_age = max_age
         self._created_timestamp: Optional[Timestamp] = None
         self._last_updated_timestamp: Optional[Timestamp] = None
+        self._online_store = online_store
 
     def __str__(self):
         return str(MessageToJson(self.to_proto()))
 
     def __eq__(self, other):
         if not isinstance(other, FeatureTable):
             raise TypeError(
@@ -84,14 +86,16 @@
             return False
         if sorted(self.features) != sorted(other.features):
             return False
         if self.batch_source != other.batch_source:
             return False
         if self.stream_source != other.stream_source:
             return False
+        if self._online_store != other._online_store:
+            return False
 
         return True
 
     @property
     def name(self):
         """
         Returns the name of this feature table
@@ -202,14 +206,28 @@
     @property
     def last_updated_timestamp(self):
         """
         Returns the last_updated_timestamp of this feature table
         """
         return self._last_updated_timestamp
 
+    @property
+    def online_store(self):
+        """
+        Returns the online store of this feature table
+        """
+        return self._online_store
+
+    @online_store.setter
+    def online_store(self, online_store: OnlineStore):
+        """
+        Sets the stream source of this feature table
+        """
+        self._online_store = online_store
+
     def add_feature(self, feature: Feature):
         """
         Adds a new feature to the feature table.
         """
         self.features.append(feature)
 
     def is_valid(self):
@@ -288,23 +306,24 @@
             ),
             batch_source=DataSource.from_proto(feature_table_proto.spec.batch_source),
             stream_source=(
                 None
                 if not feature_table_proto.spec.stream_source.ByteSize()
                 else DataSource.from_proto(feature_table_proto.spec.stream_source)
             ),
+            online_store=OnlineStore.from_proto(feature_table_proto.spec.online_store),
         )
 
         feature_table._created_timestamp = feature_table_proto.meta.created_timestamp
 
         return feature_table
 
     def to_proto(self) -> FeatureTableProto:
         """
-        Converts an feature table object to its protobuf representation
+        Converts a feature table object to its protobuf representation
 
         Returns:
             FeatureTableProto protobuf
         """
 
         meta = FeatureTableMetaProto(
             created_timestamp=self.created_timestamp,
@@ -326,14 +345,17 @@
                 else self.batch_source
             ),
             stream_source=(
                 self.stream_source.to_proto()
                 if issubclass(type(self.stream_source), DataSource)
                 else self.stream_source
             ),
+            online_store=self.online_store.to_proto()
+            if self.online_store is not None
+            else None,
         )
 
         return FeatureTableProto(spec=spec, meta=meta)
 
     def to_spec_proto(self) -> FeatureTableSpecProto:
         """
         Converts an FeatureTableProto object to its protobuf representation.
@@ -358,14 +380,17 @@
                 else self.batch_source
             ),
             stream_source=(
                 self.stream_source.to_proto()
                 if issubclass(type(self.stream_source), DataSource)
                 else self.stream_source
             ),
+            online_store=self.online_store.to_proto()
+            if self.online_store is not None
+            else None,
         )
 
         return spec
 
     def to_dict(self) -> Dict:
         """
         Converts feature table to dict
@@ -400,12 +425,13 @@
         self.name = feature_table.name
         self.entities = feature_table.entities
         self.features = feature_table.features
         self.labels = feature_table.labels
         self.max_age = feature_table.max_age
         self.batch_source = feature_table.batch_source
         self.stream_source = feature_table.stream_source
+        self.online_store = feature_table.online_store
         self._created_timestamp = feature_table.created_timestamp
         self._last_updated_timestamp = feature_table.last_updated_timestamp
 
     def __repr__(self):
         return f"FeatureTable <{self.name}>"
```

### Comparing `feast-0.9.8/feast/grpc/auth.py` & `feast-0.9.9/feast/grpc/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,42 +89,42 @@
                 " Please ensure that the "
                 "necessary parameters are passed to the client - "
                 "oauth_grant_type, oauth_client_id, oauth_client_secret, "
                 "oauth_audience, oauth_token_request_url."
             )
 
     def get_signed_meta(self):
-        """ Creates a signed authorization metadata token."""
+        """Creates a signed authorization metadata token."""
 
         current_time = time.time()
         if current_time > (self._token_expiry_ts - 500):
             self._refresh_token(self._config)
             self._token_expiry_ts = current_time + self._token_expiry_ts
         return (("authorization", "Bearer {}".format(self._token)),)
 
     def _refresh_token(self, config: Config):
-        """ Refreshes OAuth token and persists it in memory """
+        """Refreshes OAuth token and persists it in memory"""
 
         # Use static token if available
         if self._static_token:
             self._token = self._static_token
             return
 
         headers_token = {"content-type": "application/json"}
         data_token = {
             "grant_type": config.get(opt.OAUTH_GRANT_TYPE),
             "client_id": config.get(opt.OAUTH_CLIENT_ID),
             "client_secret": config.get(opt.OAUTH_CLIENT_SECRET),
             "audience": config.get(opt.OAUTH_AUDIENCE),
         }
-        data_token = json.dumps(data_token)
+        data_token_json_string = json.dumps(data_token)
         response_token = requests.post(
             config.get(opt.OAUTH_TOKEN_REQUEST_URL),
             headers=headers_token,
-            data=data_token,
+            data=data_token_json_string,
         )
         if response_token.status_code == HTTPStatus.OK:
             self._token = response_token.json().get("access_token")
             self._token_expiry_ts = response_token.json().get("expires_in")
         else:
             raise RuntimeError(
                 f"Could not fetch OAuth token, got response : {response_token.status_code}"
@@ -174,22 +174,22 @@
         if config.exists(opt.AUTH_TOKEN):
             self._static_token = config.get(opt.AUTH_TOKEN)
 
         self._request = RequestWithTimeout(timeout=5)
         self._refresh_token()
 
     def get_signed_meta(self):
-        """ Creates a signed authorization metadata token."""
+        """Creates a signed authorization metadata token."""
 
         if time.time() > self._token_expiry_ts:
             self._refresh_token()
         return (("authorization", "Bearer {}".format(self._token)),)
 
     def _refresh_token(self):
-        """ Refreshes Google ID token and persists it in memory """
+        """Refreshes Google ID token and persists it in memory"""
 
         # Use static token if available
         if self._static_token:
             self._token = self._static_token
             return
 
         from google.oauth2.id_token import fetch_id_token, verify_oauth2_token
```

### Comparing `feast-0.9.8/feast/grpc/grpc.py` & `feast-0.9.9/feast/grpc/grpc.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/job_service.py` & `feast-0.9.9/feast/job_service.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/loaders/abstract_producer.py` & `feast-0.9.9/feast/loaders/abstract_producer.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/loaders/file.py` & `feast-0.9.9/feast/loaders/file.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/loaders/ingest.py` & `feast-0.9.9/feast/loaders/ingest.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/loaders/yaml.py` & `feast-0.9.9/feast/loaders/yaml.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/online_response.py` & `feast-0.9.9/feast/online_response.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/core/CoreService_pb2.py` & `feast-0.9.9/feast/core/CoreService_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: feast/core/CoreService.proto
-"""Generated protocol buffer code."""
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from tensorflow_metadata.proto.v0 import statistics_pb2 as tensorflow__metadata_dot_proto_dot_v0_dot_statistics__pb2
+from feast.core import Entity_pb2 as feast_dot_core_dot_Entity__pb2
+from feast.core import Feature_pb2 as feast_dot_core_dot_Feature__pb2
+from feast.core import FeatureTable_pb2 as feast_dot_core_dot_FeatureTable__pb2
+from feast.core import Store_pb2 as feast_dot_core_dot_Store__pb2
+from feast.core import OnlineStore_pb2 as feast_dot_core_dot_OnlineStore__pb2
 
-from feast.protos.feast.core import Entity_pb2 as feast_dot_core_dot_Entity__pb2
-from feast.protos.feast.core import Feature_pb2 as feast_dot_core_dot_Feature__pb2
-from feast.protos.feast.core import (
-    FeatureTable_pb2 as feast_dot_core_dot_FeatureTable__pb2,
-)
-from feast.protos.feast.core import Store_pb2 as feast_dot_core_dot_Store__pb2
-from tensorflow_metadata.proto.v0 import (
-    statistics_pb2 as tensorflow__metadata_dot_proto_dot_v0_dot_statistics__pb2,
-)
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='feast/core/CoreService.proto',
   package='feast.core',
   syntax='proto3',
   serialized_options=b'\n\020feast.proto.coreB\020CoreServiceProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/core',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1c\x66\x65\x61st/core/CoreService.proto\x12\nfeast.core\x1a\x1fgoogle/protobuf/timestamp.proto\x1a-tensorflow_metadata/proto/v0/statistics.proto\x1a\x17\x66\x65\x61st/core/Entity.proto\x1a\x18\x66\x65\x61st/core/Feature.proto\x1a\x1d\x66\x65\x61st/core/FeatureTable.proto\x1a\x16\x66\x65\x61st/core/Store.proto\"1\n\x10GetEntityRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07project\x18\x02 \x01(\t\"7\n\x11GetEntityResponse\x12\"\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x12.feast.core.Entity\"\xdc\x01\n\x13ListEntitiesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32&.feast.core.ListEntitiesRequest.Filter\x1a\x8c\x01\n\x06\x46ilter\x12\x0f\n\x07project\x18\x03 \x01(\t\x12\x42\n\x06labels\x18\x04 \x03(\x0b\x32\x32.feast.core.ListEntitiesRequest.Filter.LabelsEntry\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"<\n\x14ListEntitiesResponse\x12$\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x12.feast.core.Entity\"\xee\x01\n\x13ListFeaturesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32&.feast.core.ListFeaturesRequest.Filter\x1a\x9e\x01\n\x06\x46ilter\x12\x42\n\x06labels\x18\x01 \x03(\x0b\x32\x32.feast.core.ListFeaturesRequest.Filter.LabelsEntry\x12\x10\n\x08\x65ntities\x18\x02 \x03(\t\x12\x0f\n\x07project\x18\x03 \x01(\t\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaa\x01\n\x14ListFeaturesResponse\x12@\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32..feast.core.ListFeaturesResponse.FeaturesEntry\x1aJ\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.feast.core.FeatureSpecV2:\x02\x38\x01J\x04\x08\x01\x10\x02\"a\n\x11ListStoresRequest\x12\x34\n\x06\x66ilter\x18\x01 \x01(\x0b\x32$.feast.core.ListStoresRequest.Filter\x1a\x16\n\x06\x46ilter\x12\x0c\n\x04name\x18\x01 \x01(\t\"6\n\x12ListStoresResponse\x12 \n\x05store\x18\x01 \x03(\x0b\x32\x11.feast.core.Store\"M\n\x12\x41pplyEntityRequest\x12&\n\x04spec\x18\x01 \x01(\x0b\x32\x18.feast.core.EntitySpecV2\x12\x0f\n\x07project\x18\x02 \x01(\t\"9\n\x13\x41pplyEntityResponse\x12\"\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x12.feast.core.Entity\"\x1c\n\x1aGetFeastCoreVersionRequest\".\n\x1bGetFeastCoreVersionResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"6\n\x12UpdateStoreRequest\x12 \n\x05store\x18\x01 \x01(\x0b\x32\x11.feast.core.Store\"\x95\x01\n\x13UpdateStoreResponse\x12 \n\x05store\x18\x01 \x01(\x0b\x32\x11.feast.core.Store\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32&.feast.core.UpdateStoreResponse.Status\"$\n\x06Status\x12\r\n\tNO_CHANGE\x10\x00\x12\x0b\n\x07UPDATED\x10\x01\"$\n\x14\x43reateProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x17\n\x15\x43reateProjectResponse\"%\n\x15\x41rchiveProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x18\n\x16\x41rchiveProjectResponse\"\x15\n\x13ListProjectsRequest\"(\n\x14ListProjectsResponse\x12\x10\n\x08projects\x18\x01 \x03(\t\" \n\x1eUpdateFeatureSetStatusResponse\"]\n\x18\x41pplyFeatureTableRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x30\n\ntable_spec\x18\x02 \x01(\x0b\x32\x1c.feast.core.FeatureTableSpec\"D\n\x19\x41pplyFeatureTableResponse\x12\'\n\x05table\x18\x01 \x01(\x0b\x32\x18.feast.core.FeatureTable\"7\n\x16GetFeatureTableRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"B\n\x17GetFeatureTableResponse\x12\'\n\x05table\x18\x01 \x01(\x0b\x32\x18.feast.core.FeatureTable\"\xeb\x01\n\x18ListFeatureTablesRequest\x12;\n\x06\x66ilter\x18\x01 \x01(\x0b\x32+.feast.core.ListFeatureTablesRequest.Filter\x1a\x91\x01\n\x06\x46ilter\x12\x0f\n\x07project\x18\x01 \x01(\t\x12G\n\x06labels\x18\x03 \x03(\x0b\x32\x37.feast.core.ListFeatureTablesRequest.Filter.LabelsEntry\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"E\n\x19ListFeatureTablesResponse\x12(\n\x06tables\x18\x01 \x03(\x0b\x32\x18.feast.core.FeatureTable\":\n\x19\x44\x65leteFeatureTableRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1c\n\x1a\x44\x65leteFeatureTableResponse2\xd9\t\n\x0b\x43oreService\x12\x66\n\x13GetFeastCoreVersion\x12&.feast.core.GetFeastCoreVersionRequest\x1a\'.feast.core.GetFeastCoreVersionResponse\x12H\n\tGetEntity\x12\x1c.feast.core.GetEntityRequest\x1a\x1d.feast.core.GetEntityResponse\x12Q\n\x0cListFeatures\x12\x1f.feast.core.ListFeaturesRequest\x1a .feast.core.ListFeaturesResponse\x12K\n\nListStores\x12\x1d.feast.core.ListStoresRequest\x1a\x1e.feast.core.ListStoresResponse\x12N\n\x0b\x41pplyEntity\x12\x1e.feast.core.ApplyEntityRequest\x1a\x1f.feast.core.ApplyEntityResponse\x12Q\n\x0cListEntities\x12\x1f.feast.core.ListEntitiesRequest\x1a .feast.core.ListEntitiesResponse\x12N\n\x0bUpdateStore\x12\x1e.feast.core.UpdateStoreRequest\x1a\x1f.feast.core.UpdateStoreResponse\x12T\n\rCreateProject\x12 .feast.core.CreateProjectRequest\x1a!.feast.core.CreateProjectResponse\x12W\n\x0e\x41rchiveProject\x12!.feast.core.ArchiveProjectRequest\x1a\".feast.core.ArchiveProjectResponse\x12Q\n\x0cListProjects\x12\x1f.feast.core.ListProjectsRequest\x1a .feast.core.ListProjectsResponse\x12`\n\x11\x41pplyFeatureTable\x12$.feast.core.ApplyFeatureTableRequest\x1a%.feast.core.ApplyFeatureTableResponse\x12`\n\x11ListFeatureTables\x12$.feast.core.ListFeatureTablesRequest\x1a%.feast.core.ListFeatureTablesResponse\x12Z\n\x0fGetFeatureTable\x12\".feast.core.GetFeatureTableRequest\x1a#.feast.core.GetFeatureTableResponse\x12\x63\n\x12\x44\x65leteFeatureTable\x12%.feast.core.DeleteFeatureTableRequest\x1a&.feast.core.DeleteFeatureTableResponseBY\n\x10\x66\x65\x61st.proto.coreB\x10\x43oreServiceProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/coreb\x06proto3'
+  serialized_pb=b'\n\x1c\x66\x65\x61st/core/CoreService.proto\x12\nfeast.core\x1a\x1fgoogle/protobuf/timestamp.proto\x1a-tensorflow_metadata/proto/v0/statistics.proto\x1a\x17\x66\x65\x61st/core/Entity.proto\x1a\x18\x66\x65\x61st/core/Feature.proto\x1a\x1d\x66\x65\x61st/core/FeatureTable.proto\x1a\x16\x66\x65\x61st/core/Store.proto\x1a\x1c\x66\x65\x61st/core/OnlineStore.proto\"1\n\x10GetEntityRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07project\x18\x02 \x01(\t\"7\n\x11GetEntityResponse\x12\"\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x12.feast.core.Entity\"\xdc\x01\n\x13ListEntitiesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32&.feast.core.ListEntitiesRequest.Filter\x1a\x8c\x01\n\x06\x46ilter\x12\x0f\n\x07project\x18\x03 \x01(\t\x12\x42\n\x06labels\x18\x04 \x03(\x0b\x32\x32.feast.core.ListEntitiesRequest.Filter.LabelsEntry\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"<\n\x14ListEntitiesResponse\x12$\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x12.feast.core.Entity\"\xee\x01\n\x13ListFeaturesRequest\x12\x36\n\x06\x66ilter\x18\x01 \x01(\x0b\x32&.feast.core.ListFeaturesRequest.Filter\x1a\x9e\x01\n\x06\x46ilter\x12\x42\n\x06labels\x18\x01 \x03(\x0b\x32\x32.feast.core.ListFeaturesRequest.Filter.LabelsEntry\x12\x10\n\x08\x65ntities\x18\x02 \x03(\t\x12\x0f\n\x07project\x18\x03 \x01(\t\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xaa\x01\n\x14ListFeaturesResponse\x12@\n\x08\x66\x65\x61tures\x18\x02 \x03(\x0b\x32..feast.core.ListFeaturesResponse.FeaturesEntry\x1aJ\n\rFeaturesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.feast.core.FeatureSpecV2:\x02\x38\x01J\x04\x08\x01\x10\x02\"a\n\x11ListStoresRequest\x12\x34\n\x06\x66ilter\x18\x01 \x01(\x0b\x32$.feast.core.ListStoresRequest.Filter\x1a\x16\n\x06\x46ilter\x12\x0c\n\x04name\x18\x01 \x01(\t\"6\n\x12ListStoresResponse\x12 \n\x05store\x18\x01 \x03(\x0b\x32\x11.feast.core.Store\"M\n\x12\x41pplyEntityRequest\x12&\n\x04spec\x18\x01 \x01(\x0b\x32\x18.feast.core.EntitySpecV2\x12\x0f\n\x07project\x18\x02 \x01(\t\"9\n\x13\x41pplyEntityResponse\x12\"\n\x06\x65ntity\x18\x01 \x01(\x0b\x32\x12.feast.core.Entity\"\x1c\n\x1aGetFeastCoreVersionRequest\".\n\x1bGetFeastCoreVersionResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"6\n\x12UpdateStoreRequest\x12 \n\x05store\x18\x01 \x01(\x0b\x32\x11.feast.core.Store\"\x95\x01\n\x13UpdateStoreResponse\x12 \n\x05store\x18\x01 \x01(\x0b\x32\x11.feast.core.Store\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32&.feast.core.UpdateStoreResponse.Status\"$\n\x06Status\x12\r\n\tNO_CHANGE\x10\x00\x12\x0b\n\x07UPDATED\x10\x01\"$\n\x14\x43reateProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x17\n\x15\x43reateProjectResponse\"%\n\x15\x41rchiveProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x18\n\x16\x41rchiveProjectResponse\"\x15\n\x13ListProjectsRequest\"(\n\x14ListProjectsResponse\x12\x10\n\x08projects\x18\x01 \x03(\t\" \n\x1eUpdateFeatureSetStatusResponse\"]\n\x18\x41pplyFeatureTableRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x30\n\ntable_spec\x18\x02 \x01(\x0b\x32\x1c.feast.core.FeatureTableSpec\"D\n\x19\x41pplyFeatureTableResponse\x12\'\n\x05table\x18\x01 \x01(\x0b\x32\x18.feast.core.FeatureTable\"7\n\x16GetFeatureTableRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"B\n\x17GetFeatureTableResponse\x12\'\n\x05table\x18\x01 \x01(\x0b\x32\x18.feast.core.FeatureTable\"\xeb\x01\n\x18ListFeatureTablesRequest\x12;\n\x06\x66ilter\x18\x01 \x01(\x0b\x32+.feast.core.ListFeatureTablesRequest.Filter\x1a\x91\x01\n\x06\x46ilter\x12\x0f\n\x07project\x18\x01 \x01(\t\x12G\n\x06labels\x18\x03 \x03(\x0b\x32\x37.feast.core.ListFeatureTablesRequest.Filter.LabelsEntry\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"E\n\x19ListFeatureTablesResponse\x12(\n\x06tables\x18\x01 \x03(\x0b\x32\x18.feast.core.FeatureTable\":\n\x19\x44\x65leteFeatureTableRequest\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x1c\n\x1a\x44\x65leteFeatureTableResponse\"\x19\n\x17ListOnlineStoresRequest\"I\n\x18ListOnlineStoresResponse\x12-\n\x0conline_store\x18\x01 \x03(\x0b\x32\x17.feast.core.OnlineStore\"%\n\x15GetOnlineStoreRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xa6\x01\n\x16GetOnlineStoreResponse\x12-\n\x0conline_store\x18\x01 \x01(\x0b\x32\x17.feast.core.OnlineStore\x12\x39\n\x06status\x18\x02 \x01(\x0e\x32).feast.core.GetOnlineStoreResponse.Status\"\"\n\x06Status\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08\x41RCHIVED\x10\x01\"K\n\x1aRegisterOnlineStoreRequest\x12-\n\x0conline_store\x18\x01 \x01(\x0b\x32\x17.feast.core.OnlineStore\"\xc2\x01\n\x1bRegisterOnlineStoreResponse\x12-\n\x0conline_store\x18\x01 \x01(\x0b\x32\x17.feast.core.OnlineStore\x12>\n\x06status\x18\x02 \x01(\x0e\x32..feast.core.RegisterOnlineStoreResponse.Status\"4\n\x06Status\x12\r\n\tNO_CHANGE\x10\x00\x12\x0e\n\nREGISTERED\x10\x01\x12\x0b\n\x07UPDATED\x10\x02\")\n\x19\x41rchiveOnlineStoreRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x1c\n\x1a\x41rchiveOnlineStoreResponse2\xde\x0c\n\x0b\x43oreService\x12\x66\n\x13GetFeastCoreVersion\x12&.feast.core.GetFeastCoreVersionRequest\x1a\'.feast.core.GetFeastCoreVersionResponse\x12H\n\tGetEntity\x12\x1c.feast.core.GetEntityRequest\x1a\x1d.feast.core.GetEntityResponse\x12Q\n\x0cListFeatures\x12\x1f.feast.core.ListFeaturesRequest\x1a .feast.core.ListFeaturesResponse\x12K\n\nListStores\x12\x1d.feast.core.ListStoresRequest\x1a\x1e.feast.core.ListStoresResponse\x12N\n\x0b\x41pplyEntity\x12\x1e.feast.core.ApplyEntityRequest\x1a\x1f.feast.core.ApplyEntityResponse\x12Q\n\x0cListEntities\x12\x1f.feast.core.ListEntitiesRequest\x1a .feast.core.ListEntitiesResponse\x12N\n\x0bUpdateStore\x12\x1e.feast.core.UpdateStoreRequest\x1a\x1f.feast.core.UpdateStoreResponse\x12T\n\rCreateProject\x12 .feast.core.CreateProjectRequest\x1a!.feast.core.CreateProjectResponse\x12W\n\x0e\x41rchiveProject\x12!.feast.core.ArchiveProjectRequest\x1a\".feast.core.ArchiveProjectResponse\x12Q\n\x0cListProjects\x12\x1f.feast.core.ListProjectsRequest\x1a .feast.core.ListProjectsResponse\x12`\n\x11\x41pplyFeatureTable\x12$.feast.core.ApplyFeatureTableRequest\x1a%.feast.core.ApplyFeatureTableResponse\x12`\n\x11ListFeatureTables\x12$.feast.core.ListFeatureTablesRequest\x1a%.feast.core.ListFeatureTablesResponse\x12Z\n\x0fGetFeatureTable\x12\".feast.core.GetFeatureTableRequest\x1a#.feast.core.GetFeatureTableResponse\x12\x63\n\x12\x44\x65leteFeatureTable\x12%.feast.core.DeleteFeatureTableRequest\x1a&.feast.core.DeleteFeatureTableResponse\x12]\n\x10ListOnlineStores\x12#.feast.core.ListOnlineStoresRequest\x1a$.feast.core.ListOnlineStoresResponse\x12W\n\x0eGetOnlineStore\x12!.feast.core.GetOnlineStoreRequest\x1a\".feast.core.GetOnlineStoreResponse\x12\x66\n\x13RegisterOnlineStore\x12&.feast.core.RegisterOnlineStoreRequest\x1a\'.feast.core.RegisterOnlineStoreResponse\x12\x63\n\x12\x41rchiveOnlineStore\x12%.feast.core.ArchiveOnlineStoreRequest\x1a&.feast.core.ArchiveOnlineStoreResponseBY\n\x10\x66\x65\x61st.proto.coreB\x10\x43oreServiceProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/coreb\x06proto3'
   ,
-  dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,tensorflow__metadata_dot_proto_dot_v0_dot_statistics__pb2.DESCRIPTOR,feast_dot_core_dot_Entity__pb2.DESCRIPTOR,feast_dot_core_dot_Feature__pb2.DESCRIPTOR,feast_dot_core_dot_FeatureTable__pb2.DESCRIPTOR,feast_dot_core_dot_Store__pb2.DESCRIPTOR,])
+  dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,tensorflow__metadata_dot_proto_dot_v0_dot_statistics__pb2.DESCRIPTOR,feast_dot_core_dot_Entity__pb2.DESCRIPTOR,feast_dot_core_dot_Feature__pb2.DESCRIPTOR,feast_dot_core_dot_FeatureTable__pb2.DESCRIPTOR,feast_dot_core_dot_Store__pb2.DESCRIPTOR,feast_dot_core_dot_OnlineStore__pb2.DESCRIPTOR,])
 
 
 
 _UPDATESTORERESPONSE_STATUS = _descriptor.EnumDescriptor(
   name='Status',
   full_name='feast.core.UpdateStoreResponse.Status',
   filename=None,
@@ -52,19 +48,74 @@
       name='UPDATED', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1578,
-  serialized_end=1614,
+  serialized_start=1608,
+  serialized_end=1644,
 )
 _sym_db.RegisterEnumDescriptor(_UPDATESTORERESPONSE_STATUS)
 
+_GETONLINESTORERESPONSE_STATUS = _descriptor.EnumDescriptor(
+  name='Status',
+  full_name='feast.core.GetOnlineStoreResponse.Status',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='ACTIVE', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='ARCHIVED', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=2836,
+  serialized_end=2870,
+)
+_sym_db.RegisterEnumDescriptor(_GETONLINESTORERESPONSE_STATUS)
+
+_REGISTERONLINESTORERESPONSE_STATUS = _descriptor.EnumDescriptor(
+  name='Status',
+  full_name='feast.core.RegisterOnlineStoreResponse.Status',
+  filename=None,
+  file=DESCRIPTOR,
+  create_key=_descriptor._internal_create_key,
+  values=[
+    _descriptor.EnumValueDescriptor(
+      name='NO_CHANGE', index=0, number=0,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='REGISTERED', index=1, number=1,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='UPDATED', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+  ],
+  containing_type=None,
+  serialized_options=None,
+  serialized_start=3092,
+  serialized_end=3144,
+)
+_sym_db.RegisterEnumDescriptor(_REGISTERONLINESTORERESPONSE_STATUS)
+
 
 _GETENTITYREQUEST = _descriptor.Descriptor(
   name='GetEntityRequest',
   full_name='feast.core.GetEntityRequest',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
@@ -92,16 +143,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=230,
-  serialized_end=279,
+  serialized_start=260,
+  serialized_end=309,
 )
 
 
 _GETENTITYRESPONSE = _descriptor.Descriptor(
   name='GetEntityResponse',
   full_name='feast.core.GetEntityResponse',
   filename=None,
@@ -124,16 +175,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=281,
-  serialized_end=336,
+  serialized_start=311,
+  serialized_end=366,
 )
 
 
 _LISTENTITIESREQUEST_FILTER_LABELSENTRY = _descriptor.Descriptor(
   name='LabelsEntry',
   full_name='feast.core.ListEntitiesRequest.Filter.LabelsEntry',
   filename=None,
@@ -163,16 +214,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=514,
-  serialized_end=559,
+  serialized_start=544,
+  serialized_end=589,
 )
 
 _LISTENTITIESREQUEST_FILTER = _descriptor.Descriptor(
   name='Filter',
   full_name='feast.core.ListEntitiesRequest.Filter',
   filename=None,
   file=DESCRIPTOR,
@@ -201,16 +252,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=419,
-  serialized_end=559,
+  serialized_start=449,
+  serialized_end=589,
 )
 
 _LISTENTITIESREQUEST = _descriptor.Descriptor(
   name='ListEntitiesRequest',
   full_name='feast.core.ListEntitiesRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -232,16 +283,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=339,
-  serialized_end=559,
+  serialized_start=369,
+  serialized_end=589,
 )
 
 
 _LISTENTITIESRESPONSE = _descriptor.Descriptor(
   name='ListEntitiesResponse',
   full_name='feast.core.ListEntitiesResponse',
   filename=None,
@@ -264,16 +315,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=561,
-  serialized_end=621,
+  serialized_start=591,
+  serialized_end=651,
 )
 
 
 _LISTFEATURESREQUEST_FILTER_LABELSENTRY = _descriptor.Descriptor(
   name='LabelsEntry',
   full_name='feast.core.ListFeaturesRequest.Filter.LabelsEntry',
   filename=None,
@@ -303,16 +354,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=514,
-  serialized_end=559,
+  serialized_start=544,
+  serialized_end=589,
 )
 
 _LISTFEATURESREQUEST_FILTER = _descriptor.Descriptor(
   name='Filter',
   full_name='feast.core.ListFeaturesRequest.Filter',
   filename=None,
   file=DESCRIPTOR,
@@ -348,16 +399,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=704,
-  serialized_end=862,
+  serialized_start=734,
+  serialized_end=892,
 )
 
 _LISTFEATURESREQUEST = _descriptor.Descriptor(
   name='ListFeaturesRequest',
   full_name='feast.core.ListFeaturesRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -379,16 +430,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=624,
-  serialized_end=862,
+  serialized_start=654,
+  serialized_end=892,
 )
 
 
 _LISTFEATURESRESPONSE_FEATURESENTRY = _descriptor.Descriptor(
   name='FeaturesEntry',
   full_name='feast.core.ListFeaturesResponse.FeaturesEntry',
   filename=None,
@@ -418,16 +469,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=955,
-  serialized_end=1029,
+  serialized_start=985,
+  serialized_end=1059,
 )
 
 _LISTFEATURESRESPONSE = _descriptor.Descriptor(
   name='ListFeaturesResponse',
   full_name='feast.core.ListFeaturesResponse',
   filename=None,
   file=DESCRIPTOR,
@@ -449,16 +500,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=865,
-  serialized_end=1035,
+  serialized_start=895,
+  serialized_end=1065,
 )
 
 
 _LISTSTORESREQUEST_FILTER = _descriptor.Descriptor(
   name='Filter',
   full_name='feast.core.ListStoresRequest.Filter',
   filename=None,
@@ -481,16 +532,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1112,
-  serialized_end=1134,
+  serialized_start=1142,
+  serialized_end=1164,
 )
 
 _LISTSTORESREQUEST = _descriptor.Descriptor(
   name='ListStoresRequest',
   full_name='feast.core.ListStoresRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -512,16 +563,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1037,
-  serialized_end=1134,
+  serialized_start=1067,
+  serialized_end=1164,
 )
 
 
 _LISTSTORESRESPONSE = _descriptor.Descriptor(
   name='ListStoresResponse',
   full_name='feast.core.ListStoresResponse',
   filename=None,
@@ -544,16 +595,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1136,
-  serialized_end=1190,
+  serialized_start=1166,
+  serialized_end=1220,
 )
 
 
 _APPLYENTITYREQUEST = _descriptor.Descriptor(
   name='ApplyEntityRequest',
   full_name='feast.core.ApplyEntityRequest',
   filename=None,
@@ -583,16 +634,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1192,
-  serialized_end=1269,
+  serialized_start=1222,
+  serialized_end=1299,
 )
 
 
 _APPLYENTITYRESPONSE = _descriptor.Descriptor(
   name='ApplyEntityResponse',
   full_name='feast.core.ApplyEntityResponse',
   filename=None,
@@ -615,16 +666,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1271,
-  serialized_end=1328,
+  serialized_start=1301,
+  serialized_end=1358,
 )
 
 
 _GETFEASTCOREVERSIONREQUEST = _descriptor.Descriptor(
   name='GetFeastCoreVersionRequest',
   full_name='feast.core.GetFeastCoreVersionRequest',
   filename=None,
@@ -640,16 +691,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1330,
-  serialized_end=1358,
+  serialized_start=1360,
+  serialized_end=1388,
 )
 
 
 _GETFEASTCOREVERSIONRESPONSE = _descriptor.Descriptor(
   name='GetFeastCoreVersionResponse',
   full_name='feast.core.GetFeastCoreVersionResponse',
   filename=None,
@@ -672,16 +723,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1360,
-  serialized_end=1406,
+  serialized_start=1390,
+  serialized_end=1436,
 )
 
 
 _UPDATESTOREREQUEST = _descriptor.Descriptor(
   name='UpdateStoreRequest',
   full_name='feast.core.UpdateStoreRequest',
   filename=None,
@@ -704,16 +755,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1408,
-  serialized_end=1462,
+  serialized_start=1438,
+  serialized_end=1492,
 )
 
 
 _UPDATESTORERESPONSE = _descriptor.Descriptor(
   name='UpdateStoreResponse',
   full_name='feast.core.UpdateStoreResponse',
   filename=None,
@@ -744,16 +795,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1465,
-  serialized_end=1614,
+  serialized_start=1495,
+  serialized_end=1644,
 )
 
 
 _CREATEPROJECTREQUEST = _descriptor.Descriptor(
   name='CreateProjectRequest',
   full_name='feast.core.CreateProjectRequest',
   filename=None,
@@ -776,16 +827,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1616,
-  serialized_end=1652,
+  serialized_start=1646,
+  serialized_end=1682,
 )
 
 
 _CREATEPROJECTRESPONSE = _descriptor.Descriptor(
   name='CreateProjectResponse',
   full_name='feast.core.CreateProjectResponse',
   filename=None,
@@ -801,16 +852,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1654,
-  serialized_end=1677,
+  serialized_start=1684,
+  serialized_end=1707,
 )
 
 
 _ARCHIVEPROJECTREQUEST = _descriptor.Descriptor(
   name='ArchiveProjectRequest',
   full_name='feast.core.ArchiveProjectRequest',
   filename=None,
@@ -833,16 +884,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1679,
-  serialized_end=1716,
+  serialized_start=1709,
+  serialized_end=1746,
 )
 
 
 _ARCHIVEPROJECTRESPONSE = _descriptor.Descriptor(
   name='ArchiveProjectResponse',
   full_name='feast.core.ArchiveProjectResponse',
   filename=None,
@@ -858,16 +909,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1718,
-  serialized_end=1742,
+  serialized_start=1748,
+  serialized_end=1772,
 )
 
 
 _LISTPROJECTSREQUEST = _descriptor.Descriptor(
   name='ListProjectsRequest',
   full_name='feast.core.ListProjectsRequest',
   filename=None,
@@ -883,16 +934,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1744,
-  serialized_end=1765,
+  serialized_start=1774,
+  serialized_end=1795,
 )
 
 
 _LISTPROJECTSRESPONSE = _descriptor.Descriptor(
   name='ListProjectsResponse',
   full_name='feast.core.ListProjectsResponse',
   filename=None,
@@ -915,16 +966,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1767,
-  serialized_end=1807,
+  serialized_start=1797,
+  serialized_end=1837,
 )
 
 
 _UPDATEFEATURESETSTATUSRESPONSE = _descriptor.Descriptor(
   name='UpdateFeatureSetStatusResponse',
   full_name='feast.core.UpdateFeatureSetStatusResponse',
   filename=None,
@@ -940,16 +991,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1809,
-  serialized_end=1841,
+  serialized_start=1839,
+  serialized_end=1871,
 )
 
 
 _APPLYFEATURETABLEREQUEST = _descriptor.Descriptor(
   name='ApplyFeatureTableRequest',
   full_name='feast.core.ApplyFeatureTableRequest',
   filename=None,
@@ -979,16 +1030,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1843,
-  serialized_end=1936,
+  serialized_start=1873,
+  serialized_end=1966,
 )
 
 
 _APPLYFEATURETABLERESPONSE = _descriptor.Descriptor(
   name='ApplyFeatureTableResponse',
   full_name='feast.core.ApplyFeatureTableResponse',
   filename=None,
@@ -1011,16 +1062,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1938,
-  serialized_end=2006,
+  serialized_start=1968,
+  serialized_end=2036,
 )
 
 
 _GETFEATURETABLEREQUEST = _descriptor.Descriptor(
   name='GetFeatureTableRequest',
   full_name='feast.core.GetFeatureTableRequest',
   filename=None,
@@ -1050,16 +1101,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2008,
-  serialized_end=2063,
+  serialized_start=2038,
+  serialized_end=2093,
 )
 
 
 _GETFEATURETABLERESPONSE = _descriptor.Descriptor(
   name='GetFeatureTableResponse',
   full_name='feast.core.GetFeatureTableResponse',
   filename=None,
@@ -1082,16 +1133,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2065,
-  serialized_end=2131,
+  serialized_start=2095,
+  serialized_end=2161,
 )
 
 
 _LISTFEATURETABLESREQUEST_FILTER_LABELSENTRY = _descriptor.Descriptor(
   name='LabelsEntry',
   full_name='feast.core.ListFeatureTablesRequest.Filter.LabelsEntry',
   filename=None,
@@ -1121,16 +1172,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=514,
-  serialized_end=559,
+  serialized_start=544,
+  serialized_end=589,
 )
 
 _LISTFEATURETABLESREQUEST_FILTER = _descriptor.Descriptor(
   name='Filter',
   full_name='feast.core.ListFeatureTablesRequest.Filter',
   filename=None,
   file=DESCRIPTOR,
@@ -1159,16 +1210,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2224,
-  serialized_end=2369,
+  serialized_start=2254,
+  serialized_end=2399,
 )
 
 _LISTFEATURETABLESREQUEST = _descriptor.Descriptor(
   name='ListFeatureTablesRequest',
   full_name='feast.core.ListFeatureTablesRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -1190,16 +1241,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2134,
-  serialized_end=2369,
+  serialized_start=2164,
+  serialized_end=2399,
 )
 
 
 _LISTFEATURETABLESRESPONSE = _descriptor.Descriptor(
   name='ListFeatureTablesResponse',
   full_name='feast.core.ListFeatureTablesResponse',
   filename=None,
@@ -1222,16 +1273,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2371,
-  serialized_end=2440,
+  serialized_start=2401,
+  serialized_end=2470,
 )
 
 
 _DELETEFEATURETABLEREQUEST = _descriptor.Descriptor(
   name='DeleteFeatureTableRequest',
   full_name='feast.core.DeleteFeatureTableRequest',
   filename=None,
@@ -1261,16 +1312,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2442,
-  serialized_end=2500,
+  serialized_start=2472,
+  serialized_end=2530,
 )
 
 
 _DELETEFEATURETABLERESPONSE = _descriptor.Descriptor(
   name='DeleteFeatureTableResponse',
   full_name='feast.core.DeleteFeatureTableResponse',
   filename=None,
@@ -1286,16 +1337,274 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2502,
-  serialized_end=2530,
+  serialized_start=2532,
+  serialized_end=2560,
+)
+
+
+_LISTONLINESTORESREQUEST = _descriptor.Descriptor(
+  name='ListOnlineStoresRequest',
+  full_name='feast.core.ListOnlineStoresRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2562,
+  serialized_end=2587,
+)
+
+
+_LISTONLINESTORESRESPONSE = _descriptor.Descriptor(
+  name='ListOnlineStoresResponse',
+  full_name='feast.core.ListOnlineStoresResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='online_store', full_name='feast.core.ListOnlineStoresResponse.online_store', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2589,
+  serialized_end=2662,
+)
+
+
+_GETONLINESTOREREQUEST = _descriptor.Descriptor(
+  name='GetOnlineStoreRequest',
+  full_name='feast.core.GetOnlineStoreRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='feast.core.GetOnlineStoreRequest.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2664,
+  serialized_end=2701,
+)
+
+
+_GETONLINESTORERESPONSE = _descriptor.Descriptor(
+  name='GetOnlineStoreResponse',
+  full_name='feast.core.GetOnlineStoreResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='online_store', full_name='feast.core.GetOnlineStoreResponse.online_store', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='status', full_name='feast.core.GetOnlineStoreResponse.status', index=1,
+      number=2, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+    _GETONLINESTORERESPONSE_STATUS,
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2704,
+  serialized_end=2870,
+)
+
+
+_REGISTERONLINESTOREREQUEST = _descriptor.Descriptor(
+  name='RegisterOnlineStoreRequest',
+  full_name='feast.core.RegisterOnlineStoreRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='online_store', full_name='feast.core.RegisterOnlineStoreRequest.online_store', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2872,
+  serialized_end=2947,
+)
+
+
+_REGISTERONLINESTORERESPONSE = _descriptor.Descriptor(
+  name='RegisterOnlineStoreResponse',
+  full_name='feast.core.RegisterOnlineStoreResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='online_store', full_name='feast.core.RegisterOnlineStoreResponse.online_store', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='status', full_name='feast.core.RegisterOnlineStoreResponse.status', index=1,
+      number=2, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+    _REGISTERONLINESTORERESPONSE_STATUS,
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2950,
+  serialized_end=3144,
+)
+
+
+_ARCHIVEONLINESTOREREQUEST = _descriptor.Descriptor(
+  name='ArchiveOnlineStoreRequest',
+  full_name='feast.core.ArchiveOnlineStoreRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='name', full_name='feast.core.ArchiveOnlineStoreRequest.name', index=0,
+      number=1, type=9, cpp_type=9, label=1,
+      has_default_value=False, default_value=b"".decode('utf-8'),
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3146,
+  serialized_end=3187,
+)
+
+
+_ARCHIVEONLINESTORERESPONSE = _descriptor.Descriptor(
+  name='ArchiveOnlineStoreResponse',
+  full_name='feast.core.ArchiveOnlineStoreResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=3189,
+  serialized_end=3217,
 )
 
 _GETENTITYRESPONSE.fields_by_name['entity'].message_type = feast_dot_core_dot_Entity__pb2._ENTITY
 _LISTENTITIESREQUEST_FILTER_LABELSENTRY.containing_type = _LISTENTITIESREQUEST_FILTER
 _LISTENTITIESREQUEST_FILTER.fields_by_name['labels'].message_type = _LISTENTITIESREQUEST_FILTER_LABELSENTRY
 _LISTENTITIESREQUEST_FILTER.containing_type = _LISTENTITIESREQUEST
 _LISTENTITIESREQUEST.fields_by_name['filter'].message_type = _LISTENTITIESREQUEST_FILTER
@@ -1320,14 +1629,22 @@
 _APPLYFEATURETABLERESPONSE.fields_by_name['table'].message_type = feast_dot_core_dot_FeatureTable__pb2._FEATURETABLE
 _GETFEATURETABLERESPONSE.fields_by_name['table'].message_type = feast_dot_core_dot_FeatureTable__pb2._FEATURETABLE
 _LISTFEATURETABLESREQUEST_FILTER_LABELSENTRY.containing_type = _LISTFEATURETABLESREQUEST_FILTER
 _LISTFEATURETABLESREQUEST_FILTER.fields_by_name['labels'].message_type = _LISTFEATURETABLESREQUEST_FILTER_LABELSENTRY
 _LISTFEATURETABLESREQUEST_FILTER.containing_type = _LISTFEATURETABLESREQUEST
 _LISTFEATURETABLESREQUEST.fields_by_name['filter'].message_type = _LISTFEATURETABLESREQUEST_FILTER
 _LISTFEATURETABLESRESPONSE.fields_by_name['tables'].message_type = feast_dot_core_dot_FeatureTable__pb2._FEATURETABLE
+_LISTONLINESTORESRESPONSE.fields_by_name['online_store'].message_type = feast_dot_core_dot_OnlineStore__pb2._ONLINESTORE
+_GETONLINESTORERESPONSE.fields_by_name['online_store'].message_type = feast_dot_core_dot_OnlineStore__pb2._ONLINESTORE
+_GETONLINESTORERESPONSE.fields_by_name['status'].enum_type = _GETONLINESTORERESPONSE_STATUS
+_GETONLINESTORERESPONSE_STATUS.containing_type = _GETONLINESTORERESPONSE
+_REGISTERONLINESTOREREQUEST.fields_by_name['online_store'].message_type = feast_dot_core_dot_OnlineStore__pb2._ONLINESTORE
+_REGISTERONLINESTORERESPONSE.fields_by_name['online_store'].message_type = feast_dot_core_dot_OnlineStore__pb2._ONLINESTORE
+_REGISTERONLINESTORERESPONSE.fields_by_name['status'].enum_type = _REGISTERONLINESTORERESPONSE_STATUS
+_REGISTERONLINESTORERESPONSE_STATUS.containing_type = _REGISTERONLINESTORERESPONSE
 DESCRIPTOR.message_types_by_name['GetEntityRequest'] = _GETENTITYREQUEST
 DESCRIPTOR.message_types_by_name['GetEntityResponse'] = _GETENTITYRESPONSE
 DESCRIPTOR.message_types_by_name['ListEntitiesRequest'] = _LISTENTITIESREQUEST
 DESCRIPTOR.message_types_by_name['ListEntitiesResponse'] = _LISTENTITIESRESPONSE
 DESCRIPTOR.message_types_by_name['ListFeaturesRequest'] = _LISTFEATURESREQUEST
 DESCRIPTOR.message_types_by_name['ListFeaturesResponse'] = _LISTFEATURESRESPONSE
 DESCRIPTOR.message_types_by_name['ListStoresRequest'] = _LISTSTORESREQUEST
@@ -1349,14 +1666,22 @@
 DESCRIPTOR.message_types_by_name['ApplyFeatureTableResponse'] = _APPLYFEATURETABLERESPONSE
 DESCRIPTOR.message_types_by_name['GetFeatureTableRequest'] = _GETFEATURETABLEREQUEST
 DESCRIPTOR.message_types_by_name['GetFeatureTableResponse'] = _GETFEATURETABLERESPONSE
 DESCRIPTOR.message_types_by_name['ListFeatureTablesRequest'] = _LISTFEATURETABLESREQUEST
 DESCRIPTOR.message_types_by_name['ListFeatureTablesResponse'] = _LISTFEATURETABLESRESPONSE
 DESCRIPTOR.message_types_by_name['DeleteFeatureTableRequest'] = _DELETEFEATURETABLEREQUEST
 DESCRIPTOR.message_types_by_name['DeleteFeatureTableResponse'] = _DELETEFEATURETABLERESPONSE
+DESCRIPTOR.message_types_by_name['ListOnlineStoresRequest'] = _LISTONLINESTORESREQUEST
+DESCRIPTOR.message_types_by_name['ListOnlineStoresResponse'] = _LISTONLINESTORESRESPONSE
+DESCRIPTOR.message_types_by_name['GetOnlineStoreRequest'] = _GETONLINESTOREREQUEST
+DESCRIPTOR.message_types_by_name['GetOnlineStoreResponse'] = _GETONLINESTORERESPONSE
+DESCRIPTOR.message_types_by_name['RegisterOnlineStoreRequest'] = _REGISTERONLINESTOREREQUEST
+DESCRIPTOR.message_types_by_name['RegisterOnlineStoreResponse'] = _REGISTERONLINESTORERESPONSE
+DESCRIPTOR.message_types_by_name['ArchiveOnlineStoreRequest'] = _ARCHIVEONLINESTOREREQUEST
+DESCRIPTOR.message_types_by_name['ArchiveOnlineStoreResponse'] = _ARCHIVEONLINESTORERESPONSE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 GetEntityRequest = _reflection.GeneratedProtocolMessageType('GetEntityRequest', (_message.Message,), {
   'DESCRIPTOR' : _GETENTITYREQUEST,
   '__module__' : 'feast.core.CoreService_pb2'
   # @@protoc_insertion_point(class_scope:feast.core.GetEntityRequest)
   })
@@ -1618,30 +1943,86 @@
 DeleteFeatureTableResponse = _reflection.GeneratedProtocolMessageType('DeleteFeatureTableResponse', (_message.Message,), {
   'DESCRIPTOR' : _DELETEFEATURETABLERESPONSE,
   '__module__' : 'feast.core.CoreService_pb2'
   # @@protoc_insertion_point(class_scope:feast.core.DeleteFeatureTableResponse)
   })
 _sym_db.RegisterMessage(DeleteFeatureTableResponse)
 
+ListOnlineStoresRequest = _reflection.GeneratedProtocolMessageType('ListOnlineStoresRequest', (_message.Message,), {
+  'DESCRIPTOR' : _LISTONLINESTORESREQUEST,
+  '__module__' : 'feast.core.CoreService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.core.ListOnlineStoresRequest)
+  })
+_sym_db.RegisterMessage(ListOnlineStoresRequest)
+
+ListOnlineStoresResponse = _reflection.GeneratedProtocolMessageType('ListOnlineStoresResponse', (_message.Message,), {
+  'DESCRIPTOR' : _LISTONLINESTORESRESPONSE,
+  '__module__' : 'feast.core.CoreService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.core.ListOnlineStoresResponse)
+  })
+_sym_db.RegisterMessage(ListOnlineStoresResponse)
+
+GetOnlineStoreRequest = _reflection.GeneratedProtocolMessageType('GetOnlineStoreRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETONLINESTOREREQUEST,
+  '__module__' : 'feast.core.CoreService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.core.GetOnlineStoreRequest)
+  })
+_sym_db.RegisterMessage(GetOnlineStoreRequest)
+
+GetOnlineStoreResponse = _reflection.GeneratedProtocolMessageType('GetOnlineStoreResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETONLINESTORERESPONSE,
+  '__module__' : 'feast.core.CoreService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.core.GetOnlineStoreResponse)
+  })
+_sym_db.RegisterMessage(GetOnlineStoreResponse)
+
+RegisterOnlineStoreRequest = _reflection.GeneratedProtocolMessageType('RegisterOnlineStoreRequest', (_message.Message,), {
+  'DESCRIPTOR' : _REGISTERONLINESTOREREQUEST,
+  '__module__' : 'feast.core.CoreService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.core.RegisterOnlineStoreRequest)
+  })
+_sym_db.RegisterMessage(RegisterOnlineStoreRequest)
+
+RegisterOnlineStoreResponse = _reflection.GeneratedProtocolMessageType('RegisterOnlineStoreResponse', (_message.Message,), {
+  'DESCRIPTOR' : _REGISTERONLINESTORERESPONSE,
+  '__module__' : 'feast.core.CoreService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.core.RegisterOnlineStoreResponse)
+  })
+_sym_db.RegisterMessage(RegisterOnlineStoreResponse)
+
+ArchiveOnlineStoreRequest = _reflection.GeneratedProtocolMessageType('ArchiveOnlineStoreRequest', (_message.Message,), {
+  'DESCRIPTOR' : _ARCHIVEONLINESTOREREQUEST,
+  '__module__' : 'feast.core.CoreService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.core.ArchiveOnlineStoreRequest)
+  })
+_sym_db.RegisterMessage(ArchiveOnlineStoreRequest)
+
+ArchiveOnlineStoreResponse = _reflection.GeneratedProtocolMessageType('ArchiveOnlineStoreResponse', (_message.Message,), {
+  'DESCRIPTOR' : _ARCHIVEONLINESTORERESPONSE,
+  '__module__' : 'feast.core.CoreService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.core.ArchiveOnlineStoreResponse)
+  })
+_sym_db.RegisterMessage(ArchiveOnlineStoreResponse)
+
 
 DESCRIPTOR._options = None
 _LISTENTITIESREQUEST_FILTER_LABELSENTRY._options = None
 _LISTFEATURESREQUEST_FILTER_LABELSENTRY._options = None
 _LISTFEATURESRESPONSE_FEATURESENTRY._options = None
 _LISTFEATURETABLESREQUEST_FILTER_LABELSENTRY._options = None
 
 _CORESERVICE = _descriptor.ServiceDescriptor(
   name='CoreService',
   full_name='feast.core.CoreService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=2533,
-  serialized_end=3774,
+  serialized_start=3220,
+  serialized_end=4850,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetFeastCoreVersion',
     full_name='feast.core.CoreService.GetFeastCoreVersion',
     index=0,
     containing_service=None,
     input_type=_GETFEASTCOREVERSIONREQUEST,
@@ -1775,13 +2156,53 @@
     index=13,
     containing_service=None,
     input_type=_DELETEFEATURETABLEREQUEST,
     output_type=_DELETEFEATURETABLERESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='ListOnlineStores',
+    full_name='feast.core.CoreService.ListOnlineStores',
+    index=14,
+    containing_service=None,
+    input_type=_LISTONLINESTORESREQUEST,
+    output_type=_LISTONLINESTORESRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetOnlineStore',
+    full_name='feast.core.CoreService.GetOnlineStore',
+    index=15,
+    containing_service=None,
+    input_type=_GETONLINESTOREREQUEST,
+    output_type=_GETONLINESTORERESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='RegisterOnlineStore',
+    full_name='feast.core.CoreService.RegisterOnlineStore',
+    index=16,
+    containing_service=None,
+    input_type=_REGISTERONLINESTOREREQUEST,
+    output_type=_REGISTERONLINESTORERESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
+  _descriptor.MethodDescriptor(
+    name='ArchiveOnlineStore',
+    full_name='feast.core.CoreService.ArchiveOnlineStore',
+    index=17,
+    containing_service=None,
+    input_type=_ARCHIVEONLINESTOREREQUEST,
+    output_type=_ARCHIVEONLINESTORERESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_CORESERVICE)
 
 DESCRIPTOR.services_by_name['CoreService'] = _CORESERVICE
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `feast-0.9.8/feast/protos/feast/core/CoreService_pb2_grpc.py` & `feast-0.9.9/feast/core/CoreService_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from feast.protos.feast.core import (
-    CoreService_pb2 as feast_dot_core_dot_CoreService__pb2,
-)
+from feast.core import CoreService_pb2 as feast_dot_core_dot_CoreService__pb2
 
 
 class CoreServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
@@ -82,14 +80,34 @@
                 response_deserializer=feast_dot_core_dot_CoreService__pb2.GetFeatureTableResponse.FromString,
                 )
         self.DeleteFeatureTable = channel.unary_unary(
                 '/feast.core.CoreService/DeleteFeatureTable',
                 request_serializer=feast_dot_core_dot_CoreService__pb2.DeleteFeatureTableRequest.SerializeToString,
                 response_deserializer=feast_dot_core_dot_CoreService__pb2.DeleteFeatureTableResponse.FromString,
                 )
+        self.ListOnlineStores = channel.unary_unary(
+                '/feast.core.CoreService/ListOnlineStores',
+                request_serializer=feast_dot_core_dot_CoreService__pb2.ListOnlineStoresRequest.SerializeToString,
+                response_deserializer=feast_dot_core_dot_CoreService__pb2.ListOnlineStoresResponse.FromString,
+                )
+        self.GetOnlineStore = channel.unary_unary(
+                '/feast.core.CoreService/GetOnlineStore',
+                request_serializer=feast_dot_core_dot_CoreService__pb2.GetOnlineStoreRequest.SerializeToString,
+                response_deserializer=feast_dot_core_dot_CoreService__pb2.GetOnlineStoreResponse.FromString,
+                )
+        self.RegisterOnlineStore = channel.unary_unary(
+                '/feast.core.CoreService/RegisterOnlineStore',
+                request_serializer=feast_dot_core_dot_CoreService__pb2.RegisterOnlineStoreRequest.SerializeToString,
+                response_deserializer=feast_dot_core_dot_CoreService__pb2.RegisterOnlineStoreResponse.FromString,
+                )
+        self.ArchiveOnlineStore = channel.unary_unary(
+                '/feast.core.CoreService/ArchiveOnlineStore',
+                request_serializer=feast_dot_core_dot_CoreService__pb2.ArchiveOnlineStoreRequest.SerializeToString,
+                response_deserializer=feast_dot_core_dot_CoreService__pb2.ArchiveOnlineStoreResponse.FromString,
+                )
 
 
 class CoreServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetFeastCoreVersion(self, request, context):
         """Retrieve version information about this Feast deployment
@@ -221,14 +239,43 @@
     def DeleteFeatureTable(self, request, context):
         """Delete a specific feature table
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListOnlineStores(self, request, context):
+        """Lists all online stores
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetOnlineStore(self, request, context):
+        """Returns a specific online stores
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def RegisterOnlineStore(self, request, context):
+        """Registers new online store to feast core
+        or updates properties for existing online store
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ArchiveOnlineStore(self, request, context):
+        """Archives an online store to mark it deprecated
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_CoreServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetFeastCoreVersion': grpc.unary_unary_rpc_method_handler(
                     servicer.GetFeastCoreVersion,
                     request_deserializer=feast_dot_core_dot_CoreService__pb2.GetFeastCoreVersionRequest.FromString,
                     response_serializer=feast_dot_core_dot_CoreService__pb2.GetFeastCoreVersionResponse.SerializeToString,
@@ -294,14 +341,34 @@
                     response_serializer=feast_dot_core_dot_CoreService__pb2.GetFeatureTableResponse.SerializeToString,
             ),
             'DeleteFeatureTable': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteFeatureTable,
                     request_deserializer=feast_dot_core_dot_CoreService__pb2.DeleteFeatureTableRequest.FromString,
                     response_serializer=feast_dot_core_dot_CoreService__pb2.DeleteFeatureTableResponse.SerializeToString,
             ),
+            'ListOnlineStores': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListOnlineStores,
+                    request_deserializer=feast_dot_core_dot_CoreService__pb2.ListOnlineStoresRequest.FromString,
+                    response_serializer=feast_dot_core_dot_CoreService__pb2.ListOnlineStoresResponse.SerializeToString,
+            ),
+            'GetOnlineStore': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetOnlineStore,
+                    request_deserializer=feast_dot_core_dot_CoreService__pb2.GetOnlineStoreRequest.FromString,
+                    response_serializer=feast_dot_core_dot_CoreService__pb2.GetOnlineStoreResponse.SerializeToString,
+            ),
+            'RegisterOnlineStore': grpc.unary_unary_rpc_method_handler(
+                    servicer.RegisterOnlineStore,
+                    request_deserializer=feast_dot_core_dot_CoreService__pb2.RegisterOnlineStoreRequest.FromString,
+                    response_serializer=feast_dot_core_dot_CoreService__pb2.RegisterOnlineStoreResponse.SerializeToString,
+            ),
+            'ArchiveOnlineStore': grpc.unary_unary_rpc_method_handler(
+                    servicer.ArchiveOnlineStore,
+                    request_deserializer=feast_dot_core_dot_CoreService__pb2.ArchiveOnlineStoreRequest.FromString,
+                    response_serializer=feast_dot_core_dot_CoreService__pb2.ArchiveOnlineStoreResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'feast.core.CoreService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -541,7 +608,75 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/feast.core.CoreService/DeleteFeatureTable',
             feast_dot_core_dot_CoreService__pb2.DeleteFeatureTableRequest.SerializeToString,
             feast_dot_core_dot_CoreService__pb2.DeleteFeatureTableResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ListOnlineStores(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/feast.core.CoreService/ListOnlineStores',
+            feast_dot_core_dot_CoreService__pb2.ListOnlineStoresRequest.SerializeToString,
+            feast_dot_core_dot_CoreService__pb2.ListOnlineStoresResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetOnlineStore(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/feast.core.CoreService/GetOnlineStore',
+            feast_dot_core_dot_CoreService__pb2.GetOnlineStoreRequest.SerializeToString,
+            feast_dot_core_dot_CoreService__pb2.GetOnlineStoreResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def RegisterOnlineStore(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/feast.core.CoreService/RegisterOnlineStore',
+            feast_dot_core_dot_CoreService__pb2.RegisterOnlineStoreRequest.SerializeToString,
+            feast_dot_core_dot_CoreService__pb2.RegisterOnlineStoreResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ArchiveOnlineStore(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/feast.core.CoreService/ArchiveOnlineStore',
+            feast_dot_core_dot_CoreService__pb2.ArchiveOnlineStoreRequest.SerializeToString,
+            feast_dot_core_dot_CoreService__pb2.ArchiveOnlineStoreResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `feast-0.9.8/feast/protos/feast/core/DataFormat_pb2.py` & `feast-0.9.9/feast/protos/feast/core/DataFormat_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/core/DataSource_pb2.py` & `feast-0.9.9/feast/protos/feast/core/DataSource_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/core/Entity_pb2.py` & `feast-0.9.9/feast/protos/feast/core/Entity_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/core/Entity_pb2.pyi` & `feast-0.9.9/feast/protos/feast/core/FeatureView_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
-import feast.types.Value_pb2
+import feast.core.DataSource_pb2
+import feast.core.Feature_pb2
 import google.protobuf.descriptor
+import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
 
-class Entity(google.protobuf.message.Message):
+class FeatureView(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     SPEC_FIELD_NUMBER: builtins.int
     META_FIELD_NUMBER: builtins.int
 
     @property
-    def spec(self) -> global___EntitySpecV2: ...
+    def spec(self) -> global___FeatureViewSpec: ...
 
     @property
-    def meta(self) -> global___EntityMeta: ...
+    def meta(self) -> global___FeatureViewMeta: ...
 
     def __init__(self,
         *,
-        spec : typing.Optional[global___EntitySpecV2] = ...,
-        meta : typing.Optional[global___EntityMeta] = ...,
+        spec : typing.Optional[global___FeatureViewSpec] = ...,
+        meta : typing.Optional[global___FeatureViewMeta] = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal[u"meta",b"meta",u"spec",b"spec"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal[u"meta",b"meta",u"spec",b"spec"]) -> None: ...
-global___Entity = Entity
+global___FeatureView = FeatureView
 
-class EntitySpecV2(google.protobuf.message.Message):
+class FeatureViewSpec(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class LabelsEntry(google.protobuf.message.Message):
+    class TagsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: typing.Text = ...
         value: typing.Text = ...
 
         def __init__(self,
@@ -47,37 +49,53 @@
             key : typing.Text = ...,
             value : typing.Text = ...,
             ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
 
     NAME_FIELD_NUMBER: builtins.int
     PROJECT_FIELD_NUMBER: builtins.int
-    VALUE_TYPE_FIELD_NUMBER: builtins.int
-    DESCRIPTION_FIELD_NUMBER: builtins.int
-    LABELS_FIELD_NUMBER: builtins.int
+    ENTITIES_FIELD_NUMBER: builtins.int
+    FEATURES_FIELD_NUMBER: builtins.int
+    TAGS_FIELD_NUMBER: builtins.int
+    TTL_FIELD_NUMBER: builtins.int
+    INPUT_FIELD_NUMBER: builtins.int
+    ONLINE_FIELD_NUMBER: builtins.int
     name: typing.Text = ...
     project: typing.Text = ...
-    value_type: feast.types.Value_pb2.ValueType.Enum.V = ...
-    description: typing.Text = ...
+    entities: google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text] = ...
+    online: builtins.bool = ...
 
     @property
-    def labels(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
+    def features(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[feast.core.Feature_pb2.FeatureSpecV2]: ...
+
+    @property
+    def tags(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
+
+    @property
+    def ttl(self) -> google.protobuf.duration_pb2.Duration: ...
+
+    @property
+    def input(self) -> feast.core.DataSource_pb2.DataSource: ...
 
     def __init__(self,
         *,
         name : typing.Text = ...,
         project : typing.Text = ...,
-        value_type : feast.types.Value_pb2.ValueType.Enum.V = ...,
-        description : typing.Text = ...,
-        labels : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
+        entities : typing.Optional[typing.Iterable[typing.Text]] = ...,
+        features : typing.Optional[typing.Iterable[feast.core.Feature_pb2.FeatureSpecV2]] = ...,
+        tags : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
+        ttl : typing.Optional[google.protobuf.duration_pb2.Duration] = ...,
+        input : typing.Optional[feast.core.DataSource_pb2.DataSource] = ...,
+        online : builtins.bool = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"description",b"description",u"labels",b"labels",u"name",b"name",u"project",b"project",u"value_type",b"value_type"]) -> None: ...
-global___EntitySpecV2 = EntitySpecV2
+    def HasField(self, field_name: typing_extensions.Literal[u"input",b"input",u"ttl",b"ttl"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal[u"entities",b"entities",u"features",b"features",u"input",b"input",u"name",b"name",u"online",b"online",u"project",b"project",u"tags",b"tags",u"ttl",b"ttl"]) -> None: ...
+global___FeatureViewSpec = FeatureViewSpec
 
-class EntityMeta(google.protobuf.message.Message):
+class FeatureViewMeta(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
     CREATED_TIMESTAMP_FIELD_NUMBER: builtins.int
     LAST_UPDATED_TIMESTAMP_FIELD_NUMBER: builtins.int
 
     @property
     def created_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
 
@@ -87,8 +105,8 @@
     def __init__(self,
         *,
         created_timestamp : typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
         last_updated_timestamp : typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
         ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal[u"created_timestamp",b"created_timestamp",u"last_updated_timestamp",b"last_updated_timestamp"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal[u"created_timestamp",b"created_timestamp",u"last_updated_timestamp",b"last_updated_timestamp"]) -> None: ...
-global___EntityMeta = EntityMeta
+global___FeatureViewMeta = FeatureViewMeta
```

### Comparing `feast-0.9.8/feast/protos/feast/core/FeatureTable_pb2.py` & `feast-0.9.9/feast/core/FeatureTable_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: feast/core/FeatureTable.proto
-"""Generated protocol buffer code."""
+
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
-
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from feast.core import DataSource_pb2 as feast_dot_core_dot_DataSource__pb2
+from feast.core import Feature_pb2 as feast_dot_core_dot_Feature__pb2
+from feast.core import OnlineStore_pb2 as feast_dot_core_dot_OnlineStore__pb2
 
-from feast.protos.feast.core import DataSource_pb2 as feast_dot_core_dot_DataSource__pb2
-from feast.protos.feast.core import Feature_pb2 as feast_dot_core_dot_Feature__pb2
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='feast/core/FeatureTable.proto',
   package='feast.core',
   syntax='proto3',
   serialized_options=b'\n\020feast.proto.coreB\021FeatureTableProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/core',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1d\x66\x65\x61st/core/FeatureTable.proto\x12\nfeast.core\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1b\x66\x65\x61st/core/DataSource.proto\x1a\x18\x66\x65\x61st/core/Feature.proto\"f\n\x0c\x46\x65\x61tureTable\x12*\n\x04spec\x18\x01 \x01(\x0b\x32\x1c.feast.core.FeatureTableSpec\x12*\n\x04meta\x18\x02 \x01(\x0b\x32\x1c.feast.core.FeatureTableMeta\"\xe2\x02\n\x10\x46\x65\x61tureTableSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07project\x18\t \x01(\t\x12\x10\n\x08\x65ntities\x18\x03 \x03(\t\x12+\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32\x19.feast.core.FeatureSpecV2\x12\x38\n\x06labels\x18\x05 \x03(\x0b\x32(.feast.core.FeatureTableSpec.LabelsEntry\x12*\n\x07max_age\x18\x06 \x01(\x0b\x32\x19.google.protobuf.Duration\x12,\n\x0c\x62\x61tch_source\x18\x07 \x01(\x0b\x32\x16.feast.core.DataSource\x12-\n\rstream_source\x18\x08 \x01(\x0b\x32\x16.feast.core.DataSource\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa5\x01\n\x10\x46\x65\x61tureTableMeta\x12\x35\n\x11\x63reated_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_updated_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08revision\x18\x03 \x01(\x03\x12\x0c\n\x04hash\x18\x04 \x01(\tBZ\n\x10\x66\x65\x61st.proto.coreB\x11\x46\x65\x61tureTableProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/coreb\x06proto3'
+  serialized_pb=b'\n\x1d\x66\x65\x61st/core/FeatureTable.proto\x12\nfeast.core\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1b\x66\x65\x61st/core/DataSource.proto\x1a\x18\x66\x65\x61st/core/Feature.proto\x1a\x1c\x66\x65\x61st/core/OnlineStore.proto\"f\n\x0c\x46\x65\x61tureTable\x12*\n\x04spec\x18\x01 \x01(\x0b\x32\x1c.feast.core.FeatureTableSpec\x12*\n\x04meta\x18\x02 \x01(\x0b\x32\x1c.feast.core.FeatureTableMeta\"\xb8\x03\n\x10\x46\x65\x61tureTableSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x65ntities\x18\x03 \x03(\t\x12+\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32\x19.feast.core.FeatureSpecV2\x12\x38\n\x06labels\x18\x05 \x03(\x0b\x32(.feast.core.FeatureTableSpec.LabelsEntry\x12*\n\x07max_age\x18\x06 \x01(\x0b\x32\x19.google.protobuf.Duration\x12,\n\x0c\x62\x61tch_source\x18\x07 \x01(\x0b\x32\x16.feast.core.DataSource\x12-\n\rstream_source\x18\x08 \x01(\x0b\x32\x16.feast.core.DataSource\x12\x36\n\x13staleness_threshold\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\x12-\n\x0conline_store\x18\n \x01(\x0b\x32\x17.feast.core.OnlineStore\x1a-\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xa5\x01\n\x10\x46\x65\x61tureTableMeta\x12\x35\n\x11\x63reated_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_updated_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08revision\x18\x03 \x01(\x03\x12\x0c\n\x04hash\x18\x04 \x01(\tBZ\n\x10\x66\x65\x61st.proto.coreB\x11\x46\x65\x61tureTableProtoZ3github.com/feast-dev/feast/sdk/go/protos/feast/coreb\x06proto3'
   ,
-  dependencies=[google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,feast_dot_core_dot_DataSource__pb2.DESCRIPTOR,feast_dot_core_dot_Feature__pb2.DESCRIPTOR,])
+  dependencies=[google_dot_protobuf_dot_duration__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,feast_dot_core_dot_DataSource__pb2.DESCRIPTOR,feast_dot_core_dot_Feature__pb2.DESCRIPTOR,feast_dot_core_dot_OnlineStore__pb2.DESCRIPTOR,])
 
 
 
 
 _FEATURETABLE = _descriptor.Descriptor(
   name='FeatureTable',
   full_name='feast.core.FeatureTable',
@@ -61,16 +61,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=165,
-  serialized_end=267,
+  serialized_start=195,
+  serialized_end=297,
 )
 
 
 _FEATURETABLESPEC_LABELSENTRY = _descriptor.Descriptor(
   name='LabelsEntry',
   full_name='feast.core.FeatureTableSpec.LabelsEntry',
   filename=None,
@@ -100,16 +100,16 @@
   ],
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=579,
-  serialized_end=624,
+  serialized_start=695,
+  serialized_end=740,
 )
 
 _FEATURETABLESPEC = _descriptor.Descriptor(
   name='FeatureTableSpec',
   full_name='feast.core.FeatureTableSpec',
   filename=None,
   file=DESCRIPTOR,
@@ -120,76 +120,83 @@
       name='name', full_name='feast.core.FeatureTableSpec.name', index=0,
       number=1, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=b"".decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='project', full_name='feast.core.FeatureTableSpec.project', index=1,
-      number=9, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='entities', full_name='feast.core.FeatureTableSpec.entities', index=2,
+      name='entities', full_name='feast.core.FeatureTableSpec.entities', index=1,
       number=3, type=9, cpp_type=9, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='features', full_name='feast.core.FeatureTableSpec.features', index=3,
+      name='features', full_name='feast.core.FeatureTableSpec.features', index=2,
       number=4, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='labels', full_name='feast.core.FeatureTableSpec.labels', index=4,
+      name='labels', full_name='feast.core.FeatureTableSpec.labels', index=3,
       number=5, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='max_age', full_name='feast.core.FeatureTableSpec.max_age', index=5,
+      name='max_age', full_name='feast.core.FeatureTableSpec.max_age', index=4,
       number=6, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='batch_source', full_name='feast.core.FeatureTableSpec.batch_source', index=6,
+      name='batch_source', full_name='feast.core.FeatureTableSpec.batch_source', index=5,
       number=7, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
     _descriptor.FieldDescriptor(
-      name='stream_source', full_name='feast.core.FeatureTableSpec.stream_source', index=7,
+      name='stream_source', full_name='feast.core.FeatureTableSpec.stream_source', index=6,
       number=8, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='staleness_threshold', full_name='feast.core.FeatureTableSpec.staleness_threshold', index=7,
+      number=9, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='online_store', full_name='feast.core.FeatureTableSpec.online_store', index=8,
+      number=10, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[_FEATURETABLESPEC_LABELSENTRY, ],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=270,
-  serialized_end=624,
+  serialized_start=300,
+  serialized_end=740,
 )
 
 
 _FEATURETABLEMETA = _descriptor.Descriptor(
   name='FeatureTableMeta',
   full_name='feast.core.FeatureTableMeta',
   filename=None,
@@ -233,26 +240,28 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=627,
-  serialized_end=792,
+  serialized_start=743,
+  serialized_end=908,
 )
 
 _FEATURETABLE.fields_by_name['spec'].message_type = _FEATURETABLESPEC
 _FEATURETABLE.fields_by_name['meta'].message_type = _FEATURETABLEMETA
 _FEATURETABLESPEC_LABELSENTRY.containing_type = _FEATURETABLESPEC
 _FEATURETABLESPEC.fields_by_name['features'].message_type = feast_dot_core_dot_Feature__pb2._FEATURESPECV2
 _FEATURETABLESPEC.fields_by_name['labels'].message_type = _FEATURETABLESPEC_LABELSENTRY
 _FEATURETABLESPEC.fields_by_name['max_age'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
 _FEATURETABLESPEC.fields_by_name['batch_source'].message_type = feast_dot_core_dot_DataSource__pb2._DATASOURCE
 _FEATURETABLESPEC.fields_by_name['stream_source'].message_type = feast_dot_core_dot_DataSource__pb2._DATASOURCE
+_FEATURETABLESPEC.fields_by_name['staleness_threshold'].message_type = google_dot_protobuf_dot_duration__pb2._DURATION
+_FEATURETABLESPEC.fields_by_name['online_store'].message_type = feast_dot_core_dot_OnlineStore__pb2._ONLINESTORE
 _FEATURETABLEMETA.fields_by_name['created_timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _FEATURETABLEMETA.fields_by_name['last_updated_timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 DESCRIPTOR.message_types_by_name['FeatureTable'] = _FEATURETABLE
 DESCRIPTOR.message_types_by_name['FeatureTableSpec'] = _FEATURETABLESPEC
 DESCRIPTOR.message_types_by_name['FeatureTableMeta'] = _FEATURETABLEMETA
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
```

### Comparing `feast-0.9.8/feast/protos/feast/core/FeatureView_pb2.py` & `feast-0.9.9/feast/protos/feast/core/FeatureView_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/core/Feature_pb2.py` & `feast-0.9.9/feast/protos/feast/core/Feature_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/core/Feature_pb2.pyi` & `feast-0.9.9/feast/protos/feast/storage/Redis_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -8,40 +8,26 @@
 import google.protobuf.internal.containers
 import google.protobuf.message
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
 
-class FeatureSpecV2(google.protobuf.message.Message):
+class RedisKeyV2(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    class LabelsEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text = ...
-        value: typing.Text = ...
-
-        def __init__(self,
-            *,
-            key : typing.Text = ...,
-            value : typing.Text = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal[u"key",b"key",u"value",b"value"]) -> None: ...
-
-    NAME_FIELD_NUMBER: builtins.int
-    VALUE_TYPE_FIELD_NUMBER: builtins.int
-    LABELS_FIELD_NUMBER: builtins.int
-    name: typing.Text = ...
-    value_type: feast.types.Value_pb2.ValueType.Enum.V = ...
+    PROJECT_FIELD_NUMBER: builtins.int
+    ENTITY_NAMES_FIELD_NUMBER: builtins.int
+    ENTITY_VALUES_FIELD_NUMBER: builtins.int
+    project: typing.Text = ...
+    entity_names: google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text] = ...
 
     @property
-    def labels(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]: ...
+    def entity_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[feast.types.Value_pb2.Value]: ...
 
     def __init__(self,
         *,
-        name : typing.Text = ...,
-        value_type : feast.types.Value_pb2.ValueType.Enum.V = ...,
-        labels : typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
+        project : typing.Text = ...,
+        entity_names : typing.Optional[typing.Iterable[typing.Text]] = ...,
+        entity_values : typing.Optional[typing.Iterable[feast.types.Value_pb2.Value]] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"labels",b"labels",u"name",b"name",u"value_type",b"value_type"]) -> None: ...
-global___FeatureSpecV2 = FeatureSpecV2
+    def ClearField(self, field_name: typing_extensions.Literal[u"entity_names",b"entity_names",u"entity_values",b"entity_values",u"project",b"project"]) -> None: ...
+global___RedisKeyV2 = RedisKeyV2
```

### Comparing `feast-0.9.8/feast/protos/feast/core/Registry_pb2.py` & `feast-0.9.9/feast/protos/feast/core/Registry_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/core/Registry_pb2.pyi` & `feast-0.9.9/feast/protos/feast/core/Registry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/core/Store_pb2.py` & `feast-0.9.9/feast/protos/feast/core/Store_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/serving/ServingService_pb2.py` & `feast-0.9.9/feast/protos/feast/serving/ServingService_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/serving/ServingService_pb2.pyi` & `feast-0.9.9/feast/protos/feast/serving/ServingService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/serving/ServingService_pb2_grpc.py` & `feast-0.9.9/feast/protos/feast/serving/ServingService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/storage/Redis_pb2.py` & `feast-0.9.9/feast/protos/feast/storage/Redis_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/storage/Redis_pb2.pyi` & `feast-0.9.9/feast/protos/feast/types/Field_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import feast.types.Value_pb2
 import google.protobuf.descriptor
-import google.protobuf.internal.containers
 import google.protobuf.message
 import typing
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
 
-class RedisKeyV2(google.protobuf.message.Message):
+class Field(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    PROJECT_FIELD_NUMBER: builtins.int
-    ENTITY_NAMES_FIELD_NUMBER: builtins.int
-    ENTITY_VALUES_FIELD_NUMBER: builtins.int
-    project: typing.Text = ...
-    entity_names: google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text] = ...
+    NAME_FIELD_NUMBER: builtins.int
+    VALUE_FIELD_NUMBER: builtins.int
+    name: typing.Text = ...
 
     @property
-    def entity_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[feast.types.Value_pb2.Value]: ...
+    def value(self) -> feast.types.Value_pb2.Value: ...
 
     def __init__(self,
         *,
-        project : typing.Text = ...,
-        entity_names : typing.Optional[typing.Iterable[typing.Text]] = ...,
-        entity_values : typing.Optional[typing.Iterable[feast.types.Value_pb2.Value]] = ...,
+        name : typing.Text = ...,
+        value : typing.Optional[feast.types.Value_pb2.Value] = ...,
         ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"entity_names",b"entity_names",u"entity_values",b"entity_values",u"project",b"project"]) -> None: ...
-global___RedisKeyV2 = RedisKeyV2
+    def HasField(self, field_name: typing_extensions.Literal[u"value",b"value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name",u"value",b"value"]) -> None: ...
+global___Field = Field
```

### Comparing `feast-0.9.8/feast/protos/feast/types/EntityKey_pb2.py` & `feast-0.9.9/feast/protos/feast/types/EntityKey_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/types/EntityKey_pb2.pyi` & `feast-0.9.9/feast/protos/feast/types/EntityKey_pb2.pyi`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/types/Field_pb2.py` & `feast-0.9.9/feast/protos/feast/types/Field_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/types/Field_pb2.pyi` & `feast-0.9.9/feast/types/Field_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,50 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
-import builtins
-import feast.types.Value_pb2
-import google.protobuf.descriptor
-import google.protobuf.message
-import typing
-import typing_extensions
-
-DESCRIPTOR: google.protobuf.descriptor.FileDescriptor = ...
-
-class Field(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor = ...
-    NAME_FIELD_NUMBER: builtins.int
-    VALUE_FIELD_NUMBER: builtins.int
-    name: typing.Text = ...
+from feast.types.Value_pb2 import (
+    Value as feast___types___Value_pb2___Value,
+)
+
+from google.protobuf.descriptor import (
+    Descriptor as google___protobuf___descriptor___Descriptor,
+    FileDescriptor as google___protobuf___descriptor___FileDescriptor,
+)
+
+from google.protobuf.message import (
+    Message as google___protobuf___message___Message,
+)
+
+from typing import (
+    Optional as typing___Optional,
+    Text as typing___Text,
+)
+
+from typing_extensions import (
+    Literal as typing_extensions___Literal,
+)
+
+
+builtin___bool = bool
+builtin___bytes = bytes
+builtin___float = float
+builtin___int = int
+
+
+DESCRIPTOR: google___protobuf___descriptor___FileDescriptor = ...
+
+class Field(google___protobuf___message___Message):
+    DESCRIPTOR: google___protobuf___descriptor___Descriptor = ...
+    name: typing___Text = ...
 
     @property
-    def value(self) -> feast.types.Value_pb2.Value: ...
+    def value(self) -> feast___types___Value_pb2___Value: ...
 
     def __init__(self,
         *,
-        name : typing.Text = ...,
-        value : typing.Optional[feast.types.Value_pb2.Value] = ...,
+        name : typing___Optional[typing___Text] = None,
+        value : typing___Optional[feast___types___Value_pb2___Value] = None,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal[u"value",b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal[u"name",b"name",u"value",b"value"]) -> None: ...
-global___Field = Field
+    def HasField(self, field_name: typing_extensions___Literal[u"value",b"value"]) -> builtin___bool: ...
+    def ClearField(self, field_name: typing_extensions___Literal[u"name",b"name",u"value",b"value"]) -> None: ...
+type___Field = Field
```

### Comparing `feast-0.9.8/feast/protos/feast/types/Value_pb2.py` & `feast-0.9.9/feast/protos/feast/types/Value_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/protos/feast/types/Value_pb2.pyi` & `feast-0.9.9/feast/protos/feast/types/Value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/pyspark/abc.py` & `feast-0.9.9/feast/pyspark/abc.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/pyspark/historical_feature_retrieval_job.py` & `feast-0.9.9/feast/pyspark/historical_feature_retrieval_job.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/pyspark/launcher.py` & `feast-0.9.9/feast/pyspark/launcher.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/pyspark/launchers/aws/emr.py` & `feast-0.9.9/feast/pyspark/launchers/aws/emr.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/pyspark/launchers/aws/emr_utils.py` & `feast-0.9.9/feast/pyspark/launchers/aws/emr_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
             + args,
             "Jar": "command-runner.jar",
         },
     }
 
 
 class EmrJobRef(NamedTuple):
-    """ EMR job reference. step_id can be None when using on-demand clusters, in that case each
-    cluster has only one step """
+    """EMR job reference. step_id can be None when using on-demand clusters, in that case each
+    cluster has only one step"""
 
     cluster_id: str
     step_id: Optional[str]
 
 
 def _job_ref_to_str(job_ref: EmrJobRef) -> str:
     return ":".join(["emr", job_ref.cluster_id, job_ref.step_id or ""])
```

### Comparing `feast-0.9.8/feast/pyspark/launchers/gcloud/dataproc.py` & `feast-0.9.9/feast/pyspark/launchers/gcloud/dataproc.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/pyspark/launchers/k8s/k8s.py` & `feast-0.9.9/feast/pyspark/launchers/k8s/k8s.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         assert job is not None
         return job.start_time
 
     def cancel(self):
         _cancel_job_by_id(self._api, self._namespace, self._job_id)
 
     def _wait_for_complete(self, timeout_seconds: Optional[float]) -> bool:
-        """ Returns true if the job completed successfully """
+        """Returns true if the job completed successfully"""
         start_time = time.time()
         while (timeout_seconds is None) or (time.time() - start_time < timeout_seconds):
             status = self.get_status()
             if status == SparkJobStatus.COMPLETED:
                 return True
             elif status == SparkJobStatus.FAILED:
                 return False
```

### Comparing `feast-0.9.8/feast/pyspark/launchers/k8s/k8s_utils.py` & `feast-0.9.9/feast/pyspark/launchers/k8s/k8s_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 METADATA_OUTPUT_URI = "dev.feast.outputuri"
 METADATA_JOBHASH = "dev.feast.jobhash"
 
 METADATA_KEYS = set((METADATA_JOBHASH, METADATA_OUTPUT_URI))
 
 
 def _append_items(resource: Dict[str, Any], path: Tuple[str, ...], items: List[Any]):
-    """ A helper function to manipulate k8s resource configs. It updates an array in resource
+    """A helper function to manipulate k8s resource configs. It updates an array in resource
         definition given a jsonpath-like path. Will not update resource if items is empty.
         Note that it updates resource dict in-place.
 
     Examples:
         >>> _append_items({}, ("foo", "bar"), ["A", "B"])
         {'foo': {'bar': ['A', 'B']}}
 
@@ -68,15 +68,15 @@
         obj = obj[p]
     assert isinstance(obj, list)
     obj.extend(items)
     return resource
 
 
 def _add_keys(resource: Dict[str, Any], path: Tuple[str, ...], items: Dict[str, Any]):
-    """ A helper function to manipulate k8s resource configs. It will update a dict in resource
+    """A helper function to manipulate k8s resource configs. It will update a dict in resource
         definition given a path (think jsonpath). Will ignore items set to None. Will not update
         resource if all items are None. Note that it updates resource dict in-place.
 
     Examples:
         >>> _add_keys({}, ("foo", "bar"), {"A": 1, "B": 2})
         {'foo': {'bar': {'A': 1, 'B': 2}}}
 
@@ -116,15 +116,15 @@
     jars: List[str],
     extra_metadata: Dict[str, str],
     azure_credentials: Dict[str, str],
     arguments: List[str],
     namespace: str,
     extra_labels: Dict[str, str] = None,
 ) -> Dict[str, Any]:
-    """ Prepare SparkApplication custom resource configs """
+    """Prepare SparkApplication custom resource configs"""
     job = deepcopy(job_template)
 
     labels = {LABEL_JOBID: job_id, LABEL_JOBTYPE: job_type}
     if extra_labels:
         labels = {**labels, **extra_labels}
 
     _add_keys(job, ("metadata", "labels"), labels)
```

### Comparing `feast-0.9.8/feast/pyspark/launchers/standalone/local.py` & `feast-0.9.9/feast/pyspark/launchers/standalone/local.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/remote_job.py` & `feast-0.9.9/feast/remote_job.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/serving/ServingService_pb2.py` & `feast-0.9.9/feast/serving/ServingService_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,93 +19,105 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='feast/serving/ServingService.proto',
   package='feast.serving',
   syntax='proto3',
   serialized_options=b'\n\023feast.proto.servingB\017ServingAPIProtoZ6github.com/feast-dev/feast/sdk/go/protos/feast/serving',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\"feast/serving/ServingService.proto\x12\rfeast.serving\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17\x66\x65\x61st/types/Value.proto\x1a-tensorflow_metadata/proto/v0/statistics.proto\"\x1c\n\x1aGetFeastServingInfoRequest\"{\n\x1bGetFeastServingInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\x12-\n\x04type\x18\x02 \x01(\x0e\x32\x1f.feast.serving.FeastServingType\x12\x1c\n\x14job_staging_location\x18\n \x01(\t\"9\n\x12\x46\x65\x61tureReferenceV2\x12\x15\n\rfeature_table\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xfd\x02\n\x1aGetOnlineFeaturesRequestV2\x12\x33\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32!.feast.serving.FeatureReferenceV2\x12H\n\x0b\x65ntity_rows\x18\x02 \x03(\x0b\x32\x33.feast.serving.GetOnlineFeaturesRequestV2.EntityRow\x12\x0f\n\x07project\x18\x05 \x01(\t\x1a\xce\x01\n\tEntityRow\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12O\n\x06\x66ields\x18\x02 \x03(\x0b\x32?.feast.serving.GetOnlineFeaturesRequestV2.EntityRow.FieldsEntry\x1a\x41\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.feast.types.Value:\x02\x38\x01\"\xa6\x04\n\x19GetOnlineFeaturesResponse\x12J\n\x0c\x66ield_values\x18\x01 \x03(\x0b\x32\x34.feast.serving.GetOnlineFeaturesResponse.FieldValues\x1a\xdf\x02\n\x0b\x46ieldValues\x12P\n\x06\x66ields\x18\x01 \x03(\x0b\x32@.feast.serving.GetOnlineFeaturesResponse.FieldValues.FieldsEntry\x12T\n\x08statuses\x18\x02 \x03(\x0b\x32\x42.feast.serving.GetOnlineFeaturesResponse.FieldValues.StatusesEntry\x1a\x41\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.feast.types.Value:\x02\x38\x01\x1a\x65\n\rStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x43\n\x05value\x18\x02 \x01(\x0e\x32\x34.feast.serving.GetOnlineFeaturesResponse.FieldStatus:\x02\x38\x01\"[\n\x0b\x46ieldStatus\x12\x0b\n\x07INVALID\x10\x00\x12\x0b\n\x07PRESENT\x10\x01\x12\x0e\n\nNULL_VALUE\x10\x02\x12\r\n\tNOT_FOUND\x10\x03\x12\x13\n\x0fOUTSIDE_MAX_AGE\x10\x04*o\n\x10\x46\x65\x61stServingType\x12\x1e\n\x1a\x46\x45\x41ST_SERVING_TYPE_INVALID\x10\x00\x12\x1d\n\x19\x46\x45\x41ST_SERVING_TYPE_ONLINE\x10\x01\x12\x1c\n\x18\x46\x45\x41ST_SERVING_TYPE_BATCH\x10\x02\x32\xea\x01\n\x0eServingService\x12l\n\x13GetFeastServingInfo\x12).feast.serving.GetFeastServingInfoRequest\x1a*.feast.serving.GetFeastServingInfoResponse\x12j\n\x13GetOnlineFeaturesV2\x12).feast.serving.GetOnlineFeaturesRequestV2\x1a(.feast.serving.GetOnlineFeaturesResponseB^\n\x13\x66\x65\x61st.proto.servingB\x0fServingAPIProtoZ6github.com/feast-dev/feast/sdk/go/protos/feast/servingb\x06proto3'
+  serialized_pb=b'\n\"feast/serving/ServingService.proto\x12\rfeast.serving\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17\x66\x65\x61st/types/Value.proto\x1a-tensorflow_metadata/proto/v0/statistics.proto\"\x1c\n\x1aGetFeastServingInfoRequest\"{\n\x1bGetFeastServingInfoResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\x12-\n\x04type\x18\x02 \x01(\x0e\x32\x1f.feast.serving.FeastServingType\x12\x1c\n\x14job_staging_location\x18\n \x01(\t\"9\n\x12\x46\x65\x61tureReferenceV2\x12\x15\n\rfeature_table\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xfd\x02\n\x1aGetOnlineFeaturesRequestV2\x12\x33\n\x08\x66\x65\x61tures\x18\x04 \x03(\x0b\x32!.feast.serving.FeatureReferenceV2\x12H\n\x0b\x65ntity_rows\x18\x02 \x03(\x0b\x32\x33.feast.serving.GetOnlineFeaturesRequestV2.EntityRow\x12\x0f\n\x07project\x18\x05 \x01(\t\x1a\xce\x01\n\tEntityRow\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12O\n\x06\x66ields\x18\x02 \x03(\x0b\x32?.feast.serving.GetOnlineFeaturesRequestV2.EntityRow.FieldsEntry\x1a\x41\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.feast.types.Value:\x02\x38\x01\"\xaf\x03\n\x19GetOnlineFeaturesResponse\x12J\n\x0c\x66ield_values\x18\x01 \x03(\x0b\x32\x34.feast.serving.GetOnlineFeaturesResponse.FieldValues\x1a\xc5\x02\n\x0b\x46ieldValues\x12P\n\x06\x66ields\x18\x01 \x03(\x0b\x32@.feast.serving.GetOnlineFeaturesResponse.FieldValues.FieldsEntry\x12T\n\x08statuses\x18\x02 \x03(\x0b\x32\x42.feast.serving.GetOnlineFeaturesResponse.FieldValues.StatusesEntry\x1a\x41\n\x0b\x46ieldsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.feast.types.Value:\x02\x38\x01\x1aK\n\rStatusesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0e\x32\x1a.feast.serving.FieldStatus:\x02\x38\x01\"\x8b\x02\n\x1bGetOnlineFeaturesResponseV2\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.feast.serving.GetOnlineFeaturesResponseMetadata\x12G\n\x07results\x18\x02 \x03(\x0b\x32\x36.feast.serving.GetOnlineFeaturesResponseV2.FieldVector\x1a_\n\x0b\x46ieldVector\x12\"\n\x06values\x18\x01 \x03(\x0b\x32\x12.feast.types.Value\x12,\n\x08statuses\x18\x02 \x03(\x0e\x32\x1a.feast.serving.FieldStatus\"R\n!GetOnlineFeaturesResponseMetadata\x12-\n\x0b\x66ield_names\x18\x01 \x01(\x0b\x32\x18.feast.serving.FieldList\"\x18\n\tFieldList\x12\x0b\n\x03val\x18\x01 \x03(\t*r\n\x0b\x46ieldStatus\x12\x0b\n\x07INVALID\x10\x00\x12\x0b\n\x07PRESENT\x10\x01\x12\x0e\n\nNULL_VALUE\x10\x02\x12\r\n\tNOT_FOUND\x10\x03\x12\x13\n\x0fOUTSIDE_MAX_AGE\x10\x04\x12\x15\n\x11INGESTION_FAILURE\x10\x05*o\n\x10\x46\x65\x61stServingType\x12\x1e\n\x1a\x46\x45\x41ST_SERVING_TYPE_INVALID\x10\x00\x12\x1d\n\x19\x46\x45\x41ST_SERVING_TYPE_ONLINE\x10\x01\x12\x1c\n\x18\x46\x45\x41ST_SERVING_TYPE_BATCH\x10\x02\x32\xd6\x02\n\x0eServingService\x12l\n\x13GetFeastServingInfo\x12).feast.serving.GetFeastServingInfoRequest\x1a*.feast.serving.GetFeastServingInfoResponse\x12j\n\x13GetOnlineFeaturesV2\x12).feast.serving.GetOnlineFeaturesRequestV2\x1a(.feast.serving.GetOnlineFeaturesResponse\x12j\n\x11GetOnlineFeatures\x12).feast.serving.GetOnlineFeaturesRequestV2\x1a*.feast.serving.GetOnlineFeaturesResponseV2B^\n\x13\x66\x65\x61st.proto.servingB\x0fServingAPIProtoZ6github.com/feast-dev/feast/sdk/go/protos/feast/servingb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,feast_dot_types_dot_Value__pb2.DESCRIPTOR,tensorflow__metadata_dot_proto_dot_v0_dot_statistics__pb2.DESCRIPTOR,])
 
-_FEASTSERVINGTYPE = _descriptor.EnumDescriptor(
-  name='FeastServingType',
-  full_name='feast.serving.FeastServingType',
+_FIELDSTATUS = _descriptor.EnumDescriptor(
+  name='FieldStatus',
+  full_name='feast.serving.FieldStatus',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='FEAST_SERVING_TYPE_INVALID', index=0, number=0,
+      name='INVALID', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='FEAST_SERVING_TYPE_ONLINE', index=1, number=1,
+      name='PRESENT', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='FEAST_SERVING_TYPE_BATCH', index=2, number=2,
+      name='NULL_VALUE', index=2, number=2,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='NOT_FOUND', index=3, number=3,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='OUTSIDE_MAX_AGE', index=4, number=4,
+      serialized_options=None,
+      type=None,
+      create_key=_descriptor._internal_create_key),
+    _descriptor.EnumValueDescriptor(
+      name='INGESTION_FAILURE', index=5, number=5,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1309,
-  serialized_end=1420,
+  serialized_start=1570,
+  serialized_end=1684,
 )
-_sym_db.RegisterEnumDescriptor(_FEASTSERVINGTYPE)
-
-FeastServingType = enum_type_wrapper.EnumTypeWrapper(_FEASTSERVINGTYPE)
-FEAST_SERVING_TYPE_INVALID = 0
-FEAST_SERVING_TYPE_ONLINE = 1
-FEAST_SERVING_TYPE_BATCH = 2
+_sym_db.RegisterEnumDescriptor(_FIELDSTATUS)
 
-
-_GETONLINEFEATURESRESPONSE_FIELDSTATUS = _descriptor.EnumDescriptor(
-  name='FieldStatus',
-  full_name='feast.serving.GetOnlineFeaturesResponse.FieldStatus',
+FieldStatus = enum_type_wrapper.EnumTypeWrapper(_FIELDSTATUS)
+_FEASTSERVINGTYPE = _descriptor.EnumDescriptor(
+  name='FeastServingType',
+  full_name='feast.serving.FeastServingType',
   filename=None,
   file=DESCRIPTOR,
   create_key=_descriptor._internal_create_key,
   values=[
     _descriptor.EnumValueDescriptor(
-      name='INVALID', index=0, number=0,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='PRESENT', index=1, number=1,
-      serialized_options=None,
-      type=None,
-      create_key=_descriptor._internal_create_key),
-    _descriptor.EnumValueDescriptor(
-      name='NULL_VALUE', index=2, number=2,
+      name='FEAST_SERVING_TYPE_INVALID', index=0, number=0,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='NOT_FOUND', index=3, number=3,
+      name='FEAST_SERVING_TYPE_ONLINE', index=1, number=1,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
     _descriptor.EnumValueDescriptor(
-      name='OUTSIDE_MAX_AGE', index=4, number=4,
+      name='FEAST_SERVING_TYPE_BATCH', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=1216,
-  serialized_end=1307,
+  serialized_start=1686,
+  serialized_end=1797,
 )
-_sym_db.RegisterEnumDescriptor(_GETONLINEFEATURESRESPONSE_FIELDSTATUS)
+_sym_db.RegisterEnumDescriptor(_FEASTSERVINGTYPE)
+
+FeastServingType = enum_type_wrapper.EnumTypeWrapper(_FEASTSERVINGTYPE)
+INVALID = 0
+PRESENT = 1
+NULL_VALUE = 2
+NOT_FOUND = 3
+OUTSIDE_MAX_AGE = 4
+INGESTION_FAILURE = 5
+FEAST_SERVING_TYPE_INVALID = 0
+FEAST_SERVING_TYPE_ONLINE = 1
+FEAST_SERVING_TYPE_BATCH = 2
+
 
 
 _GETFEASTSERVINGINFOREQUEST = _descriptor.Descriptor(
   name='GetFeastServingInfoRequest',
   full_name='feast.serving.GetFeastServingInfoRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -405,15 +417,15 @@
   serialized_options=b'8\001',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1113,
-  serialized_end=1214,
+  serialized_end=1188,
 )
 
 _GETONLINEFEATURESRESPONSE_FIELDVALUES = _descriptor.Descriptor(
   name='FieldValues',
   full_name='feast.serving.GetOnlineFeaturesResponse.FieldValues',
   filename=None,
   file=DESCRIPTOR,
@@ -443,15 +455,15 @@
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=863,
-  serialized_end=1214,
+  serialized_end=1188,
 )
 
 _GETONLINEFEATURESRESPONSE = _descriptor.Descriptor(
   name='GetOnlineFeaturesResponse',
   full_name='feast.serving.GetOnlineFeaturesResponse',
   filename=None,
   file=DESCRIPTOR,
@@ -466,48 +478,197 @@
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[_GETONLINEFEATURESRESPONSE_FIELDVALUES, ],
   enum_types=[
-    _GETONLINEFEATURESRESPONSE_FIELDSTATUS,
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=757,
-  serialized_end=1307,
+  serialized_end=1188,
+)
+
+
+_GETONLINEFEATURESRESPONSEV2_FIELDVECTOR = _descriptor.Descriptor(
+  name='FieldVector',
+  full_name='feast.serving.GetOnlineFeaturesResponseV2.FieldVector',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='values', full_name='feast.serving.GetOnlineFeaturesResponseV2.FieldVector.values', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='statuses', full_name='feast.serving.GetOnlineFeaturesResponseV2.FieldVector.statuses', index=1,
+      number=2, type=14, cpp_type=8, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1363,
+  serialized_end=1458,
+)
+
+_GETONLINEFEATURESRESPONSEV2 = _descriptor.Descriptor(
+  name='GetOnlineFeaturesResponseV2',
+  full_name='feast.serving.GetOnlineFeaturesResponseV2',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='metadata', full_name='feast.serving.GetOnlineFeaturesResponseV2.metadata', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='results', full_name='feast.serving.GetOnlineFeaturesResponseV2.results', index=1,
+      number=2, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[_GETONLINEFEATURESRESPONSEV2_FIELDVECTOR, ],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1191,
+  serialized_end=1458,
+)
+
+
+_GETONLINEFEATURESRESPONSEMETADATA = _descriptor.Descriptor(
+  name='GetOnlineFeaturesResponseMetadata',
+  full_name='feast.serving.GetOnlineFeaturesResponseMetadata',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='field_names', full_name='feast.serving.GetOnlineFeaturesResponseMetadata.field_names', index=0,
+      number=1, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1460,
+  serialized_end=1542,
+)
+
+
+_FIELDLIST = _descriptor.Descriptor(
+  name='FieldList',
+  full_name='feast.serving.FieldList',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='val', full_name='feast.serving.FieldList.val', index=0,
+      number=1, type=9, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1544,
+  serialized_end=1568,
 )
 
 _GETFEASTSERVINGINFORESPONSE.fields_by_name['type'].enum_type = _FEASTSERVINGTYPE
 _GETONLINEFEATURESREQUESTV2_ENTITYROW_FIELDSENTRY.fields_by_name['value'].message_type = feast_dot_types_dot_Value__pb2._VALUE
 _GETONLINEFEATURESREQUESTV2_ENTITYROW_FIELDSENTRY.containing_type = _GETONLINEFEATURESREQUESTV2_ENTITYROW
 _GETONLINEFEATURESREQUESTV2_ENTITYROW.fields_by_name['timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _GETONLINEFEATURESREQUESTV2_ENTITYROW.fields_by_name['fields'].message_type = _GETONLINEFEATURESREQUESTV2_ENTITYROW_FIELDSENTRY
 _GETONLINEFEATURESREQUESTV2_ENTITYROW.containing_type = _GETONLINEFEATURESREQUESTV2
 _GETONLINEFEATURESREQUESTV2.fields_by_name['features'].message_type = _FEATUREREFERENCEV2
 _GETONLINEFEATURESREQUESTV2.fields_by_name['entity_rows'].message_type = _GETONLINEFEATURESREQUESTV2_ENTITYROW
 _GETONLINEFEATURESRESPONSE_FIELDVALUES_FIELDSENTRY.fields_by_name['value'].message_type = feast_dot_types_dot_Value__pb2._VALUE
 _GETONLINEFEATURESRESPONSE_FIELDVALUES_FIELDSENTRY.containing_type = _GETONLINEFEATURESRESPONSE_FIELDVALUES
-_GETONLINEFEATURESRESPONSE_FIELDVALUES_STATUSESENTRY.fields_by_name['value'].enum_type = _GETONLINEFEATURESRESPONSE_FIELDSTATUS
+_GETONLINEFEATURESRESPONSE_FIELDVALUES_STATUSESENTRY.fields_by_name['value'].enum_type = _FIELDSTATUS
 _GETONLINEFEATURESRESPONSE_FIELDVALUES_STATUSESENTRY.containing_type = _GETONLINEFEATURESRESPONSE_FIELDVALUES
 _GETONLINEFEATURESRESPONSE_FIELDVALUES.fields_by_name['fields'].message_type = _GETONLINEFEATURESRESPONSE_FIELDVALUES_FIELDSENTRY
 _GETONLINEFEATURESRESPONSE_FIELDVALUES.fields_by_name['statuses'].message_type = _GETONLINEFEATURESRESPONSE_FIELDVALUES_STATUSESENTRY
 _GETONLINEFEATURESRESPONSE_FIELDVALUES.containing_type = _GETONLINEFEATURESRESPONSE
 _GETONLINEFEATURESRESPONSE.fields_by_name['field_values'].message_type = _GETONLINEFEATURESRESPONSE_FIELDVALUES
-_GETONLINEFEATURESRESPONSE_FIELDSTATUS.containing_type = _GETONLINEFEATURESRESPONSE
+_GETONLINEFEATURESRESPONSEV2_FIELDVECTOR.fields_by_name['values'].message_type = feast_dot_types_dot_Value__pb2._VALUE
+_GETONLINEFEATURESRESPONSEV2_FIELDVECTOR.fields_by_name['statuses'].enum_type = _FIELDSTATUS
+_GETONLINEFEATURESRESPONSEV2_FIELDVECTOR.containing_type = _GETONLINEFEATURESRESPONSEV2
+_GETONLINEFEATURESRESPONSEV2.fields_by_name['metadata'].message_type = _GETONLINEFEATURESRESPONSEMETADATA
+_GETONLINEFEATURESRESPONSEV2.fields_by_name['results'].message_type = _GETONLINEFEATURESRESPONSEV2_FIELDVECTOR
+_GETONLINEFEATURESRESPONSEMETADATA.fields_by_name['field_names'].message_type = _FIELDLIST
 DESCRIPTOR.message_types_by_name['GetFeastServingInfoRequest'] = _GETFEASTSERVINGINFOREQUEST
 DESCRIPTOR.message_types_by_name['GetFeastServingInfoResponse'] = _GETFEASTSERVINGINFORESPONSE
 DESCRIPTOR.message_types_by_name['FeatureReferenceV2'] = _FEATUREREFERENCEV2
 DESCRIPTOR.message_types_by_name['GetOnlineFeaturesRequestV2'] = _GETONLINEFEATURESREQUESTV2
 DESCRIPTOR.message_types_by_name['GetOnlineFeaturesResponse'] = _GETONLINEFEATURESRESPONSE
+DESCRIPTOR.message_types_by_name['GetOnlineFeaturesResponseV2'] = _GETONLINEFEATURESRESPONSEV2
+DESCRIPTOR.message_types_by_name['GetOnlineFeaturesResponseMetadata'] = _GETONLINEFEATURESRESPONSEMETADATA
+DESCRIPTOR.message_types_by_name['FieldList'] = _FIELDLIST
+DESCRIPTOR.enum_types_by_name['FieldStatus'] = _FIELDSTATUS
 DESCRIPTOR.enum_types_by_name['FeastServingType'] = _FEASTSERVINGTYPE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 GetFeastServingInfoRequest = _reflection.GeneratedProtocolMessageType('GetFeastServingInfoRequest', (_message.Message,), {
   'DESCRIPTOR' : _GETFEASTSERVINGINFOREQUEST,
   '__module__' : 'feast.serving.ServingService_pb2'
   # @@protoc_insertion_point(class_scope:feast.serving.GetFeastServingInfoRequest)
@@ -578,29 +739,58 @@
   # @@protoc_insertion_point(class_scope:feast.serving.GetOnlineFeaturesResponse)
   })
 _sym_db.RegisterMessage(GetOnlineFeaturesResponse)
 _sym_db.RegisterMessage(GetOnlineFeaturesResponse.FieldValues)
 _sym_db.RegisterMessage(GetOnlineFeaturesResponse.FieldValues.FieldsEntry)
 _sym_db.RegisterMessage(GetOnlineFeaturesResponse.FieldValues.StatusesEntry)
 
+GetOnlineFeaturesResponseV2 = _reflection.GeneratedProtocolMessageType('GetOnlineFeaturesResponseV2', (_message.Message,), {
+
+  'FieldVector' : _reflection.GeneratedProtocolMessageType('FieldVector', (_message.Message,), {
+    'DESCRIPTOR' : _GETONLINEFEATURESRESPONSEV2_FIELDVECTOR,
+    '__module__' : 'feast.serving.ServingService_pb2'
+    # @@protoc_insertion_point(class_scope:feast.serving.GetOnlineFeaturesResponseV2.FieldVector)
+    })
+  ,
+  'DESCRIPTOR' : _GETONLINEFEATURESRESPONSEV2,
+  '__module__' : 'feast.serving.ServingService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.serving.GetOnlineFeaturesResponseV2)
+  })
+_sym_db.RegisterMessage(GetOnlineFeaturesResponseV2)
+_sym_db.RegisterMessage(GetOnlineFeaturesResponseV2.FieldVector)
+
+GetOnlineFeaturesResponseMetadata = _reflection.GeneratedProtocolMessageType('GetOnlineFeaturesResponseMetadata', (_message.Message,), {
+  'DESCRIPTOR' : _GETONLINEFEATURESRESPONSEMETADATA,
+  '__module__' : 'feast.serving.ServingService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.serving.GetOnlineFeaturesResponseMetadata)
+  })
+_sym_db.RegisterMessage(GetOnlineFeaturesResponseMetadata)
+
+FieldList = _reflection.GeneratedProtocolMessageType('FieldList', (_message.Message,), {
+  'DESCRIPTOR' : _FIELDLIST,
+  '__module__' : 'feast.serving.ServingService_pb2'
+  # @@protoc_insertion_point(class_scope:feast.serving.FieldList)
+  })
+_sym_db.RegisterMessage(FieldList)
+
 
 DESCRIPTOR._options = None
 _GETONLINEFEATURESREQUESTV2_ENTITYROW_FIELDSENTRY._options = None
 _GETONLINEFEATURESRESPONSE_FIELDVALUES_FIELDSENTRY._options = None
 _GETONLINEFEATURESRESPONSE_FIELDVALUES_STATUSESENTRY._options = None
 
 _SERVINGSERVICE = _descriptor.ServiceDescriptor(
   name='ServingService',
   full_name='feast.serving.ServingService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=1423,
-  serialized_end=1657,
+  serialized_start=1800,
+  serialized_end=2142,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetFeastServingInfo',
     full_name='feast.serving.ServingService.GetFeastServingInfo',
     index=0,
     containing_service=None,
     input_type=_GETFEASTSERVINGINFOREQUEST,
@@ -614,13 +804,23 @@
     index=1,
     containing_service=None,
     input_type=_GETONLINEFEATURESREQUESTV2,
     output_type=_GETONLINEFEATURESRESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='GetOnlineFeatures',
+    full_name='feast.serving.ServingService.GetOnlineFeatures',
+    index=2,
+    containing_service=None,
+    input_type=_GETONLINEFEATURESREQUESTV2,
+    output_type=_GETONLINEFEATURESRESPONSEV2,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_SERVINGSERVICE)
 
 DESCRIPTOR.services_by_name['ServingService'] = _SERVINGSERVICE
 
 # @@protoc_insertion_point(module_scope)
```

### Comparing `feast-0.9.8/feast/serving/ServingService_pb2_grpc.py` & `feast-0.9.9/feast/serving/ServingService_pb2_grpc.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,19 @@
                 response_deserializer=feast_dot_serving_dot_ServingService__pb2.GetFeastServingInfoResponse.FromString,
                 )
         self.GetOnlineFeaturesV2 = channel.unary_unary(
                 '/feast.serving.ServingService/GetOnlineFeaturesV2',
                 request_serializer=feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesRequestV2.SerializeToString,
                 response_deserializer=feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesResponse.FromString,
                 )
+        self.GetOnlineFeatures = channel.unary_unary(
+                '/feast.serving.ServingService/GetOnlineFeatures',
+                request_serializer=feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesRequestV2.SerializeToString,
+                response_deserializer=feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesResponseV2.FromString,
+                )
 
 
 class ServingServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetFeastServingInfo(self, request, context):
         """Get information about this Feast serving.
@@ -39,27 +44,39 @@
     def GetOnlineFeaturesV2(self, request, context):
         """Get online features (v2) synchronously.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetOnlineFeatures(self, request, context):
+        """Get online features using optimized response message.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_ServingServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetFeastServingInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.GetFeastServingInfo,
                     request_deserializer=feast_dot_serving_dot_ServingService__pb2.GetFeastServingInfoRequest.FromString,
                     response_serializer=feast_dot_serving_dot_ServingService__pb2.GetFeastServingInfoResponse.SerializeToString,
             ),
             'GetOnlineFeaturesV2': grpc.unary_unary_rpc_method_handler(
                     servicer.GetOnlineFeaturesV2,
                     request_deserializer=feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesRequestV2.FromString,
                     response_serializer=feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesResponse.SerializeToString,
             ),
+            'GetOnlineFeatures': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetOnlineFeatures,
+                    request_deserializer=feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesRequestV2.FromString,
+                    response_serializer=feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesResponseV2.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'feast.serving.ServingService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -95,7 +112,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/feast.serving.ServingService/GetOnlineFeaturesV2',
             feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesRequestV2.SerializeToString,
             feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetOnlineFeatures(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/feast.serving.ServingService/GetOnlineFeatures',
+            feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesRequestV2.SerializeToString,
+            feast_dot_serving_dot_ServingService__pb2.GetOnlineFeaturesResponseV2.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `feast-0.9.8/feast/staging/entities.py` & `feast-0.9.9/feast/staging/entities.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/staging/storage_client.py` & `feast-0.9.9/feast/staging/storage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 S3 = "s3"
 S3A = "s3a"
 AZURE_SCHEME = "wasbs"
 LOCAL_FILE = "file"
 
 
 def _hash_fileobj(fileobj: IO[bytes]) -> str:
-    """ Compute sha256 hash of a file. File pointer will be reset to 0 on return. """
+    """Compute sha256 hash of a file. File pointer will be reset to 0 on return."""
     fileobj.seek(0)
     h = hashlib.sha256()
     for block in iter(lambda: fileobj.read(2 ** 20), b""):
         h.update(block)
     fileobj.seek(0)
     return h.hexdigest()
 
@@ -208,15 +208,15 @@
         blob = gs_bucket.blob(key)
         blob.upload_from_file(fileobj)
         return remote_uri
 
 
 class S3Client(AbstractStagingClient):
     """
-       Implementation of AbstractStagingClient for Aws S3 storage
+    Implementation of AbstractStagingClient for Aws S3 storage
     """
 
     def __init__(self, endpoint_url: str = None, url_scheme="s3"):
         try:
             import boto3
         except ImportError:
             raise ImportError(
@@ -311,15 +311,15 @@
                 fileobj, bucket, key, ExtraArgs={"Metadata": {"sha256sum": sha256sum}},
             )
             return remote_uri
 
 
 class AzureBlobClient(AbstractStagingClient):
     """
-       Implementation of AbstractStagingClient for Azure Blob storage
+    Implementation of AbstractStagingClient for Azure Blob storage
     """
 
     def __init__(self, account_name: str, account_access_key: str):
         try:
             from azure.storage.blob import BlobServiceClient
         except ImportError:
             raise ImportError(
@@ -399,16 +399,16 @@
         container_client = self.blob_service_client.get_container_client(bucket)
         container_client.upload_blob(name=key, data=fileobj, overwrite=True)
         return remote_uri
 
 
 class LocalFSClient(AbstractStagingClient):
     """
-       Implementation of AbstractStagingClient for local file
-       Note: The is used for E2E tests.
+    Implementation of AbstractStagingClient for local file
+    Note: The is used for E2E tests.
     """
 
     def __init__(self):
         pass
 
     def download_file(self, uri: ParseResult) -> IO[bytes]:
         """
```

### Comparing `feast-0.9.8/feast/storage/Redis_pb2.py` & `feast-0.9.9/feast/storage/Redis_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/telemetry.py` & `feast-0.9.9/feast/telemetry.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/third_party/grpc/health/v1/HealthService_pb2.py` & `feast-0.9.9/feast/third_party/grpc/health/v1/HealthService_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/third_party/grpc/health/v1/HealthService_pb2_grpc.py` & `feast-0.9.9/feast/third_party/grpc/health/v1/HealthService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/type_map.py` & `feast-0.9.9/feast/type_map.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/types/Field_pb2.py` & `feast-0.9.9/feast/types/Field_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/types/Value_pb2.py` & `feast-0.9.9/feast/types/Value_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/value_type.py` & `feast-0.9.9/feast/value_type.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast/wait.py` & `feast-0.9.9/feast/wait.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/feast.egg-info/PKG-INFO` & `feast-0.9.9/feast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feast
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python SDK for Feast
 Home-page: https://github.com/feast-dev/feast
 Author: Feast
 License: Apache
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: feast Version: 0.9.8 Summary: Python SDK for Feast
+Metadata-Version: 2.1 Name: feast Version: 0.9.9 Summary: Python SDK for Feast
 Home-page: https://github.com/feast-dev/feast Author: Feast License: Apache
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown Provides-Extra: dev Provides-Extra:
 validation
                          [docs/assets/feast_logo.png]
```

### Comparing `feast-0.9.8/feast.egg-info/SOURCES.txt` & `feast-0.9.9/feast.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 feast/data_format.py
 feast/data_source.py
 feast/entity.py
 feast/feature.py
 feast/feature_table.py
 feast/job_service.py
 feast/online_response.py
+feast/online_store.py
 feast/remote_job.py
 feast/telemetry.py
 feast/type_map.py
 feast/value_type.py
 feast/wait.py
 feast.egg-info/PKG-INFO
 feast.egg-info/SOURCES.txt
@@ -74,14 +75,17 @@
 feast/core/FeatureTable_pb2_grpc.py
 feast/core/Feature_pb2.py
 feast/core/Feature_pb2.pyi
 feast/core/Feature_pb2_grpc.py
 feast/core/JobService_pb2.py
 feast/core/JobService_pb2.pyi
 feast/core/JobService_pb2_grpc.py
+feast/core/OnlineStore_pb2.py
+feast/core/OnlineStore_pb2.pyi
+feast/core/OnlineStore_pb2_grpc.py
 feast/core/Store_pb2.py
 feast/core/Store_pb2.pyi
 feast/core/Store_pb2_grpc.py
 feast/core/__init__.py
 feast/grpc/__init__.py
 feast/grpc/auth.py
 feast/grpc/grpc.py
```

### Comparing `feast-0.9.8/requirements-dev.txt` & `feast-0.9.9/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/setup.cfg` & `feast-0.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/setup.py` & `feast-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/telemetry_tests/test_telemetry.py` & `feast-0.9.9/telemetry_tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tensorflow_metadata/proto/v0/path_pb2.py` & `feast-0.9.9/tensorflow_metadata/proto/v0/path_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tensorflow_metadata/proto/v0/schema_pb2.py` & `feast-0.9.9/tensorflow_metadata/proto/v0/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tensorflow_metadata/proto/v0/statistics_pb2.py` & `feast-0.9.9/tensorflow_metadata/proto/v0/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/conftest.py` & `feast-0.9.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/data/austin_bikeshare.bikeshare_stations.avro` & `feast-0.9.9/tests/data/austin_bikeshare.bikeshare_stations.avro`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/data/dev_featuretable.csv` & `feast-0.9.9/tests/data/dev_featuretable.csv`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/data/localhost.crt` & `feast-0.9.9/tests/data/localhost.crt`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/data/localhost.key` & `feast-0.9.9/tests/data/localhost.key`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/data/localhost.pem` & `feast-0.9.9/tests/data/localhost.pem`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/data/tensorflow_metadata/bikeshare_feature_set.yaml` & `feast-0.9.9/tests/data/tensorflow_metadata/bikeshare_feature_set.yaml`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/data/tensorflow_metadata/bikeshare_schema.json` & `feast-0.9.9/tests/data/tensorflow_metadata/bikeshare_schema.json`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/dataframes.py` & `feast-0.9.9/tests/dataframes.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/feast_core_server.py` & `feast-0.9.9/tests/feast_core_server.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/feast_serving_server.py` & `feast-0.9.9/tests/feast_serving_server.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/grpc/test_auth.py` & `feast-0.9.9/tests/grpc/test_auth.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/loaders/test_file.py` & `feast-0.9.9/tests/loaders/test_file.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/test_as_of_join.py` & `feast-0.9.9/tests/test_as_of_join.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/test_client.py` & `feast-0.9.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/test_config.py` & `feast-0.9.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/test_entity.py` & `feast-0.9.9/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/test_feature_table.py` & `feast-0.9.9/tests/test_feature_table.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/test_historical_feature_retrieval.py` & `feast-0.9.9/tests/test_historical_feature_retrieval.py`

 * *Files identical despite different names*

### Comparing `feast-0.9.8/tests/test_remote_job.py` & `feast-0.9.9/tests/test_remote_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             yield JobServiceStub(channel)
     finally:
         server.stop(None)
 
 
 class TestRemoteJob:
     def test_remote_ingestion_job(self):
-        """ Test wating for the remote ingestion job to complete """
+        """Test wating for the remote ingestion job to complete"""
 
         class MockServicer(JobServiceServicer):
             """
             The RemoteJob is expected to call GetJob until its done.
             This mock JobService returns RUNNING status on the first call, and DONE on the second.
             """
```

### Comparing `feast-0.9.8/tests/test_streaming_control_loop.py` & `feast-0.9.9/tests/test_streaming_control_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         # Register Feature Table with Core
         client.apply(ft1)
 
     def _delete_ft(self, client: Client):
         client.delete_feature_table(self.table_name)
 
     def test_streaming_job_control_loop(self) -> None:
-        """ Test streaming job control loop logic. """
+        """Test streaming job control loop logic."""
 
         reset_job_cache()
 
         core_servicer = MockCoreServicer()
 
         processes: List[subprocess.Popen] = []
```

