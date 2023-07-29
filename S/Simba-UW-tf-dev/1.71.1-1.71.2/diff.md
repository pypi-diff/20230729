# Comparing `tmp/Simba-UW-tf-dev-1.71.1.tar.gz` & `tmp/Simba-UW-tf-dev-1.71.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.71.1.tar", last modified: Fri Jul 28 13:37:11 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.71.2.tar", last modified: Sat Jul 29 17:03:14 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.71.1.tar` & `Simba-UW-tf-dev-1.71.2.tar`

### file list

```diff
@@ -1,590 +1,591 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-20 15:49:37.000000 Simba-UW-tf-dev-1.71.1/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     9467 2023-07-28 12:57:31.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    18197 2023-07-08 16:32:57.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3070 2023-07-17 20:41:07.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3113 2023-07-27 13:28:29.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    50461 2023-07-09 20:50:15.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4573 2023-07-07 20:33:35.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.71.1/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.71.1/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.71.1/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.71.1/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.71.1/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.71.1/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.71.1/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.71.1/simba/labelling/labelling_interface_old.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.71.1/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.71.1/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.71.1/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.71.1/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.1/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-26 13:43:11.000000 Simba-UW-tf-dev-1.71.1/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     2387 2023-07-26 14:28:54.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/sleap_dam_nest.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      421 2023-07-05 19:50:18.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/shap_gpu.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)      908 2023-07-11 15:05:36.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/catch_error_annotation_field.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)      685 2023-07-11 15:09:54.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/catch_error_annotation_field.py.zip
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-26 13:43:11.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    23262 2023-07-25 20:15:35.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.71.1/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-26 13:43:11.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43031 2023-07-25 18:25:16.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    40235 2023-07-27 13:06:41.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/video_processing_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37255 2023-07-17 20:42:05.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    62985 2023-07-21 15:36:14.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    74613 2023-07-26 18:04:09.000000 Simba-UW-tf-dev-1.71.1/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.71.1/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.71.1/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-26 13:43:11.000000 Simba-UW-tf-dev-1.71.1/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8092 2023-07-20 21:09:08.000000 Simba-UW-tf-dev-1.71.1/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    13497 2023-07-09 20:29:02.000000 Simba-UW-tf-dev-1.71.1/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    45537 2023-07-26 00:29:03.000000 Simba-UW-tf-dev-1.71.1/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     9839 2023-07-21 15:26:44.000000 Simba-UW-tf-dev-1.71.1/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.71.1/simba/utils/cli/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.71.1/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15116 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.71.1/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    23056 2023-07-26 15:18:06.000000 Simba-UW-tf-dev-1.71.1/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.71.1/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/st/
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.71.1/simba/st/enums.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.71.1/simba/st/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.71.1/simba/st/select_groups_pg.py
--rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.71.1/simba/st/aggregate_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.71.1/simba/st/app.py
--rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.71.1/simba/st/welcome_page.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.71.1/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.71.1/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.71.1/simba/pose_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.71.1/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-20 15:49:37.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14362 2023-07-18 10:13:52.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)    14039 2023-07-19 18:19:28.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    14824 2023-07-05 12:33:51.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7683 2023-07-26 14:01:29.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8023 2023-07-27 12:49:42.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    16810 2023-07-08 16:29:21.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14496 2023-07-08 16:28:23.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10150 2023-07-27 12:49:42.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.71.1/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/dash_app/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.71.1/simba/dash_app/plotly_dash.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-26 13:43:11.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16228 2023-07-21 15:37:27.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)    11970 2023-07-27 13:43:36.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     7707 2023-07-28 13:15:17.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.71.1/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.71.1/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.71.1/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3581 2023-07-26 17:51:54.000000 Simba-UW-tf-dev-1.71.1/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.71.1/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3368 2023-07-23 17:59:08.000000 Simba-UW-tf-dev-1.71.1/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-26 13:43:11.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43474 2023-07-25 18:46:52.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20576 2023-07-23 18:10:48.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11606 2023-07-26 17:05:17.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2302 2023-07-25 18:18:07.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12548 2023-07-26 00:26:13.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.71.1/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/ui/
--rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/ui/define_px_to_mm_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-11 15:08:27.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/config_reader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/plotting_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/plotting/plot_pose_in_dir.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/pose_importers/anipose_csv_import.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.71.1/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    59566 2023-07-09 20:45:09.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-11 15:08:27.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    25261 2023-07-09 20:40:06.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/video_processing_new.py
--rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    13078 2023-07-05 13:23:30.000000 Simba-UW-tf-dev-1.71.1/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-11 15:08:27.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    66465 2023-07-27 12:59:37.000000 Simba-UW-tf-dev-1.71.1/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.71.1/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.71.1/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.71.1/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.71.1/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.71.1/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.71.1/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.71.1/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.1/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    22010 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-28 13:37:10.000000 Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.71.1/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.71.1/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.71.1/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.71.1/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.71.1/tests/test_interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.71.1/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.71.1/tests/test_pose_importers.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.71.1/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.71.1/tests/test_pose_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.71.1/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.71.1/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.71.1/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.71.1/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.71.1/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.71.1/tests/test_video_processors.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/video_processing/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/video_processing/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/video_processing/test_imgs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/expected_animal_bp_dict/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/models/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/models/generated_models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/models/validations/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/models/validations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/project_folder/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/project_folder/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/project_folder/videos/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/project_folder/logs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/project_folder/logs/measures/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.71.1/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.71.1/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.71.1/tests/test_roi_tools.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.71.1/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.71.1/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1905 2023-07-28 13:37:08.000000 Simba-UW-tf-dev-1.71.1/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-28 13:37:11.000000 Simba-UW-tf-dev-1.71.1/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-29 14:55:50.000000 Simba-UW-tf-dev-1.71.2/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     9467 2023-07-28 12:57:31.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    18197 2023-07-08 16:32:57.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3070 2023-07-17 20:41:07.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3113 2023-07-27 13:28:29.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    50461 2023-07-09 20:50:15.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4573 2023-07-07 20:33:35.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.71.2/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.71.2/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.71.2/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.71.2/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.71.2/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.71.2/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.71.2/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.71.2/simba/labelling/labelling_interface_old.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.71.2/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.71.2/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.71.2/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.71.2/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.71.2/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-29 14:55:50.000000 Simba-UW-tf-dev-1.71.2/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     2387 2023-07-26 14:28:54.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/sleap_dam_nest.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      421 2023-07-05 19:50:18.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/shap_gpu.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)      908 2023-07-11 15:05:36.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/catch_error_annotation_field.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)      685 2023-07-11 15:09:54.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/catch_error_annotation_field.py.zip
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-29 14:55:50.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    23262 2023-07-25 20:15:35.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.71.2/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-29 14:55:50.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43031 2023-07-25 18:25:16.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    40235 2023-07-27 13:06:41.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/video_processing_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37255 2023-07-17 20:42:05.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    62985 2023-07-21 15:36:14.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    74613 2023-07-26 18:04:09.000000 Simba-UW-tf-dev-1.71.2/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.71.2/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.71.2/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-29 14:55:50.000000 Simba-UW-tf-dev-1.71.2/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8092 2023-07-20 21:09:08.000000 Simba-UW-tf-dev-1.71.2/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    13497 2023-07-09 20:29:02.000000 Simba-UW-tf-dev-1.71.2/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    45537 2023-07-26 00:29:03.000000 Simba-UW-tf-dev-1.71.2/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     9839 2023-07-21 15:26:44.000000 Simba-UW-tf-dev-1.71.2/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.71.2/simba/utils/cli/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.71.2/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15116 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.71.2/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    23268 2023-07-28 13:47:22.000000 Simba-UW-tf-dev-1.71.2/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.71.2/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/st/
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.71.2/simba/st/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.71.2/simba/st/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.71.2/simba/st/select_groups_pg.py
+-rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.71.2/simba/st/aggregate_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.71.2/simba/st/app.py
+-rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.71.2/simba/st/welcome_page.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.71.2/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.71.2/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.71.2/simba/pose_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.71.2/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.71.2/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-29 14:55:50.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14362 2023-07-18 10:13:52.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)    14039 2023-07-19 18:19:28.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    14824 2023-07-05 12:33:51.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7683 2023-07-26 14:01:29.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8023 2023-07-27 12:49:42.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16810 2023-07-08 16:29:21.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14496 2023-07-08 16:28:23.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10150 2023-07-27 12:49:42.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.71.2/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/dash_app/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.71.2/simba/dash_app/plotly_dash.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-29 14:55:50.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    31153 2023-07-29 17:01:02.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16228 2023-07-21 15:37:27.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2490 2023-07-28 22:04:50.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/relative_distance_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)    11970 2023-07-27 13:43:36.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     7707 2023-07-28 13:15:17.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.71.2/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.71.2/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-29 14:55:50.000000 Simba-UW-tf-dev-1.71.2/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3581 2023-07-26 17:51:54.000000 Simba-UW-tf-dev-1.71.2/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.71.2/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3368 2023-07-23 17:59:08.000000 Simba-UW-tf-dev-1.71.2/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-26 13:43:11.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43474 2023-07-25 18:46:52.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20576 2023-07-23 18:10:48.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11606 2023-07-26 17:05:17.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2302 2023-07-25 18:18:07.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12548 2023-07-26 00:26:13.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.71.2/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/ui/define_px_to_mm_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-11 15:08:27.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/config_reader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/plotting_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/plotting/plot_pose_in_dir.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/pose_importers/anipose_csv_import.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.71.2/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    59566 2023-07-09 20:45:09.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-11 15:08:27.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    25261 2023-07-09 20:40:06.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/video_processing_new.py
+-rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    13078 2023-07-05 13:23:30.000000 Simba-UW-tf-dev-1.71.2/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-11 15:08:27.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    66465 2023-07-27 12:59:37.000000 Simba-UW-tf-dev-1.71.2/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.71.2/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.71.2/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.71.2/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.71.2/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.71.2/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.71.2/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.71.2/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.71.2/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    22064 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-29 17:03:13.000000 Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.71.2/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.71.2/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.71.2/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.71.2/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.71.2/tests/test_interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.71.2/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.71.2/tests/test_pose_importers.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.71.2/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.71.2/tests/test_pose_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.71.2/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.71.2/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.71.2/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.71.2/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.71.2/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.71.2/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.71.2/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.71.2/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.71.2/tests/test_roi_tools.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.71.2/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.71.2/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1905 2023-07-29 17:03:12.000000 Simba-UW-tf-dev-1.71.2/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-29 17:03:14.000000 Simba-UW-tf-dev-1.71.2/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.71.1/PKG-INFO` & `Simba-UW-tf-dev-1.71.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.71.1
+Version: 1.71.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/ui/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 00001150: 6261 7208 0809 0809 5f10 197b 7b33 3534  bar....._..{{354
 00001160: 2c20 3132 347d 2c20 7b31 3037 362c 2036  , 124}, {1076, 6
 00001170: 3231 7d7d 0908 1725 313d 4960 6d79 7a7b  21}}...%1=I`myz{
 00001180: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
 00001190: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 009b 0000 0007 0070 006f 0070 005f  .........p.o.p._
 000011b0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
-000011c0: 0000 000e 3180 0000 0007 0070 006f 0070  ....1......p.o.p
+000011c0: 0000 000e 493e 0000 0007 0070 006f 0070  ....I>.....p.o.p
 000011d0: 005f 0075 0070 0073 6c73 7643 626c 6f62  ._.u.p.slsvCblob
 000011e0: 0000 02b8 6270 6c69 7374 3030 da01 0203  ....bplist00....
 000011f0: 0405 0607 0809 0a0b 0c0d 1848 4948 4a0c  ...........HIHJ.
 00001200: 4c5f 1012 7669 6577 4f70 7469 6f6e 7356  L_..viewOptionsV
 00001210: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 00001220: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 00001230: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
@@ -369,20 +369,20 @@
 00001700: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
 00001710: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
 00001720: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
 00001730: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
 00001740: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
 00001750: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001760: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
-00001770: 6200 0000 0854 f9d9 71ef 32c5 4100 0000  b....T..q.2.A...
+00001770: 6200 0000 08ec d383 5df9 39c5 4100 0000  b.......].9.A...
 00001780: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001790: 6f64 4462 6c6f 6200 0000 0854 f9d9 71ef  odDblob....T..q.
-000017a0: 32c5 4100 0000 0700 7000 6f00 7000 5f00  2.A.....p.o.p._.
+00001790: 6f64 4462 6c6f 6200 0000 08ec d383 5df9  odDblob.......].
+000017a0: 39c5 4100 0000 0700 7000 6f00 7000 5f00  9.A.....p.o.p._.
 000017b0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-000017c0: 0000 13a0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+000017c0: 0000 13c0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
 000017d0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 000017e0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001800: 0000 0000 0000 0003 0000 0000 0000 180b  ................
 00001810: 0000 0045 0000 100b 0000 0000 0000 0000  ...E............
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -497,17 +497,17 @@
 00001f00: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
 00001f10: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
 00001f20: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
 00001f30: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
 00001f40: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
 00001f50: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001f60: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
-00001f70: 6200 0000 0854 f9d9 71ef 32c5 4100 0000  b....T..q.2.A...
+00001f70: 6200 0000 08ec d383 5df9 39c5 4100 0000  b.......].9.A...
 00001f80: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001f90: 6f64 4462 6c6f 6200 0000 0854 f9d9 71ef  odDblob....T..q.
-00001fa0: 32c5 4100 0000 0700 7000 6f00 7000 5f00  2.A.....p.o.p._.
+00001f90: 6f64 4462 6c6f 6200 0000 08ec d383 5df9  odDblob.......].
+00001fa0: 39c5 4100 0000 0700 7000 6f00 7000 5f00  9.A.....p.o.p._.
 00001fb0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-00001fc0: 0000 13a0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+00001fc0: 0000 13c0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
 00001fd0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 00001fe0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/animal_directing_other_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.71.2/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/labelling/labelling_interface_old.py` & `Simba-UW-tf-dev-1.71.2/simba/labelling/labelling_interface_old.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.71.2/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.71.2/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.71.2/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.71.2/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.71.2/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.71.2/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/.DS_Store`

 * *Files 1% similar despite different names*

```diff
@@ -765,16 +765,16 @@
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003000: 0000 0000 0000 0000 0000 0011 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6473 636c 626f  .u.t.i.l.sdsclbo
 00003020: 6f6c 0000 0000 0500 7500 7400 6900 6c00  ol......u.t.i.l.
-00003030: 736c 6731 5363 6f6d 7000 0000 0000 08e1  slg1Scomp.......
-00003040: 5a00 0000 0500 7500 7400 6900 6c00 736c  Z.....u.t.i.l.sl
+00003030: 736c 6731 5363 6f6d 7000 0000 0000 08e8  slg1Scomp.......
+00003040: 3100 0000 0500 7500 7400 6900 6c00 736c  1.....u.t.i.l.sl
 00003050: 7376 4362 6c6f 6200 0003 0f62 706c 6973  svCblob....bplis
 00003060: 7430 30d8 0102 0304 0506 0708 0909 0b16  t00.............
 00003070: 5657 5859 5f10 1075 7365 5265 6c61 7469  VWXY_..useRelati
 00003080: 7665 4461 7465 735f 100f 7368 6f77 4963  veDates_..showIc
 00003090: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
 000030a0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
 000030b0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
@@ -858,19 +858,19 @@
 00003590: 0149 014a 0153 0155 0156 0158 0159 0162  .I.J.S.U.V.X.Y.b
 000035a0: 0164 0165 0166 016f 0171 0172 0174 0175  .d.e.f.o.q.r.t.u
 000035b0: 017e 0180 0181 0184 0185 018e 0190 0191  .~..............
 000035c0: 0193 0194 0195 019e 01ab 0000 0000 0000  ................
 000035d0: 0201 0000 0000 0000 0049 0000 0000 0000  .........I......
 000035e0: 0000 0000 0000 0000 01b4 0000 0005 0075  ...............u
 000035f0: 0074 0069 006c 0073 6d6f 4444 626c 6f62  .t.i.l.smoDDblob
-00003600: 0000 0008 15c2 c9dd 5538 c541 0000 0005  ........U8.A....
+00003600: 0000 0008 0628 1c35 ff39 c541 0000 0005  .....(.5.9.A....
 00003610: 0075 0074 0069 006c 0073 6d6f 6444 626c  .u.t.i.l.smodDbl
-00003620: 6f62 0000 0008 401b 6772 5433 c541 0000  ob....@.grT3.A..
+00003620: 6f62 0000 0008 0628 1c35 ff39 c541 0000  ob.....(.5.9.A..
 00003630: 0005 0075 0074 0069 006c 0073 7068 3153  ...u.t.i.l.sph1S
-00003640: 636f 6d70 0000 0000 000a 8000 0000 0005  comp............
+00003640: 636f 6d70 0000 0000 000a 9000 0000 0005  comp............
 00003650: 0075 0074 0069 006c 0073 7653 726e 6c6f  .u.t.i.l.svSrnlo
 00003660: 6e67 0000 0001 0000 0010 0076 0069 0064  ng.........v.i.d
 00003670: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
 00003680: 0073 0073 006f 0072 0073 6277 7370 626c  .s.s.o.r.sbwspbl
 00003690: 6f62 0000 00b9 6270 6c69 7374 3030 d601  ob....bplist00..
 000036a0: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 000036b0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
@@ -1035,17 +1035,17 @@
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
 00004100: 005f 6c67 3153 636f 6d70 0000 0000 0002  ._lg1Scomp......
-00004110: 5ebf 0000 000b 005f 005f 0070 0079 0063  ^......_._.p.y.c
+00004110: 5d0f 0000 000b 005f 005f 0070 0079 0063  ]......_._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 55ee c677 912b c541  blob....U..w.+.A
+00004130: 626c 6f62 0000 0008 26c4 5ce3 5039 c541  blob....&.\.P9.A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
 00004160: 6f62 0000 0008 55ee c677 912b c541 0000  ob....U..w.+.A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
 00004190: 0000 0000 0002 a000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
@@ -1369,15 +1369,15 @@
 00005580: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 00005590: 0000 0000 0000 008c 0000 000f 0064 0061  .............d.a
 000055a0: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
 000055b0: 0073 0073 006f 0072 0073 6473 636c 626f  .s.s.o.r.sdsclbo
 000055c0: 6f6c 0000 0000 0f00 6400 6100 7400 6100  ol......d.a.t.a.
 000055d0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
 000055e0: 6f00 7200 736c 6731 5363 6f6d 7000 0000  o.r.slg1Scomp...
-000055f0: 0000 06dc 6a00 0000 0f00 6400 6100 7400  ....j.....d.a.t.
+000055f0: 0000 075a 6700 0000 0f00 6400 6100 7400  ...Zg.....d.a.t.
 00005600: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
 00005610: 7300 6f00 7200 736c 7376 4362 6c6f 6200  s.o.r.slsvCblob.
 00005620: 0002 8162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
 00005630: 0506 0708 090a 0b16 4647 480a 5f10 1276  ........FGH._..v
 00005640: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
 00005650: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
 00005660: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
@@ -1456,22 +1456,22 @@
 00005af0: 0165 016e 016f 0171 0172 0174 017d 017e  .e.n.o.q.r.t.}.~
 00005b00: 0180 0181 0183 018c 018d 0190 0191 0193  ................
 00005b10: 0194 019d 01aa 01b3 0000 0000 0000 0201  ................
 00005b20: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
 00005b30: 0000 0000 0000 01b4 0000 000f 0064 0061  .............d.a
 00005b40: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
 00005b50: 0073 0073 006f 0072 0073 6d6f 4444 626c  .s.s.o.r.smoDDbl
-00005b60: 6f62 0000 0008 6cba 0dab 9c35 c541 0000  ob....l....5.A..
+00005b60: 6f62 0000 0008 2abb 736b af3a c541 0000  ob....*.sk.:.A..
 00005b70: 000f 0064 0061 0074 0061 005f 0070 0072  ...d.a.t.a._.p.r
 00005b80: 006f 0063 0065 0073 0073 006f 0072 0073  .o.c.e.s.s.o.r.s
-00005b90: 6d6f 6444 626c 6f62 0000 0008 f03d b79f  modDblob.....=..
-00005ba0: 5533 c541 0000 000f 0064 0061 0074 0061  U3.A.....d.a.t.a
+00005b90: 6d6f 6444 626c 6f62 0000 0008 2abb 736b  modDblob....*.sk
+00005ba0: af3a c541 0000 000f 0064 0061 0074 0061  .:.A.....d.a.t.a
 00005bb0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
 00005bc0: 006f 0072 0073 7068 3153 636f 6d70 0000  .o.r.sph1Scomp..
-00005bd0: 0000 0008 c000 0000 000f 0064 0061 0074  ...........d.a.t
+00005bd0: 0000 0009 5000 0000 000f 0064 0061 0074  ....P......d.a.t
 00005be0: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
 00005bf0: 0073 006f 0072 0073 7653 726e 6c6f 6e67  .s.o.r.svSrnlong
 00005c00: 0000 0001 0000 0012 0066 0065 0061 0074  .........f.e.a.t
 00005c10: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
 00005c20: 0061 0063 0074 006f 0072 0073 6277 7370  .a.c.t.o.r.sbwsp
 00005c30: 626c 6f62 0000 00b9 6270 6c69 7374 3030  blob....bplist00
 00005c40: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
@@ -1487,15 +1487,15 @@
 00005ce0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
 00005cf0: 8c00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
 00005d00: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
 00005d10: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
 00005d20: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
 00005d30: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d40: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
-00005d50: 6d70 0000 0000 000b 85a3 d40d 0e0f 1016  mp..............
+00005d50: 6d70 0000 0000 000b 8a13 d40d 0e0f 1016  mp..............
 00005d60: 390a 3b08 1101 2c09 5863 6f6d 6d65 6e74  9.;...,.Xcomment
 00005d70: 73d4 0d0e 0f10 163e 1640 0810 c808 5e64  s......>.@....^d
 00005d80: 6174 654c 6173 744f 7065 6e65 64d4 0d0e  ateLastOpened...
 00005d90: 0f10 161c 1644 0808 5964 6174 6541 6464  .....D..YdateAdd
 00005da0: 6564 0823 4028 0000 0000 0000 546e 616d  ed.#@(......Tnam
 00005db0: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
 00005dc0: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
@@ -1712,15 +1712,15 @@
 00006af0: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
 00006b00: 0908 095f 1019 7b7b 3236 302c 2031 3239  ..._..{{260, 129
 00006b10: 7d2c 207b 3131 3830 2c20 3633 367d 7d09  }, {1180, 636}}.
 00006b20: 0815 232f 3b52 5f6b 6c6d 6e6f 8b00 0000  ..#/;R_klmno....
 00006b30: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
 00006b40: 0000 0000 0000 0000 0000 0000 8c00 0000  ................
 00006b50: 0600 6d00 6900 7800 6900 6e00 736c 6731  ..m.i.x.i.n.slg1
-00006b60: 5363 6f6d 7000 0000 0000 1084 ca00 0000  Scomp...........
+00006b60: 5363 6f6d 7000 0000 0000 1091 3e00 0000  Scomp.......>...
 00006b70: 0600 6d00 6900 7800 6900 6e00 736c 7376  ..m.i.x.i.n.slsv
 00006b80: 4362 6c6f 6200 0002 8162 706c 6973 7430  Cblob....bplist0
 00006b90: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
 00006ba0: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
 00006bb0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
 00006bc0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
 00006bd0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 191f 0153 3038 c541  blob.......S08.A
+00007020: 626c 6f62 0000 0008 6a97 a1b0 5139 c541  blob....j...Q9.A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 191f 0153  modDblob.......S
-00007050: 3038 c541 0000 0006 006d 0069 0078 0069  08.A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 6a97 a1b0  modDblob....j...
+00007050: 5139 c541 0000 0006 006d 0069 0078 0069  Q9.A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 0011 e000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 0011 f000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -1810,16 +1810,16 @@
 00007110: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00007120: 6261 7208 0809 0809 5f10 187b 7b33 3037  bar....._..{{307
 00007130: 2c20 3836 7d2c 207b 3130 3736 2c20 3632  , 86}, {1076, 62
 00007140: 317d 7d09 0817 2531 3d49 606d 797a 7b7c  1}}...%1=I`myz{|
 00007150: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
 00007160: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
 00007170: 0000 9a00 0000 0500 6d00 6f00 6400 6500  ........m.o.d.e.
-00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 020d  llg1Scomp.......
-00007190: fc00 0000 0500 6d00 6f00 6400 6500 6c6c  ......m.o.d.e.ll
+00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 020f  llg1Scomp.......
+00007190: 6b00 0000 0500 6d00 6f00 6400 6500 6c6c  k.....m.o.d.e.ll
 000071a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 000071b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 000071c0: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
 000071d0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 000071e0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 000071f0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
 00007200: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
@@ -1893,15 +1893,15 @@
 00007640: 014e 0150 0159 015a 015b 015d 015f 0168  .N.P.Y.Z.[.]._.h
 00007650: 0169 016a 016c 016e 0177 0178 0179 017b  .i.j.l.n.w.x.y.{
 00007660: 017d 0186 0187 0188 018a 018c 0195 0196  .}..............
 00007670: 0197 019a 019c 019d 01a6 01ab 0000 0000  ................
 00007680: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 00007690: 0000 0000 0000 0000 0000 01ac 0000 0005  ................
 000076a0: 006d 006f 0064 0065 006c 6d6f 4444 626c  .m.o.d.e.lmoDDbl
-000076b0: 6f62 0000 0008 f04f 49f6 d036 c541 0000  ob.....OI..6.A..
+000076b0: 6f62 0000 0008 f45b 6d5d ca38 c541 0000  ob.....[m].8.A..
 000076c0: 0005 006d 006f 0064 0065 006c 6d6f 6444  ...m.o.d.e.lmodD
 000076d0: 626c 6f62 0000 0008 574d 2d38 4017 c541  blob....WM-8@..A
 000076e0: 0000 0005 006d 006f 0064 0065 006c 7068  .....m.o.d.e.lph
 000076f0: 3153 636f 6d70 0000 0000 0002 7000 0000  1Scomp......p...
 00007700: 0005 006d 006f 0064 0065 006c 7653 726e  ...m.o.d.e.lvSrn
 00007710: 6c6f 6e67 0000 0001 0000 000d 006f 0075  long.........o.u
 00007720: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
@@ -2034,15 +2034,15 @@
 00007f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
 00007f20: 197b 7b32 3630 2c20 3132 397d 2c20 7b31  .{{260, 129}, {1
 00007f30: 3138 302c 2036 3336 7d7d 0908 1523 2f3b  180, 636}}...#/;
 00007f40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
 00007f50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 00007f60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
 00007f70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
-00007f80: 636f 6d70 0000 0000 0010 0360 0000 0000  comp.......`....
+00007f80: 636f 6d70 0000 0000 0010 0568 0000 0000  comp.......h....
 00007f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -2089,15 +2089,15 @@
 00008280: 017f 0181 018a 018b 018c 018e 0197 0198  ................
 00008290: 019a 019b 019d 01a6 01a7 01aa 01ab 01ad  ................
 000082a0: 01b6 01b7 01b9 01ba 01bc 01bd 01c6 01cf  ................
 000082b0: 01d8 01e5 0000 0000 0000 0201 0000 0000  ................
 000082c0: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
 000082d0: 0000 01ee 0000 0008 0070 006c 006f 0074  .........p.l.o.t
 000082e0: 0074 0069 006e 0067 6d6f 4444 626c 6f62  .t.i.n.gmoDDblob
-000082f0: 0000 0008 67cd 2b58 3034 c541 0000 0008  ....g.+X04.A....
+000082f0: 0000 0008 9612 10b3 4f39 c541 0000 0008  ........O9.A....
 00008300: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
 00008310: 6d6f 6444 626c 6f62 0000 0008 67cd 2b58  modDblob....g.+X
 00008320: 3034 c541 0000 0008 0070 006c 006f 0074  04.A.....p.l.o.t
 00008330: 0074 0069 006e 0067 7068 3153 636f 6d70  .t.i.n.gph1Scomp
 00008340: 0000 0000 0014 4000 0000 0008 0070 006c  ......@......p.l
 00008350: 006f 0074 0074 0069 006e 0067 7653 726e  .o.t.t.i.n.gvSrn
 00008360: 6c6f 6e67 0000 0001 0000 0013 0070 006f  long.........p.o
@@ -2290,15 +2290,15 @@
 00008f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
 00008f20: 197b 7b32 3630 2c20 3132 397d 2c20 7b31  .{{260, 129}, {1
 00008f30: 3138 302c 2036 3336 7d7d 0908 1523 2f3b  180, 636}}...#/;
 00008f40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
 00008f50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 00008f60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
 00008f70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
-00008f80: 636f 6d70 0000 0000 0010 0360 0000 0000  comp.......`....
+00008f80: 636f 6d70 0000 0000 0010 0568 0000 0000  comp.......h....
 00008f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -2484,15 +2484,15 @@
 00009b30: 6964 6562 6172 0809 0809 5f10 197b 7b32  idebar...._..{{2
 00009b40: 3630 2c20 3132 397d 2c20 7b31 3138 302c  60, 129}, {1180,
 00009b50: 2036 3336 7d7d 0908 1523 2f3b 525f 6b6c   636}}...#/;R_kl
 00009b60: 6d6e 6f8b 0000 0000 0000 0101 0000 0000  mno.............
 00009b70: 0000 000d 0000 0000 0000 0000 0000 0000  ................
 00009b80: 0000 008c 0000 0009 0072 006f 0069 005f  .........r.o.i._
 00009b90: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
-00009ba0: 6d70 0000 0000 0007 a12c 0000 0009 0072  mp.......,.....r
+00009ba0: 6d70 0000 0000 0007 a12a 0000 0009 0072  mp.......*.....r
 00009bb0: 006f 0069 005f 0074 006f 006f 006c 0073  .o.i._.t.o.o.l.s
 00009bc0: 6c73 7643 626c 6f62 0000 030f 6270 6c69  lsvCblob....bpli
 00009bd0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 00009be0: 1656 570a 5958 6963 6f6e 5369 7a65 5f10  .VW.YXiconSize_.
 00009bf0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 00009c00: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
 00009c10: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
@@ -2546,26 +2546,26 @@
 00009f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
 00009f20: 197b 7b32 3630 2c20 3132 397d 2c20 7b31  .{{260, 129}, {1
 00009f30: 3138 302c 2036 3336 7d7d 0908 1523 2f3b  180, 636}}...#/;
 00009f40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
 00009f50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 00009f60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
 00009f70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
-00009f80: 636f 6d70 0000 0000 0010 0360 0000 0000  comp.......`....
+00009f80: 636f 6d70 0000 0000 0010 0568 0000 0000  comp.......h....
 00009f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000a000: 0000 0000 0000 0000 0000 001a 0000 0009  ................
 0000a010: 0072 006f 0069 005f 0074 006f 006f 006c  .r.o.i._.t.o.o.l
-0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 a613  .smoDDblob......
-0000a030: 520e 2838 c541 0000 0009 0072 006f 0069  R.(8.A.....r.o.i
+0000a020: 0073 6d6f 4444 626c 6f62 0000 0008 0d5b  .smoDDblob.....[
+0000a030: dce6 c438 c541 0000 0009 0072 006f 0069  ...8.A.....r.o.i
 0000a040: 005f 0074 006f 006f 006c 0073 6d6f 6444  ._.t.o.o.l.smodD
 0000a050: 626c 6f62 0000 0008 a613 520e 2838 c541  blob......R.(8.A
 0000a060: 0000 0009 0072 006f 0069 005f 0074 006f  .....r.o.i._.t.o
 0000a070: 006f 006c 0073 7068 3153 636f 6d70 0000  .o.l.sph1Scomp..
 0000a080: 0000 0009 9000 0000 0009 0072 006f 0069  ...........r.o.i
 0000a090: 005f 0074 006f 006f 006c 0073 7653 726e  ._.t.o.o.l.svSrn
 0000a0a0: 6c6f 6e67 0000 0001 0000 0002 0073 0074  long.........s.t
@@ -2744,16 +2744,16 @@
 0000ab70: 5369 6465 6261 7208 0809 0809 5f10 197b  Sidebar....._..{
 0000ab80: 7b33 3534 2c20 3132 347d 2c20 7b31 3037  {354, 124}, {107
 0000ab90: 362c 2036 3231 7d7d 0908 1725 313d 4960  6, 621}}...%1=I`
 0000aba0: 6d79 7a7b 7c7d 7e9a 0000 0000 0000 0101  myz{|}~.........
 0000abb0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
 0000abc0: 0000 0000 0000 009b 0000 0002 0075 0069  .............u.i
 0000abd0: 6473 636c 626f 6f6c 0000 0000 0200 7500  dsclbool......u.
-0000abe0: 696c 6731 5363 6f6d 7000 0000 0000 1226  ilg1Scomp......&
-0000abf0: e200 0000 0200 7500 696c 7376 4362 6c6f  ......u.ilsvCblo
+0000abe0: 696c 6731 5363 6f6d 7000 0000 0000 123e  ilg1Scomp......>
+0000abf0: a000 0000 0200 7500 696c 7376 4362 6c6f  ......u.ilsvCblo
 0000ac00: 6200 0002 7962 706c 6973 7430 30d8 0102  b...ybplist00...
 0000ac10: 0304 0506 0708 090a 0b18 4647 480a 5f10  ..........FGH._.
 0000ac20: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
 0000ac30: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
 0000ac40: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
 0000ac50: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
 0000ac60: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
@@ -2802,28 +2802,28 @@
 0000af10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
 0000af20: 197b 7b32 3630 2c20 3132 397d 2c20 7b31  .{{260, 129}, {1
 0000af30: 3138 302c 2036 3336 7d7d 0908 1523 2f3b  180, 636}}...#/;
 0000af40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
 0000af50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 0000af60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
 0000af70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
-0000af80: 636f 6d70 0000 0000 0010 0360 0000 0000  comp.......`....
+0000af80: 636f 6d70 0000 0000 0010 0568 0000 0000  comp.......h....
 0000af90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000d 0000 0002  ................
 0000b010: 0075 0069 6d6f 4444 626c 6f62 0000 0008  .u.imoDDblob....
 0000b020: 7eab ce1c d01f c541 0000 0002 0075 0069  ~......A.....u.i
 0000b030: 6d6f 6444 626c 6f62 0000 0008 7eab ce1c  modDblob....~...
 0000b040: d01f c541 0000 0002 0075 0069 7068 3153  ...A.....u.iph1S
-0000b050: 636f 6d70 0000 0000 0018 6000 0000 0002  comp......`.....
+0000b050: 636f 6d70 0000 0000 0018 8000 0000 0002  comp............
 0000b060: 0075 0069 7653 726e 6c6f 6e67 0000 0001  .u.ivSrnlong....
 0000b070: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
 0000b080: 0072 0076 0069 0073 0065 0064 6277 7370  .r.v.i.s.e.dbwsp
 0000b090: 626c 6f62 0000 00ca 6270 6c69 7374 3030  blob....bplist00
 0000b0a0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
 0000b0b0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
 0000b0c0: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/sleap_dam_nest.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/sleap_dam_nest.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/catch_error_annotation_field.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/catch_error_annotation_field.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/catch_error_annotation_field.py.zip` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/catch_error_annotation_field.py.zip`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -276,18 +276,18 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 0004 53d1 0000 000b 005f 005f 0070  ....S......_._.p
+000011a0: 0000 0004 53dc 0000 000b 005f 005f 0070  ....S......_._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 1da3 1858  moDDblob.......X
-000011d0: 2f38 c541 0000 000b 005f 005f 0070 0079  /8.A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 8b0e 430d  moDDblob......C.
+000011d0: af38 c541 0000 000b 005f 005f 0070 0079  .8.A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 000011f0: 6444 626c 6f62 0000 0008 1da3 1858 2f38  dDblob.......X/8
 00001200: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 00001220: 636f 6d70 0000 0000 0005 1000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
@@ -303,15 +303,15 @@
 000012e0: 302c 2031 3239 7d2c 207b 3131 3830 2c20  0, 129}, {1180, 
 000012f0: 3633 367d 7d09 0815 232f 3b52 5f6b 6c6d  636}}...#/;R_klm
 00001300: 6e6f 8b00 0000 0000 0001 0100 0000 0000  no..............
 00001310: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
 00001320: 0000 8c00 0000 0400 6d00 6900 7300 6364  ........m.i.s.cd
 00001330: 7363 6c62 6f6f 6c00 0000 0004 006d 0069  sclbool......m.i
 00001340: 0073 0063 6c67 3153 636f 6d70 0000 0000  .s.clg1Scomp....
-00001350: 0003 2b2c 0000 0004 006d 0069 0073 0063  ..+,.....m.i.s.c
+00001350: 0003 2f91 0000 0004 006d 0069 0073 0063  ../......m.i.s.c
 00001360: 6c73 7643 626c 6f62 0000 0346 6270 6c69  lsvCblob...Fbpli
 00001370: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
 00001380: 0c0d 1a58 5958 5a0c 5c5f 1012 7669 6577  ...XYXZ.\_..view
 00001390: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
 000013a0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 000013b0: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
 000013c0: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
@@ -401,16 +401,16 @@
 00001900: 6101 6201 6401 6d01 6e01 7001 7101 7301  a.b.d.m.n.p.q.s.
 00001910: 7c01 7d01 7f01 8001 8201 8b01 8c01 8d01  |.}.............
 00001920: 9601 9701 9901 9a01 9c01 a501 a701 aa01  ................
 00001930: ab01 ac01 b501 b601 b801 b901 bb01 bc01  ................
 00001940: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
 00001950: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
 00001960: 0000 0000 0001 e500 0000 0400 6d00 6900  ............m.i.
-00001970: 7300 636d 6f44 4462 6c6f 6200 0000 08d2  s.cmoDDblob.....
-00001980: eceb 7a56 38c5 4100 0000 0400 6d00 6900  ..zV8.A.....m.i.
+00001970: 7300 636d 6f44 4462 6c6f 6200 0000 0849  s.cmoDDblob....I
+00001980: db2f 93b2 38c5 4100 0000 0400 6d00 6900  ./..8.A.....m.i.
 00001990: 7300 636d 6f64 4462 6c6f 6200 0000 08d2  s.cmodDblob.....
 000019a0: eceb 7a56 38c5 4100 0000 0400 6d00 6900  ..zV8.A.....m.i.
 000019b0: 7300 6370 6831 5363 6f6d 7000 0000 0000  s.cph1Scomp.....
 000019c0: 0450 0000 0000 0400 6d00 6900 7300 6376  .P......m.i.s.cv
 000019d0: 5372 6e6c 6f6e 6700 0000 0100 0000 0000  Srnlong.........
 000019e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.71.2/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/requirements.txt` & `Simba-UW-tf-dev-1.71.2/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/utils/cli/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 000c 0bc2 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0000 1281 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 2a46 1559  moDDblob....*F.Y
-00000160: 3038 c541 0000 000b 005f 005f 0070 0079  08.A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 e40f 369b  moDDblob......6.
+00000160: 8b2b c541 0000 000b 005f 005f 0070 0079  .+.A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 2a46 1559 3038  dDblob....*F.Y08
+00000180: 6444 626c 6f62 0000 0008 e40f 369b 8b2b  dDblob......6..+
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 000d 2000 0000 0000  comp...... .....
+000001b0: 636f 6d70 0000 0000 0000 3000 0000 0000  comp......0.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.71.2/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.71.2/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.71.2/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.71.2/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.71.2/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.71.2/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.71.2/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.71.2/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.71.2/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.71.2/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.71.2/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/enums.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/utils/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -253,23 +253,23 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000e 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0006 308e 0000 000b 005f 005f 0070  ....0......_._.p
+00001030: 0000 0006 3470 0000 000b 005f 005f 0070  ....4p....._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 6dc1 49e1  moDDblob....m.I.
-00001060: 5538 c541 0000 000b 005f 005f 0070 0079  U8.A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 a20e 9820  moDDblob....... 
+00001060: 013a c541 0000 000b 005f 005f 0070 0079  .:.A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 4cd1 6098 5433  dDblob....L.`.T3
+00001080: 6444 626c 6f62 0000 0008 a20e 9820 013a  dDblob....... .:
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0007 5000 0000 0003  comp......P.....
+000010b0: 636f 6d70 0000 0000 0007 6000 0000 0003  comp......`.....
 000010c0: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
 000010d0: 00b9 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
 000010e0: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
 000010f0: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
 00001100: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00001110: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00001120: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/checks.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/cli/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0000 1281 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0005 18f0 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 e40f 369b  moDDblob......6.
-00000160: 8b2b c541 0000 000b 005f 005f 0070 0079  .+.A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 46c7 c352  moDDblob....F..R
+00000160: 2f38 c541 0000 000b 005f 005f 0070 0079  /8.A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 e40f 369b 8b2b  dDblob......6..+
+00000180: 6444 626c 6f62 0000 0008 eb3d 5300 5726  dDblob.....=S.W&
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0000 3000 0000 0000  comp......0.....
+000001b0: 636f 6d70 0000 0000 0006 a000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/errors.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/data.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,17 +448,20 @@
                       headers: List[str],
                       joined_tracks: Optional[bool] = False,
                       multi_index: Optional[bool] = True) -> pd.DataFrame:
     """
     Helper to convert .slp pose-estimation data to pandas dataframe.
 
     :param Union[str, os.PathLike] file_path: Path to .slp file on disk.
-    :param List[str] headers: List of strings representing dataframe headers.
+    :param List[str] headers: List of strings representing output dataframe headers.
     :param bool joined_tracks: If True, the .slp file has been created by joining multiple .slp files.
     :param bool multi_index: If True, inserts multi-index place-holders in the output dataframe (used in SimBA data import).
+    :raises InvalidFileTypeError: If ``file_path`` is not a valid SLEAP H5 pose-estimation file.
+    :raises DataHeaderError: If sleap file contains more or less body-parts than suggested by len(headers)
+
     :return pd.DataFrame.
     """
 
     try:
         with h5py.File(file_path, "r") as sleap_dict:
             data = {k: v[()] for k, v in sleap_dict.items()}
             data["node_names"] = [s.decode() for s in data["node_names"].tolist()]
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/utils/printing.py` & `Simba-UW-tf-dev-1.71.2/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/st/select_groups_pg.py` & `Simba-UW-tf-dev-1.71.2/simba/st/select_groups_pg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/st/aggregate_statistics.py` & `Simba-UW-tf-dev-1.71.2/simba/st/aggregate_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/st/app.py` & `Simba-UW-tf-dev-1.71.2/simba/st/app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_processors/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/plotting/.DS_Store`

 * *Files 4% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
 00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000230: 0000 000a 65b7 0000 000b 005f 005f 0070  ....e......_._.p
+00000230: 0000 000a 6693 0000 000b 005f 005f 0070  ....f......_._.p
 00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000250: 6d6f 4444 626c 6f62 0000 0008 9f76 abaf  moDDblob.....v..
-00000260: 3034 c541 0000 000b 005f 005f 0070 0079  04.A....._._.p.y
+00000250: 6d6f 4444 626c 6f62 0000 0008 fd60 fae9  moDDblob.....`..
+00000260: 5039 c541 0000 000b 005f 005f 0070 0079  P9.A....._._.p.y
 00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 00000280: 6444 626c 6f62 0000 0008 9f76 abaf 3034  dDblob.....v..04
 00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 000002b0: 636f 6d70 0000 0000 000d 8000 0000 0005  comp............
 000002c0: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
 000002d0: 6d70 0000 0000 0000 50f8 0000 0005 0074  mp......P......t
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.71.2/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.71.2/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.71.2/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.71.2/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0004 8f62 0000 000b 005f 005f 0070  .....b....._._.p
+00000130: 0000 0004 bcc4 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 e268 5c6c  moDDblob.....h\l
-00000160: 2c36 c541 0000 000b 005f 005f 0070 0079  ,6.A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 4715 d650  moDDblob....G..P
+00000160: ac3a c541 0000 000b 005f 005f 0070 0079  .:.A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 ad39 b7ae 5533  dDblob.....9..U3
+00000180: 6444 626c 6f62 0000 0008 4715 d650 ac3a  dDblob....G..P.:
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0006 1000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0006 5000 0000 0000  comp......P.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.71.2/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/model/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 000002b0: 5f10 187b 7b33 3335 2c20 3139 387d 2c20  _..{{335, 198}, 
 000002c0: 7b39 3237 2c20 3536 387d 7d09 0817 2531  {927, 568}}...%1
 000002d0: 3d49 606d 797a 7b7c 7d7e 9900 0000 0000  =I`myz{|}~......
 000002e0: 0001 0100 0000 0000 0000 0f00 0000 0000  ................
 000002f0: 0000 0000 0000 0000 0000 9a00 0000 0b00  ................
 00000300: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 00000310: 6500 5f00 5f6c 6731 5363 6f6d 7000 0000  e._._lg1Scomp...
-00000320: 0000 013b f600 0000 0b00 5f00 5f00 7000  ...;......_._.p.
+00000320: 0000 013c 5b00 0000 0b00 5f00 5f00 7000  ...<[....._._.p.
 00000330: 7900 6300 6100 6300 6800 6500 5f00 5f6d  y.c.a.c.h.e._._m
-00000340: 6f44 4462 6c6f 6200 0000 0878 db7a 237b  oDDblob....x.z#{
-00000350: 20c5 4100 0000 0b00 5f00 5f00 7000 7900   .A....._._.p.y.
+00000340: 6f44 4462 6c6f 6200 0000 08d5 1d5b 6fd5  oDDblob......[o.
+00000350: 38c5 4100 0000 0b00 5f00 5f00 7000 7900  8.A....._._.p.y.
 00000360: 6300 6100 6300 6800 6500 5f00 5f6d 6f64  c.a.c.h.e._._mod
 00000370: 4462 6c6f 6200 0000 0878 db7a 237b 20c5  Dblob....x.z#{ .
 00000380: 4100 0000 0b00 5f00 5f00 7000 7900 6300  A....._._.p.y.c.
 00000390: 6100 6300 6800 6500 5f00 5f70 6831 5363  a.c.h.e._._ph1Sc
 000003a0: 6f6d 7000 0000 0000 0180 0000 0000 0b00  omp.............
 000003b0: 5f00 5f00 7000 7900 6300 6100 6300 6800  _._.p.y.c.a.c.h.
 000003c0: 6500 5f00 5f76 5372 6e6c 6f6e 6700 0000  e._._vSrnlong...
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.71.2/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.71.2/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.71.2/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.DS_Store`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
-00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
-00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
+00000050: 0000 0001 0000 1000 0061 6c67 3153 636f  .........alg1Sco
+00000060: 6d70 0000 0000 0000 0000 0000 0000 0000  mp..............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
-00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0005 18f0 0000 000b 005f 005f 0070  ..........._._.p
-00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 46c7 c352  moDDblob....F..R
-00000160: 2f38 c541 0000 000b 005f 005f 0070 0079  /8.A....._._.p.y
-00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 eb3d 5300 5726  dDblob.....=S.W&
-00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0006 a000 0000 0000  comp............
+00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0008 0000 0005  ................
+00000210: 002e 0069 0064 0065 0061 6c67 3153 636f  ...i.d.e.alg1Sco
+00000220: 6d70 0000 0000 0000 27fc 0000 0005 002e  mp......'.......
+00000230: 0069 0064 0065 0061 6d6f 4444 626c 6f62  .i.d.e.amoDDblob
+00000240: 0000 0008 993b 4774 e2dd c441 0000 0005  .....;Gt...A....
+00000250: 002e 0069 0064 0065 0061 6d6f 6444 626c  ...i.d.e.amodDbl
+00000260: 6f62 0000 0008 993b 4774 e2dd c441 0000  ob.....;Gt...A..
+00000270: 0005 002e 0069 0064 0065 0061 7068 3153  .....i.d.e.aph1S
+00000280: 636f 6d70 0000 0000 0000 8000 0000 000b  comp............
+00000290: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+000002a0: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+000002b0: 0000 0000 addd 0000 000b 005f 005f 0070  ..........._._.p
+000002c0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+000002d0: 6d6f 4444 626c 6f62 0000 0008 0265 3b14  moDDblob.....e;.
+000002e0: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
+000002f0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00000300: 6444 626c 6f62 0000 0008 0265 3b14 7b20  dDblob.....e;.{ 
+00000310: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+00000320: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+00000330: 636f 6d70 0000 0000 0001 2000 0000 0000  comp...... .....
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
+00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.71.2/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.71.2/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.71.2/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/ui/define_px_to_mm_ui.py` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/ui/define_px_to_mm_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/feature_extractors/generic_feature_extractor.py` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/feature_extractors/generic_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/config_reader.py` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/pose_importers/anipose_csv_import.py` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/pose_importers/anipose_csv_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.71.2/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/video_processing_new.py` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/video_processing_new.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.71.2/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.71.2/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.71.2/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.71.2/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.71.2/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/SimBA.py` & `Simba-UW-tf-dev-1.71.2/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.71.2/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.71.2/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.71.2/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.71.2/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.71.2/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.71.2/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.71.2/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.71.2/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.71.2/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.71.2/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.71.2/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.71.2/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.71.2/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.71.2/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.71.2/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.71.2/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.71.2/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.71.1
+Version: 1.71.2
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 simba/data_processors/interpolate_pose.py
 simba/data_processors/interpolation_smoothing.py
 simba/data_processors/kleinberg_calculator.py
 simba/data_processors/movement_calculator.py
 simba/data_processors/mutual_exclusivity_corrector.py
 simba/data_processors/pup_retrieval_calculator.py
 simba/data_processors/pybursts_calculator.py
+simba/data_processors/relative_distance_calculator.py
 simba/data_processors/severity_bout_based_calculator.py
 simba/data_processors/severity_calculator.py
 simba/data_processors/severity_frame_based_calculator.py
 simba/data_processors/timebins_clf_calculator.py
 simba/data_processors/timebins_movement_calculator.py
 simba/feature_extractors/.DS_Store
 simba/feature_extractors/__init__.py
```

### Comparing `Simba-UW-tf-dev-1.71.1/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.71.2/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/LICENSE.md` & `Simba-UW-tf-dev-1.71.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.71.2/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.71.2/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.71.2/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_pose_importers.py` & `Simba-UW-tf-dev-1.71.2/tests/test_pose_importers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.71.2/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.71.2/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.71.2/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.71.2/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.71.2/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.71.2/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.71.2/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.71.2/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.71.2/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.71.2/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.71.2/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/README.md` & `Simba-UW-tf-dev-1.71.2/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.71.1/setup.py` & `Simba-UW-tf-dev-1.71.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-            version="1.71.1",
+            version="1.71.2",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

