# Comparing `tmp/Simba-UW-tf-dev-1.57.3.tar.gz` & `tmp/Simba-UW-tf-dev-1.57.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.3.tar", last modified: Sat Apr 22 15:30:26 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.57.4.tar", last modified: Sat Apr 22 17:32:08 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.57.3.tar` & `Simba-UW-tf-dev-1.57.4.tar`

### file list

```diff
@@ -1,395 +1,395 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/
--rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.57.3/simba/video_processing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.3/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11938 2023-04-20 14:29:24.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    10960 2023-04-19 14:59:03.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/unsupervised_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     3354 2023-04-20 14:05:40.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-20 13:38:50.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7569 2023-04-20 15:20:31.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     4812 2023-04-20 14:48:41.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     6687 2023-04-20 15:04:13.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9907 2023-04-20 12:55:14.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)     8375 2023-04-19 18:35:33.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41552 2023-04-20 14:49:52.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2331 2023-04-20 12:56:44.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    18472 2023-04-19 23:04:27.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)     8421 2023-04-20 13:33:19.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.57.3/simba/unsupervised/cluster_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.57.3/simba/enums.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/find_bounderies.py
--rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-22 15:14:38.000000 Simba-UW-tf-dev-1.57.3/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     1959 2023-04-20 20:07:38.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    26890 2023-04-20 18:25:40.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-21 18:44:23.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/extract_features_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)     8481 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/plotly_create_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.3/simba/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.3/simba/severity_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.57.3/simba/user_pose_config_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    42063 2023-04-19 23:53:37.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     8351 2023-04-22 13:11:36.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     6092 2023-04-19 18:08:18.000000 Simba-UW-tf-dev-1.57.3/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.57.3/simba/machine_model_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.3/simba/remove_keypoints_in_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/solomon_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.57.3/simba/FSTTC_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.57.3/simba/create_project_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.3/simba/video_info_table.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/extract_frames_fast.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.3/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.3/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.57.3/simba/utils/lookups.py
--rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.57.3/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.57.3/simba/utils/printing.py
--rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.3/simba/timebins_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    47395 2023-04-20 01:59:56.000000 Simba-UW-tf-dev-1.57.3/simba/train_model_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.3/simba/timebins_clf_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.57.3/simba/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.3/simba/movement_processor.py
--rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pybursts.py
--rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.57.3/simba/rw_dfs.py
--rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/reverse_2_animal_tracking.py
--rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.57.3/simba/Directing_animals_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.57.3/simba/Validate_model_one_video_run_clf.py
--rw-r--r--   0 simon      (501) staff       (20)    10872 2023-04-21 16:14:46.000000 Simba-UW-tf-dev-1.57.3/simba/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.57.3/simba/setting_menu.py
--rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.57.3/simba/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.57.3/simba/run_inference.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/misc_visualizations.py
--rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    17891 2023-04-22 14:54:57.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    12889 2023-04-22 14:51:45.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_location_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/interpolate_smooth_post_hoc.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/reverse_tracking_order.py
--rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.57.3/simba/concatenator_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/extract_annotation_frames.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_image.py
--rw-r--r--   0 simon      (501) staff       (20)    56353 2023-04-20 15:18:16.000000 Simba-UW-tf-dev-1.57.3/simba/misc_tools.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_slp.py
--rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_h5.py
--rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/dlc_multi_animal_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/import_trk.py
--rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_importers/trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)   236359 2023-04-22 15:26:04.000000 Simba-UW-tf-dev-1.57.3/simba/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/extract_seqframes.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/1.png
--rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/get_coordinates_tools_v2.py
--rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.57.3/simba/pup_retrieval_protocol.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.3/simba/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)    19358 2023-04-21 19:25:08.000000 Simba-UW-tf-dev-1.57.3/simba/train_mutiple_models.py
--rw-r--r--   0 simon      (501) staff       (20)    64554 2023-04-22 15:14:52.000000 Simba-UW-tf-dev-1.57.3/simba/SimBA.py
--rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/labelling_advanced_interface.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-22 15:14:38.000000 Simba-UW-tf-dev-1.57.3/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.3/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.3/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/assets/TheGoldenLab.PNG
--rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.57.3/simba/drop_bp_cords.py
--rw-r--r--   0 simon      (501) staff       (20)     9460 2023-04-21 14:18:35.000000 Simba-UW-tf-dev-1.57.3/simba/read_config_unit_tests.py
--rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/project_config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.57.3/simba/set_hyperparameters.py
--rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.57.3/simba/train_single_model.py
--rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/create_clf_log.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
--rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.3/simba/Kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.3/simba/reorganize_keypoint_in_pose.py
--rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.3/simba/~$features.pptx
--rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.3/simba/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    13533 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-22 15:30:25.000000 Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.3/LICENSE.md
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.3/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.3/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-22 15:30:17.000000 Simba-UW-tf-dev-1.57.3/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-22 15:30:26.000000 Simba-UW-tf-dev-1.57.3/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/
+-rw-r--r--   0 simon      (501) staff       (20)    38767 2023-04-15 18:44:14.000000 Simba-UW-tf-dev-1.57.4/simba/video_processing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-21 20:39:46.000000 Simba-UW-tf-dev-1.57.4/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11938 2023-04-20 14:29:24.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    10960 2023-04-19 14:59:03.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/unsupervised_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     3354 2023-04-20 14:05:40.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-20 13:38:50.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7569 2023-04-20 15:20:31.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4812 2023-04-20 14:48:41.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     6687 2023-04-20 15:04:13.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9907 2023-04-20 12:55:14.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     8375 2023-04-19 18:35:33.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41552 2023-04-20 14:49:52.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2331 2023-04-20 12:56:44.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    18472 2023-04-19 23:04:27.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)     8421 2023-04-20 13:33:19.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3931 2023-04-19 18:21:47.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     5895 2023-04-18 19:12:52.000000 Simba-UW-tf-dev-1.57.4/simba/unsupervised/cluster_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    19486 2023-04-18 14:10:55.000000 Simba-UW-tf-dev-1.57.4/simba/enums.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7520 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)     8596 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/find_bounderies.py
+-rw-r--r--   0 simon      (501) staff       (20)    24561 2023-04-06 11:22:38.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     9536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12664 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    32772 2023-04-22 15:14:38.000000 Simba-UW-tf-dev-1.57.4/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42823 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21575 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     1959 2023-04-20 20:07:38.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    26890 2023-04-20 18:25:40.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    28003 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-04-22 15:54:57.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-04-13 15:35:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    10774 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      905 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)   238196 2023-04-04 11:31:57.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69038 2023-04-04 11:32:25.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)   238298 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    69338 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-04 11:32:29.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2179 2023-04-04 11:32:26.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    36728 2023-04-17 19:25:13.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/extract_features_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8483 2023-04-22 17:31:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)     5380 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    46489 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24076 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16793 2023-04-15 18:48:24.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     6044 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/plotly_create_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    15351 2023-04-06 14:48:36.000000 Simba-UW-tf-dev-1.57.4/simba/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)     5928 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.4/simba/severity_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     5900 2023-04-10 16:12:09.000000 Simba-UW-tf-dev-1.57.4/simba/user_pose_config_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    42063 2023-04-19 23:53:37.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8351 2023-04-22 13:11:36.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)     6781 2023-04-11 20:14:16.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     6092 2023-04-19 18:08:18.000000 Simba-UW-tf-dev-1.57.4/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    34586 2023-04-15 19:04:12.000000 Simba-UW-tf-dev-1.57.4/simba/machine_model_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5231 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.4/simba/remove_keypoints_in_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6400 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     9984 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     9242 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16922 2023-03-28 20:30:38.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18322 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8372 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6964 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5471 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/solomon_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7286 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)    12867 2023-04-18 20:27:02.000000 Simba-UW-tf-dev-1.57.4/simba/FSTTC_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12575 2023-04-10 12:13:26.000000 Simba-UW-tf-dev-1.57.4/simba/create_project_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    13377 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.4/simba/video_info_table.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:25:58.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8632 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    13564 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    18253 2023-04-06 11:29:26.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1660 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    16427 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    13265 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2813 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/extract_frames_fast.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 20:15:03.000000 Simba-UW-tf-dev-1.57.4/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7335 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.4/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     5345 2023-04-14 15:36:09.000000 Simba-UW-tf-dev-1.57.4/simba/utils/lookups.py
+-rw-r--r--   0 simon      (501) staff       (20)    14631 2023-04-16 19:52:37.000000 Simba-UW-tf-dev-1.57.4/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1045 2023-04-12 13:34:48.000000 Simba-UW-tf-dev-1.57.4/simba/utils/printing.py
+-rw-r--r--   0 simon      (501) staff       (20)    21641 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     9980 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.4/simba/timebins_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    47395 2023-04-20 01:59:56.000000 Simba-UW-tf-dev-1.57.4/simba/train_model_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     7556 2023-04-10 15:43:18.000000 Simba-UW-tf-dev-1.57.4/simba/timebins_clf_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     8240 2023-03-17 16:23:58.000000 Simba-UW-tf-dev-1.57.4/simba/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     6566 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.4/simba/movement_processor.py
+-rw-r--r--   0 simon      (501) staff       (20)     2904 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pybursts.py
+-rw-r--r--   0 simon      (501) staff       (20)     4047 2023-04-17 01:05:46.000000 Simba-UW-tf-dev-1.57.4/simba/rw_dfs.py
+-rw-r--r--   0 simon      (501) staff       (20)     6536 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/reverse_2_animal_tracking.py
+-rw-r--r--   0 simon      (501) staff       (20)     9770 2023-04-10 14:38:06.000000 Simba-UW-tf-dev-1.57.4/simba/Directing_animals_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3570 2023-04-10 23:04:08.000000 Simba-UW-tf-dev-1.57.4/simba/Validate_model_one_video_run_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)    10872 2023-04-21 16:14:46.000000 Simba-UW-tf-dev-1.57.4/simba/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    13767 2023-03-24 12:49:19.000000 Simba-UW-tf-dev-1.57.4/simba/setting_menu.py
+-rw-r--r--   0 simon      (501) staff       (20)     6614 2023-03-19 16:33:17.000000 Simba-UW-tf-dev-1.57.4/simba/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     4771 2023-04-10 19:17:14.000000 Simba-UW-tf-dev-1.57.4/simba/run_inference.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     8634 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5353 2023-03-30 15:38:37.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    18101 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15262 2023-04-19 14:54:02.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12985 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15811 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8839 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16036 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/misc_visualizations.py
+-rw-r--r--   0 simon      (501) staff       (20)    13533 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    17734 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16340 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12691 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    12646 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5341 2023-03-30 15:46:49.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5896 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    12256 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    11246 2023-04-10 17:06:45.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)    12570 2023-04-10 16:40:38.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     9979 2023-04-10 16:36:45.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    17891 2023-04-22 14:54:57.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    20037 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10219 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12889 2023-04-22 14:51:45.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8685 2023-04-10 17:02:33.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    13027 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15890 2023-04-10 17:14:05.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13230 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     8951 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13625 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-04-10 16:38:59.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16189 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_location_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)     7609 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/interpolate_smooth_post_hoc.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     6350 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/reverse_tracking_order.py
+-rw-r--r--   0 simon      (501) staff       (20)     5772 2023-03-20 13:55:20.000000 Simba-UW-tf-dev-1.57.4/simba/concatenator_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2863 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/extract_annotation_frames.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7437 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     2166 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43921 2023-04-10 18:21:25.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     3384 2023-03-20 12:41:16.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    21277 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11934 2023-04-10 18:32:39.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3537 2023-03-15 17:12:38.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      961 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11335 2023-04-05 11:07:42.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5097 2023-04-05 20:01:02.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    15290 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22682 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_image.py
+-rw-r--r--   0 simon      (501) staff       (20)    56353 2023-04-20 15:18:16.000000 Simba-UW-tf-dev-1.57.4/simba/misc_tools.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     2494 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)    25864 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_slp.py
+-rw-r--r--   0 simon      (501) staff       (20)    24665 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_h5.py
+-rw-r--r--   0 simon      (501) staff       (20)    26731 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/dlc_multi_animal_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    23776 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)    16483 2023-04-14 16:41:29.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/import_trk.py
+-rw-r--r--   0 simon      (501) staff       (20)     7924 2023-04-10 17:34:37.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     8919 2023-04-10 17:29:32.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     7828 2023-04-10 18:12:26.000000 Simba-UW-tf-dev-1.57.4/simba/pose_importers/trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)   236359 2023-04-22 15:26:04.000000 Simba-UW-tf-dev-1.57.4/simba/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     4692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/extract_seqframes.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-10 12:22:28.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-03-20 15:55:45.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/1.png
+-rw-r--r--   0 simon      (501) staff       (20)     7273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/get_coordinates_tools_v2.py
+-rw-r--r--   0 simon      (501) staff       (20)    16252 2023-03-15 19:16:56.000000 Simba-UW-tf-dev-1.57.4/simba/pup_retrieval_protocol.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     7822 2023-04-10 16:32:30.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-15 17:05:05.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8304 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     4411 2023-04-10 16:33:31.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)     2610 2023-04-10 15:22:21.000000 Simba-UW-tf-dev-1.57.4/simba/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)    19358 2023-04-21 19:25:08.000000 Simba-UW-tf-dev-1.57.4/simba/train_mutiple_models.py
+-rw-r--r--   0 simon      (501) staff       (20)    64554 2023-04-22 15:14:52.000000 Simba-UW-tf-dev-1.57.4/simba/SimBA.py
+-rw-r--r--   0 simon      (501) staff       (20)    27472 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/labelling_advanced_interface.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-04-22 15:52:42.000000 Simba-UW-tf-dev-1.57.4/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2426 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.57.4/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.57.4/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/assets/TheGoldenLab.PNG
+-rw-r--r--   0 simon      (501) staff       (20)    15545 2023-04-14 16:40:51.000000 Simba-UW-tf-dev-1.57.4/simba/drop_bp_cords.py
+-rw-r--r--   0 simon      (501) staff       (20)     9460 2023-04-21 14:18:35.000000 Simba-UW-tf-dev-1.57.4/simba/read_config_unit_tests.py
+-rw-r--r--   0 simon      (501) staff       (20)    11742 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/project_config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    27444 2023-03-15 15:58:40.000000 Simba-UW-tf-dev-1.57.4/simba/set_hyperparameters.py
+-rw-r--r--   0 simon      (501) staff       (20)    20756 2023-04-19 14:41:07.000000 Simba-UW-tf-dev-1.57.4/simba/train_single_model.py
+-rw-r--r--   0 simon      (501) staff       (20)     6467 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/create_clf_log.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-17 14:43:38.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    24911 2023-04-17 19:39:19.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    10930 2023-04-17 19:35:15.000000 Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py
+-rw-r--r--   0 simon      (501) staff       (20)     9585 2023-04-10 13:29:16.000000 Simba-UW-tf-dev-1.57.4/simba/Kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8349 2023-04-10 13:29:17.000000 Simba-UW-tf-dev-1.57.4/simba/reorganize_keypoint_in_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)      165 2023-03-25 11:18:21.000000 Simba-UW-tf-dev-1.57.4/simba/~$features.pptx
+-rw-r--r--   0 simon      (501) staff       (20)     6557 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.57.4/simba/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    13533 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        6 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-04-22 17:32:07.000000 Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.57.4/LICENSE.md
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.57.4/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.57.4/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-04-22 17:31:56.000000 Simba-UW-tf-dev-1.57.4/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-04-22 17:32:08.000000 Simba-UW-tf-dev-1.57.4/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.57.3/PKG-INFO` & `Simba-UW-tf-dev-1.57.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.3
+Version: 1.57.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.3/simba/video_processing.py` & `Simba-UW-tf-dev-1.57.4/simba/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/unsupervised_ui.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/unsupervised_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.57.4/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/enums.py` & `Simba-UW-tf-dev-1.57.4/simba/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/find_bounderies.py` & `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/find_bounderies.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.57.4/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -288,124 +288,124 @@
 000011f0: 6444 626c 6f62 0000 0008 0a8c 6973 23f2  dDblob......is#.
 00001200: c441 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 00001220: 636f 6d70 0000 0000 000c 9000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
 00001250: 0001 0000 0004 006d 0069 0073 0063 6277  .......m.i.s.cbw
-00001260: 7370 626c 6f62 0000 00c8 6270 6c69 7374  spblob....bplist
+00001260: 7370 626c 6f62 0000 00ca 6270 6c69 7374  spblob....bplist
 00001270: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 00001280: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 00001290: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000012a0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 000012b0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 000012c0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 000012d0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000012e0: 6261 7208 0809 0809 5f10 177b 7b33 342c  bar....._..{{34,
-000012f0: 2039 307d 2c20 7b31 3031 352c 2037 3637   90}, {1015, 767
-00001300: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00001310: 7e98 0000 0000 0000 0101 0000 0000 0000  ~...............
-00001320: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-00001330: 0099 0000 0004 006d 0069 0073 0063 6c67  .......m.i.s.clg
-00001340: 3153 636f 6d70 0000 0000 0002 e73a 0000  1Scomp.......:..
-00001350: 0004 006d 0069 0073 0063 6c73 7643 626c  ...m.i.s.clsvCbl
-00001360: 6f62 0000 02b0 6270 6c69 7374 3030 da01  ob....bplist00..
-00001370: 0203 0405 0607 0809 0a0b 0c0d 1848 4948  .............HIH
-00001380: 4a4b 0c5f 1012 7669 6577 4f70 7469 6f6e  JK._..viewOption
-00001390: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-000013a0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-000013b0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-000013c0: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
-000013d0: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
-000013e0: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
-000013f0: 6f6e 585a 736f 7274 436f 6c75 6d6e 5869  onXZsortColumnXi
-00001400: 636f 6e53 697a 655f 1010 7573 6552 656c  conSize_..useRel
-00001410: 6174 6976 6544 6174 6573 1001 09ab 0e17  ativeDates......
-00001420: 1c21 252a 2f34 393e 43d4 0f10 1112 1314  .!%*/49>C.......
-00001430: 0c0c 5a69 6465 6e74 6966 6965 7255 7769  ..ZidentifierUwi
-00001440: 6474 6859 6173 6365 6e64 696e 6757 7669  dthYascendingWvi
-00001450: 7369 626c 6554 6e61 6d65 1101 a609 09d4  sibleTname......
-00001460: 1210 110f 1819 181b 0810 2308 5875 6269  ..........#.Xubi
-00001470: 7175 6974 79d4 1210 110f 0c1e 1820 0910  quity........ ..
-00001480: b508 5c64 6174 654d 6f64 6966 6965 64d4  ..\dateModified.
-00001490: 1210 110f 181e 1824 0808 5b64 6174 6543  .......$..[dateC
-000014a0: 7265 6174 6564 d412 1011 0f0c 2718 2909  reated......'.).
-000014b0: 1061 0854 7369 7a65 d412 1011 0f0c 2c0c  .a.Tsize......,.
-000014c0: 2e09 1073 0954 6b69 6e64 d412 1011 0f18  ...s.Tkind......
-000014d0: 310c 3308 1064 0955 6c61 6265 6cd4 1210  1.3..d.Ulabel...
-000014e0: 110f 1836 0c38 0810 4b09 5776 6572 7369  ...6.8..K.Wversi
-000014f0: 6f6e d412 1011 0f18 3b0c 3d08 1101 2c09  on......;.=...,.
-00001500: 5863 6f6d 6d65 6e74 73d4 1210 110f 1840  Xcomments......@
-00001510: 1842 0810 c808 5e64 6174 654c 6173 744f  .B....^dateLastO
-00001520: 7065 6e65 64d4 1210 110f 181e 1846 0808  pened........F..
-00001530: 5964 6174 6541 6464 6564 0823 0000 0000  YdateAdded.#....
-00001540: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
-00001550: 6d65 2340 3000 0000 0000 0009 0008 001d  me#@0...........
-00001560: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
-00001570: 00a1 00b4 00b6 00b7 00c3 00cc 00d7 00dd  ................
-00001580: 00e7 00ef 00f4 00f7 00f8 00f9 0102 0103  ................
-00001590: 0105 0106 010f 0118 0119 011b 011c 0129  ...............)
-000015a0: 0132 0133 0134 0140 0149 014a 014c 014d  .2.3.4.@.I.J.L.M
-000015b0: 0152 015b 015c 015e 015f 0164 016d 016e  .R.[.\.^._.d.m.n
-000015c0: 0170 0171 0177 0180 0181 0183 0184 018c  .p.q.w..........
-000015d0: 0195 0196 0199 019a 01a3 01ac 01ad 01af  ................
-000015e0: 01b0 01bf 01c8 01c9 01ca 01d4 01d5 01de  ................
-000015f0: 01e7 01ec 01f5 0000 0000 0000 0201 0000  ................
-00001600: 0000 0000 004d 0000 0000 0000 0000 0000  .....M..........
-00001610: 0000 0000 01f6 0000 0004 006d 0069 0073  ...........m.i.s
-00001620: 0063 6c73 7670 626c 6f62 0000 0295 6270  .clsvpblob....bp
-00001630: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
-00001640: 0a0b 0c0d 1f47 4847 494a 0c5f 1012 7669  .....GHGIJ._..vi
-00001650: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00001660: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-00001670: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-00001680: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
-00001690: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
-000016a0: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
-000016b0: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
-000016c0: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
-000016d0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-000016e0: 6573 1001 09d9 0e0f 1011 1213 1415 1617  es..............
-000016f0: 2025 292d 3237 3c41 5863 6f6d 6d65 6e74   %)-27<AXcomment
-00001700: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
-00001710: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
-00001720: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
-00001730: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
-00001740: 6e54 6e61 6d65 d418 191a 1b1c 1d0c 1f55  nTname.........U
-00001750: 696e 6465 7855 7769 6474 6859 6173 6365  indexUwidthYasce
-00001760: 6e64 696e 6757 7669 7369 626c 6510 0711  ndingWvisible...
-00001770: 012c 0908 d418 191a 1b21 221f 1f10 0810  .,.......!".....
-00001780: c808 08d4 1819 1a1b 0b26 1f0c 10b5 0809  .........&......
-00001790: d418 191a 1b2a 261f 1f10 0208 08d4 1819  .....*&.........
-000017a0: 1a1b 2e2f 1f0c 1003 1061 0809 d418 191a  .../.....a......
-000017b0: 1b33 340c 1f10 0510 6409 08d4 1819 1a1b  .34.....d.......
-000017c0: 3839 0c0c 1004 1073 0909 d418 191a 1b3d  89.....s.......=
-000017d0: 3e0c 1f10 0610 4b09 08d4 1b19 1a18 0c43  >.....K........C
-000017e0: 0c45 0911 01a6 0910 0008 2300 0000 0000  .E........#.....
-000017f0: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00001800: 6523 4030 0000 0000 0000 0900 0800 1d00  e#@0............
-00001810: 3200 4400 4c00 6000 7200 7b00 8d00 9800  2.D.L.`.r.{.....
-00001820: a100 b400 b600 b700 ca00 d300 e200 ef00  ................
-00001830: fb01 0001 0601 0b01 1301 1801 2101 2701  ............!.'.
-00001840: 2d01 3701 3f01 4101 4401 4501 4601 4f01  -.7.?.A.D.E.F.O.
-00001850: 5101 5301 5401 5501 5e01 6001 6101 6201  Q.S.T.U.^.`.a.b.
-00001860: 6b01 6d01 6e01 6f01 7801 7a01 7c01 7d01  k.m.n.o.x.z.|.}.
-00001870: 7e01 8701 8901 8b01 8c01 8d01 9601 9801  ~...............
-00001880: 9a01 9b01 9c01 a501 a701 a901 aa01 ab01  ................
-00001890: b401 b501 b801 b901 bb01 bc01 c501 ce01  ................
-000018a0: d301 dc00 0000 0000 0002 0100 0000 0000  ................
-000018b0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
-000018c0: 0001 dd00 0000 0400 6d00 6900 7300 636d  ........m.i.s.cm
-000018d0: 6f44 4462 6c6f 6200 0000 083b a5ee 5cdb  oDDblob....;..\.
-000018e0: f8c4 4100 0000 0400 6d00 6900 7300 636d  ..A.....m.i.s.cm
-000018f0: 6f64 4462 6c6f 6200 0000 083b a5ee 5cdb  odDblob....;..\.
-00001900: f8c4 4100 0000 0400 6d00 6900 7300 6370  ..A.....m.i.s.cp
-00001910: 6831 5363 6f6d 7000 0000 0000 03d0 0000  h1Scomp.........
-00001920: 0000 0400 6d00 6900 7300 6376 5372 6e6c  ....m.i.s.cvSrnl
-00001930: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
+000012e0: 6261 7208 0809 0809 5f10 197b 7b35 3039  bar....._..{{509
+000012f0: 2c20 3130 347d 2c20 7b31 3031 352c 2037  , 104}, {1015, 7
+00001300: 3637 7d7d 0908 1725 313d 4960 6d79 7a7b  67}}...%1=I`myz{
+00001310: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
+00001320: 0000 000f 0000 0000 0000 0000 0000 0000  ................
+00001330: 0000 009b 0000 0004 006d 0069 0073 0063  .........m.i.s.c
+00001340: 6c67 3153 636f 6d70 0000 0000 0002 ee9a  lg1Scomp........
+00001350: 0000 0004 006d 0069 0073 0063 6c73 7643  .....m.i.s.clsvC
+00001360: 626c 6f62 0000 02b0 6270 6c69 7374 3030  blob....bplist00
+00001370: da01 0203 0405 0607 0809 0a0b 0c0d 1848  ...............H
+00001380: 4948 4a4b 0c5f 1012 7669 6577 4f70 7469  IHJK._..viewOpti
+00001390: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
+000013a0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+000013b0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+000013c0: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
+000013d0: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
+000013e0: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
+000013f0: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
+00001400: 5869 636f 6e53 697a 655f 1010 7573 6552  XiconSize_..useR
+00001410: 656c 6174 6976 6544 6174 6573 1001 09ab  elativeDates....
+00001420: 0e17 1c21 252a 2f34 393e 43d4 0f10 1112  ...!%*/49>C.....
+00001430: 1314 0c0c 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
+00001440: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+00001450: 7669 7369 626c 6554 6e61 6d65 1101 a609  visibleTname....
+00001460: 09d4 1210 110f 1819 181b 0810 2308 5875  ............#.Xu
+00001470: 6269 7175 6974 79d4 1210 110f 0c1e 1820  biquity........ 
+00001480: 0910 b508 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00001490: 64d4 1210 110f 181e 1824 0808 5b64 6174  d........$..[dat
+000014a0: 6543 7265 6174 6564 d412 1011 0f0c 2718  eCreated......'.
+000014b0: 2909 1061 0854 7369 7a65 d412 1011 0f0c  )..a.Tsize......
+000014c0: 2c0c 2e09 1073 0954 6b69 6e64 d412 1011  ,....s.Tkind....
+000014d0: 0f18 310c 3308 1064 0955 6c61 6265 6cd4  ..1.3..d.Ulabel.
+000014e0: 1210 110f 1836 0c38 0810 4b09 5776 6572  .....6.8..K.Wver
+000014f0: 7369 6f6e d412 1011 0f18 3b0c 3d08 1101  sion......;.=...
+00001500: 2c09 5863 6f6d 6d65 6e74 73d4 1210 110f  ,.Xcomments.....
+00001510: 1840 1842 0810 c808 5e64 6174 654c 6173  .@.B....^dateLas
+00001520: 744f 7065 6e65 64d4 1210 110f 181e 1846  tOpened........F
+00001530: 0808 5964 6174 6541 6464 6564 0823 0000  ..YdateAdded.#..
+00001540: 0000 0000 0000 2340 2800 0000 0000 0054  ......#@(......T
+00001550: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
+00001560: 001d 0032 0044 004c 0060 0072 007b 008d  ...2.D.L.`.r.{..
+00001570: 0098 00a1 00b4 00b6 00b7 00c3 00cc 00d7  ................
+00001580: 00dd 00e7 00ef 00f4 00f7 00f8 00f9 0102  ................
+00001590: 0103 0105 0106 010f 0118 0119 011b 011c  ................
+000015a0: 0129 0132 0133 0134 0140 0149 014a 014c  .).2.3.4.@.I.J.L
+000015b0: 014d 0152 015b 015c 015e 015f 0164 016d  .M.R.[.\.^._.d.m
+000015c0: 016e 0170 0171 0177 0180 0181 0183 0184  .n.p.q.w........
+000015d0: 018c 0195 0196 0199 019a 01a3 01ac 01ad  ................
+000015e0: 01af 01b0 01bf 01c8 01c9 01ca 01d4 01d5  ................
+000015f0: 01de 01e7 01ec 01f5 0000 0000 0000 0201  ................
+00001600: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
+00001610: 0000 0000 0000 01f6 0000 0004 006d 0069  .............m.i
+00001620: 0073 0063 6c73 7670 626c 6f62 0000 0295  .s.clsvpblob....
+00001630: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
+00001640: 0809 0a0b 0c0d 1f47 4847 494a 0c5f 1012  .......GHGIJ._..
+00001650: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00001660: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00001670: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00001680: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00001690: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000016a0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+000016b0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+000016c0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+000016d0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+000016e0: 6174 6573 1001 09d9 0e0f 1011 1213 1415  ates............
+000016f0: 1617 2025 292d 3237 3c41 5863 6f6d 6d65  .. %)-27<AXcomme
+00001700: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+00001710: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
+00001720: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+00001730: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+00001740: 696f 6e54 6e61 6d65 d418 191a 1b1c 1d0c  ionTname........
+00001750: 1f55 696e 6465 7855 7769 6474 6859 6173  .UindexUwidthYas
+00001760: 6365 6e64 696e 6757 7669 7369 626c 6510  cendingWvisible.
+00001770: 0711 012c 0908 d418 191a 1b21 221f 1f10  ...,.......!"...
+00001780: 0810 c808 08d4 1819 1a1b 0b26 1f0c 10b5  ...........&....
+00001790: 0809 d418 191a 1b2a 261f 1f10 0208 08d4  .......*&.......
+000017a0: 1819 1a1b 2e2f 1f0c 1003 1061 0809 d418  ...../.....a....
+000017b0: 191a 1b33 340c 1f10 0510 6409 08d4 1819  ...34.....d.....
+000017c0: 1a1b 3839 0c0c 1004 1073 0909 d418 191a  ..89.....s......
+000017d0: 1b3d 3e0c 1f10 0610 4b09 08d4 1b19 1a18  .=>.....K.......
+000017e0: 0c43 0c45 0911 01a6 0910 0008 2300 0000  .C.E........#...
+000017f0: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
+00001800: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
+00001810: 1d00 3200 4400 4c00 6000 7200 7b00 8d00  ..2.D.L.`.r.{...
+00001820: 9800 a100 b400 b600 b700 ca00 d300 e200  ................
+00001830: ef00 fb01 0001 0601 0b01 1301 1801 2101  ..............!.
+00001840: 2701 2d01 3701 3f01 4101 4401 4501 4601  '.-.7.?.A.D.E.F.
+00001850: 4f01 5101 5301 5401 5501 5e01 6001 6101  O.Q.S.T.U.^.`.a.
+00001860: 6201 6b01 6d01 6e01 6f01 7801 7a01 7c01  b.k.m.n.o.x.z.|.
+00001870: 7d01 7e01 8701 8901 8b01 8c01 8d01 9601  }.~.............
+00001880: 9801 9a01 9b01 9c01 a501 a701 a901 aa01  ................
+00001890: ab01 b401 b501 b801 b901 bb01 bc01 c501  ................
+000018a0: ce01 d301 dc00 0000 0000 0002 0100 0000  ................
+000018b0: 0000 0000 4c00 0000 0000 0000 0000 0000  ....L...........
+000018c0: 0000 0001 dd00 0000 0400 6d00 6900 7300  ..........m.i.s.
+000018d0: 636d 6f44 4462 6c6f 6200 0000 0824 9c16  cmoDDblob....$..
+000018e0: 85e9 f8c4 4100 0000 0400 6d00 6900 7300  ....A.....m.i.s.
+000018f0: 636d 6f64 4462 6c6f 6200 0000 0824 9c16  cmodDblob....$..
+00001900: 85e9 f8c4 4100 0000 0400 6d00 6900 7300  ....A.....m.i.s.
+00001910: 6370 6831 5363 6f6d 7000 0000 0000 03e0  cph1Scomp.......
+00001920: 0000 0000 0400 6d00 6900 7300 6376 5372  ......m.i.s.cvSr
+00001930: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
 00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0063 6f6d 6d65 6e74 73d4 1210 110f 1840  .comments......@
-00002510: 1842 0810 c808 5e64 6174 654c 6173 744f  .B....^dateLastO
-00002520: 7065 6e65 64d4 1210 110f 181e 1846 0808  pened........F..
-00002530: 5964 6174 6541 6464 6564 0823 0000 0000  YdateAdded.#....
-00002540: 0000 0000 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
-00002550: 6d65 2340 3000 0000 0000 0009 0008 001d  me#@0...........
-00002560: 0032 0044 004c 0060 0072 007b 008d 0098  .2.D.L.`.r.{....
-00002570: 00a1 00b4 00b6 00b7 00c3 00cc 00d7 00dd  ................
-00002580: 00e7 00ef 00f4 00f7 00f8 00f9 0102 0103  ................
-00002590: 0105 0106 010f 0118 0119 011b 011c 0129  ...............)
-000025a0: 0132 0133 0134 0140 0149 014a 014c 014d  .2.3.4.@.I.J.L.M
-000025b0: 0152 015b 015c 015e 015f 0164 016d 016e  .R.[.\.^._.d.m.n
-000025c0: 0170 0171 0177 0180 0181 0183 0184 018c  .p.q.w..........
-000025d0: 0195 0196 0199 019a 01a3 01ac 01ad 01af  ................
-000025e0: 01b0 01bf 01c8 01c9 01ca 01d4 01d5 01de  ................
-000025f0: 01e7 01ec 01f5 0000 0000 0000 0201 0000  ................
-00002600: 0000 0000 004d 0000 0000 0000 0000 0000  .....M..........
-00002610: 0000 0000 01f6 0000 0004 006d 0069 0073  ...........m.i.s
-00002620: 0063 6c73 7670 626c 6f62 0000 0295 6270  .clsvpblob....bp
-00002630: 6c69 7374 3030 da01 0203 0405 0607 0809  list00..........
-00002640: 0a0b 0c0d 1f47 4847 494a 0c5f 1012 7669  .....GHGIJ._..vi
-00002650: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-00002660: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
-00002670: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
-00002680: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
-00002690: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
-000026a0: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
-000026b0: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
-000026c0: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
-000026d0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-000026e0: 6573 1001 09d9 0e0f 1011 1213 1415 1617  es..............
-000026f0: 2025 292d 3237 3c41 5863 6f6d 6d65 6e74   %)-27<AXcomment
-00002700: 735e 6461 7465 4c61 7374 4f70 656e 6564  s^dateLastOpened
-00002710: 5c64 6174 654d 6f64 6966 6965 645b 6461  \dateModified[da
-00002720: 7465 4372 6561 7465 6454 7369 7a65 556c  teCreatedTsizeUl
-00002730: 6162 656c 546b 696e 6457 7665 7273 696f  abelTkindWversio
-00002740: 6e54 6e61 6d65 d418 191a 1b1c 1d0c 1f55  nTname.........U
-00002750: 696e 6465 7855 7769 6474 6859 6173 6365  indexUwidthYasce
-00002760: 6e64 696e 6757 7669 7369 626c 6510 0711  ndingWvisible...
-00002770: 012c 0908 d418 191a 1b21 221f 1f10 0810  .,.......!".....
-00002780: c808 08d4 1819 1a1b 0b26 1f0c 10b5 0809  .........&......
-00002790: d418 191a 1b2a 261f 1f10 0208 08d4 1819  .....*&.........
-000027a0: 1a1b 2e2f 1f0c 1003 1061 0809 d418 191a  .../.....a......
-000027b0: 1b33 340c 1f10 0510 6409 08d4 1819 1a1b  .34.....d.......
-000027c0: 3839 0c0c 1004 1073 0909 d418 191a 1b3d  89.....s.......=
-000027d0: 3e0c 1f10 0610 4b09 08d4 1b19 1a18 0c43  >.....K........C
-000027e0: 0c45 0911 01a6 0910 0008 2300 0000 0000  .E........#.....
-000027f0: 0000 0023 4028 0000 0000 0000 546e 616d  ...#@(......Tnam
-00002800: 6523 4030                                e#@0
+00002500: 0009 5863 6f6d 6d65 6e74 73d4 1210 110f  ..Xcomments.....
+00002510: 1840 1842 0810 c808 5e64 6174 654c 6173  .@.B....^dateLas
+00002520: 744f 7065 6e65 64d4 1210 110f 181e 1846  tOpened........F
+00002530: 0808 5964 6174 6541 6464 6564 0823 0000  ..YdateAdded.#..
+00002540: 0000 0000 0000 2340 2800 0000 0000 0054  ......#@(......T
+00002550: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
+00002560: 001d 0032 0044 004c 0060 0072 007b 008d  ...2.D.L.`.r.{..
+00002570: 0098 00a1 00b4 00b6 00b7 00c3 00cc 00d7  ................
+00002580: 00dd 00e7 00ef 00f4 00f7 00f8 00f9 0102  ................
+00002590: 0103 0105 0106 010f 0118 0119 011b 011c  ................
+000025a0: 0129 0132 0133 0134 0140 0149 014a 014c  .).2.3.4.@.I.J.L
+000025b0: 014d 0152 015b 015c 015e 015f 0164 016d  .M.R.[.\.^._.d.m
+000025c0: 016e 0170 0171 0177 0180 0181 0183 0184  .n.p.q.w........
+000025d0: 018c 0195 0196 0199 019a 01a3 01ac 01ad  ................
+000025e0: 01af 01b0 01bf 01c8 01c9 01ca 01d4 01d5  ................
+000025f0: 01de 01e7 01ec 01f5 0000 0000 0000 0201  ................
+00002600: 0000 0000 0000 004d 0000 0000 0000 0000  .......M........
+00002610: 0000 0000 0000 01f6 0000 0004 006d 0069  .............m.i
+00002620: 0073 0063 6c73 7670 626c 6f62 0000 0295  .s.clsvpblob....
+00002630: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
+00002640: 0809 0a0b 0c0d 1f47 4847 494a 0c5f 1012  .......GHGIJ._..
+00002650: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00002660: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00002670: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00002680: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00002690: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000026a0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+000026b0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+000026c0: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
+000026d0: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
+000026e0: 6174 6573 1001 09d9 0e0f 1011 1213 1415  ates............
+000026f0: 1617 2025 292d 3237 3c41 5863 6f6d 6d65  .. %)-27<AXcomme
+00002700: 6e74 735e 6461 7465 4c61 7374 4f70 656e  nts^dateLastOpen
+00002710: 6564 5c64 6174 654d 6f64 6966 6965 645b  ed\dateModified[
+00002720: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
+00002730: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
+00002740: 696f 6e54 6e61 6d65 d418 191a 1b1c 1d0c  ionTname........
+00002750: 1f55 696e 6465 7855 7769 6474 6859 6173  .UindexUwidthYas
+00002760: 6365 6e64 696e 6757 7669 7369 626c 6510  cendingWvisible.
+00002770: 0711 012c 0908 d418 191a 1b21 221f 1f10  ...,.......!"...
+00002780: 0810 c808 08d4 1819 1a1b 0b26 1f0c 10b5  ...........&....
+00002790: 0809 d418 191a 1b2a 261f 1f10 0208 08d4  .......*&.......
+000027a0: 1819 1a1b 2e2f 1f0c 1003 1061 0809 d418  ...../.....a....
+000027b0: 191a 1b33 340c 1f10 0510 6409 08d4 1819  ...34.....d.....
+000027c0: 1a1b 3839 0c0c 1004 1073 0909 d418 191a  ..89.....s......
+000027d0: 1b3d 3e0c 1f10 0610 4b09 08d4 1b19 1a18  .=>.....K.......
+000027e0: 0c43 0c45 0911 01a6 0910 0008 2300 0000  .C.E........#...
+000027f0: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
+00002800: 616d 6523                                ame#
```

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.quickhull_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.convex_hull_perimeter_2d-16.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/__pycache__/perimeter_jit.process-7.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/extract_features_9bp.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/extract_features_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,9 +132,9 @@
             video_timer.stop_timer()
             print('Saving features for video {}...'.format(file_name))
             print('Feature extraction complete for video {} (elapsed time: {}s)'.format(file_name, video_timer.elapsed_time_str))
 
         self.timer.stop_timer()
         stdout_success(f'Feature extraction complete for {str(len(self.files_found))} video(s). Results are saved inside the project_folder/csv/features_extracted directory', elapsed_time=self.timer.elapsed_time_str)
 
-# test = UserDefinedFeatureExtractor(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
-# test.extract_features()
+## test = UserDefinedFeatureExtractor(config_path='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/project_config.ini')
+## test.extract_features()
```

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/unit_tests.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.4/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotly_create_h5.py` & `Simba-UW-tf-dev-1.57.4/simba/plotly_create_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/requirements.txt` & `Simba-UW-tf-dev-1.57.4/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/severity_processor.py` & `Simba-UW-tf-dev-1.57.4/simba/severity_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/user_pose_config_creator.py` & `Simba-UW-tf-dev-1.57.4/simba/user_pose_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.57.4/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.57.4/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.57.4/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.57.4/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/machine_model_settings_pop_up.py` & `Simba-UW-tf-dev-1.57.4/simba/machine_model_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/remove_keypoints_in_pose.py` & `Simba-UW-tf-dev-1.57.4/simba/remove_keypoints_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.57.4/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/multi_cropper.py` & `Simba-UW-tf-dev-1.57.4/simba/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/FSTTC_calculator.py` & `Simba-UW-tf-dev-1.57.4/simba/FSTTC_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/create_project_pop_up.py` & `Simba-UW-tf-dev-1.57.4/simba/create_project_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/video_info_table.py` & `Simba-UW-tf-dev-1.57.4/simba/video_info_table.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.57.4/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/extract_frames_fast.py` & `Simba-UW-tf-dev-1.57.4/simba/extract_frames_fast.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.57.4/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.57.4/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/utils/errors.py` & `Simba-UW-tf-dev-1.57.4/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/utils/printing.py` & `Simba-UW-tf-dev-1.57.4/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/labelling_interface.py` & `Simba-UW-tf-dev-1.57.4/simba/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/timebins_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.4/simba/timebins_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/train_model_functions.py` & `Simba-UW-tf-dev-1.57.4/simba/train_model_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.57.4/simba/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/timebins_clf_analyzer.py` & `Simba-UW-tf-dev-1.57.4/simba/timebins_clf_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/calculate_px_dist.py` & `Simba-UW-tf-dev-1.57.4/simba/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/movement_processor.py` & `Simba-UW-tf-dev-1.57.4/simba/movement_processor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pybursts.py` & `Simba-UW-tf-dev-1.57.4/simba/pybursts.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/rw_dfs.py` & `Simba-UW-tf-dev-1.57.4/simba/rw_dfs.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/reverse_2_animal_tracking.py` & `Simba-UW-tf-dev-1.57.4/simba/reverse_2_animal_tracking.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/Directing_animals_analyzer.py` & `Simba-UW-tf-dev-1.57.4/simba/Directing_animals_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/Validate_model_one_video_run_clf.py` & `Simba-UW-tf-dev-1.57.4/simba/Validate_model_one_video_run_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/tkinter_functions.py` & `Simba-UW-tf-dev-1.57.4/simba/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/setting_menu.py` & `Simba-UW-tf-dev-1.57.4/simba/setting_menu.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/interpolate_pose.py` & `Simba-UW-tf-dev-1.57.4/simba/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/run_inference.py` & `Simba-UW-tf-dev-1.57.4/simba/run_inference.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/misc_visualizations.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/misc_visualizations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.57.4/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.57.4/simba/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/interpolate_smooth_post_hoc.py` & `Simba-UW-tf-dev-1.57.4/simba/interpolate_smooth_post_hoc.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/dash_app.py` & `Simba-UW-tf-dev-1.57.4/simba/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/reverse_tracking_order.py` & `Simba-UW-tf-dev-1.57.4/simba/reverse_tracking_order.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/concatenator_pop_up.py` & `Simba-UW-tf-dev-1.57.4/simba/concatenator_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/extract_annotation_frames.py` & `Simba-UW-tf-dev-1.57.4/simba/extract_annotation_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.57.4/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/misc_tools.py` & `Simba-UW-tf-dev-1.57.4/simba/misc_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_slp.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_slp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_h5.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_h5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_importers/dlc_multi_animal_importer.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_importers/dlc_multi_animal_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_importers/sleap_importer_csv.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_importers/sleap_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_importers/import_trk.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_importers/import_trk.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pop_up_classes.py` & `Simba-UW-tf-dev-1.57.4/simba/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/extract_seqframes.py` & `Simba-UW-tf-dev-1.57.4/simba/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.57.4/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/get_coordinates_tools_v2.py` & `Simba-UW-tf-dev-1.57.4/simba/get_coordinates_tools_v2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pup_retrieval_protocol.py` & `Simba-UW-tf-dev-1.57.4/simba/pup_retrieval_protocol.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.57.4/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/pose_reset.py` & `Simba-UW-tf-dev-1.57.4/simba/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/train_mutiple_models.py` & `Simba-UW-tf-dev-1.57.4/simba/train_mutiple_models.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/SimBA.py` & `Simba-UW-tf-dev-1.57.4/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.57.4/simba/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.57.4/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.57.4/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/assets/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -484,276 +484,276 @@
 00001e30: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00001e40: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00001e50: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00001e60: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00001e70: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00001e80: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00001e90: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00001ea0: 01c5 5522 f4c4 4100 0000 0500 6900 6300  ..U"..A.....i.c.
-00001eb0: 6f00 6e00 736d 6f64 4462 6c6f 6200 0000  o.n.smodDblob...
-00001ec0: 08c1 fc21 5522 f4c4 4100 0000 0500 6900  ...!U"..A.....i.
-00001ed0: 6300 6f00 6e00 7370 6831 5363 6f6d 7000  c.o.n.sph1Scomp.
-00001ee0: 0000 0000 0800 0000 0000 0500 6900 6300  ............i.c.
-00001ef0: 6f00 6e00 7376 5372 6e6c 6f6e 6700 0000  o.n.svSrnlong...
-00001f00: 0100 0000 0300 6900 6d00 6762 7773 7062  ......i.m.gbwspb
-00001f10: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
-00001f20: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
-00001f30: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00001f40: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00001f50: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00001f60: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00001f70: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00001f80: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00001f90: 0808 0908 095f 1019 7b7b 3338 382c 2032  ....._..{{388, 2
-00001fa0: 3136 7d2c 207b 3130 3932 2c20 3432 327d  16}, {1092, 422}
-00001fb0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-00001fc0: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
-00001fd0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-00001fe0: 9b00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
-00001ff0: 6f6d 7000 0000 0000 1110 bf00 0000 0300  omp.............
-00002000: 6900 6d00 0000 0000 0000 0012 0000 0005  i.m.............
+00001ea0: 01c5 6300 6f00 6e00 736d 6f44 4462 6c6f  ..c.o.n.smoDDblo
+00001eb0: 6200 0000 08c1 fc21 5522 f4c4 4100 0000  b......!U"..A...
+00001ec0: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
+00001ed0: 6c6f 6200 0000 08c1 fc21 5522 f4c4 4100  lob......!U"..A.
+00001ee0: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
+00001ef0: 5363 6f6d 7000 0000 0000 0800 0000 0000  Scomp...........
+00001f00: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
+00001f10: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
+00001f20: 6762 7773 7062 6c6f 6200 0000 ca62 706c  gbwspblob....bpl
+00001f30: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
+00001f40: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+00001f50: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
+00001f60: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+00001f70: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+00001f80: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+00001f90: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+00001fa0: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
+00001fb0: 3338 382c 2032 3136 7d2c 207b 3130 3932  388, 216}, {1092
+00001fc0: 2c20 3432 327d 7d09 0817 2531 3d49 606d  , 422}}...%1=I`m
+00001fd0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
+00001fe0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+00001ff0: 0000 0000 0000 9b00 0000 0300 6900 6d00  ............i.m.
+00002000: 676c 6731 0000 0000 0000 0012 0000 0005  glg1............
 00002010: 0069 0063 006f 006e 0073 6277 7370 626c  .i.c.o.n.sbwspbl
 00002020: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
 00002030: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
 00002040: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00002050: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
 00002060: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
 00002070: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
 00002080: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
 00002090: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-000020a0: 0809 0809 5f10 197b 7b34 3230 2c20 3131  ...._..{{420, 11
-000020b0: 337d 2c20 7b31 3031 352c 2037 3637 7d7d  3}, {1015, 767}}
+000020a0: 0809 0809 5f10 197b 7b34 3139 2c20 3131  ...._..{{419, 11
+000020b0: 347d 2c20 7b31 3031 352c 2037 3637 7d7d  4}, {1015, 767}}
 000020c0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
 000020d0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
 000020e0: 0000 0000 0000 0000 0000 0000 0000 009b  ................
 000020f0: 0000 0005 0069 0063 006f 006e 0073 6c67  .....i.c.o.n.slg
 00002100: 3153 636f 6d70 0000 0000 0005 98d9 0000  1Scomp..........
 00002110: 0005 0069 0063 006f 006e 0073 6c73 7643  ...i.c.o.n.slsvC
-00002120: 626c 6f62 0000 02af 6270 6c69 7374 3030  blob....bplist00
-00002130: da01 0203 0405 0607 0809 0a0b 0c0d 1a48  ...............H
-00002140: 4948 4a0c 4c5f 1012 7669 6577 4f70 7469  IHJ.L_..viewOpti
-00002150: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-00002160: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-00002170: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-00002180: 416c 6c53 697a 6573 5f10 0f73 6372 6f6c  AllSizes_..scrol
-00002190: 6c50 6f73 6974 696f 6e59 5874 6578 7453  lPositionYXtextS
-000021a0: 697a 655f 100f 7363 726f 6c6c 506f 7369  ize_..scrollPosi
-000021b0: 7469 6f6e 585a 736f 7274 436f 6c75 6d6e  tionXZsortColumn
-000021c0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-000021d0: 7465 7358 6963 6f6e 5369 7a65 1001 09ab  tesXiconSize....
-000021e0: 0e17 1c21 252a 2f34 393e 43d4 0f10 1112  ...!%*/49>C.....
-000021f0: 1314 0c0c 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
-00002200: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00002210: 7669 7369 626c 6554 6e61 6d65 10ea 0909  visibleTname....
-00002220: d40f 1011 1218 191a 1a58 7562 6971 7569  .........Xubiqui
-00002230: 7479 1023 0808 d40f 1011 121d 1e1a 0c5c  ty.#...........\
-00002240: 6461 7465 4d6f 6469 6669 6564 10b5 0809  dateModified....
-00002250: d40f 1011 1222 1e1a 1a5b 6461 7465 4372  ....."...[dateCr
-00002260: 6561 7465 6408 08d4 0f10 1112 2627 1a0c  eated.......&'..
-00002270: 5473 697a 6510 6108 09d4 0f10 1112 2b2c  Tsize.a.......+,
-00002280: 0c0c 546b 696e 6410 7309 09d4 0f10 1112  ..Tkind.s.......
-00002290: 3031 0c1a 556c 6162 656c 1064 0908 d40f  01..Ulabel.d....
-000022a0: 1011 1235 360c 1a57 7665 7273 696f 6e10  ...56..Wversion.
-000022b0: 4b09 08d4 0f10 1112 3a3b 0c1a 5863 6f6d  K.......:;..Xcom
-000022c0: 6d65 6e74 7311 012c 0908 d40f 1011 123f  ments..,.......?
-000022d0: 401a 1a5e 6461 7465 4c61 7374 4f70 656e  @..^dateLastOpen
-000022e0: 6564 10c8 0808 d40f 1011 1244 1e1a 1a59  ed.........D...Y
-000022f0: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
-00002300: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
-00002310: 616d 6509 2340 3000 0000 0000 0000 0800  ame.#@0.........
-00002320: 1d00 3200 4400 4c00 6000 7200 7b00 8d00  ..2.D.L.`.r.{...
-00002330: 9800 ab00 b400 b600 b700 c300 cc00 d700  ................
-00002340: dd00 e700 ef00 f400 f600 f700 f801 0101  ................
-00002350: 0a01 0c01 0d01 0e01 1701 2401 2601 2701  ..........$.&.'.
-00002360: 2801 3101 3d01 3e01 3f01 4801 4d01 4f01  (.1.=.>.?.H.M.O.
-00002370: 5001 5101 5a01 5f01 6101 6201 6301 6c01  P.Q.Z._.a.b.c.l.
-00002380: 7201 7401 7501 7601 7f01 8701 8901 8a01  r.t.u.v.........
-00002390: 8b01 9401 9d01 a001 a101 a201 ab01 ba01  ................
-000023a0: bc01 bd01 be01 c701 d101 d201 d301 d401  ................
-000023b0: dd01 e601 eb01 ec00 0000 0000 0002 0100  ................
-000023c0: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
-000023d0: 0000 0000 0001 f500 0000 0500 6900 6300  ............i.c.
-000023e0: 6f00 6e00 736c 7376 7062 6c6f 6200 0002  o.n.slsvpblob...
-000023f0: 9462 706c 6973 7430 30da 0102 0304 0506  .bplist00.......
-00002400: 0708 090a 0b0c 0d1c 4748 4749 0c4b 5f10  ........GHGI.K_.
-00002410: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00002420: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
-00002430: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00002440: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00002450: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
-00002460: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
-00002470: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
-00002480: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
-00002490: 656c 6174 6976 6544 6174 6573 5869 636f  elativeDatesXico
-000024a0: 6e53 697a 6510 0109 d90e 0f10 1112 1314  nSize...........
-000024b0: 1516 1720 2529 2d32 373c 4158 636f 6d6d  ... %)-27<AXcomm
-000024c0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-000024d0: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-000024e0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-000024f0: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-00002500: 7369 6f6e 546e 616d 65d4 1819 1a1b 1c1d  sionTname.......
-00002510: 0c1f 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
-00002520: 5961 7363 656e 6469 6e67 5569 6e64 6578  YascendingUindex
-00002530: 0811 012c 0910 07d4 1819 1a1b 1c22 1c24  ...,.........".$
-00002540: 0810 c808 1008 d418 191a 1b0c 271c 0b09  ............'...
-00002550: 10b5 08d4 1819 1a1b 1c27 1c2c 0808 1002  .........'.,....
-00002560: d418 191a 1b0c 2f1c 3109 1061 0810 03d4  ....../.1..a....
-00002570: 1819 1a1b 1c34 0c36 0810 6409 1005 d418  .....4.6..d.....
-00002580: 191a 1b0c 390c 3b09 1073 0910 04d4 1819  ....9.;..s......
-00002590: 1a1b 1c3e 0c40 0810 4b09 1006 d418 191a  ...>.@..K.......
-000025a0: 1b0c 430c 4509 10ea 0910 0008 2300 0000  ..C.E.......#...
-000025b0: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
-000025c0: 616d 6509 2340 3000 0000 0000 0000 0800  ame.#@0.........
-000025d0: 1d00 3200 4400 4c00 6000 7200 7b00 8d00  ..2.D.L.`.r.{...
-000025e0: 9800 ab00 b400 b600 b700 ca00 d300 e200  ................
-000025f0: ef00 fb01 0001 0601 0b01 1301 1801 2101  ..............!.
-00002600: 2901 2f01 3901 3f01 4001 4301 4401 4601  )./.9.?.@.C.D.F.
-00002610: 4f01 5001 5201 5301 5501 5e01 5f01 6101  O.P.R.S.U.^._.a.
-00002620: 6201 6b01 6c01 6d01 6f01 7801 7901 7b01  b.k.l.m.o.x.y.{.
-00002630: 7c01 7e01 8701 8801 8a01 8b01 8d01 9601  |.~.............
-00002640: 9701 9901 9a01 9c01 a501 a601 a801 a901  ................
-00002650: ab01 b401 b501 b701 b801 ba01 bb01 c401  ................
-00002660: cd01 d201 d300 0000 0000 0002 0100 0000  ................
-00002670: 0000 0000 4c00 0000 0000 0000 0000 0000  ....L...........
-00002680: 0000 0001 dc00 0000 0500 6900 6300 6f00  ..........i.c.o.
-00002690: 6e00 736d 6f44 4462 6c6f 6200 0000 08c1  n.smoDDblob.....
-000026a0: fc21 5522 f4c4 4100 0000 0500 6900 6300  .!U"..A.....i.c.
-000026b0: 6f00 6e00 736d 6f64 4462 6c6f 6200 0000  o.n.smodDblob...
-000026c0: 08c1 fc21 5522 f4c4 4100 0000 0500 6900  ...!U"..A.....i.
-000026d0: 6300 6f00 6e00 7370 6831 5363 6f6d 7000  c.o.n.sph1Scomp.
-000026e0: 0000 0000 0800 0000 0000 0500 6900 6300  ............i.c.
-000026f0: 6f00 6e00 7376 5372 6e6c 6f6e 6700 0000  o.n.svSrnlong...
-00002700: 0100 0000 0300 6900 6d00 6762 7773 7062  ......i.m.gbwspb
-00002710: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
-00002720: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
-00002730: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00002740: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00002750: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00002760: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00002770: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00002780: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00002790: 0808 0908 095f 1019 7b7b 3338 382c 2032  ....._..{{388, 2
-000027a0: 3136 7d2c 207b 3130 3932 2c20 3432 327d  16}, {1092, 422}
-000027b0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-000027c0: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
-000027d0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-000027e0: 9b00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
-000027f0: 6f6d 7000 0000 0000 1110 bf00 0000 0300  omp.............
-00002800: 6900 6d00 676c 7376 4362 6c6f 6200 0002  i.m.glsvCblob...
-00002810: b062 706c 6973 7430 30da 0102 0304 0506  .bplist00.......
-00002820: 0708 090a 0b0c 0d1a 4849 484a 0c4c 5f10  ........HIHJ.L_.
-00002830: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00002840: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
-00002850: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00002860: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00002870: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
-00002880: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
-00002890: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
-000028a0: 6f72 7443 6f6c 756d 6e5f 1010 7573 6552  ortColumn_..useR
-000028b0: 656c 6174 6976 6544 6174 6573 5869 636f  elativeDatesXico
-000028c0: 6e53 697a 6510 0109 ab0e 171c 2125 2a2f  nSize.......!%*/
-000028d0: 3439 3e43 d40f 1011 1213 140c 0c5a 6964  49>C.........Zid
-000028e0: 656e 7469 6669 6572 5577 6964 7468 5961  entifierUwidthYa
-000028f0: 7363 656e 6469 6e67 5776 6973 6962 6c65  scendingWvisible
-00002900: 546e 616d 6511 0137 0909 d40f 1011 1218  Tname..7........
-00002910: 191a 1a58 7562 6971 7569 7479 1023 0808  ...Xubiquity.#..
-00002920: d40f 1011 121d 1e1a 0c5c 6461 7465 4d6f  .........\dateMo
-00002930: 6469 6669 6564 10b5 0809 d40f 1011 1222  dified........."
-00002940: 1e1a 1a5b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
-00002950: 08d4 0f10 1112 2627 1a0c 5473 697a 6510  ......&'..Tsize.
-00002960: 6108 09d4 0f10 1112 2b2c 0c0c 546b 696e  a.......+,..Tkin
-00002970: 6410 7309 09d4 0f10 1112 3031 0c1a 556c  d.s.......01..Ul
-00002980: 6162 656c 1064 0908 d40f 1011 1235 360c  abel.d.......56.
-00002990: 1a57 7665 7273 696f 6e10 4b09 08d4 0f10  .Wversion.K.....
-000029a0: 1112 3a3b 0c1a 5863 6f6d 6d65 6e74 7311  ..:;..Xcomments.
-000029b0: 012c 0908 d40f 1011 123f 401a 1a5e 6461  .,.......?@..^da
-000029c0: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
-000029d0: d40f 1011 1244 1e1a 1a59 6461 7465 4164  .....D...YdateAd
-000029e0: 6465 6408 0808 2300 0000 0000 0000 0023  ded...#........#
-000029f0: 4028 0000 0000 0000 546e 616d 6509 2340  @(......Tname.#@
-00002a00: 3000 0000 0000 0000 0800 1d00 3200 4400  0...........2.D.
-00002a10: 4c00 6000 7200 7b00 8d00 9800 ab00 b400  L.`.r.{.........
-00002a20: b600 b700 c300 cc00 d700 dd00 e700 ef00  ................
-00002a30: f400 f700 f800 f901 0201 0b01 0d01 0e01  ................
-00002a40: 0f01 1801 2501 2701 2801 2901 3201 3e01  ....%.'.(.).2.>.
-00002a50: 3f01 4001 4901 4e01 5001 5101 5201 5b01  ?.@.I.N.P.Q.R.[.
-00002a60: 6001 6201 6301 6401 6d01 7301 7501 7601  `.b.c.d.m.s.u.v.
-00002a70: 7701 8001 8801 8a01 8b01 8c01 9501 9e01  w...............
-00002a80: a101 a201 a301 ac01 bb01 bd01 be01 bf01  ................
-00002a90: c801 d201 d301 d401 d501 de01 e701 ec01  ................
-00002aa0: ed00 0000 0000 0002 0100 0000 0000 0000  ................
-00002ab0: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
-00002ac0: f600 0000 0300 6900 6d00 676c 7376 7062  ......i.m.glsvpb
-00002ad0: 6c6f 6200 0002 9562 706c 6973 7430 30da  lob....bplist00.
-00002ae0: 0102 0304 0506 0708 090a 0b0c 0d1c 4748  ..............GH
-00002af0: 4749 0c4b 5f10 1276 6965 774f 7074 696f  GI.K_..viewOptio
-00002b00: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
-00002b10: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00002b20: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00002b30: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
-00002b40: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
-00002b50: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
-00002b60: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e5f  ionXZsortColumn_
-00002b70: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
-00002b80: 6573 5869 636f 6e53 697a 6510 0109 d90e  esXiconSize.....
-00002b90: 0f10 1112 1314 1516 1720 2529 2d32 373c  ......... %)-27<
-00002ba0: 4158 636f 6d6d 656e 7473 5e64 6174 654c  AXcomments^dateL
-00002bb0: 6173 744f 7065 6e65 645c 6461 7465 4d6f  astOpened\dateMo
-00002bc0: 6469 6669 6564 5b64 6174 6543 7265 6174  dified[dateCreat
-00002bd0: 6564 5473 697a 6555 6c61 6265 6c54 6b69  edTsizeUlabelTki
-00002be0: 6e64 5776 6572 7369 6f6e 546e 616d 65d4  ndWversionTname.
-00002bf0: 1819 1a1b 1c1d 0c1f 5776 6973 6962 6c65  ........Wvisible
-00002c00: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-00002c10: 5569 6e64 6578 0811 012c 0910 07d4 1819  Uindex...,......
-00002c20: 1a1b 1c22 1c24 0810 c808 1008 d418 191a  ...".$..........
-00002c30: 1b0c 271c 0b09 10b5 08d4 1819 1a1b 1c27  ..'............'
-00002c40: 1c2c 0808 1002 d418 191a 1b0c 2f1c 3109  .,........../.1.
-00002c50: 1061 0810 03d4 1819 1a1b 1c34 0c36 0810  .a.........4.6..
-00002c60: 6409 1005 d418 191a 1b0c 390c 3b09 1073  d.........9.;..s
-00002c70: 0910 04d4 1819 1a1b 1c3e 0c40 0810 4b09  .........>.@..K.
-00002c80: 1006 d418 191a 1b0c 430c 4509 1101 3709  ........C.E...7.
-00002c90: 1000 0823 0000 0000 0000 0000 2340 2800  ...#........#@(.
-00002ca0: 0000 0000 0054 6e61 6d65 0923 4030 0000  .....Tname.#@0..
-00002cb0: 0000 0000 0008 001d 0032 0044 004c 0060  .........2.D.L.`
-00002cc0: 0072 007b 008d 0098 00ab 00b4 00b6 00b7  .r.{............
-00002cd0: 00ca 00d3 00e2 00ef 00fb 0100 0106 010b  ................
-00002ce0: 0113 0118 0121 0129 012f 0139 013f 0140  .....!.)./.9.?.@
-00002cf0: 0143 0144 0146 014f 0150 0152 0153 0155  .C.D.F.O.P.R.S.U
-00002d00: 015e 015f 0161 0162 016b 016c 016d 016f  .^._.a.b.k.l.m.o
-00002d10: 0178 0179 017b 017c 017e 0187 0188 018a  .x.y.{.|.~......
-00002d20: 018b 018d 0196 0197 0199 019a 019c 01a5  ................
-00002d30: 01a6 01a8 01a9 01ab 01b4 01b5 01b8 01b9  ................
-00002d40: 01bb 01bc 01c5 01ce 01d3 01d4 0000 0000  ................
-00002d50: 0000 0201 0000 0000 0000 004c 0000 0000  ...........L....
-00002d60: 0000 0000 0000 0000 0000 01dd 0000 0003  ................
-00002d70: 0069 006d 0067 6d6f 4444 626c 6f62 0000  .i.m.gmoDDblob..
-00002d80: 0008 69d3 090c 67f2 c441 0000 0003 0069  ..i...g..A.....i
-00002d90: 006d 0067 6d6f 6444 626c 6f62 0000 0008  .m.gmodDblob....
-00002da0: 69d3 090c 67f2 c441 0000 0003 0069 006d  i...g..A.....i.m
-00002db0: 0067 7068 3153 636f 6d70 0000 0000 0011  .gph1Scomp......
-00002dc0: 3000 0000 0003 0069 006d 0067 7653 726e  0......i.m.gvSrn
-00002dd0: 6c6f 6e67 0000 0001 0000 0007 006c 006f  long.........l.o
-00002de0: 006f 006b 0075 0070 0073 6277 7370 626c  .o.k.u.p.sbwspbl
-00002df0: 6f62 0000 00c8 6270 6c69 7374 3030 d701  ob....bplist00..
-00002e00: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-00002e10: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00002e20: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00002e30: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00002e40: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00002e50: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00002e60: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00002e70: 0809 0809 5f10 177b 7b30 2c20 3131 367d  ...._..{{0, 116}
-00002e80: 2c20 7b31 3235 302c 2037 3631 7d7d 0908  , {1250, 761}}..
-00002e90: 1725 313d 4960 6d79 7a7b 7c7d 7e98 0000  .%1=I`myz{|}~...
-00002ea0: 0000 0000 0101 0000 0000 0000 000f 0000  ................
-00002eb0: 0000 0000 0000 0000 0000 0000 0099 0000  ................
-00002ec0: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
-00002ed0: 6c67 3153 636f 6d70 0000 0000 0004 b1fb  lg1Scomp........
-00002ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002120: 626c 6f62 0000 02ba 6270 6c69 7374 3030  blob....bplist00
+00002130: da01 0203 0405 0607 0809 0a0b 0b0d 1a48  ...............H
+00002140: 494a 4b4c 4d5f 1010 7573 6552 656c 6174  IJKLM_..useRelat
+00002150: 6976 6544 6174 6573 5f10 0f73 686f 7749  iveDates_..showI
+00002160: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
+00002170: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
+00002180: 6c53 697a 6573 5f10 0f73 6372 6f6c 6c50  lSizes_..scrollP
+00002190: 6f73 6974 696f 6e59 5874 6578 7453 697a  ositionYXtextSiz
+000021a0: 655f 100f 7363 726f 6c6c 506f 7369 7469  e_..scrollPositi
+000021b0: 6f6e 585a 736f 7274 436f 6c75 6d6e 5869  onXZsortColumnXi
+000021c0: 636f 6e53 697a 655f 1012 7669 6577 4f70  conSize_..viewOp
+000021d0: 7469 6f6e 7356 6572 7369 6f6e 0909 ab0e  tionsVersion....
+000021e0: 171c 2125 2a2f 3439 3e43 d40f 1011 1213  ..!%*/49>C......
+000021f0: 140b 0b5a 6964 656e 7469 6669 6572 5577  ...ZidentifierUw
+00002200: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+00002210: 6973 6962 6c65 546e 616d 6510 ea09 09d4  isibleTname.....
+00002220: 0f10 1112 1819 1a1a 5875 6269 7175 6974  ........Xubiquit
+00002230: 7910 2308 08d4 0f10 1112 1d1e 1a0b 5c64  y.#...........\d
+00002240: 6174 654d 6f64 6966 6965 6410 b508 09d4  ateModified.....
+00002250: 0f10 1112 221e 1a1a 5b64 6174 6543 7265  ...."...[dateCre
+00002260: 6174 6564 0808 d40f 1011 1226 271a 0b54  ated.......&'..T
+00002270: 7369 7a65 1061 0809 d40f 1011 122b 2c0b  size.a.......+,.
+00002280: 0b54 6b69 6e64 1073 0909 d40f 1011 1230  .Tkind.s.......0
+00002290: 310b 1a55 6c61 6265 6c10 6409 08d4 0f10  1..Ulabel.d.....
+000022a0: 1112 3536 0b1a 5776 6572 7369 6f6e 104b  ..56..Wversion.K
+000022b0: 0908 d40f 1011 123a 3b0b 1a58 636f 6d6d  .......:;..Xcomm
+000022c0: 656e 7473 1101 2c09 08d4 0f10 1112 3f40  ents..,.......?@
+000022d0: 1a1a 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
+000022e0: 6410 c808 08d4 0f10 1112 441e 1a1a 5964  d.........D...Yd
+000022f0: 6174 6541 6464 6564 0808 0823 4056 c000  ateAdded...#@V..
+00002300: 0000 0000 2340 2800 0000 0000 0023 0000  ....#@(......#..
+00002310: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
+00002320: 0000 0000 1001 0008 001d 0030 0042 004a  ...........0.B.J
+00002330: 005e 0070 0079 008b 0096 009f 00b4 00b5  .^.p.y..........
+00002340: 00b6 00c2 00cb 00d6 00dc 00e6 00ee 00f3  ................
+00002350: 00f5 00f6 00f7 0100 0109 010b 010c 010d  ................
+00002360: 0116 0123 0125 0126 0127 0130 013c 013d  ...#.%.&.'.0.<.=
+00002370: 013e 0147 014c 014e 014f 0150 0159 015e  .>.G.L.N.O.P.Y.^
+00002380: 0160 0161 0162 016b 0171 0173 0174 0175  .`.a.b.k.q.s.t.u
+00002390: 017e 0186 0188 0189 018a 0193 019c 019f  .~..............
+000023a0: 01a0 01a1 01aa 01b9 01bb 01bc 01bd 01c6  ................
+000023b0: 01d0 01d1 01d2 01d3 01dc 01e5 01ee 01f3  ................
+000023c0: 01fc 0000 0000 0000 0201 0000 0000 0000  ................
+000023d0: 004e 0000 0000 0000 0000 0000 0000 0000  .N..............
+000023e0: 01fe 0000 0005 0069 0063 006f 006e 0073  .......i.c.o.n.s
+000023f0: 6c73 7670 626c 6f62 0000 029f 6270 6c69  lsvpblob....bpli
+00002400: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00002410: 0b0d 1c48 494a 4b4c 295f 1010 7573 6552  ...HIJKL)_..useR
+00002420: 656c 6174 6976 6544 6174 6573 5f10 0f73  elativeDates_..s
+00002430: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00002440: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00002450: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00002460: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+00002470: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+00002480: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+00002490: 6d6e 5869 636f 6e53 697a 655f 1012 7669  mnXiconSize_..vi
+000024a0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+000024b0: 0909 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
+000024c0: 2e33 383d 4258 636f 6d6d 656e 7473 5e64  .38=BXcomments^d
+000024d0: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
+000024e0: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
+000024f0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
+00002500: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
+00002510: 616d 65d4 1819 1a1b 1c1d 0b1f 5776 6973  ame.........Wvis
+00002520: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00002530: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
+00002540: 07d4 1819 1a1b 1c22 1c24 0810 c808 1008  .......".$......
+00002550: d418 191a 1b0b 271c 2909 10b5 0810 01d4  ......'.).......
+00002560: 1819 1a1b 1c27 1c2d 0808 1002 d418 191a  .....'.-........
+00002570: 1b0b 301c 3209 1061 0810 03d4 1819 1a1b  ..0.2..a........
+00002580: 1c35 0b37 0810 6409 1005 d418 191a 1b0b  .5.7..d.........
+00002590: 3a0b 3c09 1073 0910 04d4 1819 1a1b 1c3f  :.<..s.........?
+000025a0: 0b41 0810 4b09 1006 d418 191a 1b0b 440b  .A..K.........D.
+000025b0: 4609 10ea 0910 0008 2340 56c0 0000 0000  F.......#@V.....
+000025c0: 0023 4028 0000 0000 0000 2300 0000 0000  .#@(......#.....
+000025d0: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
+000025e0: 0000 0800 1d00 3000 4200 4a00 5e00 7000  ......0.B.J.^.p.
+000025f0: 7900 8b00 9600 9f00 b400 b500 b600 c900  y...............
+00002600: d200 e100 ee00 fa00 ff01 0501 0a01 1201  ................
+00002610: 1701 2001 2801 2e01 3801 3e01 3f01 4201  .. .(...8.>.?.B.
+00002620: 4301 4501 4e01 4f01 5101 5201 5401 5d01  C.E.N.O.Q.R.T.].
+00002630: 5e01 6001 6101 6301 6c01 6d01 6e01 7001  ^.`.a.c.l.m.n.p.
+00002640: 7901 7a01 7c01 7d01 7f01 8801 8901 8b01  y.z.|.}.........
+00002650: 8c01 8e01 9701 9801 9a01 9b01 9d01 a601  ................
+00002660: a701 a901 aa01 ac01 b501 b601 b801 b901  ................
+00002670: bb01 bc01 c501 ce01 d701 dc00 0000 0000  ................
+00002680: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+00002690: 0000 0000 0000 0000 0001 e500 0000 0500  ................
+000026a0: 6900 6300 6f00 6e00 736d 6f44 4462 6c6f  i.c.o.n.smoDDblo
+000026b0: 6200 0000 08c1 fc21 5522 f4c4 4100 0000  b......!U"..A...
+000026c0: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
+000026d0: 6c6f 6200 0000 08c1 fc21 5522 f4c4 4100  lob......!U"..A.
+000026e0: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
+000026f0: 5363 6f6d 7000 0000 0000 0800 0000 0000  Scomp...........
+00002700: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
+00002710: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
+00002720: 6762 7773 7062 6c6f 6200 0000 ca62 706c  gbwspblob....bpl
+00002730: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
+00002740: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+00002750: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
+00002760: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+00002770: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+00002780: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+00002790: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+000027a0: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
+000027b0: 3338 382c 2032 3136 7d2c 207b 3130 3932  388, 216}, {1092
+000027c0: 2c20 3432 327d 7d09 0817 2531 3d49 606d  , 422}}...%1=I`m
+000027d0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
+000027e0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+000027f0: 0000 0000 0000 9b00 0000 0300 6900 6d00  ............i.m.
+00002800: 676c 6731 5363 6f6d 7000 0000 0000 1110  glg1Scomp.......
+00002810: bf00 0000 0300 6900 6d00 676c 7376 4362  ......i.m.glsvCb
+00002820: 6c6f 6200 0002 b062 706c 6973 7430 30da  lob....bplist00.
+00002830: 0102 0304 0506 0708 090a 0b0c 0d1a 4849  ..............HI
+00002840: 484a 0c4c 5f10 1276 6965 774f 7074 696f  HJ.L_..viewOptio
+00002850: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+00002860: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00002870: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+00002880: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
+00002890: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
+000028a0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
+000028b0: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e5f  ionXZsortColumn_
+000028c0: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+000028d0: 6573 5869 636f 6e53 697a 6510 0109 ab0e  esXiconSize.....
+000028e0: 171c 2125 2a2f 3439 3e43 d40f 1011 1213  ..!%*/49>C......
+000028f0: 140c 0c5a 6964 656e 7469 6669 6572 5577  ...ZidentifierUw
+00002900: 6964 7468 5961 7363 656e 6469 6e67 5776  idthYascendingWv
+00002910: 6973 6962 6c65 546e 616d 6511 0137 0909  isibleTname..7..
+00002920: d40f 1011 1218 191a 1a58 7562 6971 7569  .........Xubiqui
+00002930: 7479 1023 0808 d40f 1011 121d 1e1a 0c5c  ty.#...........\
+00002940: 6461 7465 4d6f 6469 6669 6564 10b5 0809  dateModified....
+00002950: d40f 1011 1222 1e1a 1a5b 6461 7465 4372  ....."...[dateCr
+00002960: 6561 7465 6408 08d4 0f10 1112 2627 1a0c  eated.......&'..
+00002970: 5473 697a 6510 6108 09d4 0f10 1112 2b2c  Tsize.a.......+,
+00002980: 0c0c 546b 696e 6410 7309 09d4 0f10 1112  ..Tkind.s.......
+00002990: 3031 0c1a 556c 6162 656c 1064 0908 d40f  01..Ulabel.d....
+000029a0: 1011 1235 360c 1a57 7665 7273 696f 6e10  ...56..Wversion.
+000029b0: 4b09 08d4 0f10 1112 3a3b 0c1a 5863 6f6d  K.......:;..Xcom
+000029c0: 6d65 6e74 7311 012c 0908 d40f 1011 123f  ments..,.......?
+000029d0: 401a 1a5e 6461 7465 4c61 7374 4f70 656e  @..^dateLastOpen
+000029e0: 6564 10c8 0808 d40f 1011 1244 1e1a 1a59  ed.........D...Y
+000029f0: 6461 7465 4164 6465 6408 0808 2300 0000  dateAdded...#...
+00002a00: 0000 0000 0023 4028 0000 0000 0000 546e  .....#@(......Tn
+00002a10: 616d 6509 2340 3000 0000 0000 0000 0800  ame.#@0.........
+00002a20: 1d00 3200 4400 4c00 6000 7200 7b00 8d00  ..2.D.L.`.r.{...
+00002a30: 9800 ab00 b400 b600 b700 c300 cc00 d700  ................
+00002a40: dd00 e700 ef00 f400 f700 f800 f901 0201  ................
+00002a50: 0b01 0d01 0e01 0f01 1801 2501 2701 2801  ..........%.'.(.
+00002a60: 2901 3201 3e01 3f01 4001 4901 4e01 5001  ).2.>.?.@.I.N.P.
+00002a70: 5101 5201 5b01 6001 6201 6301 6401 6d01  Q.R.[.`.b.c.d.m.
+00002a80: 7301 7501 7601 7701 8001 8801 8a01 8b01  s.u.v.w.........
+00002a90: 8c01 9501 9e01 a101 a201 a301 ac01 bb01  ................
+00002aa0: bd01 be01 bf01 c801 d201 d301 d401 d501  ................
+00002ab0: de01 e701 ec01 ed00 0000 0000 0002 0100  ................
+00002ac0: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
+00002ad0: 0000 0000 0001 f600 0000 0300 6900 6d00  ............i.m.
+00002ae0: 676c 7376 7062 6c6f 6200 0002 9562 706c  glsvpblob....bpl
+00002af0: 6973 7430 30da 0102 0304 0506 0708 090a  ist00...........
+00002b00: 0b0c 0d1c 4748 4749 0c4b 5f10 1276 6965  ....GHGI.K_..vie
+00002b10: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
+00002b20: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
+00002b30: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
+00002b40: 756c 6174 6541 6c6c 5369 7a65 735f 100f  ulateAllSizes_..
+00002b50: 7363 726f 6c6c 506f 7369 7469 6f6e 5958  scrollPositionYX
+00002b60: 7465 7874 5369 7a65 5f10 0f73 6372 6f6c  textSize_..scrol
+00002b70: 6c50 6f73 6974 696f 6e58 5a73 6f72 7443  lPositionXZsortC
+00002b80: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
+00002b90: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
+00002ba0: 6510 0109 d90e 0f10 1112 1314 1516 1720  e.............. 
+00002bb0: 2529 2d32 373c 4158 636f 6d6d 656e 7473  %)-27<AXcomments
+00002bc0: 5e64 6174 654c 6173 744f 7065 6e65 645c  ^dateLastOpened\
+00002bd0: 6461 7465 4d6f 6469 6669 6564 5b64 6174  dateModified[dat
+00002be0: 6543 7265 6174 6564 5473 697a 6555 6c61  eCreatedTsizeUla
+00002bf0: 6265 6c54 6b69 6e64 5776 6572 7369 6f6e  belTkindWversion
+00002c00: 546e 616d 65d4 1819 1a1b 1c1d 0c1f 5776  Tname.........Wv
+00002c10: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
+00002c20: 656e 6469 6e67 5569 6e64 6578 0811 012c  endingUindex...,
+00002c30: 0910 07d4 1819 1a1b 1c22 1c24 0810 c808  .........".$....
+00002c40: 1008 d418 191a 1b0c 271c 0b09 10b5 08d4  ........'.......
+00002c50: 1819 1a1b 1c27 1c2c 0808 1002 d418 191a  .....'.,........
+00002c60: 1b0c 2f1c 3109 1061 0810 03d4 1819 1a1b  ../.1..a........
+00002c70: 1c34 0c36 0810 6409 1005 d418 191a 1b0c  .4.6..d.........
+00002c80: 390c 3b09 1073 0910 04d4 1819 1a1b 1c3e  9.;..s.........>
+00002c90: 0c40 0810 4b09 1006 d418 191a 1b0c 430c  .@..K.........C.
+00002ca0: 4509 1101 3709 1000 0823 0000 0000 0000  E...7....#......
+00002cb0: 0000 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
+00002cc0: 0923 4030 0000 0000 0000 0008 001d 0032  .#@0...........2
+00002cd0: 0044 004c 0060 0072 007b 008d 0098 00ab  .D.L.`.r.{......
+00002ce0: 00b4 00b6 00b7 00ca 00d3 00e2 00ef 00fb  ................
+00002cf0: 0100 0106 010b 0113 0118 0121 0129 012f  ...........!.)./
+00002d00: 0139 013f 0140 0143 0144 0146 014f 0150  .9.?.@.C.D.F.O.P
+00002d10: 0152 0153 0155 015e 015f 0161 0162 016b  .R.S.U.^._.a.b.k
+00002d20: 016c 016d 016f 0178 0179 017b 017c 017e  .l.m.o.x.y.{.|.~
+00002d30: 0187 0188 018a 018b 018d 0196 0197 0199  ................
+00002d40: 019a 019c 01a5 01a6 01a8 01a9 01ab 01b4  ................
+00002d50: 01b5 01b8 01b9 01bb 01bc 01c5 01ce 01d3  ................
+00002d60: 01d4 0000 0000 0000 0201 0000 0000 0000  ................
+00002d70: 004c 0000 0000 0000 0000 0000 0000 0000  .L..............
+00002d80: 01dd 0000 0003 0069 006d 0067 6d6f 4444  .......i.m.gmoDD
+00002d90: 626c 6f62 0000 0008 69d3 090c 67f2 c441  blob....i...g..A
+00002da0: 0000 0003 0069 006d 0067 6d6f 6444 626c  .....i.m.gmodDbl
+00002db0: 6f62 0000 0008 69d3 090c 67f2 c441 0000  ob....i...g..A..
+00002dc0: 0003 0069 006d 0067 7068 3153 636f 6d70  ...i.m.gph1Scomp
+00002dd0: 0000 0000 0011 3000 0000 0003 0069 006d  ......0......i.m
+00002de0: 0067 7653 726e 6c6f 6e67 0000 0001 0000  .gvSrnlong......
+00002df0: 0007 006c 006f 006f 006b 0075 0070 0073  ...l.o.o.k.u.p.s
+00002e00: 6277 7370 626c 6f62 0000 00c8 6270 6c69  bwspblob....bpli
+00002e10: 7374 3030 d701 0203 0405 0607 0808 0a08  st00............
+00002e20: 0a0d 0a5d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
+00002e30: 725b 5368 6f77 5061 7468 6261 725b 5368  r[ShowPathbar[Sh
+00002e40: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
+00002e50: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
+00002e60: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
+00002e70: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
+00002e80: 6465 6261 7208 0809 0809 5f10 177b 7b30  debar....._..{{0
+00002e90: 2c20 3131 367d 2c20 7b31 3235 302c 2037  , 116}, {1250, 7
+00002ea0: 3631 7d7d 0908 1725 313d 4960 6d79 7a7b  61}}...%1=I`myz{
+00002eb0: 7c7d 7e98 0000 0000 0000 0101 0000 0000  |}~.............
+00002ec0: 0000 000f 0000 0000 0000 0000 0000 0000  ................
+00002ed0: 0000 0099 0000 0007 006c 006f 006f 006b  .........l.o.o.k
+00002ee0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
+00002ef0: 0000 0004 b1fb 0000 0000 0000 0000 0000  ................
 00002f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -868,37 +868,37 @@
 00003630: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00003640: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00003650: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00003660: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00003670: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00003680: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00003690: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-000036a0: 01c5 5522 f4c4 4100 0000 0500 6900 6300  ..U"..A.....i.c.
-000036b0: 6f00 6e00 736d 6f64 4462 6c6f 6200 0000  o.n.smodDblob...
-000036c0: 08c1 fc21 5522 f4c4 4100 0000 0500 6900  ...!U"..A.....i.
-000036d0: 6300 6f00 6e00 7370 6831 5363 6f6d 7000  c.o.n.sph1Scomp.
-000036e0: 0000 0000 0800 0000 0000 0500 6900 6300  ............i.c.
-000036f0: 6f00 6e00 7376 5372 6e6c 6f6e 6700 0000  o.n.svSrnlong...
-00003700: 0100 0000 0300 6900 6d00 6762 7773 7062  ......i.m.gbwspb
-00003710: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
-00003720: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
-00003730: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00003740: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00003750: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00003760: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00003770: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00003780: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00003790: 0808 0908 095f 1019 7b7b 3338 382c 2032  ....._..{{388, 2
-000037a0: 3136 7d2c 207b 3130 3932 2c20 3432 327d  16}, {1092, 422}
-000037b0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-000037c0: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
-000037d0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-000037e0: 9b00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
-000037f0: 6f6d 7000 0000 0000 1110 bf00 0000 0300  omp.............
-00003800: 6900 6d00 0000 0006 0000 0000 0000 380b  i.m...........8.
+000036a0: 01c5 6300 6f00 6e00 736d 6f44 4462 6c6f  ..c.o.n.smoDDblo
+000036b0: 6200 0000 08c1 fc21 5522 f4c4 4100 0000  b......!U"..A...
+000036c0: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
+000036d0: 6c6f 6200 0000 08c1 fc21 5522 f4c4 4100  lob......!U"..A.
+000036e0: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
+000036f0: 5363 6f6d 7000 0000 0000 0800 0000 0000  Scomp...........
+00003700: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
+00003710: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
+00003720: 6762 7773 7062 6c6f 6200 0000 ca62 706c  gbwspblob....bpl
+00003730: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
+00003740: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+00003750: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
+00003760: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+00003770: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+00003780: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+00003790: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+000037a0: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
+000037b0: 3338 382c 2032 3136 7d2c 207b 3130 3932  388, 216}, {1092
+000037c0: 2c20 3432 327d 7d09 0817 2531 3d49 606d  , 422}}...%1=I`m
+000037d0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
+000037e0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+000037f0: 0000 0000 0000 9b00 0000 0300 6900 6d00  ............i.m.
+00003800: 676c 6731 0000 0006 0000 0000 0000 380b  glg1..........8.
 00003810: 0000 0045 0000 100b 0000 300b 0000 200c  ...E......0... .
 00003820: 0000 180b 0000 0000 0000 0000 0000 0000  ................
 00003830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -996,30 +996,30 @@
 00003e30: 011d 011e 011f 0128 012d 012f 0130 0131  .......(.-./.0.1
 00003e40: 013a 013f 0141 0142 0143 014c 0152 0154  .:.?.A.B.C.L.R.T
 00003e50: 0155 0156 015f 0167 0169 016a 016b 0174  .U.V._.g.i.j.k.t
 00003e60: 017d 0180 0181 0182 018b 019a 019c 019d  .}..............
 00003e70: 019e 01a7 01b1 01b2 01b3 01b4 01bd 01c2  ................
 00003e80: 01c3 0000 0000 0000 0201 0000 0000 0000  ................
 00003e90: 004a 0000 0000 0000 0000 0000 0000 0000  .J..............
-00003ea0: 01c5 5522 f4c4 4100 0000 0500 6900 6300  ..U"..A.....i.c.
-00003eb0: 6f00 6e00 736d 6f64 4462 6c6f 6200 0000  o.n.smodDblob...
-00003ec0: 08c1 fc21 5522 f4c4 4100 0000 0500 6900  ...!U"..A.....i.
-00003ed0: 6300 6f00 6e00 7370 6831 5363 6f6d 7000  c.o.n.sph1Scomp.
-00003ee0: 0000 0000 0800 0000 0000 0500 6900 6300  ............i.c.
-00003ef0: 6f00 6e00 7376 5372 6e6c 6f6e 6700 0000  o.n.svSrnlong...
-00003f00: 0100 0000 0300 6900 6d00 6762 7773 7062  ......i.m.gbwspb
-00003f10: 6c6f 6200 0000 ca62 706c 6973 7430 30d7  lob....bplist00.
-00003f20: 0102 0304 0506 0708 080a 080a 0d0a 5d53  ..............]S
-00003f30: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00003f40: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00003f50: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00003f60: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00003f70: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00003f80: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00003f90: 0808 0908 095f 1019 7b7b 3338 382c 2032  ....._..{{388, 2
-00003fa0: 3136 7d2c 207b 3130 3932 2c20 3432 327d  16}, {1092, 422}
-00003fb0: 7d09 0817 2531 3d49 606d 797a 7b7c 7d7e  }...%1=I`myz{|}~
-00003fc0: 9a00 0000 0000 0001 0100 0000 0000 0000  ................
-00003fd0: 0f00 0000 0000 0000 0000 0000 0000 0000  ................
-00003fe0: 9b00 0000 0300 6900 6d00 676c 6731 5363  ......i.m.glg1Sc
-00003ff0: 6f6d 7000 0000 0000 1110 bf00 0000 0300  omp.............
-00004000: 6900 6d00                                i.m.
+00003ea0: 01c5 6300 6f00 6e00 736d 6f44 4462 6c6f  ..c.o.n.smoDDblo
+00003eb0: 6200 0000 08c1 fc21 5522 f4c4 4100 0000  b......!U"..A...
+00003ec0: 0500 6900 6300 6f00 6e00 736d 6f64 4462  ..i.c.o.n.smodDb
+00003ed0: 6c6f 6200 0000 08c1 fc21 5522 f4c4 4100  lob......!U"..A.
+00003ee0: 0000 0500 6900 6300 6f00 6e00 7370 6831  ....i.c.o.n.sph1
+00003ef0: 5363 6f6d 7000 0000 0000 0800 0000 0000  Scomp...........
+00003f00: 0500 6900 6300 6f00 6e00 7376 5372 6e6c  ..i.c.o.n.svSrnl
+00003f10: 6f6e 6700 0000 0100 0000 0300 6900 6d00  ong.........i.m.
+00003f20: 6762 7773 7062 6c6f 6200 0000 ca62 706c  gbwspblob....bpl
+00003f30: 6973 7430 30d7 0102 0304 0506 0708 080a  ist00...........
+00003f40: 080a 0d0a 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+00003f50: 6172 5b53 686f 7750 6174 6862 6172 5b53  ar[ShowPathbar[S
+00003f60: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+00003f70: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+00003f80: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+00003f90: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+00003fa0: 6964 6562 6172 0808 0908 095f 1019 7b7b  idebar....._..{{
+00003fb0: 3338 382c 2032 3136 7d2c 207b 3130 3932  388, 216}, {1092
+00003fc0: 2c20 3432 327d 7d09 0817 2531 3d49 606d  , 422}}...%1=I`m
+00003fd0: 797a 7b7c 7d7e 9a00 0000 0000 0001 0100  yz{|}~..........
+00003fe0: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+00003ff0: 0000 0000 0000 9b00 0000 0300 6900 6d00  ............i.m.
+00004000: 676c 6731                                glg1
```

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.57.4/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.57.4/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.57.4/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.57.4/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.57.4/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.57.4/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.57.4/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.57.4/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.57.4/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/drop_bp_cords.py` & `Simba-UW-tf-dev-1.57.4/simba/drop_bp_cords.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/read_config_unit_tests.py` & `Simba-UW-tf-dev-1.57.4/simba/read_config_unit_tests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/project_config_creator.py` & `Simba-UW-tf-dev-1.57.4/simba/project_config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/set_hyperparameters.py` & `Simba-UW-tf-dev-1.57.4/simba/set_hyperparameters.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/train_single_model.py` & `Simba-UW-tf-dev-1.57.4/simba/train_single_model.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/create_clf_log.py` & `Simba-UW-tf-dev-1.57.4/simba/create_clf_log.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/.DS_Store` & `Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/batch_process_menus.py` & `Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.57.4/simba/batch_process_videos/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/Kleinberg_calculator.py` & `Simba-UW-tf-dev-1.57.4/simba/Kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/reorganize_keypoint_in_pose.py` & `Simba-UW-tf-dev-1.57.4/simba/reorganize_keypoint_in_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/simba/play_annotation_video.py` & `Simba-UW-tf-dev-1.57.4/simba/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.57.3
+Version: 1.57.4
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.57.4/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/LICENSE.md` & `Simba-UW-tf-dev-1.57.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/README.md` & `Simba-UW-tf-dev-1.57.4/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.57.3/setup.py` & `Simba-UW-tf-dev-1.57.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.57.3",
+    version="1.57.4",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

