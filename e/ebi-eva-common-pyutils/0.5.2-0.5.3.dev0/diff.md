# Comparing `tmp/ebi_eva_common_pyutils-0.5.2.tar.gz` & `tmp/ebi_eva_common_pyutils-0.5.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebi_eva_common_pyutils-0.5.2.tar", last modified: Fri Mar  3 13:20:54 2023, max compression
+gzip compressed data, was "ebi_eva_common_pyutils-0.5.3.dev0.tar", last modified: Fri Apr 21 14:24:20 2023, max compression
```

## Comparing `ebi_eva_common_pyutils-0.5.2.tar` & `ebi_eva_common_pyutils-0.5.3.dev0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.320646 ebi_eva_common_pyutils-0.5.2/
--rw-r--r--   0 tcezard    (502) staff       (20)     1492 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/CHANGELOG.md
--rw-r--r--   0 tcezard    (502) staff       (20)    11357 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/LICENSE
--rw-r--r--   0 tcezard    (502) staff       (20)       28 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/MANIFEST.in
--rw-r--r--   0 tcezard    (502) staff       (20)      540 2023-03-03 13:20:54.320762 ebi_eva_common_pyutils-0.5.2/PKG-INFO
--rw-r--r--   0 tcezard    (502) staff       (20)     1434 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/README.md
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.313119 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4984 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/archive_directory.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.315516 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/assembly/
--rw-r--r--   0 tcezard    (502) staff       (20)       66 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/assembly/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)      673 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/assembly/assembly.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2151 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/command_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     1192 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/common_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2242 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/config.py
--rw-r--r--   0 tcezard    (502) staff       (20)     7838 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/config_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.316160 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/contig_alias/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/contig_alias/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3056 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/contig_alias/contig_alias.py
--rw-r--r--   0 tcezard    (502) staff       (20)     1452 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/ena_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     1375 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/file_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4990 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/logger.py
--rw-r--r--   0 tcezard    (502) staff       (20)    13489 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/metadata_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3589 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/mongo_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.316806 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/mongodb/
--rw-r--r--   0 tcezard    (502) staff       (20)       72 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/mongodb/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     9676 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/mongodb/mongo_database.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4009 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/ncbi_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2285 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/network_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.317687 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/nextflow/
--rw-r--r--   0 tcezard    (502) staff       (20)      120 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/nextflow/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)    10114 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
--rw-r--r--   0 tcezard    (502) staff       (20)     4398 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/pg_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.318788 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/reference/
--rw-r--r--   0 tcezard    (502) staff       (20)      134 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/reference/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)    12162 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/reference/assembly.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3911 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/reference/sequence.py
--rw-r--r--   0 tcezard    (502) staff       (20)     9540 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/spring_properties.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.319429 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/taxonomy/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/taxonomy/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     2259 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/taxonomy/taxonomy.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.320335 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/variation/
--rw-r--r--   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/variation/__init__.py
--rw-r--r--   0 tcezard    (502) staff       (20)     3515 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/variation/assembly_utils.py
--rw-r--r--   0 tcezard    (502) staff       (20)     5230 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/variation/contig_utils.py
-drwxr-xr-x   0 tcezard    (502) staff       (20)        0 2023-03-03 13:20:54.314776 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils.egg-info/
--rw-r--r--   0 tcezard    (502) staff       (20)      540 2023-03-03 13:20:54.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 tcezard    (502) staff       (20)     1606 2023-03-03 13:20:54.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 tcezard    (502) staff       (20)        1 2023-03-03 13:20:54.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 tcezard    (502) staff       (20)       81 2023-03-03 13:20:54.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils.egg-info/requires.txt
--rw-r--r--   0 tcezard    (502) staff       (20)       23 2023-03-03 13:20:54.000000 ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils.egg-info/top_level.txt
--rw-r--r--   0 tcezard    (502) staff       (20)      225 2023-03-03 13:20:54.321230 ebi_eva_common_pyutils-0.5.2/setup.cfg
--rw-r--r--   0 tcezard    (502) staff       (20)      907 2023-03-03 13:20:53.000000 ebi_eva_common_pyutils-0.5.2/setup.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1492 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/CHANGELOG.md
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    11357 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/LICENSE
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       28 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/MANIFEST.in
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/PKG-INFO
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1434 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/README.md
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4984 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/archive_directory.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/assembly/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       66 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/assembly/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      673 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/assembly/assembly.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2151 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/command_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1192 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/common_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2242 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/config.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     8342 2023-04-21 07:36:06.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/config_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/contig_alias/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/contig_alias/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3056 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/contig_alias/contig_alias.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1452 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/ena_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1375 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/file_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4990 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/logger.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    13489 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/metadata_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3589 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/mongo_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/mongodb/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       72 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/mongodb/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     9676 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/mongodb/mongo_database.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4965 2023-04-21 08:17:45.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/ncbi_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2285 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/network_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/nextflow/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      120 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/nextflow/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    10114 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     4398 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/pg_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/reference/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      134 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/reference/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    12162 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/reference/assembly.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3911 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/reference/sequence.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)    13161 2023-04-21 12:50:30.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/spring_properties.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/taxonomy/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/taxonomy/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     2259 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/taxonomy/taxonomy.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/variation/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        0 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/variation/__init__.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     3515 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/variation/assembly_utils.py
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     5230 2023-04-17 14:40:08.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/variation/contig_utils.py
+drwxr-xr-x   0 nkumar2   (9636) eva       (1254)        0 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils.egg-info/
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      517 2023-04-21 14:24:20.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)     1699 2023-04-21 14:24:20.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)        1 2023-04-21 14:24:20.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       81 2023-04-21 14:24:20.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils.egg-info/requires.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)       23 2023-04-21 14:24:20.000000 ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      225 2023-04-21 14:24:20.925983 ebi_eva_common_pyutils-0.5.3.dev0/setup.cfg
+-rw-r--r--   0 nkumar2   (9636) eva       (1254)      911 2023-04-21 13:27:10.000000 ebi_eva_common_pyutils-0.5.3.dev0/setup.py
```

### Comparing `ebi_eva_common_pyutils-0.5.2/CHANGELOG.md` & `ebi_eva_common_pyutils-0.5.3.dev0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/LICENSE` & `ebi_eva_common_pyutils-0.5.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/PKG-INFO` & `ebi_eva_common_pyutils-0.5.3.dev0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 Metadata-Version: 2.1
 Name: ebi_eva_common_pyutils
-Version: 0.5.2
+Version: 0.5.3.dev0
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `ebi_eva_common_pyutils-0.5.2/README.md` & `ebi_eva_common_pyutils-0.5.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/archive_directory.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/archive_directory.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/assembly/assembly.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/assembly/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/command_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/common_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/common_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/config.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/config.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/config_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/config_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,26 @@
     properties = get_properties_from_xml_file(profile_name, settings_xml_file)
     pg_url = properties['eva.accession.jdbc.url']
     pg_user = properties['eva.accession.user']
     pg_pass = properties['eva.accession.password']
     return pg_url, pg_user, pg_pass
 
 
+def get_variant_pg_creds_for_profile(profile_name: str, settings_xml_file: str):
+    """
+    Gets host, username, and password for variant load job tracker database.
+    Useful for filling properties files.
+    """
+    properties = get_properties_from_xml_file(profile_name, settings_xml_file)
+    variant_url = properties['eva.variant.jdbc.url']
+    variant_user = properties['eva.variant.user']
+    variant_pass = properties['eva.variant.password']
+    return variant_url, variant_user, variant_pass
+
+
 def get_contig_alias_db_creds_for_profile(profile_name: str, settings_xml_file: str):
     """
     Gets url, username, and password for contig alias database.
 
     """
     properties = get_properties_from_xml_file(profile_name, settings_xml_file)
     contig_alias_url = properties['contig-alias.url']
```

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/contig_alias/contig_alias.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/contig_alias/contig_alias.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/ena_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/ena_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/file_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/logger.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/logger.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/metadata_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/mongo_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/mongo_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/mongodb/mongo_database.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/mongodb/mongo_database.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/ncbi_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/ncbi_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -90,7 +90,27 @@
     if match:
         rank = match.group(1)
     if rank not in ['species', 'subspecies']:
         logger.warning('Taxonomy id %s does not point to a species', taxid)
     match = re.search('<ScientificName>(.+?)</ScientificName>', r.text, re.MULTILINE)
     if match:
         return match.group(1)
+
+
+def get_species_name_from_ncbi(assembly_acc):
+    # We first need to search for the species associated with the assembly
+    assembly_dicts = get_ncbi_assembly_dicts_from_term(assembly_acc)
+    taxid_and_assembly_name = set([
+        (assembly_dict.get('taxid'), assembly_dict.get('assemblyname'))
+        for assembly_dict in assembly_dicts
+        if assembly_dict.get('assemblyaccession') == assembly_acc or
+           assembly_dict.get('synonym', {}).get('genbank') == assembly_acc
+    ])
+    # This is a search so could retrieve multiple results
+    if len(taxid_and_assembly_name) != 1:
+        raise ValueError(f'Multiple assembly found for {assembly_acc}. '
+                         f'Cannot resolve single assembly for assembly {assembly_acc} in NCBI.')
+
+    taxonomy_id, _ = taxid_and_assembly_name.pop()
+
+    scientific_name = retrieve_species_scientific_name_from_tax_id_ncbi(taxonomy_id)
+    return scientific_name.replace(' ', '_').lower()
```

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/network_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/network_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/nextflow/nextflow_pipeline.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/pg_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/pg_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/reference/assembly.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/reference/assembly.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/reference/sequence.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/reference/sequence.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/spring_properties.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/spring_properties.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from collections import defaultdict
 
 from ebi_eva_common_pyutils.config_utils import get_primary_mongo_creds_for_profile, get_accession_pg_creds_for_profile, \
-    get_count_service_creds_for_profile, get_properties_from_xml_file
+    get_count_service_creds_for_profile, get_properties_from_xml_file, get_variant_pg_creds_for_profile
 
 
 class SpringPropertiesGenerator:
     """
     Class to generate Spring properties for various Spring Batch pipelines.
     These methods can be used to generate complete properties files entirely in Python; alternatively, certain
     properties can be left unfilled and supplied as command-line arguments (e.g. by a NextFlow process).
@@ -72,14 +72,16 @@
             'spring.data.mongodb.username': mongo_user,
             'spring.data.mongodb.password': mongo_pass,
             'spring.data.mongodb.authentication-database': 'admin',
             'mongodb.read-preference': read_preference,
             'spring.main.web-application-type': 'none',
             'spring.main.allow-bean-definition-overriding': 'true',
             'spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation': 'true',
+            'spring.jpa.properties.hibernate.temp.use_jdbc_metadata_defaults': False,
+            'spring.jpa.database-platform': 'org.hibernate.dialect.PostgreSQL9Dialect',
             'parameters.chunkSize': chunk_size,
             'parameters.assemblyAccession': assembly_accession,
         }
 
     def _accessioning_properties(self, *, instance=''):
         """Properties common to accessioning and clustering pipelines."""
         counts_url, counts_username, counts_password = get_count_service_creds_for_profile(
@@ -118,14 +120,71 @@
                 'parameters.taxonomyAccession': taxonomy_accession,
                 'parameters.vcfAggregation': aggregation,
                 'parameters.vcf': vcf_file,
                 'parameters.outputVcf': output_vcf
             },
         )
 
+    def get_variant_load_properties(self,  project_accession, study_name, output_dir, annotation_dir, stats_dir,
+                                    read_preference='secondaryPreferred'):
+        mongo_host, mongo_user, mongo_pass = get_primary_mongo_creds_for_profile(
+            self.maven_profile, self.private_settings_file)
+        variant_url, variant_user, variant_pass = get_variant_pg_creds_for_profile(self.maven_profile, self.private_settings_file)
+        files_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.files']
+        variants_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.variants']
+        annotation_metadata_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotation-metadata']
+        annotation_collection = get_properties_from_xml_file(
+            self.maven_profile, self.private_settings_file)['eva.mongo.collections.annotations']
+
+        return self._format({
+            'spring.profiles.active': 'production,mongo',
+            'spring.profiles.include': 'variant-writer-mongo,variant-annotation-mongo',
+            'spring.data.mongodb.authentication-database': 'admin',
+            'spring.data.mongodb.host': mongo_host,
+            'spring.data.mongodb.password': mongo_pass,
+            'spring.data.mongodb.port': 27017,
+            'spring.data.mongodb.username': mongo_user,
+            'spring.data.mongodb.authentication-mechanism': 'SCRAM-SHA-1',
+            'job.repository.driverClassName': 'org.postgresql.Driver',
+            'job.repository.url': variant_url,
+            'job.repository.username': variant_user,
+            'job.repository.password': variant_pass,
+
+            'app.opencga.path': '/nfs/production/keane/eva/software/opencga/',
+            'app.vep.cache.path': '/nfs/production/keane/eva/datasources/vep-cache',
+            'annotation.overwrite': False,
+            'app.vep.num-forks': 4,
+            'app.vep.timeout': 500,
+            'config.chunk.size': 200,
+            'config.restartability.allow': 'false',
+            'config.db.read-preference': read_preference,
+            'db.collections.files.name': files_collection,
+            'db.collections.variants.name': variants_collection,
+            'db.collections.annotation-metadata.name': annotation_metadata_collection,
+            'db.collections.annotations.name': annotation_collection,
+            'input.study.id': project_accession,
+            'input.study.name': study_name,
+            'input.study.type': 'COLLECTION',
+            'logging.level.embl.ebi.variation.eva': 'DEBUG',
+            'logging.level.org.opencb.opencga': 'DEBUG',
+            'logging.level.org.springframework': 'INFO',
+            'output.dir': str(output_dir),
+            'output.dir.annotation': str(annotation_dir),
+            'output.dir.statistics': str(stats_dir),
+            'spring.main.allow-bean-definition-overriding': 'true',
+            'spring.jpa.database-platform': 'org.hibernate.dialect.PostgreSQL9Dialect',
+            'spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation': True,
+            'spring.jpa.properties.hibernate.temp.use_jdbc_metadata_defaults': False,
+            'statistics.skip': False
+        },
+    )
+
     def get_remapping_extraction_properties(self, *, taxonomy=None, source_assembly=None, fasta=None,
                                             assembly_report=None,
                                             projects='', output_folder=None):
         """Properties for remapping extraction pipeline."""
         return self._format(
             self._common_properties(assembly_accession=source_assembly, read_preference='secondaryPreferred',
                                     chunk_size=1000),
```

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/taxonomy/taxonomy.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/taxonomy/taxonomy.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/variation/assembly_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/variation/assembly_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils/variation/contig_utils.py` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils/variation/contig_utils.py`

 * *Files identical despite different names*

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils.egg-info/PKG-INFO` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 Metadata-Version: 2.1
 Name: ebi-eva-common-pyutils
-Version: 0.5.2
+Version: 0.5.3.dev0
 Summary: EBI EVA - Common Python Utilities
 Home-page: https://github.com/EBIVariation/eva-common-pyutils
 License: Apache
 Keywords: EBI,EVA,PYTHON,UTILITIES
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `ebi_eva_common_pyutils-0.5.2/ebi_eva_common_pyutils.egg-info/SOURCES.txt` & `ebi_eva_common_pyutils-0.5.3.dev0/ebi_eva_common_pyutils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+/home/nkumar2/PycharmProjects/eva-common-pyutils/ebi_eva_common_pyutils/archive_directory.py
 ebi_eva_common_pyutils/__init__.py
 ebi_eva_common_pyutils/archive_directory.py
 ebi_eva_common_pyutils/command_utils.py
 ebi_eva_common_pyutils/common_utils.py
 ebi_eva_common_pyutils/config.py
 ebi_eva_common_pyutils/config_utils.py
 ebi_eva_common_pyutils/ena_utils.py
```

### Comparing `ebi_eva_common_pyutils-0.5.2/setup.py` & `ebi_eva_common_pyutils-0.5.3.dev0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages
 
 setup(
     name='ebi_eva_common_pyutils',
     scripts=[os.path.join(os.path.dirname(__file__), 'ebi_eva_common_pyutils', 'archive_directory.py')],
     packages=find_packages(),
-    version='0.5.2',
+    version='0.5.3-dev',
     license='Apache',
     description='EBI EVA - Common Python Utilities',
     url='https://github.com/EBIVariation/eva-common-pyutils',
     keywords=['EBI', 'EVA', 'PYTHON', 'UTILITIES'],
     install_requires=['psycopg2-binary', 'requests', 'pymongo', 'lxml', 'pyyaml', 'cached-property', 'retry',
                       'networkx<=2.5'],
     classifiers=[
```

