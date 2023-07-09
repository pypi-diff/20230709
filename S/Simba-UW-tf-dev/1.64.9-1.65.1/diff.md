# Comparing `tmp/Simba-UW-tf-dev-1.64.9.tar.gz` & `tmp/Simba-UW-tf-dev-1.65.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.64.9.tar", last modified: Sat Jul  8 16:36:45 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.65.1.tar", last modified: Sun Jul  9 20:51:15 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.64.9.tar` & `Simba-UW-tf-dev-1.65.1.tar`

### file list

```diff
@@ -1,584 +1,585 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.9/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     9015 2023-06-29 20:55:17.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    18197 2023-07-08 16:32:57.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    50444 2023-07-05 17:57:07.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4573 2023-07-07 20:33:35.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.64.9/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.64.9/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.64.9/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.64.9/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.64.9/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.64.9/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.9/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.64.9/simba/labelling/labelling_interface_old.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.64.9/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.64.9/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.64.9/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.64.9/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.9/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.9/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      421 2023-07-05 19:50:18.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/shap_gpu.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    22875 2023-07-07 20:39:37.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.64.9/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    38471 2023-07-07 19:58:19.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/video_processing_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.64.9/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.64.9/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.64.9/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.9/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7801 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.64.9/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)    11291 2023-07-08 15:46:46.000000 Simba-UW-tf-dev-1.64.9/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43615 2023-07-05 18:25:40.000000 Simba-UW-tf-dev-1.64.9/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.64.9/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.64.9/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15116 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.64.9/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    20667 2023-07-08 16:12:55.000000 Simba-UW-tf-dev-1.64.9/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.64.9/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/st/
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.64.9/simba/st/enums.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.64.9/simba/st/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.9/simba/st/select_groups_pg.py
--rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.9/simba/st/aggregate_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.64.9/simba/st/app.py
--rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.64.9/simba/st/welcome_page.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.9/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.9/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.9/simba/pose_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.9/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.9/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    14824 2023-07-05 12:33:51.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    16810 2023-07-08 16:29:21.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    14496 2023-07-08 16:28:23.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.9/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/dash_app/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.64.9/simba/dash_app/plotly_dash.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.64.9/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.64.9/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.9/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.64.9/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.64.9/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.64.9/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.64.9/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/ui/
--rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/ui/define_px_to_mm_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/config_reader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/plotting_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/plotting/plot_pose_in_dir.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/pose_importers/anipose_csv_import.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.64.9/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    59883 2023-07-05 17:43:17.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    25424 2023-07-05 13:32:03.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/video_processing_new.py
--rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    13078 2023-07-05 13:23:30.000000 Simba-UW-tf-dev-1.64.9/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    66845 2023-07-06 16:27:17.000000 Simba-UW-tf-dev-1.64.9/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.9/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.64.9/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.64.9/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.64.9/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.64.9/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.64.9/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.9/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-08 16:36:44.000000 Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    21717 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-08 16:36:44.000000 Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-08 16:36:44.000000 Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-08 16:36:44.000000 Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-08 16:36:44.000000 Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.64.9/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.64.9/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.64.9/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.64.9/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.9/tests/test_interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.64.9/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.64.9/tests/test_pose_importers.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.64.9/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.64.9/tests/test_pose_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.64.9/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.64.9/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.64.9/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.64.9/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.64.9/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.64.9/tests/test_video_processors.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/video_processing/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/video_processing/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/video_processing/test_imgs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/expected_animal_bp_dict/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/models/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/models/generated_models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/models/validations/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/models/validations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/project_folder/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/project_folder/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/project_folder/videos/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/project_folder/logs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/project_folder/logs/measures/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.64.9/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.64.9/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.64.9/tests/test_roi_tools.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.64.9/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.64.9/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-07-08 16:36:43.000000 Simba-UW-tf-dev-1.64.9/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-08 16:36:45.000000 Simba-UW-tf-dev-1.64.9/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-08 18:11:16.000000 Simba-UW-tf-dev-1.65.1/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     9015 2023-06-29 20:55:17.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    18197 2023-07-08 16:32:57.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    50461 2023-07-09 20:50:15.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4573 2023-07-07 20:33:35.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.65.1/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.65.1/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.65.1/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.65.1/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.65.1/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.65.1/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.65.1/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.65.1/simba/labelling/labelling_interface_old.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.65.1/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.65.1/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.65.1/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.65.1/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.65.1/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-08 18:15:09.000000 Simba-UW-tf-dev-1.65.1/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      421 2023-07-05 19:50:18.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/shap_gpu.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    22875 2023-07-07 20:39:37.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.65.1/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38471 2023-07-07 19:58:19.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/video_processing_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.65.1/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.65.1/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.65.1/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-08 18:12:56.000000 Simba-UW-tf-dev-1.65.1/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7801 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.65.1/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)    13497 2023-07-09 20:29:02.000000 Simba-UW-tf-dev-1.65.1/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    45067 2023-07-09 20:32:34.000000 Simba-UW-tf-dev-1.65.1/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.65.1/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.65.1/simba/utils/cli/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.65.1/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15116 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.65.1/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    20668 2023-07-09 20:32:34.000000 Simba-UW-tf-dev-1.65.1/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.65.1/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/st/
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.65.1/simba/st/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.65.1/simba/st/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.65.1/simba/st/select_groups_pg.py
+-rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.65.1/simba/st/aggregate_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.65.1/simba/st/app.py
+-rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.65.1/simba/st/welcome_page.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.65.1/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.65.1/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.65.1/simba/pose_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.65.1/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.65.1/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-08 18:11:21.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    14824 2023-07-05 12:33:51.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16810 2023-07-08 16:29:21.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    14496 2023-07-08 16:28:23.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.65.1/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/dash_app/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.65.1/simba/dash_app/plotly_dash.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.65.1/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.65.1/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.65.1/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.65.1/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.65.1/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.65.1/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.65.1/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/ui/define_px_to_mm_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/config_reader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/plotting_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/plotting/plot_pose_in_dir.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/pose_importers/anipose_csv_import.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.65.1/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    59566 2023-07-09 20:45:09.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    25261 2023-07-09 20:40:06.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/video_processing_new.py
+-rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    13078 2023-07-05 13:23:30.000000 Simba-UW-tf-dev-1.65.1/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    66845 2023-07-06 16:27:17.000000 Simba-UW-tf-dev-1.65.1/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.65.1/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.65.1/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.65.1/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.65.1/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.65.1/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.65.1/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.65.1/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.65.1/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    21743 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-09 20:51:14.000000 Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.65.1/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.65.1/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.65.1/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.65.1/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.65.1/tests/test_interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.65.1/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.65.1/tests/test_pose_importers.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.65.1/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.65.1/tests/test_pose_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.65.1/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.65.1/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.65.1/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.65.1/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.65.1/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.65.1/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.65.1/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.65.1/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.65.1/tests/test_roi_tools.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.65.1/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.65.1/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-07-09 20:51:12.000000 Simba-UW-tf-dev-1.65.1/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-09 20:51:15.000000 Simba-UW-tf-dev-1.65.1/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.64.9/PKG-INFO` & `Simba-UW-tf-dev-1.65.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.64.9
+Version: 1.65.1
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/ui/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 00001150: 6261 7208 0809 0809 5f10 197b 7b33 3534  bar....._..{{354
 00001160: 2c20 3132 347d 2c20 7b31 3037 362c 2036  , 124}, {1076, 6
 00001170: 3231 7d7d 0908 1725 313d 4960 6d79 7a7b  21}}...%1=I`myz{
 00001180: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
 00001190: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 009b 0000 0007 0070 006f 0070 005f  .........p.o.p._
 000011b0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
-000011c0: 0000 000e 1b54 0000 0007 0070 006f 0070  .....T.....p.o.p
+000011c0: 0000 000e 2edc 0000 0007 0070 006f 0070  ...........p.o.p
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
-00001770: 6200 0000 088b 58e4 39f3 2ac5 4100 0000  b.....X.9.*.A...
+00001770: 6200 0000 082b ff82 9ce3 2cc5 4100 0000  b....+....,.A...
 00001780: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001790: 6f64 4462 6c6f 6200 0000 088b 58e4 39f3  odDblob.....X.9.
-000017a0: 2ac5 4100 0000 0700 7000 6f00 7000 5f00  *.A.....p.o.p._.
+00001790: 6f64 4462 6c6f 6200 0000 082b ff82 9ce3  odDblob....+....
+000017a0: 2cc5 4100 0000 0700 7000 6f00 7000 5f00  ,.A.....p.o.p._.
 000017b0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-000017c0: 0000 1380 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+000017c0: 0000 13a0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
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
-00001f70: 6200 0000 088b 58e4 39f3 2ac5 4100 0000  b.....X.9.*.A...
+00001f70: 6200 0000 082b ff82 9ce3 2cc5 4100 0000  b....+....,.A...
 00001f80: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001f90: 6f64 4462 6c6f 6200 0000 088b 58e4 39f3  odDblob.....X.9.
-00001fa0: 2ac5 4100 0000 0700 7000 6f00 7000 5f00  *.A.....p.o.p._.
+00001f90: 6f64 4462 6c6f 6200 0000 082b ff82 9ce3  odDblob....+....
+00001fa0: 2cc5 4100 0000 0700 7000 6f00 7000 5f00  ,.A.....p.o.p._.
 00001fb0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-00001fc0: 0000 1380 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
+00001fc0: 0000 13a0 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
 00001fd0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 00001fe0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
 
     def run(self):
         check_file_exist_and_readable(file_path=self.selected_video.file_path)
         superimpose_frame_count(file_path=self.selected_video.file_path, gpu=self.use_gpu_var.get())
 
 class MultiShortenPopUp(PopUpMixin):
     def __init__(self):
-        super().__init__(title='CLIP VIDEO INTO MULTIPLE VIDEOS')
+        super().__init__(title='CLIP VIDEO INTO MULTIPLE VIDEOS', size=(800, 200))
         settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='Split videos into different parts', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
         self.selected_video = FileSelect(settings_frm, "Video path", title='Select a video file', lblwidth=10)
         self.clip_cnt = Entry_Box(settings_frm, '# of clips', '10', validation='numeric')
         self.use_gpu_var = BooleanVar(value=False)
         use_gpu_cb = Checkbutton(settings_frm, text='Use GPU (reduced runtime)', variable=self.use_gpu_var)
         confirm_settings_btn = Button(settings_frm, text='Confirm', command=lambda: self.show_start_stop())
         settings_frm.grid(row=0, sticky=NW)
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.65.1/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/labelling/labelling_interface_old.py` & `Simba-UW-tf-dev-1.65.1/simba/labelling/labelling_interface_old.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.65.1/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.65.1/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.65.1/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.65.1/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/.DS_Store`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0005  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
 00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
 00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0005 0000 000b  ................
+00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000120: 0065 005f 005f 6473 636c 626f 6f6c 0000  .e._._dsclbool..
-00000130: 0000 0b00 5f00 5f00 7000 7900 6300 6100  ...._._.p.y.c.a.
-00000140: 6300 6800 6500 5f00 5f6c 6731 5363 6f6d  c.h.e._._lg1Scom
-00000150: 7000 0000 0000 019d 1900 0000 0b00 5f00  p............._.
-00000160: 5f00 7000 7900 6300 6100 6300 6800 6500  _.p.y.c.a.c.h.e.
-00000170: 5f00 5f6d 6f44 4462 6c6f 6200 0000 0842  _._moDDblob....B
-00000180: 7ed8 c953 0fc5 4100 0000 0b00 5f00 5f00  ~..S..A....._._.
-00000190: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
-000001a0: 5f6d 6f64 4462 6c6f 6200 0000 0842 7ed8  _modDblob....B~.
-000001b0: c953 0fc5 4100 0000 0b00 5f00 5f00 7000  .S..A....._._.p.
-000001c0: 7900 6300 6100 6300 6800 6500 5f00 5f70  y.c.a.c.h.e._._p
-000001d0: 6831 5363 6f6d 7000 0000 0000 0220 0000  h1Scomp...... ..
+00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+00000130: 0000 0004 7300 0000 000b 005f 005f 0070  ....s......_._.p
+00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00000150: 6d6f 4444 626c 6f62 0000 0008 41ed 4121  moDDblob....A.A!
+00000160: 1721 c541 0000 000b 005f 005f 0070 0079  .!.A....._._.p.y
+00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00000180: 6444 626c 6f62 0000 0008 41ed 4121 1721  dDblob....A.A!.!
+00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+000001b0: 636f 6d70 0000 0000 0005 f000 0000 0000  comp............
+000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.65.1/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.65.1/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
-00000010: 0000 1800 0000 300c 0000 100b 0000 400c  ......0.......@.
+00000000: 0000 0001 4275 6431 0000 b800 0000 0800  ....Bud1........
+00000010: 0000 b800 0000 300c 0000 100c 0000 400c  ......0.......@.
 00000020: 0000 500c 0000 0000 0000 0000 0000 0800  ..P.............
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 000a 0000 0002 0000 00be  ................
+00000040: 0000 0000 0000 000a 0000 0002 0000 00c0  ................
 00000050: 0000 000c 0000 1000 006f 0074 0074 0069  .........o.t.t.i
 00000060: 006e 0067 0000 0000 0000 0000 0000 0000  .n.g............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -60,77 +60,77 @@
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0003 0000 0001 0000 000b  ................
 00000410: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
-00000420: 006e 0067 6c73 7643 626c 6f62 0000 032b  .n.glsvCblob...+
+00000420: 006e 0067 6c73 7643 626c 6f62 0000 0333  .n.glsvCblob...3
 00000430: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00000440: 0809 0a0b 0c0d 1855 5657 580c 5a5f 1012  .......UVWX.Z_..
-00000450: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00000460: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00000470: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00000480: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00000490: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-000004a0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
-000004b0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
-000004c0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-000004d0: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
-000004e0: 5369 7a65 1001 09ae 0e17 1c21 252a 2f34  Size.......!%*/4
-000004f0: 393e 4347 4c50 d40f 1011 120c 140c 1657  9>CGLP.........W
-00000500: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
-00000510: 6365 6e64 696e 675a 6964 656e 7469 6669  cendingZidentifi
-00000520: 6572 0911 01c7 0954 6e61 6d65 d40f 1011  er.....Tname....
-00000530: 1218 1918 1b08 1023 0858 7562 6971 7569  .......#.Xubiqui
-00000540: 7479 d40f 1011 120c 1e18 2009 10b5 085c  ty........ ....\
-00000550: 6461 7465 4d6f 6469 6669 6564 d40f 1011  dateModified....
-00000560: 1218 1e18 2408 085b 6461 7465 4372 6561  ....$..[dateCrea
-00000570: 7465 64d4 0f10 1112 0c27 1829 0910 6108  ted......'.)..a.
-00000580: 5473 697a 65d4 0f10 1112 0c2c 0c2e 0910  Tsize......,....
-00000590: 7309 546b 696e 64d4 0f10 1112 1831 0c33  s.Tkind......1.3
-000005a0: 0810 6409 556c 6162 656c d40f 1011 1218  ..d.Ulabel......
-000005b0: 360c 3808 104b 0957 7665 7273 696f 6ed4  6.8..K.Wversion.
-000005c0: 0f10 1112 183b 0c3d 0811 012c 0958 636f  .....;.=...,.Xco
-000005d0: 6d6d 656e 7473 d40f 1011 1218 4018 4208  mments......@.B.
-000005e0: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
-000005f0: 6564 d40f 1011 1218 1e18 4608 0859 6461  ed........F..Yda
-00000600: 7465 4164 6465 64d4 0f10 1112 1849 184b  teAdded......I.K
-00000610: 0810 d208 5a73 6861 7265 4f77 6e65 72d4  ....ZshareOwner.
-00000620: 0f10 1112 1849 184f 0808 5f10 0f73 6861  .....I.O.._..sha
-00000630: 7265 4c61 7374 4564 6974 6f72 d40f 1011  reLastEditor....
-00000640: 1218 4918 5308 085f 1010 696e 7669 7461  ..I.S.._..invita
-00000650: 7469 6f6e 5374 6174 7573 0823 0000 0000  tionStatus.#....
-00000660: 0000 0000 2340 2800 0000 0000 0023 4000  ....#@(......#@.
-00000670: 0000 0000 0000 546e 616d 6509 2340 3000  ......Tname.#@0.
-00000680: 0000 0000 0000 0800 1d00 3200 4400 4c00  ..........2.D.L.
-00000690: 6000 7200 7b00 8d00 9800 ab00 b400 b600  `.r.{...........
-000006a0: b700 c600 cf00 d700 dd00 e700 f200 f300  ................
-000006b0: f600 f700 fc01 0501 0601 0801 0901 1201  ................
-000006c0: 1b01 1c01 1e01 1f01 2c01 3501 3601 3701  ........,.5.6.7.
-000006d0: 4301 4c01 4d01 4f01 5001 5501 5e01 5f01  C.L.M.O.P.U.^._.
-000006e0: 6101 6201 6701 7001 7101 7301 7401 7a01  a.b.g.p.q.s.t.z.
-000006f0: 8301 8401 8601 8701 8f01 9801 9901 9c01  ................
-00000700: 9d01 a601 af01 b001 b201 b301 c201 cb01  ................
-00000710: cc01 cd01 d701 e001 e101 e301 e401 ef01  ................
-00000720: f801 f901 fa02 0c02 1502 1602 1702 2a02  ..............*.
-00000730: 2b02 3402 3d02 4602 4b02 4c00 0000 0000  +.4.=.F.K.L.....
-00000740: 0002 0100 0000 0000 0000 5b00 0000 0000  ..........[.....
-00000750: 0000 0000 0000 0000 0002 5500 0000 0000  ..........U.....
-00000760: 5c64 6174 654d 6f64 6966 6965 6409 1001  \dateModified...
-00000770: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
-00000780: 0077 008c 0095 0096 00a2 00ab 00b6 00bc  .w..............
-00000790: 00c6 00ce 00d3 00d6 00d7 00d8 00e1 00ea  ................
-000007a0: 00ec 00ed 00ee 00f7 00f8 00fa 00fb 0108  ................
-000007b0: 0111 011d 011e 011f 0128 012d 012f 0130  .........(.-./.0
-000007c0: 0131 013a 013f 0141 0142 0143 014c 0152  .1.:.?.A.B.C.L.R
-000007d0: 0154 0155 0156 015f 0167 0169 016a 016b  .T.U.V._.g.i.j.k
-000007e0: 0174 017d 0180 0181 0182 018b 019a 019c  .t.}............
-000007f0: 019d 019e 01a7 01b1 01b2 01b3 01b4 01bd  ................
-00000800: 01ca 01cb 0000 0001 0000 0000 0000 080b  ................
+00000440: 0809 0a0b 0b0d 1a55 5657 5859 5a5f 1010  .......UVWXYZ_..
+00000450: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+00000460: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00000470: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00000480: 6375 6c61 7465 416c 6c53 697a 6573 5f10  culateAllSizes_.
+00000490: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e59  .scrollPositionY
+000004a0: 5874 6578 7453 697a 655f 100f 7363 726f  XtextSize_..scro
+000004b0: 6c6c 506f 7369 7469 6f6e 585a 736f 7274  llPositionXZsort
+000004c0: 436f 6c75 6d6e 5869 636f 6e53 697a 655f  ColumnXiconSize_
+000004d0: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+000004e0: 7369 6f6e 0909 ae0e 171c 2125 2a2f 3439  sion......!%*/49
+000004f0: 3e43 474c 50d4 0f10 1112 1314 0b0b 5a69  >CGLP.........Zi
+00000500: 6465 6e74 6966 6965 7255 7769 6474 6859  dentifierUwidthY
+00000510: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
+00000520: 6554 6e61 6d65 1101 c709 09d4 0f10 1112  eTname..........
+00000530: 1819 1a1a 5875 6269 7175 6974 7910 2308  ....Xubiquity.#.
+00000540: 08d4 0f10 1112 1d1e 1a0b 5c64 6174 654d  ..........\dateM
+00000550: 6f64 6966 6965 6410 b508 09d4 0f10 1112  odified.........
+00000560: 221e 1a1a 5b64 6174 6543 7265 6174 6564  "...[dateCreated
+00000570: 0808 d40f 1011 1226 271a 0b54 7369 7a65  .......&'..Tsize
+00000580: 1061 0809 d40f 1011 122b 2c0b 0b54 6b69  .a.......+,..Tki
+00000590: 6e64 1073 0909 d40f 1011 1230 310b 1a55  nd.s.......01..U
+000005a0: 6c61 6265 6c10 6409 08d4 0f10 1112 3536  label.d.......56
+000005b0: 0b1a 5776 6572 7369 6f6e 104b 0908 d40f  ..Wversion.K....
+000005c0: 1011 123a 3b0b 1a58 636f 6d6d 656e 7473  ...:;..Xcomments
+000005d0: 1101 2c09 08d4 0f10 1112 3f40 1a1a 5e64  ..,.......?@..^d
+000005e0: 6174 654c 6173 744f 7065 6e65 6410 c808  ateLastOpened...
+000005f0: 08d4 0f10 1112 441e 1a1a 5964 6174 6541  ......D...YdateA
+00000600: 6464 6564 0808 d40f 1011 1248 491a 1a5a  dded.......HI..Z
+00000610: 7368 6172 654f 776e 6572 10d2 0808 d40f  shareOwner......
+00000620: 1011 124d 491a 1a5f 100f 7368 6172 654c  ...MI.._..shareL
+00000630: 6173 7445 6469 746f 7208 08d4 0f10 1112  astEditor.......
+00000640: 5149 1a1a 5f10 1069 6e76 6974 6174 696f  QI.._..invitatio
+00000650: 6e53 7461 7475 7308 0808 2300 0000 0000  nStatus...#.....
+00000660: 0000 0023 4028 0000 0000 0000 2340 0000  ...#@(......#@..
+00000670: 0000 0000 005c 6461 7465 4d6f 6469 6669  .....\dateModifi
+00000680: 6564 2340 3000 0000 0000 0010 0100 0800  ed#@0...........
+00000690: 1d00 3000 4200 4a00 5e00 7000 7900 8b00  ..0.B.J.^.p.y...
+000006a0: 9600 9f00 b400 b500 b600 c500 ce00 d900  ................
+000006b0: df00 e900 f100 f600 f900 fa00 fb01 0401  ................
+000006c0: 0d01 0f01 1001 1101 1a01 2701 2901 2a01  ..........'.).*.
+000006d0: 2b01 3401 4001 4101 4201 4b01 5001 5201  +.4.@.A.B.K.P.R.
+000006e0: 5301 5401 5d01 6201 6401 6501 6601 6f01  S.T.].b.d.e.f.o.
+000006f0: 7501 7701 7801 7901 8201 8a01 8c01 8d01  u.w.x.y.........
+00000700: 8e01 9701 a001 a301 a401 a501 ae01 bd01  ................
+00000710: bf01 c001 c101 ca01 d401 d501 d601 df01  ................
+00000720: ea01 ec01 ed01 ee01 f702 0902 0a02 0b02  ................
+00000730: 1402 2702 2802 2902 2a02 3302 3c02 4502  ..'.(.).*.3.<.E.
+00000740: 5202 5b00 0000 0000 0002 0100 0000 0000  R.[.............
+00000750: 0000 5b00 0000 0000 0000 0000 0000 0000  ..[.............
+00000760: 0002 5d3e 1818 5e64 6174 654c 6173 744f  ..]>..^dateLastO
+00000770: 7065 6e65 6410 c808 08d4 0d0e 0f10 421c  pened.........B.
+00000780: 1818 5964 6174 6541 6464 6564 0808 0823  ..YdateAdded...#
+00000790: 4028 0000 0000 0000 5c64 6174 654d 6f64  @(......\dateMod
+000007a0: 6966 6965 6409 1001 0008 0019 0022 0034  ified........".4
+000007b0: 003c 0050 0059 0064 0077 008c 0095 0096  .<.P.Y.d.w......
+000007c0: 00a2 00ab 00b6 00bc 00c6 00ce 00d3 00d6  ................
+000007d0: 00d7 00d8 00e1 00ea 00ec 00ed 00ee 00f7  ................
+000007e0: 00f8 00fa 00fb 0108 0111 011d 011e 011f  ................
+000007f0: 0128 012d 012f 0130 0131 013a 013f 0141  .(.-./.0.1.:.?.A
+00000800: 0142 0143 0000 0001 0000 0000 0000 080b  .B.C............
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -296,106 +296,106 @@
 00001270: 5801 6001 6201 6301 6401 6d01 7601 7901  X.`.b.c.d.m.v.y.
 00001280: 7a01 7b01 8401 9301 9501 9601 9701 a001  z.{.............
 00001290: aa01 ab01 ac01 ad01 b601 c301 cc00 0000  ................
 000012a0: 0000 0002 0100 0000 0000 0000 4a00 0000  ............J...
 000012b0: 0000 0000 0000 0000 0000 0001 cd00 0000  ................
 000012c0: 0900 0000 0900 7200 6f00 6900 5f00 7400  ......r.o.i._.t.
 000012d0: 6f00 6f00 6c00 736c 7376 7062 6c6f 6200  o.o.l.slsvpblob.
-000012e0: 0002 5e62 706c 6973 7430 30d8 0102 0304  ..^bplist00.....
-000012f0: 0506 0708 090a 0b1d 4546 470a 5f10 1276  ........EFG._..v
-00001300: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00001310: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
-00001320: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-00001330: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
-00001340: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
-00001350: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
-00001360: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
-00001370: 0109 d90c 0d0e 0f10 1112 1314 151e 2327  ..............#'
-00001380: 2b30 353a 3f58 636f 6d6d 656e 7473 5e64  +05:?Xcomments^d
-00001390: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
-000013a0: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
-000013b0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-000013c0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-000013d0: 616d 65d4 1617 1819 1a1b 0a1d 5569 6e64  ame.........Uind
-000013e0: 6578 5577 6964 7468 5961 7363 656e 6469  exUwidthYascendi
-000013f0: 6e67 5776 6973 6962 6c65 1007 1101 2c09  ngWvisible....,.
-00001400: 08d4 1617 1819 1f20 1d1d 1008 10c8 0808  ....... ........
-00001410: d416 1718 1909 241d 0a10 b508 09d4 1617  ......$.........
-00001420: 1819 2824 1d1d 1002 0808 d416 1718 192c  ..($...........,
-00001430: 2d1d 0a10 0310 6108 09d4 1617 1819 3132  -.....a.......12
-00001440: 0a1d 1005 1064 0908 d416 1718 1936 370a  .....d.......67.
-00001450: 0a10 0410 7309 09d4 1617 1819 3b3c 0a1d  ....s.......;<..
-00001460: 1006 104b 0908 d416 1718 1940 410a 0a10  ...K.......@A...
-00001470: 0011 01c7 0909 0823 4028 0000 0000 0000  .......#@(......
-00001480: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
-00001490: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
-000014a0: 7900 8c00 8e00 8f00 a200 ab00 ba00 c700  y...............
-000014b0: d300 d800 de00 e300 eb00 f000 f900 ff01  ................
-000014c0: 0501 0f01 1701 1901 1c01 1d01 1e01 2701  ..............'.
-000014d0: 2901 2b01 2c01 2d01 3601 3801 3901 3a01  ).+.,.-.6.8.9.:.
-000014e0: 4301 4501 4601 4701 5001 5201 5401 5501  C.E.F.G.P.R.T.U.
-000014f0: 5601 5f01 6101 6301 6401 6501 6e01 7001  V._.a.c.d.e.n.p.
-00001500: 7201 7301 7401 7d01 7f01 8101 8201 8301  r.s.t.}.........
-00001510: 8c01 8e01 9101 9201 9301 9401 9d01 a201  ................
-00001520: ab00 0000 0000 0002 0100 0000 0000 0000  ................
-00001530: 4900 0000 0000 0000 0000 0000 0000 0001  I...............
-00001540: ac00 0000 0c00 0000 0200 7500 696d 6f64  ..........u.imod
-00001550: 4462 6c6f 6200 0000 087e abce 1cd0 1fc5  Dblob....~......
-00001560: 4100 0000 0d00 0000 0500 7500 7400 6900  A.........u.t.i.
-00001570: 6c00 7364 7363 6c62 6f6f 6c00 0000 0000  l.sdsclbool.....
-00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000015a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000015b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000015c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000015d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000015e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000015f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001800: 0000 0000 0000 000e 0000 0000 0000 180b  ................
-00001810: 0000 0045 0000 300c 0000 100b 0000 400c  ...E..0.......@.
-00001820: 0000 500c 0000 600c 0000 700c 0000 800c  ..P...`...p.....
-00001830: 0000 900c 0000 040a 0000 200c 0000 a00c  .......... .....
-00001840: 0000 b00c 0000 0000 0000 0000 0000 0000  ................
-00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000012e0: 0002 6662 706c 6973 7430 30d8 0102 0304  ..fbplist00.....
+000012f0: 0506 0708 090a 0b1d 4647 0a33 5869 636f  ........FG.3Xico
+00001300: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
+00001310: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00001320: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00001330: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+00001340: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
+00001350: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
+00001360: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
+00001370: 4030 0000 0000 0000 09d9 0c0d 0e0f 1011  @0..............
+00001380: 1213 1415 1e23 282d 3236 3b40 5863 6f6d  .....#(-26;@Xcom
+00001390: 6d65 6e74 7355 6c61 6265 6c57 7665 7273  mentsUlabelWvers
+000013a0: 696f 6e5b 6461 7465 4372 6561 7465 6454  ion[dateCreatedT
+000013b0: 7369 7a65 5c64 6174 654d 6f64 6966 6965  size\dateModifie
+000013c0: 6454 6b69 6e64 546e 616d 655e 6461 7465  dTkindTname^date
+000013d0: 4c61 7374 4f70 656e 6564 d416 1718 191a  LastOpened......
+000013e0: 1b0a 1d55 696e 6465 7855 7769 6474 6859  ...UindexUwidthY
+000013f0: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
+00001400: 6510 0711 012c 0908 d416 1718 191f 200a  e....,........ .
+00001410: 1d10 0510 6409 08d4 1617 1819 2425 0a1d  ....d.......$%..
+00001420: 1006 104b 0908 d416 1718 1929 2a1d 1d10  ...K.......)*...
+00001430: 0210 b508 08d4 1617 1819 2e2f 1d0a 1003  .........../....
+00001440: 1061 0809 d416 1718 1933 2a1d 0a10 0108  .a.......3*.....
+00001450: 09d4 1617 1819 3738 0a0a 1004 1073 0909  ......78.....s..
+00001460: d416 1718 193c 3d0a 0a10 0011 01c7 0909  .....<=.........
+00001470: d416 1718 1941 421d 1d10 0810 c808 0808  .....AB.........
+00001480: 2340 2800 0000 0000 005c 6461 7465 4d6f  #@(......\dateMo
+00001490: 6469 6669 6564 0900 0800 1900 2200 3400  dified......".4.
+000014a0: 3c00 5000 5900 6400 7700 8c00 9500 9600  <.P.Y.d.w.......
+000014b0: a900 b200 b800 c000 cc00 d100 de00 e300  ................
+000014c0: e800 f701 0001 0601 0c01 1601 1e01 2001  .............. .
+000014d0: 2301 2401 2501 2e01 3001 3201 3301 3401  #.$.%...0.2.3.4.
+000014e0: 3d01 3f01 4101 4201 4301 4c01 4e01 5001  =.?.A.B.C.L.N.P.
+000014f0: 5101 5201 5b01 5d01 5f01 6001 6101 6a01  Q.R.[.]._.`.a.j.
+00001500: 6c01 6d01 6e01 7701 7901 7b01 7c01 7d01  l.m.n.w.y.{.|.}.
+00001510: 8601 8801 8b01 8c01 8d01 9601 9801 9a01  ................
+00001520: 9b01 9c01 9d01 a601 b300 0000 0000 0002  ................
+00001530: 0100 0000 0000 0000 4900 0000 0000 0000  ........I.......
+00001540: 0000 0000 0000 0001 b400 0000 0c00 0000  ................
+00001550: 0200 7500 696c 7376 7062 6c6f 6200 0002  ..u.ilsvpblob...
+00001560: 5e62 706c 6973 7430 30d8 0102 0304 0506  ^bplist00.......
+00001570: 0708 090a 0b1a 4546 470a 5f10 1276 6965  ......EFG._..vie
+00001580: 774f 7074 696f 6e73 5665 7273 696f 6e5f  wOptionsVersion_
+00001590: 100f 7368 6f77 4963 6f6e 5072 6576 6965  ..showIconPrevie
+000015a0: 7757 636f 6c75 6d6e 735f 1011 6361 6c63  wWcolumns_..calc
+000015b0: 756c 6174 6541 6c6c 5369 7a65 7358 7465  ulateAllSizesXte
+000015c0: 7874 5369 7a65 5a73 6f72 7443 6f6c 756d  xtSizeZsortColum
+000015d0: 6e58 6963 6f6e 5369 7a65 5f10 1075 7365  nXiconSize_..use
+000015e0: 5265 6c61 7469 7665 4461 7465 7310 0109  RelativeDates...
+000015f0: d90c 0d0e 0f10 1112 1314 151e 2327 2b30  ............#'+0
+00001600: 353a 3f58 636f 6d6d 656e 7473 5e64 6174  5:?Xcomments^dat
+00001610: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
+00001620: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
+00001630: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
+00001640: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
+00001650: 65d4 1617 1819 1a0a 1c1d 5776 6973 6962  e.........Wvisib
+00001660: 6c65 5961 7363 656e 6469 6e67 5577 6964  leYascendingUwid
+00001670: 7468 5569 6e64 6578 0809 1101 2c10 07d4  thUindex....,...
+00001680: 1617 1819 1a1a 2122 0808 10c8 1008 d416  ......!"........
+00001690: 1718 190a 1a26 0909 0810 b5d4 1617 1819  .....&..........
+000016a0: 1a1a 262a 0808 1002 d416 1718 190a 1a2e  ..&*............
+000016b0: 2f09 0810 6110 03d4 1617 1819 1a0a 3334  /...a.........34
+000016c0: 0809 1064 1005 d416 1718 190a 0a38 3909  ...d.........89.
+000016d0: 0910 7310 04d4 1617 1819 1a0a 3d3e 0809  ..s.........=>..
+000016e0: 104b 1006 d419 1817 1640 410a 0a10 0011  .K.......@A.....
+000016f0: 01c7 0909 0823 4028 0000 0000 0000 546e  .....#@(......Tn
+00001700: 616d 6523 4030 0000 0000 0000 0900 0800  ame#@0..........
+00001710: 1900 2e00 4000 4800 5c00 6500 7000 7900  ....@.H.\.e.p.y.
+00001720: 8c00 8e00 8f00 a200 ab00 ba00 c700 d300  ................
+00001730: d800 de00 e300 eb00 f000 f901 0101 0b01  ................
+00001740: 1101 1701 1801 1901 1c01 1e01 2701 2801  ............'.(.
+00001750: 2901 2b01 2d01 3601 3701 3801 3a01 4301  ).+.-.6.7.8.:.C.
+00001760: 4401 4501 4701 5001 5101 5201 5401 5601  D.E.G.P.Q.R.T.V.
+00001770: 5f01 6001 6101 6301 6501 6e01 6f01 7001  _.`.a.c.e.n.o.p.
+00001780: 7201 7401 7d01 7e01 7f01 8101 8301 8c01  r.t.}.~.........
+00001790: 8e01 9101 9201 9301 9401 9d01 a201 ab00  ................
+000017a0: 0000 0000 0002 0100 0000 0000 0000 4900  ..............I.
+000017b0: 0000 0000 0000 0000 0000 0000 0001 ac00  ................
+000017c0: 0000 0d00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
+000017d0: 7362 7773 7062 6c6f 6200 0000 b962 706c  sbwspblob....bpl
+000017e0: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
+000017f0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
+00001800: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
+00001810: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
+00001820: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00001830: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00001840: 7753 6964 6562 6172 0809 0809 5f10 197b  wSidebar...._..{
+00001850: 7b32 3630 2c20 3132 397d 2c20 7b31 3138  {260, 129}, {118
+00001860: 302c 2036 3336 7d7d 0908 1523 2f3b 525f  0, 636}}...#/;R_
+00001870: 6b6c 6d6e 6f8b 0000 0000 0000 0101 0000  klmno...........
+00001880: 0000 0000 000d 0000 0000 0000 0000 0000  ................
+00001890: 0000 0000 008c 0000 0000 0000 0000 0000  ................
 000018a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -442,79 +442,79 @@
 00001b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
-00001c10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
+00001c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001c30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001c40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
-00001c50: 0100 0002 0000 0000 0000 0000 0100 0008  ................
-00001c60: 0000 0000 0000 0000 0000 0000 0100 00c0  ................
-00001c70: 0000 0000 0000 0000 0100 0100 0000 0000  ................
-00001c80: 0100 0200 0000 0000 0100 0400 0000 0000  ................
-00001c90: 0100 0800 0000 0000 0100 1000 0000 0000  ................
-00001ca0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
-00001cb0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
-00001cc0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
-00001cd0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
-00001ce0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00001cf0: 0031 363b 4058 636f 6d6d 656e 7473 5e64  .16;@Xcomments^d
-00001d00: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
-00001d10: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
-00001d20: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-00001d30: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-00001d40: 616d 65d4 1617 1819 1a1b 0a1d 5776 6973  ame.........Wvis
-00001d50: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-00001d60: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
-00001d70: 07d4 1617 1819 1a20 1a22 0810 c808 1008  ....... ."......
-00001d80: d419 1718 1624 250a 0a10 0110 b509 09d4  .....$%.........
-00001d90: 1617 1819 1a25 1a2b 0808 1002 d416 1718  .....%.+........
-00001da0: 190a 2e1a 3009 1061 0810 03d4 1617 1819  ....0..a........
-00001db0: 1a33 0a35 0810 6409 1005 d416 1718 190a  .3.5..d.........
-00001dc0: 380a 3a09 1073 0910 04d4 1617 1819 1a3d  8.:..s.........=
-00001dd0: 0a3f 0810 4b09 1006 d416 1718 190a 420a  .?..K.........B.
-00001de0: 4409 1101 c709 1000 0823 4028 0000 0000  D........#@(....
-00001df0: 0000 5c64 6174 654d 6f64 6966 6965 6409  ..\dateModified.
-00001e00: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
-00001e10: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
-00001e20: 00da 00df 00e5 00ea 00f2 00f7 0100 0108  ................
-00001e30: 010e 0118 011e 011f 0122 0123 0125 012e  .........".#.%..
-00001e40: 012f 0131 0132 0134 013d 013f 0141 0142  ./.1.2.4.=.?.A.B
-00001e50: 0143 014c 014d 014e 0150 0159 015a 015c  .C.L.M.N.P.Y.Z.\
-00001e60: 015d 015f 0168 0169 016b 016c 016e 0177  .]._.h.i.k.l.n.w
-00001e70: 0178 017a 017b 017d 0186 0187 0189 018a  .x.z.{.}........
-00001e80: 018c 0195 0196 0199 019a 019c 019d 01a6  ................
-00001e90: 01b3 0000 0000 0000 0201 0000 0000 0000  ................
-00001ea0: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
-00001eb0: 01b4 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
-00001ec0: 0065 0072 0076 0069 0073 0065 0064 6d6f  .e.r.v.i.s.e.dmo
-00001ed0: 4444 626c 6f62 0000 0008 cbf3 6409 d917  DDblob......d...
-00001ee0: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
-00001ef0: 0065 0072 0076 0069 0073 0065 0064 6d6f  .e.r.v.i.s.e.dmo
-00001f00: 6444 626c 6f62 0000 0008 cbf3 6409 d917  dDblob......d...
-00001f10: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
-00001f20: 0065 0072 0076 0069 0073 0065 0064 7068  .e.r.v.i.s.e.dph
-00001f30: 3153 636f 6d70 0000 0000 0004 d000 0000  1Scomp..........
-00001f40: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
-00001f50: 0076 0069 0073 0065 0064 7653 726e 6c6f  .v.i.s.e.dvSrnlo
-00001f60: 6e67 0000 0001 0000 0005 0075 0074 0069  ng.........u.t.i
-00001f70: 006c 0073 6277 7370 626c 6f62 0000 00b9  .l.sbwspblob....
-00001f80: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
-00001f90: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00001fa0: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
-00001fb0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00001fc0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00001fd0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00001fe0: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-00001ff0: 1019 7b7b 3730 352c 2032 3037 7d2c 207b  ..{{705, 207}, {
-00002000: 3132 3437 0000 0007 0000 0003 0000 0004  1247............
+00001c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002000: 0000 0000 0000 0007 0000 0003 0000 0004  ................
 00002010: 0000 0012 0062 006f 0075 006e 0064 0069  .....b.o.u.n.d.i
 00002020: 006e 0067 005f 0062 006f 0078 005f 0074  .n.g._.b.o.x._.t
 00002030: 006f 006f 006c 0073 6c73 7670 626c 6f62  .o.o.l.slsvpblob
 00002040: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
 00002050: 0405 0607 0809 0a0b 1d45 4647 0a5f 1012  .........EFG._..
 00002060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00002070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
@@ -635,23 +635,23 @@
 000027a0: 011c 011e 0127 0128 012a 012b 012d 0136  .....'.(.*.+.-.6
 000027b0: 0137 0139 013a 0143 0144 0145 0147 0150  .7.9.:.C.D.E.G.P
 000027c0: 0151 0153 0154 0156 015f 0160 0162 0163  .Q.S.T.V._.`.b.c
 000027d0: 0165 016e 016f 0171 0172 0174 017d 017e  .e.n.o.q.r.t.}.~
 000027e0: 0180 0181 0183 018c 018d 0190 0191 0193  ................
 000027f0: 0194 019d 01aa 01b3 0000 0000 0000 0201  ................
 00002800: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
-00002810: 0000 0000 0000 01b4 0000 0000 0000 0000  ................
-00002820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002810: 0000 0000 0000 01b4 5f10 1443 6f6e 7461  ........_..Conta
+00002820: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
+00002830: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
+00002840: 7753 6964 6562 6172 0809 0809 5f10 197b  wSidebar...._..{
+00002850: 7b32 3630 2c20 3132 397d 2c20 7b31 3138  {260, 129}, {118
+00002860: 302c 2036 3336 7d7d 0908 1523 2f3b 525f  0, 636}}...#/;R_
+00002870: 6b6c 6d6e 6f8b 0000 0000 0000 0101 0000  klmno...........
+00002880: 0000 0000 000d 0000 0000 0000 0000 0000  ................
+00002890: 0000 0000 008c 0000 0000 0000 0000 0000  ................
 000028a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000028f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -762,236 +762,236 @@
 00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003000: 0000 0000 0000 0000 0000 0010 0000 0005  ................
-00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 0008 78a2 0000 0005 0075  mp......x......u
-00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
-00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
-00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
-00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-000030a0: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-000030b0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-000030c0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
-000030d0: 1001 09ab 0c15 1d22 262b 3035 3a3f 44d4  ......."&+05:?D.
-000030e0: 0d0e 0f10 0a0a 1314 5776 6973 6962 6c65  ........Wvisible
-000030f0: 5961 7363 656e 6469 6e67 5577 6964 7468  YascendingUwidth
-00003100: 5a69 6465 6e74 6966 6965 7209 0911 0204  Zidentifier.....
-00003110: 546e 616d 65d4 1617 1810 191a 191c 5776  Tname.........Wv
-00003120: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-00003130: 656e 6469 6e67 0810 2308 5875 6269 7175  ending..#.Xubiqu
-00003140: 6974 79d4 0d0e 0f10 0a19 2021 0908 10b5  ity....... !....
-00003150: 5c64 6174 654d 6f64 6966 6965 64d4 0d0e  \dateModified...
-00003160: 0f10 1919 2025 0808 5b64 6174 6543 7265  .... %..[dateCre
-00003170: 6174 6564 d40d 0e0f 100a 1929 2a09 0810  ated.......)*...
-00003180: 6154 7369 7a65 d40d 0e0f 100a 0a2e 2f09  aTsize......../.
-00003190: 0910 7354 6b69 6e64 d40d 0e0f 1019 0a33  ..sTkind.......3
-000031a0: 3408 0910 6455 6c61 6265 6cd4 0d0e 0f10  4...dUlabel.....
-000031b0: 190a 3839 0809 104b 5776 6572 7369 6f6e  ..89...KWversion
-000031c0: d40d 0e0f 1019 0a3d 3e08 0911 012c 5863  .......=>....,Xc
-000031d0: 6f6d 6d65 6e74 73d4 0d0e 0f10 1919 4243  omments.......BC
-000031e0: 0808 10c8 5e64 6174 654c 6173 744f 7065  ....^dateLastOpe
-000031f0: 6e65 64d4 1617 1810 1920 1947 0808 5964  ned...... .G..Yd
-00003200: 6174 6541 6464 6564 0823 4028 0000 0000  ateAdded.#@(....
-00003210: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
-00003220: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-00003230: 7000 8300 8c00 8e00 8f00 9b00 a400 ac00  p...............
-00003240: b600 bc00 c700 c800 c900 cc00 d100 da00  ................
-00003250: e200 e800 f200 f300 f500 f600 ff01 0801  ................
-00003260: 0901 0a01 0c01 1901 2201 2301 2401 3001  ........".#.$.0.
-00003270: 3901 3a01 3b01 3d01 4201 4b01 4c01 4d01  9.:.;.=.B.K.L.M.
-00003280: 4f01 5401 5d01 5e01 5f01 6101 6701 7001  O.T.].^._.a.g.p.
-00003290: 7101 7201 7401 7c01 8501 8601 8701 8a01  q.r.t.|.........
-000032a0: 9301 9c01 9d01 9e01 a001 af01 b801 b901  ................
-000032b0: ba01 c401 c501 ce01 d301 d400 0000 0000  ................
-000032c0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
-000032d0: 0000 0000 0000 0000 0001 dd00 0000 0500  ................
-000032e0: 7500 7400 6900 6c00 736c 7376 7062 6c6f  u.t.i.l.slsvpblo
-000032f0: 6200 0002 5e62 706c 6973 7430 30d8 0102  b...^bplist00...
-00003300: 0304 0506 0708 090a 0b1d 4546 0a48 5f10  ..........EF.H_.
-00003310: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00003320: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
-00003330: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
-00003340: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
-00003350: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
-00003360: 6f6c 756d 6e5f 1010 7573 6552 656c 6174  olumn_..useRelat
-00003370: 6976 6544 6174 6573 5869 636f 6e53 697a  iveDatesXiconSiz
-00003380: 6510 0109 d90c 0d0e 0f10 1112 1314 151e  e...............
-00003390: 2328 2d32 373c 4158 636f 6d6d 656e 7473  #(-27<AXcomments
-000033a0: 5e64 6174 654c 6173 744f 7065 6e65 645b  ^dateLastOpened[
-000033b0: 6461 7465 4372 6561 7465 6454 7369 7a65  dateCreatedTsize
-000033c0: 556c 6162 656c 546b 696e 6457 7665 7273  UlabelTkindWvers
-000033d0: 696f 6e54 6e61 6d65 5c64 6174 654d 6f64  ionTname\dateMod
-000033e0: 6966 6965 64d4 1617 1819 1a0a 1c1d 5569  ified.........Ui
-000033f0: 6e64 6578 5961 7363 656e 6469 6e67 5577  ndexYascendingUw
-00003400: 6964 7468 5776 6973 6962 6c65 1007 0911  idthWvisible....
-00003410: 012c 08d4 1617 1819 1f1d 211d 1008 0810  .,........!.....
-00003420: c808 d416 1718 1924 1d26 1d10 0208 10b5  .......$.&......
-00003430: 08d4 1617 1819 291d 2b0a 1003 0810 6109  ......).+.....a.
-00003440: d416 1718 192e 0a30 1d10 0509 1064 08d4  .......0.....d..
-00003450: 1617 1819 330a 350a 1004 0910 7309 d416  ....3.5.....s...
-00003460: 1718 1938 0a3a 1d10 0609 104b 08d4 1617  ...8.:.....K....
-00003470: 1819 3d0a 3f0a 1000 0911 0204 09d4 1617  ..=.?...........
-00003480: 1819 091d 260a 0809 0823 4028 0000 0000  ....&....#@(....
-00003490: 0000 546e 616d 6509 2340 3000 0000 0000  ..Tname.#@0.....
-000034a0: 0000 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-000034b0: 7000 8300 8c00 8e00 8f00 a200 ab00 ba00  p...............
-000034c0: c600 cb00 d100 d600 de00 e300 f000 f900  ................
-000034d0: ff01 0901 0f01 1701 1901 1a01 1d01 1e01  ................
-000034e0: 2701 2901 2a01 2c01 2d01 3601 3801 3901  '.).*.,.-.6.8.9.
-000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
-00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
-00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
-00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
-00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
-00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
-00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 0886 592f  smoDDblob.....Y/
-00003570: 92f6 2ac5 4100 0000 0500 7500 7400 6900  ..*.A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 0886  l.smodDblob.....
-00003590: 592f 92f6 2ac5 4100 0000 0500 7500 7400  Y/..*.A.....u.t.
-000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000035b0: 0000 0a00 0000 0000 0500 7500 7400 6900  ..........u.t.i.
-000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
-000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
-000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-000035f0: 7200 7362 7773 7062 6c6f 6200 0000 b962  r.sbwspblob....b
-00003600: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
-00003610: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
-00003620: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
-00003630: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
-00003640: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
-00003650: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
-00003660: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
-00003670: 197b 7b37 3035 2c20 3230 377d 2c20 7b31  .{{705, 207}, {1
-00003680: 3234 372c 2035 3638 7d7d 0908 1523 2f3b  247, 568}}...#/;
-00003690: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
-000036a0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
-000036b0: 0000 0000 0000 008c 0000 0010 0076 0069  .............v.i
-000036c0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
-000036d0: 0065 0073 0073 006f 0072 0073 6473 636c  .e.s.s.o.r.sdscl
-000036e0: 626f 6f6c 0000 0000 1000 7600 6900 6400  bool......v.i.d.
-000036f0: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
-00003700: 7300 7300 6f00 7200 736c 6731 5363 6f6d  s.s.o.r.slg1Scom
-00003710: 7000 0000 0000 0622 c000 0000 1000 7600  p......"......v.
-00003720: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
-00003730: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
-00003740: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
-00003750: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
-00003760: 0a4c 5869 636f 6e53 697a 655f 100f 7368  .LXiconSize_..sh
-00003770: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00003780: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00003790: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-000037a0: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-000037b0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000037c0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-000037d0: 7273 696f 6e23 4030 0000 0000 0000 09ab  rsion#@0........
-000037e0: 0c15 1d22 262b 3035 3a3f 44d4 0d0e 0f10  ..."&+05:?D.....
-000037f0: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
-00003800: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00003810: 7669 7369 626c 6554 6e61 6d65 1101 c709  visibleTname....
-00003820: 09d4 1617 180d 191a 191c 5776 6973 6962  ..........Wvisib
-00003830: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
-00003840: 6e67 0810 2308 5875 6269 7175 6974 79d4  ng..#.Xubiquity.
-00003850: 0d0e 0f10 1e1f 190a 5c64 6174 654d 6f64  ........\dateMod
-00003860: 6966 6965 6410 b508 09d4 0d0e 0f10 231f  ified.........#.
-00003870: 1919 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
-00003880: d40d 0e0f 1027 2819 0a54 7369 7a65 1061  .....'(..Tsize.a
-00003890: 0809 d40d 0e0f 102c 2d0a 0a54 6b69 6e64  .......,-..Tkind
-000038a0: 1073 0909 d40d 0e0f 1031 320a 1955 6c61  .s.......12..Ula
-000038b0: 6265 6c10 6409 08d4 0d0e 0f10 3637 0a19  bel.d.......67..
-000038c0: 5776 6572 7369 6f6e 104b 0908 d40d 0e0f  Wversion.K......
-000038d0: 103b 3c0a 1958 636f 6d6d 656e 7473 1101  .;<..Xcomments..
-000038e0: 2c09 08d4 0d0e 0f10 4041 1919 5e64 6174  ,.......@A..^dat
-000038f0: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
-00003900: 1617 180d 191f 1947 0808 5964 6174 6541  .......G..YdateA
-00003910: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
-00003920: 616d 6509 1001 0008 0019 0022 0034 003c  ame........".4.<
-00003930: 0050 0059 0064 0077 008c 0095 0096 00a2  .P.Y.d.w........
-00003940: 00ab 00b6 00bc 00c6 00ce 00d3 00d6 00d7  ................
-00003950: 00d8 00e1 00e9 00ef 00f9 00fa 00fc 00fd  ................
-00003960: 0106 010f 011c 011e 011f 0120 0129 0135  ........... .).5
-00003970: 0136 0137 0140 0145 0147 0148 0149 0152  .6.7.@.E.G.H.I.R
-00003980: 0157 0159 015a 015b 0164 016a 016c 016d  .W.Y.Z.[.d.j.l.m
-00003990: 016e 0177 017f 0181 0182 0183 018c 0195  .n.w............
-000039a0: 0198 0199 019a 01a3 01b2 01b4 01b5 01b6  ................
-000039b0: 01bf 01c0 01c1 01cb 01cc 01d5 01da 01db  ................
-000039c0: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
-000039d0: 0000 0000 0000 0000 0000 0000 0000 01dd  ................
-000039e0: 0000 0010 0076 0069 0064 0065 006f 005f  .....v.i.d.e.o._
-000039f0: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
-00003a00: 0072 0073 6c73 7670 626c 6f62 0000 025e  .r.slsvpblob...^
-00003a10: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
-00003a20: 0809 0a0b 1a46 470a 4458 6963 6f6e 5369  .....FG.DXiconSi
-00003a30: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
-00003a40: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00003a50: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00003a60: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-00003a70: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-00003a80: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
-00003a90: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
-00003aa0: 0000 0000 0009 d90c 0d0e 0f10 1112 1314  ................
-00003ab0: 151e 2328 2d32 373c 4158 636f 6d6d 656e  ..#(-27<AXcommen
-00003ac0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
-00003ad0: 645b 6461 7465 4372 6561 7465 6454 7369  d[dateCreatedTsi
-00003ae0: 7a65 556c 6162 656c 546b 696e 6457 7665  zeUlabelTkindWve
-00003af0: 7273 696f 6e54 6e61 6d65 5c64 6174 654d  rsionTname\dateM
-00003b00: 6f64 6966 6965 64d4 1617 1819 1a1b 0a1d  odified.........
-00003b10: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-00003b20: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
-00003b30: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
-00003b40: c808 1008 d416 1718 191a 251a 2708 10b5  ..........%.'...
-00003b50: 0810 02d4 1617 1819 0a2a 1a2c 0910 6108  .........*.,..a.
-00003b60: 1003 d416 1718 191a 2f0a 3108 1064 0910  ......../.1..d..
-00003b70: 05d4 1617 1819 0a34 0a36 0910 7309 1004  .......4.6..s...
-00003b80: d416 1718 191a 390a 3b08 104b 0910 06d4  ......9.;..K....
-00003b90: 1617 1819 0a3e 0a40 0911 01c7 0910 00d4  .....>.@........
-00003ba0: 1617 1819 0a25 1a44 0908 1001 0823 4028  .....%.D.....#@(
-00003bb0: 0000 0000 0000 546e 616d 6509 0008 0019  ......Tname.....
-00003bc0: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
-00003bd0: 0095 0096 00a9 00b2 00c1 00cd 00d2 00d8  ................
-00003be0: 00dd 00e5 00ea 00f7 0100 0108 010e 0118  ................
-00003bf0: 011e 011f 0122 0123 0125 012e 012f 0131  .....".#.%.../.1
-00003c00: 0132 0134 013d 013e 0140 0141 0143 014c  .2.4.=.>.@.A.C.L
-00003c10: 014d 014f 0150 0152 015b 015c 015e 015f  .M.O.P.R.[.\.^._
-00003c20: 0161 016a 016b 016d 016e 0170 0179 017a  .a.j.k.m.n.p.y.z
-00003c30: 017c 017d 017f 0188 0189 018c 018d 018f  .|.}............
-00003c40: 0198 0199 019a 019c 019d 01a6 01ab 0000  ................
-00003c50: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
-00003c60: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
-00003c70: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
-00003c80: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-00003c90: 0073 6d6f 4444 626c 6f62 0000 0008 3e94  .smoDDblob....>.
-00003ca0: a59a f12a c541 0000 0010 0076 0069 0064  ...*.A.....v.i.d
-00003cb0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
-00003cc0: 0073 0073 006f 0072 0073 6d6f 6444 626c  .s.s.o.r.smodDbl
-00003cd0: 6f62 0000 0008 707b be2b d62a c541 0000  ob....p{.+.*.A..
-00003ce0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
-00003cf0: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-00003d00: 0073 7068 3153 636f 6d70 0000 0000 0007  .sph1Scomp......
-00003d10: 7000 0000 0010 0076 0069 0064 0065 006f  p......v.i.d.e.o
-00003d20: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
-00003d30: 006f 0072 0073 7653 726e 6c6f 6e67 0000  .o.r.svSrnlong..
-00003d40: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00003d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003000: 0000 0000 0000 0000 0000 0011 0000 0005  ................
+00003010: 0075 0074 0069 006c 0073 6473 636c 626f  .u.t.i.l.sdsclbo
+00003020: 6f6c 0000 0000 0500 7500 7400 6900 6c00  ol......u.t.i.l.
+00003030: 736c 6731 5363 6f6d 7000 0000 0000 08b2  slg1Scomp.......
+00003040: 1000 0000 0500 7500 7400 6900 6c00 736c  ......u.t.i.l.sl
+00003050: 7376 4362 6c6f 6200 0003 0f62 706c 6973  svCblob....bplis
+00003060: 7430 30d8 0102 0304 0506 0708 0909 0b16  t00.............
+00003070: 5657 5859 5f10 1075 7365 5265 6c61 7469  VWXY_..useRelati
+00003080: 7665 4461 7465 735f 100f 7368 6f77 4963  veDates_..showIc
+00003090: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+000030a0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+000030b0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+000030c0: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
+000030d0: 7a65 5f10 1276 6965 774f 7074 696f 6e73  ze_..viewOptions
+000030e0: 5665 7273 696f 6e09 09ae 0c15 1a1f 2328  Version.......#(
+000030f0: 2d32 373c 4145 4d51 d40d 0e0f 1009 0913  -27<AEMQ........
+00003100: 1457 7669 7369 626c 6559 6173 6365 6e64  .WvisibleYascend
+00003110: 696e 6755 7769 6474 685a 6964 656e 7469  ingUwidthZidenti
+00003120: 6669 6572 0909 1102 0454 6e61 6d65 d40d  fier.....Tname..
+00003130: 0f0e 1016 1716 1908 1023 0858 7562 6971  .........#.Xubiq
+00003140: 7569 7479 d40d 0e0f 1009 161d 1e09 0810  uity............
+00003150: b55c 6461 7465 4d6f 6469 6669 6564 d40d  .\dateModified..
+00003160: 0e0f 1016 161d 2208 085b 6461 7465 4372  ......"..[dateCr
+00003170: 6561 7465 64d4 0d0e 0f10 0916 2627 0908  eated.......&'..
+00003180: 1061 5473 697a 65d4 0d0e 0f10 0909 2b2c  .aTsize.......+,
+00003190: 0909 1073 546b 696e 64d4 0d0e 0f10 1609  ...sTkind.......
+000031a0: 3031 0809 1064 556c 6162 656c d40d 0e0f  01...dUlabel....
+000031b0: 1016 0935 3608 0910 4b57 7665 7273 696f  ...56...KWversio
+000031c0: 6ed4 0d0e 0f10 1609 3a3b 0809 1101 2c58  n.......:;....,X
+000031d0: 636f 6d6d 656e 7473 d40d 0e0f 1016 163f  comments.......?
+000031e0: 4008 0810 c85e 6461 7465 4c61 7374 4f70  @....^dateLastOp
+000031f0: 656e 6564 d40d 0f0e 1016 1d16 4408 0859  ened........D..Y
+00003200: 6461 7465 4164 6465 64d4 4647 4810 164a  dateAdded.FGH..J
+00003210: 164c 5776 6973 6962 6c65 5577 6964 7468  .LWvisibleUwidth
+00003220: 5961 7363 656e 6469 6e67 0810 d208 5a73  Yascending....Zs
+00003230: 6861 7265 4f77 6e65 72d4 4647 4810 164a  hareOwner.FGH..J
+00003240: 1650 0808 5f10 0f73 6861 7265 4c61 7374  .P.._..shareLast
+00003250: 4564 6974 6f72 d446 4748 1016 4a16 5408  Editor.FGH..J.T.
+00003260: 085f 1010 696e 7669 7461 7469 6f6e 5374  ._..invitationSt
+00003270: 6174 7573 0823 4028 0000 0000 0000 5c64  atus.#@(......\d
+00003280: 6174 654d 6f64 6966 6965 6423 4030 0000  ateModified#@0..
+00003290: 0000 0000 1001 0008 0019 002c 003e 0046  ...........,.>.F
+000032a0: 005a 0063 006e 0077 008c 008d 008e 009d  .Z.c.n.w........
+000032b0: 00a6 00ae 00b8 00be 00c9 00ca 00cb 00ce  ................
+000032c0: 00d3 00dc 00dd 00df 00e0 00e9 00f2 00f3  ................
+000032d0: 00f4 00f6 0103 010c 010d 010e 011a 0123  ...............#
+000032e0: 0124 0125 0127 012c 0135 0136 0137 0139  .$.%.'.,.5.6.7.9
+000032f0: 013e 0147 0148 0149 014b 0151 015a 015b  .>.G.H.I.K.Q.Z.[
+00003300: 015c 015e 0166 016f 0170 0171 0174 017d  .\.^.f.o.p.q.t.}
+00003310: 0186 0187 0188 018a 0199 01a2 01a3 01a4  ................
+00003320: 01ae 01b7 01bf 01c5 01cf 01d0 01d2 01d3  ................
+00003330: 01de 01e7 01e8 01e9 01fb 0204 0205 0206  ................
+00003340: 0219 021a 0223 0230 0239 0000 0000 0000  .....#.0.9......
+00003350: 0201 0000 0000 0000 005a 0000 0000 0000  .........Z......
+00003360: 0000 0000 0000 0000 023b 0000 0005 0075  .........;.....u
+00003370: 0074 0069 006c 0073 6c73 7670 626c 6f62  .t.i.l.slsvpblob
+00003380: 0000 0266 6270 6c69 7374 3030 d801 0203  ...fbplist00....
+00003390: 0405 0607 0809 090b 1d46 4748 335f 1010  .........FGH3_..
+000033a0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000033b0: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+000033c0: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+000033d0: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+000033e0: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+000033f0: 6d6e 5869 636f 6e53 697a 655f 1012 7669  mnXiconSize_..vi
+00003400: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00003410: 0909 d90c 0d0e 0f10 1112 1314 151e 2328  ..............#(
+00003420: 2d32 363b 4058 636f 6d6d 656e 7473 556c  -26;@XcommentsUl
+00003430: 6162 656c 5776 6572 7369 6f6e 5b64 6174  abelWversion[dat
+00003440: 6543 7265 6174 6564 5473 697a 655c 6461  eCreatedTsize\da
+00003450: 7465 4d6f 6469 6669 6564 546b 696e 6454  teModifiedTkindT
+00003460: 6e61 6d65 5e64 6174 654c 6173 744f 7065  name^dateLastOpe
+00003470: 6e65 64d4 1617 1819 1a09 1c1d 5569 6e64  ned.........Uind
+00003480: 6578 5961 7363 656e 6469 6e67 5577 6964  exYascendingUwid
+00003490: 7468 5776 6973 6962 6c65 1007 0911 012c  thWvisible.....,
+000034a0: 08d4 1617 1819 1f09 211d 1005 0910 6408  ........!.....d.
+000034b0: d416 1718 1924 0926 1d10 0609 104b 08d4  .....$.&.....K..
+000034c0: 1617 1819 291d 2b1d 1002 0810 b508 d416  ....).+.........
+000034d0: 1718 192e 1d30 0910 0308 1061 09d4 1617  .....0.....a....
+000034e0: 1819 331d 2b09 1001 0809 d416 1718 1937  ..3.+..........7
+000034f0: 0939 0910 0409 1073 09d4 1617 1819 3c09  .9.....s......<.
+00003500: 3e09 1000 0911 0204 09d4 1617 1819 411d  >.............A.
+00003510: 431d 1008 0810 c808 0823 4028 0000 0000  C........#@(....
+00003520: 0000 5c64 6174 654d 6f64 6966 6965 6423  ..\dateModified#
+00003530: 4030 0000 0000 0000 0008 0019 002c 003e  @0...........,.>
+00003540: 0046 005a 0063 006e 0077 008c 008d 008e  .F.Z.c.n.w......
+00003550: 00a1 00aa 00b0 00b8 00c4 00c9 00d6 00db  ................
+00003560: 00e0 00ef 00f8 00fe 0108 010e 0116 0118  ................
+00003570: 0119 011c 011d 0126 0128 0129 012b 012c  .......&.(.).+.,
+00003580: 0135 0137 0138 013a 013b 0144 0146 0147  .5.7.8.:.;.D.F.G
+00003590: 0149 014a 0153 0155 0156 0158 0159 0162  .I.J.S.U.V.X.Y.b
+000035a0: 0164 0165 0166 016f 0171 0172 0174 0175  .d.e.f.o.q.r.t.u
+000035b0: 017e 0180 0181 0184 0185 018e 0190 0191  .~..............
+000035c0: 0193 0194 0195 019e 01ab 0000 0000 0000  ................
+000035d0: 0201 0000 0000 0000 0049 0000 0000 0000  .........I......
+000035e0: 0000 0000 0000 0000 01b4 0000 0005 0075  ...............u
+000035f0: 0074 0069 006c 0073 6d6f 4444 626c 6f62  .t.i.l.smoDDblob
+00003600: 0000 0008 d4f8 ef43 e12c c541 0000 0005  .......C.,.A....
+00003610: 0075 0074 0069 006c 0073 6d6f 6444 626c  .u.t.i.l.smodDbl
+00003620: 6f62 0000 0008 d4f8 ef43 e12c c541 0000  ob.......C.,.A..
+00003630: 0005 0075 0074 0069 006c 0073 7068 3153  ...u.t.i.l.sph1S
+00003640: 636f 6d70 0000 0000 000a 5000 0000 0005  comp......P.....
+00003650: 0075 0074 0069 006c 0073 7653 726e 6c6f  .u.t.i.l.svSrnlo
+00003660: 6e67 0000 0001 0000 0010 0076 0069 0064  ng.........v.i.d
+00003670: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
+00003680: 0073 0073 006f 0072 0073 6277 7370 626c  .s.s.o.r.sbwspbl
+00003690: 6f62 0000 00b9 6270 6c69 7374 3030 d601  ob....bplist00..
+000036a0: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
+000036b0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
+000036c0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+000036d0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+000036e0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+000036f0: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+00003700: 7208 0908 095f 1019 7b7b 3236 302c 2031  r...._..{{260, 1
+00003710: 3239 7d2c 207b 3131 3830 2c20 3633 367d  29}, {1180, 636}
+00003720: 7d09 0815 232f 3b52 5f6b 6c6d 6e6f 8b00  }...#/;R_klmno..
+00003730: 0000 0000 0001 0100 0000 0000 0000 0d00  ................
+00003740: 0000 0000 0000 0000 0000 0000 0000 8c00  ................
+00003750: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
+00003760: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
+00003770: 7200 7364 7363 6c62 6f6f 6c00 0000 0010  r.sdsclbool.....
+00003780: 0076 0069 0064 0065 006f 005f 0070 0072  .v.i.d.e.o._.p.r
+00003790: 006f 0063 0065 0073 0073 006f 0072 0073  .o.c.e.s.s.o.r.s
+000037a0: 6c67 3153 636f 6d70 0000 0000 0006 22c0  lg1Scomp......".
+000037b0: 0000 0010 0076 0069 0064 0065 006f 005f  .....v.i.d.e.o._
+000037c0: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
+000037d0: 0072 0073 6c73 7643 626c 6f62 0000 0297  .r.slsvCblob....
+000037e0: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+000037f0: 0809 0a0b 1949 4a0a 4c58 6963 6f6e 5369  .....IJ.LXiconSi
+00003800: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+00003810: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00003820: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00003830: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+00003840: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+00003850: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
+00003860: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
+00003870: 0000 0000 0009 ab0c 151d 2226 2b30 353a  .........."&+05:
+00003880: 3f44 d40d 0e0f 1011 120a 0a5a 6964 656e  ?D.........Ziden
+00003890: 7469 6669 6572 5577 6964 7468 5961 7363  tifierUwidthYasc
+000038a0: 656e 6469 6e67 5776 6973 6962 6c65 546e  endingWvisibleTn
+000038b0: 616d 6511 01c7 0909 d416 1718 0d19 1a19  ame.............
+000038c0: 1c57 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
+000038d0: 6173 6365 6e64 696e 6708 1023 0858 7562  ascending..#.Xub
+000038e0: 6971 7569 7479 d40d 0e0f 101e 1f19 0a5c  iquity.........\
+000038f0: 6461 7465 4d6f 6469 6669 6564 10b5 0809  dateModified....
+00003900: d40d 0e0f 1023 1f19 195b 6461 7465 4372  .....#...[dateCr
+00003910: 6561 7465 6408 08d4 0d0e 0f10 2728 190a  eated.......'(..
+00003920: 5473 697a 6510 6108 09d4 0d0e 0f10 2c2d  Tsize.a.......,-
+00003930: 0a0a 546b 696e 6410 7309 09d4 0d0e 0f10  ..Tkind.s.......
+00003940: 3132 0a19 556c 6162 656c 1064 0908 d40d  12..Ulabel.d....
+00003950: 0e0f 1036 370a 1957 7665 7273 696f 6e10  ...67..Wversion.
+00003960: 4b09 08d4 0d0e 0f10 3b3c 0a19 5863 6f6d  K.......;<..Xcom
+00003970: 6d65 6e74 7311 012c 0908 d40d 0e0f 1040  ments..,.......@
+00003980: 4119 195e 6461 7465 4c61 7374 4f70 656e  A..^dateLastOpen
+00003990: 6564 10c8 0808 d416 1718 0d19 1f19 4708  ed............G.
+000039a0: 0859 6461 7465 4164 6465 6408 2340 2800  .YdateAdded.#@(.
+000039b0: 0000 0000 0054 6e61 6d65 0910 0100 0800  .....Tname......
+000039c0: 1900 2200 3400 3c00 5000 5900 6400 7700  ..".4.<.P.Y.d.w.
+000039d0: 8c00 9500 9600 a200 ab00 b600 bc00 c600  ................
+000039e0: ce00 d300 d600 d700 d800 e100 e900 ef00  ................
+000039f0: f900 fa00 fc00 fd01 0601 0f01 1c01 1e01  ................
+00003a00: 1f01 2001 2901 3501 3601 3701 4001 4501  .. .).5.6.7.@.E.
+00003a10: 4701 4801 4901 5201 5701 5901 5a01 5b01  G.H.I.R.W.Y.Z.[.
+00003a20: 6401 6a01 6c01 6d01 6e01 7701 7f01 8101  d.j.l.m.n.w.....
+00003a30: 8201 8301 8c01 9501 9801 9901 9a01 a301  ................
+00003a40: b201 b401 b501 b601 bf01 c001 c101 cb01  ................
+00003a50: cc01 d501 da01 db00 0000 0000 0002 0100  ................
+00003a60: 0000 0000 0000 4d00 0000 0000 0000 0000  ......M.........
+00003a70: 0000 0000 0001 dd00 0000 1000 7600 6900  ............v.i.
+00003a80: 6400 6500 6f00 5f00 7000 7200 6f00 6300  d.e.o._.p.r.o.c.
+00003a90: 6500 7300 7300 6f00 7200 736c 7376 7062  e.s.s.o.r.slsvpb
+00003aa0: 6c6f 6200 0002 5e62 706c 6973 7430 30d8  lob...^bplist00.
+00003ab0: 0102 0304 0506 0708 090a 0b1a 4647 0a44  ............FG.D
+00003ac0: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
+00003ad0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00003ae0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+00003af0: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+00003b00: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
+00003b10: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
+00003b20: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00003b30: 696f 6e23 4030 0000 0000 0000 09d9 0c0d  ion#@0..........
+00003b40: 0e0f 1011 1213 1415 1e23 282d 3237 3c41  .........#(-27<A
+00003b50: 5863 6f6d 6d65 6e74 735e 6461 7465 4c61  Xcomments^dateLa
+00003b60: 7374 4f70 656e 6564 5b64 6174 6543 7265  stOpened[dateCre
+00003b70: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
+00003b80: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
+00003b90: 655c 6461 7465 4d6f 6469 6669 6564 d416  e\dateModified..
+00003ba0: 1718 191a 1b0a 1d57 7669 7369 626c 6555  .......WvisibleU
+00003bb0: 7769 6474 6859 6173 6365 6e64 696e 6755  widthYascendingU
+00003bc0: 696e 6465 7808 1101 2c09 1007 d416 1718  index...,.......
+00003bd0: 191a 201a 2208 10c8 0810 08d4 1617 1819  .. ."...........
+00003be0: 1a25 1a27 0810 b508 1002 d416 1718 190a  .%.'............
+00003bf0: 2a1a 2c09 1061 0810 03d4 1617 1819 1a2f  *.,..a........./
+00003c00: 0a31 0810 6409 1005 d416 1718 190a 340a  .1..d.........4.
+00003c10: 3609 1073 0910 04d4 1617 1819 1a39 0a3b  6..s.........9.;
+00003c20: 0810 4b09 1006 d416 1718 190a 3e0a 4009  ..K.........>.@.
+00003c30: 1101 c709 1000 d416 1718 190a 251a 4409  ............%.D.
+00003c40: 0810 0108 2340 2800 0000 0000 0054 6e61  ....#@(......Tna
+00003c50: 6d65 0900 0800 1900 2200 3400 3c00 5000  me......".4.<.P.
+00003c60: 5900 6400 7700 8c00 9500 9600 a900 b200  Y.d.w...........
+00003c70: c100 cd00 d200 d800 dd00 e500 ea00 f701  ................
+00003c80: 0001 0801 0e01 1801 1e01 1f01 2201 2301  ............".#.
+00003c90: 2501 2e01 2f01 3101 3201 3401 3d01 3e01  %.../.1.2.4.=.>.
+00003ca0: 4001 4101 4301 4c01 4d01 4f01 5001 5201  @.A.C.L.M.O.P.R.
+00003cb0: 5b01 5c01 5e01 5f01 6101 6a01 6b01 6d01  [.\.^._.a.j.k.m.
+00003cc0: 6e01 7001 7901 7a01 7c01 7d01 7f01 8801  n.p.y.z.|.}.....
+00003cd0: 8901 8c01 8d01 8f01 9801 9901 9a01 9c01  ................
+00003ce0: 9d01 a601 ab00 0000 0000 0002 0100 0000  ................
+00003cf0: 0000 0000 4900 0000 0000 0000 0000 0000  ....I...........
+00003d00: 0000 0001 ac00 0000 1000 7600 6900 6400  ..........v.i.d.
+00003d10: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
+00003d20: 7300 7300 6f00 7200 736d 6f44 4462 6c6f  s.s.o.r.smoDDblo
+00003d30: 6200 0000 083e 94a5 9af1 2ac5 4100 0000  b....>....*.A...
+00003d40: 1000 7600 6900 6400 6500 6f00 5f00 7000  ..v.i.d.e.o._.p.
+00003d50: 7200 6f00 6300 6500 7300 7300 6f00 7200  r.o.c.e.s.s.o.r.
+00003d60: 736d 6f64 4462 6c6f 6200 0000 0870 7bbe  smodDblob....p{.
+00003d70: 2bd6 2ac5 4100 0000 1000 7600 6900 6400  +.*.A.....v.i.d.
+00003d80: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
+00003d90: 7300 7300 6f00 7200 7370 6831 5363 6f6d  s.s.o.r.sph1Scom
+00003da0: 7000 0000 0000 0770 0000 0000 1000 7600  p......p......v.
+00003db0: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
+00003dc0: 6300 6500 7300 7300 6f00 7200 7376 5372  c.e.s.s.o.r.svSr
+00003dd0: 6e6c 6f6e 6700 0000 0100 0000 0000 0000  nlong...........
 00003de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1035,17 +1035,17 @@
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
 00004100: 005f 6c67 3153 636f 6d70 0000 0000 0002  ._lg1Scomp......
-00004110: 5ebd 0000 000b 005f 005f 0070 0079 0063  ^......_._.p.y.c
+00004110: 5ebf 0000 000b 005f 005f 0070 0079 0063  ^......_._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 85f6 aa84 f02a c541  blob.........*.A
+00004130: 626c 6f62 0000 0008 55ee c677 912b c541  blob....U..w.+.A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
 00004160: 6f62 0000 0008 2902 255f d129 c541 0000  ob....).%_.).A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
 00004190: 0000 0000 0002 a000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
@@ -1351,153 +1351,153 @@
 00005460: 6200 0000 0874 2dd3 1049 1ec5 4100 0000  b....t-..I..A...
 00005470: 0800 6400 6100 7300 6800 5f00 6100 7000  ..d.a.s.h._.a.p.
 00005480: 7070 6831 5363 6f6d 7000 0000 0000 0150  pph1Scomp......P
 00005490: 0000 0000 0800 6400 6100 7300 6800 5f00  ......d.a.s.h._.
 000054a0: 6100 7000 7076 5372 6e6c 6f6e 6700 0000  a.p.pvSrnlong...
 000054b0: 0100 0000 0f00 6400 6100 7400 6100 5f00  ......d.a.t.a._.
 000054c0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-000054d0: 7200 7362 7773 7062 6c6f 6200 0000 ca62  r.sbwspblob....b
-000054e0: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
-000054f0: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
-00005500: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
-00005510: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00005520: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00005530: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00005540: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00005550: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
-00005560: 7b7b 3335 342c 2031 3234 7d2c 207b 3130  {{354, 124}, {10
-00005570: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
-00005580: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
-00005590: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-000055a0: 0000 0000 0000 0000 9b00 0000 0f00 6400  ..............d.
-000055b0: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
-000055c0: 6500 7300 7300 6f00 7200 7364 7363 6c62  e.s.s.o.r.sdsclb
-000055d0: 6f6f 6c00 0000 000f 0064 0061 0074 0061  ool......d.a.t.a
-000055e0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
-000055f0: 006f 0072 0073 6c67 3153 636f 6d70 0000  .o.r.slg1Scomp..
-00005600: 0000 0006 b2a0 0000 000f 0064 0061 0074  ...........d.a.t
-00005610: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
-00005620: 0073 006f 0072 0073 6c73 7643 626c 6f62  .s.o.r.slsvCblob
-00005630: 0000 0281 6270 6c69 7374 3030 d801 0203  ....bplist00....
-00005640: 0405 0607 0809 0a0b 1646 4748 0a5f 1012  .........FGH._..
-00005650: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
-00005660: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
-00005670: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00005680: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00005690: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-000056a0: 6c75 6d6e 5869 636f 6e53 697a 655f 1010  lumnXiconSize_..
-000056b0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000056c0: 1001 09ab 0c15 1a1f 2328 2d32 373c 41d4  ........#(-27<A.
-000056d0: 0d0e 0f10 1112 0a0a 5a69 6465 6e74 6966  ........Zidentif
-000056e0: 6965 7255 7769 6474 6859 6173 6365 6e64  ierUwidthYascend
-000056f0: 696e 6757 7669 7369 626c 6554 6e61 6d65  ingWvisibleTname
-00005700: 1101 c709 09d4 100e 0f0d 1617 1619 0810  ................
-00005710: 2308 5875 6269 7175 6974 79d4 0d0e 0f10  #.Xubiquity.....
-00005720: 1b1c 160a 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
-00005730: 6410 b508 09d4 0d0e 0f10 201c 1616 5b64  d......... ...[d
-00005740: 6174 6543 7265 6174 6564 0808 d40d 0e0f  ateCreated......
-00005750: 1024 2516 0a54 7369 7a65 1061 0809 d40d  .$%..Tsize.a....
-00005760: 0e0f 1029 2a0a 0a54 6b69 6e64 1073 0909  ...)*..Tkind.s..
-00005770: d40d 0e0f 102e 2f0a 1655 6c61 6265 6c10  ....../..Ulabel.
-00005780: 6409 08d4 0d0e 0f10 3334 0a16 5776 6572  d.......34..Wver
-00005790: 7369 6f6e 104b 0908 d40d 0e0f 1038 390a  sion.K.......89.
-000057a0: 1658 636f 6d6d 656e 7473 1101 2c09 08d4  .Xcomments..,...
-000057b0: 0d0e 0f10 3d3e 1616 5e64 6174 654c 6173  ....=>..^dateLas
-000057c0: 744f 7065 6e65 6410 c808 08d4 100e 0f0d  tOpened.........
-000057d0: 161c 1644 0808 5964 6174 6541 6464 6564  ...D..YdateAdded
-000057e0: 0823 4028 0000 0000 0000 5c64 6174 654d  .#@(......\dateM
-000057f0: 6f64 6966 6965 6423 4030 0000 0000 0000  odified#@0......
-00005800: 0900 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-00005810: 7000 7900 8c00 8e00 8f00 9b00 a400 af00  p.y.............
-00005820: b500 bf00 c700 cc00 cf00 d000 d100 da00  ................
-00005830: db00 dd00 de00 e700 f000 fd00 ff01 0001  ................
-00005840: 0101 0a01 1601 1701 1801 2101 2601 2801  ..........!.&.(.
-00005850: 2901 2a01 3301 3801 3a01 3b01 3c01 4501  ).*.3.8.:.;.<.E.
-00005860: 4b01 4d01 4e01 4f01 5801 6001 6201 6301  K.M.N.O.X.`.b.c.
-00005870: 6401 6d01 7601 7901 7a01 7b01 8401 9301  d.m.v.y.z.{.....
-00005880: 9501 9601 9701 a001 a101 a201 ac01 ad01  ................
-00005890: b601 c301 cc00 0000 0000 0002 0100 0000  ................
-000058a0: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
-000058b0: 0000 0001 cd00 0000 0f00 6400 6100 7400  ..........d.a.t.
-000058c0: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
-000058d0: 7300 6f00 7200 736c 7376 7062 6c6f 6200  s.o.r.slsvpblob.
-000058e0: 0002 6662 706c 6973 7430 30d8 0102 0304  ..fbplist00.....
-000058f0: 0506 0708 090a 0b1a 4546 470a 5f10 1276  ........EFG._..v
-00005900: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
-00005910: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
-00005920: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
-00005930: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
-00005940: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
-00005950: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
-00005960: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
-00005970: 0109 d90c 0d0e 0f10 1112 1314 151e 2327  ..............#'
-00005980: 2b30 353a 3f58 636f 6d6d 656e 7473 5e64  +05:?Xcomments^d
-00005990: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
-000059a0: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
-000059b0: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-000059c0: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-000059d0: 616d 65d4 1617 1819 1a1b 0a1d 5776 6973  ame.........Wvis
-000059e0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-000059f0: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
-00005a00: 07d4 1617 1819 1a20 1a22 0810 c808 1008  ....... ."......
-00005a10: d416 1718 190a 251a 0909 10b5 08d4 1617  ......%.........
-00005a20: 1819 1a25 1a2a 0808 1002 d416 1718 190a  ...%.*..........
-00005a30: 2d1a 2f09 1061 0810 03d4 1617 1819 1a32  -./..a.........2
-00005a40: 0a34 0810 6409 1005 d416 1718 190a 370a  .4..d.........7.
-00005a50: 3909 1073 0910 04d4 1617 1819 1a3c 0a3e  9..s.........<.>
-00005a60: 0810 4b09 1006 d416 1718 190a 410a 4309  ..K.........A.C.
-00005a70: 1101 c709 1000 0823 4028 0000 0000 0000  .......#@(......
-00005a80: 5c64 6174 654d 6f64 6966 6965 6423 4030  \dateModified#@0
-00005a90: 0000 0000 0000 0900 0800 1900 2e00 4000  ..............@.
-00005aa0: 4800 5c00 6500 7000 7900 8c00 8e00 8f00  H.\.e.p.y.......
-00005ab0: a200 ab00 ba00 c700 d300 d800 de00 e300  ................
-00005ac0: eb00 f000 f901 0101 0701 1101 1701 1801  ................
-00005ad0: 1b01 1c01 1e01 2701 2801 2a01 2b01 2d01  ......'.(.*.+.-.
-00005ae0: 3601 3701 3901 3a01 4301 4401 4501 4701  6.7.9.:.C.D.E.G.
-00005af0: 5001 5101 5301 5401 5601 5f01 6001 6201  P.Q.S.T.V._.`.b.
-00005b00: 6301 6501 6e01 6f01 7101 7201 7401 7d01  c.e.n.o.q.r.t.}.
-00005b10: 7e01 8001 8101 8301 8c01 8d01 9001 9101  ~...............
-00005b20: 9301 9401 9d01 aa01 b300 0000 0000 0002  ................
-00005b30: 0100 0000 0000 0000 4900 0000 0000 0000  ........I.......
-00005b40: 0000 0000 0000 0001 b400 0000 0f00 6400  ..............d.
-00005b50: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
-00005b60: 6500 7300 7300 6f00 7200 736d 6f44 4462  e.s.s.o.r.smoDDb
-00005b70: 6c6f 6200 0000 083b e05c 3068 26c5 4100  lob....;.\0h&.A.
-00005b80: 0000 0f00 6400 6100 7400 6100 5f00 7000  ....d.a.t.a._.p.
-00005b90: 7200 6f00 6300 6500 7300 7300 6f00 7200  r.o.c.e.s.s.o.r.
-00005ba0: 736d 6f64 4462 6c6f 6200 0000 083b e05c  smodDblob....;.\
-00005bb0: 3068 26c5 4100 0000 0f00 6400 6100 7400  0h&.A.....d.a.t.
-00005bc0: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
-00005bd0: 7300 6f00 7200 7370 6831 5363 6f6d 7000  s.o.r.sph1Scomp.
-00005be0: 0000 0000 08a0 0000 0000 0f00 6400 6100  ............d.a.
-00005bf0: 7400 6100 5f00 7000 7200 6f00 6300 6500  t.a._.p.r.o.c.e.
-00005c00: 7300 7300 6f00 7200 7376 5372 6e6c 6f6e  s.s.o.r.svSrnlon
-00005c10: 6700 0000 0100 0000 1200 6600 6500 6100  g.........f.e.a.
-00005c20: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
-00005c30: 7200 6100 6300 7400 6f00 7200 7362 7773  r.a.c.t.o.r.sbws
-00005c40: 7062 6c6f 6200 0000 c962 706c 6973 7430  pblob....bplist0
-00005c50: 30d7 0102 0304 0506 0708 080a 080a 0d0a  0...............
-00005c60: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-00005c70: 686f 7750 6174 6862 6172 5b53 686f 7754  howPathbar[ShowT
-00005c80: 6f6f 6c62 6172 5b53 686f 7754 6162 5669  oolbar[ShowTabVi
-00005c90: 6577 5f10 1443 6f6e 7461 696e 6572 5368  ew_..ContainerSh
-00005ca0: 6f77 5369 6465 6261 725c 5769 6e64 6f77  owSidebar\Window
-00005cb0: 426f 756e 6473 5b53 686f 7753 6964 6562  Bounds[ShowSideb
-00005cc0: 6172 0808 0908 095f 1018 7b7b 3330 372c  ar....._..{{307,
-00005cd0: 2038 367d 2c20 7b31 3037 362c 2036 3231   86}, {1076, 621
-00005ce0: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
-00005cf0: 7e99 0000 0000 0000 0101 0000 0000 0000  ~...............
-00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
-00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
-00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
-00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
-00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
-00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
-00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
-00005d70: 6f6d 7000 0000 0000 0b5a cc10 c808 5e64  omp......Z....^d
+000054d0: 7200 7362 7773 7062 6c6f 6200 0000 b962  r.sbwspblob....b
+000054e0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
+000054f0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+00005500: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
+00005510: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
+00005520: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
+00005530: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
+00005540: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
+00005550: 197b 7b32 3630 2c20 3132 397d 2c20 7b31  .{{260, 129}, {1
+00005560: 3138 302c 2036 3336 7d7d 0908 1523 2f3b  180, 636}}...#/;
+00005570: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
+00005580: 0000 0000 0000 000d 0000 0000 0000 0000  ................
+00005590: 0000 0000 0000 008c 0000 000f 0064 0061  .............d.a
+000055a0: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
+000055b0: 0073 0073 006f 0072 0073 6473 636c 626f  .s.s.o.r.sdsclbo
+000055c0: 6f6c 0000 0000 0f00 6400 6100 7400 6100  ol......d.a.t.a.
+000055d0: 5f00 7000 7200 6f00 6300 6500 7300 7300  _.p.r.o.c.e.s.s.
+000055e0: 6f00 7200 736c 6731 5363 6f6d 7000 0000  o.r.slg1Scomp...
+000055f0: 0000 06b2 a000 0000 0f00 6400 6100 7400  ..........d.a.t.
+00005600: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
+00005610: 7300 6f00 7200 736c 7376 4362 6c6f 6200  s.o.r.slsvCblob.
+00005620: 0002 8162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
+00005630: 0506 0708 090a 0b16 4647 480a 5f10 1276  ........FGH._..v
+00005640: 6965 774f 7074 696f 6e73 5665 7273 696f  iewOptionsVersio
+00005650: 6e5f 100f 7368 6f77 4963 6f6e 5072 6576  n_..showIconPrev
+00005660: 6965 7757 636f 6c75 6d6e 735f 1011 6361  iewWcolumns_..ca
+00005670: 6c63 756c 6174 6541 6c6c 5369 7a65 7358  lculateAllSizesX
+00005680: 7465 7874 5369 7a65 5a73 6f72 7443 6f6c  textSizeZsortCol
+00005690: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
+000056a0: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
+000056b0: 0109 ab0c 151a 1f23 282d 3237 3c41 d40d  .......#(-27<A..
+000056c0: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
+000056d0: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
+000056e0: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
+000056f0: 01c7 0909 d410 0e0f 0d16 1716 1908 1023  ...............#
+00005700: 0858 7562 6971 7569 7479 d40d 0e0f 101b  .Xubiquity......
+00005710: 1c16 0a5c 6461 7465 4d6f 6469 6669 6564  ...\dateModified
+00005720: 10b5 0809 d40d 0e0f 1020 1c16 165b 6461  ......... ...[da
+00005730: 7465 4372 6561 7465 6408 08d4 0d0e 0f10  teCreated.......
+00005740: 2425 160a 5473 697a 6510 6108 09d4 0d0e  $%..Tsize.a.....
+00005750: 0f10 292a 0a0a 546b 696e 6410 7309 09d4  ..)*..Tkind.s...
+00005760: 0d0e 0f10 2e2f 0a16 556c 6162 656c 1064  ...../..Ulabel.d
+00005770: 0908 d40d 0e0f 1033 340a 1657 7665 7273  .......34..Wvers
+00005780: 696f 6e10 4b09 08d4 0d0e 0f10 3839 0a16  ion.K.......89..
+00005790: 5863 6f6d 6d65 6e74 7311 012c 0908 d40d  Xcomments..,....
+000057a0: 0e0f 103d 3e16 165e 6461 7465 4c61 7374  ...=>..^dateLast
+000057b0: 4f70 656e 6564 10c8 0808 d410 0e0f 0d16  Opened..........
+000057c0: 1c16 4408 0859 6461 7465 4164 6465 6408  ..D..YdateAdded.
+000057d0: 2340 2800 0000 0000 005c 6461 7465 4d6f  #@(......\dateMo
+000057e0: 6469 6669 6564 2340 3000 0000 0000 0009  dified#@0.......
+000057f0: 0008 0019 002e 0040 0048 005c 0065 0070  .......@.H.\.e.p
+00005800: 0079 008c 008e 008f 009b 00a4 00af 00b5  .y..............
+00005810: 00bf 00c7 00cc 00cf 00d0 00d1 00da 00db  ................
+00005820: 00dd 00de 00e7 00f0 00fd 00ff 0100 0101  ................
+00005830: 010a 0116 0117 0118 0121 0126 0128 0129  .........!.&.(.)
+00005840: 012a 0133 0138 013a 013b 013c 0145 014b  .*.3.8.:.;.<.E.K
+00005850: 014d 014e 014f 0158 0160 0162 0163 0164  .M.N.O.X.`.b.c.d
+00005860: 016d 0176 0179 017a 017b 0184 0193 0195  .m.v.y.z.{......
+00005870: 0196 0197 01a0 01a1 01a2 01ac 01ad 01b6  ................
+00005880: 01c3 01cc 0000 0000 0000 0201 0000 0000  ................
+00005890: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
+000058a0: 0000 01cd 0000 000f 0064 0061 0074 0061  .........d.a.t.a
+000058b0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
+000058c0: 006f 0072 0073 6c73 7670 626c 6f62 0000  .o.r.slsvpblob..
+000058d0: 0266 6270 6c69 7374 3030 d801 0203 0405  .fbplist00......
+000058e0: 0607 0809 0a0b 1a45 4647 0a5f 1012 7669  .......EFG._..vi
+000058f0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+00005900: 5f10 0f73 686f 7749 636f 6e50 7265 7669  _..showIconPrevi
+00005910: 6577 5763 6f6c 756d 6e73 5f10 1163 616c  ewWcolumns_..cal
+00005920: 6375 6c61 7465 416c 6c53 697a 6573 5874  culateAllSizesXt
+00005930: 6578 7453 697a 655a 736f 7274 436f 6c75  extSizeZsortColu
+00005940: 6d6e 5869 636f 6e53 697a 655f 1010 7573  mnXiconSize_..us
+00005950: 6552 656c 6174 6976 6544 6174 6573 1001  eRelativeDates..
+00005960: 09d9 0c0d 0e0f 1011 1213 1415 1e23 272b  .............#'+
+00005970: 3035 3a3f 5863 6f6d 6d65 6e74 735e 6461  05:?Xcomments^da
+00005980: 7465 4c61 7374 4f70 656e 6564 5c64 6174  teLastOpened\dat
+00005990: 654d 6f64 6966 6965 645b 6461 7465 4372  eModified[dateCr
+000059a0: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+000059b0: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+000059c0: 6d65 d416 1718 191a 1b0a 1d57 7669 7369  me.........Wvisi
+000059d0: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+000059e0: 696e 6755 696e 6465 7808 1101 2c09 1007  ingUindex...,...
+000059f0: d416 1718 191a 201a 2208 10c8 0810 08d4  ...... .".......
+00005a00: 1617 1819 0a25 1a09 0910 b508 d416 1718  .....%..........
+00005a10: 191a 251a 2a08 0810 02d4 1617 1819 0a2d  ..%.*..........-
+00005a20: 1a2f 0910 6108 1003 d416 1718 191a 320a  ./..a.........2.
+00005a30: 3408 1064 0910 05d4 1617 1819 0a37 0a39  4..d.........7.9
+00005a40: 0910 7309 1004 d416 1718 191a 3c0a 3e08  ..s.........<.>.
+00005a50: 104b 0910 06d4 1617 1819 0a41 0a43 0911  .K.........A.C..
+00005a60: 01c7 0910 0008 2340 2800 0000 0000 005c  ......#@(......\
+00005a70: 6461 7465 4d6f 6469 6669 6564 2340 3000  dateModified#@0.
+00005a80: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
+00005a90: 005c 0065 0070 0079 008c 008e 008f 00a2  .\.e.p.y........
+00005aa0: 00ab 00ba 00c7 00d3 00d8 00de 00e3 00eb  ................
+00005ab0: 00f0 00f9 0101 0107 0111 0117 0118 011b  ................
+00005ac0: 011c 011e 0127 0128 012a 012b 012d 0136  .....'.(.*.+.-.6
+00005ad0: 0137 0139 013a 0143 0144 0145 0147 0150  .7.9.:.C.D.E.G.P
+00005ae0: 0151 0153 0154 0156 015f 0160 0162 0163  .Q.S.T.V._.`.b.c
+00005af0: 0165 016e 016f 0171 0172 0174 017d 017e  .e.n.o.q.r.t.}.~
+00005b00: 0180 0181 0183 018c 018d 0190 0191 0193  ................
+00005b10: 0194 019d 01aa 01b3 0000 0000 0000 0201  ................
+00005b20: 0000 0000 0000 0049 0000 0000 0000 0000  .......I........
+00005b30: 0000 0000 0000 01b4 0000 000f 0064 0061  .............d.a
+00005b40: 0074 0061 005f 0070 0072 006f 0063 0065  .t.a._.p.r.o.c.e
+00005b50: 0073 0073 006f 0072 0073 6d6f 4444 626c  .s.s.o.r.smoDDbl
+00005b60: 6f62 0000 0008 3be0 5c30 6826 c541 0000  ob....;.\0h&.A..
+00005b70: 000f 0064 0061 0074 0061 005f 0070 0072  ...d.a.t.a._.p.r
+00005b80: 006f 0063 0065 0073 0073 006f 0072 0073  .o.c.e.s.s.o.r.s
+00005b90: 6d6f 6444 626c 6f62 0000 0008 3be0 5c30  modDblob....;.\0
+00005ba0: 6826 c541 0000 000f 0064 0061 0074 0061  h&.A.....d.a.t.a
+00005bb0: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
+00005bc0: 006f 0072 0073 7068 3153 636f 6d70 0000  .o.r.sph1Scomp..
+00005bd0: 0000 0008 a000 0000 000f 0064 0061 0074  ...........d.a.t
+00005be0: 0061 005f 0070 0072 006f 0063 0065 0073  .a._.p.r.o.c.e.s
+00005bf0: 0073 006f 0072 0073 7653 726e 6c6f 6e67  .s.o.r.svSrnlong
+00005c00: 0000 0001 0000 0012 0066 0065 0061 0074  .........f.e.a.t
+00005c10: 0075 0072 0065 005f 0065 0078 0074 0072  .u.r.e._.e.x.t.r
+00005c20: 0061 0063 0074 006f 0072 0073 6277 7370  .a.c.t.o.r.sbwsp
+00005c30: 626c 6f62 0000 00b9 6270 6c69 7374 3030  blob....bplist00
+00005c40: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+00005c50: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00005c60: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00005c70: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00005c80: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00005c90: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00005ca0: 6261 7208 0908 095f 1019 7b7b 3236 302c  bar...._..{{260,
+00005cb0: 2031 3239 7d2c 207b 3131 3830 2c20 3633   129}, {1180, 63
+00005cc0: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
+00005cd0: 8b00 0000 0000 0001 0100 0000 0000 0000  ................
+00005ce0: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
+00005cf0: 8c00 0000 1200 6600 6500 6100 7400 7500  ......f.e.a.t.u.
+00005d00: 7200 6500 5f00 6500 7800 7400 7200 6100  r.e._.e.x.t.r.a.
+00005d10: 6300 7400 6f00 7200 7364 7363 6c62 6f6f  c.t.o.r.sdsclboo
+00005d20: 6c00 0000 0012 0066 0065 0061 0074 0075  l......f.e.a.t.u
+00005d30: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
+00005d40: 0063 0074 006f 0072 0073 6c67 3153 636f  .c.t.o.r.slg1Sco
+00005d50: 6d70 0000 0000 000b 77d4 d40d 0e0f 1016  mp......w.......
+00005d60: 390a 3b08 1101 2c09 5863 6f6d 6d65 6e74  9.;...,.Xcomment
+00005d70: 73d4 0d0e 0f10 163e 1640 0810 c808 5e64  s......>.@....^d
 00005d80: 6174 654c 6173 744f 7065 6e65 64d4 0d0e  ateLastOpened...
 00005d90: 0f10 161c 1644 0808 5964 6174 6541 6464  .....D..YdateAdd
 00005da0: 6564 0823 4028 0000 0000 0000 546e 616d  ed.#@(......Tnam
 00005db0: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
 00005dc0: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
 00005dd0: 8e00 8f00 9b00 a400 ac00 b200 bc00 c700  ................
 00005de0: c800 cb00 cc00 d100 da00 db00 dd00 de00  ................
@@ -1579,22 +1579,22 @@
 000062a0: a501 ae01 b001 b201 b301 b401 bd01 bf01  ................
 000062b0: c201 c301 c401 c501 ce01 d701 e400 0000  ................
 000062c0: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
 000062d0: 0000 0000 0000 0000 0000 0001 e500 0000  ................
 000062e0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000062f0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 00006300: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
-00006310: 087c 26ff 39a7 29c5 4100 0000 1200 6600  .|&.9.).A.....f.
+00006310: 086e 2ef7 c457 2cc5 4100 0000 1200 6600  .n...W,.A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
-00006340: 736d 6f64 4462 6c6f 6200 0000 087c 26ff  smodDblob....|&.
-00006350: 39a7 29c5 4100 0000 1200 6600 6500 6100  9.).A.....f.e.a.
+00006340: 736d 6f64 4462 6c6f 6200 0000 086e 2ef7  smodDblob....n..
+00006350: c457 2cc5 4100 0000 1200 6600 6500 6100  .W,.A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
-00006380: 5363 6f6d 7000 0000 0000 0de0 0000 0000  Scomp...........
+00006380: 5363 6f6d 7000 0000 0000 0df0 0000 0000  Scomp...........
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
 000063e0: 0000 b862 706c 6973 7430 30d6 0102 0304  ...bplist00.....
 000063f0: 0506 0708 0708 0b08 5d53 686f 7753 7461  ........]ShowSta
@@ -1699,71 +1699,71 @@
 00006a20: 626c 6f62 0000 0008 6a3a 0fc2 4122 c541  blob....j:..A".A
 00006a30: 0000 0009 006c 0061 0062 0065 006c 006c  .....l.a.b.e.l.l
 00006a40: 0069 006e 0067 7068 3153 636f 6d70 0000  .i.n.gph1Scomp..
 00006a50: 0000 0003 a000 0000 0009 006c 0061 0062  ...........l.a.b
 00006a60: 0065 006c 006c 0069 006e 0067 7653 726e  .e.l.l.i.n.gvSrn
 00006a70: 6c6f 6e67 0000 0001 0000 0006 006d 0069  long.........m.i
 00006a80: 0078 0069 006e 0073 6277 7370 626c 6f62  .x.i.n.sbwspblob
-00006a90: 0000 00c8 6270 6c69 7374 3030 d701 0203  ....bplist00....
-00006aa0: 0405 0607 0808 0a08 0a0d 0a5d 5368 6f77  ...........]Show
-00006ab0: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
-00006ac0: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
-00006ad0: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
-00006ae0: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
-00006af0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
-00006b00: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
-00006b10: 0809 5f10 177b 7b30 2c20 3130 357d 2c20  .._..{{0, 105}, 
-00006b20: 7b31 3139 392c 2037 3639 7d7d 0908 1725  {1199, 769}}...%
-00006b30: 313d 4960 6d79 7a7b 7c7d 7e98 0000 0000  1=I`myz{|}~.....
-00006b40: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-00006b50: 0000 0000 0000 0000 0000 0099 0000 0006  ................
-00006b60: 006d 0069 0078 0069 006e 0073 6c67 3153  .m.i.x.i.n.slg1S
-00006b70: 636f 6d70 0000 0000 0010 6607 0000 0006  comp......f.....
-00006b80: 006d 0069 0078 0069 006e 0073 6c73 7643  .m.i.x.i.n.slsvC
-00006b90: 626c 6f62 0000 0281 6270 6c69 7374 3030  blob....bplist00
-00006ba0: d801 0203 0405 0607 0809 0a0b 1646 4748  .............FGH
-00006bb0: 0a5f 1012 7669 6577 4f70 7469 6f6e 7356  ._..viewOptionsV
-00006bc0: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
-00006bd0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00006be0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00006bf0: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
-00006c00: 7274 436f 6c75 6d6e 5869 636f 6e53 697a  rtColumnXiconSiz
-00006c10: 655f 1010 7573 6552 656c 6174 6976 6544  e_..useRelativeD
-00006c20: 6174 6573 1001 09ab 0c15 1a1f 2328 2d32  ates........#(-2
-00006c30: 373c 41d4 0d0e 0f10 1112 0a0a 5a69 6465  7<A.........Zide
-00006c40: 6e74 6966 6965 7255 7769 6474 6859 6173  ntifierUwidthYas
-00006c50: 6365 6e64 696e 6757 7669 7369 626c 6554  cendingWvisibleT
-00006c60: 6e61 6d65 1101 c709 09d4 100e 0f0d 1617  name............
-00006c70: 1619 0810 2308 5875 6269 7175 6974 79d4  ....#.Xubiquity.
-00006c80: 0d0e 0f10 1b1c 160a 5c64 6174 654d 6f64  ........\dateMod
-00006c90: 6966 6965 6410 b508 09d4 0d0e 0f10 201c  ified......... .
-00006ca0: 1616 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
-00006cb0: d40d 0e0f 1024 2516 0a54 7369 7a65 1061  .....$%..Tsize.a
-00006cc0: 0809 d40d 0e0f 1029 2a0a 0a54 6b69 6e64  .......)*..Tkind
-00006cd0: 1073 0909 d40d 0e0f 102e 2f0a 1655 6c61  .s......../..Ula
-00006ce0: 6265 6c10 6409 08d4 0d0e 0f10 3334 0a16  bel.d.......34..
-00006cf0: 5776 6572 7369 6f6e 104b 0908 d40d 0e0f  Wversion.K......
-00006d00: 1038 390a 1658 636f 6d6d 656e 7473 1101  .89..Xcomments..
-00006d10: 2c09 08d4 0d0e 0f10 3d3e 1616 5e64 6174  ,.......=>..^dat
-00006d20: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
-00006d30: 100e 0f0d 161c 1644 0808 5964 6174 6541  .......D..YdateA
-00006d40: 6464 6564 0823 4028 0000 0000 0000 5c64  dded.#@(......\d
-00006d50: 6174 654d 6f64 6966 6965 6423 4030 0000  ateModified#@0..
-00006d60: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
-00006d70: 5c00 6500 7000 7900 8c00 8e00 8f00 9b00  \.e.p.y.........
-00006d80: a400 af00 b500 bf00 c700 cc00 cf00 d000  ................
-00006d90: d100 da00 db00 dd00 de00 e700 f000 fd00  ................
-00006da0: ff01 0001 0101 0a01 1601 1701 1801 2101  ..............!.
-00006db0: 2601 2801 2901 2a01 3301 3801 3a01 3b01  &.(.).*.3.8.:.;.
-00006dc0: 3c01 4501 4b01 4d01 4e01 4f01 5801 6001  <.E.K.M.N.O.X.`.
-00006dd0: 6201 6301 6401 6d01 7601 7901 7a01 7b01  b.c.d.m.v.y.z.{.
-00006de0: 8401 9301 9501 9601 9701 a001 a101 a201  ................
-00006df0: ac01 ad01 b601 c301 cc00 0000 0000 0002  ................
-00006e00: 0100 0000 0000 0000 4a00 0000 0000 0000  ........J.......
-00006e10: 0000 0000 0000 0001 cd01 4601 4801 4901  ..........F.H.I.
+00006a90: 0000 00b9 6270 6c69 7374 3030 d601 0203  ....bplist00....
+00006aa0: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
+00006ab0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
+00006ac0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00006ad0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00006ae0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00006af0: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00006b00: 0908 095f 1019 7b7b 3236 302c 2031 3239  ..._..{{260, 129
+00006b10: 7d2c 207b 3131 3830 2c20 3633 367d 7d09  }, {1180, 636}}.
+00006b20: 0815 232f 3b52 5f6b 6c6d 6e6f 8b00 0000  ..#/;R_klmno....
+00006b30: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
+00006b40: 0000 0000 0000 0000 0000 0000 8c00 0000  ................
+00006b50: 0600 6d00 6900 7800 6900 6e00 736c 6731  ..m.i.x.i.n.slg1
+00006b60: 5363 6f6d 7000 0000 0000 1072 d000 0000  Scomp......r....
+00006b70: 0600 6d00 6900 7800 6900 6e00 736c 7376  ..m.i.x.i.n.slsv
+00006b80: 4362 6c6f 6200 0002 8162 706c 6973 7430  Cblob....bplist0
+00006b90: 30d8 0102 0304 0506 0708 090a 0b16 4647  0.............FG
+00006ba0: 480a 5f10 1276 6965 774f 7074 696f 6e73  H._..viewOptions
+00006bb0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
+00006bc0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
+00006bd0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
+00006be0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
+00006bf0: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
+00006c00: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
+00006c10: 4461 7465 7310 0109 ab0c 151a 1f23 282d  Dates........#(-
+00006c20: 3237 3c41 d40d 0e0f 1011 120a 0a5a 6964  27<A.........Zid
+00006c30: 656e 7469 6669 6572 5577 6964 7468 5961  entifierUwidthYa
+00006c40: 7363 656e 6469 6e67 5776 6973 6962 6c65  scendingWvisible
+00006c50: 546e 616d 6511 01c7 0909 d410 0e0f 0d16  Tname...........
+00006c60: 1716 1908 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
+00006c70: d40d 0e0f 101b 1c16 0a5c 6461 7465 4d6f  .........\dateMo
+00006c80: 6469 6669 6564 10b5 0809 d40d 0e0f 1020  dified......... 
+00006c90: 1c16 165b 6461 7465 4372 6561 7465 6408  ...[dateCreated.
+00006ca0: 08d4 0d0e 0f10 2425 160a 5473 697a 6510  ......$%..Tsize.
+00006cb0: 6108 09d4 0d0e 0f10 292a 0a0a 546b 696e  a.......)*..Tkin
+00006cc0: 6410 7309 09d4 0d0e 0f10 2e2f 0a16 556c  d.s......../..Ul
+00006cd0: 6162 656c 1064 0908 d40d 0e0f 1033 340a  abel.d.......34.
+00006ce0: 1657 7665 7273 696f 6e10 4b09 08d4 0d0e  .Wversion.K.....
+00006cf0: 0f10 3839 0a16 5863 6f6d 6d65 6e74 7311  ..89..Xcomments.
+00006d00: 012c 0908 d40d 0e0f 103d 3e16 165e 6461  .,.......=>..^da
+00006d10: 7465 4c61 7374 4f70 656e 6564 10c8 0808  teLastOpened....
+00006d20: d410 0e0f 0d16 1c16 4408 0859 6461 7465  ........D..Ydate
+00006d30: 4164 6465 6408 2340 2800 0000 0000 005c  Added.#@(......\
+00006d40: 6461 7465 4d6f 6469 6669 6564 2340 3000  dateModified#@0.
+00006d50: 0000 0000 0009 0008 0019 002e 0040 0048  .............@.H
+00006d60: 005c 0065 0070 0079 008c 008e 008f 009b  .\.e.p.y........
+00006d70: 00a4 00af 00b5 00bf 00c7 00cc 00cf 00d0  ................
+00006d80: 00d1 00da 00db 00dd 00de 00e7 00f0 00fd  ................
+00006d90: 00ff 0100 0101 010a 0116 0117 0118 0121  ...............!
+00006da0: 0126 0128 0129 012a 0133 0138 013a 013b  .&.(.).*.3.8.:.;
+00006db0: 013c 0145 014b 014d 014e 014f 0158 0160  .<.E.K.M.N.O.X.`
+00006dc0: 0162 0163 0164 016d 0176 0179 017a 017b  .b.c.d.m.v.y.z.{
+00006dd0: 0184 0193 0195 0196 0197 01a0 01a1 01a2  ................
+00006de0: 01ac 01ad 01b6 01c3 01cc 0000 0000 0000  ................
+00006df0: 0201 0000 0000 0000 004a 0000 0000 0000  .........J......
+00006e00: 0000 0000 0000 0000 01cd 2501 2a01 3301  ..........%.*.3.
+00006e10: 3401 3601 3701 3c01 4501 4601 4801 4901  4.6.7.<.E.F.H.I.
 00006e20: 4f01 5801 5901 5b01 5c01 6401 6d01 6e01  O.X.Y.[.\.d.m.n.
 00006e30: 7101 7201 7b01 8401 8501 8701 8801 9701  q.r.{...........
 00006e40: a001 a101 a201 ac01 ad01 b601 bb01 c400  ................
 00006e50: 0000 0000 0002 0100 0000 0000 0000 4a00  ..............J.
 00006e60: 0000 0000 0000 0000 0000 0000 0001 c500  ................
 00006e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 e4a6 81c8 0729 c541  blob.........).A
+00007020: 626c 6f62 0000 0008 a399 d1ed 522c c541  blob........R,.A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 e4a6 81c8  modDblob........
-00007050: 0729 c541 0000 0006 006d 0069 0078 0069  .).A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 a399 d1ed  modDblob........
+00007050: 522c c541 0000 0006 006d 0069 0078 0069  R,.A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 0011 c000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 0011 d000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -2028,251 +2028,251 @@
 00007eb0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
 00007ec0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
 00007ed0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
 00007ee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
 00007ef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
 00007f00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
 00007f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
-00007f20: 197b 7b37 3035 2c20 3230 377d 2c20 7b31  .{{705, 207}, {1
-00007f30: 3234 372c 2035 3638 7d7d 0908 1523 2f3b  247, 568}}...#/;
+00007f20: 197b 7b32 3630 2c20 3132 397d 2c20 7b31  .{{260, 129}, {1
+00007f30: 3138 302c 2036 3336 7d7d 0908 1523 2f3b  180, 636}}...#/;
 00007f40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
 00007f50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 00007f60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
 00007f70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
-00007f80: 636f 6d70 0000 0000 000f f490 0000 0000  comp............
+00007f80: 636f 6d70 0000 0000 0010 0215 0000 0000  comp............
 00007f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
 00008010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-00008020: 6c73 7670 626c 6f62 0000 02a0 6270 6c69  lsvpblob....bpli
+00008020: 6c73 7670 626c 6f62 0000 02a8 6270 6c69  lsvpblob....bpli
 00008030: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00008040: 0c0d 1f47 4849 4a0c 4c5f 1012 7669 6577  ...GHIJ.L_..view
-00008050: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
-00008060: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00008070: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00008080: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00008090: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-000080a0: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-000080b0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-000080c0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-000080d0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
-000080e0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
-000080f0: 2a2f 3437 3c41 5863 6f6d 6d65 6e74 7355  */47<AXcommentsU
-00008100: 6c61 6265 6c57 7665 7273 696f 6e5b 6461  labelWversion[da
-00008110: 7465 4372 6561 7465 6454 7369 7a65 5c64  teCreatedTsize\d
-00008120: 6174 654d 6f64 6966 6965 6454 6b69 6e64  ateModifiedTkind
-00008130: 546e 616d 655e 6461 7465 4c61 7374 4f70  Tname^dateLastOp
-00008140: 656e 6564 d418 191a 1b1c 1d0c 1f55 696e  ened.........Uin
-00008150: 6465 7855 7769 6474 6859 6173 6365 6e64  dexUwidthYascend
-00008160: 696e 6757 7669 7369 626c 6510 0711 012c  ingWvisible....,
-00008170: 0908 d418 191a 1b21 220c 1f10 0510 6409  .......!".....d.
-00008180: 08d4 1819 1a1b 2627 0c1f 1006 104b 0908  ......&'.....K..
-00008190: d418 191a 1b2b 2c1f 1f10 0210 b508 08d4  .....+,.........
-000081a0: 1819 1a1b 3031 1f0c 1003 1061 0809 d418  ....01.....a....
-000081b0: 191a 1b0b 2c1f 0c08 09d4 1819 1a1b 3839  ....,.........89
-000081c0: 0c0c 1004 1073 0909 d418 191a 1b3d 3e0c  .....s.......=>.
-000081d0: 0c10 0011 01c7 0909 d418 191a 1b42 431f  .............BC.
-000081e0: 1f10 0810 c808 0808 2300 0000 0000 0000  ........#.......
-000081f0: 0023 4028 0000 0000 0000 2340 0000 0000  .#@(......#@....
-00008200: 0000 0054 6e61 6d65 0923 4030 0000 0000  ...Tname.#@0....
-00008210: 0000 0008 001d 0032 0044 004c 0060 0072  .......2.D.L.`.r
-00008220: 007b 008d 0098 00ab 00b4 00b6 00b7 00ca  .{..............
-00008230: 00d3 00d9 00e1 00ed 00f2 00ff 0104 0109  ................
-00008240: 0118 0121 0127 012d 0137 013f 0141 0144  ...!.'.-.7.?.A.D
-00008250: 0145 0146 014f 0151 0153 0154 0155 015e  .E.F.O.Q.S.T.U.^
-00008260: 0160 0162 0163 0164 016d 016f 0171 0172  .`.b.c.d.m.o.q.r
-00008270: 0173 017c 017e 0180 0181 0182 018b 018c  .s.|.~..........
-00008280: 018d 0196 0198 019a 019b 019c 01a5 01a7  ................
-00008290: 01aa 01ab 01ac 01b5 01b7 01b9 01ba 01bb  ................
-000082a0: 01bc 01c5 01ce 01d7 01dc 01dd 0000 0000  ................
-000082b0: 0000 0201 0000 0000 0000 004d 0000 0000  ...........M....
-000082c0: 0000 0000 0000 0000 0000 01e6 0000 0008  ................
-000082d0: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-000082e0: 6d6f 4444 626c 6f62 0000 0008 f673 8c57  moDDblob.....s.W
-000082f0: cd2a c541 0000 0008 0070 006c 006f 0074  .*.A.....p.l.o.t
-00008300: 0074 0069 006e 0067 6d6f 6444 626c 6f62  .t.i.n.gmodDblob
-00008310: 0000 0008 f673 8c57 cd2a c541 0000 0008  .....s.W.*.A....
-00008320: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-00008330: 7068 3153 636f 6d70 0000 0000 0014 2000  ph1Scomp...... .
-00008340: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
-00008350: 006e 0067 7653 726e 6c6f 6e67 0000 0001  .n.gvSrnlong....
-00008360: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-00008370: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-00008380: 0074 0069 006f 006e 0073 6277 7370 626c  .t.i.o.n.sbwspbl
-00008390: 6f62 0000 00ca 6270 6c69 7374 3030 d701  ob....bplist00..
-000083a0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-000083b0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-000083c0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-000083d0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-000083e0: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-000083f0: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00008400: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00008410: 0809 0809 5f10 197b 7b31 3337 2c20 3134  ...._..{{137, 14
-00008420: 337d 2c20 7b31 3330 322c 2037 3134 7d7d  3}, {1302, 714}}
-00008430: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e9a  ...%1=I`myz{|}~.
-00008440: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-00008450: 0000 0000 0000 0000 0000 0000 0000 009b  ................
-00008460: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-00008470: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-00008480: 0074 0069 006f 006e 0073 6473 636c 626f  .t.i.o.n.sdsclbo
-00008490: 6f6c 0000 0000 1300 7000 6f00 7300 6500  ol......p.o.s.e.
-000084a0: 5f00 6300 6f00 6e00 6600 6900 6700 7500  _.c.o.n.f.i.g.u.
-000084b0: 7200 6100 7400 6900 6f00 6e00 736c 6731  r.a.t.i.o.n.slg1
-000084c0: 5363 6f6d 7000 0000 0000 06ae 5600 0000  Scomp.......V...
-000084d0: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
-000084e0: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
-000084f0: 6900 6f00 6e00 736c 7376 4362 6c6f 6200  i.o.n.slsvCblob.
-00008500: 0002 b062 706c 6973 7430 30da 0102 0304  ...bplist00.....
-00008510: 0506 0708 090a 0b0c 0d18 4849 484a 4b0c  ..........HIHJK.
-00008520: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00008530: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
-00008540: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-00008550: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-00008560: 7a65 735f 100f 7363 726f 6c6c 506f 7369  zes_..scrollPosi
-00008570: 7469 6f6e 5958 7465 7874 5369 7a65 5f10  tionYXtextSize_.
-00008580: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e58  .scrollPositionX
-00008590: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
-000085a0: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
-000085b0: 7665 4461 7465 7310 0109 ab0e 171c 2125  veDates.......!%
-000085c0: 2a2f 3439 3e43 d40f 1011 120c 140c 1657  */49>C.........W
-000085d0: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
-000085e0: 6365 6e64 696e 675a 6964 656e 7469 6669  cendingZidentifi
-000085f0: 6572 0911 01c7 0954 6e61 6d65 d40f 1011  er.....Tname....
-00008600: 1218 1918 1b08 1023 0858 7562 6971 7569  .......#.Xubiqui
-00008610: 7479 d40f 1011 120c 1e18 2009 10b5 085c  ty........ ....\
-00008620: 6461 7465 4d6f 6469 6669 6564 d40f 1011  dateModified....
-00008630: 1218 1e18 2408 085b 6461 7465 4372 6561  ....$..[dateCrea
-00008640: 7465 64d4 0f10 1112 0c27 1829 0910 6108  ted......'.)..a.
-00008650: 5473 697a 65d4 0f10 1112 0c2c 0c2e 0910  Tsize......,....
-00008660: 7309 546b 696e 64d4 0f10 1112 1831 0c33  s.Tkind......1.3
-00008670: 0810 6409 556c 6162 656c d40f 1011 1218  ..d.Ulabel......
-00008680: 360c 3808 104b 0957 7665 7273 696f 6ed4  6.8..K.Wversion.
-00008690: 0f10 1112 183b 0c3d 0811 012c 0958 636f  .....;.=...,.Xco
-000086a0: 6d6d 656e 7473 d40f 1011 1218 4018 4208  mments......@.B.
-000086b0: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
-000086c0: 6564 d40f 1011 1218 1e18 4608 0859 6461  ed........F..Yda
-000086d0: 7465 4164 6465 6408 2300 0000 0000 0000  teAdded.#.......
-000086e0: 0023 4028 0000 0000 0000 546e 616d 6523  .#@(......Tname#
-000086f0: 4030 0000 0000 0000 0900 0800 1d00 3200  @0............2.
-00008700: 4400 4c00 6000 7200 7b00 8d00 9800 a100  D.L.`.r.{.......
-00008710: b400 b600 b700 c300 cc00 d400 da00 e400  ................
-00008720: ef00 f000 f300 f400 f901 0201 0301 0501  ................
-00008730: 0601 0f01 1801 1901 1b01 1c01 2901 3201  ............).2.
-00008740: 3301 3401 4001 4901 4a01 4c01 4d01 5201  3.4.@.I.J.L.M.R.
-00008750: 5b01 5c01 5e01 5f01 6401 6d01 6e01 7001  [.\.^._.d.m.n.p.
-00008760: 7101 7701 8001 8101 8301 8401 8c01 9501  q.w.............
-00008770: 9601 9901 9a01 a301 ac01 ad01 af01 b001  ................
-00008780: bf01 c801 c901 ca01 d401 d501 de01 e701  ................
-00008790: ec01 f500 0000 0000 0002 0100 0000 0000  ................
-000087a0: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
-000087b0: 0001 f600 0000 1300 7000 6f00 7300 6500  ........p.o.s.e.
-000087c0: 5f00 6300 6f00 6e00 6600 6900 6700 7500  _.c.o.n.f.i.g.u.
-000087d0: 7200 6100 7400 6900 6f00 6e00 736c 7376  r.a.t.i.o.n.slsv
-000087e0: 7062 6c6f 6200 0002 9562 706c 6973 7430  pblob....bplist0
-000087f0: 30da 0102 0304 0506 0708 090a 0b0c 0d1f  0...............
-00008800: 4748 4749 4a0c 5f10 1276 6965 774f 7074  GHGIJ._..viewOpt
-00008810: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
-00008820: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00008830: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00008840: 6541 6c6c 5369 7a65 735f 100f 7363 726f  eAllSizes_..scro
-00008850: 6c6c 506f 7369 7469 6f6e 5958 7465 7874  llPositionYXtext
-00008860: 5369 7a65 5f10 0f73 6372 6f6c 6c50 6f73  Size_..scrollPos
-00008870: 6974 696f 6e58 5a73 6f72 7443 6f6c 756d  itionXZsortColum
-00008880: 6e58 6963 6f6e 5369 7a65 5f10 1075 7365  nXiconSize_..use
-00008890: 5265 6c61 7469 7665 4461 7465 7310 0109  RelativeDates...
-000088a0: d90e 0f10 1112 1314 1516 1720 2529 2d32  ........... %)-2
-000088b0: 373c 4158 636f 6d6d 656e 7473 5e64 6174  7<AXcomments^dat
-000088c0: 654c 6173 744f 7065 6e65 645c 6461 7465  eLastOpened\date
-000088d0: 4d6f 6469 6669 6564 5b64 6174 6543 7265  Modified[dateCre
-000088e0: 6174 6564 5473 697a 6555 6c61 6265 6c54  atedTsizeUlabelT
-000088f0: 6b69 6e64 5776 6572 7369 6f6e 546e 616d  kindWversionTnam
-00008900: 65d4 1819 1a1b 1c1d 0c1f 5569 6e64 6578  e.........Uindex
-00008910: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-00008920: 5776 6973 6962 6c65 1007 1101 2c09 08d4  Wvisible....,...
-00008930: 1819 1a1b 2122 1f1f 1008 10c8 0808 d418  ....!"..........
-00008940: 191a 1b0b 261f 0c10 b508 09d4 1819 1a1b  ....&...........
-00008950: 2a26 1f1f 1002 0808 d418 191a 1b2e 2f1f  *&............/.
-00008960: 0c10 0310 6108 09d4 1819 1a1b 3334 0c1f  ....a.......34..
-00008970: 1005 1064 0908 d418 191a 1b38 390c 0c10  ...d.......89...
-00008980: 0410 7309 09d4 1819 1a1b 3d3e 0c1f 1006  ..s.......=>....
-00008990: 104b 0908 d418 191a 1b42 430c 0c10 0011  .K.......BC.....
-000089a0: 01c7 0909 0823 0000 0000 0000 0000 2340  .....#........#@
-000089b0: 2800 0000 0000 0054 6e61 6d65 2340 3000  (......Tname#@0.
-000089c0: 0000 0000 0009 0008 001d 0032 0044 004c  ...........2.D.L
-000089d0: 0060 0072 007b 008d 0098 00a1 00b4 00b6  .`.r.{..........
-000089e0: 00b7 00ca 00d3 00e2 00ef 00fb 0100 0106  ................
-000089f0: 010b 0113 0118 0121 0127 012d 0137 013f  .......!.'.-.7.?
-00008a00: 0141 0144 0145 0146 014f 0151 0153 0154  .A.D.E.F.O.Q.S.T
-00008a10: 0155 015e 0160 0161 0162 016b 016d 016e  .U.^.`.a.b.k.m.n
-00008a20: 016f 0178 017a 017c 017d 017e 0187 0189  .o.x.z.|.}.~....
-00008a30: 018b 018c 018d 0196 0198 019a 019b 019c  ................
-00008a40: 01a5 01a7 01a9 01aa 01ab 01b4 01b6 01b9  ................
-00008a50: 01ba 01bb 01bc 01c5 01ce 01d3 01dc 0000  ................
-00008a60: 0000 0000 0201 0000 0000 0000 004c 0000  .............L..
-00008a70: 0000 0000 0000 0000 0000 0000 01dd 0000  ................
-00008a80: 0013 0070 006f 0073 0065 005f 0063 006f  ...p.o.s.e._.c.o
-00008a90: 006e 0066 0069 0067 0075 0072 0061 0074  .n.f.i.g.u.r.a.t
-00008aa0: 0069 006f 006e 0073 6d6f 4444 626c 6f62  .i.o.n.smoDDblob
-00008ab0: 0000 0008 d97e 4b74 e2dd c441 0000 0013  .....~Kt...A....
-00008ac0: 0070 006f 0073 0065 005f 0063 006f 006e  .p.o.s.e._.c.o.n
-00008ad0: 0066 0069 0067 0075 0072 0061 0074 0069  .f.i.g.u.r.a.t.i
-00008ae0: 006f 006e 0073 6d6f 6444 626c 6f62 0000  .o.n.smodDblob..
-00008af0: 0008 d97e 4b74 e2dd c441 0000 0013 0070  ...~Kt...A.....p
-00008b00: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
-00008b10: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
-00008b20: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00008b30: 0007 3000 0000 0013 0070 006f 0073 0065  ..0......p.o.s.e
-00008b40: 005f 0063 006f 006e 0066 0069 0067 0075  ._.c.o.n.f.i.g.u
-00008b50: 0072 0061 0074 0069 006f 006e 0073 7653  .r.a.t.i.o.n.svS
-00008b60: 726e 6c6f 6e67 0000 0001 0000 001b 0070  rnlong.........p
-00008b70: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
-00008b80: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
-00008b90: 006e 0073 005f 0061 0072 0063 0068 0069  .n.s._.a.r.c.h.i
-00008ba0: 0076 0065 6c67 3153 636f 6d70 0000 0000  .v.elg1Scomp....
-00008bb0: 0006 faed 0000 001b 0070 006f 0073 0065  .........p.o.s.e
-00008bc0: 005f 0063 006f 006e 0066 0069 0067 0075  ._.c.o.n.f.i.g.u
-00008bd0: 0072 0061 0074 0069 006f 006e 0073 005f  .r.a.t.i.o.n.s._
-00008be0: 0061 0072 0063 0068 0069 0076 0065 6d6f  .a.r.c.h.i.v.emo
-00008bf0: 4444 626c 6f62 0000 0008 8983 1ea9 cbfe  DDblob..........
-00008c00: c441 0000 001b 0070 006f 0073 0065 005f  .A.....p.o.s.e._
-00008c10: 0063 006f 006e 0066 0069 0067 0075 0072  .c.o.n.f.i.g.u.r
-00008c20: 0061 0074 0069 006f 006e 0073 005f 0061  .a.t.i.o.n.s._.a
-00008c30: 0072 0063 0068 0069 0076 0065 6d6f 6444  .r.c.h.i.v.emodD
-00008c40: 626c 6f62 0000 0008 8983 1ea9 cbfe c441  blob...........A
-00008c50: 0000 001b 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
-00008c60: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
-00008c70: 0074 0069 006f 006e 0073 005f 0061 0072  .t.i.o.n.s._.a.r
-00008c80: 0063 0068 0069 0076 0065 7068 3153 636f  .c.h.i.v.eph1Sco
-00008c90: 6d70 0000 0000 0007 9000 0000 000e 0070  mp.............p
-00008ca0: 006f 0073 0065 005f 0069 006d 0070 006f  .o.s.e._.i.m.p.o
-00008cb0: 0072 0074 0065 0072 0073 6277 7370 626c  .r.t.e.r.sbwspbl
-00008cc0: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
-00008cd0: 0203 0405 0607 0808 0a08 0a0d 0a5d 5368  .............]Sh
-00008ce0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00008cf0: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
-00008d00: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00008d10: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00008d20: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00008d30: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00008d40: 0809 0809 5f10 187b 7b33 362c 2031 3331  ...._..{{36, 131
-00008d50: 7d2c 207b 3133 3032 2c20 3731 347d 7d09  }, {1302, 714}}.
-00008d60: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
-00008d70: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-00008d80: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
-00008d90: 0000 0e00 7000 6f00 7300 6500 5f00 6900  ....p.o.s.e._.i.
-00008da0: 6d00 7000 6f00 7200 7400 6500 7200 7364  m.p.o.r.t.e.r.sd
-00008db0: 7363 6c62 6f6f 6c00 0000 000e 0070 006f  sclbool......p.o
-00008dc0: 0073 0065 005f 0069 006d 0070 006f 0072  .s.e._.i.m.p.o.r
-00008dd0: 0074 0065 0072 0073 6c67 3153 636f 6d70  .t.e.r.slg1Scomp
-00008de0: 0000 0000 0003 87aa 7400 6f00 6f00 6c00  ........t.o.o.l.
+00008040: 0b0d 1c48 494a 4b4c 375f 1010 7573 6552  ...HIJKL7_..useR
+00008050: 656c 6174 6976 6544 6174 6573 5f10 0f73  elativeDates_..s
+00008060: 686f 7749 636f 6e50 7265 7669 6577 5763  howIconPreviewWc
+00008070: 6f6c 756d 6e73 5f10 1163 616c 6375 6c61  olumns_..calcula
+00008080: 7465 416c 6c53 697a 6573 5f10 0f73 6372  teAllSizes_..scr
+00008090: 6f6c 6c50 6f73 6974 696f 6e59 5874 6578  ollPositionYXtex
+000080a0: 7453 697a 655f 100f 7363 726f 6c6c 506f  tSize_..scrollPo
+000080b0: 7369 7469 6f6e 585a 736f 7274 436f 6c75  sitionXZsortColu
+000080c0: 6d6e 5869 636f 6e53 697a 655f 1012 7669  mnXiconSize_..vi
+000080d0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+000080e0: 0909 d90e 0f10 1112 1314 1516 1720 252a  ............. %*
+000080f0: 2f34 383d 4258 636f 6d6d 656e 7473 556c  /48=BXcommentsUl
+00008100: 6162 656c 5776 6572 7369 6f6e 5b64 6174  abelWversion[dat
+00008110: 6543 7265 6174 6564 5473 697a 655c 6461  eCreatedTsize\da
+00008120: 7465 4d6f 6469 6669 6564 546b 696e 6454  teModifiedTkindT
+00008130: 6e61 6d65 5e64 6174 654c 6173 744f 7065  name^dateLastOpe
+00008140: 6e65 64d4 1819 1a1b 1c1d 0b1f 5776 6973  ned.........Wvis
+00008150: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+00008160: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
+00008170: 07d4 1819 1a1b 1c22 0b24 0810 6409 1005  .......".$..d...
+00008180: d418 191a 1b1c 270b 2908 104b 0910 06d4  ......'.)..K....
+00008190: 1819 1a1b 1c2c 1c2e 0810 b508 1002 d418  .....,..........
+000081a0: 191a 1b0b 311c 3309 1061 0810 03d4 1819  ....1.3..a......
+000081b0: 1a1b 0b2c 1c37 0908 1001 d418 191a 1b0b  ...,.7..........
+000081c0: 3a0b 3c09 1073 0910 04d4 1819 1a1b 0b3f  :.<..s.........?
+000081d0: 0b41 0911 01c7 0910 00d4 1819 1a1b 1c44  .A.............D
+000081e0: 1c46 0810 c808 1008 0823 0000 0000 0000  .F.......#......
+000081f0: 0000 2340 2800 0000 0000 0023 4000 0000  ..#@(......#@...
+00008200: 0000 0000 5c64 6174 654d 6f64 6966 6965  ....\dateModifie
+00008210: 6423 4030 0000 0000 0000 0008 001d 0030  d#@0...........0
+00008220: 0042 004a 005e 0070 0079 008b 0096 009f  .B.J.^.p.y......
+00008230: 00b4 00b5 00b6 00c9 00d2 00d8 00e0 00ec  ................
+00008240: 00f1 00fe 0103 0108 0117 0120 0128 012e  ........... .(..
+00008250: 0138 013e 013f 0142 0143 0145 014e 014f  .8.>.?.B.C.E.N.O
+00008260: 0151 0152 0154 015d 015e 0160 0161 0163  .Q.R.T.].^.`.a.c
+00008270: 016c 016d 016f 0170 0172 017b 017c 017e  .l.m.o.p.r.{.|.~
+00008280: 017f 0181 018a 018b 018c 018e 0197 0198  ................
+00008290: 019a 019b 019d 01a6 01a7 01aa 01ab 01ad  ................
+000082a0: 01b6 01b7 01b9 01ba 01bc 01bd 01c6 01cf  ................
+000082b0: 01d8 01e5 0000 0000 0000 0201 0000 0000  ................
+000082c0: 0000 004d 0000 0000 0000 0000 0000 0000  ...M............
+000082d0: 0000 01ee 0000 0008 0070 006c 006f 0074  .........p.l.o.t
+000082e0: 0074 0069 006e 0067 6d6f 4444 626c 6f62  .t.i.n.gmoDDblob
+000082f0: 0000 0008 828d b130 e32c c541 0000 0008  .......0.,.A....
+00008300: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
+00008310: 6d6f 6444 626c 6f62 0000 0008 828d b130  modDblob.......0
+00008320: e32c c541 0000 0008 0070 006c 006f 0074  .,.A.....p.l.o.t
+00008330: 0074 0069 006e 0067 7068 3153 636f 6d70  .t.i.n.gph1Scomp
+00008340: 0000 0000 0014 4000 0000 0008 0070 006c  ......@......p.l
+00008350: 006f 0074 0074 0069 006e 0067 7653 726e  .o.t.t.i.n.gvSrn
+00008360: 6c6f 6e67 0000 0001 0000 0013 0070 006f  long.........p.o
+00008370: 0073 0065 005f 0063 006f 006e 0066 0069  .s.e._.c.o.n.f.i
+00008380: 0067 0075 0072 0061 0074 0069 006f 006e  .g.u.r.a.t.i.o.n
+00008390: 0073 6277 7370 626c 6f62 0000 00ca 6270  .sbwspblob....bp
+000083a0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+000083b0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+000083c0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+000083d0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+000083e0: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+000083f0: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00008400: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00008410: 5369 6465 6261 7208 0809 0809 5f10 197b  Sidebar....._..{
+00008420: 7b31 3337 2c20 3134 337d 2c20 7b31 3330  {137, 143}, {130
+00008430: 322c 2037 3134 7d7d 0908 1725 313d 4960  2, 714}}...%1=I`
+00008440: 6d79 7a7b 7c7d 7e9a 0000 0000 0000 0101  myz{|}~.........
+00008450: 0000 0000 0000 000f 0000 0000 0000 0000  ................
+00008460: 0000 0000 0000 009b 0000 0013 0070 006f  .............p.o
+00008470: 0073 0065 005f 0063 006f 006e 0066 0069  .s.e._.c.o.n.f.i
+00008480: 0067 0075 0072 0061 0074 0069 006f 006e  .g.u.r.a.t.i.o.n
+00008490: 0073 6473 636c 626f 6f6c 0000 0000 1300  .sdsclbool......
+000084a0: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
+000084b0: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
+000084c0: 6f00 6e00 736c 6731 5363 6f6d 7000 0000  o.n.slg1Scomp...
+000084d0: 0000 06ae 5600 0000 1300 7000 6f00 7300  ....V.....p.o.s.
+000084e0: 6500 5f00 6300 6f00 6e00 6600 6900 6700  e._.c.o.n.f.i.g.
+000084f0: 7500 7200 6100 7400 6900 6f00 6e00 736c  u.r.a.t.i.o.n.sl
+00008500: 7376 4362 6c6f 6200 0002 b062 706c 6973  svCblob....bplis
+00008510: 7430 30da 0102 0304 0506 0708 090a 0b0c  t00.............
+00008520: 0d18 4849 484a 4b0c 5f10 1276 6965 774f  ..HIHJK._..viewO
+00008530: 7074 696f 6e73 5665 7273 696f 6e5f 100f  ptionsVersion_..
+00008540: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+00008550: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+00008560: 6174 6541 6c6c 5369 7a65 735f 100f 7363  ateAllSizes_..sc
+00008570: 726f 6c6c 506f 7369 7469 6f6e 5958 7465  rollPositionYXte
+00008580: 7874 5369 7a65 5f10 0f73 6372 6f6c 6c50  xtSize_..scrollP
+00008590: 6f73 6974 696f 6e58 5a73 6f72 7443 6f6c  ositionXZsortCol
+000085a0: 756d 6e58 6963 6f6e 5369 7a65 5f10 1075  umnXiconSize_..u
+000085b0: 7365 5265 6c61 7469 7665 4461 7465 7310  seRelativeDates.
+000085c0: 0109 ab0e 171c 2125 2a2f 3439 3e43 d40f  ......!%*/49>C..
+000085d0: 1011 120c 140c 1657 7669 7369 626c 6555  .......WvisibleU
+000085e0: 7769 6474 6859 6173 6365 6e64 696e 675a  widthYascendingZ
+000085f0: 6964 656e 7469 6669 6572 0911 01c7 0954  identifier.....T
+00008600: 6e61 6d65 d40f 1011 1218 1918 1b08 1023  name...........#
+00008610: 0858 7562 6971 7569 7479 d40f 1011 120c  .Xubiquity......
+00008620: 1e18 2009 10b5 085c 6461 7465 4d6f 6469  .. ....\dateModi
+00008630: 6669 6564 d40f 1011 1218 1e18 2408 085b  fied........$..[
+00008640: 6461 7465 4372 6561 7465 64d4 0f10 1112  dateCreated.....
+00008650: 0c27 1829 0910 6108 5473 697a 65d4 0f10  .'.)..a.Tsize...
+00008660: 1112 0c2c 0c2e 0910 7309 546b 696e 64d4  ...,....s.Tkind.
+00008670: 0f10 1112 1831 0c33 0810 6409 556c 6162  .....1.3..d.Ulab
+00008680: 656c d40f 1011 1218 360c 3808 104b 0957  el......6.8..K.W
+00008690: 7665 7273 696f 6ed4 0f10 1112 183b 0c3d  version......;.=
+000086a0: 0811 012c 0958 636f 6d6d 656e 7473 d40f  ...,.Xcomments..
+000086b0: 1011 1218 4018 4208 10c8 085e 6461 7465  ....@.B....^date
+000086c0: 4c61 7374 4f70 656e 6564 d40f 1011 1218  LastOpened......
+000086d0: 1e18 4608 0859 6461 7465 4164 6465 6408  ..F..YdateAdded.
+000086e0: 2300 0000 0000 0000 0023 4028 0000 0000  #........#@(....
+000086f0: 0000 546e 616d 6523 4030 0000 0000 0000  ..Tname#@0......
+00008700: 0900 0800 1d00 3200 4400 4c00 6000 7200  ......2.D.L.`.r.
+00008710: 7b00 8d00 9800 a100 b400 b600 b700 c300  {...............
+00008720: cc00 d400 da00 e400 ef00 f000 f300 f400  ................
+00008730: f901 0201 0301 0501 0601 0f01 1801 1901  ................
+00008740: 1b01 1c01 2901 3201 3301 3401 4001 4901  ....).2.3.4.@.I.
+00008750: 4a01 4c01 4d01 5201 5b01 5c01 5e01 5f01  J.L.M.R.[.\.^._.
+00008760: 6401 6d01 6e01 7001 7101 7701 8001 8101  d.m.n.p.q.w.....
+00008770: 8301 8401 8c01 9501 9601 9901 9a01 a301  ................
+00008780: ac01 ad01 af01 b001 bf01 c801 c901 ca01  ................
+00008790: d401 d501 de01 e701 ec01 f500 0000 0000  ................
+000087a0: 0002 0100 0000 0000 0000 4d00 0000 0000  ..........M.....
+000087b0: 0000 0000 0000 0000 0001 f600 0000 1300  ................
+000087c0: 7000 6f00 7300 6500 5f00 6300 6f00 6e00  p.o.s.e._.c.o.n.
+000087d0: 6600 6900 6700 7500 7200 6100 7400 6900  f.i.g.u.r.a.t.i.
+000087e0: 6f00 6e00 736c 7376 7062 6c6f 6200 0002  o.n.slsvpblob...
+000087f0: 9562 706c 6973 7430 30da 0102 0304 0506  .bplist00.......
+00008800: 0708 090a 0b0c 0d1f 4748 4749 4a0c 5f10  ........GHGIJ._.
+00008810: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+00008820: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
+00008830: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+00008840: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+00008850: 735f 100f 7363 726f 6c6c 506f 7369 7469  s_..scrollPositi
+00008860: 6f6e 5958 7465 7874 5369 7a65 5f10 0f73  onYXtextSize_..s
+00008870: 6372 6f6c 6c50 6f73 6974 696f 6e58 5a73  crollPositionXZs
+00008880: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
+00008890: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
+000088a0: 4461 7465 7310 0109 d90e 0f10 1112 1314  Dates...........
+000088b0: 1516 1720 2529 2d32 373c 4158 636f 6d6d  ... %)-27<AXcomm
+000088c0: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
+000088d0: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
+000088e0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+000088f0: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
+00008900: 7369 6f6e 546e 616d 65d4 1819 1a1b 1c1d  sionTname.......
+00008910: 0c1f 5569 6e64 6578 5577 6964 7468 5961  ..UindexUwidthYa
+00008920: 7363 656e 6469 6e67 5776 6973 6962 6c65  scendingWvisible
+00008930: 1007 1101 2c09 08d4 1819 1a1b 2122 1f1f  ....,.......!"..
+00008940: 1008 10c8 0808 d418 191a 1b0b 261f 0c10  ............&...
+00008950: b508 09d4 1819 1a1b 2a26 1f1f 1002 0808  ........*&......
+00008960: d418 191a 1b2e 2f1f 0c10 0310 6108 09d4  ....../.....a...
+00008970: 1819 1a1b 3334 0c1f 1005 1064 0908 d418  ....34.....d....
+00008980: 191a 1b38 390c 0c10 0410 7309 09d4 1819  ...89.....s.....
+00008990: 1a1b 3d3e 0c1f 1006 104b 0908 d418 191a  ..=>.....K......
+000089a0: 1b42 430c 0c10 0011 01c7 0909 0823 0000  .BC..........#..
+000089b0: 0000 0000 0000 2340 2800 0000 0000 0054  ......#@(......T
+000089c0: 6e61 6d65 2340 3000 0000 0000 0009 0008  name#@0.........
+000089d0: 001d 0032 0044 004c 0060 0072 007b 008d  ...2.D.L.`.r.{..
+000089e0: 0098 00a1 00b4 00b6 00b7 00ca 00d3 00e2  ................
+000089f0: 00ef 00fb 0100 0106 010b 0113 0118 0121  ...............!
+00008a00: 0127 012d 0137 013f 0141 0144 0145 0146  .'.-.7.?.A.D.E.F
+00008a10: 014f 0151 0153 0154 0155 015e 0160 0161  .O.Q.S.T.U.^.`.a
+00008a20: 0162 016b 016d 016e 016f 0178 017a 017c  .b.k.m.n.o.x.z.|
+00008a30: 017d 017e 0187 0189 018b 018c 018d 0196  .}.~............
+00008a40: 0198 019a 019b 019c 01a5 01a7 01a9 01aa  ................
+00008a50: 01ab 01b4 01b6 01b9 01ba 01bb 01bc 01c5  ................
+00008a60: 01ce 01d3 01dc 0000 0000 0000 0201 0000  ................
+00008a70: 0000 0000 004c 0000 0000 0000 0000 0000  .....L..........
+00008a80: 0000 0000 01dd 0000 0013 0070 006f 0073  ...........p.o.s
+00008a90: 0065 005f 0063 006f 006e 0066 0069 0067  .e._.c.o.n.f.i.g
+00008aa0: 0075 0072 0061 0074 0069 006f 006e 0073  .u.r.a.t.i.o.n.s
+00008ab0: 6d6f 4444 626c 6f62 0000 0008 d97e 4b74  moDDblob.....~Kt
+00008ac0: e2dd c441 0000 0013 0070 006f 0073 0065  ...A.....p.o.s.e
+00008ad0: 005f 0063 006f 006e 0066 0069 0067 0075  ._.c.o.n.f.i.g.u
+00008ae0: 0072 0061 0074 0069 006f 006e 0073 6d6f  .r.a.t.i.o.n.smo
+00008af0: 6444 626c 6f62 0000 0008 d97e 4b74 e2dd  dDblob.....~Kt..
+00008b00: c441 0000 0013 0070 006f 0073 0065 005f  .A.....p.o.s.e._
+00008b10: 0063 006f 006e 0066 0069 0067 0075 0072  .c.o.n.f.i.g.u.r
+00008b20: 0061 0074 0069 006f 006e 0073 7068 3153  .a.t.i.o.n.sph1S
+00008b30: 636f 6d70 0000 0000 0007 3000 0000 0013  comp......0.....
+00008b40: 0070 006f 0073 0065 005f 0063 006f 006e  .p.o.s.e._.c.o.n
+00008b50: 0066 0069 0067 0075 0072 0061 0074 0069  .f.i.g.u.r.a.t.i
+00008b60: 006f 006e 0073 7653 726e 6c6f 6e67 0000  .o.n.svSrnlong..
+00008b70: 0001 0000 001b 0070 006f 0073 0065 005f  .......p.o.s.e._
+00008b80: 0063 006f 006e 0066 0069 0067 0075 0072  .c.o.n.f.i.g.u.r
+00008b90: 0061 0074 0069 006f 006e 0073 005f 0061  .a.t.i.o.n.s._.a
+00008ba0: 0072 0063 0068 0069 0076 0065 6c67 3153  .r.c.h.i.v.elg1S
+00008bb0: 636f 6d70 0000 0000 0006 faed 0000 001b  comp............
+00008bc0: 0070 006f 0073 0065 005f 0063 006f 006e  .p.o.s.e._.c.o.n
+00008bd0: 0066 0069 0067 0075 0072 0061 0074 0069  .f.i.g.u.r.a.t.i
+00008be0: 006f 006e 0073 005f 0061 0072 0063 0068  .o.n.s._.a.r.c.h
+00008bf0: 0069 0076 0065 6d6f 4444 626c 6f62 0000  .i.v.emoDDblob..
+00008c00: 0008 8983 1ea9 cbfe c441 0000 001b 0070  .........A.....p
+00008c10: 006f 0073 0065 005f 0063 006f 006e 0066  .o.s.e._.c.o.n.f
+00008c20: 0069 0067 0075 0072 0061 0074 0069 006f  .i.g.u.r.a.t.i.o
+00008c30: 006e 0073 005f 0061 0072 0063 0068 0069  .n.s._.a.r.c.h.i
+00008c40: 0076 0065 6d6f 6444 626c 6f62 0000 0008  .v.emodDblob....
+00008c50: 8983 1ea9 cbfe c441 0000 001b 0070 006f  .......A.....p.o
+00008c60: 0073 0065 005f 0063 006f 006e 0066 0069  .s.e._.c.o.n.f.i
+00008c70: 0067 0075 0072 0061 0074 0069 006f 006e  .g.u.r.a.t.i.o.n
+00008c80: 0073 005f 0061 0072 0063 0068 0069 0076  .s._.a.r.c.h.i.v
+00008c90: 0065 7068 3153 636f 6d70 0000 0000 0007  .eph1Scomp......
+00008ca0: 9000 0000 000e 0070 006f 0073 0065 005f  .......p.o.s.e._
+00008cb0: 0069 006d 0070 006f 0072 0074 0065 0072  .i.m.p.o.r.t.e.r
+00008cc0: 0073 6277 7370 626c 6f62 0000 00c9 6270  .sbwspblob....bp
+00008cd0: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+00008ce0: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00008cf0: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+00008d00: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00008d10: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00008d20: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00008d30: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00008d40: 5369 6465 6261 7208 0809 0809 5f10 187b  Sidebar....._..{
+00008d50: 7b33 362c 2031 3331 7d2c 207b 3133 3032  {36, 131}, {1302
+00008d60: 2c20 3731 347d 7d09 0817 2531 3d49 606d  , 714}}...%1=I`m
+00008d70: 797a 7b7c 7d7e 9900 0000 0000 0001 0100  yz{|}~..........
+00008d80: 0000 0000 0000 0f00 0000 0000 0000 0000  ................
+00008d90: 0000 0000 0000 9a00 0000 0e00 7000 6f00  ............p.o.
+00008da0: 7300 6500 5f00 6900 6d00 7000 6f00 7200  s.e._.i.m.p.o.r.
+00008db0: 7400 6500 7200 7364 7363 6c62 6f6f 6c00  t.e.r.sdsclbool.
+00008dc0: 0000 000e 0070 006f 0073 0065 005f 0069  .....p.o.s.e._.i
+00008dd0: 006d 0070 006f 0072 0074 0065 0072 0073  .m.p.o.r.t.e.r.s
+00008de0: 6c67 3153 636f 6d70 0000 0000 0003 87aa  lg1Scomp........
 00008df0: 736d 6f44 4462 6c6f 6200 0000 08aa 2e11  smoDDblob.......
 00008e00: 6564 14c5 4100 0000 0d00 6f00 7500 7400  ed..A.....o.u.t.
 00008e10: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00008e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08aa  l.smodDblob.....
 00008e30: 2e11 6564 14c5 4100 0000 0d00 6f00 7500  ..ed..A.....o.u.
 00008e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
 00008e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
@@ -2284,21 +2284,21 @@
 00008eb0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
 00008ec0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
 00008ed0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
 00008ee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
 00008ef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
 00008f00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
 00008f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
-00008f20: 197b 7b37 3035 2c20 3230 377d 2c20 7b31  .{{705, 207}, {1
-00008f30: 3234 372c 2035 3638 7d7d 0908 1523 2f3b  247, 568}}...#/;
+00008f20: 197b 7b32 3630 2c20 3132 397d 2c20 7b31  .{{260, 129}, {1
+00008f30: 3138 302c 2036 3336 7d7d 0908 1523 2f3b  180, 636}}...#/;
 00008f40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
 00008f50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 00008f60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
 00008f70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
-00008f80: 636f 6d70 0000 0000 000f f490 0000 0000  comp............
+00008f80: 636f 6d70 0000 0000 0010 0215 0000 0000  comp............
 00008f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -2470,91 +2470,91 @@
 00009a50: 6f00 7300 6500 5f00 7000 7200 6f00 6300  o.s.e._.p.r.o.c.
 00009a60: 6500 7300 7300 6f00 7200 7370 6831 5363  e.s.s.o.r.sph1Sc
 00009a70: 6f6d 7000 0000 0000 01e0 0000 0000 0f00  omp.............
 00009a80: 7000 6f00 7300 6500 5f00 7000 7200 6f00  p.o.s.e._.p.r.o.
 00009a90: 6300 6500 7300 7300 6f00 7200 7376 5372  c.e.s.s.o.r.svSr
 00009aa0: 6e6c 6f6e 6700 0000 0100 0000 0900 7200  nlong.........r.
 00009ab0: 6f00 6900 5f00 7400 6f00 6f00 6c00 7362  o.i._.t.o.o.l.sb
-00009ac0: 7773 7062 6c6f 6200 0000 ca62 706c 6973  wspblob....bplis
-00009ad0: 7430 30d7 0102 0304 0506 0708 080a 080a  t00.............
-00009ae0: 0d0a 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-00009af0: 5b53 686f 7750 6174 6862 6172 5b53 686f  [ShowPathbar[Sho
-00009b00: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
-00009b10: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
-00009b20: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
-00009b30: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
-00009b40: 6562 6172 0808 0908 095f 1019 7b7b 3233  ebar....._..{{23
-00009b50: 322c 2031 3931 7d2c 207b 3133 3032 2c20  2, 191}, {1302, 
-00009b60: 3731 347d 7d09 0817 2531 3d49 606d 797a  714}}...%1=I`myz
-00009b70: 7b7c 7d7e 9a00 0000 0000 0001 0100 0000  {|}~............
-00009b80: 0000 0000 0f00 0000 0000 0000 0000 0000  ................
-00009b90: 0000 0000 9b00 0000 0900 7200 6f00 6900  ..........r.o.i.
-00009ba0: 5f00 7400 6f00 6f00 6c00 736c 6731 5363  _.t.o.o.l.slg1Sc
-00009bb0: 6f6d 7000 0000 0000 079c b900 0000 0900  omp.............
-00009bc0: 7200 6f00 6900 5f00 7400 6f00 6f00 6c00  r.o.i._.t.o.o.l.
-00009bd0: 736c 7376 4362 6c6f 6200 0002 7962 706c  slsvCblob...ybpl
-00009be0: 6973 7430 30d8 0102 0304 0506 0708 090a  ist00...........
-00009bf0: 0b16 4647 480a 5f10 1276 6965 774f 7074  ..FGH._..viewOpt
-00009c00: 696f 6e73 5665 7273 696f 6e5f 100f 7368  ionsVersion_..sh
-00009c10: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00009c20: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00009c30: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-00009c40: 7a65 5a73 6f72 7443 6f6c 756d 6e58 6963  zeZsortColumnXic
-00009c50: 6f6e 5369 7a65 5f10 1075 7365 5265 6c61  onSize_..useRela
-00009c60: 7469 7665 4461 7465 7310 0109 ab0c 151a  tiveDates.......
-00009c70: 1f23 282d 3237 3c41 d40d 0e0f 100a 120a  .#(-27<A........
-00009c80: 1457 7669 7369 626c 6555 7769 6474 6859  .WvisibleUwidthY
-00009c90: 6173 6365 6e64 696e 675a 6964 656e 7469  ascendingZidenti
-00009ca0: 6669 6572 0911 01c7 0954 6e61 6d65 d40d  fier.....Tname..
-00009cb0: 0e0f 1016 1716 1908 1023 0858 7562 6971  .........#.Xubiq
-00009cc0: 7569 7479 d40d 0e0f 100a 1c16 1e09 10b5  uity............
-00009cd0: 085c 6461 7465 4d6f 6469 6669 6564 d40d  .\dateModified..
-00009ce0: 0e0f 1016 1c16 2208 085b 6461 7465 4372  ......"..[dateCr
-00009cf0: 6561 7465 64d4 0d0e 0f10 0a25 1627 0910  eated......%.'..
-00009d00: 6108 5473 697a 65d4 0d0e 0f10 0a2a 0a2c  a.Tsize......*.,
-00009d10: 0910 7309 546b 696e 64d4 0d0e 0f10 162f  ..s.Tkind....../
-00009d20: 0a31 0810 6409 556c 6162 656c d40d 0e0f  .1..d.Ulabel....
-00009d30: 1016 340a 3608 104b 0957 7665 7273 696f  ..4.6..K.Wversio
-00009d40: 6ed4 0d0e 0f10 1639 0a3b 0811 012c 0958  n......9.;...,.X
-00009d50: 636f 6d6d 656e 7473 d40d 0e0f 1016 3e16  comments......>.
-00009d60: 4008 10c8 085e 6461 7465 4c61 7374 4f70  @....^dateLastOp
-00009d70: 656e 6564 d40d 0e0f 1016 1c16 4408 0859  ened........D..Y
-00009d80: 6461 7465 4164 6465 6408 2340 2800 0000  dateAdded.#@(...
-00009d90: 0000 0054 6e61 6d65 2340 3000 0000 0000  ...Tname#@0.....
-00009da0: 0009 0008 0019 002e 0040 0048 005c 0065  .........@.H.\.e
-00009db0: 0070 0079 008c 008e 008f 009b 00a4 00ac  .p.y............
-00009dc0: 00b2 00bc 00c7 00c8 00cb 00cc 00d1 00da  ................
-00009dd0: 00db 00dd 00de 00e7 00f0 00f1 00f3 00f4  ................
-00009de0: 0101 010a 010b 010c 0118 0121 0122 0124  ...........!.".$
-00009df0: 0125 012a 0133 0134 0136 0137 013c 0145  .%.*.3.4.6.7.<.E
-00009e00: 0146 0148 0149 014f 0158 0159 015b 015c  .F.H.I.O.X.Y.[.\
-00009e10: 0164 016d 016e 0171 0172 017b 0184 0185  .d.m.n.q.r.{....
-00009e20: 0187 0188 0197 01a0 01a1 01a2 01ac 01ad  ................
-00009e30: 01b6 01bb 01c4 0000 0000 0000 0201 0000  ................
-00009e40: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
-00009e50: 0000 0000 01c5 6831 5363 6f6d 7000 0000  ......h1Scomp...
-00009e60: 0000 0210 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
-00009e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
-00009e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
-00009e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
-00009ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b962  n.gbwspblob....b
-00009eb0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
-00009ec0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
-00009ed0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
+00009ac0: 7773 7062 6c6f 6200 0000 b962 706c 6973  wspblob....bplis
+00009ad0: 7430 30d6 0102 0304 0506 0708 0708 0b08  t00.............
+00009ae0: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
+00009af0: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
+00009b00: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
+00009b10: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
+00009b20: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
+00009b30: 6964 6562 6172 0809 0809 5f10 197b 7b32  idebar...._..{{2
+00009b40: 3630 2c20 3132 397d 2c20 7b31 3138 302c  60, 129}, {1180,
+00009b50: 2036 3336 7d7d 0908 1523 2f3b 525f 6b6c   636}}...#/;R_kl
+00009b60: 6d6e 6f8b 0000 0000 0000 0101 0000 0000  mno.............
+00009b70: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00009b80: 0000 008c 0000 0009 0072 006f 0069 005f  .........r.o.i._
+00009b90: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
+00009ba0: 6d70 0000 0000 0007 9cb9 0000 0009 0072  mp.............r
+00009bb0: 006f 0069 005f 0074 006f 006f 006c 0073  .o.i._.t.o.o.l.s
+00009bc0: 6c73 7643 626c 6f62 0000 030f 6270 6c69  lsvCblob....bpli
+00009bd0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
+00009be0: 1656 570a 5958 6963 6f6e 5369 7a65 5f10  .VW.YXiconSize_.
+00009bf0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00009c00: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00009c10: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
+00009c20: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
+00009c30: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00009c40: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
+00009c50: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
+00009c60: 0009 ae0c 151a 1f23 282d 3237 3c41 454d  .......#(-27<AEM
+00009c70: 51d4 0d0e 0f10 0a12 0a14 5776 6973 6962  Q.........Wvisib
+00009c80: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00009c90: 6e67 5a69 6465 6e74 6966 6965 7209 1101  ngZidentifier...
+00009ca0: c709 546e 616d 65d4 0d0e 0f10 1617 1619  ..Tname.........
+00009cb0: 0810 2308 5875 6269 7175 6974 79d4 0d0e  ..#.Xubiquity...
+00009cc0: 0f10 0a1c 161e 0910 b508 5c64 6174 654d  ..........\dateM
+00009cd0: 6f64 6966 6965 64d4 0d0e 0f10 161c 1622  odified........"
+00009ce0: 0808 5b64 6174 6543 7265 6174 6564 d40d  ..[dateCreated..
+00009cf0: 0e0f 100a 2516 2709 1061 0854 7369 7a65  ....%.'..a.Tsize
+00009d00: d40d 0e0f 100a 2a0a 2c09 1073 0954 6b69  ......*.,..s.Tki
+00009d10: 6e64 d40d 0e0f 1016 2f0a 3108 1064 0955  nd....../.1..d.U
+00009d20: 6c61 6265 6cd4 0d0e 0f10 1634 0a36 0810  label......4.6..
+00009d30: 4b09 5776 6572 7369 6f6e d40d 0e0f 1016  K.Wversion......
+00009d40: 390a 3b08 1101 2c09 5863 6f6d 6d65 6e74  9.;...,.Xcomment
+00009d50: 73d4 0d0e 0f10 163e 1640 0810 c808 5e64  s......>.@....^d
+00009d60: 6174 654c 6173 744f 7065 6e65 64d4 0d0e  ateLastOpened...
+00009d70: 0f10 161c 1644 0808 5964 6174 6541 6464  .....D..YdateAdd
+00009d80: 6564 d446 4748 1016 4a16 4c57 7669 7369  ed.FGH..J.LWvisi
+00009d90: 626c 6555 7769 6474 6859 6173 6365 6e64  bleUwidthYascend
+00009da0: 696e 6708 10d2 085a 7368 6172 654f 776e  ing....ZshareOwn
+00009db0: 6572 d446 4748 1016 4a16 5008 085f 100f  er.FGH..J.P.._..
+00009dc0: 7368 6172 654c 6173 7445 6469 746f 72d4  shareLastEditor.
+00009dd0: 4647 4810 164a 1654 0808 5f10 1069 6e76  FGH..J.T.._..inv
+00009de0: 6974 6174 696f 6e53 7461 7475 7308 2340  itationStatus.#@
+00009df0: 2800 0000 0000 005c 6461 7465 4d6f 6469  (......\dateModi
+00009e00: 6669 6564 0910 0100 0800 1900 2200 3400  fied........".4.
+00009e10: 3c00 5000 5900 6400 7700 8c00 9500 9600  <.P.Y.d.w.......
+00009e20: a500 ae00 b600 bc00 c600 d100 d200 d500  ................
+00009e30: d600 db00 e400 e500 e700 e800 f100 fa00  ................
+00009e40: fb00 fd00 fe01 0b01 1401 1501 1601 2201  ..............".
+00009e50: 2b01 2c01 2e01 2f01 3401 3d01 3e01 4001  +.,.../.4.=.>.@.
+00009e60: 4101 4601 4f01 5001 5201 5301 5901 6201  A.F.O.P.R.S.Y.b.
+00009e70: 6301 6501 6601 6e01 7701 7801 7b01 7c01  c.e.f.n.w.x.{.|.
+00009e80: 8501 8e01 8f01 9101 9201 a101 aa01 ab01  ................
+00009e90: ac01 b601 bf01 c701 cd01 d701 d801 da01  ................
+00009ea0: db01 e601 ef01 f001 f102 0302 0c02 0d02  ................
+00009eb0: 0e02 2102 2202 2b02 3802 3900 0000 0000  ..!.".+.8.9.....
+00009ec0: 0002 0100 0000 0000 0000 5a00 0000 0000  ..........Z.....
+00009ed0: 0000 0000 0000 0000 0002 3b62 6172 5b53  ..........;bar[S
 00009ee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
 00009ef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
 00009f00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
 00009f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
-00009f20: 197b 7b37 3035 2c20 3230 377d 2c20 7b31  .{{705, 207}, {1
-00009f30: 3234 372c 2035 3638 7d7d 0908 1523 2f3b  247, 568}}...#/;
+00009f20: 197b 7b32 3630 2c20 3132 397d 2c20 7b31  .{{260, 129}, {1
+00009f30: 3138 302c 2036 3336 7d7d 0908 1523 2f3b  180, 636}}...#/;
 00009f40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
 00009f50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
 00009f60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
 00009f70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
-00009f80: 636f 6d70 0000 0000 000f f490 0000 0000  comp............
+00009f80: 636f 6d70 0000 0000 0010 0215 0000 0000  comp............
 00009f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -2699,375 +2699,375 @@
 0000a8a0: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
 0000a8b0: 0530 0000 0000 1b00 7400 6800 6900 7200  .0......t.h.i.r.
 0000a8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
 0000a8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
 0000a8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
 0000a8f0: 6e6c 6f6e 6700 0000 0100 0000 1000 7400  nlong.........t.
 0000a900: 6800 7200 6500 6500 5f00 6400 6900 6d00  h.r.e.e._.d.i.m.
-0000a910: 6500 6e00 7300 6900 6f00 6e00 736c 6731  e.n.s.i.o.n.slg1
-0000a920: 5363 6f6d 7000 0000 0000 033c cc00 0000  Scomp......<....
-0000a930: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
-0000a940: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
-0000a950: 736d 6f44 4462 6c6f 6200 0000 08f6 8857  smoDDblob......W
-0000a960: d65e 24c5 4100 0000 1000 7400 6800 7200  .^$.A.....t.h.r.
-0000a970: 6500 6500 5f00 6400 6900 6d00 6500 6e00  e.e._.d.i.m.e.n.
-0000a980: 7300 6900 6f00 6e00 736d 6f64 4462 6c6f  s.i.o.n.smodDblo
-0000a990: 6200 0000 08f6 8857 d65e 24c5 4100 0000  b......W.^$.A...
-0000a9a0: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
-0000a9b0: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
-0000a9c0: 7370 6831 5363 6f6d 7000 0000 0000 03a0  sph1Scomp.......
-0000a9d0: 0000 0000 0200 7500 6962 7773 7062 6c6f  ......u.ibwspblo
-0000a9e0: 6200 0000 ca62 706c 6973 7430 30d7 0102  b....bplist00...
-0000a9f0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
-0000aa00: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
-0000aa10: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
-0000aa20: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-0000aa30: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-0000aa40: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-0000aa50: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-0000aa60: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
-0000aa70: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
-0000aa80: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
-0000aa90: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-0000aaa0: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
-0000aab0: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
-0000aac0: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000aad0: 0000 0000 0012 10b6 0000 0002 0075 0069  .............u.i
-0000aae0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
-0000aaf0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-0000ab00: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
-0000ab10: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-0000ab20: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-0000ab30: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-0000ab40: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
-0000ab50: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
-0000ab60: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
-0000ab70: 6976 6544 6174 6573 1001 09ab 0c15 1a1f  iveDates........
-0000ab80: 2328 2d32 373c 41d4 0d0e 0f10 0a12 0a14  #(-27<A.........
-0000ab90: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-0000aba0: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
-0000abb0: 6965 7209 1101 c709 546e 616d 65d4 100e  ier.....Tname...
-0000abc0: 0f0d 1617 1818 5875 6269 7175 6974 7910  ......Xubiquity.
-0000abd0: 2308 08d4 100f 0e0d 1b18 1d0a 5c64 6174  #...........\dat
-0000abe0: 654d 6f64 6966 6965 6408 10b5 09d4 100f  eModified.......
-0000abf0: 0e0d 2018 1d18 5b64 6174 6543 7265 6174  .. ...[dateCreat
-0000ac00: 6564 0808 d410 0f0e 0d24 1826 0a54 7369  ed.......$.&.Tsi
-0000ac10: 7a65 0810 6109 d410 0f0e 0d29 0a2b 0a54  ze..a......).+.T
-0000ac20: 6b69 6e64 0910 7309 d410 0f0e 0d2e 0a30  kind..s........0
-0000ac30: 1855 6c61 6265 6c09 1064 08d4 100f 0e0d  .Ulabel..d......
-0000ac40: 330a 3518 5776 6572 7369 6f6e 0910 4b08  3.5.Wversion..K.
-0000ac50: d410 0f0e 0d38 0a3a 1858 636f 6d6d 656e  .....8.:.Xcommen
-0000ac60: 7473 0911 012c 08d4 100f 0e0d 3d18 3f18  ts...,......=.?.
-0000ac70: 5e64 6174 654c 6173 744f 7065 6e65 6408  ^dateLastOpened.
-0000ac80: 10c8 08d4 100e 0f0d 421d 1818 5964 6174  ........B...Ydat
-0000ac90: 6541 6464 6564 0808 0823 4028 0000 0000  eAdded...#@(....
-0000aca0: 0000 546e 616d 6523 4030 0000 0000 0000  ..Tname#@0......
-0000acb0: 0900 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-0000acc0: 7000 7900 8c00 8e00 8f00 9b00 a400 ac00  p.y.............
-0000acd0: b200 bc00 c700 c800 cb00 cc00 d100 da00  ................
-0000ace0: e300 e500 e600 e700 f000 fd00 fe01 0001  ................
-0000acf0: 0101 0a01 1601 1701 1801 2101 2601 2701  ..........!.&.'.
-0000ad00: 2901 2a01 3301 3801 3901 3b01 3c01 4501  ).*.3.8.9.;.<.E.
-0000ad10: 4b01 4c01 4e01 4f01 5801 6001 6101 6301  K.L.N.O.X.`.a.c.
-0000ad20: 6401 6d01 7601 7701 7a01 7b01 8401 9301  d.m.v.w.z.{.....
-0000ad30: 9401 9601 9701 a001 aa01 ab01 ac01 ad01  ................
-0000ad40: b601 bb01 c400 0000 0000 0002 0100 0000  ................
-0000ad50: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
-0000ad60: 0000 0001 c500 0000 0200 7500 696c 7376  ..........u.ilsv
-0000ad70: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
-0000ad80: 30d8 0102 0304 0506 0708 090a 0b1a 4546  0.............EF
-0000ad90: 470a 5f10 1276 6965 774f 7074 696f 6e73  G._..viewOptions
-0000ada0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-0000adb0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-0000adc0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-0000add0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-0000ade0: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-0000adf0: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-0000ae00: 4461 7465 7310 0109 d90c 0d0e 0f10 1112  Dates...........
-0000ae10: 1314 151e 2327 2b30 353a 3f58 636f 6d6d  ....#'+05:?Xcomm
-0000ae20: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-0000ae30: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-0000ae40: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-0000ae50: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-0000ae60: 7369 6f6e 546e 616d 65d4 1617 1819 1a0a  sionTname.......
-0000ae70: 1c1d 5776 6973 6962 6c65 5961 7363 656e  ..WvisibleYascen
-0000ae80: 6469 6e67 5577 6964 7468 5569 6e64 6578  dingUwidthUindex
-0000ae90: 0809 1101 2c10 07d4 1617 1819 1a1a 2122  ....,.........!"
-0000aea0: 0808 10c8 1008 d416 1718 190a 1a26 0909  .............&..
-0000aeb0: 0810 b5d4 1617 1819 1a1a 262a 0808 1002  ..........&*....
-0000aec0: d416 1718 190a 1a2e 2f09 0810 6110 03d4  ......../...a...
-0000aed0: 1617 1819 1a0a 3334 0809 1064 1005 d416  ......34...d....
-0000aee0: 1718 190a 0a38 3909 0910 7310 04d4 1617  .....89...s.....
-0000aef0: 1819 1a0a 3d3e 0809 104b 1006 d419 1817  ....=>...K......
-0000af00: 1640 410a 0a10 0011 01c7 0909 0823 4028  .@A..........#@(
-0000af10: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
-0000af20: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
-0000af30: 5c00 6500 7000 7900 8c00 8e00 8f00 a200  \.e.p.y.........
-0000af40: ab00 ba00 c700 d300 d800 de00 e300 eb00  ................
-0000af50: f000 f901 0101 0b01 1101 1701 1801 1901  ................
-0000af60: 1c01 1e01 2701 2801 2901 2b01 2d01 3601  ....'.(.).+.-.6.
-0000af70: 3701 3801 3a01 4301 4401 4501 4701 5001  7.8.:.C.D.E.G.P.
-0000af80: 5101 5201 5401 5601 5f01 6001 6101 6301  Q.R.T.V._.`.a.c.
-0000af90: 6501 6e01 6f01 7001 7201 7401 7d01 7e01  e.n.o.p.r.t.}.~.
-0000afa0: 7f01 8101 8301 8c01 8e01 9101 9201 9301  ................
-0000afb0: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
-0000afc0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-0000afd0: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
-0000afe0: 6f44 4462 6c6f 6200 0000 087e abce 1cd0  oDDblob....~....
-0000aff0: 1fc5 4100 0000 0000 0000 0000 0000 0000  ..A.............
-0000b000: 0000 0000 0000 0000 0000 000c 0000 0002  ................
-0000b010: 0075 0069 7068 3153 636f 6d70 0000 0000  .u.iph1Scomp....
-0000b020: 0018 4000 0000 0002 0075 0069 7653 726e  ..@......u.ivSrn
-0000b030: 6c6f 6e67 0000 0001 0000 000c 0075 006e  long.........u.n
-0000b040: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
-0000b050: 0065 0064 6277 7370 626c 6f62 0000 00ca  .e.dbwspblob....
-0000b060: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
-0000b070: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
-0000b080: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
-0000b090: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-0000b0a0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-0000b0b0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-0000b0c0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-0000b0d0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-0000b0e0: 197b 7b33 3534 2c20 3132 347d 2c20 7b31  .{{354, 124}, {1
-0000b0f0: 3037 362c 2036 3231 7d7d 0908 1725 313d  076, 621}}...%1=
-0000b100: 4960 6d79 7a7b 7c7d 7e9a 0000 0000 0000  I`myz{|}~.......
-0000b110: 0101 0000 0000 0000 000f 0000 0000 0000  ................
-0000b120: 0000 0000 0000 0000 009b 0000 000c 0075  ...............u
-0000b130: 006e 0073 0075 0070 0065 0072 0076 0069  .n.s.u.p.e.r.v.i
-0000b140: 0073 0065 0064 6473 636c 626f 6f6c 0000  .s.e.ddsclbool..
-0000b150: 0000 0c00 7500 6e00 7300 7500 7000 6500  ....u.n.s.u.p.e.
-0000b160: 7200 7600 6900 7300 6500 646c 6731 5363  r.v.i.s.e.dlg1Sc
-0000b170: 6f6d 7000 0000 0000 03e8 6900 0000 0c00  omp.......i.....
-0000b180: 7500 6e00 7300 7500 7000 6500 7200 7600  u.n.s.u.p.e.r.v.
-0000b190: 6900 7300 6500 646c 7376 4362 6c6f 6200  i.s.e.dlsvCblob.
-0000b1a0: 0002 8162 706c 6973 7430 30d8 0102 0304  ...bplist00.....
-0000b1b0: 0506 0708 090a 0b18 4647 0a49 5869 636f  ........FG.IXico
-0000b1c0: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
-0000b1d0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-0000b1e0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-0000b1f0: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
-0000b200: 7443 6f6c 756d 6e5f 1010 7573 6552 656c  tColumn_..useRel
-0000b210: 6174 6976 6544 6174 6573 5f10 1276 6965  ativeDates_..vie
-0000b220: 774f 7074 696f 6e73 5665 7273 696f 6e23  wOptionsVersion#
-0000b230: 4030 0000 0000 0000 09ab 0c15 1a1f 2328  @0............#(
-0000b240: 2d32 373c 41d4 0d0e 0f10 1112 0a0a 5a69  -27<A.........Zi
-0000b250: 6465 6e74 6966 6965 7255 7769 6474 6859  dentifierUwidthY
-0000b260: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
-0000b270: 6554 6e61 6d65 1101 c709 09d4 0d0e 0f10  eTname..........
-0000b280: 1617 1818 5875 6269 7175 6974 7910 2308  ....Xubiquity.#.
-0000b290: 08d4 100e 0f0d 0a1c 0a1e 0910 b509 5c64  ..............\d
-0000b2a0: 6174 654d 6f64 6966 6965 64d4 0d0e 0f10  ateModified.....
-0000b2b0: 201c 1818 5b64 6174 6543 7265 6174 6564   ...[dateCreated
-0000b2c0: 0808 d40d 0e0f 1024 2518 0a54 7369 7a65  .......$%..Tsize
-0000b2d0: 1061 0809 d40d 0e0f 1029 2a0a 0a54 6b69  .a.......)*..Tki
-0000b2e0: 6e64 1073 0909 d40d 0e0f 102e 2f0a 1855  nd.s......../..U
-0000b2f0: 6c61 6265 6c10 6409 08d4 0d0e 0f10 3334  label.d.......34
-0000b300: 0a18 5776 6572 7369 6f6e 104b 0908 d40d  ..Wversion.K....
-0000b310: 0e0f 1038 390a 1858 636f 6d6d 656e 7473  ...89..Xcomments
-0000b320: 1101 2c09 08d4 0d0e 0f10 3d3e 1818 5e64  ..,.......=>..^d
-0000b330: 6174 654c 6173 744f 7065 6e65 6410 c808  ateLastOpened...
-0000b340: 08d4 0d0e 0f10 421c 1818 5964 6174 6541  ......B...YdateA
-0000b350: 6464 6564 0808 0823 4028 0000 0000 0000  dded...#@(......
-0000b360: 5c64 6174 654d 6f64 6966 6965 6409 1001  \dateModified...
-0000b370: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
-0000b380: 0077 008c 0095 0096 00a2 00ab 00b6 00bc  .w..............
-0000b390: 00c6 00ce 00d3 00d6 00d7 00d8 00e1 00ea  ................
-0000b3a0: 00ec 00ed 00ee 00f7 00f8 00fa 00fb 0108  ................
-0000b3b0: 0111 011d 011e 011f 0128 012d 012f 0130  .........(.-./.0
-0000b3c0: 0131 013a 013f 0141 0142 0143 014c 0152  .1.:.?.A.B.C.L.R
-0000b3d0: 0154 0155 0156 015f 0167 0169 016a 016b  .T.U.V._.g.i.j.k
-0000b3e0: 0174 017d 0180 0181 0182 018b 019a 019c  .t.}............
-0000b3f0: 019d 019e 01a7 01b1 01b2 01b3 01b4 01bd  ................
-0000b400: 01ca 01cb 0000 0000 0000 0201 0000 0000  ................
-0000b410: 0000 004a 0000 0000 0000 0000 0000 0000  ...J............
-0000b420: 0000 01cd 0000 000c 0075 006e 0073 0075  .........u.n.s.u
-0000b430: 0070 0065 0072 0076 0069 0073 0065 0064  .p.e.r.v.i.s.e.d
-0000b440: 6c73 7670 626c 6f62 0000 0266 6270 6c69  lsvpblob...fbpli
-0000b450: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-0000b460: 1a46 470a 2458 6963 6f6e 5369 7a65 5f10  .FG.$XiconSize_.
-0000b470: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-0000b480: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-0000b490: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-0000b4a0: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-0000b4b0: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-0000b4c0: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-0000b4d0: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-0000b4e0: 0009 d90c 0d0e 0f10 1112 1314 151e 2328  ..............#(
-0000b4f0: 2c31 363b 4058 636f 6d6d 656e 7473 5e64  ,16;@Xcomments^d
-0000b500: 6174 654c 6173 744f 7065 6e65 645c 6461  ateLastOpened\da
-0000b510: 7465 4d6f 6469 6669 6564 5b64 6174 6543  teModified[dateC
-0000b520: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-0000b530: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-0000b540: 616d 65d4 1617 1819 1a1b 0a1d 5776 6973  ame.........Wvis
-0000b550: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
-0000b560: 6469 6e67 5569 6e64 6578 0811 012c 0910  dingUindex...,..
-0000b570: 07d4 1617 1819 1a20 1a22 0810 c808 1008  ....... ."......
-0000b580: d419 1718 1624 250a 0a10 0110 b509 09d4  .....$%.........
-0000b590: 1617 1819 1a25 1a2b 0808 1002 d416 1718  .....%.+........
-0000b5a0: 190a 2e1a 3009 1061 0810 03d4 1617 1819  ....0..a........
-0000b5b0: 1a33 0a35 0810 6409 1005 d416 1718 190a  .3.5..d.........
-0000b5c0: 380a 3a09 1073 0910 04d4 1617 1819 1a3d  8.:..s.........=
-0000b5d0: 0a3f 0810 4b09 1006 d416 1718 190a 420a  .?..K.........B.
-0000b5e0: 4409 1101 c709 1000 0823 4028 0000 0000  D........#@(....
-0000b5f0: 0000 5c64 6174 654d 6f64 6966 6965 6409  ..\dateModified.
-0000b600: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
-0000b610: 0077 008c 0095 0096 00a9 00b2 00c1 00ce  .w..............
-0000b620: 00da 00df 00e5 00ea 00f2 00f7 0100 0108  ................
-0000b630: 010e 0118 011e 011f 0122 0123 0125 012e  .........".#.%..
-0000b640: 012f 0131 0132 0134 013d 013f 0141 0142  ./.1.2.4.=.?.A.B
-0000b650: 0143 014c 014d 014e 0150 0159 015a 015c  .C.L.M.N.P.Y.Z.\
-0000b660: 015d 015f 0168 0169 016b 016c 016e 0177  .]._.h.i.k.l.n.w
-0000b670: 0178 017a 017b 017d 0186 0187 0189 018a  .x.z.{.}........
-0000b680: 018c 0195 0196 0199 019a 019c 019d 01a6  ................
-0000b690: 01b3 0000 0000 0000 0201 0000 0000 0000  ................
-0000b6a0: 0049 0000 0000 0000 0000 0000 0000 0000  .I..............
-0000b6b0: 01b4 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
-0000b6c0: 0065 0072 0076 0069 0073 0065 0064 6d6f  .e.r.v.i.s.e.dmo
-0000b6d0: 4444 626c 6f62 0000 0008 cbf3 6409 d917  DDblob......d...
-0000b6e0: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
-0000b6f0: 0065 0072 0076 0069 0073 0065 0064 6d6f  .e.r.v.i.s.e.dmo
-0000b700: 6444 626c 6f62 0000 0008 cbf3 6409 d917  dDblob......d...
-0000b710: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
-0000b720: 0065 0072 0076 0069 0073 0065 0064 7068  .e.r.v.i.s.e.dph
-0000b730: 3153 636f 6d70 0000 0000 0004 d000 0000  1Scomp..........
-0000b740: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
-0000b750: 0076 0069 0073 0065 0064 7653 726e 6c6f  .v.i.s.e.dvSrnlo
-0000b760: 6e67 0000 0001 0000 0005 0075 0074 0069  ng.........u.t.i
-0000b770: 006c 0073 6277 7370 626c 6f62 0000 00b9  .l.sbwspblob....
-0000b780: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
-0000b790: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
-0000b7a0: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
-0000b7b0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-0000b7c0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-0000b7d0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-0000b7e0: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-0000b7f0: 1019 7b7b 3730 352c 2032 3037 7d2c 207b  ..{{705, 207}, {
-0000b800: 3132 3437 2c20 3536 387d 7d09 0815 232f  1247, 568}}...#/
-0000b810: 3b52 5f6b 6c6d 6e6f 8b00 0000 0000 0001  ;R_klmno........
-0000b820: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
-0000b830: 0000 0000 0000 0000 8c00 6100 6200 6500  ..........a.b.e.
-0000b840: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
-0000b850: 6500 7200 736d 6f64 4462 6c6f 6200 0000  e.r.smodDblob...
-0000b860: 086b 121b 34c6 1fc5 4100 0000 1b00 7400  .k..4...A.....t.
-0000b870: 6800 6900 7200 6400 5f00 7000 6100 7200  h.i.r.d._.p.a.r.
-0000b880: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
-0000b890: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
-0000b8a0: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
-0000b8b0: 0530 0000 0000 1b00 7400 6800 6900 7200  .0......t.h.i.r.
-0000b8c0: 6400 5f00 7000 6100 7200 7400 7900 5f00  d._.p.a.r.t.y._.
-0000b8d0: 6c00 6100 6200 6500 6c00 5f00 6100 7000  l.a.b.e.l._.a.p.
-0000b8e0: 7000 6500 6e00 6400 6500 7200 7376 5372  p.e.n.d.e.r.svSr
-0000b8f0: 6e6c 6f6e 6700 0000 0100 0000 1000 7400  nlong.........t.
-0000b900: 6800 7200 6500 6500 5f00 6400 6900 6d00  h.r.e.e._.d.i.m.
-0000b910: 6500 6e00 7300 6900 6f00 6e00 736c 6731  e.n.s.i.o.n.slg1
-0000b920: 5363 6f6d 7000 0000 0000 033c cc00 0000  Scomp......<....
-0000b930: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
-0000b940: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
-0000b950: 736d 6f44 4462 6c6f 6200 0000 08f6 8857  smoDDblob......W
-0000b960: d65e 24c5 4100 0000 1000 7400 6800 7200  .^$.A.....t.h.r.
-0000b970: 6500 6500 5f00 6400 6900 6d00 6500 6e00  e.e._.d.i.m.e.n.
-0000b980: 7300 6900 6f00 6e00 736d 6f64 4462 6c6f  s.i.o.n.smodDblo
-0000b990: 6200 0000 08f6 8857 d65e 24c5 4100 0000  b......W.^$.A...
-0000b9a0: 1000 7400 6800 7200 6500 6500 5f00 6400  ..t.h.r.e.e._.d.
-0000b9b0: 6900 6d00 6500 6e00 7300 6900 6f00 6e00  i.m.e.n.s.i.o.n.
-0000b9c0: 7370 6831 5363 6f6d 7000 0000 0000 03a0  sph1Scomp.......
-0000b9d0: 0000 0000 0200 7500 6962 7773 7062 6c6f  ......u.ibwspblo
-0000b9e0: 6200 0000 ca62 706c 6973 7430 30d7 0102  b....bplist00...
-0000b9f0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
-0000ba00: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
-0000ba10: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
-0000ba20: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-0000ba30: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-0000ba40: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-0000ba50: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-0000ba60: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
-0000ba70: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
-0000ba80: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
-0000ba90: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
-0000baa0: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
-0000bab0: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
-0000bac0: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000bad0: 0000 0000 0012 10b6 0000 0002 0075 0069  .............u.i
-0000bae0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
-0000baf0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-0000bb00: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
-0000bb10: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
-0000bb20: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
-0000bb30: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
-0000bb40: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
-0000bb50: 655a 736f 7274 436f 6c75 6d6e 5869 636f  eZsortColumnXico
-0000bb60: 6e53 697a 655f 1010 7573 6552 656c 6174  nSize_..useRelat
-0000bb70: 6976 6544 6174 6573 1001 09ab 0c15 1a1f  iveDates........
-0000bb80: 2328 2d32 373c 41d4 0d0e 0f10 0a12 0a14  #(-27<A.........
-0000bb90: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-0000bba0: 7363 656e 6469 6e67 5a69 6465 6e74 6966  scendingZidentif
-0000bbb0: 6965 7209 1101 c709 546e 616d 65d4 100e  ier.....Tname...
-0000bbc0: 0f0d 1617 1818 5875 6269 7175 6974 7910  ......Xubiquity.
-0000bbd0: 2308 08d4 100f 0e0d 1b18 1d0a 5c64 6174  #...........\dat
-0000bbe0: 654d 6f64 6966 6965 6408 10b5 09d4 100f  eModified.......
-0000bbf0: 0e0d 2018 1d18 5b64 6174 6543 7265 6174  .. ...[dateCreat
-0000bc00: 6564 0808 d410 0f0e 0d24 1826 0a54 7369  ed.......$.&.Tsi
-0000bc10: 7a65 0810 6109 d410 0f0e 0d29 0a2b 0a54  ze..a......).+.T
-0000bc20: 6b69 6e64 0910 7309 d410 0f0e 0d2e 0a30  kind..s........0
-0000bc30: 1855 6c61 6265 6c09 1064 08d4 100f 0e0d  .Ulabel..d......
-0000bc40: 330a 3518 5776 6572 7369 6f6e 0910 4b08  3.5.Wversion..K.
-0000bc50: d410 0f0e 0d38 0a3a 1858 636f 6d6d 656e  .....8.:.Xcommen
-0000bc60: 7473 0911 012c 08d4 100f 0e0d 3d18 3f18  ts...,......=.?.
-0000bc70: 5e64 6174 654c 6173 744f 7065 6e65 6408  ^dateLastOpened.
-0000bc80: 10c8 08d4 100e 0f0d 421d 1818 5964 6174  ........B...Ydat
-0000bc90: 6541 6464 6564 0808 0823 4028 0000 0000  eAdded...#@(....
-0000bca0: 0000 546e 616d 6523 4030 0000 0000 0000  ..Tname#@0......
-0000bcb0: 0900 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
-0000bcc0: 7000 7900 8c00 8e00 8f00 9b00 a400 ac00  p.y.............
-0000bcd0: b200 bc00 c700 c800 cb00 cc00 d100 da00  ................
-0000bce0: e300 e500 e600 e700 f000 fd00 fe01 0001  ................
-0000bcf0: 0101 0a01 1601 1701 1801 2101 2601 2701  ..........!.&.'.
-0000bd00: 2901 2a01 3301 3801 3901 3b01 3c01 4501  ).*.3.8.9.;.<.E.
-0000bd10: 4b01 4c01 4e01 4f01 5801 6001 6101 6301  K.L.N.O.X.`.a.c.
-0000bd20: 6401 6d01 7601 7701 7a01 7b01 8401 9301  d.m.v.w.z.{.....
-0000bd30: 9401 9601 9701 a001 aa01 ab01 ac01 ad01  ................
-0000bd40: b601 bb01 c400 0000 0000 0002 0100 0000  ................
-0000bd50: 0000 0000 4a00 0000 0000 0000 0000 0000  ....J...........
-0000bd60: 0000 0001 c500 0000 0200 7500 696c 7376  ..........u.ilsv
-0000bd70: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
-0000bd80: 30d8 0102 0304 0506 0708 090a 0b1a 4546  0.............EF
-0000bd90: 470a 5f10 1276 6965 774f 7074 696f 6e73  G._..viewOptions
-0000bda0: 5665 7273 696f 6e5f 100f 7368 6f77 4963  Version_..showIc
-0000bdb0: 6f6e 5072 6576 6965 7757 636f 6c75 6d6e  onPreviewWcolumn
-0000bdc0: 735f 1011 6361 6c63 756c 6174 6541 6c6c  s_..calculateAll
-0000bdd0: 5369 7a65 7358 7465 7874 5369 7a65 5a73  SizesXtextSizeZs
-0000bde0: 6f72 7443 6f6c 756d 6e58 6963 6f6e 5369  ortColumnXiconSi
-0000bdf0: 7a65 5f10 1075 7365 5265 6c61 7469 7665  ze_..useRelative
-0000be00: 4461 7465 7310 0109 d90c 0d0e 0f10 1112  Dates...........
-0000be10: 1314 151e 2327 2b30 353a 3f58 636f 6d6d  ....#'+05:?Xcomm
-0000be20: 656e 7473 5e64 6174 654c 6173 744f 7065  ents^dateLastOpe
-0000be30: 6e65 645c 6461 7465 4d6f 6469 6669 6564  ned\dateModified
-0000be40: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
-0000be50: 6555 6c61 6265 6c54 6b69 6e64 5776 6572  eUlabelTkindWver
-0000be60: 7369 6f6e 546e 616d 65d4 1617 1819 1a0a  sionTname.......
-0000be70: 1c1d 5776 6973 6962 6c65 5961 7363 656e  ..WvisibleYascen
-0000be80: 6469 6e67 5577 6964 7468 5569 6e64 6578  dingUwidthUindex
-0000be90: 0809 1101 2c10 07d4 1617 1819 1a1a 2122  ....,.........!"
-0000bea0: 0808 10c8 1008 d416 1718 190a 1a26 0909  .............&..
-0000beb0: 0810 b5d4 1617 1819 1a1a 262a 0808 1002  ..........&*....
-0000bec0: d416 1718 190a 1a2e 2f09 0810 6110 03d4  ......../...a...
-0000bed0: 1617 1819 1a0a 3334 0809 1064 1005 d416  ......34...d....
-0000bee0: 1718 190a 0a38 3909 0910 7310 04d4 1617  .....89...s.....
-0000bef0: 1819 1a0a 3d3e 0809 104b 1006 d419 1817  ....=>...K......
-0000bf00: 1640 410a 0a10 0011 01c7 0909 0823 4028  .@A..........#@(
-0000bf10: 0000 0000 0000 546e 616d 6523 4030 0000  ......Tname#@0..
-0000bf20: 0000 0000 0900 0800 1900 2e00 4000 4800  ............@.H.
-0000bf30: 5c00 6500 7000 7900 8c00 8e00 8f00 a200  \.e.p.y.........
-0000bf40: ab00 ba00 c700 d300 d800 de00 e300 eb00  ................
-0000bf50: f000 f901 0101 0b01 1101 1701 1801 1901  ................
-0000bf60: 1c01 1e01 2701 2801 2901 2b01 2d01 3601  ....'.(.).+.-.6.
-0000bf70: 3701 3801 3a01 4301 4401 4501 4701 5001  7.8.:.C.D.E.G.P.
-0000bf80: 5101 5201 5401 5601 5f01 6001 6101 6301  Q.R.T.V._.`.a.c.
-0000bf90: 6501 6e01 6f01 7001 7201 7401 7d01 7e01  e.n.o.p.r.t.}.~.
-0000bfa0: 7f01 8101 8301 8c01 8e01 9101 9201 9301  ................
-0000bfb0: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
-0000bfc0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-0000bfd0: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
-0000bfe0: 6f44 4462 6c6f 6200 0000 087e abce 1cd0  oDDblob....~....
-0000bff0: 1fc5 4100 0000 0000 0000 0000 0000 0000  ..A.............
-0000c000: 0000 0000                                ....
+0000a910: 6500 6e00 7300 6900 6f00 6e00 7362 7773  e.n.s.i.o.n.sbws
+0000a920: 7062 6c6f 6200 0000 b962 706c 6973 7430  pblob....bplist0
+0000a930: 30d6 0102 0304 0506 0708 0708 0b08 5d53  0.............]S
+0000a940: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
+0000a950: 7754 6f6f 6c62 6172 5b53 686f 7754 6162  wToolbar[ShowTab
+0000a960: 5669 6577 5f10 1443 6f6e 7461 696e 6572  View_..Container
+0000a970: 5368 6f77 5369 6465 6261 725c 5769 6e64  ShowSidebar\Wind
+0000a980: 6f77 426f 756e 6473 5b53 686f 7753 6964  owBounds[ShowSid
+0000a990: 6562 6172 0809 0809 5f10 197b 7b32 3630  ebar...._..{{260
+0000a9a0: 2c20 3132 397d 2c20 7b31 3138 302c 2036  , 129}, {1180, 6
+0000a9b0: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
+0000a9c0: 6f8b 0000 0000 0000 0101 0000 0000 0000  o...............
+0000a9d0: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+0000a9e0: 008c 0000 0010 0074 0068 0072 0065 0065  .......t.h.r.e.e
+0000a9f0: 005f 0064 0069 006d 0065 006e 0073 0069  ._.d.i.m.e.n.s.i
+0000aa00: 006f 006e 0073 6c67 3153 636f 6d70 0000  .o.n.slg1Scomp..
+0000aa10: 0000 0003 3ccc 0000 0010 0074 0068 0072  ....<......t.h.r
+0000aa20: 0065 0065 005f 0064 0069 006d 0065 006e  .e.e._.d.i.m.e.n
+0000aa30: 0073 0069 006f 006e 0073 6d6f 4444 626c  .s.i.o.n.smoDDbl
+0000aa40: 6f62 0000 0008 f688 57d6 5e24 c541 0000  ob......W.^$.A..
+0000aa50: 0010 0074 0068 0072 0065 0065 005f 0064  ...t.h.r.e.e._.d
+0000aa60: 0069 006d 0065 006e 0073 0069 006f 006e  .i.m.e.n.s.i.o.n
+0000aa70: 0073 6d6f 6444 626c 6f62 0000 0008 f688  .smodDblob......
+0000aa80: 57d6 5e24 c541 0000 0010 0074 0068 0072  W.^$.A.....t.h.r
+0000aa90: 0065 0065 005f 0064 0069 006d 0065 006e  .e.e._.d.i.m.e.n
+0000aaa0: 0073 0069 006f 006e 0073 7068 3153 636f  .s.i.o.n.sph1Sco
+0000aab0: 6d70 0000 0000 0003 a000 0000 0010 0074  mp.............t
+0000aac0: 0068 0072 0065 0065 005f 0064 0069 006d  .h.r.e.e._.d.i.m
+0000aad0: 0065 006e 0073 0069 006f 006e 0073 7653  .e.n.s.i.o.n.svS
+0000aae0: 726e 6c6f 6e67 0000 0001 0000 0002 0075  rnlong.........u
+0000aaf0: 0069 6277 7370 626c 6f62 0000 00ca 6270  .ibwspblob....bp
+0000ab00: 6c69 7374 3030 d701 0203 0405 0607 0808  list00..........
+0000ab10: 0a08 0a0d 0a5d 5368 6f77 5374 6174 7573  .....]ShowStatus
+0000ab20: 4261 725b 5368 6f77 5061 7468 6261 725b  Bar[ShowPathbar[
+0000ab30: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+0000ab40: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+0000ab50: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+0000ab60: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+0000ab70: 5369 6465 6261 7208 0809 0809 5f10 197b  Sidebar....._..{
+0000ab80: 7b33 3534 2c20 3132 347d 2c20 7b31 3037  {354, 124}, {107
+0000ab90: 362c 2036 3231 7d7d 0908 1725 313d 4960  6, 621}}...%1=I`
+0000aba0: 6d79 7a7b 7c7d 7e9a 0000 0000 0000 0101  myz{|}~.........
+0000abb0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
+0000abc0: 0000 0000 0000 009b 0000 0002 0075 0069  .............u.i
+0000abd0: 6473 636c 626f 6f6c 0000 0000 0200 7500  dsclbool......u.
+0000abe0: 696c 6731 5363 6f6d 7000 0000 0000 1224  ilg1Scomp......$
+0000abf0: 3e00 0000 0200 7500 696c 7376 4362 6c6f  >.....u.ilsvCblo
+0000ac00: 6200 0002 7962 706c 6973 7430 30d8 0102  b...ybplist00...
+0000ac10: 0304 0506 0708 090a 0b18 4647 480a 5f10  ..........FGH._.
+0000ac20: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
+0000ac30: 696f 6e5f 100f 7368 6f77 4963 6f6e 5072  ion_..showIconPr
+0000ac40: 6576 6965 7757 636f 6c75 6d6e 735f 1011  eviewWcolumns_..
+0000ac50: 6361 6c63 756c 6174 6541 6c6c 5369 7a65  calculateAllSize
+0000ac60: 7358 7465 7874 5369 7a65 5a73 6f72 7443  sXtextSizeZsortC
+0000ac70: 6f6c 756d 6e58 6963 6f6e 5369 7a65 5f10  olumnXiconSize_.
+0000ac80: 1075 7365 5265 6c61 7469 7665 4461 7465  .useRelativeDate
+0000ac90: 7310 0109 ab0c 151a 1f23 282d 3237 3c41  s........#(-27<A
+0000aca0: d40d 0e0f 100a 120a 1457 7669 7369 626c  .........Wvisibl
+0000acb0: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
+0000acc0: 675a 6964 656e 7469 6669 6572 0911 01c7  gZidentifier....
+0000acd0: 0954 6e61 6d65 d410 0e0f 0d16 1718 1858  .Tname.........X
+0000ace0: 7562 6971 7569 7479 1023 0808 d410 0f0e  ubiquity.#......
+0000acf0: 0d1b 181d 0a5c 6461 7465 4d6f 6469 6669  .....\dateModifi
+0000ad00: 6564 0810 b509 d410 0f0e 0d20 181d 185b  ed......... ...[
+0000ad10: 6461 7465 4372 6561 7465 6408 08d4 100f  dateCreated.....
+0000ad20: 0e0d 2418 260a 5473 697a 6508 1061 09d4  ..$.&.Tsize..a..
+0000ad30: 100f 0e0d 290a 2b0a 546b 696e 6409 1073  ....).+.Tkind..s
+0000ad40: 09d4 100f 0e0d 2e0a 3018 556c 6162 656c  ........0.Ulabel
+0000ad50: 0910 6408 d410 0f0e 0d33 0a35 1857 7665  ..d......3.5.Wve
+0000ad60: 7273 696f 6e09 104b 08d4 100f 0e0d 380a  rsion..K......8.
+0000ad70: 3a18 5863 6f6d 6d65 6e74 7309 1101 2c08  :.Xcomments...,.
+0000ad80: d410 0f0e 0d3d 183f 185e 6461 7465 4c61  .....=.?.^dateLa
+0000ad90: 7374 4f70 656e 6564 0810 c808 d410 0e0f  stOpened........
+0000ada0: 0d42 1d18 1859 6461 7465 4164 6465 6408  .B...YdateAdded.
+0000adb0: 0808 2340 2800 0000 0000 0054 6e61 6d65  ..#@(......Tname
+0000adc0: 2340 3000 0000 0000 0009 0008 0019 002e  #@0.............
+0000add0: 0040 0048 005c 0065 0070 0079 008c 008e  .@.H.\.e.p.y....
+0000ade0: 008f 009b 00a4 00ac 00b2 00bc 00c7 00c8  ................
+0000adf0: 00cb 00cc 00d1 00da 00e3 00e5 00e6 00e7  ................
+0000ae00: 00f0 00fd 00fe 0100 0101 010a 0116 0117  ................
+0000ae10: 0118 0121 0126 0127 0129 012a 0133 0138  ...!.&.'.).*.3.8
+0000ae20: 0139 013b 013c 0145 014b 014c 014e 014f  .9.;.<.E.K.L.N.O
+0000ae30: 0158 0160 0161 0163 0164 016d 0176 0177  .X.`.a.c.d.m.v.w
+0000ae40: 017a 017b 0184 0193 0194 0196 0197 01a0  .z.{............
+0000ae50: 01aa 01ab 01ac 01ad 01b6 01bb 01c4 0000  ................
+0000ae60: 0000 0000 0201 0000 0000 0000 004a 0000  .............J..
+0000ae70: 0000 0000 0000 0000 0000 0000 01c5 7c01  ..............|.
+0000ae80: 8501 8e01 8f01 9101 9201 a101 aa01 ab01  ................
+0000ae90: ac01 b601 bf01 c701 cd01 d701 d801 da01  ................
+0000aea0: db01 e601 ef01 f001 f102 0302 0c02 0d02  ................
+0000aeb0: 0e02 2102 2202 2b02 3802 3900 0000 0000  ..!.".+.8.9.....
+0000aec0: 0002 0100 0000 0000 0000 5a00 0000 0000  ..........Z.....
+0000aed0: 0000 0000 0000 0000 0002 3b62 6172 5b53  ..........;bar[S
+0000aee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
+0000aef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
+0000af00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
+0000af10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
+0000af20: 197b 7b32 3630 2c20 3132 397d 2c20 7b31  .{{260, 129}, {1
+0000af30: 3138 302c 2036 3336 7d7d 0908 1523 2f3b  180, 636}}...#/;
+0000af40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
+0000af50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
+0000af60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
+0000af70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
+0000af80: 636f 6d70 0000 0000 0010 0215 0000 0000  comp............
+0000af90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b000: 0000 0000 0000 0000 0000 000d 0000 0002  ................
+0000b010: 0075 0069 6d6f 4444 626c 6f62 0000 0008  .u.imoDDblob....
+0000b020: 7eab ce1c d01f c541 0000 0002 0075 0069  ~......A.....u.i
+0000b030: 6d6f 6444 626c 6f62 0000 0008 7eab ce1c  modDblob....~...
+0000b040: d01f c541 0000 0002 0075 0069 7068 3153  ...A.....u.iph1S
+0000b050: 636f 6d70 0000 0000 0018 6000 0000 0002  comp......`.....
+0000b060: 0075 0069 7653 726e 6c6f 6e67 0000 0001  .u.ivSrnlong....
+0000b070: 0000 000c 0075 006e 0073 0075 0070 0065  .....u.n.s.u.p.e
+0000b080: 0072 0076 0069 0073 0065 0064 6277 7370  .r.v.i.s.e.dbwsp
+0000b090: 626c 6f62 0000 00ca 6270 6c69 7374 3030  blob....bplist00
+0000b0a0: d701 0203 0405 0607 0808 0a08 0a0d 0a5d  ...............]
+0000b0b0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+0000b0c0: 6f77 5061 7468 6261 725b 5368 6f77 546f  owPathbar[ShowTo
+0000b0d0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+0000b0e0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+0000b0f0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+0000b100: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+0000b110: 7208 0809 0809 5f10 197b 7b33 3534 2c20  r....._..{{354, 
+0000b120: 3132 347d 2c20 7b31 3037 362c 2036 3231  124}, {1076, 621
+0000b130: 7d7d 0908 1725 313d 4960 6d79 7a7b 7c7d  }}...%1=I`myz{|}
+0000b140: 7e9a 0000 0000 0000 0101 0000 0000 0000  ~...............
+0000b150: 000f 0000 0000 0000 0000 0000 0000 0000  ................
+0000b160: 009b 0000 000c 0075 006e 0073 0075 0070  .......u.n.s.u.p
+0000b170: 0065 0072 0076 0069 0073 0065 0064 6473  .e.r.v.i.s.e.dds
+0000b180: 636c 626f 6f6c 0000 0000 0c00 7500 6e00  clbool......u.n.
+0000b190: 7300 7500 7000 6500 7200 7600 6900 7300  s.u.p.e.r.v.i.s.
+0000b1a0: 6500 646c 6731 5363 6f6d 7000 0000 0000  e.dlg1Scomp.....
+0000b1b0: 03e8 6900 0000 0c00 7500 6e00 7300 7500  ..i.....u.n.s.u.
+0000b1c0: 7000 6500 7200 7600 6900 7300 6500 646c  p.e.r.v.i.s.e.dl
+0000b1d0: 7376 4362 6c6f 6200 0002 8162 706c 6973  svCblob....bplis
+0000b1e0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
+0000b1f0: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
+0000b200: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+0000b210: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+0000b220: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+0000b230: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
+0000b240: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+0000b250: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
+0000b260: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
+0000b270: 09ab 0c15 1a1f 2328 2d32 373c 41d4 0d0e  ......#(-27<A...
+0000b280: 0f10 1112 0a0a 5a69 6465 6e74 6966 6965  ......Zidentifie
+0000b290: 7255 7769 6474 6859 6173 6365 6e64 696e  rUwidthYascendin
+0000b2a0: 6757 7669 7369 626c 6554 6e61 6d65 1101  gWvisibleTname..
+0000b2b0: c709 09d4 0d0e 0f10 1617 1818 5875 6269  ............Xubi
+0000b2c0: 7175 6974 7910 2308 08d4 100e 0f0d 0a1c  quity.#.........
+0000b2d0: 0a1e 0910 b509 5c64 6174 654d 6f64 6966  ......\dateModif
+0000b2e0: 6965 64d4 0d0e 0f10 201c 1818 5b64 6174  ied..... ...[dat
+0000b2f0: 6543 7265 6174 6564 0808 d40d 0e0f 1024  eCreated.......$
+0000b300: 2518 0a54 7369 7a65 1061 0809 d40d 0e0f  %..Tsize.a......
+0000b310: 1029 2a0a 0a54 6b69 6e64 1073 0909 d40d  .)*..Tkind.s....
+0000b320: 0e0f 102e 2f0a 1855 6c61 6265 6c10 6409  ..../..Ulabel.d.
+0000b330: 08d4 0d0e 0f10 3334 0a18 5776 6572 7369  ......34..Wversi
+0000b340: 6f6e 104b 0908 d40d 0e0f 1038 390a 1858  on.K.......89..X
+0000b350: 636f 6d6d 656e 7473 1101 2c09 08d4 0d0e  comments..,.....
+0000b360: 0f10 3d3e 1818 5e64 6174 654c 6173 744f  ..=>..^dateLastO
+0000b370: 7065 6e65 6410 c808 08d4 0d0e 0f10 421c  pened.........B.
+0000b380: 1818 5964 6174 6541 6464 6564 0808 0823  ..YdateAdded...#
+0000b390: 4028 0000 0000 0000 5c64 6174 654d 6f64  @(......\dateMod
+0000b3a0: 6966 6965 6409 1001 0008 0019 0022 0034  ified........".4
+0000b3b0: 003c 0050 0059 0064 0077 008c 0095 0096  .<.P.Y.d.w......
+0000b3c0: 00a2 00ab 00b6 00bc 00c6 00ce 00d3 00d6  ................
+0000b3d0: 00d7 00d8 00e1 00ea 00ec 00ed 00ee 00f7  ................
+0000b3e0: 00f8 00fa 00fb 0108 0111 011d 011e 011f  ................
+0000b3f0: 0128 012d 012f 0130 0131 013a 013f 0141  .(.-./.0.1.:.?.A
+0000b400: 0142 0143 014c 0152 0154 0155 0156 015f  .B.C.L.R.T.U.V._
+0000b410: 0167 0169 016a 016b 0174 017d 0180 0181  .g.i.j.k.t.}....
+0000b420: 0182 018b 019a 019c 019d 019e 01a7 01b1  ................
+0000b430: 01b2 01b3 01b4 01bd 01ca 01cb 0000 0000  ................
+0000b440: 0000 0201 0000 0000 0000 004a 0000 0000  ...........J....
+0000b450: 0000 0000 0000 0000 0000 01cd 0000 000c  ................
+0000b460: 0075 006e 0073 0075 0070 0065 0072 0076  .u.n.s.u.p.e.r.v
+0000b470: 0069 0073 0065 0064 6c73 7670 626c 6f62  .i.s.e.dlsvpblob
+0000b480: 0000 0266 6270 6c69 7374 3030 d801 0203  ...fbplist00....
+0000b490: 0405 0607 0809 0a0b 1a46 470a 2458 6963  .........FG.$Xic
+0000b4a0: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
+0000b4b0: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
+0000b4c0: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
+0000b4d0: 697a 6573 5874 6578 7453 697a 655a 736f  izesXtextSizeZso
+0000b4e0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+0000b4f0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+0000b500: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+0000b510: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
+0000b520: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
+0000b530: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
+0000b540: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
+0000b550: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+0000b560: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+0000b570: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
+0000b580: 1a1b 0a1d 5776 6973 6962 6c65 5577 6964  ....WvisibleUwid
+0000b590: 7468 5961 7363 656e 6469 6e67 5569 6e64  thYascendingUind
+0000b5a0: 6578 0811 012c 0910 07d4 1617 1819 1a20  ex...,......... 
+0000b5b0: 1a22 0810 c808 1008 d419 1718 1624 250a  ."...........$%.
+0000b5c0: 0a10 0110 b509 09d4 1617 1819 1a25 1a2b  .............%.+
+0000b5d0: 0808 1002 d416 1718 190a 2e1a 3009 1061  ............0..a
+0000b5e0: 0810 03d4 1617 1819 1a33 0a35 0810 6409  .........3.5..d.
+0000b5f0: 1005 d416 1718 190a 380a 3a09 1073 0910  ........8.:..s..
+0000b600: 04d4 1617 1819 1a3d 0a3f 0810 4b09 1006  .......=.?..K...
+0000b610: d416 1718 190a 420a 4409 1101 c709 1000  ......B.D.......
+0000b620: 0823 4028 0000 0000 0000 5c64 6174 654d  .#@(......\dateM
+0000b630: 6f64 6966 6965 6409 0008 0019 0022 0034  odified......".4
+0000b640: 003c 0050 0059 0064 0077 008c 0095 0096  .<.P.Y.d.w......
+0000b650: 00a9 00b2 00c1 00ce 00da 00df 00e5 00ea  ................
+0000b660: 00f2 00f7 0100 0108 010e 0118 011e 011f  ................
+0000b670: 0122 0123 0125 012e 012f 0131 0132 0134  .".#.%.../.1.2.4
+0000b680: 013d 013f 0141 0142 0143 014c 014d 014e  .=.?.A.B.C.L.M.N
+0000b690: 0150 0159 015a 015c 015d 015f 0168 0169  .P.Y.Z.\.]._.h.i
+0000b6a0: 016b 016c 016e 0177 0178 017a 017b 017d  .k.l.n.w.x.z.{.}
+0000b6b0: 0186 0187 0189 018a 018c 0195 0196 0199  ................
+0000b6c0: 019a 019c 019d 01a6 01b3 0000 0000 0000  ................
+0000b6d0: 0201 0000 0000 0000 0049 0000 0000 0000  .........I......
+0000b6e0: 0000 0000 0000 0000 01b4 0000 000c 0075  ...............u
+0000b6f0: 006e 0073 0075 0070 0065 0072 0076 0069  .n.s.u.p.e.r.v.i
+0000b700: 0073 0065 0064 6d6f 4444 626c 6f62 0000  .s.e.dmoDDblob..
+0000b710: 0008 cbf3 6409 d917 c541 0000 000c 0075  ....d....A.....u
+0000b720: 006e 0073 0075 0070 0065 0072 0076 0069  .n.s.u.p.e.r.v.i
+0000b730: 0073 0065 0064 6d6f 6444 626c 6f62 0000  .s.e.dmodDblob..
+0000b740: 0008 cbf3 6409 d917 c541 0000 000c 0075  ....d....A.....u
+0000b750: 006e 0073 0075 0070 0065 0072 0076 0069  .n.s.u.p.e.r.v.i
+0000b760: 0073 0065 0064 7068 3153 636f 6d70 0000  .s.e.dph1Scomp..
+0000b770: 0000 0004 d000 0000 000c 0075 006e 0073  ...........u.n.s
+0000b780: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+0000b790: 0064 7653 726e 6c6f 6e67 0000 0001 8e01  .dvSrnlong......
+0000b7a0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
+0000b7b0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
+0000b7c0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
+0000b7d0: 1b00 7400 6800 6900 7200 6400 5f00 7000  ..t.h.i.r.d._.p.
+0000b7e0: 6100 7200 7400 7900 5f00 6c00 6100 6200  a.r.t.y._.l.a.b.
+0000b7f0: 6500 6c00 5f00 6100 7000 7000 6500 6e00  e.l._.a.p.p.e.n.
+0000b800: 6400 6500 0000 000e 0000 0000 0000 b80b  d.e.............
+0000b810: 0000 0045 0000 300c 0000 100c 0000 400c  ...E..0.......@.
+0000b820: 0000 500c 0000 600c 0000 700c 0000 800c  ..P...`...p.....
+0000b830: 0000 900c 0000 040a 0000 200c 0000 a00c  .......... .....
+0000b840: 0000 b00b 0000 0000 0000 0000 0000 0000  ................
+0000b850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b8a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b8b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b8c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b8d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b8e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b8f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b9a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b9b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b9c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b9d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b9e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000b9f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000ba90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000baa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000baf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bb90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bbb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bbc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bbd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bbe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bbf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bc00: 0000 0000 0000 0000 0000 0000 0000 0001  ................
+0000bc10: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
+0000bc20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+0000bc30: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
+0000bc40: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+0000bc50: 0100 0002 0000 0000 0000 0000 0100 0008  ................
+0000bc60: 0000 0000 0000 0000 0000 0000 0100 00c0  ................
+0000bc70: 0000 0000 0000 0000 0100 0100 0000 0000  ................
+0000bc80: 0100 0200 0000 0000 0100 0400 0000 0000  ................
+0000bc90: 0100 0800 0000 0000 0100 1000 0000 0000  ................
+0000bca0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
+0000bcb0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
+0000bcc0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
+0000bcd0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
+0000bce0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
+0000bcf0: 0061 7469 7665 4461 7465 735f 1012 7669  .ativeDates_..vi
+0000bd00: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+0000bd10: 2340 3000 0000 0000 0009 d90c 0d0e 0f10  #@0.............
+0000bd20: 1112 1314 151e 2328 2c31 363b 4058 636f  ......#(,16;@Xco
+0000bd30: 6d6d 656e 7473 5e64 6174 654c 6173 744f  mments^dateLastO
+0000bd40: 7065 6e65 645c 6461 7465 4d6f 6469 6669  pened\dateModifi
+0000bd50: 6564 5b64 6174 6543 7265 6174 6564 5473  ed[dateCreatedTs
+0000bd60: 697a 6555 6c61 6265 6c54 6b69 6e64 5776  izeUlabelTkindWv
+0000bd70: 6572 7369 6f6e 546e 616d 65d4 1617 1819  ersionTname.....
+0000bd80: 1a1b 0a1d 5776 6973 6962 6c65 5577 6964  ....WvisibleUwid
+0000bd90: 7468 5961 7363 656e 6469 6e67 5569 6e64  thYascendingUind
+0000bda0: 6578 0811 012c 0910 07d4 1617 1819 1a20  ex...,......... 
+0000bdb0: 1a22 0810 c808 1008 d419 1718 1624 250a  ."...........$%.
+0000bdc0: 0a10 0110 b509 09d4 1617 1819 1a25 1a2b  .............%.+
+0000bdd0: 0808 1002 d416 1718 190a 2e1a 3009 1061  ............0..a
+0000bde0: 0810 03d4 1617 1819 1a33 0a35 0810 6409  .........3.5..d.
+0000bdf0: 1005 d416 1718 190a 380a 3a09 1073 0910  ........8.:..s..
+0000be00: 04d4 1617 1819 1a3d 0a3f 0810 4b09 1006  .......=.?..K...
+0000be10: d416 1718 190a 420a 4409 1101 c709 1000  ......B.D.......
+0000be20: 0823 4028 0000 0000 0000 5c64 6174 654d  .#@(......\dateM
+0000be30: 6f64 6966 6965 6409 0008 0019 0022 0034  odified......".4
+0000be40: 003c 0050 0059 0064 0077 008c 0095 0096  .<.P.Y.d.w......
+0000be50: 00a9 00b2 00c1 00ce 00da 00df 00e5 00ea  ................
+0000be60: 00f2 00f7 0100 0108 010e 0118 011e 011f  ................
+0000be70: 0122 0123 0125 012e 012f 0131 0132 0134  .".#.%.../.1.2.4
+0000be80: 013d 013f 0141 0142 0143 014c 014d 014e  .=.?.A.B.C.L.M.N
+0000be90: 0150 0159 015a 015c 015d 015f 0168 0169  .P.Y.Z.\.]._.h.i
+0000bea0: 016b 016c 016e 0177 0178 017a 017b 017d  .k.l.n.w.x.z.{.}
+0000beb0: 0186 0187 0189 018a 018c 0195 0196 0199  ................
+0000bec0: 019a 019c 019d 01a6 01b3 0000 0000 0000  ................
+0000bed0: 0201 0000 0000 0000 0049 0000 0000 0000  .........I......
+0000bee0: 0000 0000 0000 0000 01b4 0000 000c 0075  ...............u
+0000bef0: 006e 0073 0075 0070 0065 0072 0076 0069  .n.s.u.p.e.r.v.i
+0000bf00: 0073 0065 0064 6d6f 4444 626c 6f62 0000  .s.e.dmoDDblob..
+0000bf10: 0008 cbf3 6409 d917 c541 0000 000c 0075  ....d....A.....u
+0000bf20: 006e 0073 0075 0070 0065 0072 0076 0069  .n.s.u.p.e.r.v.i
+0000bf30: 0073 0065 0064 6d6f 6444 626c 6f62 0000  .s.e.dmodDblob..
+0000bf40: 0008 cbf3 6409 d917 c541 0000 000c 0075  ....d....A.....u
+0000bf50: 006e 0073 0075 0070 0065 0072 0076 0069  .n.s.u.p.e.r.v.i
+0000bf60: 0073 0065 0064 7068 3153 636f 6d70 0000  .s.e.dph1Scomp..
+0000bf70: 0000 0004 d000 0000 000c 0075 006e 0073  ...........u.n.s
+0000bf80: 0075 0070 0065 0072 0076 0069 0073 0065  .u.p.e.r.v.i.s.e
+0000bf90: 0064 7653 726e 6c6f 6e67 0000 0001 8e01  .dvSrnlong......
+0000bfa0: 9101 9201 9301 9401 9d01 a201 ab00 0000  ................
+0000bfb0: 0000 0002 0100 0000 0000 0000 4900 0000  ............I...
+0000bfc0: 0000 0000 0000 0000 0000 0001 ac00 0000  ................
+0000bfd0: 1b00 7400 6800 6900 7200 6400 5f00 7000  ..t.h.i.r.d._.p.
+0000bfe0: 6100 7200 7400 7900 5f00 6c00 6100 6200  a.r.t.y._.l.a.b.
+0000bff0: 6500 6c00 5f00 6100 7000 7000 6500 6e00  e.l._.a.p.p.e.n.
+0000c000: 6400 6500                                d.e.
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -276,18 +276,18 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 0004 473f 0000 000b 005f 005f 0070  ....G?....._._.p
+000011a0: 0000 0004 52ac 0000 000b 005f 005f 0070  ....R......_._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 1611 2c41  moDDblob......,A
-000011d0: a729 c541 0000 000b 005f 005f 0070 0079  .).A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 adae 79e0  moDDblob......y.
+000011d0: 572c c541 0000 000b 005f 005f 0070 0079  W,.A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
 000011f0: 6444 626c 6f62 0000 0008 1611 2c41 a729  dDblob......,A.)
 00001200: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 00001220: 636f 6d70 0000 0000 0005 0000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.65.1/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/requirements.txt` & `Simba-UW-tf-dev-1.65.1/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/utils/cli/.DS_Store`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 000b f7a8 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0000 1281 0000 000b 005f 005f 0070  ..........._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 1584 a98c  moDDblob........
-00000160: 892b c541 0000 000b 005f 005f 0070 0079  .+.A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 e40f 369b  moDDblob......6.
+00000160: 8b2b c541 0000 000b 005f 005f 0070 0079  .+.A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 1584 a98c 892b  dDblob.........+
+00000180: 6444 626c 6f62 0000 0008 e40f 369b 8b2b  dDblob......6..+
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 000d 0000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0000 3000 0000 0000  comp......0.....
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.65.1/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.65.1/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.65.1/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.65.1/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.65.1/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.65.1/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.65.1/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.65.1/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.65.1/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.65.1/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.65.1/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/enums.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/utils/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -253,141 +253,141 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000e 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0006 0cc4 0000 000b 005f 005f 0070  ..........._._.p
+00001030: 0000 0006 19b9 0000 000b 005f 005f 0070  ..........._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 7b56 d344  moDDblob....{V.D
-00001060: 002b c541 0000 000b 005f 005f 0070 0079  .+.A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 1801 9146  moDDblob.......F
+00001060: e12c c541 0000 000b 005f 005f 0070 0079  .,.A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 7b56 d344 002b  dDblob....{V.D.+
+00001080: 6444 626c 6f62 0000 0008 1801 9146 e12c  dDblob.......F.,
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0007 3000 0000 0003  comp......0.....
+000010b0: 636f 6d70 0000 0000 0007 4000 0000 0003  comp......@.....
 000010c0: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
-000010d0: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
-000010e0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
-000010f0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
-00001100: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
-00001110: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00001120: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00001130: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00001140: 5368 6f77 5369 6465 6261 7208 0809 0809  ShowSidebar.....
-00001150: 5f10 197b 7b32 3332 2c20 3139 317d 2c20  _..{{232, 191}, 
-00001160: 7b31 3330 322c 2037 3134 7d7d 0908 1725  {1302, 714}}...%
-00001170: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
-00001180: 0000 0101 0000 0000 0000 000f 0000 0000  ................
-00001190: 0000 0000 0000 0000 0000 009b 0000 0003  ................
-000011a0: 0063 006c 0069 6c67 3153 636f 6d70 0000  .c.l.ilg1Scomp..
-000011b0: 0000 0000 22e5 0000 0003 0063 006c 0069  ...."......c.l.i
-000011c0: 6c73 7643 626c 6f62 0000 0297 6270 6c69  lsvCblob....bpli
-000011d0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
-000011e0: 1949 4a0a 4c58 6963 6f6e 5369 7a65 5f10  .IJ.LXiconSize_.
-000011f0: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00001200: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00001210: 6c61 7465 416c 6c53 697a 6573 5874 6578  lateAllSizesXtex
-00001220: 7453 697a 655a 736f 7274 436f 6c75 6d6e  tSizeZsortColumn
-00001230: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
-00001240: 7465 735f 1012 7669 6577 4f70 7469 6f6e  tes_..viewOption
-00001250: 7356 6572 7369 6f6e 2340 3000 0000 0000  sVersion#@0.....
-00001260: 0009 ab0c 151d 2226 2b30 353a 3f44 d40d  ......"&+05:?D..
-00001270: 0e0f 1011 120a 0a5a 6964 656e 7469 6669  .......Zidentifi
-00001280: 6572 5577 6964 7468 5961 7363 656e 6469  erUwidthYascendi
-00001290: 6e67 5776 6973 6962 6c65 546e 616d 6511  ngWvisibleTname.
-000012a0: 01c7 0909 d416 1718 0d19 1a19 1c57 7669  .............Wvi
-000012b0: 7369 626c 6555 7769 6474 6859 6173 6365  sibleUwidthYasce
-000012c0: 6e64 696e 6708 1023 0858 7562 6971 7569  nding..#.Xubiqui
-000012d0: 7479 d40d 0e0f 101e 1f19 0a5c 6461 7465  ty.........\date
-000012e0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
-000012f0: 1023 1f19 195b 6461 7465 4372 6561 7465  .#...[dateCreate
-00001300: 6408 08d4 0d0e 0f10 2728 190a 5473 697a  d.......'(..Tsiz
-00001310: 6510 6108 09d4 0d0e 0f10 2c2d 0a0a 546b  e.a.......,-..Tk
-00001320: 696e 6410 7309 09d4 0d0e 0f10 3132 0a19  ind.s.......12..
-00001330: 556c 6162 656c 1064 0908 d40d 0e0f 1036  Ulabel.d.......6
-00001340: 370a 1957 7665 7273 696f 6e10 4b09 08d4  7..Wversion.K...
-00001350: 0d0e 0f10 3b3c 0a19 5863 6f6d 6d65 6e74  ....;<..Xcomment
-00001360: 7311 012c 0908 d40d 0e0f 1040 4119 195e  s..,.......@A..^
-00001370: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
-00001380: 0808 d416 1718 0d19 1f19 4708 0859 6461  ..........G..Yda
-00001390: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
-000013a0: 0054 6e61 6d65 0910 0100 0800 1900 2200  .Tname........".
-000013b0: 3400 3c00 5000 5900 6400 7700 8c00 9500  4.<.P.Y.d.w.....
-000013c0: 9600 a200 ab00 b600 bc00 c600 ce00 d300  ................
-000013d0: d600 d700 d800 e100 e900 ef00 f900 fa00  ................
-000013e0: fc00 fd01 0601 0f01 1c01 1e01 1f01 2001  .............. .
-000013f0: 2901 3501 3601 3701 4001 4501 4701 4801  ).5.6.7.@.E.G.H.
-00001400: 4901 5201 5701 5901 5a01 5b01 6401 6a01  I.R.W.Y.Z.[.d.j.
-00001410: 6c01 6d01 6e01 7701 7f01 8101 8201 8301  l.m.n.w.........
-00001420: 8c01 9501 9801 9901 9a01 a301 b201 b401  ................
-00001430: b501 b601 bf01 c001 c101 cb01 cc01 d501  ................
-00001440: da01 db00 0000 0000 0002 0100 0000 0000  ................
-00001450: 0000 4d00 0000 0000 0000 0000 0000 0000  ..M.............
-00001460: 0001 dd00 0000 0300 6300 6c00 696c 7376  ........c.l.ilsv
-00001470: 7062 6c6f 6200 0002 5e62 706c 6973 7430  pblob...^bplist0
-00001480: 30d8 0102 0304 0506 0708 090a 0b1a 4647  0.............FG
-00001490: 0a44 5869 636f 6e53 697a 655f 100f 7368  .DXiconSize_..sh
-000014a0: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-000014b0: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-000014c0: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-000014d0: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-000014e0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000014f0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-00001500: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
-00001510: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
-00001520: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
-00001530: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
-00001540: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-00001550: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-00001560: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
-00001570: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
-00001580: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
-00001590: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
-000015a0: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
-000015b0: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
-000015c0: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
-000015d0: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
-000015e0: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
-000015f0: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
-00001600: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
-00001610: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
-00001620: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
-00001630: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
-00001640: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
-00001650: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
-00001660: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
-00001670: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
-00001680: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
-00001690: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
-000016a0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
-000016b0: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
-000016c0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-000016d0: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
-000016e0: 696d 6f44 4462 6c6f 6200 0000 0834 2b08  imoDDblob....4+.
-000016f0: c0c8 11c5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
-00001700: 6f64 4462 6c6f 6200 0000 0834 2b08 c0c8  odDblob....4+...
-00001710: 11c5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
-00001720: 5363 6f6d 7000 0000 0000 0040 0000 0000  Scomp......@....
-00001730: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
-00001740: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
-00001750: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
-00001760: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
-00001770: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
-00001780: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
-00001790: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
-000017a0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
-000017b0: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
-000017c0: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
-000017d0: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
-000017e0: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
-000017f0: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
-00001800: 0b00 7700 6100 7200 6e00 6900 6e00 6700  ..w.a.r.n.i.n.g.
-00001810: 7300 2e00 7000 7900 0000 0000 0000 0000  s...p.y.........
+000010d0: 00b9 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
+000010e0: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
+000010f0: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
+00001100: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00001110: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00001120: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00001130: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
+00001140: 095f 1019 7b7b 3236 302c 2031 3239 7d2c  ._..{{260, 129},
+00001150: 207b 3131 3830 2c20 3633 367d 7d09 0815   {1180, 636}}...
+00001160: 232f 3b52 5f6b 6c6d 6e6f 8b00 0000 0000  #/;R_klmno......
+00001170: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
+00001180: 0000 0000 0000 0000 0000 8c00 0000 0300  ................
+00001190: 6300 6c00 696c 6731 5363 6f6d 7000 0000  c.l.ilg1Scomp...
+000011a0: 0000 0042 0600 0000 0300 6300 6c00 696c  ...B......c.l.il
+000011b0: 7376 4362 6c6f 6200 0002 9762 706c 6973  svCblob....bplis
+000011c0: 7430 30d8 0102 0304 0506 0708 090a 0b19  t00.............
+000011d0: 494a 0a4c 5869 636f 6e53 697a 655f 100f  IJ.LXiconSize_..
+000011e0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
+000011f0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
+00001200: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
+00001210: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
+00001220: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+00001230: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
+00001240: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
+00001250: 09ab 0c15 1d22 262b 3035 3a3f 44d4 0d0e  ....."&+05:?D...
+00001260: 0f10 1112 0a0a 5a69 6465 6e74 6966 6965  ......Zidentifie
+00001270: 7255 7769 6474 6859 6173 6365 6e64 696e  rUwidthYascendin
+00001280: 6757 7669 7369 626c 6554 6e61 6d65 1101  gWvisibleTname..
+00001290: c709 09d4 1617 180d 191a 191c 5776 6973  ............Wvis
+000012a0: 6962 6c65 5577 6964 7468 5961 7363 656e  ibleUwidthYascen
+000012b0: 6469 6e67 0810 2308 5875 6269 7175 6974  ding..#.Xubiquit
+000012c0: 79d4 0d0e 0f10 1e1f 190a 5c64 6174 654d  y.........\dateM
+000012d0: 6f64 6966 6965 6410 b508 09d4 0d0e 0f10  odified.........
+000012e0: 231f 1919 5b64 6174 6543 7265 6174 6564  #...[dateCreated
+000012f0: 0808 d40d 0e0f 1027 2819 0a54 7369 7a65  .......'(..Tsize
+00001300: 1061 0809 d40d 0e0f 102c 2d0a 0a54 6b69  .a.......,-..Tki
+00001310: 6e64 1073 0909 d40d 0e0f 1031 320a 1955  nd.s.......12..U
+00001320: 6c61 6265 6c10 6409 08d4 0d0e 0f10 3637  label.d.......67
+00001330: 0a19 5776 6572 7369 6f6e 104b 0908 d40d  ..Wversion.K....
+00001340: 0e0f 103b 3c0a 1958 636f 6d6d 656e 7473  ...;<..Xcomments
+00001350: 1101 2c09 08d4 0d0e 0f10 4041 1919 5e64  ..,.......@A..^d
+00001360: 6174 654c 6173 744f 7065 6e65 6410 c808  ateLastOpened...
+00001370: 08d4 1617 180d 191f 1947 0808 5964 6174  .........G..Ydat
+00001380: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
+00001390: 546e 616d 6509 1001 0008 0019 0022 0034  Tname........".4
+000013a0: 003c 0050 0059 0064 0077 008c 0095 0096  .<.P.Y.d.w......
+000013b0: 00a2 00ab 00b6 00bc 00c6 00ce 00d3 00d6  ................
+000013c0: 00d7 00d8 00e1 00e9 00ef 00f9 00fa 00fc  ................
+000013d0: 00fd 0106 010f 011c 011e 011f 0120 0129  ............. .)
+000013e0: 0135 0136 0137 0140 0145 0147 0148 0149  .5.6.7.@.E.G.H.I
+000013f0: 0152 0157 0159 015a 015b 0164 016a 016c  .R.W.Y.Z.[.d.j.l
+00001400: 016d 016e 0177 017f 0181 0182 0183 018c  .m.n.w..........
+00001410: 0195 0198 0199 019a 01a3 01b2 01b4 01b5  ................
+00001420: 01b6 01bf 01c0 01c1 01cb 01cc 01d5 01da  ................
+00001430: 01db 0000 0000 0000 0201 0000 0000 0000  ................
+00001440: 004d 0000 0000 0000 0000 0000 0000 0000  .M..............
+00001450: 01dd 0000 0003 0063 006c 0069 6c73 7670  .......c.l.ilsvp
+00001460: 626c 6f62 0000 025e 6270 6c69 7374 3030  blob...^bplist00
+00001470: d801 0203 0405 0607 0809 0a0b 1a46 470a  .............FG.
+00001480: 4458 6963 6f6e 5369 7a65 5f10 0f73 686f  DXiconSize_..sho
+00001490: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
+000014a0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
+000014b0: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
+000014c0: 655a 736f 7274 436f 6c75 6d6e 5f10 1075  eZsortColumn_..u
+000014d0: 7365 5265 6c61 7469 7665 4461 7465 735f  seRelativeDates_
+000014e0: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
+000014f0: 7369 6f6e 2340 3000 0000 0000 0009 d90c  sion#@0.........
+00001500: 0d0e 0f10 1112 1314 151e 2328 2d32 373c  ..........#(-27<
+00001510: 4158 636f 6d6d 656e 7473 5e64 6174 654c  AXcomments^dateL
+00001520: 6173 744f 7065 6e65 645b 6461 7465 4372  astOpened[dateCr
+00001530: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+00001540: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+00001550: 6d65 5c64 6174 654d 6f64 6966 6965 64d4  me\dateModified.
+00001560: 1617 1819 1a1b 0a1d 5776 6973 6962 6c65  ........Wvisible
+00001570: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00001580: 5569 6e64 6578 0811 012c 0910 07d4 1617  Uindex...,......
+00001590: 1819 1a20 1a22 0810 c808 1008 d416 1718  ... ."..........
+000015a0: 191a 251a 2708 10b5 0810 02d4 1617 1819  ..%.'...........
+000015b0: 0a2a 1a2c 0910 6108 1003 d416 1718 191a  .*.,..a.........
+000015c0: 2f0a 3108 1064 0910 05d4 1617 1819 0a34  /.1..d.........4
+000015d0: 0a36 0910 7309 1004 d416 1718 191a 390a  .6..s.........9.
+000015e0: 3b08 104b 0910 06d4 1617 1819 0a3e 0a40  ;..K.........>.@
+000015f0: 0911 01c7 0910 00d4 1617 1819 0a25 1a44  .............%.D
+00001600: 0908 1001 0823 4028 0000 0000 0000 546e  .....#@(......Tn
+00001610: 616d 6509 0008 0019 0022 0034 003c 0050  ame......".4.<.P
+00001620: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
+00001630: 00c1 00cd 00d2 00d8 00dd 00e5 00ea 00f7  ................
+00001640: 0100 0108 010e 0118 011e 011f 0122 0123  .............".#
+00001650: 0125 012e 012f 0131 0132 0134 013d 013e  .%.../.1.2.4.=.>
+00001660: 0140 0141 0143 014c 014d 014f 0150 0152  .@.A.C.L.M.O.P.R
+00001670: 015b 015c 015e 015f 0161 016a 016b 016d  .[.\.^._.a.j.k.m
+00001680: 016e 0170 0179 017a 017c 017d 017f 0188  .n.p.y.z.|.}....
+00001690: 0189 018c 018d 018f 0198 0199 019a 019c  ................
+000016a0: 019d 01a6 01ab 0000 0000 0000 0201 0000  ................
+000016b0: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+000016c0: 0000 0000 01ac 0000 0003 0063 006c 0069  ...........c.l.i
+000016d0: 6d6f 4444 626c 6f62 0000 0008 b9da e924  moDDblob.......$
+000016e0: ef2c c541 0000 0003 0063 006c 0069 6d6f  .,.A.....c.l.imo
+000016f0: 6444 626c 6f62 0000 0008 b9da e924 ef2c  dDblob.......$.,
+00001700: c541 0000 0003 0063 006c 0069 7068 3153  .A.....c.l.iph1S
+00001710: 636f 6d70 0000 0000 0000 7000 0000 0003  comp......p.....
+00001720: 0063 006c 0069 7653 726e 6c6f 6e67 0000  .c.l.ivSrnlong..
+00001730: 0001 0000 0009 0065 0072 0072 006f 0072  .......e.r.r.o.r
+00001740: 0073 002e 0070 0079 7074 624c 7573 7472  .s...p.yptbLustr
+00001750: 0000 003d 0053 0079 0073 0074 0065 006d  ...=.S.y.s.t.e.m
+00001760: 002f 0056 006f 006c 0075 006d 0065 0073  ./.V.o.l.u.m.e.s
+00001770: 002f 0044 0061 0074 0061 002f 0055 0073  ./.D.a.t.a./.U.s
+00001780: 0065 0072 0073 002f 0073 0069 006d 006f  .e.r.s./.s.i.m.o
+00001790: 006e 002f 0044 0065 0073 006b 0074 006f  .n./.D.e.s.k.t.o
+000017a0: 0070 002f 0065 006e 0076 0073 002f 0073  .p./.e.n.v.s./.s
+000017b0: 0069 006d 0062 0061 005f 0064 0065 0076  .i.m.b.a._.d.e.v
+000017c0: 002f 0073 0069 006d 0062 0061 002f 0000  ./.s.i.m.b.a./..
+000017d0: 0009 0065 0072 0072 006f 0072 0073 002e  ...e.r.r.o.r.s..
+000017e0: 0070 0079 7074 624e 7573 7472 0000 000b  .p.yptbNustr....
+000017f0: 0077 0061 0072 006e 0069 006e 0067 0073  .w.a.r.n.i.n.g.s
+00001800: 002e 0070 0079 0000 0000 0000 0000 0000  ...p.y..........
+00001810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0073 696f 6e23 4030 0000 0000 0000 09d9  .sion#@0........
-00002510: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
-00002520: 3c41 5863 6f6d 6d65 6e74 735e 6461 7465  <AXcomments^date
-00002530: 4c61 7374 4f70 656e 6564 5b64 6174 6543  LastOpened[dateC
-00002540: 7265 6174 6564 5473 697a 6555 6c61 6265  reatedTsizeUlabe
-00002550: 6c54 6b69 6e64 5776 6572 7369 6f6e 546e  lTkindWversionTn
-00002560: 616d 655c 6461 7465 4d6f 6469 6669 6564  ame\dateModified
-00002570: d416 1718 191a 1b0a 1d57 7669 7369 626c  .........Wvisibl
-00002580: 6555 7769 6474 6859 6173 6365 6e64 696e  eUwidthYascendin
-00002590: 6755 696e 6465 7808 1101 2c09 1007 d416  gUindex...,.....
-000025a0: 1718 191a 201a 2208 10c8 0810 08d4 1617  .... .".........
-000025b0: 1819 1a25 1a27 0810 b508 1002 d416 1718  ...%.'..........
-000025c0: 190a 2a1a 2c09 1061 0810 03d4 1617 1819  ..*.,..a........
-000025d0: 1a2f 0a31 0810 6409 1005 d416 1718 190a  ./.1..d.........
-000025e0: 340a 3609 1073 0910 04d4 1617 1819 1a39  4.6..s.........9
-000025f0: 0a3b 0810 4b09 1006 d416 1718 190a 3e0a  .;..K.........>.
-00002600: 4009 1101 c709 1000 d416 1718 190a 251a  @.............%.
-00002610: 4409 0810 0108 2340 2800 0000 0000 0054  D.....#@(......T
-00002620: 6e61 6d65 0900 0800 1900 2200 3400 3c00  name......".4.<.
-00002630: 5000 5900 6400 7700 8c00 9500 9600 a900  P.Y.d.w.........
-00002640: b200 c100 cd00 d200 d800 dd00 e500 ea00  ................
-00002650: f701 0001 0801 0e01 1801 1e01 1f01 2201  ..............".
-00002660: 2301 2501 2e01 2f01 3101 3201 3401 3d01  #.%.../.1.2.4.=.
-00002670: 3e01 4001 4101 4301 4c01 4d01 4f01 5001  >.@.A.C.L.M.O.P.
-00002680: 5201 5b01 5c01 5e01 5f01 6101 6a01 6b01  R.[.\.^._.a.j.k.
-00002690: 6d01 6e01 7001 7901 7a01 7c01 7d01 7f01  m.n.p.y.z.|.}...
-000026a0: 8801 8901 8c01 8d01 8f01 9801 9901 9a01  ................
-000026b0: 9c01 9d01 a601 ab00 0000 0000 0002 0100  ................
-000026c0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
-000026d0: 0000 0000 0001 ac00 0000 0300 6300 6c00  ............c.l.
-000026e0: 696d 6f44 4462 6c6f 6200 0000 0834 2b08  imoDDblob....4+.
-000026f0: c0c8 11c5 4100 0000 0300 6300 6c00 696d  ....A.....c.l.im
-00002700: 6f64 4462 6c6f 6200 0000 0834 2b08 c0c8  odDblob....4+...
-00002710: 11c5 4100 0000 0300 6300 6c00 6970 6831  ..A.....c.l.iph1
-00002720: 5363 6f6d 7000 0000 0000 0040 0000 0000  Scomp......@....
-00002730: 0300 6300 6c00 6976 5372 6e6c 6f6e 6700  ..c.l.ivSrnlong.
-00002740: 0000 0100 0000 0900 6500 7200 7200 6f00  ........e.r.r.o.
-00002750: 7200 7300 2e00 7000 7970 7462 4c75 7374  r.s...p.yptbLust
-00002760: 7200 0000 3d00 5300 7900 7300 7400 6500  r...=.S.y.s.t.e.
-00002770: 6d00 2f00 5600 6f00 6c00 7500 6d00 6500  m./.V.o.l.u.m.e.
-00002780: 7300 2f00 4400 6100 7400 6100 2f00 5500  s./.D.a.t.a./.U.
-00002790: 7300 6500 7200 7300 2f00 7300 6900 6d00  s.e.r.s./.s.i.m.
-000027a0: 6f00 6e00 2f00 4400 6500 7300 6b00 7400  o.n./.D.e.s.k.t.
-000027b0: 6f00 7000 2f00 6500 6e00 7600 7300 2f00  o.p./.e.n.v.s./.
-000027c0: 7300 6900 6d00 6200 6100 5f00 6400 6500  s.i.m.b.a._.d.e.
-000027d0: 7600 2f00 7300 6900 6d00 6200 6100 2f00  v./.s.i.m.b.a./.
-000027e0: 0000 0900 6500 7200 7200 6f00 7200 7300  ....e.r.r.o.r.s.
-000027f0: 2e00 7000 7970 7462 4e75 7374 7200 0000  ..p.yptbNustr...
-00002800: 0b00 7700                                ..w.
+00002500: 000e 0f10 1112 1314 151e 2328 2d32 373c  ..........#(-27<
+00002510: 4158 636f 6d6d 656e 7473 5e64 6174 654c  AXcomments^dateL
+00002520: 6173 744f 7065 6e65 645b 6461 7465 4372  astOpened[dateCr
+00002530: 6561 7465 6454 7369 7a65 556c 6162 656c  eatedTsizeUlabel
+00002540: 546b 696e 6457 7665 7273 696f 6e54 6e61  TkindWversionTna
+00002550: 6d65 5c64 6174 654d 6f64 6966 6965 64d4  me\dateModified.
+00002560: 1617 1819 1a1b 0a1d 5776 6973 6962 6c65  ........Wvisible
+00002570: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
+00002580: 5569 6e64 6578 0811 012c 0910 07d4 1617  Uindex...,......
+00002590: 1819 1a20 1a22 0810 c808 1008 d416 1718  ... ."..........
+000025a0: 191a 251a 2708 10b5 0810 02d4 1617 1819  ..%.'...........
+000025b0: 0a2a 1a2c 0910 6108 1003 d416 1718 191a  .*.,..a.........
+000025c0: 2f0a 3108 1064 0910 05d4 1617 1819 0a34  /.1..d.........4
+000025d0: 0a36 0910 7309 1004 d416 1718 191a 390a  .6..s.........9.
+000025e0: 3b08 104b 0910 06d4 1617 1819 0a3e 0a40  ;..K.........>.@
+000025f0: 0911 01c7 0910 00d4 1617 1819 0a25 1a44  .............%.D
+00002600: 0908 1001 0823 4028 0000 0000 0000 546e  .....#@(......Tn
+00002610: 616d 6509 0008 0019 0022 0034 003c 0050  ame......".4.<.P
+00002620: 0059 0064 0077 008c 0095 0096 00a9 00b2  .Y.d.w..........
+00002630: 00c1 00cd 00d2 00d8 00dd 00e5 00ea 00f7  ................
+00002640: 0100 0108 010e 0118 011e 011f 0122 0123  .............".#
+00002650: 0125 012e 012f 0131 0132 0134 013d 013e  .%.../.1.2.4.=.>
+00002660: 0140 0141 0143 014c 014d 014f 0150 0152  .@.A.C.L.M.O.P.R
+00002670: 015b 015c 015e 015f 0161 016a 016b 016d  .[.\.^._.a.j.k.m
+00002680: 016e 0170 0179 017a 017c 017d 017f 0188  .n.p.y.z.|.}....
+00002690: 0189 018c 018d 018f 0198 0199 019a 019c  ................
+000026a0: 019d 01a6 01ab 0000 0000 0000 0201 0000  ................
+000026b0: 0000 0000 0049 0000 0000 0000 0000 0000  .....I..........
+000026c0: 0000 0000 01ac 0000 0003 0063 006c 0069  ...........c.l.i
+000026d0: 6d6f 4444 626c 6f62 0000 0008 b9da e924  moDDblob.......$
+000026e0: ef2c c541 0000 0003 0063 006c 0069 6d6f  .,.A.....c.l.imo
+000026f0: 6444 626c 6f62 0000 0008 b9da e924 ef2c  dDblob.......$.,
+00002700: c541 0000 0003 0063 006c 0069 7068 3153  .A.....c.l.iph1S
+00002710: 636f 6d70 0000 0000 0000 7000 0000 0003  comp......p.....
+00002720: 0063 006c 0069 7653 726e 6c6f 6e67 0000  .c.l.ivSrnlong..
+00002730: 0001 0000 0009 0065 0072 0072 006f 0072  .......e.r.r.o.r
+00002740: 0073 002e 0070 0079 7074 624c 7573 7472  .s...p.yptbLustr
+00002750: 0000 003d 0053 0079 0073 0074 0065 006d  ...=.S.y.s.t.e.m
+00002760: 002f 0056 006f 006c 0075 006d 0065 0073  ./.V.o.l.u.m.e.s
+00002770: 002f 0044 0061 0074 0061 002f 0055 0073  ./.D.a.t.a./.U.s
+00002780: 0065 0072 0073 002f 0073 0069 006d 006f  .e.r.s./.s.i.m.o
+00002790: 006e 002f 0044 0065 0073 006b 0074 006f  .n./.D.e.s.k.t.o
+000027a0: 0070 002f 0065 006e 0076 0073 002f 0073  .p./.e.n.v.s./.s
+000027b0: 0069 006d 0062 0061 005f 0064 0065 0076  .i.m.b.a._.d.e.v
+000027c0: 002f 0073 0069 006d 0062 0061 002f 0000  ./.s.i.m.b.a./..
+000027d0: 0009 0065 0072 0072 006f 0072 0073 002e  ...e.r.r.o.r.s..
+000027e0: 0070 0079 7074 624e 7573 7472 0000 000b  .p.yptbNustr....
+000027f0: 0077 0061 0072 006e 0069 006e 0067 0073  .w.a.r.n.i.n.g.s
+00002800: 002e 0070                                ...p
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/checks.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/checks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 __author__ = "Simon Nilsson"
 """
 @authors: Xiaoyu Tong, Jia Jie Choong, Simon Nilsson
 """
+
+
 import os
 import trafaret as t
 import pandas as pd
 from typing import Any, Optional, Tuple, List, Union
 import subprocess
 import re
 
@@ -48,14 +50,17 @@
     :param Any value: Value of variable
     :param Optional[int] max_value: Maximum allowed value of the variable. If None, then no maximum. Default: None.
     :param Optional[int]: Minimum allowed value of the variable. If None, then no minimum. Default: None.
     :param Optional[bool] raise_error: If True, then raise error if invalid integer. Default: True.
 
     :return bool: False if invalid. True if valid.
     :return str: If invalid, then error msg. Else empty str.
+
+    :examples:
+    >>> check_int(name='My_fps', input=25, min_value=1)
     """
     msg = ''
     try:
         t.Int().check(value)
     except t.DataError as e:
         msg=f'{name} should be an integer number in SimBA, but is set to {str(value)}'
         if raise_error:
@@ -91,14 +96,17 @@
     :param Any value: Value of variable
     :param Optional[Tuple[Any]] options: Tuple of allowed strings. If empty tuple, then any string allowed. Default: ().
     :param Optional[bool] allow_blank: If True, allow empty string. Default: False.
     :param Optional[bool] raise_error: If True, then raise error if invalid string. Default: True.
 
     :return bool: False if invalid. True if valid.
     :return str: If invalid, then error msg. Else empty str.
+
+    :examples:
+    >>> check_str(name='split_eval', input='gini', options=['entropy', 'gini'])
     """
 
     msg = ''
     try:
         t.String(allow_blank=allow_blank).check(value)
     except t.DataError as e:
         msg = f'{name} should be an string in SimBA, but is set to {str(value)}'
@@ -131,14 +139,17 @@
     :param Any value: Value of variable
     :param Optional[int] max_value: Maximum allowed value of the float. If None, then no maximum. Default: None.
     :param Optional[int]: Minimum allowed value of the float. If None, then no minimum. Default: None.
     :param Optional[bool] raise_error: If True, then raise error if invalid float. Default: True.
 
     :return bool: False if invalid. True if valid.
     :return str: If invalid, then error msg. Else empty str.
+
+    :examples:
+    >>> check_float(name='My_float', value=0.5, max_value=1.0, min_value=0.0)
     """
 
 
     msg = ''
     try:
         t.Float().check(value)
     except t.DataError as e:
@@ -186,44 +197,47 @@
 
     :param str in_dir: Putative directory path.
     :raise NotDirectoryError: The directory does not exist.
     """
     if not os.path.isdir(in_dir):
         raise NotDirectoryError(msg=f'{in_dir} is not a valid directory')
 
-
 def check_that_column_exist(df: pd.DataFrame,
                             column_name: str,
                             file_name: str) -> None:
     """
     Check if single named field exist within a dataframe.
 
     :param pd.DataFrame df:
     :param str column_name: Name of putative field.
     :param str file_name: Path of ``df`` on disk.
-    :raise ColumnNotFoundError: The  ``column_name`` does not exist within ``df``.
+    :raise ColumnNotFoundError: The ``column_name`` does not exist within ``df``.
     """
 
     if column_name not in df.columns:
         raise ColumnNotFoundError(column_name=column_name, file_name=file_name)
 
 def check_if_valid_input(name: str,
                          input: str,
                          options: List[str],
                          raise_error: bool = True) -> (bool, str):
     """
     Check if string variable is valid option
 
-    :param str name: Name of variable
-    :param Any input: Value of variable
+    :param str name: Atrbitrary name of variable.
+    :param Any input: Value of variable.
     :param List[str] options: Allowed options of ``input``
     :param Optional[bool] raise_error: If True, then raise error if invalid value. Default: True.
 
     :return bool: False if invalid. True if valid.
-    :return str: If invalid, then error msg. Else empty str.
+    :return str: If invalid, then error msg. Else, empty str.
+
+    :example:
+    >>> check_if_valid_input(name='split_eval', input='gini', options=['entropy', 'gini'])
+    >>> (True, '')
     """
 
     msg = ''
     if input not in options:
         msg = f'{name} is set to {str(input)}, which is an invalid setting. OPTIONS {options}'
         if raise_error:
             raise InvalidInputError(msg=msg)
@@ -235,15 +249,15 @@
 
 
 def check_minimum_roll_windows(roll_windows_values: List[int],
                                minimum_fps: float) -> List[int]:
 
     """
     Remove any rolling temporal window that are shorter than a single frame in
-    any of the videos in the project.
+    any of the videos within the project.
 
     :param List[int] roll_windows_values: Rolling temporal windows represented as frame counts. E.g., [10, 15, 30, 60]
     :param float minimum_fps: The lowest fps of the videos that are to be analyzed. E.g., 10.
 
     :return List[int]: roll_windows_values without impassable windows.
     """
 
@@ -254,19 +268,26 @@
             pass
     roll_windows_values = list(set(roll_windows_values))
     return roll_windows_values
 
 
 def check_same_number_of_rows_in_dfs(dfs: List[pd.DataFrame]) -> bool:
     """
-    Helper to check if dataframes contains an equal number of rows
+    Helper to check that each dataframe in list contains an equal number of rows
 
     :param List[pd.DataFrame] dfs: List of dataframes.
     :return bool: True if dataframes has an equal number of rows. Else False.
+
+    >>> df_1, df_2 = pd.DataFrame([[1, 2], [1, 2]]), pd.DataFrame([[4, 2], [9, 3], [1, 5]])
+    >>> check_same_number_of_rows_in_dfs(dfs=[df_1, df_2])
+    >>> False
+    >>> df_1, df_2 = pd.DataFrame([[1, 2], [1, 2]]), pd.DataFrame([[4, 2], [9, 3]])
+    >>> True
     """
+
     row_cnt = None
     for df_cnt, df in enumerate(dfs):
         if df_cnt == 0:
             row_cnt = len(df)
         else:
             if len(df) != row_cnt:
                 return False
@@ -274,46 +295,83 @@
 
 def check_if_headers_in_dfs_are_unique(dfs: List[pd.DataFrame]) -> List[str]:
     """
     Helper to check heaaders in multiple dataframes are unique.
 
     :param List[pd.DataFrame] dfs: List of dataframes.
     :return List[str]: List of columns headers seen in multiple dataframes. Empty if None.
+
+    :examples:
+    >>> df_1, df_2 = pd.DataFrame([[1, 2]], columns=['My_column_1', 'My_column_2']), pd.DataFrame([[4, 2]], columns=['My_column_3', 'My_column_1'])
+    >>> check_if_headers_in_dfs_are_unique(dfs=[df_1, df_2])
+    >>> ['My_column_1']
     """
     seen_headers = []
     for df_cnt, df in enumerate(dfs):
         seen_headers.extend(list(df.columns))
     duplicates = list(set([x for x in seen_headers if seen_headers.count(x) > 1]))
     return duplicates
 
+def check_if_string_value_is_valid_video_timestamp(value: str, name: str) -> None:
+    """
+    Helper to check if a string is in a valid HH:MM:SS format
+
+    :param str value: Timestamp in HH:MM:SS format.
+    :param str name: An arbitrary string name of the timestamp.
+    :raises InvalidInputError: If the timestamp is in invalid format
 
-def check_if_string_value_is_valid_video_timestamp(value: str, name: str):
-    """ Helper to check if a string is in a valid HH:MM:SS format"""
+    :example:
+    >>> check_if_string_value_is_valid_video_timestamp(value='00:0b:10', name='My time stamp')
+    >>> "InvalidInputError: My time stamp is should be in the format XX:XX:XX where X is an integer between 0-9"
+    """
     r = re.compile('.{2}:.{2}:.{2}')
     if (len(value) != 8) or (not r.match(value)) or (re.search('[a-zA-Z]', value)):
         raise InvalidInputError(msg=f'{name} is should be in the format XX:XX:XX where X is an integer between 0-9')
 
-def check_that_hhmmss_start_is_before_end(start_time: str, end_time: str, name: str):
-    """Helper to check that a start time in HH:MM:SS format is before an endtime in HH:MM:SS format"""
+def check_that_hhmmss_start_is_before_end(start_time: str,
+                                          end_time: str,
+                                          name: str) -> None:
+    """
+    Helper to check that a start time in HH:MM:SS format is before an end time in HH:MM:SS format
+
+    :param str start_time: Period start time in HH:MM:SS format.
+    :param str end_time: Period end time in HH:MM:SS format.
+    :param int name: Name of the variable
+    :raises InvalidInputError: If end time is before the start time.
+
+    :example:
+    >>> check_that_hhmmss_start_is_before_end(start_time='00:00:05', end_time='00:00:01', name='My time period')
+    >>> "InvalidInputError: My time period has an end-time which is before the start-time"
+    >>> check_that_hhmmss_start_is_before_end(start_time='00:00:01', end_time='00:00:05')
+    """
     start_h, start_m, start_s = start_time.split(':')
     end_h, end_m, end_s = end_time.split(':')
     start_in_s = int(start_h) * 3600 + int(start_m) * 60 + int(start_s)
     end_in_s = int(end_h) * 3600 + int(end_m) * 60 + int(end_s)
     if end_in_s < start_in_s:
-        raise InvalidInputError(f'{name} has has an end-time which is before the start-time.')
+        raise InvalidInputError(f'{name} has an end-time which is before the start-time.')
 
 def check_nvidea_gpu_available() -> bool:
-    """ Helper to check of NVIDEA GPU is available"""
+    """
+    Helper to check of NVIDEA GPU is available via ``nvidia-smi``.
+    returns bool: True if nvidia-smi returns not None. Else False.
+    """
     try:
         subprocess.check_output('nvidia-smi')
         return True
     except Exception:
         return False
 
 
 def check_ffmpeg_available() -> bool:
-    """ Helper to check of FFMpeg is available"""
+    """
+    Helper to check of FFMpeg is available via subprocess ``ffmpeg``.
+
+    returns bool: True if ``ffmpeg`` returns not None. Else False.
+    """
     try:
         subprocess.call('ffmpeg', stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
         return True
     except Exception:
-        return False
+        return False
+
+
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/read_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,36 +12,38 @@
 import pickle
 import cv2
 from pyarrow import csv
 import os
 from pathlib import Path
 import multiprocessing
 from typing import List, Optional, Any, Union, Tuple, Dict
-
+from datetime import timedelta
 
 from simba.utils.printing import SimbaTimer
 
 
 from simba.utils.errors import (InvalidFileTypeError,
                                 MissingProjectConfigEntryError,
                                 NotDirectoryError,
                                 InvalidInputError,
                                 ParametersFileError,
                                 InvalidFilepathError,
                                 InvalidVideoFileError,
                                 DuplicationError,
                                 NoFilesFoundError,
                                 DataHeaderError,
-                                FileExistError)
+                                FileExistError,
+                                FrameRangeError)
 from simba.utils.warnings import InvalidValueWarning, NoFileFoundWarning, FileExistWarning
 from simba.utils.printing import stdout_success
 from simba.utils.enums import Formats, Dtypes, ConfigKey
 from simba.utils.checks import (check_file_exist_and_readable,
                                 check_if_filepath_list_is_empty,
-                                check_nvidea_gpu_available)
+                                check_nvidea_gpu_available,
+                                check_if_string_value_is_valid_video_timestamp)
 
 PARSE_OPTIONS = csv.ParseOptions(delimiter=',')
 READ_OPTIONS = csv.ReadOptions(encoding='utf8')
 
 def read_df(file_path: Union[str, os.PathLike],
             file_type: Union[str, os.PathLike],
             has_index: Optional[bool] = True,
@@ -325,15 +327,15 @@
     _, video_data['video_name'], _ = get_fn_ext(video_path)
     video_data['fps'] = int(cap.get(cv2.CAP_PROP_FPS))
     video_data['width'] = int(cap.get(cv2.CAP_PROP_FRAME_WIDTH))
     video_data['height'] = int(cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
     video_data['frame_count'] = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
     for k, v in video_data.items():
         if v == 0:
-            raise InvalidVideoFileError(msg=f'SIMBA WARNING: Video {video_data["video_name"]} has {k} of {str(v)} (full error video path: {video_path}).')
+            raise InvalidVideoFileError(msg=f'Video {video_data["video_name"]} has {k} of {str(v)} (full error video path: {video_path}).')
     video_data['resolution_str'] = str(f'{video_data["width"]} x {video_data["height"]}')
     video_data['video_length_s'] = int(video_data['frame_count'] / video_data['fps'])
     return video_data
 
 def remove_a_folder(folder_dir: Union[str, os.PathLike]) -> None:
     """Helper to remove a directory"""
     shutil.rmtree(folder_dir, ignore_errors=True)
@@ -942,7 +944,32 @@
                 video_paths.append(file_path)
             else:
                 video_paths.append(file_name)
     if len(video_paths) == 0:
         raise NoFilesFoundError(msg=f'No videos in mp4 or avi format found imported to SimBA project in the {videos_dir} directory')
     else:
         return video_paths
+
+
+def check_if_hhmmss_timestamp_is_valid_part_of_video(timestamp: str,
+                                                     video_path: Union[str, os.PathLike]) -> None:
+    """
+    Helper to check that a timestamp in HH:MM:SS format occurs in a video file.
+
+    :param str timestamp: Timestamp in HH:MM:SS format.
+    :param str video_path: Path to a video file.
+    :raises FrameRangeError: If timestamp is not in the video file
+
+    :example:
+    >>> check_if_hhmmss_timestamp_is_valid_part_of_video(timestamp='01:00:05', video_path='/Users/simon/Desktop/video_tests/Together_1.avi')
+    >>> "InvalidInputError: My time period has an end-time which is before the start-time"
+     """
+
+    check_file_exist_and_readable(file_path=video_path)
+    check_if_string_value_is_valid_video_timestamp(value=timestamp, name='Timestamp')
+    video_meta_data = get_video_meta_data(video_path=video_path)
+    h, m, s = timestamp.split(':')
+    time_stamp_in_seconds = int(h) * 3600 + int(m) * 60 + int(s)
+    if not video_meta_data['video_length_s'] >= time_stamp_in_seconds:
+        video_length_str = timedelta(seconds=video_meta_data['video_length_s'])
+        raise FrameRangeError(msg=f'The timestamp {timestamp} does not occur in video {video_meta_data["video_name"]}, the video has length {video_length_str}')
+
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/errors.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/data.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,8 +442,8 @@
     user_class = getattr(user_module, class_name)
     print(f'Running user-defined {class_name} feature extraction file...')
     user_class(config_path=config_path)
 
 
 # config = read_config_file(config_path='/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/project_config.ini')
 # smooth_data_savitzky_golay(config=config,file_path='/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/csv/input_csv/Together_1.csv', time_window_parameter=500, overwrite=False)
-find_frame_numbers_from_time_stamp(start_time='00:00:00', end_time='00:00:01', fps=20)
+#find_frame_numbers_from_time_stamp(start_time='00:00:00', end_time='00:00:01', fps=20)
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/utils/printing.py` & `Simba-UW-tf-dev-1.65.1/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/st/select_groups_pg.py` & `Simba-UW-tf-dev-1.65.1/simba/st/select_groups_pg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/st/aggregate_statistics.py` & `Simba-UW-tf-dev-1.65.1/simba/st/aggregate_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/st/app.py` & `Simba-UW-tf-dev-1.65.1/simba/st/app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_processors/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/mixins/.DS_Store`

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
-00000130: 0000 0000 a209 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 000c 037a 0000 000b 005f 005f 0070  .....z....._._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 beac 8729  moDDblob.......)
-00000160: 7b20 c541 0000 000b 005f 005f 0070 0079  { .A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 f515 c39f  moDDblob........
+00000160: e32c c541 0000 000b 005f 005f 0070 0079  .,.A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 beac 8729 7b20  dDblob.......){ 
+00000180: 6444 626c 6f62 0000 0008 f515 c39f e32c  dDblob.........,
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0001 4000 0000 0000  comp......@.....
+000001b0: 636f 6d70 0000 0000 000d 1000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/plotting/.DS_Store`

 * *Files 22% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0008 0000 000b  ................
 00000210: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000220: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000230: 0000 000a 5a7d 0000 000b 005f 005f 0070  ....Z}....._._.p
+00000230: 0000 000a 65a8 0000 000b 005f 005f 0070  ....e......_._.p
 00000240: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000250: 6d6f 4444 626c 6f62 0000 0008 71e6 4321  moDDblob....q.C!
-00000260: 1721 c541 0000 000b 005f 005f 0070 0079  .!.A....._._.p.y
+00000250: 6d6f 4444 626c 6f62 0000 0008 269e 8b35  moDDblob....&..5
+00000260: e32c c541 0000 000b 005f 005f 0070 0079  .,.A....._._.p.y
 00000270: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000280: 6444 626c 6f62 0000 0008 71e6 4321 1721  dDblob....q.C!.!
+00000280: 6444 626c 6f62 0000 0008 269e 8b35 e32c  dDblob....&..5.,
 00000290: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000002a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000002b0: 636f 6d70 0000 0000 000d 7000 0000 0005  comp......p.....
+000002b0: 636f 6d70 0000 0000 000d 8000 0000 0005  comp............
 000002c0: 0074 006f 006f 006c 0073 6c67 3153 636f  .t.o.o.l.slg1Sco
 000002d0: 6d70 0000 0000 0000 50f8 0000 0005 0074  mp......P......t
 000002e0: 006f 006f 006c 0073 6d6f 4444 626c 6f62  .o.o.l.smoDDblob
 000002f0: 0000 0008 1e86 d77f cc0c c541 0000 0005  ...........A....
 00000300: 0074 006f 006f 006c 0073 6d6f 6444 626c  .t.o.o.l.smodDbl
 00000310: 6f62 0000 0008 1e86 d77f cc0c c541 0000  ob...........A..
 00000320: 0005 0074 006f 006f 006c 0073 7068 3153  ...t.o.o.l.sph1S
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.65.1/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.65.1/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.65.1/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.65.1/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.DS_Store`

 * *Files 12% similar despite different names*

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
-00000130: 0000 0004 7300 0000 000b 005f 005f 0070  ....s......_._.p
-00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 41ed 4121  moDDblob....A.A!
-00000160: 1721 c541 0000 000b 005f 005f 0070 0079  .!.A....._._.p.y
-00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 41ed 4121 1721  dDblob....A.A!.!
-00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0005 f000 0000 0000  comp............
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
+000002b0: 0000 0000 73e1 0000 000b 005f 005f 0070  ....s......_._.p
+000002c0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+000002d0: 6d6f 4444 626c 6f62 0000 0008 b6b0 7cbf  moDDblob......|.
+000002e0: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+000002f0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00000300: 6444 626c 6f62 0000 0008 b6b0 7cbf 1b1f  dDblob......|...
+00000310: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+00000320: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+00000330: 636f 6d70 0000 0000 0000 c000 0000 0000  comp............
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

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.65.1/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.65.1/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.65.1/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.65.1/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.65.1/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.65.1/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.65.1/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/ui/define_px_to_mm_ui.py` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/ui/define_px_to_mm_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/feature_extractors/generic_feature_extractor.py` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/feature_extractors/generic_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/config_reader.py` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/pose_importers/anipose_csv_import.py` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/pose_importers/anipose_csv_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.65.1/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/video_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,24 @@
 import multiprocessing
 from typing import List, Union, Optional
 
 from simba.utils.checks import (check_file_exist_and_readable,
                                 check_int,
                                 check_if_filepath_list_is_empty,
                                 check_nvidea_gpu_available,
-                                check_ffmpeg_available)
+                                check_ffmpeg_available,
+                                check_if_string_value_is_valid_video_timestamp,
+                                check_that_hhmmss_start_is_before_end)
 from simba.utils.read_write import (get_fn_ext,
                                     get_video_meta_data,
                                     find_all_videos_in_directory,
                                     find_core_cnt,
                                     read_config_entry,
                                     read_config_file)
+from simba.utils.read_write import check_if_hhmmss_timestamp_is_valid_part_of_video
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.video_processors.extract_frames import video_to_frames
 from simba.utils.enums import Formats, Paths, ConfigKey
 
 from simba.utils.errors import (NotDirectoryError,
                                 NoFilesFoundError,
                                 FileExistError,
@@ -417,14 +420,17 @@
     """
 
     if gpu and not check_nvidea_gpu_available():
         raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
     timer = SimbaTimer(start=True)
     check_file_exist_and_readable(file_path=file_path)
     dir, file_name, ext = get_fn_ext(filepath=file_path)
+    check_if_string_value_is_valid_video_timestamp(value=start_time, name='START TIME')
+    check_if_string_value_is_valid_video_timestamp(value=end_time, name='END TIME')
+    check_that_hhmmss_start_is_before_end(start_time=start_time, end_time=end_time, name=f'{file_name} timestamps')
     save_name = os.path.join(dir, file_name + '_clipped.mp4')
     if os.path.isfile(save_name):
         raise FileExistError(msg='SIMBA ERROR: The outfile file already exist: {}.'.format(save_name))
     if gpu:
         command = 'ffmpeg -hwaccel auto -c:v h264_cuvid -i "{}" -ss {} -to {} -async 1 "{}"'.format(file_path, start_time, end_time, save_name)
     else:
         command = (str('ffmpeg -i ') + '"' + str(file_path) + '"' + ' -ss ' + str(start_time) + ' -to ' + str(end_time) + ' -async 1 ' + '"' + save_name + '"')
@@ -631,48 +637,37 @@
     >>> _ = multi_split_video(file_path='project_folder/videos/Video_1.mp4', start_times=['00:00:05', '00:00:20'], end_times=['00:00:10', '00:00:25'])
     """
 
     timer = SimbaTimer(start=True)
     check_file_exist_and_readable(file_path=file_path)
     video_meta_data = get_video_meta_data(file_path)
     dir_name, file_name, ext = get_fn_ext(filepath=file_path)
-    r = re.compile('.{2}:.{2}:.{2}')
     for start_time_cnt, start_time in enumerate(start_times):
-        if (len(start_time) != 8) or (not r.match(start_time)) or (re.search('[a-zA-Z]', start_time)):
-            raise InvalidInputError(msg=f'Start time for clip {str(start_time_cnt+1)} is should be in the format XX:XX:XX where X is an integer between 0-9')
+        check_if_string_value_is_valid_video_timestamp(value=start_time, name=f'Start time for clip {start_time_cnt+1}')
     for end_time_cnt, end_time in enumerate(end_times):
-        if (len(end_time) != 8) or (not r.match(end_time)) or (re.search('[a-zA-Z]', end_time)):
-            raise InvalidInputError(msg=f'End time for clip {str(end_time_cnt+1)} is should be in the format XX:XX:XX where X is an integer between 0-9')
+        check_if_string_value_is_valid_video_timestamp(value=end_time, name=f'End time for clip {end_time_cnt+1}')
     for clip_cnt, (start_time, end_time) in enumerate(zip(start_times, end_times)):
-        start_h, start_m, start_s = start_time.split(':')
-        end_h, end_m, end_s = end_time.split(':')
-        start_in_s = int(start_h) * 3600 + int(start_m) * 60 + int(start_s)
-        end_in_s = int(end_h) * 3600 + int(end_m) * 60 + int(end_s)
-        if end_in_s < start_in_s:
-            raise InvalidInputError(f'Clip {str(clip_cnt+1)} has has an end-time which is before the start-time.')
-        if end_in_s == start_in_s:
-            raise InvalidInputError(msg=f'Clip {str(clip_cnt+1)} has the same start time and end time.')
-        if end_in_s > video_meta_data['video_length_s']:
-            raise InvalidInputError(f'Clip {str(clip_cnt + 1)} has end time at {str(end_in_s)} seconds into the video, which is greater then the lenth of the video ({str(video_meta_data["video_length_s"])}s).')
+        check_that_hhmmss_start_is_before_end(start_time=start_time, end_time=end_time, name=f'Clip {str(clip_cnt+1)}')
+        check_if_hhmmss_timestamp_is_valid_part_of_video(timestamp=start_time, video_path=file_path)
+        check_if_hhmmss_timestamp_is_valid_part_of_video(timestamp=end_time, video_path=file_path)
         save_path = os.path.join(dir_name, file_name + '_{}'.format(str(clip_cnt+1)) + '.mp4')
         if os.path.isfile(save_path):
             raise FileExistError(msg=f'The outfile file already exist: {save_path}.')
         if gpu:
             if not check_nvidea_gpu_available():
                 raise FFMPEGCodecGPUError(msg='NVIDEA GPU not available (as evaluated by nvidea-smi returning None')
             command = 'ffmpeg -hwaccel auto -i "{}" -ss {} -to {} -c:v h264_nvenc -async 1 "{}"'.format(file_path, start_time, end_time, save_path)
         else:
             command = (str('ffmpeg -i ') + '"' + file_path + '"' + ' -ss ' + start_time + ' -to ' + end_time + ' -async 1 ' + '"' + save_path + '"')
         print('Processing video clip {}...'.format(str(clip_cnt+1)))
         subprocess.call(command, shell=True, stdout=subprocess.PIPE)
     timer.stop_timer()
     stdout_success(msg=f'Video {file_name} converted into {str(len(start_times))} clips in directory {dir_name}!', elapsed_time=timer.elapsed_time_str)
 
-#multi_split_video(file_path=r'C:\Users\Nape_Computer_2\Desktop\test_videos\Box1_PM2_day_5_20211104T171021.mp4', start_times=['00:00:05', '00:00:05'], end_times=['00:00:55', '00:00:55'], gpu=True)
-
+#multi_split_video(file_path=r'/Users/simon/Desktop/time_s_converted.mp4', start_times=['00:00:01', '00:00:02'], end_times=['00:00:04', '00:00:05'], gpu=False)
 
 def crop_single_video(file_path: Union[str, os.PathLike],
                       gpu: Optional[bool] = False) -> None:
     """
     Crop a single video using cv2.selectROI interface. Results is saved in the same directory as input video with the
     ``_cropped.mp4`` suffix`.
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/batch_process_menus.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 from typing import Union
 
 from simba.video_processors.batch_process_create_ffmpeg_commands import FFMPEGCommandCreator
 from simba.utils.enums import Options, Keys, Links
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.errors import InvalidInputError, IntegerError, NoFilesFoundError, FFMPEGCodecGPUError
-from simba.utils.checks import check_file_exist_and_readable, check_nvidea_gpu_available
+from simba.utils.read_write import check_if_hhmmss_timestamp_is_valid_part_of_video
+from simba.utils.checks import (check_file_exist_and_readable,
+                                check_nvidea_gpu_available,
+                                check_int,
+                                check_if_string_value_is_valid_video_timestamp,
+                                check_that_hhmmss_start_is_before_end)
 from simba.utils.read_write import get_fn_ext, get_video_meta_data
 from simba.ui.tkinter_functions import CreateLabelFrameWithIcon
 
 class BatchProcessFrame(PopUpMixin):
     """
     Interactive GUI that collect user-inputs for batch processing videos (e.g., cropping,
     clipping etc.). User-selected output is stored in json file format within the user-defined `output_dir`
@@ -324,35 +329,27 @@
             json.dump(out_video_dict, fp)
         self.perform_unit_tests(out_video_dict['video_data'])
 
     def perform_unit_tests(self, out_video_dict):
         timer = SimbaTimer(start=True)
         for video_name, video_data in out_video_dict.items():
             if video_data['crop']:
-                if not isinstance(video_data['crop_settings']['width'], int):
-                    raise IntegerError(msg=f'Crop width for video {video_name} is not an integer')
-                if not isinstance(video_data['crop_settings']['height'], int):
-                    raise IntegerError(msg=f'Crop height for video {video_name} is not an integer')
+                check_int(value=video_data['crop_settings']['width'], min_value=1, name=f'Crop width for video {video_name}')
+                check_int(value=video_data['crop_settings']['height'], min_value=1, name=f'Crop height for video {video_name}')
             if video_data['clip']:
-                r = re.compile('.{2}:.{2}:.{2}')
                 for variable in ['start', 'stop']:
-                    if len(video_data['clip_settings'][variable]) != 8:
-                        raise InvalidInputError(msg=f'Clip {variable} time for video {video_name} is should be in the format XX:XX:XX where X is an integer between 0-9')
-                    elif not r.match(video_data['clip_settings'][variable]):
-                        raise InvalidInputError(msg=f'Clip {variable} time for video {video_name} is should be in the format XX:XX:XX where X is an integer between 0-9')
-                    elif re.search('[a-zA-Z]', video_data['clip_settings'][variable]):
-                        raise InvalidInputError(msg=f'Clip {variable} time for video {video_name} is should be in the format XX:XX:XX where X is an integer between 0-9')
+                    check_if_string_value_is_valid_video_timestamp(value=video_data['clip_settings'][variable], name=f'Clip {variable} time for video {video_name}')
+                check_that_hhmmss_start_is_before_end(start_time=video_data['clip_settings']['start'], end_time=video_data['clip_settings']['stop'], name=f'Clip time for video {video_name}')
+                for variable in ['start', 'stop']:
+                    check_if_hhmmss_timestamp_is_valid_part_of_video(timestamp=video_data['clip_settings'][variable], video_path=video_data['video_info']['file_path'])
             if video_data['downsample']:
-                if not isinstance(video_data['downsample_settings']['width'], int):
-                    raise IntegerError(msg=f'Downsample width for video {video_name} is not an integer')
-                if not isinstance(video_data['downsample_settings']['height'], int):
-                    raise IntegerError(msg=f'Downsample height for video {video_name} is not an integer')
+                check_int(value=video_data['downsample_settings']['width'], min_value=1, name=f'Downsample width for video {video_name}')
+                check_int(value=video_data['downsample_settings']['height'], min_value=1, name=f'Downsample height for video {video_name}')
             if video_data['fps']:
-                if not isinstance(video_data['fps_settings']['fps'], int):
-                    raise IntegerError(msg=f'FPS settings for video {video_name} is not an integer')
+                check_int(value=video_data['fps_settings']['fps'], min_value=1, name=f'FPS settings for video {video_name}')
 
         ffmpeg_runner = FFMPEGCommandCreator(json_path=self.save_path)
         ffmpeg_runner.crop_videos()
         ffmpeg_runner.clip_videos()
         ffmpeg_runner.downsample_videos()
         ffmpeg_runner.apply_fps()
         ffmpeg_runner.apply_grayscale()
```

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/video_processing_new.py` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/video_processing_new.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.65.1/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.65.1/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.65.1/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.65.1/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.65.1/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/SimBA.py` & `Simba-UW-tf-dev-1.65.1/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.65.1/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.65.1/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.65.1/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.65.1/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.65.1/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.65.1/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.65.1/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.65.1/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.65.1/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.65.1/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.65.1/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.65.1/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.65.1/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.65.1/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.65.1/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.65.1/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.65.1/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.64.9
+Version: 1.65.1
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -449,14 +449,15 @@
 simba/utils/data.py
 simba/utils/enums.py
 simba/utils/errors.py
 simba/utils/lookups.py
 simba/utils/printing.py
 simba/utils/read_write.py
 simba/utils/warnings.py
+simba/utils/cli/.DS_Store
 simba/utils/cli/__init__.py
 simba/utils/cli/cli_tools.py
 simba/video_processors/.DS_Store
 simba/video_processors/__init__.py
 simba/video_processors/batch_process_create_ffmpeg_commands.py
 simba/video_processors/batch_process_menus.py
 simba/video_processors/calculate_px_dist.py
```

### Comparing `Simba-UW-tf-dev-1.64.9/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.65.1/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/LICENSE.md` & `Simba-UW-tf-dev-1.65.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.65.1/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.65.1/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.65.1/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_pose_importers.py` & `Simba-UW-tf-dev-1.65.1/tests/test_pose_importers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.65.1/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.65.1/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.65.1/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.65.1/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.65.1/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.65.1/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.65.1/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.65.1/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.65.1/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.65.1/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.65.1/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/README.md` & `Simba-UW-tf-dev-1.65.1/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.9/setup.py` & `Simba-UW-tf-dev-1.65.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.64.9",
+    version="1.65.1",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

