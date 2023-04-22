# Comparing `tmp/Simba-UW-tf-dev-1.57.2.tar.gz` & `tmp/Simba-UW-tf-dev-1.57.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.2.tar", last modified: Fri Apr 21 19:35:06 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.3.tar", last modified: Sat Apr 22 15:30:26 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.57.2.tar` & `Simba-UW-tf-dev-1.57.3.tar`

### file list

```diff
@@ -1,394 +1,395 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/
--rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.57.2/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.2/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11938 2023-04-20 14:29:24.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10960 2023-04-19 14:59:03.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     3354 2023-04-20 14:05:40.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-20 13:38:50.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7569 2023-04-20 15:20:31.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4812 2023-04-20 14:48:41.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     6687 2023-04-20 15:04:13.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9907 2023-04-20 12:55:14.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     8375 2023-04-19 18:35:33.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41552 2023-04-20 14:49:52.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2331 2023-04-20 12:56:44.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    18472 2023-04-19 23:04:27.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)     8421 2023-04-20 13:33:19.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.57.2/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.57.2/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-20 15:30:01.000000 Simba-UW-tf-dev-1.57.2/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     1959 2023-04-20 20:07:38.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    26890 2023-04-20 18:25:40.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-21 18:44:23.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.2/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.2/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.57.2/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42063 2023-04-19 23:53:37.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8292 2023-04-21 12:36:21.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6092 2023-04-19 18:08:18.000000 Simba-UW-tf-dev-1.57.2/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.57.2/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.2/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.57.2/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.57.2/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.2/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.2/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.2/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.57.2/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.57.2/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.57.2/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.2/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    47395 2023-04-20 01:59:56.000000 Simba-UW-tf-dev-1.57.2/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.2/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.57.2/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.2/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.57.2/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.57.2/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.57.2/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    10872 2023-04-21 16:14:46.000000 Simba-UW-tf-dev-1.57.2/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.57.2/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.57.2/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.57.2/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17352 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12507 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.57.2/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    56353 2023-04-20 15:18:16.000000 Simba-UW-tf-dev-1.57.2/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.2/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   234964 2023-04-13 14:18:43.000000 Simba-UW-tf-dev-1.57.2/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.57.2/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.2/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    19358 2023-04-21 19:25:08.000000 Simba-UW-tf-dev-1.57.2/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    64335 2023-04-21 19:27:47.000000 Simba-UW-tf-dev-1.57.2/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-21 16:17:45.000000 Simba-UW-tf-dev-1.57.2/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.2/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.2/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.57.2/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     9460 2023-04-21 14:18:35.000000 Simba-UW-tf-dev-1.57.2/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.57.2/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.57.2/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.2/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.2/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.2/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.2/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13500 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-21 19:35:05.000000 Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.2/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.2/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.2/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-21 19:34:57.000000 Simba-UW-tf-dev-1.57.2/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-21 19:35:06.000000 Simba-UW-tf-dev-1.57.2/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.57.3/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.3/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11938 2023-04-20 14:29:24.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10960 2023-04-19 14:59:03.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     3354 2023-04-20 14:05:40.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-20 13:38:50.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7569 2023-04-20 15:20:31.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4812 2023-04-20 14:48:41.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     6687 2023-04-20 15:04:13.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9907 2023-04-20 12:55:14.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     8375 2023-04-19 18:35:33.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41552 2023-04-20 14:49:52.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2331 2023-04-20 12:56:44.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18472 2023-04-19 23:04:27.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)     8421 2023-04-20 13:33:19.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.57.3/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-22 15:14:38.000000 Simba-UW-tf-dev-1.57.3/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     1959 2023-04-20 20:07:38.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    26890 2023-04-20 18:25:40.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-21 18:44:23.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.3/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.3/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.57.3/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42063 2023-04-19 23:53:37.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8351 2023-04-22 13:11:36.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6092 2023-04-19 18:08:18.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.57.3/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.3/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.57.3/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.57.3/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.3/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.3/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.3/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.57.3/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.57.3/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.57.3/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.3/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    47395 2023-04-20 01:59:56.000000 Simba-UW-tf-dev-1.57.3/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.3/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.57.3/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.3/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.57.3/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.57.3/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.57.3/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    10872 2023-04-21 16:14:46.000000 Simba-UW-tf-dev-1.57.3/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.57.3/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.57.3/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.57.3/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17891 2023-04-22 14:54:57.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12889 2023-04-22 14:51:45.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.57.3/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    56353 2023-04-20 15:18:16.000000 Simba-UW-tf-dev-1.57.3/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   236359 2023-04-22 15:26:04.000000 Simba-UW-tf-dev-1.57.3/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.57.3/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.3/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    19358 2023-04-21 19:25:08.000000 Simba-UW-tf-dev-1.57.3/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    64554 2023-04-22 15:14:52.000000 Simba-UW-tf-dev-1.57.3/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-22 15:14:38.000000 Simba-UW-tf-dev-1.57.3/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.57.3/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     9460 2023-04-21 14:18:35.000000 Simba-UW-tf-dev-1.57.3/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.57.3/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.57.3/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.3/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13533 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.3/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.3/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.3/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-22 15:30:17.000000 Simba-UW-tf-dev-1.57.3/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.57.2/PKG-INFO` & `Simba-UW-tf-dev-1.57.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.2
+Version: 1.57.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.2/simba/video_processing.py` & `Simba-UW-tf-dev-1.57.3/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.57.3/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/enums.py` & `Simba-UW-tf-dev-1.57.3/simba/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/find_bounderies.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -509,261 +509,261 @@
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0013 0000 000b  ................
 00002010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00002020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00002030: 0000 0042 1115 0000 000b 005f 005f 0070  ...B......._._.p
+00002030: 0000 0042 1d4f 0000 000b 005f 005f 0070  ...B.O....._._.p
 00002040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00002050: 6d6f 4444 626c 6f62 0000 0008 4af4 9086  moDDblob....J...
-00002060: aef8 c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+00002050: 6d6f 4444 626c 6f62 0000 0008 3293 8634  moDDblob....2..4
+00002060: 16fa c441 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
 00002070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 00002080: 6444 626c 6f62 0000 0008 6a13 8953 eaf6  dDblob....j..S..
 00002090: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000020a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000020b0: 636f 6d70 0000 0000 0050 0000 0000 0006  comp.....P......
 000020c0: 0061 0073 0073 0065 0074 0073 6277 7370  .a.s.s.e.t.sbwsp
-000020d0: 626c 6f62 0000 00c8 6270 6c69 7374 3030  blob....bplist00
+000020d0: 626c 6f62 0000 00ca 6270 6c69 7374 3030  blob....bplist00
 000020e0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
 000020f0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 00002100: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
 00002110: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00002120: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00002130: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00002140: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00002150: 7208 0809 0809 5f10 177b 7b33 342c 2039  r....._..{{34, 9
-00002160: 307d 2c20 7b31 3031 352c 2037 3637 7d7d  0}, {1015, 767}}
-00002170: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e98  ...%1=I`myz{|}~.
-00002180: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00002190: 0000 0000 0000 0000 0000 0000 0000 0099  ................
-000021a0: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
-000021b0: 6c67 3153 636f 6d70 0000 0000 007d d138  lg1Scomp.....}.8
-000021c0: 0000 0006 0061 0073 0073 0065 0074 0073  .....a.s.s.e.t.s
-000021d0: 6c73 7643 626c 6f62 0000 02b0 6270 6c69  lsvCblob....bpli
-000021e0: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-000021f0: 0c0d 1848 4948 4a4b 0c5f 1012 7669 6577  ...HIHJK._..view
-00002200: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-00002210: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00002220: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00002230: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00002240: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-00002250: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-00002260: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-00002270: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-00002280: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-00002290: 1001 09ab 0e17 1c21 252a 2f34 393e 43d4  .......!%*/49>C.
-000022a0: 0f10 1112 0c14 0c16 5776 6973 6962 6c65  ........Wvisible
-000022b0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-000022c0: 5a69 6465 6e74 6966 6965 7209 1101 2709  Zidentifier...'.
-000022d0: 546e 616d 65d4 0f10 1112 1819 181b 0810  Tname...........
-000022e0: 2308 5875 6269 7175 6974 79d4 0f10 1112  #.Xubiquity.....
-000022f0: 0c1e 1820 0910 b508 5c64 6174 654d 6f64  ... ....\dateMod
-00002300: 6966 6965 64d4 0f10 1112 181e 1824 0808  ified........$..
-00002310: 5b64 6174 6543 7265 6174 6564 d40f 1011  [dateCreated....
-00002320: 120c 2718 2909 1061 0854 7369 7a65 d40f  ..'.)..a.Tsize..
-00002330: 1011 120c 2c0c 2e09 1073 0954 6b69 6e64  ....,....s.Tkind
-00002340: d40f 1011 1218 310c 3308 1064 0955 6c61  ......1.3..d.Ula
-00002350: 6265 6cd4 0f10 1112 1836 0c38 0810 4b09  bel......6.8..K.
-00002360: 5776 6572 7369 6f6e d40f 1011 1218 3b0c  Wversion......;.
-00002370: 3d08 1101 2c09 5863 6f6d 6d65 6e74 73d4  =...,.Xcomments.
-00002380: 0f10 1112 1840 1842 0810 c808 5e64 6174  .....@.B....^dat
-00002390: 654c 6173 744f 7065 6e65 64d4 0f10 1112  eLastOpened.....
-000023a0: 181e 1846 0808 5964 6174 6541 6464 6564  ...F..YdateAdded
-000023b0: 0823 0000 0000 0000 0000 2340 2800 0000  .#........#@(...
-000023c0: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
-000023d0: 0009 0008 001d 0032 0044 004c 0060 0072  .......2.D.L.`.r
-000023e0: 007b 008d 0098 00a1 00b4 00b6 00b7 00c3  .{..............
-000023f0: 00cc 00d4 00da 00e4 00ef 00f0 00f3 00f4  ................
-00002400: 00f9 0102 0103 0105 0106 010f 0118 0119  ................
-00002410: 011b 011c 0129 0132 0133 0134 0140 0149  .....).2.3.4.@.I
-00002420: 014a 014c 014d 0152 015b 015c 015e 015f  .J.L.M.R.[.\.^._
-00002430: 0164 016d 016e 0170 0171 0177 0180 0181  .d.m.n.p.q.w....
-00002440: 0183 0184 018c 0195 0196 0199 019a 01a3  ................
-00002450: 01ac 01ad 01af 01b0 01bf 01c8 01c9 01ca  ................
-00002460: 01d4 01d5 01de 01e7 01ec 01f5 0000 0000  ................
-00002470: 0000 0201 0000 0000 0000 004d 0000 0000  ...........M....
-00002480: 0000 0000 0000 0000 0000 01f6 0000 0006  ................
-00002490: 0061 0073 0073 0065 0074 0073 6c73 7670  .a.s.s.e.t.slsvp
-000024a0: 626c 6f62 0000 0295 6270 6c69 7374 3030  blob....bplist00
-000024b0: da01 0203 0405 0607 0809 0a0b 0c0d 1f47  ...............G
-000024c0: 4847 494a 0c5f 1012 7669 6577 4f70 7469  HGIJ._..viewOpti
-000024d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-000024e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-000024f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00002500: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
-00002510: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
-00002520: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
-00002530: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
-00002540: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
-00002550: 656c 6174 6976 6544 6174 6573 1001 09d9  elativeDates....
-00002560: 0e0f 1011 1213 1415 1617 2025 292d 3237  .......... %)-27
-00002570: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
-00002580: 4c61 7374 4f70 656e 6564 5c64 6174 654d  LastOpened\dateM
-00002590: 6f64 6966 6965 645b 6461 7465 4372 6561  odified[dateCrea
-000025a0: 7465 6454 7369 7a65 556c 6162 656c 546b  tedTsizeUlabelTk
-000025b0: 696e 6457 7665 7273 696f 6e54 6e61 6d65  indWversionTname
-000025c0: d418 191a 1b1c 1d0c 1f55 696e 6465 7855  .........UindexU
-000025d0: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-000025e0: 7669 7369 626c 6510 0711 012c 0908 d418  visible....,....
-000025f0: 191a 1b21 221f 1f10 0810 c808 08d4 1819  ...!"...........
-00002600: 1a1b 0b26 1f0c 10b5 0809 d418 191a 1b2a  ...&...........*
-00002610: 261f 1f10 0208 08d4 1819 1a1b 2e2f 1f0c  &............/..
-00002620: 1003 1061 0809 d418 191a 1b33 340c 1f10  ...a.......34...
-00002630: 0510 6409 08d4 1819 1a1b 3839 0c0c 1004  ..d.......89....
-00002640: 1073 0909 d418 191a 1b3d 3e0c 1f10 0610  .s.......=>.....
-00002650: 4b09 08d4 1819 1a1b 4243 0c0c 1000 1101  K.......BC......
-00002660: 2709 0908 2300 0000 0000 0000 0023 4028  '...#........#@(
-00002670: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
-00002680: 0000 0000 0900 0800 1d00 3200 4400 4c00  ..........2.D.L.
-00002690: 6000 7200 7b00 8d00 9800 a100 b400 b600  `.r.{...........
-000026a0: b700 ca00 d300 e200 ef00 fb01 0001 0601  ................
-000026b0: 0b01 1301 1801 2101 2701 2d01 3701 3f01  ......!.'.-.7.?.
-000026c0: 4101 4401 4501 4601 4f01 5101 5301 5401  A.D.E.F.O.Q.S.T.
-000026d0: 5501 5e01 6001 6101 6201 6b01 6d01 6e01  U.^.`.a.b.k.m.n.
-000026e0: 6f01 7801 7a01 7c01 7d01 7e01 8701 8901  o.x.z.|.}.~.....
-000026f0: 8b01 8c01 8d01 9601 9801 9a01 9b01 9c01  ................
-00002700: a501 a701 a901 aa01 ab01 b401 b601 b901  ................
-00002710: ba01 bb01 bc01 c501 ce01 d301 dc00 0000  ................
-00002720: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
-00002730: 0000 0000 0000 0000 0000 0001 dd00 0000  ................
-00002740: 0600 6100 7300 7300 6500 7400 736d 6f44  ..a.s.s.e.t.smoD
-00002750: 4462 6c6f 6200 0000 08cf 958c e8d0 e1c4  Dblob...........
-00002760: 4100 0000 0600 6100 7300 7300 6500 7400  A.....a.s.s.e.t.
-00002770: 736d 6f64 4462 6c6f 6200 0000 08cf 958c  smodDblob.......
-00002780: e8d0 e1c4 4100 0000 0600 6100 7300 7300  ....A.....a.s.s.
-00002790: 6500 7400 7370 6831 5363 6f6d 7000 0000  e.t.sph1Scomp...
-000027a0: 0000 8190 0000 0000 0600 6100 7300 7300  ..........a.s.s.
-000027b0: 6500 7400 7376 5372 6e6c 6f6e 6700 0000  e.t.svSrnlong...
-000027c0: 0100 0000 1400 6200 6100 7400 6300 6800  ......b.a.t.c.h.
-000027d0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
-000027e0: 5f00 7600 6900 6400 6500 6f00 7362 7773  _.v.i.d.e.o.sbws
-000027f0: 7062 6c6f 6200 0000 ca62 706c 6973 7430  pblob....bplist0
-00002800: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
-00002810: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-00002820: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
-00002830: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00002840: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-00002850: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-00002860: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00002870: 6172 0808 0908 095f 1019 7b7b 3130 3632  ar....._..{{1062
-00002880: 2c20 3337 337d 2c20 7b37 3730 2c20 3433  , 373}, {770, 43
-00002890: 367d 7d09 0817 2531 3d49 606d 797a 7b7c  6}}...%1=I`myz{|
-000028a0: 7d7e 9a00 0000 0000 0001 0100 0000 0000  }~..............
-000028b0: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
-000028c0: 0000 9b00 0000 1400 6200 6100 7400 6300  ........b.a.t.c.
-000028d0: 6800 5f00 7000 7200 6f00 6300 6500 7300  h._.p.r.o.c.e.s.
-000028e0: 7300 5f00 7600 6900 6400 6500 6f00 736c  s._.v.i.d.e.o.sl
-000028f0: 6731 5363 6f6d 7000 0000 0000 017e 5700  g1Scomp......~W.
-00002900: 0000 1400 6200 6100 7400 6300 6800 5f00  ....b.a.t.c.h._.
-00002910: 7000 7200 6f00 6300 6500 7300 7300 5f00  p.r.o.c.e.s.s._.
-00002920: 7600 6900 6400 6500 6f00 736c 7376 4362  v.i.d.e.o.slsvCb
-00002930: 6c6f 6200 0003 0762 706c 6973 7430 30d8  lob....bplist00.
-00002940: 0102 0304 0506 0708 090a 0b19 5657 0a59  ............VW.Y
-00002950: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
-00002960: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00002970: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00002980: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
-00002990: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-000029a0: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-000029b0: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-000029c0: 696f 6e23 4030 0000 0000 0000 09ae 0c15  ion#@0..........
-000029d0: 1d22 262b 3035 3a3f 4448 4d51 d40d 0e0f  ."&+05:?DHMQ....
-000029e0: 1011 120a 0a5a 6964 656e 7469 6669 6572  .....Zidentifier
-000029f0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-00002a00: 5776 6973 6962 6c65 546e 616d 6511 032a  WvisibleTname..*
-00002a10: 0909 d416 1718 0d19 1a19 1c57 7669 7369  ...........Wvisi
-00002a20: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
-00002a30: 696e 6708 1023 0858 7562 6971 7569 7479  ing..#.Xubiquity
-00002a40: d40d 0e0f 101e 1f19 0a5c 6461 7465 4d6f  .........\dateMo
-00002a50: 6469 6669 6564 10b5 0809 d40d 0e0f 1023  dified.........#
-00002a60: 1f19 195b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
-00002a70: 08d4 0d0e 0f10 2728 190a 5473 697a 6510  ......'(..Tsize.
-00002a80: 6108 09d4 0d0e 0f10 2c2d 0a0a 546b 696e  a.......,-..Tkin
-00002a90: 6410 7309 09d4 0d0e 0f10 3132 0a19 556c  d.s.......12..Ul
-00002aa0: 6162 656c 1064 0908 d40d 0e0f 1036 370a  abel.d.......67.
-00002ab0: 1957 7665 7273 696f 6e10 4b09 08d4 0d0e  .Wversion.K.....
-00002ac0: 0f10 3b3c 0a19 5863 6f6d 6d65 6e74 7311  ..;<..Xcomments.
-00002ad0: 012c 0908 d40d 0e0f 1040 4119 195e 6461  .,.......@A..^da
-00002ae0: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
-00002af0: d416 1718 0d19 1f19 4708 0859 6461 7465  ........G..Ydate
-00002b00: 4164 6465 64d4 0d17 1816 494a 1919 5a73  Added.....IJ..Zs
-00002b10: 6861 7265 4f77 6e65 7210 d208 08d4 0d17  hareOwner.......
-00002b20: 1816 4e4a 1919 5f10 0f73 6861 7265 4c61  ..NJ.._..shareLa
-00002b30: 7374 4564 6974 6f72 0808 d40d 1718 1652  stEditor.......R
-00002b40: 4a19 195f 1010 696e 7669 7461 7469 6f6e  J.._..invitation
-00002b50: 5374 6174 7573 0808 0823 4028 0000 0000  Status...#@(....
-00002b60: 0000 546e 616d 6509 1001 0008 0019 0022  ..Tname........"
-00002b70: 0034 003c 0050 0059 0064 0077 008c 0095  .4.<.P.Y.d.w....
-00002b80: 0096 00a5 00ae 00b9 00bf 00c9 00d1 00d6  ................
-00002b90: 00d9 00da 00db 00e4 00ec 00f2 00fc 00fd  ................
-00002ba0: 00ff 0100 0109 0112 011f 0121 0122 0123  ...........!.".#
-00002bb0: 012c 0138 0139 013a 0143 0148 014a 014b  .,.8.9.:.C.H.J.K
-00002bc0: 014c 0155 015a 015c 015d 015e 0167 016d  .L.U.Z.\.].^.g.m
-00002bd0: 016f 0170 0171 017a 0182 0184 0185 0186  .o.p.q.z........
-00002be0: 018f 0198 019b 019c 019d 01a6 01b5 01b7  ................
-00002bf0: 01b8 01b9 01c2 01c3 01c4 01ce 01d7 01e2  ................
-00002c00: 01e4 01e5 01e6 01ef 0201 0202 0203 020c  ................
-00002c10: 021f 0220 0221 0222 022b 0230 0231 0000  ... .!.".+.0.1..
-00002c20: 0000 0000 0201 0000 0000 0000 005a 0000  .............Z..
-00002c30: 0000 0000 0000 0000 0000 0000 0233 0000  .............3..
-00002c40: 0014 0062 0061 0074 0063 0068 005f 0070  ...b.a.t.c.h._.p
-00002c50: 0072 006f 0063 0065 0073 0073 005f 0076  .r.o.c.e.s.s._.v
-00002c60: 0069 0064 0065 006f 0073 6c73 7670 626c  .i.d.e.o.slsvpbl
-00002c70: 6f62 0000 025e 6270 6c69 7374 3030 d801  ob...^bplist00..
-00002c80: 0203 0405 0607 0809 0a0b 1a46 470a 3558  ...........FG.5X
-00002c90: 6963 6f6e 5369 7a65 5f10 0f73 686f 7749  iconSize_..showI
-00002ca0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00002cb0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00002cc0: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-00002cd0: 736f 7274 436f 6c75 6d6e 5f10 1075 7365  sortColumn_..use
-00002ce0: 5265 6c61 7469 7665 4461 7465 735f 1012  RelativeDates_..
-00002cf0: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00002d00: 6f6e 2340 3000 0000 0000 0009 d90c 0d0e  on#@0...........
-00002d10: 0f10 1112 1314 151e 2328 2d32 363b 4058  ........#(-26;@X
-00002d20: 636f 6d6d 656e 7473 556c 6162 656c 5776  commentsUlabelWv
-00002d30: 6572 7369 6f6e 5b64 6174 6543 7265 6174  ersion[dateCreat
-00002d40: 6564 5473 697a 655c 6461 7465 4d6f 6469  edTsize\dateModi
-00002d50: 6669 6564 546b 696e 6454 6e61 6d65 5e64  fiedTkindTname^d
-00002d60: 6174 654c 6173 744f 7065 6e65 64d4 1617  ateLastOpened...
-00002d70: 1819 1a1b 0a1d 5776 6973 6962 6c65 5577  ......WvisibleUw
-00002d80: 6964 7468 5961 7363 656e 6469 6e67 5569  idthYascendingUi
-00002d90: 6e64 6578 0811 012c 0910 07d4 1617 1819  ndex...,........
-00002da0: 1a20 0a22 0810 6409 1005 d416 1718 191a  . ."..d.........
-00002db0: 250a 2708 104b 0910 06d4 1617 1819 1a2a  %.'..K.........*
-00002dc0: 1a2c 0810 b508 1002 d416 1718 190a 2f1a  .,............/.
-00002dd0: 3109 1061 0810 03d4 1617 1819 0a2a 1a35  1..a.........*.5
-00002de0: 0908 1001 d416 1718 190a 380a 3a09 1073  ..........8.:..s
-00002df0: 0910 04d4 1617 1819 0a3d 0a3f 0911 032a  .........=.?...*
-00002e00: 0910 00d4 1617 1819 1a42 1a44 0810 c808  .........B.D....
-00002e10: 1008 0823 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00002e20: 6509 0008 0019 0022 0034 003c 0050 0059  e......".4.<.P.Y
-00002e30: 0064 0077 008c 0095 0096 00a9 00b2 00b8  .d.w............
-00002e40: 00c0 00cc 00d1 00de 00e3 00e8 00f7 0100  ................
-00002e50: 0108 010e 0118 011e 011f 0122 0123 0125  ...........".#.%
-00002e60: 012e 012f 0131 0132 0134 013d 013e 0140  .../.1.2.4.=.>.@
-00002e70: 0141 0143 014c 014d 014f 0150 0152 015b  .A.C.L.M.O.P.R.[
-00002e80: 015c 015e 015f 0161 016a 016b 016c 016e  .\.^._.a.j.k.l.n
-00002e90: 0177 0178 017a 017b 017d 0186 0187 018a  .w.x.z.{.}......
-00002ea0: 018b 018d 0196 0197 0199 019a 019c 019d  ................
-00002eb0: 01a6 01ab 0000 0000 0000 0201 0000 0000  ................
-00002ec0: 0000 0049 0000 0000 0000 0000 0000 0000  ...I............
-00002ed0: 0000 01ac 0000 0014 0062 0061 0074 0063  .........b.a.t.c
-00002ee0: 0068 005f 0070 0072 006f 0063 0065 0073  .h._.p.r.o.c.e.s
-00002ef0: 0073 005f 0076 0069 0064 0065 006f 0073  .s._.v.i.d.e.o.s
-00002f00: 6d6f 4444 626c 6f62 0000 0008 f203 dcf3  moDDblob........
-00002f10: ebf6 c441 0000 0014 0062 0061 0074 0063  ...A.....b.a.t.c
-00002f20: 0068 005f 0070 0072 006f 0063 0065 0073  .h._.p.r.o.c.e.s
-00002f30: 0073 005f 0076 0069 0064 0065 006f 0073  .s._.v.i.d.e.o.s
-00002f40: 6d6f 6444 626c 6f62 0000 0008 4b60 d4fa  modDblob....K`..
-00002f50: 99f1 c441 0000 0014 0062 0061 0074 0063  ...A.....b.a.t.c
-00002f60: 0068 005f 0070 0072 006f 0063 0065 0073  .h._.p.r.o.c.e.s
-00002f70: 0073 005f 0076 0069 0064 0065 006f 0073  .s._.v.i.d.e.o.s
-00002f80: 7068 3153 636f 6d70 0000 0000 0001 f000  ph1Scomp........
-00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002150: 7208 0809 0809 5f10 197b 7b34 3230 2c20  r....._..{{420, 
+00002160: 3131 337d 2c20 7b31 3031 352c 2037 3637  113}, {1015, 767
+00002170: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
+00002180: 7e9a 0000 0000 0000 0101 0000 0000 0000  ~...............
+00002190: 000f 0000 0000 0000 0000 0000 0000 0000  ................
+000021a0: 009b 0000 0006 0061 0073 0073 0065 0074  .......a.s.s.e.t
+000021b0: 0073 6c67 3153 636f 6d70 0000 0000 007d  .slg1Scomp.....}
+000021c0: d138 0000 0006 0061 0073 0073 0065 0074  .8.....a.s.s.e.t
+000021d0: 0073 6c73 7643 626c 6f62 0000 02b0 6270  .slsvCblob....bp
+000021e0: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
+000021f0: 0a0b 0c0d 1848 4948 4a4b 0c5f 1012 7669  .....HIHJK._..vi
+00002200: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00002210: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00002220: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00002230: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
+00002240: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
+00002250: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
+00002260: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
+00002270: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
+00002280: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+00002290: 6573 1001 09ab 0e17 1c21 252a 2f34 393e  es.......!%*/49>
+000022a0: 43d4 0f10 1112 0c14 0c16 5776 6973 6962  C.........Wvisib
+000022b0: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+000022c0: 6e67 5a69 6465 6e74 6966 6965 7209 1101  ngZidentifier...
+000022d0: 2709 546e 616d 65d4 0f10 1112 1819 181b  '.Tname.........
+000022e0: 0810 2308 5875 6269 7175 6974 79d4 0f10  ..#.Xubiquity...
+000022f0: 1112 0c1e 1820 0910 b508 5c64 6174 654d  ..... ....\dateM
+00002300: 6f64 6966 6965 64d4 0f10 1112 181e 1824  odified........$
+00002310: 0808 5b64 6174 6543 7265 6174 6564 d40f  ..[dateCreated..
+00002320: 1011 120c 2718 2909 1061 0854 7369 7a65  ....'.)..a.Tsize
+00002330: d40f 1011 120c 2c0c 2e09 1073 0954 6b69  ......,....s.Tki
+00002340: 6e64 d40f 1011 1218 310c 3308 1064 0955  nd......1.3..d.U
+00002350: 6c61 6265 6cd4 0f10 1112 1836 0c38 0810  label......6.8..
+00002360: 4b09 5776 6572 7369 6f6e d40f 1011 1218  K.Wversion......
+00002370: 3b0c 3d08 1101 2c09 5863 6f6d 6d65 6e74  ;.=...,.Xcomment
+00002380: 73d4 0f10 1112 1840 1842 0810 c808 5e64  s......@.B....^d
+00002390: 6174 654c 6173 744f 7065 6e65 64d4 0f10  ateLastOpened...
+000023a0: 1112 181e 1846 0808 5964 6174 6541 6464  .....F..YdateAdd
+000023b0: 6564 0823 0000 0000 0000 0000 2340 2800  ed.#........#@(.
+000023c0: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+000023d0: 0000 0009 0008 001d 0032 0044 004c 0060  .........2.D.L.`
+000023e0: 0072 007b 008d 0098 00a1 00b4 00b6 00b7  .r.{............
+000023f0: 00c3 00cc 00d4 00da 00e4 00ef 00f0 00f3  ................
+00002400: 00f4 00f9 0102 0103 0105 0106 010f 0118  ................
+00002410: 0119 011b 011c 0129 0132 0133 0134 0140  .......).2.3.4.@
+00002420: 0149 014a 014c 014d 0152 015b 015c 015e  .I.J.L.M.R.[.\.^
+00002430: 015f 0164 016d 016e 0170 0171 0177 0180  ._.d.m.n.p.q.w..
+00002440: 0181 0183 0184 018c 0195 0196 0199 019a  ................
+00002450: 01a3 01ac 01ad 01af 01b0 01bf 01c8 01c9  ................
+00002460: 01ca 01d4 01d5 01de 01e7 01ec 01f5 0000  ................
+00002470: 0000 0000 0201 0000 0000 0000 004d 0000  .............M..
+00002480: 0000 0000 0000 0000 0000 0000 01f6 0000  ................
+00002490: 0006 0061 0073 0073 0065 0074 0073 6c73  ...a.s.s.e.t.sls
+000024a0: 7670 626c 6f62 0000 0295 6270 6c69 7374  vpblob....bplist
+000024b0: 3030 da01 0203 0405 0607 0809 0a0b 0c0d  00..............
+000024c0: 1f47 4847 494a 0c5f 1012 7669 6577 4f70  .GHGIJ._..viewOp
+000024d0: 7469 6f6e 7356 6572 7369 6f6e 5f10 0f73  tionsVersion_..s
+000024e0: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+000024f0: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00002500: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00002510: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+00002520: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+00002530: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+00002540: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
+00002550: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
+00002560: 09d9 0e0f 1011 1213 1415 1617 2025 292d  ............ %)-
+00002570: 3237 3c41 5863 6f6d 6d65 6e74 735e 6461  27<AXcomments^da
+00002580: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+00002590: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+000025a0: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+000025b0: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+000025c0: 6d65 d418 191a 1b1c 1d0c 1f55 696e 6465  me.........Uinde
+000025d0: 7855 7769 6474 6859 6173 6365 6e64 696e  xUwidthYascendin
+000025e0: 6757 7669 7369 626c 6510 0711 012c 0908  gWvisible....,..
+000025f0: d418 191a 1b21 221f 1f10 0810 c808 08d4  .....!".........
+00002600: 1819 1a1b 0b26 1f0c 10b5 0809 d418 191a  .....&..........
+00002610: 1b2a 261f 1f10 0208 08d4 1819 1a1b 2e2f  .*&............/
+00002620: 1f0c 1003 1061 0809 d418 191a 1b33 340c  .....a.......34.
+00002630: 1f10 0510 6409 08d4 1819 1a1b 3839 0c0c  ....d.......89..
+00002640: 1004 1073 0909 d418 191a 1b3d 3e0c 1f10  ...s.......=>...
+00002650: 0610 4b09 08d4 1819 1a1b 4243 0c0c 1000  ..K.......BC....
+00002660: 1101 2709 0908 2300 0000 0000 0000 0023  ..'...#........#
+00002670: 4028 0000 0000 0000 546e 616d 6523 4030  @(......Tname#@0
+00002680: 0000 0000 0000 0900 0800 1d00 3200 4400  ............2.D.
+00002690: 4c00 6000 7200 7b00 8d00 9800 a100 b400  L.`.r.{.........
+000026a0: b600 b700 ca00 d300 e200 ef00 fb01 0001  ................
+000026b0: 0601 0b01 1301 1801 2101 2701 2d01 3701  ........!.'.-.7.
+000026c0: 3f01 4101 4401 4501 4601 4f01 5101 5301  ?.A.D.E.F.O.Q.S.
+000026d0: 5401 5501 5e01 6001 6101 6201 6b01 6d01  T.U.^.`.a.b.k.m.
+000026e0: 6e01 6f01 7801 7a01 7c01 7d01 7e01 8701  n.o.x.z.|.}.~...
+000026f0: 8901 8b01 8c01 8d01 9601 9801 9a01 9b01  ................
+00002700: 9c01 a501 a701 a901 aa01 ab01 b401 b601  ................
+00002710: b901 ba01 bb01 bc01 c501 ce01 d301 dc00  ................
+00002720: 0000 0000 0002 0100 0000 0000 0000 4c00  ..............L.
+00002730: 0000 0000 0000 0000 0000 0000 0001 dd00  ................
+00002740: 0000 0600 6100 7300 7300 6500 7400 736d  ....a.s.s.e.t.sm
+00002750: 6f44 4462 6c6f 6200 0000 08cf 958c e8d0  oDDblob.........
+00002760: e1c4 4100 0000 0600 6100 7300 7300 6500  ..A.....a.s.s.e.
+00002770: 7400 736d 6f64 4462 6c6f 6200 0000 08cf  t.smodDblob.....
+00002780: 958c e8d0 e1c4 4100 0000 0600 6100 7300  ......A.....a.s.
+00002790: 7300 6500 7400 7370 6831 5363 6f6d 7000  s.e.t.sph1Scomp.
+000027a0: 0000 0000 8190 0000 0000 0600 6100 7300  ............a.s.
+000027b0: 7300 6500 7400 7376 5372 6e6c 6f6e 6700  s.e.t.svSrnlong.
+000027c0: 0000 0100 0000 1400 6200 6100 7400 6300  ........b.a.t.c.
+000027d0: 6800 5f00 7000 7200 6f00 6300 6500 7300  h._.p.r.o.c.e.s.
+000027e0: 7300 5f00 7600 6900 6400 6500 6f00 7362  s._.v.i.d.e.o.sb
+000027f0: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
+00002800: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
+00002810: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00002820: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
+00002830: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+00002840: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+00002850: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+00002860: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+00002870: 6562 6172 0808 0908 095f 1019 7b7b 3130  ebar....._..{{10
+00002880: 3632 2c20 3337 337d 2c20 7b37 3730 2c20  62, 373}, {770, 
+00002890: 3433 367d 7d09 0817 2531 3d49 606d 797a  436}}...%1=I`myz
+000028a0: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
+000028b0: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
+000028c0: 0000 0000 9b00 0000 1400 6200 6100 7400  ..........b.a.t.
+000028d0: 6300 6800 5f00 7000 7200 6f00 6300 6500  c.h._.p.r.o.c.e.
+000028e0: 7300 7300 5f00 7600 6900 6400 6500 6f00  s.s._.v.i.d.e.o.
+000028f0: 736c 6731 5363 6f6d 7000 0000 0000 017e  slg1Scomp......~
+00002900: 5700 0000 1400 6200 6100 7400 6300 6800  W.....b.a.t.c.h.
+00002910: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+00002920: 5f00 7600 6900 6400 6500 6f00 736c 7376  _.v.i.d.e.o.slsv
+00002930: 4362 6c6f 6200 0003 0762 706c 6973 7430  Cblob....bplist0
+00002940: 30d8 0102 0304 0506 0708 090a 0b19 5657  0.............VW
+00002950: 0a59 5869 636f 6e53 697a 655f 100f 7368  .YXiconSize_..sh
+00002960: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00002970: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00002980: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+00002990: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+000029a0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000029b0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+000029c0: 7273 696f 6e23 4030 0000 0000 0000 09ae  rsion#@0........
+000029d0: 0c15 1d22 262b 3035 3a3f 4448 4d51 d40d  ..."&+05:?DHMQ..
+000029e0: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
+000029f0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
+00002a00: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
+00002a10: 032a 0909 d416 1718 0d19 1a19 1c57 7669  .*...........Wvi
+00002a20: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
+00002a30: 6e64 696e 6708 1023 0858 7562 6971 7569  nding..#.Xubiqui
+00002a40: 7479 d40d 0e0f 101e 1f19 0a5c 6461 7465  ty.........\date
+00002a50: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
+00002a60: 1023 1f19 195b 6461 7465 4372 6561 7465  .#...[dateCreate
+00002a70: 6408 08d4 0d0e 0f10 2728 190a 5473 697a  d.......'(..Tsiz
+00002a80: 6510 6108 09d4 0d0e 0f10 2c2d 0a0a 546b  e.a.......,-..Tk
+00002a90: 696e 6410 7309 09d4 0d0e 0f10 3132 0a19  ind.s.......12..
+00002aa0: 556c 6162 656c 1064 0908 d40d 0e0f 1036  Ulabel.d.......6
+00002ab0: 370a 1957 7665 7273 696f 6e10 4b09 08d4  7..Wversion.K...
+00002ac0: 0d0e 0f10 3b3c 0a19 5863 6f6d 6d65 6e74  ....;<..Xcomment
+00002ad0: 7311 012c 0908 d40d 0e0f 1040 4119 195e  s..,.......@A..^
+00002ae0: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
+00002af0: 0808 d416 1718 0d19 1f19 4708 0859 6461  ..........G..Yda
+00002b00: 7465 4164 6465 64d4 0d17 1816 494a 1919  teAdded.....IJ..
+00002b10: 5a73 6861 7265 4f77 6e65 7210 d208 08d4  ZshareOwner.....
+00002b20: 0d17 1816 4e4a 1919 5f10 0f73 6861 7265  ....NJ.._..share
+00002b30: 4c61 7374 4564 6974 6f72 0808 d40d 1718  LastEditor......
+00002b40: 1652 4a19 195f 1010 696e 7669 7461 7469  .RJ.._..invitati
+00002b50: 6f6e 5374 6174 7573 0808 0823 4028 0000  onStatus...#@(..
+00002b60: 0000 0000 546e 616d 6509 1001 0008 0019  ....Tname.......
+00002b70: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
+00002b80: 0095 0096 00a5 00ae 00b9 00bf 00c9 00d1  ................
+00002b90: 00d6 00d9 00da 00db 00e4 00ec 00f2 00fc  ................
+00002ba0: 00fd 00ff 0100 0109 0112 011f 0121 0122  .............!."
+00002bb0: 0123 012c 0138 0139 013a 0143 0148 014a  .#.,.8.9.:.C.H.J
+00002bc0: 014b 014c 0155 015a 015c 015d 015e 0167  .K.L.U.Z.\.].^.g
+00002bd0: 016d 016f 0170 0171 017a 0182 0184 0185  .m.o.p.q.z......
+00002be0: 0186 018f 0198 019b 019c 019d 01a6 01b5  ................
+00002bf0: 01b7 01b8 01b9 01c2 01c3 01c4 01ce 01d7  ................
+00002c00: 01e2 01e4 01e5 01e6 01ef 0201 0202 0203  ................
+00002c10: 020c 021f 0220 0221 0222 022b 0230 0231  ..... .!.".+.0.1
+00002c20: 0000 0000 0000 0201 0000 0000 0000 005a  ...............Z
+00002c30: 0000 0000 0000 0000 0000 0000 0000 0233  ...............3
+00002c40: 0000 0014 0062 0061 0074 0063 0068 005f  .....b.a.t.c.h._
+00002c50: 0070 0072 006f 0063 0065 0073 0073 005f  .p.r.o.c.e.s.s._
+00002c60: 0076 0069 0064 0065 006f 0073 6c73 7670  .v.i.d.e.o.slsvp
+00002c70: 626c 6f62 0000 025e 6270 6c69 7374 3030  blob...^bplist00
+00002c80: d801 0203 0405 0607 0809 0a0b 1a46 470a  .............FG.
+00002c90: 3558 6963 6f6e 5369 7a65 5f10 0f73 686f  5XiconSize_..sho
+00002ca0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+00002cb0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+00002cc0: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
+00002cd0: 655a 736f 7274 436f 6c75 6d6e 5f10 1075  eZsortColumn_..u
+00002ce0: 7365 5265 6c61 7469 7665 4461 7465 735f  seRelativeDates_
+00002cf0: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+00002d00: 7369 6f6e 2340 3000 0000 0000 0009 d90c  sion#@0.........
+00002d10: 0d0e 0f10 1112 1314 151e 2328 2d32 363b  ..........#(-26;
+00002d20: 4058 636f 6d6d 656e 7473 556c 6162 656c  @XcommentsUlabel
+00002d30: 5776 6572 7369 6f6e 5b64 6174 6543 7265  Wversion[dateCre
+00002d40: 6174 6564 5473 697a 655c 6461 7465 4d6f  atedTsize\dateMo
+00002d50: 6469 6669 6564 546b 696e 6454 6e61 6d65  difiedTkindTname
+00002d60: 5e64 6174 654c 6173 744f 7065 6e65 64d4  ^dateLastOpened.
+00002d70: 1617 1819 1a1b 0a1d 5776 6973 6962 6c65  ........Wvisible
+00002d80: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00002d90: 5569 6e64 6578 0811 012c 0910 07d4 1617  Uindex...,......
+00002da0: 1819 1a20 0a22 0810 6409 1005 d416 1718  ... ."..d.......
+00002db0: 191a 250a 2708 104b 0910 06d4 1617 1819  ..%.'..K........
+00002dc0: 1a2a 1a2c 0810 b508 1002 d416 1718 190a  .*.,............
+00002dd0: 2f1a 3109 1061 0810 03d4 1617 1819 0a2a  /.1..a.........*
+00002de0: 1a35 0908 1001 d416 1718 190a 380a 3a09  .5..........8.:.
+00002df0: 1073 0910 04d4 1617 1819 0a3d 0a3f 0911  .s.........=.?..
+00002e00: 032a 0910 00d4 1617 1819 1a42 1a44 0810  .*.........B.D..
+00002e10: c808 1008 0823 4028 0000 0000 0000 546e  .....#@(......Tn
+00002e20: 616d 6509 0008 0019 0022 0034 003c 0050  ame......".4.<.P
+00002e30: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
+00002e40: 00b8 00c0 00cc 00d1 00de 00e3 00e8 00f7  ................
+00002e50: 0100 0108 010e 0118 011e 011f 0122 0123  .............".#
+00002e60: 0125 012e 012f 0131 0132 0134 013d 013e  .%.../.1.2.4.=.>
+00002e70: 0140 0141 0143 014c 014d 014f 0150 0152  .@.A.C.L.M.O.P.R
+00002e80: 015b 015c 015e 015f 0161 016a 016b 016c  .[.\.^._.a.j.k.l
+00002e90: 016e 0177 0178 017a 017b 017d 0186 0187  .n.w.x.z.{.}....
+00002ea0: 018a 018b 018d 0196 0197 0199 019a 019c  ................
+00002eb0: 019d 01a6 01ab 0000 0000 0000 0201 0000  ................
+00002ec0: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+00002ed0: 0000 0000 01ac 0000 0014 0062 0061 0074  ...........b.a.t
+00002ee0: 0063 0068 005f 0070 0072 006f 0063 0065  .c.h._.p.r.o.c.e
+00002ef0: 0073 0073 005f 0076 0069 0064 0065 006f  .s.s._.v.i.d.e.o
+00002f00: 0073 6d6f 4444 626c 6f62 0000 0008 f203  .smoDDblob......
+00002f10: dcf3 ebf6 c441 0000 0014 0062 0061 0074  .....A.....b.a.t
+00002f20: 0063 0068 005f 0070 0072 006f 0063 0065  .c.h._.p.r.o.c.e
+00002f30: 0073 0073 005f 0076 0069 0064 0065 006f  .s.s._.v.i.d.e.o
+00002f40: 0073 6d6f 6444 626c 6f62 0000 0008 4b60  .smodDblob....K`
+00002f50: d4fa 99f1 c441 0000 0014 0062 0061 0074  .....A.....b.a.t
+00002f60: 0063 0068 005f 0070 0072 006f 0063 0065  .c.h._.p.r.o.c.e
+00002f70: 0073 0073 005f 0076 0069 0064 0065 006f  .s.s._.v.i.d.e.o
+00002f80: 0073 7068 3153 636f 6d70 0000 0000 0001  .sph1Scomp......
+00002f90: f000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003000: 0000 0000 0000 0000 0000 0019 0000 000c  ................
@@ -965,15 +965,15 @@
 00003c40: 0000 0000 0000 0000 0000 0000 0000 9900  ................
 00003c50: 0000 1200 6600 6500 6100 7400 7500 7200  ....f.e.a.t.u.r.
 00003c60: 6500 5f00 6500 7800 7400 7200 6100 6300  e._.e.x.t.r.a.c.
 00003c70: 7400 6f00 7200 7364 7363 6c62 6f6f 6c00  t.o.r.sdsclbool.
 00003c80: 0000 0012 0066 0065 0061 0074 0075 0072  .....f.e.a.t.u.r
 00003c90: 0065 005f 0065 0078 0074 0072 0061 0063  .e._.e.x.t.r.a.c
 00003ca0: 0074 006f 0072 0073 6c67 3153 636f 6d70  .t.o.r.slg1Scomp
-00003cb0: 0000 0000 0012 6893 0000 0012 0066 0065  ......h......f.e
+00003cb0: 0000 0000 0012 d944 0000 0012 0066 0065  .......D.....f.e
 00003cc0: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
 00003cd0: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
 00003ce0: 6c73 7643 626c 6f62 0000 02b8 6270 6c69  lsvCblob....bpli
 00003cf0: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
 00003d00: 0c0d 1a48 4948 4a4b 0c5f 1012 7669 6577  ...HIHJK._..view
 00003d10: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
 00003d20: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
@@ -1025,19 +1025,19 @@
 00004000: 0000 0000 0000 0000 0000 0015 0000 0012  ................
 00004010: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 00004020: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 00004030: 0072 0073 6d6f 4444 626c 6f62 0000 0008  .r.smoDDblob....
 00004040: e84a b14c eaf6 c441 0000 0012 0066 0065  .J.L...A.....f.e
 00004050: 0061 0074 0075 0072 0065 005f 0065 0078  .a.t.u.r.e._.e.x
 00004060: 0074 0072 0061 0063 0074 006f 0072 0073  .t.r.a.c.t.o.r.s
-00004070: 6d6f 6444 626c 6f62 0000 0008 ae8b 457c  modDblob......E|
-00004080: 94f5 c441 0000 0012 0066 0065 0061 0074  ...A.....f.e.a.t
+00004070: 6d6f 6444 626c 6f62 0000 0008 e84a b14c  modDblob.....J.L
+00004080: eaf6 c441 0000 0012 0066 0065 0061 0074  ...A.....f.e.a.t
 00004090: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
 000040a0: 0061 0063 0074 006f 0072 0073 7068 3153  .a.c.t.o.r.sph1S
-000040b0: 636f 6d70 0000 0000 0014 d000 0000 0012  comp............
+000040b0: 636f 6d70 0000 0000 0015 5000 0000 0012  comp......P.....
 000040c0: 0066 0065 0061 0074 0075 0072 0065 005f  .f.e.a.t.u.r.e._
 000040d0: 0065 0078 0074 0072 0061 0063 0074 006f  .e.x.t.r.a.c.t.o
 000040e0: 0072 0073 7653 726e 6c6f 6e67 0000 0001  .r.svSrnlong....
 000040f0: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
 00004100: 6277 7370 626c 6f62 0000 00c9 6270 6c69  bwspblob....bpli
 00004110: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
 00004120: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
@@ -1049,17 +1049,17 @@
 00004180: 6465 6261 7208 0809 0809 5f10 187b 7b33  debar....._..{{3
 00004190: 3934 2c20 3138 317d 2c20 7b37 3730 2c20  94, 181}, {770, 
 000041a0: 3433 367d 7d09 0817 2531 3d49 606d 797a  436}}...%1=I`myz
 000041b0: 7b7c 7d7e 9900 0000 0000 0001 0100 0000  {|}~............
 000041c0: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
 000041d0: 0000 0000 9a00 0000 0600 6d00 6900 7800  ..........m.i.x.
 000041e0: 6900 6e00 736c 6731 5363 6f6d 7000 0000  i.n.slg1Scomp...
-000041f0: 0000 01b8 da00 0000 0600 6d00 6900 7800  ..........m.i.x.
+000041f0: 0000 01b9 c300 0000 0600 6d00 6900 7800  ..........m.i.x.
 00004200: 6900 6e00 736d 6f44 4462 6c6f 6200 0000  i.n.smoDDblob...
-00004210: 0821 b3af 405b f8c4 4100 0000 0600 6d00  .!..@[..A.....m.
+00004210: 08a5 671d 440a fac4 4100 0000 0600 6d00  ..g.D...A.....m.
 00004220: 6900 7800 6900 6e00 736d 6f64 4462 6c6f  i.x.i.n.smodDblo
 00004230: 6200 0000 0821 b3af 405b f8c4 4100 0000  b....!..@[..A...
 00004240: 0600 6d00 6900 7800 6900 6e00 7370 6831  ..m.i.x.i.n.sph1
 00004250: 5363 6f6d 7000 0000 0000 0210 0000 0000  Scomp...........
 00004260: 0600 6d00 6900 7800 6900 6e00 7376 5372  ..m.i.x.i.n.svSr
 00004270: 6e6c 6f6e 6700 0000 0100 0000 0d00 6f00  nlong.........o.
 00004280: 7500 7400 6c00 6900 6500 7200 5f00 7400  u.t.l.i.e.r._.t.
@@ -1193,15 +1193,15 @@
 00004a80: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
 00004a90: 3135 392c 2031 3233 7d2c 207b 3130 3736  159, 123}, {1076
 00004aa0: 2c20 3632 317d 7d09 0817 2531 3d49 606d  , 621}}...%1=I`m
 00004ab0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
 00004ac0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
 00004ad0: 0000 0000 0000 9b00 0000 0800 7000 6c00  ............p.l.
 00004ae0: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00004af0: 6f6d 7000 0000 0000 0a1b 6500 0000 0800  omp.......e.....
+00004af0: 6f6d 7000 0000 0000 0a1f d300 0000 0800  omp.............
 00004b00: 7000 6c00 6f00 7400 7400 6900 6e00 676c  p.l.o.t.t.i.n.gl
 00004b10: 7376 4362 6c6f 6200 0002 bb62 706c 6973  svCblob....bplis
 00004b20: 7430 30da 0102 0304 0506 0708 090a 0b0c  t00.............
 00004b30: 0d1a 4849 4a4b 4c0c 5f10 1276 6965 774f  ..HIJKL._..viewO
 00004b40: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
 00004b50: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 00004b60: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
@@ -1276,16 +1276,16 @@
 00004fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005000: 0000 0000 0000 0000 0000 0014 0000 0008  ................
 00005010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-00005020: 6d6f 4444 626c 6f62 0000 0008 7b27 5505  moDDblob....{'U.
-00005030: 1cf8 c441 0000 0008 0070 006c 006f 0074  ...A.....p.l.o.t
+00005020: 6d6f 4444 626c 6f62 0000 0008 34e5 9d60  moDDblob....4..`
+00005030: 16fa c441 0000 0008 0070 006c 006f 0074  ...A.....p.l.o.t
 00005040: 0074 0069 006e 0067 6d6f 6444 626c 6f62  .t.i.n.gmodDblob
 00005050: 0000 0008 65be f96a 3ef2 c441 0000 0008  ....e..j>..A....
 00005060: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
 00005070: 7068 3153 636f 6d70 0000 0000 000c 4000  ph1Scomp......@.
 00005080: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
 00005090: 006e 0067 7653 726e 6c6f 6e67 0000 0001  .n.gvSrnlong....
 000050a0: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
```

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/extract_features_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.57.3/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/requirements.txt` & `Simba-UW-tf-dev-1.57.3/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/severity_processor.py` & `Simba-UW-tf-dev-1.57.3/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.57.3/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.57.3/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.57.3/simba/mixins/config_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from simba.read_config_unit_tests import (read_config_file,
                                           read_project_path_and_file_type,
                                           read_config_entry)
 from simba.feature_extractors.unit_tests import read_video_info_csv
 from simba.drop_bp_cords import createColorListofList
-from simba.misc_tools import SimbaTimer, find_core_cnt, check_multi_animal_status
+from simba.misc_tools import SimbaTimer, find_core_cnt, check_multi_animal_status, get_color_dict
 from simba.train_model_functions import get_all_clf_names
 from simba.drop_bp_cords import getBpNames, create_body_part_dictionary, getBpHeaders
 from simba.utils.errors import NoROIDataError
 from simba.utils.lookups import get_emojis
 import os, glob
 import pandas as pd
 import itertools
@@ -66,14 +66,15 @@
         self.x_cols, self.y_cols, self.p_cols = getBpNames(config_path)
         self.column_headers = getBpHeaders(config_path)
         self.multiprocess_chunksize = Defaults.CHUNK_SIZE.value
         self.maxtasksperchild = Defaults.MAX_TASK_PER_CHILD.value
         self.clr_lst = createColorListofList(self.animal_cnt, int(len(self.x_cols)/self.animal_cnt) + 1)
         self.animal_bp_dict = create_body_part_dictionary(self.multi_animal_status, self.multi_animal_id_list, self.animal_cnt, self.x_cols, self.y_cols, self.p_cols, [])
         self.project_bps = list(set([x[:-2] for x in self.column_headers]))
+        self.color_dict = get_color_dict()
         self.emojis = get_emojis()
         if read_video_info:
             self.video_info_df = read_video_info_csv(os.path.join(self.project_path, Paths.VIDEO_INFO.value))
 
     def read_roi_data(self):
         """
         Method to read in ROI definitions from SimBA project
```

### Comparing `Simba-UW-tf-dev-1.57.2/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.57.3/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.57.3/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.57.3/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.57.3/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.57.3/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.57.3/simba/FSTTC_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.57.3/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/video_info_table.py` & `Simba-UW-tf-dev-1.57.3/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.57.3/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.57.3/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.57.3/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/utils/errors.py` & `Simba-UW-tf-dev-1.57.3/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/utils/printing.py` & `Simba-UW-tf-dev-1.57.3/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.57.3/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.3/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.57.3/simba/train_model_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.57.3/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.57.3/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.57.3/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/movement_processor.py` & `Simba-UW-tf-dev-1.57.3/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pybursts.py` & `Simba-UW-tf-dev-1.57.3/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.57.3/simba/rw_dfs.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.57.3/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.57.3/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.57.3/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.57.3/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/setting_menu.py` & `Simba-UW-tf-dev-1.57.3/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.57.3/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/run_inference.py` & `Simba-UW-tf-dev-1.57.3/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/misc_visualizations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/path_plotter_mp.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,43 +105,42 @@
 
     Notes
     ----------
     `Visualization tutorials <https://github.com/sgoldenlab/simba/blob/master/docs/tutorial.md#step-11-visualizations>`__.
 
     Examples
     ----------
-    >>> style_attr = {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': 'White', 'max lines': 100}
+    >>> input_style_attr = {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': 'White', 'max lines': 100}
     >>> animal_attr = {0: ['Ear_right_1', 'Red']}
-    >>> clf_attr = {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Red', 'Size: 30']}
+    >>> input_clf_attr = {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Red', 'Size: 30']}
     >>> path_plotter = PathPlotterMulticore(config_path=r'MyConfigPath', frame_setting=False, video_setting=True, style_attr=style_attr, animal_attr=animal_attr, files_found=['project_folder/csv/machine_results/MyVideo.csv'], cores=5, clf_attr=clf_attr)
     >>> path_plotter.create_path_plots()
     """
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
                  last_frame: bool,
                  files_found: list,
-                 style_attr: dict or None,
+                 input_style_attr: dict or None,
                  animal_attr: dict,
-                 clf_attr: dict or None,
+                 input_clf_attr: dict or None,
                  cores: int):
 
         if platform.system() == "Darwin":
             multiprocessing.set_start_method('spawn', force=True)
 
         super().__init__(config_path=config_path)
-        self.video_setting, self.frame_setting, self.style_attr, self.files_found, self.animal_attr, self.clf_attr, self.last_frame, self.cores = video_setting, frame_setting, style_attr, files_found, animal_attr, clf_attr, last_frame, cores
+        self.video_setting, self.frame_setting, self.input_style_attr, self.files_found, self.animal_attr, self.input_clf_attr, self.last_frame, self.cores = video_setting, frame_setting, input_style_attr, files_found, animal_attr, input_clf_attr, last_frame, cores
         if (not frame_setting) and (not video_setting) and (not last_frame):
             raise NoSpecifiedOutputError(msg='SIMBA ERROR: Please choice to create path frames and/or video path plots')
         self.no_animals_path_plot = len(animal_attr.keys())
         if not os.path.exists(self.path_plot_dir): os.makedirs(self.path_plot_dir)
-        check_if_filepath_list_is_empty(filepaths=self.files_found,
-                                        error_msg='SIMBA ERROR: Zero files found in the project_folder/csv/machine_results directory. To plot paths without performing machine classifications, use path plotter functions in [ROI] tab.')
+        check_if_filepath_list_is_empty(filepaths=self.files_found, error_msg='SIMBA ERROR: Zero files found in the project_folder/csv/machine_results directory. To plot paths without performing machine classifications, use path plotter functions in [ROI] tab.')
         print(f'Processing {str(len(self.files_found))} videos...')
 
     def create_path_plots(self):
         """
         Method to create path plot videos and/or frames.Results are store in the
         'project_folder/frames/path_plots' directory of the SimBA project.
         """
@@ -162,16 +161,17 @@
                 self.video_folder = os.path.join(self.path_plot_dir, self.video_name)
                 if os.path.exists(self.temp_folder):
                     remove_a_folder(self.temp_folder)
                     remove_a_folder(self.video_folder)
                 os.makedirs(self.temp_folder)
                 self.save_video_path = os.path.join(self.path_plot_dir, self.video_name + '.mp4')
 
-            if self.clf_attr:
+            if self.input_clf_attr:
                 clf_names = []
+                self.clf_attr = {}
                 for v in self.clf_attr.values():
                     clf_names.append(v[0])
 
             if self.last_frame:
                 self.__get_deque_lookups()
                 _ = make_path_plot(data_df=self.data_df,
                                    video_info=self.video_info,
@@ -195,15 +195,15 @@
                 data_arr = self.__split_array_into_max_lines(data=data_arr, max_lines=self.style_attr['max lines'])
                 data_arr = np.array_split(data_arr, self.cores)
                 data = []
                 for cnt, i in enumerate(data_arr):
                     data.append(self.__insert_group_idx_column(data=i, group=cnt))
                 frm_per_core = data[0].shape[0]
 
-                print('Creating gantt, multiprocessing (chunksize: {}, cores: {})...'.format(str(self.multiprocess_chunksize), str(self.cores)))
+                print('Creating path plots, multiprocessing (chunksize: {}, cores: {})...'.format(str(self.multiprocess_chunksize), str(self.cores)))
                 with multiprocessing.Pool(self.cores, maxtasksperchild=self.maxtasksperchild) as pool:
                     constants = functools.partial(_image_creator,
                                                   video_setting=self.video_setting,
                                                   video_name=self.video_name,
                                                   frame_setting=self.frame_setting,
                                                   video_save_dir=self.temp_folder,
                                                   frame_folder_dir=self.save_frame_folder_dir,
@@ -256,24 +256,27 @@
         results = np.full((data.shape[0], data.shape[1], data.shape[2] + 1), np.nan)
         group_col = np.full((data.shape[1], 1), group)
         for frm_idx in prange(data.shape[0]):
             results[frm_idx] = np.hstack((group_col, data[frm_idx]))
         return results
 
     def __get_styles(self):
-        self.color_dict = get_color_dict()
-        if self.style_attr is not None:
-            self.style_attr['bg color'] = self.color_dict[self.style_attr['bg color']]
-            self.style_attr['max lines'] = int(self.style_attr['max lines'] * (int(self.video_info['fps'].values[0]) / 1000))
-            if self.style_attr['width'] == 'As input':
+        self.style_attr = {}
+        if self.input_style_attr is not None:
+            self.style_attr['bg color'] = self.color_dict[self.input_style_attr['bg color']]
+            self.style_attr['max lines'] = int(self.input_style_attr['max lines'] * (int(self.video_info['fps'].values[0]) / 1000))
+            self.style_attr['font thickness'] = self.input_style_attr['font thickness']
+            self.style_attr['line width'] = self.input_style_attr['line width']
+            self.style_attr['font size'] = self.input_style_attr['font size']
+            self.style_attr['circle size'] = self.input_style_attr['circle size']
+            if self.input_style_attr['width'] == 'As input':
                 self.style_attr['width'], self.style_attr['height'] = int(self.video_info['Resolution_width'].values[0]), int(self.video_info['Resolution_height'].values[0])
             else:
                 pass
         else:
-            self.style_attr = {}
             space_scaler, radius_scaler, res_scaler, font_scaler = 25, 10, 1500, 0.8
             self.style_attr['width'] = int(self.video_info['Resolution_width'].values[0])
             self.style_attr['height'] = int(self.video_info['Resolution_height'].values[0])
             max_res = max(self.style_attr['width'], self.style_attr['height'])
             self.style_attr['circle size'] = int(radius_scaler / (res_scaler / max_res))
             self.style_attr['font size'] = int(font_scaler / (res_scaler / max_res))
             self.style_attr['bg color'] = self.color_dict['White']
@@ -300,23 +303,24 @@
 
 # style_attr = {'width': 'As input', 'height': 'As input', 'line width': 5, 'font size': 5, 'font thickness': 2, 'circle size': 5, 'bg color': 'White', 'max lines': 1000}
 # animal_attr = {0: ['Ear_right_1', 'Red'], 1: ['Ear_right_2', 'Lime']}
 # clf_attr = {0: ['Attack', 'Black', 'Size: 30'], 1: ['Sniffing', 'Red', 'Size: 30']}
 
 # clf_attr = None
 # style_attr = None
-#
-# path_plotter = PathPlotterMulticore(config_path='/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/project_config.ini',
+
+# path_plotter = PathPlotterMulticore(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini',
 #                                     frame_setting=False,
 #                                     video_setting=True,
-#                                     last_frame=True,
-#                                     clf_attr=clf_attr,
-#                                     style_attr=style_attr,
+#                                     last_frame=False,
+#                                     input_clf_attr=clf_attr,
+#                                     input_style_attr=style_attr,
 #                                     animal_attr=animal_attr,
-#                                     files_found=['/Users/simon/Desktop/envs/troubleshooting/two_animals_16bp_032023/project_folder/csv/targets_inserted/Together_1.csv'],
+#                                     files_found=['/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/targets_inserted/Together_1.csv',
+#                                                  '/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/csv/targets_inserted/Together_2.csv'],
 #                                     cores=5)
 # path_plotter.create_path_plots()
 
 # path_plotter = PathPlotterMulticore(config_path='/Users/simon/Desktop/envs/simba_dev/tests/test_data/two_C57_madlc/project_folder/project_config.ini',
 #                                     frame_setting=False,
 #                                     video_setting=True,
 #                                     last_frame=True,
```

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/path_plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,20 +56,20 @@
 
     def __init__(self,
                  config_path: str,
                  frame_setting: bool,
                  video_setting: bool,
                  last_frame: bool,
                  files_found: list,
-                 style_attr: dict,
+                 input_style_attr: dict,
                  animal_attr: dict,
-                 clf_attr: dict):
+                 input_clf_attr: dict):
 
         super().__init__(config_path=config_path)
-        self.video_setting, self.frame_setting, self.style_attr, self.files_found, self.animal_attr, self.clf_attr, self.last_frame = video_setting, frame_setting, style_attr, files_found, animal_attr, clf_attr, last_frame
+        self.video_setting, self.frame_setting, self.input_style_attr, self.files_found, self.animal_attr, self.input_clf_attr, self.last_frame = video_setting, frame_setting, input_style_attr, files_found, animal_attr, input_clf_attr, last_frame
         if (not frame_setting) and (not video_setting) and (not last_frame):
             raise NoSpecifiedOutputError(msg='SIMBA ERROR: Please choice to create path frames and/or video path plots')
 
         self.no_animals_path_plot = len(animal_attr.keys())
         if not os.path.exists(self.path_plot_dir): os.makedirs(self.path_plot_dir)
         self.font = Formats.FONT.value
         check_if_filepath_list_is_empty(filepaths=self.files_found,
@@ -96,16 +96,17 @@
                 self.writer = cv2.VideoWriter(self.video_save_path, self.fourcc, self.fps, (self.style_attr['width'], self.style_attr['height']))
 
             if self.frame_setting:
                 self.save_video_folder = os.path.join(self.path_plot_dir, self.video_name)
                 if not os.path.exists(self.save_video_folder):
                     os.makedirs(self.save_video_folder)
 
-            if self.clf_attr:
+            if self.input_clf_attr:
                 clf_names = []
+                self.clf_attr = {}
                 for v in self.clf_attr.values():
                     clf_names.append(v[0])
                 clf_df = self.data_df[clf_names]
 
             if self.last_frame:
                 _ = make_path_plot(data_df=self.data_df,
                                    video_info=self.video_info,
@@ -158,24 +159,27 @@
                 video_timer.stop_timer()
                 print('Path visualization for video {} saved (elapsed time {}s)...'.format(self.video_name, video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
         stdout_success(msg=f'Path visualizations for {str(len(self.files_found))} videos saved in project_folder/frames/output/path_plots directory', elapsed_time=self.timer.elapsed_time_str)
 
     def __get_styles(self):
-        self.color_dict = get_color_dict()
-        if self.style_attr is not None:
-            self.style_attr['bg color'] = self.color_dict[self.style_attr['bg color']]
-            self.style_attr['max lines'] = int(self.style_attr['max lines'] * (int(self.video_info['fps'].values[0]) / 1000))
-            if self.style_attr['width'] == 'As input':
+        self.style_attr = {}
+        if self.input_style_attr is not None:
+            self.style_attr['bg color'] = self.color_dict[self.input_style_attr['bg color']]
+            self.style_attr['max lines'] = int(self.input_style_attr['max lines'] * (int(self.video_info['fps'].values[0]) / 1000))
+            self.style_attr['font thickness'] = self.input_style_attr['font thickness']
+            self.style_attr['line width'] = self.input_style_attr['line width']
+            self.style_attr['font size'] = self.input_style_attr['font size']
+            self.style_attr['circle size'] = self.input_style_attr['circle size']
+            if self.input_style_attr['width'] == 'As input':
                 self.style_attr['width'], self.style_attr['height'] = int(self.video_info['Resolution_width'].values[0]), int(self.video_info['Resolution_height'].values[0])
             else:
                 pass
         else:
-            self.style_attr = {}
             space_scaler, radius_scaler, res_scaler, font_scaler = 25, 10, 1500, 0.8
             self.style_attr['width'] = int(self.video_info['Resolution_width'].values[0])
             self.style_attr['height'] = int(self.video_info['Resolution_height'].values[0])
             max_res = max(self.style_attr['width'], self.style_attr['height'])
             self.style_attr['circle size'] = int(radius_scaler / (res_scaler / max_res))
             self.style_attr['font size'] = int(font_scaler / (res_scaler / max_res))
             self.style_attr['bg color'] = self.color_dict['White']
```

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.57.3/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.57.3/simba/interpolate_smooth_post_hoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/dash_app.py` & `Simba-UW-tf-dev-1.57.3/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.57.3/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.57.3/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.57.3/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/misc_tools.py` & `Simba-UW-tf-dev-1.57.3/simba/misc_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.3/simba/pop_up_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
                               get_color_dict,
                               find_all_videos_in_directory,
                               get_file_name_info_in_directory,
                               SimbaTimer,
                               find_files_of_filetypes_in_directory,
                               archive_processed_files,
                               copy_img_folder,
-                              str_2_bool)
+                              str_2_bool,
+                              concatenate_videos_in_folder)
 from simba.utils.printing import stdout_success, stdout_trash
 from simba.drop_bp_cords import get_fn_ext
 from simba.utils.lookups import get_third_party_appender_file_formats
 from simba.third_party_label_appenders.third_party_appender import ThirdPartyLabelAppender
 from simba.plotting.ROI_feature_visualizer import ROIfeatureVisualizer
 from simba.get_coordinates_tools_v2 import get_coordinates_nilsson
 from simba.roi_tools.ROI_clf_calculator import ROIClfCalculator
@@ -2415,26 +2416,26 @@
 
         if not self.multiprocessing_var.get():
             path_plotter = PathPlotterSingleCore(config_path=self.config_path,
                                                  frame_setting=self.path_frames_var.get(),
                                                  video_setting=self.path_videos_var.get(),
                                                  last_frame=self.path_last_frm_var.get(),
                                                  files_found=data_paths,
-                                                 style_attr=style_attr,
+                                                 input_style_attr=style_attr,
                                                  animal_attr=animal_attr,
-                                                 clf_attr=clf_attr)
+                                                 input_clf_attr=clf_attr)
         else:
             path_plotter = PathPlotterMulticore(config_path=self.config_path,
                                                 frame_setting=self.path_frames_var.get(),
                                                 video_setting=self.path_videos_var.get(),
                                                 last_frame=self.path_last_frm_var.get(),
                                                 files_found=data_paths,
-                                                style_attr=style_attr,
+                                                input_style_attr=style_attr,
                                                 animal_attr=animal_attr,
-                                                clf_attr=clf_attr,
+                                                input_clf_attr=clf_attr,
                                                 cores=int(self.multiprocess_dropdown.getChoices()))
 
         path_plotter.create_path_plots()
 
 #_ = PathPlotPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/Two_animals_16bps/project_folder/project_config.ini')
 
 class DistancePlotterPopUp(PopUpMixin):
@@ -3627,15 +3628,14 @@
                                                                          create_gantt=self.gantt_dropdown.getChoices())
         validation_video_creator.run()
 
 
 class VideoRotatorPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='ROTATE VIDEOS')
-
         self.save_dir_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SAVE LOCATION', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
         self.save_dir = FolderSelect(self.save_dir_frm, 'Save directory:', lblwidth=20)
 
         self.rotate_dir_frm = LabelFrame(self.main_frm, text='ROTATE VIDEOS IN DIRECTORY', font=Formats.LABELFRAME_HEADER_FORMAT.value)
         self.input_dir = FolderSelect(self.rotate_dir_frm, 'Video directory:', lblwidth=20)
         self.run_dir = Button(self.rotate_dir_frm, text='RUN', fg='blue', command=lambda: self.run(input_path=self.input_dir.folder_path,
                                                                                                    output_path=self.save_dir.folder_path))
@@ -3652,21 +3652,46 @@
         self.input_dir.grid(row=0, column=0, sticky=NW)
         self.run_dir.grid(row=1, column=0, sticky=NW)
 
         self.rotate_video_frm.grid(row=2, column=0, sticky=NW)
         self.input_file.grid(row=0, column=0, sticky=NW)
         self.run_file.grid(row=1, column=0, sticky=NW)
 
-
     def run(self, input_path: str, output_path: str):
         check_if_dir_exists(in_dir=output_path)
         rotator = VideoRotator(input_path=input_path, output_dir=output_path)
         rotator.run()
 
 
+class VideoTemporalJoinPopUp(PopUpMixin):
+    def __init__(self):
+        super().__init__(title='ROTATE VIDEOS')
+        self.settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
+        self.input_dir = FolderSelect(self.settings_frm, 'INPUT DIRECTORY:', lblwidth=20)
+        self.file_format = DropDownMenu(self.settings_frm, 'INPUT FORMAT:', Options.VIDEO_FORMAT_OPTIONS.value, '20')
+        self.file_format.setChoices(Options.VIDEO_FORMAT_OPTIONS.value[0])
+        self.settings_frm.grid(row=0, column=0, sticky=NW)
+        self.input_dir.grid(row=0, column=0, sticky=NW)
+        self.file_format.grid(row=1, column=0, sticky=NW)
+        self.create_run_frm(run_function=self.run)
+
+    def run(self):
+        check_if_dir_exists(in_dir=self.input_dir.folder_path)
+        print(f'Concatenating videos in {self.input_dir.folder_path} directory...')
+        save_path = os.path.join(self.input_dir.folder_path, f'concatenated.mp4')
+        concatenate_videos_in_folder(in_folder=self.input_dir.folder_path,
+                                     save_path=save_path,
+                                     remove_splits=False,
+                                     video_format=self.file_format.getChoices())
+
+
+
+
+
+
 
 #_ = ValidationVideoPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
 
 
 #_ = ThirdPartyAnnotatorAppenderPopUp(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
```

### Comparing `Simba-UW-tf-dev-1.57.2/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.57.3/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.57.3/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.57.3/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/pose_reset.py` & `Simba-UW-tf-dev-1.57.3/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.57.3/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/SimBA.py` & `Simba-UW-tf-dev-1.57.3/simba/SimBA.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,16 @@
                                   SmoothingPopUp,
                                   BatchPreProcessPopUp,
                                   AppendROIFeaturesByBodyPartPopUp,
                                   ExtractAnnotationFramesPopUp,
                                   FeatureSubsetExtractorPopUp,
                                   ThirdPartyAnnotatorAppenderPopUp,
                                   ValidationVideoPopUp,
-                                  VideoRotatorPopUp)
+                                  VideoRotatorPopUp,
+                                  VideoTemporalJoinPopUp)
 from simba.bounding_box_tools.boundary_menus import BoundaryMenus
 from simba.labelling_interface import select_labelling_video
 from simba.labelling_advanced_interface import select_labelling_video_advanced
 from simba.enums import (Formats,
                          OS,
                          Defaults,
                          TagNames)
@@ -791,14 +792,15 @@
 
         video_process_menu.add_command(label='CLAHE enhance video', compound='left', image=self.menu_icons['clahe']['img'], command=CLAHEPopUp)
         video_process_menu.add_command(label='Superimpose frame numbers on video', compound='left', image=self.menu_icons['trash']['img'], command=lambda:superimpose_frame_count(file_path=askopenfilename()))
         video_process_menu.add_command(label='Convert to grayscale', compound='left', image=self.menu_icons['grey']['img'], command=lambda:video_to_greyscale(file_path=askopenfilename()))
         video_process_menu.add_command(label='Merge frames to video', compound='left', image=self.menu_icons['merge']['img'], command=MergeFrames2VideoPopUp)
         video_process_menu.add_command(label='Generate gifs', compound='left', image=self.menu_icons['gif']['img'], command=CreateGIFPopUP)
         video_process_menu.add_command(label='Rotate videos', compound='left', image=self.menu_icons['rotate']['img'], command=VideoRotatorPopUp)
+        video_process_menu.add_command(label='Temporal join videos', compound='left', image=self.menu_icons['stopwatch']['img'], command=VideoTemporalJoinPopUp)
         video_process_menu.add_command(label='Print classifier info...', compound='left', image=self.menu_icons['print']['img'], command=PrintModelInfoPopUp)
 
         extract_frames_menu = Menu(video_process_menu)
         extract_frames_menu.add_command(label='Extract defined frames',command=ExtractSpecificFramesPopUp)
         extract_frames_menu.add_command(label='Extract frames',command=ExtractAllFramesPopUp)
         extract_frames_menu.add_command(label='Extract frames from seq files', command=ExtractSEQFramesPopUp)
         video_process_menu.add_cascade(label='Extract frames...', compound='left', image=self.menu_icons['frames']['img'], menu=extract_frames_menu)
```

### Comparing `Simba-UW-tf-dev-1.57.2/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.57.3/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/assets/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -516,16 +516,16 @@
 00002030: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00002040: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00002050: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00002060: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00002070: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00002080: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00002090: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-000020a0: 0809 0809 5f10 197b 7b31 3635 302c 2033  ...._..{{1650, 3
-000020b0: 3538 7d2c 207b 3737 302c 2034 3336 7d7d  58}, {770, 436}}
+000020a0: 0809 0809 5f10 197b 7b34 3230 2c20 3131  ...._..{{420, 11
+000020b0: 337d 2c20 7b31 3031 352c 2037 3637 7d7d  3}, {1015, 767}}
 000020c0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
 000020d0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
 000020e0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
 000020f0: 0000 0005 0069 0063 006f 006e 0073 6c67  .....i.c.o.n.slg
 00002100: 3153 636f 6d70 0000 0000 0005 98d9 0000  1Scomp..........
 00002110: 0005 0069 0063 006f 006e 0073 6c73 7643  ...i.c.o.n.slsvC
 00002120: 626c 6f62 0000 02af 6270 6c69 7374 3030  blob....bplist00
```

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.57.3/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.57.3/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.57.3/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.3/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.57.3/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.57.3/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.57.3/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.57.3/simba/drop_bp_cords.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.57.3/simba/read_config_unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.57.3/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.57.3/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/train_single_model.py` & `Simba-UW-tf-dev-1.57.3/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.57.3/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.57.3/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.57.3/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.57.3/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.2
+Version: 1.57.3
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 simba/assets/icons/print.png
 simba/assets/icons/reorganize.png
 simba/assets/icons/restart.png
 simba/assets/icons/roi.png
 simba/assets/icons/rotate.png
 simba/assets/icons/sample.png
 simba/assets/icons/settings.png
+simba/assets/icons/stopwatch.png
 simba/assets/icons/superimpose.png
 simba/assets/icons/trash.png
 simba/assets/icons/video.png
 simba/assets/icons/visualize.png
 simba/assets/icons/concat_icons/horizontal.png
 simba/assets/icons/concat_icons/mixed_mosaic.png
 simba/assets/icons/concat_icons/mosaic.png
```

### Comparing `Simba-UW-tf-dev-1.57.2/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/LICENSE.md` & `Simba-UW-tf-dev-1.57.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/README.md` & `Simba-UW-tf-dev-1.57.3/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.2/setup.py` & `Simba-UW-tf-dev-1.57.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.57.2",
+    version="1.57.3",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

