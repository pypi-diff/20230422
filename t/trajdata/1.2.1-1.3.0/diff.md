# Comparing `tmp/trajdata-1.2.1.tar.gz` & `tmp/trajdata-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trajdata-1.2.1.tar", last modified: Sat Feb 11 07:59:57 2023, max compression
+gzip compressed data, was "trajdata-1.3.0.tar", last modified: Fri Apr 21 23:47:20 2023, max compression
```

## Comparing `trajdata-1.2.1.tar` & `trajdata-1.3.0.tar`

### file list

```diff
@@ -1,107 +1,111 @@
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.261929 trajdata-1.2.1/
--rw-r--r--   0 bivanovic (41443) dip         (30)    11357 2022-07-10 04:26:11.000000 trajdata-1.2.1/LICENSE
--rw-r--r--   0 bivanovic (41443) dip         (30)    11300 2023-02-11 07:59:57.261929 trajdata-1.2.1/PKG-INFO
--rw-r--r--   0 bivanovic (41443) dip         (30)    10696 2022-11-18 02:24:41.000000 trajdata-1.2.1/README.md
--rw-r--r--   0 bivanovic (41443) dip         (30)      135 2022-07-10 04:26:11.000000 trajdata-1.2.1/pyproject.toml
--rw-r--r--   0 bivanovic (41443) dip         (30)      972 2023-02-11 07:59:57.261929 trajdata-1.2.1/setup.cfg
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.253929 trajdata-1.2.1/src/
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.253929 trajdata-1.2.1/src/trajdata/
--rw-r--r--   0 bivanovic (41443) dip         (30)      135 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/__init__.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.253929 trajdata-1.2.1/src/trajdata/augmentation/
--rw-r--r--   0 bivanovic (41443) dip         (30)      181 2022-11-12 07:40:30.000000 trajdata-1.2.1/src/trajdata/augmentation/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      548 2022-07-30 07:42:53.000000 trajdata-1.2.1/src/trajdata/augmentation/augmentation.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1786 2022-07-10 04:26:11.000000 trajdata-1.2.1/src/trajdata/augmentation/low_vel_yaw_correction.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1785 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/augmentation/noise_histories.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/caching/
--rw-r--r--   0 bivanovic (41443) dip         (30)       68 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/caching/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    35781 2023-02-11 07:43:40.000000 trajdata-1.2.1/src/trajdata/caching/df_cache.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     2311 2022-11-12 07:57:45.000000 trajdata-1.2.1/src/trajdata/caching/env_cache.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     6507 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/caching/scene_cache.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/data_structures/
--rw-r--r--   0 bivanovic (41443) dip         (30)      551 2023-02-01 00:28:01.000000 trajdata-1.2.1/src/trajdata/data_structures/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1944 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/data_structures/agent.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    13883 2023-02-11 07:41:45.000000 trajdata-1.2.1/src/trajdata/data_structures/batch.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    22625 2023-02-11 07:41:45.000000 trajdata-1.2.1/src/trajdata/data_structures/batch_element.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    36157 2023-02-11 07:41:45.000000 trajdata-1.2.1/src/trajdata/data_structures/collation.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3965 2022-07-20 07:32:10.000000 trajdata-1.2.1/src/trajdata/data_structures/data_index.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      841 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/data_structures/environment.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3570 2023-02-01 00:28:01.000000 trajdata-1.2.1/src/trajdata/data_structures/scene.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1865 2022-11-12 08:00:43.000000 trajdata-1.2.1/src/trajdata/data_structures/scene_metadata.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      411 2022-07-10 04:26:11.000000 trajdata-1.2.1/src/trajdata/data_structures/scene_tag.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    15444 2023-02-11 07:41:45.000000 trajdata-1.2.1/src/trajdata/data_structures/state.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    41820 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/dataset.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/dataset_specific/
--rw-r--r--   0 bivanovic (41443) dip         (30)      110 2022-11-12 07:42:49.000000 trajdata-1.2.1/src/trajdata/dataset_specific/__init__.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/dataset_specific/eth_ucy_peds/
--rw-r--r--   0 bivanovic (41443) dip         (30)       42 2022-07-10 04:26:11.000000 trajdata-1.2.1/src/trajdata/dataset_specific/eth_ucy_peds/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    12036 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/dataset_specific/eth_ucy_peds/eupeds_dataset.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/dataset_specific/lyft/
--rw-r--r--   0 bivanovic (41443) dip         (30)       38 2022-07-10 04:26:11.000000 trajdata-1.2.1/src/trajdata/dataset_specific/lyft/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    12667 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/dataset_specific/lyft/lyft_dataset.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     6613 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/dataset_specific/lyft/lyft_utils.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/dataset_specific/nuplan/
--rw-r--r--   0 bivanovic (41443) dip         (30)       42 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/dataset_specific/nuplan/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    15566 2023-02-01 00:28:01.000000 trajdata-1.2.1/src/trajdata/dataset_specific/nuplan/nuplan_dataset.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    14656 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/dataset_specific/nuplan/nuplan_utils.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/dataset_specific/nusc/
--rw-r--r--   0 bivanovic (41443) dip         (30)       38 2022-07-10 04:26:11.000000 trajdata-1.2.1/src/trajdata/dataset_specific/nusc/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    12101 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/dataset_specific/nusc/nusc_dataset.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    19061 2023-02-11 07:41:45.000000 trajdata-1.2.1/src/trajdata/dataset_specific/nusc/nusc_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3310 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/dataset_specific/raw_dataset.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      483 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/dataset_specific/scene_records.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/filtering/
--rw-r--r--   0 bivanovic (41443) dip         (30)       23 2022-11-12 07:42:55.000000 trajdata-1.2.1/src/trajdata/filtering/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3659 2023-02-11 07:41:45.000000 trajdata-1.2.1/src/trajdata/filtering/filters.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/maps/
--rw-r--r--   0 bivanovic (41443) dip         (30)      193 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/maps/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      111 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/maps/lane_route.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1483 2023-01-05 00:00:22.000000 trajdata-1.2.1/src/trajdata/maps/map_api.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     6663 2023-02-11 07:46:27.000000 trajdata-1.2.1/src/trajdata/maps/map_kdtree.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     2116 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/maps/raster_map.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      121 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/maps/traffic_light_status.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    21905 2023-02-10 07:47:20.000000 trajdata-1.2.1/src/trajdata/maps/vec_map.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     5194 2023-01-05 00:04:06.000000 trajdata-1.2.1/src/trajdata/maps/vec_map_elements.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/parallel/
--rw-r--r--   0 bivanovic (41443) dip         (30)       83 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/parallel/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3423 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/parallel/data_preprocessor.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/proto/
--rw-r--r--   0 bivanovic (41443) dip         (30)        0 2022-10-24 06:19:35.000000 trajdata-1.2.1/src/trajdata/proto/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     5969 2023-02-11 07:47:31.000000 trajdata-1.2.1/src/trajdata/proto/vectorized_map_pb2.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.257929 trajdata-1.2.1/src/trajdata/simulation/
--rw-r--r--   0 bivanovic (41443) dip         (30)       39 2022-11-12 06:09:23.000000 trajdata-1.2.1/src/trajdata/simulation/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1056 2023-02-11 07:41:45.000000 trajdata-1.2.1/src/trajdata/simulation/sim_cache.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    10217 2023-02-11 07:41:45.000000 trajdata-1.2.1/src/trajdata/simulation/sim_df_cache.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1077 2022-07-10 04:26:11.000000 trajdata-1.2.1/src/trajdata/simulation/sim_metrics.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     8635 2023-02-11 07:59:18.000000 trajdata-1.2.1/src/trajdata/simulation/sim_scene.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3872 2022-10-24 06:19:35.000000 trajdata-1.2.1/src/trajdata/simulation/sim_stats.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      786 2022-07-10 04:26:11.000000 trajdata-1.2.1/src/trajdata/simulation/sim_vis.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.261929 trajdata-1.2.1/src/trajdata/utils/
--rw-r--r--   0 bivanovic (41443) dip         (30)        0 2022-07-10 04:26:11.000000 trajdata-1.2.1/src/trajdata/utils/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     2724 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/utils/agent_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    10322 2023-02-11 07:46:27.000000 trajdata-1.2.1/src/trajdata/utils/arr_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3736 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/utils/batch_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3204 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/utils/df_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1686 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/utils/env_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    10596 2023-02-11 07:47:31.000000 trajdata-1.2.1/src/trajdata/utils/map_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     1843 2022-11-18 01:28:43.000000 trajdata-1.2.1/src/trajdata/utils/parallel_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     8175 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/utils/raster_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     3520 2022-11-12 08:23:30.000000 trajdata-1.2.1/src/trajdata/utils/scene_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     5688 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/utils/state_utils.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      186 2022-07-10 04:26:11.000000 trajdata-1.2.1/src/trajdata/utils/string_utils.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.261929 trajdata-1.2.1/src/trajdata/visualization/
--rw-r--r--   0 bivanovic (41443) dip         (30)       52 2023-02-11 07:46:27.000000 trajdata-1.2.1/src/trajdata/visualization/__init__.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    13225 2023-02-04 18:48:20.000000 trajdata-1.2.1/src/trajdata/visualization/vis.py
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.253929 trajdata-1.2.1/src/trajdata.egg-info/
--rw-r--r--   0 bivanovic (41443) dip         (30)    11300 2023-02-11 07:59:57.000000 trajdata-1.2.1/src/trajdata.egg-info/PKG-INFO
--rw-r--r--   0 bivanovic (41443) dip         (30)     3141 2023-02-11 07:59:57.000000 trajdata-1.2.1/src/trajdata.egg-info/SOURCES.txt
--rw-r--r--   0 bivanovic (41443) dip         (30)        1 2023-02-11 07:59:57.000000 trajdata-1.2.1/src/trajdata.egg-info/dependency_links.txt
--rw-r--r--   0 bivanovic (41443) dip         (30)      255 2023-02-11 07:59:57.000000 trajdata-1.2.1/src/trajdata.egg-info/requires.txt
--rw-r--r--   0 bivanovic (41443) dip         (30)        9 2023-02-11 07:59:57.000000 trajdata-1.2.1/src/trajdata.egg-info/top_level.txt
-drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-02-11 07:59:57.261929 trajdata-1.2.1/tests/
--rw-r--r--   0 bivanovic (41443) dip         (30)     8075 2023-02-04 18:48:20.000000 trajdata-1.2.1/tests/test_batch_conversion.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     7443 2023-02-11 07:41:45.000000 trajdata-1.2.1/tests/test_collation.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     7569 2023-02-11 07:41:45.000000 trajdata-1.2.1/tests/test_datasizes.py
--rw-r--r--   0 bivanovic (41443) dip         (30)      992 2022-11-17 10:42:27.000000 trajdata-1.2.1/tests/test_description_matching.py
--rw-r--r--   0 bivanovic (41443) dip         (30)    13585 2023-02-11 07:41:45.000000 trajdata-1.2.1/tests/test_state.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     6304 2023-02-04 18:48:52.000000 trajdata-1.2.1/tests/test_traffic_data.py
--rw-r--r--   0 bivanovic (41443) dip         (30)     2068 2023-01-05 00:04:06.000000 trajdata-1.2.1/tests/test_vec_map.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.219476 trajdata-1.3.0/
+-rw-r--r--   0 bivanovic (41443) dip         (30)    11357 2022-07-10 04:26:11.000000 trajdata-1.3.0/LICENSE
+-rw-r--r--   0 bivanovic (41443) dip         (30)    11300 2023-04-21 23:47:20.219476 trajdata-1.3.0/PKG-INFO
+-rw-r--r--   0 bivanovic (41443) dip         (30)    10696 2022-11-18 02:24:41.000000 trajdata-1.3.0/README.md
+-rw-r--r--   0 bivanovic (41443) dip         (30)      135 2022-07-10 04:26:11.000000 trajdata-1.3.0/pyproject.toml
+-rw-r--r--   0 bivanovic (41443) dip         (30)      986 2023-04-21 23:47:20.219476 trajdata-1.3.0/setup.cfg
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.211476 trajdata-1.3.0/src/
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.211476 trajdata-1.3.0/src/trajdata/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      135 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/__init__.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/augmentation/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      181 2022-11-12 07:40:30.000000 trajdata-1.3.0/src/trajdata/augmentation/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      548 2022-07-30 07:42:53.000000 trajdata-1.3.0/src/trajdata/augmentation/augmentation.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1786 2022-07-10 04:26:11.000000 trajdata-1.3.0/src/trajdata/augmentation/low_vel_yaw_correction.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1785 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/augmentation/noise_histories.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/caching/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       68 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/caching/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    35781 2023-02-11 07:43:40.000000 trajdata-1.3.0/src/trajdata/caching/df_cache.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     2311 2022-11-12 07:57:45.000000 trajdata-1.3.0/src/trajdata/caching/env_cache.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     6507 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/caching/scene_cache.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/data_structures/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      551 2023-02-01 00:28:01.000000 trajdata-1.3.0/src/trajdata/data_structures/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1944 2023-02-15 17:46:18.000000 trajdata-1.3.0/src/trajdata/data_structures/agent.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    13883 2023-02-11 07:41:45.000000 trajdata-1.3.0/src/trajdata/data_structures/batch.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    22665 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/data_structures/batch_element.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    36157 2023-02-11 07:41:45.000000 trajdata-1.3.0/src/trajdata/data_structures/collation.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3965 2022-07-20 07:32:10.000000 trajdata-1.3.0/src/trajdata/data_structures/data_index.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      841 2023-02-15 17:47:17.000000 trajdata-1.3.0/src/trajdata/data_structures/environment.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3570 2023-02-01 00:28:01.000000 trajdata-1.3.0/src/trajdata/data_structures/scene.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1865 2023-02-15 17:46:08.000000 trajdata-1.3.0/src/trajdata/data_structures/scene_metadata.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      411 2022-07-10 04:26:11.000000 trajdata-1.3.0/src/trajdata/data_structures/scene_tag.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    15442 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/data_structures/state.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    41820 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/dataset.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/dataset_specific/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      110 2022-11-12 07:42:49.000000 trajdata-1.3.0/src/trajdata/dataset_specific/__init__.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/dataset_specific/eth_ucy_peds/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       42 2022-07-10 04:26:11.000000 trajdata-1.3.0/src/trajdata/dataset_specific/eth_ucy_peds/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12036 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/dataset_specific/eth_ucy_peds/eupeds_dataset.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/dataset_specific/lyft/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       38 2022-07-10 04:26:11.000000 trajdata-1.3.0/src/trajdata/dataset_specific/lyft/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12667 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/dataset_specific/lyft/lyft_dataset.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     6613 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/dataset_specific/lyft/lyft_utils.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/dataset_specific/nuplan/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       42 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/dataset_specific/nuplan/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    15566 2023-02-15 17:41:49.000000 trajdata-1.3.0/src/trajdata/dataset_specific/nuplan/nuplan_dataset.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    14656 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/dataset_specific/nuplan/nuplan_utils.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/dataset_specific/nusc/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       38 2022-07-10 04:26:11.000000 trajdata-1.3.0/src/trajdata/dataset_specific/nusc/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    12101 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/dataset_specific/nusc/nusc_dataset.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    19061 2023-02-11 07:41:45.000000 trajdata-1.3.0/src/trajdata/dataset_specific/nusc/nusc_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3310 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/dataset_specific/raw_dataset.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      483 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/dataset_specific/scene_records.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/filtering/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       23 2022-11-12 07:42:55.000000 trajdata-1.3.0/src/trajdata/filtering/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3659 2023-02-11 07:41:45.000000 trajdata-1.3.0/src/trajdata/filtering/filters.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/maps/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      193 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/maps/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      111 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/maps/lane_route.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1483 2023-01-05 00:00:22.000000 trajdata-1.3.0/src/trajdata/maps/map_api.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     6670 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/maps/map_kdtree.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     2116 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/maps/raster_map.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      121 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/maps/traffic_light_status.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    21905 2023-02-10 07:47:20.000000 trajdata-1.3.0/src/trajdata/maps/vec_map.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     5194 2023-01-05 00:04:06.000000 trajdata-1.3.0/src/trajdata/maps/vec_map_elements.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/parallel/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       83 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/parallel/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3423 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/parallel/data_preprocessor.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata/proto/
+-rw-r--r--   0 bivanovic (41443) dip         (30)        0 2022-10-24 06:19:35.000000 trajdata-1.3.0/src/trajdata/proto/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     5969 2023-04-07 21:05:44.000000 trajdata-1.3.0/src/trajdata/proto/vectorized_map_pb2.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.219476 trajdata-1.3.0/src/trajdata/simulation/
+-rw-r--r--   0 bivanovic (41443) dip         (30)       39 2022-11-12 06:09:23.000000 trajdata-1.3.0/src/trajdata/simulation/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1056 2023-02-11 07:41:45.000000 trajdata-1.3.0/src/trajdata/simulation/sim_cache.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    10217 2023-02-11 07:41:45.000000 trajdata-1.3.0/src/trajdata/simulation/sim_df_cache.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1077 2022-07-10 04:26:11.000000 trajdata-1.3.0/src/trajdata/simulation/sim_metrics.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     8635 2023-02-11 07:41:45.000000 trajdata-1.3.0/src/trajdata/simulation/sim_scene.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3872 2022-10-24 06:19:35.000000 trajdata-1.3.0/src/trajdata/simulation/sim_stats.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      786 2022-07-10 04:26:11.000000 trajdata-1.3.0/src/trajdata/simulation/sim_vis.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.219476 trajdata-1.3.0/src/trajdata/utils/
+-rw-r--r--   0 bivanovic (41443) dip         (30)        0 2022-07-10 04:26:11.000000 trajdata-1.3.0/src/trajdata/utils/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     2724 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/utils/agent_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    10314 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/utils/arr_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     7225 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/utils/batch_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3204 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/utils/df_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1686 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/utils/env_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    10518 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/utils/map_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     1843 2022-11-18 01:28:43.000000 trajdata-1.3.0/src/trajdata/utils/parallel_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     8175 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/utils/raster_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3520 2022-11-12 08:23:30.000000 trajdata-1.3.0/src/trajdata/utils/scene_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     5684 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/utils/state_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      186 2022-07-10 04:26:11.000000 trajdata-1.3.0/src/trajdata/utils/string_utils.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    19023 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/utils/vis_utils.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.219476 trajdata-1.3.0/src/trajdata/visualization/
+-rw-r--r--   0 bivanovic (41443) dip         (30)      160 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/visualization/__init__.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    17001 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/visualization/interactive_animation.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     5798 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/visualization/interactive_figure.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     7029 2023-04-21 23:35:15.000000 trajdata-1.3.0/src/trajdata/visualization/interactive_vis.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    13225 2023-02-04 18:48:20.000000 trajdata-1.3.0/src/trajdata/visualization/vis.py
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.215476 trajdata-1.3.0/src/trajdata.egg-info/
+-rw-r--r--   0 bivanovic (41443) dip         (30)    11300 2023-04-21 23:47:20.000000 trajdata-1.3.0/src/trajdata.egg-info/PKG-INFO
+-rw-r--r--   0 bivanovic (41443) dip         (30)     3320 2023-04-21 23:47:20.000000 trajdata-1.3.0/src/trajdata.egg-info/SOURCES.txt
+-rw-r--r--   0 bivanovic (41443) dip         (30)        1 2023-04-21 23:47:20.000000 trajdata-1.3.0/src/trajdata.egg-info/dependency_links.txt
+-rw-r--r--   0 bivanovic (41443) dip         (30)      268 2023-04-21 23:47:20.000000 trajdata-1.3.0/src/trajdata.egg-info/requires.txt
+-rw-r--r--   0 bivanovic (41443) dip         (30)        9 2023-04-21 23:47:20.000000 trajdata-1.3.0/src/trajdata.egg-info/top_level.txt
+drwxr-xr-x   0 bivanovic (41443) dip         (30)        0 2023-04-21 23:47:20.219476 trajdata-1.3.0/tests/
+-rw-r--r--   0 bivanovic (41443) dip         (30)    10463 2023-04-21 23:35:15.000000 trajdata-1.3.0/tests/test_batch_conversion.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     7443 2023-02-11 07:41:45.000000 trajdata-1.3.0/tests/test_collation.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     7569 2023-02-11 07:41:45.000000 trajdata-1.3.0/tests/test_datasizes.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)      992 2022-11-17 10:42:27.000000 trajdata-1.3.0/tests/test_description_matching.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)    13585 2023-02-11 07:41:45.000000 trajdata-1.3.0/tests/test_state.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     6304 2023-02-04 18:48:52.000000 trajdata-1.3.0/tests/test_traffic_data.py
+-rw-r--r--   0 bivanovic (41443) dip         (30)     2068 2023-01-05 00:04:06.000000 trajdata-1.3.0/tests/test_vec_map.py
```

### Comparing `trajdata-1.2.1/LICENSE` & `trajdata-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/PKG-INFO` & `trajdata-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajdata
-Version: 1.2.1
+Version: 1.3.0
 Summary: A unified interface to many trajectory forecasting datasets.
 Home-page: https://github.com/nvr-avg/trajdata
 Author: Boris Ivanovic
 Author-email: bivanovic@nvidia.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `trajdata-1.2.1/README.md` & `trajdata-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/setup.cfg` & `trajdata-1.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trajdata
-version = 1.2.1
+version = 1.3.0
 author = Boris Ivanovic
 author_email = bivanovic@nvidia.com
 description = A unified interface to many trajectory forecasting datasets.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0
 url = https://github.com/nvr-avg/trajdata
@@ -26,14 +26,15 @@
 	dill>=0.3.4
 	pandas>=1.4.1
 	pyarrow>=7.0.0
 	torch>=1.10.2
 	zarr>=2.11.0
 	kornia>=0.6.4
 	seaborn>=0.12
+	bokeh>=3.0.3
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	black
```

### Comparing `trajdata-1.2.1/src/trajdata/augmentation/augmentation.py` & `trajdata-1.3.0/src/trajdata/augmentation/augmentation.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/augmentation/low_vel_yaw_correction.py` & `trajdata-1.3.0/src/trajdata/augmentation/low_vel_yaw_correction.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/augmentation/noise_histories.py` & `trajdata-1.3.0/src/trajdata/augmentation/noise_histories.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/caching/df_cache.py` & `trajdata-1.3.0/src/trajdata/caching/df_cache.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/caching/env_cache.py` & `trajdata-1.3.0/src/trajdata/caching/env_cache.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/caching/scene_cache.py` & `trajdata-1.3.0/src/trajdata/caching/scene_cache.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/__init__.py` & `trajdata-1.3.0/src/trajdata/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/agent.py` & `trajdata-1.3.0/src/trajdata/data_structures/agent.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/batch.py` & `trajdata-1.3.0/src/trajdata/data_structures/batch.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/batch_element.py` & `trajdata-1.3.0/src/trajdata/data_structures/batch_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -542,14 +542,15 @@
                 curr_state.get_attr("x")[i],
                 curr_state.get_attr("y")[i],
                 desired_patch_size,
                 resolution,
                 offset_xy,
                 heading[i],
                 return_rgb,
+                rot_pad_factor=sqrt(2),
                 no_map_val=no_map_fill_val,
             )
             map_patches.append(
                 RasterizedMapPatch(
                     data=patch_data,
                     rot_angle=heading[i],
                     crop_size=desired_patch_size,
```

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/collation.py` & `trajdata-1.3.0/src/trajdata/data_structures/collation.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/data_index.py` & `trajdata-1.3.0/src/trajdata/data_structures/data_index.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/environment.py` & `trajdata-1.3.0/src/trajdata/data_structures/environment.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/scene.py` & `trajdata-1.3.0/src/trajdata/data_structures/scene.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/scene_metadata.py` & `trajdata-1.3.0/src/trajdata/data_structures/scene_metadata.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/data_structures/state.py` & `trajdata-1.3.0/src/trajdata/data_structures/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
     Convenience class which offers property access to state elements
     Standardizes order of state dimensions
     """
 
     _FUNCS = {
         "cos": torch.cos,
         "sin": torch.sin,
-        "arctan": torch.arctan2,
+        "arctan": torch.atan2,
         "lon_component": lon_component,
         "lat_component": lat_component,
         "x_component": x_component,
         "y_component": y_component,
     }
 
     CAPTURED_FUNCS: Set[Callable] = {
```

### Comparing `trajdata-1.2.1/src/trajdata/dataset.py` & `trajdata-1.3.0/src/trajdata/dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/dataset_specific/eth_ucy_peds/eupeds_dataset.py` & `trajdata-1.3.0/src/trajdata/dataset_specific/eth_ucy_peds/eupeds_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/dataset_specific/lyft/lyft_dataset.py` & `trajdata-1.3.0/src/trajdata/dataset_specific/lyft/lyft_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/dataset_specific/lyft/lyft_utils.py` & `trajdata-1.3.0/src/trajdata/dataset_specific/lyft/lyft_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/dataset_specific/nuplan/nuplan_dataset.py` & `trajdata-1.3.0/src/trajdata/dataset_specific/nuplan/nuplan_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/dataset_specific/nuplan/nuplan_utils.py` & `trajdata-1.3.0/src/trajdata/dataset_specific/nuplan/nuplan_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/dataset_specific/nusc/nusc_dataset.py` & `trajdata-1.3.0/src/trajdata/dataset_specific/nusc/nusc_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/dataset_specific/nusc/nusc_utils.py` & `trajdata-1.3.0/src/trajdata/dataset_specific/nusc/nusc_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/dataset_specific/raw_dataset.py` & `trajdata-1.3.0/src/trajdata/dataset_specific/raw_dataset.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/filtering/filters.py` & `trajdata-1.3.0/src/trajdata/filtering/filters.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/maps/map_api.py` & `trajdata-1.3.0/src/trajdata/maps/map_api.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/maps/map_kdtree.py` & `trajdata-1.3.0/src/trajdata/maps/map_kdtree.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from trajdata.maps.vec_map import VectorMap
 
-from typing import Optional
+from typing import Optional, Tuple
 
 import numpy as np
 from scipy.spatial import KDTree
 from tqdm import tqdm
 
 from trajdata.maps.vec_map_elements import MapElement, MapElementType, Polyline
 from trajdata.utils.arr_utils import angle_wrap
```

### Comparing `trajdata-1.2.1/src/trajdata/maps/raster_map.py` & `trajdata-1.3.0/src/trajdata/maps/raster_map.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/maps/vec_map.py` & `trajdata-1.3.0/src/trajdata/maps/vec_map.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/maps/vec_map_elements.py` & `trajdata-1.3.0/src/trajdata/maps/vec_map_elements.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/parallel/data_preprocessor.py` & `trajdata-1.3.0/src/trajdata/parallel/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/proto/vectorized_map_pb2.py` & `trajdata-1.3.0/src/trajdata/proto/vectorized_map_pb2.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/simulation/sim_cache.py` & `trajdata-1.3.0/src/trajdata/simulation/sim_cache.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/simulation/sim_df_cache.py` & `trajdata-1.3.0/src/trajdata/simulation/sim_df_cache.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/simulation/sim_metrics.py` & `trajdata-1.3.0/src/trajdata/simulation/sim_metrics.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/simulation/sim_scene.py` & `trajdata-1.3.0/src/trajdata/simulation/sim_scene.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/simulation/sim_stats.py` & `trajdata-1.3.0/src/trajdata/simulation/sim_stats.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/simulation/sim_vis.py` & `trajdata-1.3.0/src/trajdata/simulation/sim_vis.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/utils/agent_utils.py` & `trajdata-1.3.0/src/trajdata/utils/agent_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/utils/arr_utils.py` & `trajdata-1.3.0/src/trajdata/utils/arr_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,31 +160,31 @@
     offset: Optional[np.ndarray] = None,
     angle: Optional[np.ndarray] = None,
     rot_mat: Optional[np.ndarray] = None,
 ) -> np.ndarray:
     """
     Args:
         coords (np.ndarray): [..., 2] coordinates
-        offset (Optional[np.ndarray], optional): [..., 2] offset to transalte. Defaults to None.
+        offset (Optional[np.ndarray], optional): [..., 2] offset to translate. Defaults to None.
         angle (Optional[np.ndarray], optional): [...] angle to rotate by. Defaults to None.
         rot_mat (Optional[np.ndarray], optional): [..., 2,2] rotation matrix to apply. Defaults to None.
             If rot_mat is given, angle is ignored.
 
     Returns:
         np.ndarray: transformed coords
     """
-    if offset is not None:
-        coords = coords + offset
-
     if rot_mat is None and angle is not None:
         rot_mat = rotation_matrix(angle)
 
     if rot_mat is not None:
         coords = np.einsum("...ij,...j->...i", rot_mat, coords)
 
+    if offset is not None:
+        coords += offset
+
     return coords
 
 
 def transform_coords_np(
     coords: np.ndarray, tf_mat: np.ndarray, translate: bool = True
 ) -> np.ndarray:
     """
@@ -236,15 +236,15 @@
     Returns transformed set of xyh points
 
     Args:
         xyh (np.ndarray): shape [...,3]
         tf_mat (np.ndarray): shape [...,3,3]
     """
     transformed_xy = transform_coords_np(xyh[..., :2], tf_mat)
-    transformed_angles = transform_angles_np(xyh[..., 3], tf_mat)
+    transformed_angles = transform_angles_np(xyh[..., 2], tf_mat)
     return np.concatenate([transformed_xy, transformed_angles[..., None]], axis=-1)
 
 
 def agent_aware_diff(values: np.ndarray, agent_ids: np.ndarray) -> np.ndarray:
     values_diff: np.ndarray = np.diff(
         values, axis=0, prepend=values[[0]] - (values[[1]] - values[[0]])
     )
```

### Comparing `trajdata-1.2.1/src/trajdata/utils/df_utils.py` & `trajdata-1.3.0/src/trajdata/utils/df_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/utils/env_utils.py` & `trajdata-1.3.0/src/trajdata/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/utils/map_utils.py` & `trajdata-1.3.0/src/trajdata/utils/map_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from tqdm import tqdm
-
 if TYPE_CHECKING:
     from trajdata.maps import map_kdtree, vec_map
 
 from pathlib import Path
 from typing import Dict, Final, Optional
 
 import dill
 import numpy as np
 from scipy.stats import circmean
 
-import trajdata.maps.vec_map_elements as vec_map_elems
 import trajdata.proto.vectorized_map_pb2 as map_proto
 from trajdata.utils import arr_utils
 
 MM_PER_M: Final[float] = 1000
 
 
 def decompress_values(data: np.ndarray) -> np.ndarray:
```

### Comparing `trajdata-1.2.1/src/trajdata/utils/parallel_utils.py` & `trajdata-1.3.0/src/trajdata/utils/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/utils/raster_utils.py` & `trajdata-1.3.0/src/trajdata/utils/raster_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/utils/scene_utils.py` & `trajdata-1.3.0/src/trajdata/utils/scene_utils.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata/utils/state_utils.py` & `trajdata-1.3.0/src/trajdata/utils/state_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         rot_mat Optional[nd.array]: rotation matrix A such that c = A @ b returns coordinates in the new frame
             if not given, it is computed frome frame_state
     """
     new_state = state.copy()
     attributes = state._format_dict.keys()
 
     frame_heading = frame_state.heading[..., 0]
-    if rot_mat is not None:
+    if rot_mat is None:
         rot_mat = rotation_matrix(frame_heading)
 
     if "x" in attributes and "y" in attributes:
         # transform xy position with translation and rotation
         new_state.position = (
             transform_coords_2d_np(state.position, rot_mat=rot_mat)
             + frame_state.position
```

### Comparing `trajdata-1.2.1/src/trajdata/visualization/vis.py` & `trajdata-1.3.0/src/trajdata/visualization/vis.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/src/trajdata.egg-info/PKG-INFO` & `trajdata-1.3.0/src/trajdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trajdata
-Version: 1.2.1
+Version: 1.3.0
 Summary: A unified interface to many trajectory forecasting datasets.
 Home-page: https://github.com/nvr-avg/trajdata
 Author: Boris Ivanovic
 Author-email: bivanovic@nvidia.com
 License: Apache License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `trajdata-1.2.1/src/trajdata.egg-info/SOURCES.txt` & `trajdata-1.3.0/src/trajdata.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,19 @@
 src/trajdata/utils/env_utils.py
 src/trajdata/utils/map_utils.py
 src/trajdata/utils/parallel_utils.py
 src/trajdata/utils/raster_utils.py
 src/trajdata/utils/scene_utils.py
 src/trajdata/utils/state_utils.py
 src/trajdata/utils/string_utils.py
+src/trajdata/utils/vis_utils.py
 src/trajdata/visualization/__init__.py
+src/trajdata/visualization/interactive_animation.py
+src/trajdata/visualization/interactive_figure.py
+src/trajdata/visualization/interactive_vis.py
 src/trajdata/visualization/vis.py
 tests/test_batch_conversion.py
 tests/test_collation.py
 tests/test_datasizes.py
 tests/test_description_matching.py
 tests/test_state.py
 tests/test_traffic_data.py
```

### Comparing `trajdata-1.2.1/tests/test_collation.py` & `trajdata-1.3.0/tests/test_collation.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/tests/test_datasizes.py` & `trajdata-1.3.0/tests/test_datasizes.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/tests/test_description_matching.py` & `trajdata-1.3.0/tests/test_description_matching.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/tests/test_state.py` & `trajdata-1.3.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/tests/test_traffic_data.py` & `trajdata-1.3.0/tests/test_traffic_data.py`

 * *Files identical despite different names*

### Comparing `trajdata-1.2.1/tests/test_vec_map.py` & `trajdata-1.3.0/tests/test_vec_map.py`

 * *Files identical despite different names*

