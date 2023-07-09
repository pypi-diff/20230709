# Comparing `tmp/pyxy3d-0.1.6.tar.gz` & `tmp/pyxy3d-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxy3d-0.1.6.tar", max compression
+gzip compressed data, was "pyxy3d-0.1.7.tar", max compression
```

## Comparing `pyxy3d-0.1.6.tar` & `pyxy3d-0.1.7.tar`

### file list

```diff
@@ -1,65 +1,233 @@
--rw-r--r--   0        0        0    35190 2023-06-16 16:25:22.726638 pyxy3d-0.1.6/LICENSE.md
--rw-r--r--   0        0        0      964 2023-06-29 14:05:33.545092 pyxy3d-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2644 2023-06-21 16:47:49.102536 pyxy3d-0.1.6/pyxy3d/__init__.py
--rw-r--r--   0        0        0      686 2023-06-28 15:19:10.033043 pyxy3d-0.1.6/pyxy3d/__main__.py
--rw-r--r--   0        0        0    10148 2023-06-13 12:10:26.418277 pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/capture_volume.py
--rw-r--r--   0        0        0     3898 2023-05-06 23:17:45.300248 pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
--rw-r--r--   0        0        0     4680 2023-05-06 23:17:45.300248 pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
--rw-r--r--   0        0        0     4010 2023-06-28 15:19:10.033043 pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/point_estimates.py
--rw-r--r--   0        0        0    15888 2023-05-24 15:08:32.472149 pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/quality_controller.py
--rw-r--r--   0        0        0     1766 2023-05-06 23:17:45.315853 pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/seaborn_summaries.py
--rw-r--r--   0        0        0    10868 2023-05-24 15:08:32.473147 pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/set_origin_functions.py
--rw-r--r--   0        0        0     9510 2023-05-06 23:17:45.315853 pyxy3d-0.1.6/pyxy3d/calibration/charuco.py
--rw-r--r--   0        0        0     1685 2023-05-06 23:17:45.315853 pyxy3d-0.1.6/pyxy3d/calibration/draw_charuco.py
--rw-r--r--   0        0        0     9886 2023-06-13 12:10:26.418277 pyxy3d-0.1.6/pyxy3d/calibration/monocalibrator.py
--rw-r--r--   0        0        0    12385 2023-06-07 20:46:34.092944 pyxy3d-0.1.6/pyxy3d/calibration/stereocalibrator.py
--rw-r--r--   0        0        0    10631 2023-05-24 15:08:32.475147 pyxy3d-0.1.6/pyxy3d/cameras/camera.py
--rw-r--r--   0        0        0     7710 2023-06-13 12:10:26.422277 pyxy3d-0.1.6/pyxy3d/cameras/camera_array.py
--rw-r--r--   0        0        0    12868 2023-05-06 23:17:45.315853 pyxy3d-0.1.6/pyxy3d/cameras/camera_array_initializer.py
--rw-r--r--   0        0        0    11935 2023-06-09 15:21:03.574426 pyxy3d-0.1.6/pyxy3d/cameras/live_stream.py
--rw-r--r--   0        0        0    13543 2023-06-16 16:25:22.746734 pyxy3d-0.1.6/pyxy3d/cameras/synchronizer.py
--rw-r--r--   0        0        0    12973 2023-06-28 15:19:10.033043 pyxy3d-0.1.6/pyxy3d/configurator.py
--rw-r--r--   0        0        0     7036 2023-05-19 14:51:39.073378 pyxy3d-0.1.6/pyxy3d/export.py
--rw-r--r--   0        0        0     4052 2023-06-13 12:10:26.422277 pyxy3d-0.1.6/pyxy3d/gui/calibrate_capture_volume_widget.py
--rw-r--r--   0        0        0    17771 2023-06-07 15:23:42.550781 pyxy3d-0.1.6/pyxy3d/gui/camera_config/camera_config_dialogue.py
--rw-r--r--   0        0        0     5794 2023-05-31 21:07:55.283584 pyxy3d-0.1.6/pyxy3d/gui/camera_config/camera_summary_widget.py
--rw-r--r--   0        0        0     3893 2023-06-07 15:23:42.556515 pyxy3d-0.1.6/pyxy3d/gui/camera_config/frame_emitter.py
--rw-r--r--   0        0        0     3760 2023-06-13 12:10:26.426275 pyxy3d-0.1.6/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
--rw-r--r--   0        0        0    11157 2023-06-09 14:58:35.082613 pyxy3d-0.1.6/pyxy3d/gui/charuco_widget.py
--rw-r--r--   0        0        0    10800 2023-06-16 16:25:22.748751 pyxy3d-0.1.6/pyxy3d/gui/extrinsic_calibration_widget.py
--rw-r--r--   0        0        0    13851 2023-06-16 16:25:22.748751 pyxy3d-0.1.6/pyxy3d/gui/frame_builders/paired_frame_builder.py
--rw-r--r--   0        0        0    19878 2023-05-06 23:17:45.322358 pyxy3d-0.1.6/pyxy3d/gui/icons/pyxy_logo.svg
--rw-r--r--   0        0        0      941 2023-05-06 23:17:45.322358 pyxy3d-0.1.6/pyxy3d/gui/icons/rotate-camera-left.svg
--rw-r--r--   0        0        0      944 2023-05-06 23:17:45.322358 pyxy3d-0.1.6/pyxy3d/gui/icons/rotate-camera-right.svg
--rw-r--r--   0        0        0     2460 2023-05-31 14:26:10.311966 pyxy3d-0.1.6/pyxy3d/gui/log_widget.py
--rw-r--r--   0        0        0    16022 2023-06-28 15:19:10.033043 pyxy3d-0.1.6/pyxy3d/gui/main_widget.py
--rw-r--r--   0        0        0     3292 2023-06-07 20:46:34.100379 pyxy3d-0.1.6/pyxy3d/gui/navigation_bars.py
--rw-r--r--   0        0        0     1988 2023-06-07 15:23:42.559518 pyxy3d-0.1.6/pyxy3d/gui/playback_widget.py
--rw-r--r--   0        0        0    11310 2023-06-07 15:23:42.559518 pyxy3d-0.1.6/pyxy3d/gui/post_processing_widget.py
--rw-r--r--   0        0        0      950 2023-05-31 14:26:10.319966 pyxy3d-0.1.6/pyxy3d/gui/progress_dialog.py
--rw-r--r--   0        0        0    15210 2023-06-28 15:19:10.033043 pyxy3d-0.1.6/pyxy3d/gui/recording_widget.py
--rw-r--r--   0        0        0     3404 2023-06-07 20:46:34.102378 pyxy3d-0.1.6/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
--rw-r--r--   0        0        0     6843 2023-06-13 12:10:26.438272 pyxy3d-0.1.6/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
--rw-r--r--   0        0        0     9146 2023-05-17 15:15:57.175775 pyxy3d-0.1.6/pyxy3d/gui/vizualize/camera_mesh.py
--rw-r--r--   0        0        0     5054 2023-06-13 12:10:26.438272 pyxy3d-0.1.6/pyxy3d/gui/vizualize/playback_triangulation_widget.py
--rw-r--r--   0        0        0     5450 2023-05-24 15:08:32.491137 pyxy3d-0.1.6/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
--rw-r--r--   0        0        0     1135 2023-05-17 16:18:01.121529 pyxy3d-0.1.6/pyxy3d/helper.py
--rw-r--r--   0        0        0     6646 2023-05-31 21:07:55.283584 pyxy3d-0.1.6/pyxy3d/interface.py
--rw-r--r--   0        0        0     3111 2023-05-31 21:07:55.283584 pyxy3d-0.1.6/pyxy3d/logger.py
--rw-r--r--   0        0        0     7326 2023-06-28 15:19:10.033043 pyxy3d-0.1.6/pyxy3d/post_processor.py
--rw-r--r--   0        0        0    11830 2023-05-31 14:26:10.327964 pyxy3d-0.1.6/pyxy3d/recording/recorded_stream.py
--rw-r--r--   0        0        0     9108 2023-06-28 15:19:10.041090 pyxy3d-0.1.6/pyxy3d/recording/video_recorder.py
--rw-r--r--   0        0        0    21689 2023-06-28 15:19:10.043128 pyxy3d-0.1.6/pyxy3d/session/session.py
--rw-r--r--   0        0        0        0 2023-05-06 23:17:45.337987 pyxy3d-0.1.6/pyxy3d/trackers/__init__.py
--rw-r--r--   0        0        0     5004 2023-05-17 15:15:57.196405 pyxy3d-0.1.6/pyxy3d/trackers/charuco_tracker.py
--rw-r--r--   0        0        0     4651 2023-05-17 15:15:57.196405 pyxy3d-0.1.6/pyxy3d/trackers/hand_tracker.py
--rw-r--r--   0        0        0     1330 2023-05-17 15:15:57.196405 pyxy3d-0.1.6/pyxy3d/trackers/helper.py
--rw-r--r--   0        0        0    10677 2023-05-19 14:51:39.073378 pyxy3d-0.1.6/pyxy3d/trackers/holistic_opensim_tracker.py
--rw-r--r--   0        0        0     9146 2023-05-17 21:15:06.258248 pyxy3d-0.1.6/pyxy3d/trackers/holistic_tracker.py
--rw-r--r--   0        0        0     4239 2023-05-17 15:15:57.196405 pyxy3d-0.1.6/pyxy3d/trackers/pose_tracker.py
--rw-r--r--   0        0        0      669 2023-06-28 16:24:50.078474 pyxy3d-0.1.6/pyxy3d/trackers/tracker_enum.py
--rw-r--r--   0        0        0     8778 2023-05-06 23:17:45.337987 pyxy3d-0.1.6/pyxy3d/triangulate/array_stereo_triangulator.py
--rw-r--r--   0        0        0     5762 2023-05-06 23:17:45.337987 pyxy3d-0.1.6/pyxy3d/triangulate/stereo_points_builder.py
--rw-r--r--   0        0        0     7616 2023-05-17 16:18:01.121529 pyxy3d-0.1.6/pyxy3d/triangulate/sync_packet_triangulator.py
--rw-r--r--   0        0        0     7057 2023-06-28 16:33:04.058653 pyxy3d-0.1.6/README.md
--rw-r--r--   0        0        0     7819 1970-01-01 00:00:00.000000 pyxy3d-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35190 2023-06-14 20:19:57.480906 pyxy3d-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0      964 2023-07-09 15:22:38.188239 pyxy3d-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2644 2023-06-21 22:25:18.660194 pyxy3d-0.1.7/pyxy3d/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-23 18:50:36.211967 pyxy3d-0.1.7/pyxy3d/__main__.py
+-rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.1.7/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
+-rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
+-rw-r--r--   0        0        0     3517 2023-06-24 16:06:11.047479 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
+-rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
+-rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
+-rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/capture_volume.py
+-rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
+-rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
+-rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
+-rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
+-rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
+-rw-r--r--   0        0        0     4010 2023-06-23 18:50:36.212965 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/point_estimates.py
+-rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/quality_controller.py
+-rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/seaborn_summaries.py
+-rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/set_origin_functions.py
+-rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.1.7/pyxy3d/calibration/charuco.py
+-rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.1.7/pyxy3d/calibration/draw_charuco.py
+-rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.1.7/pyxy3d/calibration/monocalibrator.py
+-rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.1.7/pyxy3d/calibration/stereocalibrator.py
+-rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
+-rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
+-rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
+-rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
+-rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
+-rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
+-rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
+-rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     9898 2023-06-23 18:06:50.115857 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
+-rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.1.7/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
+-rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.1.7/pyxy3d/cameras/camera.py
+-rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.1.7/pyxy3d/cameras/camera_array.py
+-rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.1.7/pyxy3d/cameras/camera_array_initializer.py
+-rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.1.7/pyxy3d/cameras/live_stream.py
+-rw-r--r--   0        0        0    13543 2023-06-23 18:06:44.991101 pyxy3d-0.1.7/pyxy3d/cameras/synchronizer.py
+-rw-r--r--   0        0        0    12973 2023-06-27 18:50:03.752908 pyxy3d-0.1.7/pyxy3d/configurator.py
+-rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.1.7/pyxy3d/export.py
+-rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5691 2023-06-22 12:39:42.763393 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
+-rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8558 2023-06-22 12:39:48.156709 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0    11663 2023-06-24 17:18:38.710003 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
+-rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9611 2023-06-24 17:18:39.209013 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
+-rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
+-rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
+-rw-r--r--   0        0        0    12549 2023-07-09 14:52:45.450317 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
+-rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
+-rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.1.7/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.1.7/pyxy3d/gui/calibrate_capture_volume_widget.py
+-rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.1.7/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
+-rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.1.7/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
+-rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.1.7/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.1.7/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
+-rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.1.7/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
+-rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.1.7/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
+-rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.1.7/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.1.7/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.1.7/pyxy3d/gui/camera_config/camera_config_dialogue.py
+-rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.1.7/pyxy3d/gui/camera_config/camera_summary_widget.py
+-rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.1.7/pyxy3d/gui/camera_config/frame_emitter.py
+-rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.1.7/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.1.7/pyxy3d/gui/charuco_widget.py
+-rw-r--r--   0        0        0    10800 2023-06-15 18:45:15.728953 pyxy3d-0.1.7/pyxy3d/gui/extrinsic_calibration_widget.py
+-rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.1.7/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.1.7/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.1.7/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     9669 2023-06-22 12:39:48.162709 pyxy3d-0.1.7/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.1.7/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.1.7/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.1.7/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.1.7/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    13851 2023-06-15 18:45:15.729953 pyxy3d-0.1.7/pyxy3d/gui/frame_builders/paired_frame_builder.py
+-rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.1.7/pyxy3d/gui/icons/pyxy_logo.svg
+-rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.1.7/pyxy3d/gui/icons/rotate-camera-left.svg
+-rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.1.7/pyxy3d/gui/icons/rotate-camera-right.svg
+-rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.1.7/pyxy3d/gui/log_widget.py
+-rw-r--r--   0        0        0    16022 2023-06-24 17:14:07.184787 pyxy3d-0.1.7/pyxy3d/gui/main_widget.py
+-rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.1.7/pyxy3d/gui/navigation_bars.py
+-rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.1.7/pyxy3d/gui/playback_widget.py
+-rw-r--r--   0        0        0    11310 2023-06-24 17:14:09.527789 pyxy3d-0.1.7/pyxy3d/gui/post_processing_widget.py
+-rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.1.7/pyxy3d/gui/progress_dialog.py
+-rw-r--r--   0        0        0    15677 2023-07-09 15:20:51.201851 pyxy3d-0.1.7/pyxy3d/gui/recording_widget.py
+-rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.1.7/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
+-rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.1.7/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
+-rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.1.7/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
+-rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.1.7/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.1.7/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.1.7/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.1.7/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.1.7/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
+-rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.1.7/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.1.7/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.1.7/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.1.7/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
+-rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.1.7/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
+-rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.1.7/pyxy3d/gui/vizualize/camera_mesh.py
+-rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.1.7/pyxy3d/gui/vizualize/playback_triangulation_widget.py
+-rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.1.7/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
+-rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.1.7/pyxy3d/helper.py
+-rw-r--r--   0        0        0     6646 2023-06-15 00:37:58.434754 pyxy3d-0.1.7/pyxy3d/interface.py
+-rw-r--r--   0        0        0     3111 2023-06-23 18:15:31.076726 pyxy3d-0.1.7/pyxy3d/logger.py
+-rw-r--r--   0        0        0     7326 2023-06-26 23:53:47.788450 pyxy3d-0.1.7/pyxy3d/post_processor.py
+-rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.1.7/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.1.7/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     6095 2023-06-24 16:07:56.108685 pyxy3d-0.1.7/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
+-rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.1.7/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
+-rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.1.7/pyxy3d/recording/recorded_stream.py
+-rw-r--r--   0        0        0     9108 2023-06-24 16:07:34.481427 pyxy3d-0.1.7/pyxy3d/recording/video_recorder.py
+-rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.1.7/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
+-rw-r--r--   0        0        0    16640 2023-06-24 17:18:37.307013 pyxy3d-0.1.7/pyxy3d/session/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0    21689 2023-06-24 17:14:19.745502 pyxy3d-0.1.7/pyxy3d/session/session.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.1.7/pyxy3d/trackers/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.1.7/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.1.7/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.1.7/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.1.7/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.1.7/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.1.7/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.1.7/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.1.7/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.1.7/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
+-rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.1.7/pyxy3d/trackers/charuco_tracker.py
+-rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.1.7/pyxy3d/trackers/hand_tracker.py
+-rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.1.7/pyxy3d/trackers/helper.py
+-rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.1.7/pyxy3d/trackers/holistic_opensim_tracker.py
+-rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.1.7/pyxy3d/trackers/holistic_tracker.py
+-rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.1.7/pyxy3d/trackers/pose_tracker.py
+-rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.1.7/pyxy3d/trackers/tracker_enum.py
+-rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
+-rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
+-rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
+-rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
+-rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
+-rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
+-rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
+-rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
+-rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
+-rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
+-rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
+-rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
+-rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
+-rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
+-rw-r--r--   0        0        0   275452 2023-06-27 19:48:44.535266 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.4.nbc
+-rw-r--r--   0        0        0     4841 2023-06-27 19:48:44.532265 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
+-rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
+-rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
+-rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
+-rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
+-rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
+-rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
+-rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
+-rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
+-rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
+-rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
+-rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
+-rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
+-rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
+-rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
+-rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
+-rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
+-rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
+-rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
+-rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.1.7/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.1.7/pyxy3d/triangulate/array_stereo_triangulator.py
+-rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.1.7/pyxy3d/triangulate/stereo_points_builder.py
+-rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.1.7/pyxy3d/triangulate/sync_packet_triangulator.py
+-rw-r--r--   0        0        0     7057 2023-06-29 14:49:20.926620 pyxy3d-0.1.7/README.md
+-rw-r--r--   0        0        0     7819 1970-01-01 00:00:00.000000 pyxy3d-0.1.7/PKG-INFO
```

### Comparing `pyxy3d-0.1.6/LICENSE.md` & `pyxy3d-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyproject.toml` & `pyxy3d-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyxy3d"
-version = "0.1.6"
+version = "0.1.7"
 description = "A package for calibrating standard webcams to enable 3d motion tracking"
 authors = ["Mac Prible <prible@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.10.11"  #frequent segfaults in python 3.10.11
```

### Comparing `pyxy3d-0.1.6/pyxy3d/__init__.py` & `pyxy3d-0.1.7/pyxy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/__main__.py` & `pyxy3d-0.1.7/pyxy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/capture_volume.py` & `pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/capture_volume.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py` & `pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py` & `pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/point_estimates.py` & `pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/quality_controller.py` & `pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/quality_controller.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/seaborn_summaries.py` & `pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/seaborn_summaries.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/capture_volume/set_origin_functions.py` & `pyxy3d-0.1.7/pyxy3d/calibration/capture_volume/set_origin_functions.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/charuco.py` & `pyxy3d-0.1.7/pyxy3d/calibration/charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/draw_charuco.py` & `pyxy3d-0.1.7/pyxy3d/calibration/draw_charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/monocalibrator.py` & `pyxy3d-0.1.7/pyxy3d/calibration/monocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/calibration/stereocalibrator.py` & `pyxy3d-0.1.7/pyxy3d/calibration/stereocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/cameras/camera.py` & `pyxy3d-0.1.7/pyxy3d/cameras/camera.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/cameras/camera_array.py` & `pyxy3d-0.1.7/pyxy3d/cameras/camera_array.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/cameras/camera_array_initializer.py` & `pyxy3d-0.1.7/pyxy3d/cameras/camera_array_initializer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/cameras/live_stream.py` & `pyxy3d-0.1.7/pyxy3d/cameras/live_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/cameras/synchronizer.py` & `pyxy3d-0.1.7/pyxy3d/cameras/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/configurator.py` & `pyxy3d-0.1.7/pyxy3d/configurator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/export.py` & `pyxy3d-0.1.7/pyxy3d/export.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/calibrate_capture_volume_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/calibrate_capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/camera_config/camera_config_dialogue.py` & `pyxy3d-0.1.7/pyxy3d/gui/camera_config/camera_config_dialogue.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/camera_config/camera_summary_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/camera_config/camera_summary_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/camera_config/frame_emitter.py` & `pyxy3d-0.1.7/pyxy3d/gui/camera_config/frame_emitter.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/charuco_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/charuco_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/extrinsic_calibration_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/extrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/frame_builders/paired_frame_builder.py` & `pyxy3d-0.1.7/pyxy3d/gui/frame_builders/paired_frame_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/icons/pyxy_logo.svg` & `pyxy3d-0.1.7/pyxy3d/gui/icons/pyxy_logo.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/icons/rotate-camera-left.svg` & `pyxy3d-0.1.7/pyxy3d/gui/icons/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/icons/rotate-camera-right.svg` & `pyxy3d-0.1.7/pyxy3d/gui/icons/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/log_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/main_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/main_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/navigation_bars.py` & `pyxy3d-0.1.7/pyxy3d/gui/navigation_bars.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/playback_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/playback_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/post_processing_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/post_processing_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/progress_dialog.py` & `pyxy3d-0.1.7/pyxy3d/gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/recording_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/recording_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,17 +176,17 @@
         for port, drop_rate in dropped_fps.items():
             text += f"{port}: {drop_rate:.0%}        "
 
         self.dropped_fps_label.setText(text)
          
         
     def ImageUpdateSlot(self, q_image):
-        self.recording_frame_display.resize(self.recording_frame_display.sizeHint())
         qpixmap = QPixmap.fromImage(q_image)
         self.recording_frame_display.setPixmap(qpixmap)
+        # self.recording_frame_display.resize(self.recording_frame_display.sizeHint())
         
 class UnpairedFrameBuilder:
     def __init__(self, synchronizer: Synchronizer, single_frame_height=250):
         self.synchronizer = synchronizer 
         self.single_frame_height = single_frame_height
 
         # self.rotation_counts = {}
@@ -197,15 +197,14 @@
             self.ports.append(port)
         self.ports.sort()
         
         # reasonable default for the shape of the all-cameras frame
         # make it as square as you can get it
         camera_count = len(self.ports)
         self.frame_columns = int(math.ceil(camera_count**.5))
-        self.frame_rows = int(math.ceil(camera_count/self.frame_columns))
 
         self.new_sync_packet_notice = Queue()
         self.synchronizer.subscribe_to_notice(self.new_sync_packet_notice)
     
     def unsubscribe_from_synchronizer(self):
         logger.info("Unsubscribe frame builder from synchronizer.")
         self.synchronizer.unsubscribe_to_notice(self.new_sync_packet_notice) 
@@ -299,47 +298,53 @@
                                 fontScale=1,
                                 color=(0, 0, 255),
                                 thickness=2,
                             )
             
             thumbnail_frames[port] = text_frame
                     
+        # Begin to assemble the individual frames into a grid
         frame_rows = [] 
-        current_row = None
+        current_row = None # no frames laid down yet
         current_row_length = 0
-        frames_added = 0 
-        frames_remaining = len(self.ports)
+
         for port,frame in thumbnail_frames.items():
-            # for column in range(self.frame_columns):
             if current_row is None:
                 current_row = frame
+                current_row_length += 1
             else:
-                current_row = np.hstack([current_row,frame])  
-            current_row_length +=1
-            frames_remaining -=1
-
-            if frames_remaining ==0:
-                # pad with blanks
-                while current_row_length < self.frame_columns:
-                    current_row = np.hstack([current_row,self.get_frame_or_blank(None)]) 
-                    current_row_length += 1
-
-            if current_row_length == self.frame_columns:
-                frame_rows.append(current_row)            
-                current_row = None
-                current_row_length = 0
+                current_row = np.hstack([current_row, frame])  
+                current_row_length += 1
+                if current_row_length == self.frame_columns:
+
+                    current_row = prep_img_for_qpixmap(current_row)
+                    frame_rows.append(current_row)            
+                    current_row = None
+                    current_row_length = 0
+            
         
+
+        # After the loop
+        if current_row is not None:
+            while current_row_length < self.frame_columns:
+                current_row = np.hstack([current_row, self.get_frame_or_blank(None)]) 
+
+                current_row_length += 1
+
+            current_row = prep_img_for_qpixmap(current_row)
+            frame_rows.append(current_row)
+
+
         mega_frame = None
         for row in frame_rows:
             if mega_frame is None:
                 mega_frame = row
             else:
                 mega_frame = np.vstack([mega_frame,row]) 
-                         
-         
+        
         return mega_frame
 
 class UnpairedFrameEmitter(QThread):
     ImageBroadcast = pyqtSignal(QImage)
     dropped_fps = pyqtSignal(dict)
     
     def __init__(self, unpaired_frame_builder:UnpairedFrameBuilder):
@@ -350,27 +355,33 @@
         self.keep_collecting = Event() 
         
     def run(self):
 
         self.keep_collecting.set()
         
         while self.keep_collecting.is_set():
-            # that that it is important to make sure that this signal is sent only once
-            # to avoid multiple calibration attempts 
-                      
             recording_frame = self.recording_frame_builder.get_recording_frame()
 
             if recording_frame is not None:
                 image = cv2_to_qlabel(recording_frame)
                 self.ImageBroadcast.emit(image)
                 self.dropped_fps.emit(self.recording_frame_builder.synchronizer.dropped_fps)
 
         logger.info("Stereoframe emitter run thread ended...") 
             
+def prep_img_for_qpixmap(image:np.ndarray):
+    """
+    qpixmap needs dimensions divisible by 4 and without that weird things happen.
+    """
+    if image.shape[1] % 4 != 0:  # If the width of the row isn't divisible by 4
+        padding_width = 4 - (image.shape[1] % 4)  # Calculate how much padding is needed
+        padding = np.zeros((image.shape[0], padding_width, image.shape[2]), dtype=image.dtype)  # Create a black image of the required size
+        image = np.hstack([image, padding])  # Add the padding to the right of the image
 
+    return image
 
 def get_empty_pairs(board_counts, min_threshold):
     empty_pairs = [key for key, value in board_counts.items() if value < min_threshold]
     return empty_pairs
 
 def resize(image, new_height):
     (current_height, current_width) = image.shape[:2]
@@ -386,14 +397,15 @@
     
     qt_frame = QImage(
         image.data,
         image.shape[1],
         image.shape[0],
         QImage.Format.Format_RGB888,
     )
+
     return qt_frame
 
 
 def launch_recording_widget(session_path):
             config = Configurator(session_path)
             session = Session(config)
             # session.load_stream_tools()
```

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py` & `pyxy3d-0.1.7/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/vizualize/camera_mesh.py` & `pyxy3d-0.1.7/pyxy3d/gui/vizualize/camera_mesh.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/vizualize/playback_triangulation_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/vizualize/playback_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/gui/vizualize/realtime_triangulation_widget.py` & `pyxy3d-0.1.7/pyxy3d/gui/vizualize/realtime_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/helper.py` & `pyxy3d-0.1.7/pyxy3d/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/interface.py` & `pyxy3d-0.1.7/pyxy3d/interface.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/logger.py` & `pyxy3d-0.1.7/pyxy3d/logger.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/post_processor.py` & `pyxy3d-0.1.7/pyxy3d/post_processor.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/recording/recorded_stream.py` & `pyxy3d-0.1.7/pyxy3d/recording/recorded_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/recording/video_recorder.py` & `pyxy3d-0.1.7/pyxy3d/recording/video_recorder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/session/session.py` & `pyxy3d-0.1.7/pyxy3d/session/session.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/trackers/charuco_tracker.py` & `pyxy3d-0.1.7/pyxy3d/trackers/charuco_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/trackers/hand_tracker.py` & `pyxy3d-0.1.7/pyxy3d/trackers/hand_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/trackers/helper.py` & `pyxy3d-0.1.7/pyxy3d/trackers/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/trackers/holistic_opensim_tracker.py` & `pyxy3d-0.1.7/pyxy3d/trackers/holistic_opensim_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/trackers/holistic_tracker.py` & `pyxy3d-0.1.7/pyxy3d/trackers/holistic_tracker.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-import pyxy3d.logger
-
-logger = pyxy3d.logger.get(__name__)
-from threading import Thread, Event
-from queue import Queue
-
-import mediapipe as mp
-import numpy as np
-import cv2
-
-# cap = cv2.VideoCapture(0)
-from pyxy3d.interface import Tracker, PointPacket
-from pyxy3d.trackers.helper import apply_rotation, unrotate_points
-
-DRAW_IGNORE_LIST = [
-    "nose",
-    "left_eye_inner",
-    "left_eye",
-    "left_eye_outer",
-    "right_eye_inner",
-    "right_eye",
-    "right_eye_outer",
-    "left_ear",
-    "right_ear",
-    "mouth_left",
-    "mouth_right",
-    "left_wrist_pose",
-    "right_wrist_pose",
-    "left_pinky",
-    "right_pinky",
-    "left_index",
-    "right_index",
-    "left_thumb",
-    "right_thumb",
-]
-
-POINT_NAMES = {
-    0: "nose",
-    1: "left_eye_inner",
-    2: "left_eye",
-    3: "left_eye_outer",
-    4: "right_eye_inner",
-    5: "right_eye",
-    6: "right_eye_outer",
-    7: "left_ear",
-    8: "right_ear",
-    9: "mouth_left",
-    10: "mouth_right",
-    11: "left_shoulder",
-    12: "right_shoulder",
-    13: "left_elbow",
-    14: "right_elbow",
-    15: "left_wrist_pose",
-    16: "right_wrist_pose",
-    17: "left_pinky",
-    18: "right_pinky",
-    19: "left_index",
-    20: "right_index",
-    21: "left_thumb",
-    22: "right_thumb",
-    23: "left_hip",
-    24: "right_hip",
-    25: "left_knee",
-    26: "right_knee",
-    27: "left_ankle",
-    28: "right_ankle",
-    29: "left_heel",
-    30: "right_heel",
-    31: "left_foot_index",
-    32: "right_foot_index",
-    100: "right_wrist",
-    101: "right_thumb_CMC",
-    102: "right_thumb_MCP",
-    103: "right_thumb_IP",
-    104: "right_thumb_tip",
-    105: "right_index_finger_MCP",
-    106: "right_index_finger_PIP",
-    107: "right_index_finger_DIP",
-    108: "right_index_finger_tip",
-    109: "right_middle_finger_MCP",
-    110: "right_middle_finger_PIP",
-    111: "right_middle_finger_DIP",
-    112: "right_middle_finger_tip",
-    113: "right_ring_finger_MCP",
-    114: "right_ring_finger_PIP",
-    115: "right_ring_finger_DIP",
-    116: "right_ring_finger_tip",
-    117: "right_pinky_MCP",
-    118: "right_pinky_PIP",
-    119: "right_pinky_DIP",
-    120: "right_pinky_tip",
-    200: "left_wrist",
-    201: "left_thumb_CMC",
-    202: "left_thumb_MCP",
-    203: "left_thumb_IP",
-    204: "left_thumb_tip",
-    205: "left_index_finger_MCP",
-    206: "left_index_finger_PIP",
-    207: "left_index_finger_DIP",
-    208: "left_index_finger_tip",
-    209: "left_middle_finger_MCP",
-    210: "left_middle_finger_PIP",
-    211: "left_middle_finger_DIP",
-    212: "left_middle_finger_tip",
-    213: "left_ring_finger_MCP",
-    214: "left_ring_finger_PIP",
-    215: "left_ring_finger_DIP",
-    216: "left_ring_finger_tip",
-    217: "left_pinky_MCP",
-    218: "left_pinky_PIP",
-    219: "left_pinky_DIP",
-    220: "left_pinky_tip",
-}
-
-
-# keep ids in distinct ranges to avoid clashes
-POSE_OFFSET = 0
-RIGHT_HAND_OFFSET = 100
-LEFT_HAND_OFFSET = 200
-FACE_OFFSET = 500
-
-
-class HolisticTracker(Tracker):
-    def __init__(self) -> None:
-        # each port gets its own mediapipe context manager
-        # use a dictionary of queues for passing
-        self.in_queues = {}
-        self.out_queues = {}
-        self.threads = {}
-
-    @property
-    def name(self):
-        return "HOLISTIC"
-
-    def run_frame_processor(self, port: int, rotation_count: int):
-        # Create a MediaPipe pose instance
-        with mp.solutions.holistic.Holistic(
-            min_detection_confidence=0.8, min_tracking_confidence=0.8
-        ) as holistic:
-            while True:
-                frame = self.in_queues[port].get()
-                # apply rotation as needed
-                frame = apply_rotation(frame, rotation_count)
-
-                height, width, color = frame.shape
-                # Convert the image to RGB format
-                frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-                results = holistic.process(frame)
-
-                # initialize variables so none will be created if no points detected
-                point_ids = []
-                landmark_xy = []
-
-                if results.pose_landmarks:
-                    for landmark_id, landmark in enumerate(
-                        results.pose_landmarks.landmark
-                    ):
-                        # mediapipe expresses in terms of percent of frame, so must map to pixel position
-                        x, y = int(landmark.x * width), int(landmark.y * height)
-                        if (
-                            landmark.x < 0
-                            or landmark.x > 1
-                            or landmark.y < 0
-                            or landmark.y > 1
-                        ):
-                            # ignore
-                            pass
-                        else:
-                            point_ids.append(landmark_id + POSE_OFFSET)
-                            landmark_xy.append((x, y))
-
-                if results.right_hand_landmarks:
-                    for landmark_id, landmark in enumerate(
-                        results.right_hand_landmarks.landmark
-                    ):
-                        # mediapipe expresses in terms of percent of frame, so must map to pixel position
-                        x, y = int(landmark.x * width), int(landmark.y * height)
-                        if (
-                            landmark.x < 0
-                            or landmark.x > 1
-                            or landmark.y < 0
-                            or landmark.y > 1
-                        ):
-                            # ignore
-                            pass
-                        else:
-                            point_ids.append(landmark_id + RIGHT_HAND_OFFSET)
-                            landmark_xy.append((x, y))
-
-                if results.left_hand_landmarks:
-                    for landmark_id, landmark in enumerate(
-                        results.left_hand_landmarks.landmark
-                    ):
-                        # mediapipe expresses in terms of percent of frame, so must map to pixel positionND_OFFSET
-                        x, y = int(landmark.x * width), int(landmark.y * height)
-                        if (
-                            landmark.x < 0
-                            or landmark.x > 1
-                            or landmark.y < 0
-                            or landmark.y > 1
-                        ):
-                            # ignore
-                            pass
-                        else:
-                            point_ids.append(landmark_id + LEFT_HAND_OFFSET)
-                            landmark_xy.append((x, y))
-
-                if results.face_landmarks:
-                    for landmark_id, landmark in enumerate(
-                        results.face_landmarks.landmark
-                    ):
-                        # mediapipe expresses in terms of percent of frame, so must map to pixel positionFSET
-                        x, y = int(landmark.x * width), int(landmark.y * height)
-                        if (
-                            landmark.x < 0
-                            or landmark.x > 1
-                            or landmark.y < 0
-                            or landmark.y > 1
-                        ):
-                            # ignore
-                            pass
-                        else:
-                            point_ids.append(landmark_id + FACE_OFFSET)
-                            landmark_xy.append((x, y))
-
-                point_ids = np.array(point_ids)
-                landmark_xy = np.array(landmark_xy)
-                landmark_xy = unrotate_points(
-                    landmark_xy, rotation_count, width, height
-                )
-                point_packet = PointPacket(point_ids, landmark_xy)
-
-                self.out_queues[port].put(point_packet)
-
-    def get_points(
-        self, frame: np.ndarray, port: int, rotation_count: int
-    ) -> PointPacket:
-        if port not in self.in_queues.keys():
-            self.in_queues[port] = Queue(1)
-            self.out_queues[port] = Queue(1)
-
-            self.threads[port] = Thread(
-                target=self.run_frame_processor,
-                args=(port, rotation_count),
-                daemon=True,
-            )
-
-            self.threads[port].start()
-
-        self.in_queues[port].put(frame)
-        point_packet = self.out_queues[port].get()
-
-        return point_packet
-
-    def get_point_name(self, point_id) -> str:
-        if point_id < FACE_OFFSET:
-            point_name = POINT_NAMES[point_id]
-        else:
-            point_name = "face_" + str(point_id - FACE_OFFSET)
-        return point_name
-
-    def draw_instructions(self, point_id: int) -> dict:
-        point_name = self.get_point_name(point_id)
-        if point_name in DRAW_IGNORE_LIST:
-            rules = {"radius": 0, "color": (0, 0, 0), "thickness": 0}
-        elif point_name.startswith("left"):
-            rules = {"radius": 5, "color": (0, 0, 220), "thickness": 3}
-        elif point_name.startswith("right"):
-            rules = {"radius": 5, "color": (220, 0, 0), "thickness": 3}
-        else:
-            rules = {"radius": 1, "color": (220, 0, 220), "thickness": 1}
-
-        return rules
+import pyxy3d.logger
+
+logger = pyxy3d.logger.get(__name__)
+from threading import Thread, Event
+from queue import Queue
+
+import mediapipe as mp
+import numpy as np
+import cv2
+
+# cap = cv2.VideoCapture(0)
+from pyxy3d.interface import Tracker, PointPacket
+from pyxy3d.trackers.helper import apply_rotation, unrotate_points
+
+DRAW_IGNORE_LIST = [
+    "nose",
+    "left_eye_inner",
+    "left_eye",
+    "left_eye_outer",
+    "right_eye_inner",
+    "right_eye",
+    "right_eye_outer",
+    "left_ear",
+    "right_ear",
+    "mouth_left",
+    "mouth_right",
+    "left_wrist_pose",
+    "right_wrist_pose",
+    "left_pinky",
+    "right_pinky",
+    "left_index",
+    "right_index",
+    "left_thumb",
+    "right_thumb",
+]
+
+POINT_NAMES = {
+    0: "nose",
+    1: "left_eye_inner",
+    2: "left_eye",
+    3: "left_eye_outer",
+    4: "right_eye_inner",
+    5: "right_eye",
+    6: "right_eye_outer",
+    7: "left_ear",
+    8: "right_ear",
+    9: "mouth_left",
+    10: "mouth_right",
+    11: "left_shoulder",
+    12: "right_shoulder",
+    13: "left_elbow",
+    14: "right_elbow",
+    15: "left_wrist_pose",
+    16: "right_wrist_pose",
+    17: "left_pinky",
+    18: "right_pinky",
+    19: "left_index",
+    20: "right_index",
+    21: "left_thumb",
+    22: "right_thumb",
+    23: "left_hip",
+    24: "right_hip",
+    25: "left_knee",
+    26: "right_knee",
+    27: "left_ankle",
+    28: "right_ankle",
+    29: "left_heel",
+    30: "right_heel",
+    31: "left_foot_index",
+    32: "right_foot_index",
+    100: "right_wrist",
+    101: "right_thumb_CMC",
+    102: "right_thumb_MCP",
+    103: "right_thumb_IP",
+    104: "right_thumb_tip",
+    105: "right_index_finger_MCP",
+    106: "right_index_finger_PIP",
+    107: "right_index_finger_DIP",
+    108: "right_index_finger_tip",
+    109: "right_middle_finger_MCP",
+    110: "right_middle_finger_PIP",
+    111: "right_middle_finger_DIP",
+    112: "right_middle_finger_tip",
+    113: "right_ring_finger_MCP",
+    114: "right_ring_finger_PIP",
+    115: "right_ring_finger_DIP",
+    116: "right_ring_finger_tip",
+    117: "right_pinky_MCP",
+    118: "right_pinky_PIP",
+    119: "right_pinky_DIP",
+    120: "right_pinky_tip",
+    200: "left_wrist",
+    201: "left_thumb_CMC",
+    202: "left_thumb_MCP",
+    203: "left_thumb_IP",
+    204: "left_thumb_tip",
+    205: "left_index_finger_MCP",
+    206: "left_index_finger_PIP",
+    207: "left_index_finger_DIP",
+    208: "left_index_finger_tip",
+    209: "left_middle_finger_MCP",
+    210: "left_middle_finger_PIP",
+    211: "left_middle_finger_DIP",
+    212: "left_middle_finger_tip",
+    213: "left_ring_finger_MCP",
+    214: "left_ring_finger_PIP",
+    215: "left_ring_finger_DIP",
+    216: "left_ring_finger_tip",
+    217: "left_pinky_MCP",
+    218: "left_pinky_PIP",
+    219: "left_pinky_DIP",
+    220: "left_pinky_tip",
+}
+
+
+# keep ids in distinct ranges to avoid clashes
+POSE_OFFSET = 0
+RIGHT_HAND_OFFSET = 100
+LEFT_HAND_OFFSET = 200
+FACE_OFFSET = 500
+
+
+class HolisticTracker(Tracker):
+    def __init__(self) -> None:
+        # each port gets its own mediapipe context manager
+        # use a dictionary of queues for passing
+        self.in_queues = {}
+        self.out_queues = {}
+        self.threads = {}
+
+    @property
+    def name(self):
+        return "HOLISTIC"
+
+    def run_frame_processor(self, port: int, rotation_count: int):
+        # Create a MediaPipe pose instance
+        with mp.solutions.holistic.Holistic(
+            min_detection_confidence=0.8, min_tracking_confidence=0.8
+        ) as holistic:
+            while True:
+                frame = self.in_queues[port].get()
+                # apply rotation as needed
+                frame = apply_rotation(frame, rotation_count)
+
+                height, width, color = frame.shape
+                # Convert the image to RGB format
+                frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+                results = holistic.process(frame)
+
+                # initialize variables so none will be created if no points detected
+                point_ids = []
+                landmark_xy = []
+
+                if results.pose_landmarks:
+                    for landmark_id, landmark in enumerate(
+                        results.pose_landmarks.landmark
+                    ):
+                        # mediapipe expresses in terms of percent of frame, so must map to pixel position
+                        x, y = int(landmark.x * width), int(landmark.y * height)
+                        if (
+                            landmark.x < 0
+                            or landmark.x > 1
+                            or landmark.y < 0
+                            or landmark.y > 1
+                        ):
+                            # ignore
+                            pass
+                        else:
+                            point_ids.append(landmark_id + POSE_OFFSET)
+                            landmark_xy.append((x, y))
+
+                if results.right_hand_landmarks:
+                    for landmark_id, landmark in enumerate(
+                        results.right_hand_landmarks.landmark
+                    ):
+                        # mediapipe expresses in terms of percent of frame, so must map to pixel position
+                        x, y = int(landmark.x * width), int(landmark.y * height)
+                        if (
+                            landmark.x < 0
+                            or landmark.x > 1
+                            or landmark.y < 0
+                            or landmark.y > 1
+                        ):
+                            # ignore
+                            pass
+                        else:
+                            point_ids.append(landmark_id + RIGHT_HAND_OFFSET)
+                            landmark_xy.append((x, y))
+
+                if results.left_hand_landmarks:
+                    for landmark_id, landmark in enumerate(
+                        results.left_hand_landmarks.landmark
+                    ):
+                        # mediapipe expresses in terms of percent of frame, so must map to pixel positionND_OFFSET
+                        x, y = int(landmark.x * width), int(landmark.y * height)
+                        if (
+                            landmark.x < 0
+                            or landmark.x > 1
+                            or landmark.y < 0
+                            or landmark.y > 1
+                        ):
+                            # ignore
+                            pass
+                        else:
+                            point_ids.append(landmark_id + LEFT_HAND_OFFSET)
+                            landmark_xy.append((x, y))
+
+                if results.face_landmarks:
+                    for landmark_id, landmark in enumerate(
+                        results.face_landmarks.landmark
+                    ):
+                        # mediapipe expresses in terms of percent of frame, so must map to pixel positionFSET
+                        x, y = int(landmark.x * width), int(landmark.y * height)
+                        if (
+                            landmark.x < 0
+                            or landmark.x > 1
+                            or landmark.y < 0
+                            or landmark.y > 1
+                        ):
+                            # ignore
+                            pass
+                        else:
+                            point_ids.append(landmark_id + FACE_OFFSET)
+                            landmark_xy.append((x, y))
+
+                point_ids = np.array(point_ids)
+                landmark_xy = np.array(landmark_xy)
+                landmark_xy = unrotate_points(
+                    landmark_xy, rotation_count, width, height
+                )
+                point_packet = PointPacket(point_ids, landmark_xy)
+
+                self.out_queues[port].put(point_packet)
+
+    def get_points(
+        self, frame: np.ndarray, port: int, rotation_count: int
+    ) -> PointPacket:
+        if port not in self.in_queues.keys():
+            self.in_queues[port] = Queue(1)
+            self.out_queues[port] = Queue(1)
+
+            self.threads[port] = Thread(
+                target=self.run_frame_processor,
+                args=(port, rotation_count),
+                daemon=True,
+            )
+
+            self.threads[port].start()
+
+        self.in_queues[port].put(frame)
+        point_packet = self.out_queues[port].get()
+
+        return point_packet
+
+    def get_point_name(self, point_id) -> str:
+        if point_id < FACE_OFFSET:
+            point_name = POINT_NAMES[point_id]
+        else:
+            point_name = "face_" + str(point_id - FACE_OFFSET)
+        return point_name
+
+    def draw_instructions(self, point_id: int) -> dict:
+        point_name = self.get_point_name(point_id)
+        if point_name in DRAW_IGNORE_LIST:
+            rules = {"radius": 0, "color": (0, 0, 0), "thickness": 0}
+        elif point_name.startswith("left"):
+            rules = {"radius": 5, "color": (0, 0, 220), "thickness": 3}
+        elif point_name.startswith("right"):
+            rules = {"radius": 5, "color": (220, 0, 0), "thickness": 3}
+        else:
+            rules = {"radius": 1, "color": (220, 0, 220), "thickness": 1}
+
+        return rules
```

### Comparing `pyxy3d-0.1.6/pyxy3d/trackers/pose_tracker.py` & `pyxy3d-0.1.7/pyxy3d/trackers/pose_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/trackers/tracker_enum.py` & `pyxy3d-0.1.7/pyxy3d/trackers/tracker_enum.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/triangulate/array_stereo_triangulator.py` & `pyxy3d-0.1.7/pyxy3d/triangulate/array_stereo_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/triangulate/stereo_points_builder.py` & `pyxy3d-0.1.7/pyxy3d/triangulate/stereo_points_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/pyxy3d/triangulate/sync_packet_triangulator.py` & `pyxy3d-0.1.7/pyxy3d/triangulate/sync_packet_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/README.md` & `pyxy3d-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.6/PKG-INFO` & `pyxy3d-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxy3d
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for calibrating standard webcams to enable 3d motion tracking
 License: AGPL-3.0-only
 Author: Mac Prible
 Author-email: prible@gmail.com
 Requires-Python: >=3.10,<3.10.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

