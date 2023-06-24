# Comparing `tmp/pyxy3d-0.1.4.tar.gz` & `tmp/pyxy3d-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxy3d-0.1.4.tar", max compression
+gzip compressed data, was "pyxy3d-0.1.5.tar", max compression
```

## Comparing `pyxy3d-0.1.4.tar` & `pyxy3d-0.1.5.tar`

### file list

```diff
@@ -1,232 +1,232 @@
--rw-r--r--   0        0        0    35190 2023-06-14 20:19:57.480906 pyxy3d-0.1.4/LICENSE.md
--rw-r--r--   0        0        0      964 2023-06-23 18:50:49.716635 pyxy3d-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2644 2023-06-21 22:25:18.660194 pyxy3d-0.1.4/pyxy3d/__init__.py
--rw-r--r--   0        0        0      686 2023-06-23 18:50:36.211967 pyxy3d-0.1.4/pyxy3d/__main__.py
--rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
--rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
--rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
--rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
--rw-r--r--   0        0        0     3517 2023-06-23 17:33:53.743685 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
--rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
--rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
--rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
--rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/capture_volume.py
--rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
--rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
--rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
--rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
--rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
--rw-r--r--   0        0        0     4010 2023-06-23 18:50:36.212965 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/point_estimates.py
--rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/quality_controller.py
--rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/seaborn_summaries.py
--rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/set_origin_functions.py
--rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.1.4/pyxy3d/calibration/charuco.py
--rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.1.4/pyxy3d/calibration/draw_charuco.py
--rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.1.4/pyxy3d/calibration/monocalibrator.py
--rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.1.4/pyxy3d/calibration/stereocalibrator.py
--rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
--rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
--rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
--rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
--rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
--rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
--rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
--rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
--rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
--rw-r--r--   0        0        0     9898 2023-06-23 18:06:50.115857 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
--rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
--rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.1.4/pyxy3d/cameras/camera.py
--rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.1.4/pyxy3d/cameras/camera_array.py
--rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.1.4/pyxy3d/cameras/camera_array_initializer.py
--rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.1.4/pyxy3d/cameras/live_stream.py
--rw-r--r--   0        0        0    13543 2023-06-23 18:06:44.991101 pyxy3d-0.1.4/pyxy3d/cameras/synchronizer.py
--rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.1.4/pyxy3d/configurator.py
--rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.1.4/pyxy3d/export.py
--rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5691 2023-06-22 12:39:42.763393 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
--rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8558 2023-06-22 12:39:48.156709 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0    11663 2023-06-23 18:41:19.758263 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
--rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
--rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
--rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
--rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
--rw-r--r--   0        0        0    12241 2023-06-23 18:41:17.940707 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
--rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
--rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
--rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
--rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.1.4/pyxy3d/gui/calibrate_capture_volume_widget.py
--rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
--rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
--rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
--rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
--rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
--rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.1.4/pyxy3d/gui/camera_config/camera_config_dialogue.py
--rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.1.4/pyxy3d/gui/camera_config/camera_summary_widget.py
--rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.1.4/pyxy3d/gui/camera_config/frame_emitter.py
--rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.1.4/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
--rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.1.4/pyxy3d/gui/charuco_widget.py
--rw-r--r--   0        0        0    10800 2023-06-15 18:45:15.728953 pyxy3d-0.1.4/pyxy3d/gui/extrinsic_calibration_widget.py
--rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0     9669 2023-06-22 12:39:48.162709 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
--rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0    13851 2023-06-15 18:45:15.729953 pyxy3d-0.1.4/pyxy3d/gui/frame_builders/paired_frame_builder.py
--rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.1.4/pyxy3d/gui/icons/pyxy_logo.svg
--rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.1.4/pyxy3d/gui/icons/rotate-camera-left.svg
--rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.1.4/pyxy3d/gui/icons/rotate-camera-right.svg
--rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.1.4/pyxy3d/gui/log_widget.py
--rw-r--r--   0        0        0    16022 2023-06-23 18:50:36.214966 pyxy3d-0.1.4/pyxy3d/gui/main_widget.py
--rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.1.4/pyxy3d/gui/navigation_bars.py
--rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.1.4/pyxy3d/gui/playback_widget.py
--rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.1.4/pyxy3d/gui/post_processing_widget.py
--rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.1.4/pyxy3d/gui/progress_dialog.py
--rw-r--r--   0        0        0    15210 2023-06-23 18:50:36.215967 pyxy3d-0.1.4/pyxy3d/gui/recording_widget.py
--rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
--rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
--rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
--rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
--rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
--rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
--rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.1.4/pyxy3d/gui/vizualize/camera_mesh.py
--rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.1.4/pyxy3d/gui/vizualize/playback_triangulation_widget.py
--rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.1.4/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
--rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.1.4/pyxy3d/helper.py
--rw-r--r--   0        0        0     6646 2023-06-15 00:37:58.434754 pyxy3d-0.1.4/pyxy3d/interface.py
--rw-r--r--   0        0        0     3111 2023-06-23 18:15:31.076726 pyxy3d-0.1.4/pyxy3d/logger.py
--rw-r--r--   0        0        0     7131 2023-06-23 18:50:36.216966 pyxy3d-0.1.4/pyxy3d/post_processor.py
--rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.1.4/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
--rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.1.4/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
--rw-r--r--   0        0        0     6089 2023-06-23 18:18:50.373825 pyxy3d-0.1.4/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
--rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.1.4/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
--rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.1.4/pyxy3d/recording/recorded_stream.py
--rw-r--r--   0        0        0     9108 2023-06-23 18:50:36.219967 pyxy3d-0.1.4/pyxy3d/recording/video_recorder.py
--rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.1.4/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
--rw-r--r--   0        0        0    16634 2023-06-23 17:48:49.082871 pyxy3d-0.1.4/pyxy3d/session/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0    21689 2023-06-23 18:50:36.220967 pyxy3d-0.1.4/pyxy3d/session/session.py
--rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.1.4/pyxy3d/trackers/__init__.py
--rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
--rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.1.4/pyxy3d/trackers/charuco_tracker.py
--rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.1.4/pyxy3d/trackers/hand_tracker.py
--rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.1.4/pyxy3d/trackers/helper.py
--rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.1.4/pyxy3d/trackers/holistic_opensim_tracker.py
--rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.1.4/pyxy3d/trackers/holistic_tracker.py
--rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.1.4/pyxy3d/trackers/pose_tracker.py
--rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.1.4/pyxy3d/trackers/tracker_enum.py
--rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
--rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
--rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
--rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
--rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
--rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
--rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
--rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
--rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
--rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
--rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
--rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
--rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
--rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
--rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
--rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
--rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
--rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
--rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
--rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
--rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
--rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
--rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
--rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
--rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
--rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
--rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
--rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
--rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
--rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
--rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
--rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
--rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
--rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
--rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
--rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.1.4/pyxy3d/triangulate/array_stereo_triangulator.py
--rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.1.4/pyxy3d/triangulate/stereo_points_builder.py
--rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.1.4/pyxy3d/triangulate/sync_packet_triangulator.py
--rw-r--r--   0        0        0     7485 2023-06-23 18:50:36.209967 pyxy3d-0.1.4/README.md
--rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 pyxy3d-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35190 2023-06-14 20:19:57.480906 pyxy3d-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0      964 2023-06-24 17:20:59.991301 pyxy3d-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2644 2023-06-21 22:25:18.660194 pyxy3d-0.1.5/pyxy3d/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-23 18:50:36.211967 pyxy3d-0.1.5/pyxy3d/__main__.py
+-rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
+-rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
+-rw-r--r--   0        0        0     3517 2023-06-24 16:06:11.047479 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
+-rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
+-rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
+-rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/capture_volume.py
+-rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
+-rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
+-rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
+-rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
+-rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
+-rw-r--r--   0        0        0     4010 2023-06-23 18:50:36.212965 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/point_estimates.py
+-rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/quality_controller.py
+-rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/seaborn_summaries.py
+-rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/set_origin_functions.py
+-rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.1.5/pyxy3d/calibration/charuco.py
+-rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.1.5/pyxy3d/calibration/draw_charuco.py
+-rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.1.5/pyxy3d/calibration/monocalibrator.py
+-rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.1.5/pyxy3d/calibration/stereocalibrator.py
+-rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
+-rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
+-rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
+-rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
+-rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
+-rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
+-rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
+-rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     9898 2023-06-23 18:06:50.115857 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
+-rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
+-rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.1.5/pyxy3d/cameras/camera.py
+-rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.1.5/pyxy3d/cameras/camera_array.py
+-rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.1.5/pyxy3d/cameras/camera_array_initializer.py
+-rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.1.5/pyxy3d/cameras/live_stream.py
+-rw-r--r--   0        0        0    13543 2023-06-23 18:06:44.991101 pyxy3d-0.1.5/pyxy3d/cameras/synchronizer.py
+-rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.1.5/pyxy3d/configurator.py
+-rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.1.5/pyxy3d/export.py
+-rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5691 2023-06-22 12:39:42.763393 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
+-rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8558 2023-06-22 12:39:48.156709 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0    11663 2023-06-24 17:18:38.710003 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
+-rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9611 2023-06-24 17:18:39.209013 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
+-rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
+-rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
+-rw-r--r--   0        0        0    12241 2023-06-24 16:06:09.196440 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
+-rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
+-rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.1.5/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.1.5/pyxy3d/gui/calibrate_capture_volume_widget.py
+-rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
+-rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
+-rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
+-rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
+-rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
+-rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.1.5/pyxy3d/gui/camera_config/camera_config_dialogue.py
+-rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.1.5/pyxy3d/gui/camera_config/camera_summary_widget.py
+-rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.1.5/pyxy3d/gui/camera_config/frame_emitter.py
+-rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.1.5/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.1.5/pyxy3d/gui/charuco_widget.py
+-rw-r--r--   0        0        0    10800 2023-06-15 18:45:15.728953 pyxy3d-0.1.5/pyxy3d/gui/extrinsic_calibration_widget.py
+-rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     9669 2023-06-22 12:39:48.162709 pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    13851 2023-06-15 18:45:15.729953 pyxy3d-0.1.5/pyxy3d/gui/frame_builders/paired_frame_builder.py
+-rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.1.5/pyxy3d/gui/icons/pyxy_logo.svg
+-rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.1.5/pyxy3d/gui/icons/rotate-camera-left.svg
+-rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.1.5/pyxy3d/gui/icons/rotate-camera-right.svg
+-rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.1.5/pyxy3d/gui/log_widget.py
+-rw-r--r--   0        0        0    16022 2023-06-24 17:14:07.184787 pyxy3d-0.1.5/pyxy3d/gui/main_widget.py
+-rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.1.5/pyxy3d/gui/navigation_bars.py
+-rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.1.5/pyxy3d/gui/playback_widget.py
+-rw-r--r--   0        0        0    11310 2023-06-24 17:14:09.527789 pyxy3d-0.1.5/pyxy3d/gui/post_processing_widget.py
+-rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.1.5/pyxy3d/gui/progress_dialog.py
+-rw-r--r--   0        0        0    15210 2023-06-23 18:50:36.215967 pyxy3d-0.1.5/pyxy3d/gui/recording_widget.py
+-rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
+-rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
+-rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
+-rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
+-rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
+-rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
+-rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.1.5/pyxy3d/gui/vizualize/camera_mesh.py
+-rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.1.5/pyxy3d/gui/vizualize/playback_triangulation_widget.py
+-rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.1.5/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
+-rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.1.5/pyxy3d/helper.py
+-rw-r--r--   0        0        0     6646 2023-06-15 00:37:58.434754 pyxy3d-0.1.5/pyxy3d/interface.py
+-rw-r--r--   0        0        0     3111 2023-06-23 18:15:31.076726 pyxy3d-0.1.5/pyxy3d/logger.py
+-rw-r--r--   0        0        0     7131 2023-06-23 18:50:36.216966 pyxy3d-0.1.5/pyxy3d/post_processor.py
+-rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.1.5/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.1.5/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     6095 2023-06-24 16:07:56.108685 pyxy3d-0.1.5/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
+-rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.1.5/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
+-rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.1.5/pyxy3d/recording/recorded_stream.py
+-rw-r--r--   0        0        0     9108 2023-06-24 16:07:34.481427 pyxy3d-0.1.5/pyxy3d/recording/video_recorder.py
+-rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.1.5/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
+-rw-r--r--   0        0        0    16640 2023-06-24 17:18:37.307013 pyxy3d-0.1.5/pyxy3d/session/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0    21689 2023-06-24 17:14:19.745502 pyxy3d-0.1.5/pyxy3d/session/session.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.1.5/pyxy3d/trackers/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
+-rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.1.5/pyxy3d/trackers/charuco_tracker.py
+-rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.1.5/pyxy3d/trackers/hand_tracker.py
+-rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.1.5/pyxy3d/trackers/helper.py
+-rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.1.5/pyxy3d/trackers/holistic_opensim_tracker.py
+-rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.1.5/pyxy3d/trackers/holistic_tracker.py
+-rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.1.5/pyxy3d/trackers/pose_tracker.py
+-rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.1.5/pyxy3d/trackers/tracker_enum.py
+-rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
+-rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
+-rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
+-rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
+-rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
+-rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
+-rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
+-rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
+-rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
+-rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
+-rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
+-rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
+-rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
+-rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
+-rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
+-rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
+-rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
+-rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
+-rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
+-rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
+-rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
+-rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
+-rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
+-rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
+-rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
+-rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
+-rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
+-rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
+-rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
+-rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
+-rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
+-rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
+-rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
+-rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.1.5/pyxy3d/triangulate/array_stereo_triangulator.py
+-rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.1.5/pyxy3d/triangulate/stereo_points_builder.py
+-rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.1.5/pyxy3d/triangulate/sync_packet_triangulator.py
+-rw-r--r--   0        0        0     7056 2023-06-24 16:28:11.303261 pyxy3d-0.1.5/README.md
+-rw-r--r--   0        0        0     7818 1970-01-01 00:00:00.000000 pyxy3d-0.1.5/PKG-INFO
```

### Comparing `pyxy3d-0.1.4/LICENSE.md` & `pyxy3d-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyproject.toml` & `pyxy3d-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyxy3d"
-version = "0.1.4"
+version = "0.1.5"
 description = "A package for calibrating standard webcams to enable 3d motion tracking"
 authors = ["Mac Prible <prible@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.10.11"  #frequent segfaults in python 3.10.11
```

### Comparing `pyxy3d-0.1.4/pyxy3d/__init__.py` & `pyxy3d-0.1.5/pyxy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/__main__.py` & `pyxy3d-0.1.5/pyxy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 17:33:37 2023 UTC, .py size: 4010 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 71d7 9564 aa0f 0000  o.......q..d....
+00000000: 6f0d 0d0a 0000 0000 7ce9 9564 aa0f 0000  o.......|..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6402 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6403 6c07 6d08 5a08 0100 6400 6401 6c09  d.l.m.Z...d.d.l.
 00000060: 5a0a 6400 6401 6c0b 5a0c 6400 6404 6c0d  Z.d.d.l.Z.d.d.l.
 00000070: 6d0e 5a0e 0100 6400 6405 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
```

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/capture_volume.py` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/capture_volume.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/point_estimates.py` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/quality_controller.py` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/quality_controller.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/seaborn_summaries.py` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/seaborn_summaries.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/capture_volume/set_origin_functions.py` & `pyxy3d-0.1.5/pyxy3d/calibration/capture_volume/set_origin_functions.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/charuco.py` & `pyxy3d-0.1.5/pyxy3d/calibration/charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/draw_charuco.py` & `pyxy3d-0.1.5/pyxy3d/calibration/draw_charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/monocalibrator.py` & `pyxy3d-0.1.5/pyxy3d/calibration/monocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/calibration/stereocalibrator.py` & `pyxy3d-0.1.5/pyxy3d/calibration/stereocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/camera.py` & `pyxy3d-0.1.5/pyxy3d/cameras/camera.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/camera_array.py` & `pyxy3d-0.1.5/pyxy3d/cameras/camera_array.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/camera_array_initializer.py` & `pyxy3d-0.1.5/pyxy3d/cameras/camera_array_initializer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/live_stream.py` & `pyxy3d-0.1.5/pyxy3d/cameras/live_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/cameras/synchronizer.py` & `pyxy3d-0.1.5/pyxy3d/cameras/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/configurator.py` & `pyxy3d-0.1.5/pyxy3d/configurator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/export.py` & `pyxy3d-0.1.5/pyxy3d/export.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 18:40:23 2023 UTC, .py size: 16022 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 17e7 9564 963e 0000  o..........d.>..
+00000000: 6f0d 0d0a 0000 0000 5f24 9764 963e 0000  o......._$.d.>..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c00 5a01 6501  d.l.Z.d.d.l.Z.e.
 00000040: 6a02 a003 6504 a101 5a02 6400 6402 6c05  j...e...Z.d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6501  m.Z.m.Z.m.Z...e.
 00000060: 6a02 a003 6504 a101 5a02 6400 6403 6c09  j...e...Z.d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun 10 20:29:24 2023 UTC, .py size: 11310 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 24dd 8464 2e2c 0000  o.......$..d.,..
+00000000: 6f0d 0d0a 0000 0000 6124 9764 2e2c 0000  o.......a$.d.,..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7001 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6402 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6403 6c09 6d0a 5a0a 6d0b 5a0b 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6401 6c0c 5a0d 6400 6404 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -228,15 +228,15 @@
 00000e30: 696e 2074 6865 2072 6563 6f72 6469 6e67  in the recording
 00000e40: 2064 6972 6563 746f 7279 206e 616d 6564   directory named
 00000e50: 2060 7879 7a5f 5452 4143 4b45 524e 414d   `xyz_TRACKERNAM
 00000e60: 452e 6373 7660 0a20 2020 2020 2020 2072  E.csv`.        r
 00000e70: 6200 0000 7263 0000 0029 0672 3900 0000  b...rc...).r9...
 00000e80: 7260 0000 0072 3b00 0000 7202 0000 0072  r`...r;...r....r
 00000e90: 6100 0000 724a 0000 0029 0372 4200 0000  a...rJ...).rB...
-00000ea0: 5a0a 7879 7a5f 6f75 7470 7574 da0b 7461  Z.xyz_output..ta
+00000ea0: 5a0a 7879 7a5f 6f75 7470 7574 5a0b 7461  Z.xyz_outputZ.ta
 00000eb0: 7267 6574 5f70 6174 6872 4700 0000 7247  rget_pathrG...rG
 00000ec0: 0000 0072 4800 0000 da1b 6375 7272 656e  ...rH.....curren
 00000ed0: 745f 7365 6c65 6374 696f 6e5f 7072 6f63  t_selection_proc
 00000ee0: 6573 7365 6484 0000 0073 0600 0000 1405  essed....s......
 00000ef0: 0c01 0802 7a30 506f 7374 5072 6f63 6573  ....z0PostProces
 00000f00: 7369 6e67 5769 6467 6574 2e63 7572 7265  singWidget.curre
 00000f10: 6e74 5f73 656c 6563 7469 6f6e 5f70 726f  nt_selection_pro
@@ -244,26 +244,26 @@
 00000f30: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
 00000f40: 2800 0000 7c00 6a00 a001 a100 6400 7501  (...|.j.....d.u.
 00000f50: 7210 7c00 6a00 a001 a100 a002 a100 7d01  r.|.j.........}.
 00000f60: 7c01 5300 6400 7d01 7c01 5300 725d 0000  |.S.d.}.|.S.r]..
 00000f70: 0029 0372 3200 0000 725e 0000 0072 5f00  .).r2...r^...r_.
 00000f80: 0000 2902 7242 0000 00da 0d61 6374 6976  ..).rB.....activ
 00000f90: 655f 666f 6c64 6572 7247 0000 0072 4700  e_folderrG...rG.
-00000fa0: 0000 7248 0000 0072 6900 0000 8e00 0000  ..rH...ri.......
+00000fa0: 0000 7248 0000 0072 6800 0000 8e00 0000  ..rH...rh.......
 00000fb0: 730a 0000 000e 020e 0104 0304 ff04 017a  s..............z
 00000fc0: 2250 6f73 7450 726f 6365 7373 696e 6757  "PostProcessingW
 00000fd0: 6964 6765 742e 6163 7469 7665 5f66 6f6c  idget.active_fol
 00000fe0: 6465 7263 0100 0000 0000 0000 0000 0000  derc............
 00000ff0: 0200 0000 0400 0000 4300 0000 7324 0000  ........C...s$..
 00001000: 0074 007c 006a 016a 027c 006a 0383 027d  .t.|.j.j.|.j...}
 00001010: 0174 04a0 0564 017c 019b 009d 02a1 0101  .t...d.|........
 00001020: 007c 0153 0029 024e 7a19 4163 7469 7665  .|.S.).Nz.Active
 00001030: 2072 6563 6f72 6469 6e67 2070 6174 6820   recording path 
 00001040: 6973 2029 0672 0200 0000 722b 0000 0072  is ).r....r+...r
-00001050: 5900 0000 7269 0000 0072 4b00 0000 724c  Y...ri...rK...rL
+00001050: 5900 0000 7268 0000 0072 4b00 0000 724c  Y...rh...rK...rL
 00001060: 0000 0029 0272 4200 0000 7255 0000 0072  ...).rB...rU...r
 00001070: 4700 0000 7247 0000 0072 4800 0000 7235  G...rG...rH...r5
 00001080: 0000 0096 0000 0073 0600 0000 1002 1001  .......s........
 00001090: 0401 7a2a 506f 7374 5072 6f63 6573 7369  ..z*PostProcessi
 000010a0: 6e67 5769 6467 6574 2e61 6374 6976 655f  ngWidget.active_
 000010b0: 7265 636f 7264 696e 675f 7061 7468 6301  recording_pathc.
 000010c0: 0000 0000 0000 0000 0000 0003 0000 0007  ................
@@ -275,17 +275,17 @@
 00001120: 782c 792c 7a29 2065 7374 696d 6174 6573  x,y,z) estimates
 00001130: 7a13 286e 6f20 7072 6f63 6573 7365 6420  z.(no processed 
 00001140: 6461 7461 297a 173c 6469 7620 616c 6967  data)z.<div alig
 00001150: 6e3d 2763 656e 7465 7227 3e3c 623e 7a0a  n='center'><b>z.
 00001160: 2054 7261 636b 6572 3a20 da01 207a 0b20   Tracker: .. z. 
 00001170: 3c2f 623e 3c2f 6469 763e 2907 7249 0000  </b></div>).rI..
 00001180: 0072 4a00 0000 7239 0000 0072 6000 0000  .rJ...r9...r`...
-00001190: 723b 0000 00da 0574 6974 6c65 7269 0000  r;.....titleri..
+00001190: 723b 0000 00da 0574 6974 6c65 7268 0000  r;.....titlerh..
 000011a0: 0029 0372 4200 0000 da06 7375 6666 6978  .).rB.....suffix
-000011b0: 726b 0000 0072 4700 0000 7247 0000 0072  rk...rG...rG...r
+000011b0: 726a 0000 0072 4700 0000 7247 0000 0072  rj...rG...rG...r
 000011c0: 4800 0000 da0e 7669 7a5f 7469 746c 655f  H.....viz_title_
 000011d0: 6874 6d6c 9c00 0000 730a 0000 000a 0206  html....s.......
 000011e0: 0104 0226 0204 027a 2350 6f73 7450 726f  ...&...z#PostPro
 000011f0: 6365 7373 696e 6757 6964 6765 742e 7669  cessingWidget.vi
 00001200: 7a5f 7469 746c 655f 6874 6d6c 6301 0000  z_title_htmlc...
 00001210: 0000 0000 0000 0000 0001 0000 0004 0000  ................
 00001220: 0043 0000 0073 b200 0000 7c00 a000 7401  .C...s....|...t.
@@ -345,15 +345,15 @@
 00001580: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
 00001590: 0000 0300 0000 4300 0000 7320 0000 007c  ......C...s ...|
 000015a0: 006a 00a0 01a1 0072 0d7c 017c 006a 027c  .j.....r.|.|.j.|
 000015b0: 006a 003c 0064 0053 0009 0064 0053 0072  .j.<.d.S...d.S.r
 000015c0: 5d00 0000 2903 7249 0000 0072 4a00 0000  ]...).rI...rJ...
 000015d0: 7231 0000 0029 0272 4200 0000 5a0c 6375  r1...).rB...Z.cu
 000015e0: 7273 6f72 5f76 616c 7565 7247 0000 0072  rsor_valuerG...r
-000015f0: 4700 0000 7248 0000 0072 7800 0000 c400  G...rH...rx.....
+000015f0: 4700 0000 7248 0000 0072 7700 0000 c400  G...rH...rw.....
 00001600: 0000 7306 0000 000a 0110 0106 047a 2c50  ..s..........z,P
 00001610: 6f73 7450 726f 6365 7373 696e 6757 6964  ostProcessingWid
 00001620: 6765 742e 7374 6f72 655f 7379 6e63 5f69  get.store_sync_i
 00001630: 6e64 6578 5f63 7572 736f 7263 0100 0000  ndex_cursorc....
 00001640: 0000 0000 0000 0000 0300 0000 0400 0000  ................
 00001650: 4300 0000 7344 0000 007c 006a 0064 0175  C...sD...|.j.d.u
 00001660: 0172 1b74 017c 006a 026a 037c 006a 0083  .r.t.|.j.j.|.j..
@@ -361,22 +361,22 @@
 00001680: 0274 07a0 087c 02a1 0101 0064 0153 0074  .t...|.....d.S.t
 00001690: 09a0 0a64 02a1 0101 0064 0153 0029 037a  ...d.....d.S.).z
 000016a0: 3a4f 7065 6e73 2074 6865 2063 7572 7265  :Opens the curre
 000016b0: 6e74 6c79 2061 6374 6976 6520 666f 6c64  ntly active fold
 000016c0: 6572 2069 6e20 6120 7379 7374 656d 2066  er in a system f
 000016d0: 696c 6520 6272 6f77 7365 724e 7a12 4e6f  ile browserNz.No
 000016e0: 2066 6f6c 6465 7220 7365 6c65 6374 6564   folder selected
-000016f0: 290b 7269 0000 0072 0200 0000 722b 0000  ).ri...r....r+..
+000016f0: 290b 7268 0000 0072 0200 0000 722b 0000  ).rh...r....r+..
 00001700: 0072 5900 0000 720b 0000 005a 0d66 726f  .rY...r....Z.fro
 00001710: 6d4c 6f63 616c 4669 6c65 da03 7374 7272  mLocalFile..strr
 00001720: 0c00 0000 5a07 6f70 656e 5572 6c72 4b00  ....Z.openUrlrK.
 00001730: 0000 da04 7761 726e 2903 7242 0000 00da  ....warn).rB....
 00001740: 0b66 6f6c 6465 725f 7061 7468 da03 7572  .folder_path..ur
 00001750: 6c72 4700 0000 7247 0000 0072 4800 0000  lrG...rG...rH...
-00001760: 727b 0000 00cc 0000 0073 0a00 0000 0a02  r{.......s......
+00001760: 727a 0000 00cc 0000 0073 0a00 0000 0a02  rz.......s......
 00001770: 1001 0e01 0e01 0e02 7a20 506f 7374 5072  ........z PostPr
 00001780: 6f63 6573 7369 6e67 5769 6467 6574 2e6f  ocessingWidget.o
 00001790: 7065 6e5f 666f 6c64 6572 6301 0000 0000  pen_folderc.....
 000017a0: 0000 0000 0000 0004 0000 0005 0000 0003  ................
 000017b0: 0000 0073 8000 0000 7400 8801 6a01 6a02  ...s....t...j.j.
 000017c0: 8801 6a03 8302 8900 7404 a005 6401 8800  ..j.....t...d...
 000017d0: 9b00 9d02 a101 0100 8801 6a06 a007 a100  ..........j.....
@@ -414,15 +414,15 @@
 000019d0: 7472 637a 0f53 6176 696e 6720 6461 7461  trcz.Saving data
 000019e0: 2074 6f20 2911 724b 0000 0072 4c00 0000   to ).rK...rL...
 000019f0: 7227 0000 0072 2200 0000 7230 0000 00da  r'...r"...r0....
 00001a00: 1264 6973 6162 6c65 5f61 6c6c 5f69 6e70  .disable_all_inp
 00001a10: 7574 735a 0a63 7265 6174 655f 7879 7a72  utsZ.create_xyzr
 00001a20: 0200 0000 7249 0000 00da 0670 6172 656e  ....rI.....paren
 00001a30: 7472 5300 0000 7207 0000 0072 3900 0000  trS...r....r9...
-00001a40: 7260 0000 00da 0576 616c 7565 727c 0000  r`.....valuer|..
+00001a40: 7260 0000 00da 0576 616c 7565 727b 0000  r`.....valuer{..
 00001a50: 00da 0465 6d69 7429 02da 0d61 6374 6976  ...emit)...activ
 00001a60: 655f 636f 6e66 6967 5a08 7472 635f 7061  e_configZ.trc_pa
 00001a70: 7468 a903 da0e 7265 636f 7264 696e 675f  th....recording_
 00001a80: 7061 7468 7242 0000 005a 0c74 7261 636b  pathrB...Z.track
 00001a90: 6572 5f65 6e75 6d72 4700 0000 7248 0000  er_enumrG...rH..
 00001aa0: 00da 1170 726f 6365 7373 696e 675f 776f  ...processing_wo
 00001ab0: 726b 6572 df00 0000 731c 0000 0010 0108  rker....s.......
@@ -430,21 +430,21 @@
 00001ad0: 0302 0310 0104 ff0e 037a 3f50 6f73 7450  .........z?PostP
 00001ae0: 726f 6365 7373 696e 6757 6964 6765 742e  rocessingWidget.
 00001af0: 7072 6f63 6573 735f 6375 7272 656e 742e  process_current.
 00001b00: 3c6c 6f63 616c 733e 2e70 726f 6365 7373  <locals>.process
 00001b10: 696e 675f 776f 726b 6572 7247 0000 0054  ing_workerrG...T
 00001b20: 2903 da06 7461 7267 6574 da04 6172 6773  )...target..args
 00001b30: da06 6461 656d 6f6e 290b 7202 0000 0072  ..daemon).r....r
-00001b40: 2b00 0000 7259 0000 0072 6900 0000 724b  +...rY...ri...rK
+00001b40: 2b00 0000 7259 0000 0072 6800 0000 724b  +...rY...rh...rK
 00001b50: 0000 0072 4c00 0000 7239 0000 0072 6000  ...rL...r9...r`.
 00001b60: 0000 723b 0000 0072 0300 0000 da05 7374  ..r;...r......st
 00001b70: 6172 7429 0472 4200 0000 5a15 7265 636f  art).rB...Z.reco
 00001b80: 7264 696e 675f 636f 6e66 6967 5f74 6f6d  rding_config_tom
-00001b90: 6c72 8900 0000 da06 7468 7265 6164 7247  lr......threadrG
-00001ba0: 0000 0072 8700 0000 7248 0000 0072 7a00  ...r....rH...rz.
+00001b90: 6c72 8800 0000 da06 7468 7265 6164 7247  lr......threadrG
+00001ba0: 0000 0072 8600 0000 7248 0000 0072 7900  ...r....rH...ry.
 00001bb0: 0000 d500 0000 7312 0000 0010 0110 010a  ......s.........
 00001bc0: 0112 010a 0110 0110 040e 140c 017a 2450  .............z$P
 00001bd0: 6f73 7450 726f 6365 7373 696e 6757 6964  ostProcessingWid
 00001be0: 6765 742e 7072 6f63 6573 735f 6375 7272  get.process_curr
 00001bf0: 656e 7463 0100 0000 0000 0000 0000 0000  entc............
 00001c00: 0300 0000 0400 0000 4300 0000 735a 0000  ........C...sZ..
 00001c10: 0074 007c 006a 0183 017d 0174 02a0 0364  .t.|.j...}.t...d
@@ -458,18 +458,18 @@
 00001c90: 2063 616d 6572 6120 6172 7261 7920 7374   camera array st
 00001ca0: 6f72 6564 2069 6e20 636f 6e66 6967 2e74  ored in config.t
 00001cb0: 6f6d 6c20 696e 2029 0d72 2700 0000 7235  oml in ).r'...r5
 00001cc0: 0000 0072 4b00 0000 724c 0000 0072 3600  ...rK...rL...r6.
 00001cd0: 0000 7237 0000 005a 1375 7064 6174 655f  ..r7...Z.update_
 00001ce0: 6361 6d65 7261 5f61 7272 6179 7251 0000  camera_arrayrQ..
 00001cf0: 0072 3a00 0000 da07 7365 7454 6578 7472  .r:.....setTextr
-00001d00: 6d00 0000 da17 7570 6461 7465 5f65 6e61  m.....update_ena
+00001d00: 6c00 0000 da17 7570 6461 7465 5f65 6e61  l.....update_ena
 00001d10: 626c 6564 5f64 6973 6162 6c65 64da 1675  bled_disabled..u
 00001d20: 7064 6174 655f 736c 6964 6572 5f70 6f73  pdate_slider_pos
-00001d30: 6974 696f 6e29 0372 4200 0000 7286 0000  ition).rB...r...
+00001d30: 6974 696f 6e29 0372 4200 0000 7285 0000  ition).rB...r...
 00001d40: 0072 4300 0000 7247 0000 0072 4700 0000  .rC...rG...rG...
 00001d50: 7248 0000 0072 3f00 0000 f700 0000 7310  rH...r?.......s.
 00001d60: 0000 000a 0212 0108 010c 0208 020e 0108  ................
 00001d70: 010c 017a 2750 6f73 7450 726f 6365 7373  ...z'PostProcess
 00001d80: 696e 6757 6964 6765 742e 7265 6672 6573  ingWidget.refres
 00001d90: 685f 7669 7375 616c 697a 6572 6301 0000  h_visualizerc...
 00001da0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
@@ -479,89 +479,89 @@
 00001de0: 6a04 6a05 a001 6401 a101 0100 6402 5300  j.j...d.....d.S.
 00001df0: 2903 7a39 7573 6564 2074 6f20 746f 6767  ).z9used to togg
 00001e00: 6c65 206f 6666 2061 6c6c 2069 6e70 7574  le off all input
 00001e10: 7320 7769 6c6c 2070 726f 6365 7373 696e  s will processin
 00001e20: 6720 6973 2067 6f69 6e67 206f 6e46 4ea9  g is going onFN.
 00001e30: 0672 3200 0000 da0a 7365 7445 6e61 626c  .r2.....setEnabl
 00001e40: 6564 7239 0000 0072 3d00 0000 7237 0000  edr9...r=...r7..
-00001e50: 0072 7600 0000 7250 0000 0072 4700 0000  .rv...rP...rG...
-00001e60: 7247 0000 0072 4800 0000 7282 0000 0004  rG...rH...r.....
+00001e50: 0072 7500 0000 7250 0000 0072 4700 0000  .ru...rP...rG...
+00001e60: 7247 0000 0072 4800 0000 7281 0000 0004  rG...rH...r.....
 00001e70: 0100 0073 0800 0000 0c02 0c01 0c02 1201  ...s............
 00001e80: 7a27 506f 7374 5072 6f63 6573 7369 6e67  z'PostProcessing
 00001e90: 5769 6467 6574 2e64 6973 6162 6c65 5f61  Widget.disable_a
 00001ea0: 6c6c 5f69 6e70 7574 7363 0100 0000 0000  ll_inputsc......
 00001eb0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001ec0: 0000 7292 0000 0029 037a a20a 2020 2020  ..r....).z..    
+00001ec0: 0000 7291 0000 0029 037a a20a 2020 2020  ..r....).z..    
 00001ed0: 2020 2020 6166 7465 7220 7072 6f63 6573      after proces
 00001ee0: 7369 6e67 2063 6f6d 706c 6574 6573 2c20  sing completes, 
 00001ef0: 7377 6974 6865 7320 6576 6572 7974 6869  swithes everythi
 00001f00: 6e67 206f 6e20 6167 6169 6e2c 0a20 2020  ng on again,.   
 00001f10: 2020 2020 2062 7574 2066 696e 6520 7475       but fine tu
 00001f20: 6e69 6e67 206f 6620 656e 6162 6c65 2f64  ning of enable/d
 00001f30: 6973 6162 6c65 2077 696c 6c20 6861 7070  isable will happ
 00001f40: 656e 2077 6974 6820 7365 6c66 2e75 7064  en with self.upd
 00001f50: 6174 655f 656e 6162 6c65 645f 6469 7361  ate_enabled_disa
 00001f60: 626c 6564 0a20 2020 2020 2020 2054 4e72  bled.        TNr
-00001f70: 9300 0000 7250 0000 0072 4700 0000 7247  ....rP...rG...rG
-00001f80: 0000 0072 4800 0000 727d 0000 000c 0100  ...rH...r}......
+00001f70: 9200 0000 7250 0000 0072 4700 0000 7247  ....rP...rG...rG
+00001f80: 0000 0072 4800 0000 727c 0000 000c 0100  ...rH...r|......
 00001f90: 0073 0800 0000 0c05 0c01 0c02 1201 7a26  .s............z&
 00001fa0: 506f 7374 5072 6f63 6573 7369 6e67 5769  PostProcessingWi
 00001fb0: 6467 6574 2e65 6e61 626c 655f 616c 6c5f  dget.enable_all_
 00001fc0: 696e 7075 7473 6301 0000 0000 0000 0000  inputsc.........
 00001fd0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
 00001fe0: 4600 0000 7c00 6a00 a001 a100 7214 7c00  F...|.j.....r.|.
 00001ff0: 6a02 a003 6401 a101 0100 7c00 6a04 6a05  j...d.....|.j.j.
 00002000: a003 6402 a101 0100 6400 5300 7c00 6a02  ..d.....d.S.|.j.
 00002010: a003 6402 a101 0100 7c00 6a04 6a05 a003  ..d.....|.j.j...
 00002020: 6401 a101 0100 6400 5300 2903 4e46 5429  d.....d.S.).NFT)
 00002030: 0672 4900 0000 724a 0000 0072 3d00 0000  .rI...rJ...r=...
-00002040: 7294 0000 0072 3700 0000 7276 0000 0072  r....r7...rv...r
+00002040: 7293 0000 0072 3700 0000 7275 0000 0072  r....r7...ru...r
 00002050: 5000 0000 7247 0000 0072 4700 0000 7248  P...rG...rG...rH
-00002060: 0000 0072 9000 0000 1701 0000 730a 0000  ...r........s...
+00002060: 0000 0072 8f00 0000 1701 0000 730a 0000  ...r........s...
 00002070: 000a 010c 0212 010c 0412 017a 2c50 6f73  ...........z,Pos
 00002080: 7450 726f 6365 7373 696e 6757 6964 6765  tProcessingWidge
 00002090: 742e 7570 6461 7465 5f65 6e61 626c 6564  t.update_enabled
 000020a0: 5f64 6973 6162 6c65 6463 0100 0000 0000  _disabledc......
 000020b0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
 000020c0: 0000 7342 0000 007c 006a 007c 006a 01a0  ..sB...|.j.|.j..
 000020d0: 02a1 0076 0072 1e7c 006a 017c 006a 0019  ...v.r.|.j.|.j..
 000020e0: 007d 017c 006a 036a 04a0 057c 01a1 0101  .}.|.j.j...|....
 000020f0: 007c 006a 036a 06a0 077c 01a1 0101 0064  .|.j.j...|.....d
 00002100: 0053 0009 0064 0053 0072 5d00 0000 2908  .S...d.S.r]...).
 00002110: 7249 0000 0072 3100 0000 da04 6b65 7973  rI...r1.....keys
-00002120: 7237 0000 0072 7600 0000 da08 7365 7456  r7...rv.....setV
+00002120: 7237 0000 0072 7500 0000 da08 7365 7456  r7...ru.....setV
 00002130: 616c 7565 da0a 7669 7375 616c 697a 6572  alue..visualizer
 00002140: da0e 6469 7370 6c61 795f 706f 696e 7473  ..display_points
 00002150: 2902 7242 0000 005a 1161 6374 6976 655f  ).rB...Z.active_
 00002160: 7379 6e63 5f69 6e64 6578 7247 0000 0072  sync_indexrG...r
-00002170: 4700 0000 7248 0000 0072 9100 0000 2201  G...rH...r....".
+00002170: 4700 0000 7248 0000 0072 9000 0000 2201  G...rH...r....".
 00002180: 0000 730a 0000 0010 020c 010e 0112 0106  ..s.............
 00002190: 027a 2b50 6f73 7450 726f 6365 7373 696e  .z+PostProcessin
 000021a0: 6757 6964 6765 742e 7570 6461 7465 5f73  gWidget.update_s
 000021b0: 6c69 6465 725f 706f 7369 7469 6f6e 291d  lider_position).
 000021c0: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 000021d0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-000021e0: 6d65 5f5f 7209 0000 0072 7c00 0000 7223  me__r....r|...r#
+000021e0: 6d65 5f5f 7209 0000 0072 7b00 0000 7223  me__r....r{...r#
 000021f0: 0000 0072 2e00 0000 7251 0000 0072 3300  ...r....rQ...r3.
 00002200: 0000 da08 7072 6f70 6572 7479 7261 0000  ....propertyra..
-00002210: 0072 4900 0000 da04 626f 6f6c 7268 0000  .rI.....boolrh..
-00002220: 0072 6900 0000 7202 0000 0072 3500 0000  .ri...r....r5...
-00002230: 726d 0000 0072 4000 0000 7241 0000 0072  rm...r@...rA...r
-00002240: 7800 0000 727b 0000 0072 7a00 0000 723f  x...r{...rz...r?
-00002250: 0000 0072 8200 0000 727d 0000 0072 9000  ...r....r}...r..
-00002260: 0000 7291 0000 00da 0d5f 5f63 6c61 7373  ..r......__class
+00002210: 0072 4900 0000 da04 626f 6f6c 7267 0000  .rI.....boolrg..
+00002220: 0072 6800 0000 7202 0000 0072 3500 0000  .rh...r....r5...
+00002230: 726c 0000 0072 4000 0000 7241 0000 0072  rl...r@...rA...r
+00002240: 7700 0000 727a 0000 0072 7900 0000 723f  w...rz...ry...r?
+00002250: 0000 0072 8100 0000 727c 0000 0072 8f00  ...r....r|...r..
+00002260: 0000 7290 0000 00da 0d5f 5f63 6c61 7373  ..r......__class
 00002270: 6365 6c6c 5f5f 7247 0000 0072 4700 0000  cell__rG...rG...
 00002280: 7245 0000 0072 4800 0000 722a 0000 0032  rE...rH...r*...2
 00002290: 0000 0073 3400 0000 0800 0601 1202 0827  ...s4..........'
 000022a0: 080a 020f 0a01 0208 0a01 0e05 020a 0a01  ................
 000022b0: 0207 1001 0205 0a01 080a 0813 080a 0808  ................
 000022c0: 0809 0822 080d 0808 080b 100b 722a 0000  ..."........r*..
 000022d0: 0029 44da 0d70 7978 7933 642e 6c6f 6767  .)D..pyxy3d.logg
 000022e0: 6572 da06 7079 7879 3364 724b 0000 00da  er..pyxy3drK....
-000022f0: 0367 6574 7299 0000 00da 0373 7973 da04  .getr......sys..
+000022f0: 0367 6574 7298 0000 00da 0373 7973 da04  .getr......sys..
 00002300: 6d61 7468 da07 7061 7468 6c69 6272 0200  math..pathlibr..
 00002310: 0000 da09 7468 7265 6164 696e 6772 0300  ....threadingr..
 00002320: 0000 7204 0000 00da 056e 756d 7079 da02  ..r......numpy..
 00002330: 6e70 da05 7175 6575 6572 0500 0000 da06  np..queuer......
 00002340: 7061 6e64 6173 724d 0000 005a 1c70 7978  pandasrM...Z.pyx
 00002350: 7933 642e 7472 6163 6b65 7273 2e74 7261  y3d.trackers.tra
 00002360: 636b 6572 5f65 6e75 6d72 0600 0000 5a0d  cker_enumr....Z.
```

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 18:41:03 2023 UTC, .py size: 15210 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3fe7 9564 6a3b 0000  o.......?..dj;..
+00000000: 6f0d 0d0a 0000 0000 7ce9 9564 6a3b 0000  o.......|..dj;..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7e01 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6402 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6403 6c09 6d0a 5a0a 6d0b 5a0b 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6401 6c0c 5a0d 6400 6404 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
```

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/calibrate_capture_volume_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/calibrate_capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/camera_config_dialogue.py` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/camera_config_dialogue.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/camera_summary_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/camera_summary_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/frame_emitter.py` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/frame_emitter.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/charuco_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/charuco_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/extrinsic_calibration_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/extrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/frame_builders/paired_frame_builder.py` & `pyxy3d-0.1.5/pyxy3d/gui/frame_builders/paired_frame_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/icons/pyxy_logo.svg` & `pyxy3d-0.1.5/pyxy3d/gui/icons/pyxy_logo.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/icons/rotate-camera-left.svg` & `pyxy3d-0.1.5/pyxy3d/gui/icons/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/icons/rotate-camera-right.svg` & `pyxy3d-0.1.5/pyxy3d/gui/icons/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/log_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/main_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/main_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/navigation_bars.py` & `pyxy3d-0.1.5/pyxy3d/gui/navigation_bars.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/playback_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/playback_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/post_processing_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/post_processing_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/progress_dialog.py` & `pyxy3d-0.1.5/pyxy3d/gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/recording_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/recording_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/camera_mesh.py` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/camera_mesh.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/playback_triangulation_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/playback_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/gui/vizualize/realtime_triangulation_widget.py` & `pyxy3d-0.1.5/pyxy3d/gui/vizualize/realtime_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/helper.py` & `pyxy3d-0.1.5/pyxy3d/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/interface.py` & `pyxy3d-0.1.5/pyxy3d/interface.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/logger.py` & `pyxy3d-0.1.5/pyxy3d/logger.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/post_processor.py` & `pyxy3d-0.1.5/pyxy3d/post_processor.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 18:18:46 2023 UTC, .py size: 9105 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 06e2 9564 9123 0000  o..........d.#..
+00000000: 6f0d 0d0a 0000 0000 c614 9764 9423 0000  o..........d.#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6402 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
 00000050: 6403 6c07 6d08 5a08 0100 6400 6404 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6400 6401 6c0c  m.Z.m.Z...d.d.l.
 00000070: 5a0c 6400 6401 6c0d 5a0d 6400 6401 6c0e  Z.d.d.l.Z.d.d.l.
@@ -105,277 +105,277 @@
 00000680: 7206 7c00 a000 a100 0100 6700 6700 6700  r.|.......g.g.g.
 00000690: 6700 6401 9c04 7c00 5f01 6700 6700 6700  g.d...|._.g.g.g.
 000006a0: 6700 6700 6700 6700 6700 6700 6402 9c09  g.g.g.g.g.g.d...
 000006b0: 7c00 5f02 7c00 6a03 a004 7c00 6a05 a101  |._.|.j...|.j...
 000006c0: 0100 6403 7d04 7406 a007 6404 a101 0100  ..d.}.t...d.....
 000006d0: 7c00 6a05 a008 a100 6405 6b04 7335 7c00  |.j.....d.k.s5|.
 000006e0: 6a09 a00a a100 73ff 7c00 6a05 a00b a100  j.....s.|.j.....
-000006f0: 7d05 7406 a007 6406 a101 0100 7c00 6a05  }.t...d.....|.j.
+000006f0: 7d05 7406 a00c 6406 a101 0100 7c00 6a05  }.t...d.....|.j.
 00000700: a008 a100 7d06 7c06 6407 1600 6405 6b02  ....}.|.d...d.k.
 00000710: 7259 7c06 6405 6b03 7259 7406 a007 6408  rY|.d.k.rYt...d.
 00000720: 7c00 6a05 a008 a100 9b00 9d02 a101 0100  |.j.............
 00000730: 7c05 6400 7500 7263 7406 a007 6409 a101  |.d.u.rct...d...
-00000740: 0100 6e9c 7c05 6a0c 7c00 5f0c 7c05 6a0d  ..n.|.j.|._.|.j.
-00000750: a00e a100 4400 5d71 5c02 7d07 7d08 7c08  ....D.]q\.}.}.|.
-00000760: 6400 7501 72dd 7406 a007 640a a101 0100  d.u.r.t...d.....
-00000770: 7c02 727f 7c08 6a0f 7d09 6e03 7c08 6a10  |.r.|.j.}.n.|.j.
-00000780: 7d09 7c08 6a11 7d0a 7c08 6a12 7d0b 7c01  }.|.j.}.|.j.}.|.
-00000790: 72b8 7406 a007 640b a101 0100 7c00 6a13  r.t...d.....|.j.
-000007a0: 7c07 1900 a014 7c09 a101 0100 7c00 6a01  |.....|.....|.j.
-000007b0: 640c 1900 a015 7c00 6a0c a101 0100 7c00  d.....|.j.....|.
-000007c0: 6a01 640d 1900 a015 7c07 a101 0100 7c00  j.d.....|.....|.
-000007d0: 6a01 640e 1900 a015 7c0a a101 0100 7c00  j.d.....|.....|.
-000007e0: 6a01 640f 1900 a015 7c0b a101 0100 7c08  j.d.....|.....|.
-000007f0: a016 7c00 6a0c a101 7d0c 7c0c 6400 7501  ..|.j...}.|.d.u.
-00000800: 72dd 7c00 6a02 a017 a100 a00e a100 4400  r.|.j.........D.
-00000810: 5d13 5c02 7d0d 7d0e 7406 a007 6410 a101  ].\.}.}.t...d...
-00000820: 0100 7c00 6a02 7c0d 1900 a018 7c0c 7c0d  ..|.j.|.....|.|.
+00000740: 0100 6e9c 7c05 6a0d 7c00 5f0d 7c05 6a0e  ..n.|.j.|._.|.j.
+00000750: a00f a100 4400 5d71 5c02 7d07 7d08 7c08  ....D.]q\.}.}.|.
+00000760: 6400 7501 72dd 7406 a00c 640a a101 0100  d.u.r.t...d.....
+00000770: 7c02 727f 7c08 6a10 7d09 6e03 7c08 6a11  |.r.|.j.}.n.|.j.
+00000780: 7d09 7c08 6a12 7d0a 7c08 6a13 7d0b 7c01  }.|.j.}.|.j.}.|.
+00000790: 72b8 7406 a00c 640b a101 0100 7c00 6a14  r.t...d.....|.j.
+000007a0: 7c07 1900 a015 7c09 a101 0100 7c00 6a01  |.....|.....|.j.
+000007b0: 640c 1900 a016 7c00 6a0d a101 0100 7c00  d.....|.j.....|.
+000007c0: 6a01 640d 1900 a016 7c07 a101 0100 7c00  j.d.....|.....|.
+000007d0: 6a01 640e 1900 a016 7c0a a101 0100 7c00  j.d.....|.....|.
+000007e0: 6a01 640f 1900 a016 7c0b a101 0100 7c08  j.d.....|.....|.
+000007f0: a017 7c00 6a0d a101 7d0c 7c0c 6400 7501  ..|.j...}.|.d.u.
+00000800: 72dd 7c00 6a02 a018 a100 a00f a100 4400  r.|.j.........D.
+00000810: 5d13 5c02 7d0d 7d0e 7406 a00c 6410 a101  ].\.}.}.t...d...
+00000820: 0100 7c00 6a02 7c0d 1900 a019 7c0c 7c0d  ..|.j.|.....|.|.
 00000830: 1900 a101 0100 71c9 716c 7c04 73f3 7c00  ......q.ql|.s.|.
 00000840: 6a09 a00a a100 72f3 7406 a007 6411 a101  j.....r.t...d...
-00000850: 0100 6412 7d04 7c00 6a03 a019 7c00 6a05  ..d.}.|.j...|.j.
+00000850: 0100 6412 7d04 7c00 6a03 a01a 7c00 6a05  ..d.}.|.j...|.j.
 00000860: a101 0100 7c00 6a05 a008 a100 6405 6b04  ....|.j.....d.k.
 00000870: 7335 7c00 6a09 a00a a100 7235 7c01 9001  s5|.j.....r5|...
 00000880: 721f 7406 a007 6413 a101 0100 7c00 6a03  r.t...d.....|.j.
-00000890: 6a1a 4400 5d0a 7d07 7c00 6a13 7c07 1900  j.D.].}.|.j.|...
-000008a0: a01b a100 0100 9001 710b 7406 a007 6414  ........q.t...d.
-000008b0: a101 0100 7c00 a01c a100 0100 7406 a007  ....|.......t...
-000008c0: 6415 a101 0100 7c03 9001 722b 7c00 a01d  d.....|...r+|...
-000008d0: a100 0100 7c00 6a09 a01e a100 0100 6403  ....|.j.......d.
-000008e0: 7c00 5f1f 7406 a007 6416 a101 0100 6400  |._.t...d.....d.
+00000890: 6a1b 4400 5d0a 7d07 7c00 6a14 7c07 1900  j.D.].}.|.j.|...
+000008a0: a01c a100 0100 9001 710b 7406 a007 6414  ........q.t...d.
+000008b0: a101 0100 7c00 a01d a100 0100 7406 a007  ....|.......t...
+000008c0: 6415 a101 0100 7c03 9001 722b 7c00 a01e  d.....|...r+|...
+000008d0: a100 0100 7c00 6a09 a01f a100 0100 6403  ....|.j.......d.
+000008e0: 7c00 5f20 7406 a007 6416 a101 0100 6400  |._ t...d.....d.
 000008f0: 5300 2917 4e29 0472 1300 0000 7228 0000  S.).N).r....r(..
 00000900: 00da 0b66 7261 6d65 5f69 6e64 6578 da0a  ...frame_index..
 00000910: 6672 616d 655f 7469 6d65 2909 7213 0000  frame_time).r...
 00000920: 0072 2800 0000 7231 0000 0072 3200 0000  .r(...r1...r2...
 00000930: da08 706f 696e 745f 6964 da09 696d 675f  ..point_id..img_
 00000940: 6c6f 635f 78da 0969 6d67 5f6c 6f63 5f79  loc_x..img_loc_y
 00000950: da09 6f62 6a5f 6c6f 635f 78da 096f 626a  ..obj_loc_x..obj
 00000960: 5f6c 6f63 5f79 467a 2645 6e74 6572 696e  _loc_yFz&Enterin
 00000970: 6720 5361 7665 2064 6174 6120 776f 726b  g Save data work
 00000980: 6572 206c 6f6f 7020 656e 7465 7265 6472  er loop enteredr
-00000990: 0100 0000 7a1e 4765 7474 696e 6720 7369  ....z.Getting si
-000009a0: 647a 6520 6f66 2073 796e 6320 7061 636b  dze of sync pack
-000009b0: 6574 2071 e919 0000 007a 3153 697a 6520  et q.....z1Size 
-000009c0: 6f66 2075 6e73 6176 6564 2066 7261 6d65  of unsaved frame
-000009d0: 7320 6f6e 2074 6865 2072 6563 6f72 6469  s on the recordi
-000009e0: 6e67 2071 7565 7565 2069 7320 7a33 456e  ng queue is z3En
-000009f0: 6420 6f66 2073 796e 6320 7061 636b 6574  d of sync packet
-00000a00: 7320 7369 676e 616c 6564 2e2e 2e62 7265  s signaled...bre
-00000a10: 616b 696e 6720 7265 636f 7264 206c 6f6f  aking record loo
-00000a20: 707a 1b50 726f 6365 7373 696f 6e67 2066  pz.Processiong f
-00000a30: 7261 6d65 2070 6163 6b65 742e 2e2e 7a0d  rame packet...z.
-00000a40: 5772 6974 696e 6720 6672 616d 6572 1300  Writing framer..
-00000a50: 0000 7228 0000 0072 3100 0000 7232 0000  ..r(...r1...r2..
-00000a60: 007a 2545 7874 656e 6469 6e67 2074 6964  .z%Extending tid
-00000a70: 7920 7461 626c 6520 6f66 2070 6f69 6e74  y table of point
-00000a80: 2068 6973 746f 7279 7a21 5361 7665 2066   historyz!Save f
-00000a90: 7261 6d65 2077 6f72 6b65 7220 7769 6e64  rame worker wind
-00000aa0: 696e 6720 646f 776e 2e2e 2e54 7a1a 7265  ing down...Tz.re
-00000ab0: 6c65 6173 696e 6720 7669 6465 6f20 7772  leasing video wr
-00000ac0: 6974 6572 732e 2e2e 7a21 496e 6974 6961  iters...z!Initia
-00000ad0: 7465 2073 746f 7269 6e67 206f 6620 6672  te storing of fr
-00000ae0: 616d 6520 6869 7374 6f72 797a 2149 6e69  ame historyz!Ini
-00000af0: 7469 6174 6520 7374 6f72 696e 6720 6f66  tiate storing of
-00000b00: 2070 6f69 6e74 2068 6973 746f 7279 7a27   point historyz'
-00000b10: 4162 6f75 7420 746f 2065 6d69 7420 6061  About to emit `a
-00000b20: 6c6c 2066 7261 6d65 7320 7361 7665 6460  ll frames saved`
-00000b30: 2073 6967 6e61 6c29 2072 2d00 0000 da0d   signal) r-.....
-00000b40: 6672 616d 655f 6869 7374 6f72 79da 1270  frame_history..p
-00000b50: 6f69 6e74 5f64 6174 615f 6869 7374 6f72  oint_data_histor
-00000b60: 7972 0b00 0000 da19 7375 6273 6372 6962  yr......subscrib
-00000b70: 655f 746f 5f73 796e 635f 7061 636b 6574  e_to_sync_packet
-00000b80: 7372 1500 0000 7220 0000 0072 2100 0000  sr....r ...r!...
-00000b90: da05 7173 697a 6572 1400 0000 da06 6973  ..qsizer......is
-00000ba0: 5f73 6574 da03 6765 7472 1300 0000 da0d  _set..getr......
-00000bb0: 6672 616d 655f 7061 636b 6574 7372 1d00  frame_packetsr..
-00000bc0: 0000 da11 6672 616d 655f 7769 7468 5f70  ....frame_with_p
-00000bd0: 6f69 6e74 73da 0566 7261 6d65 7231 0000  oints..framer1..
-00000be0: 0072 3200 0000 721b 0000 00da 0577 7269  .r2...r......wri
-00000bf0: 7465 da06 6170 7065 6e64 da0d 746f 5f74  te..append..to_t
-00000c00: 6964 795f 7461 626c 65da 0463 6f70 79da  idy_table..copy.
-00000c10: 0665 7874 656e 64da 1572 656c 6561 7365  .extend..release
-00000c20: 5f73 796e 635f 7061 636b 6574 5f71 da05  _sync_packet_q..
-00000c30: 706f 7274 73da 0772 656c 6561 7365 da13  ports..release..
-00000c40: 7374 6f72 655f 6672 616d 655f 6869 7374  store_frame_hist
-00000c50: 6f72 7972 3000 0000 da05 636c 6561 7272  oryr0.....clearr
-00000c60: 1200 0000 290f 7216 0000 0072 2e00 0000  ....).r....r....
-00000c70: 722f 0000 0072 3000 0000 5a21 7379 6e63  r/...r0...Z!sync
-00000c80: 726f 6e69 7a65 725f 7375 6273 6372 6970  ronizer_subscrip
-00000c90: 7469 6f6e 5f72 656c 6561 7365 64da 0b73  tion_released..s
-00000ca0: 796e 635f 7061 636b 6574 da07 6261 636b  ync_packet..back
-00000cb0: 6c6f 6772 2800 0000 da0c 6672 616d 655f  logr(.....frame_
-00000cc0: 7061 636b 6574 7241 0000 0072 3100 0000  packetrA...r1...
-00000cd0: 7232 0000 005a 0e6e 6577 5f74 6964 795f  r2...Z.new_tidy_
-00000ce0: 7461 626c 65da 036b 6579 da05 7661 6c75  table..key..valu
-00000cf0: 6572 1900 0000 7219 0000 0072 1a00 0000  er....r....r....
-00000d00: da10 7361 7665 5f64 6174 615f 776f 726b  ..save_data_work
-00000d10: 6572 3700 0000 7388 0000 0004 0208 0102  er7...s.........
-00000d20: 0402 0102 0102 0108 fc02 0802 0102 0102  ................
-00000d30: 0102 0102 0102 0102 0102 0108 f70e 0d04  ................
-00000d40: 010a 0318 010a 010a 030a 0114 0116 0108  ................
-00000d50: 020a 0202 0108 0212 0208 010a 0104 0208  ................
-00000d60: 0106 0206 0206 0104 020a 0210 0112 0310  ................
-00000d70: 0110 0110 010c 0208 0116 010a 0116 0102  ................
-00000d80: 800e 020a 0104 010e 0118 d006 350a 010c  ............5...
-00000d90: 0112 010a 0408 010a 0206 0108 010a 0106  ................
-00000da0: 010e 017a 1e56 6964 656f 5265 636f 7264  ...z.VideoRecord
-00000db0: 6572 2e73 6176 655f 6461 7461 5f77 6f72  er.save_data_wor
-00000dc0: 6b65 7263 0100 0000 0000 0000 0000 0000  kerc............
-00000dd0: 0300 0000 0600 0000 4300 0000 734a 0000  ........C...sJ..
-00000de0: 0074 00a0 017c 006a 02a1 017d 0174 0374  .t...|.j...}.t.t
-00000df0: 047c 006a 0564 017c 006a 069b 0064 029d  .|.j.d.|.j...d..
-00000e00: 0383 0283 017d 0274 07a0 0864 037c 029b  .....}.t...d.|..
-00000e10: 009d 02a1 0101 007c 016a 097c 0264 0464  .......|.j.|.d.d
-00000e20: 0564 068d 0301 0064 0053 0029 074e da02  .d.....d.S.).N..
-00000e30: 7879 7a04 2e63 7376 7a16 5374 6f72 696e  xyz..csvz.Storin
-00000e40: 6720 706f 696e 7420 6461 7461 2069 6e20  g point data in 
-00000e50: 4654 a902 da05 696e 6465 78da 0668 6561  FT....index..hea
-00000e60: 6465 7229 0ada 0270 64da 0944 6174 6146  der)...pd..DataF
-00000e70: 7261 6d65 723a 0000 0072 1e00 0000 7202  ramer:...r....r.
-00000e80: 0000 0072 1f00 0000 720c 0000 0072 2000  ...r....r....r .
-00000e90: 0000 7221 0000 00da 0674 6f5f 6373 7629  ..r!.....to_csv)
-00000ea0: 0372 1600 0000 da02 6466 da0f 706f 696e  .r......df..poin
-00000eb0: 745f 6461 7461 5f70 6174 6872 1900 0000  t_data_pathr....
-00000ec0: 7219 0000 0072 1a00 0000 7230 0000 009e  r....r....r0....
-00000ed0: 0000 0073 0800 0000 0c01 1a01 1001 1401  ...s............
-00000ee0: 7a21 5669 6465 6f52 6563 6f72 6465 722e  z!VideoRecorder.
-00000ef0: 7374 6f72 655f 706f 696e 745f 6869 7374  store_point_hist
-00000f00: 6f72 7963 0100 0000 0000 0000 0000 0000  oryc............
-00000f10: 0300 0000 0500 0000 4300 0000 7340 0000  ........C...s@..
-00000f20: 0074 00a0 017c 006a 02a1 017d 0174 0374  .t...|.j...}.t.t
-00000f30: 047c 006a 0564 0183 0283 017d 0274 06a0  .|.j.d.....}.t..
-00000f40: 0764 027c 029b 009d 02a1 0101 007c 016a  .d.|.........|.j
-00000f50: 087c 0264 0364 0464 058d 0301 0064 0053  .|.d.d.d.....d.S
-00000f60: 0029 064e 7a16 6672 616d 655f 7469 6d65  .).Nz.frame_time
-00000f70: 5f68 6973 746f 7279 2e63 7376 7a19 5374  _history.csvz.St
-00000f80: 6f72 696e 6720 6672 616d 6520 6869 7374  oring frame hist
-00000f90: 6f72 7920 746f 2046 5472 5300 0000 2909  ory to FTrS...).
-00000fa0: 7256 0000 0072 5700 0000 7239 0000 0072  rV...rW...r9...r
-00000fb0: 1e00 0000 7202 0000 0072 1f00 0000 7220  ....r....r....r 
-00000fc0: 0000 0072 2100 0000 7258 0000 0029 0372  ...r!...rX...).r
-00000fd0: 1600 0000 7259 0000 005a 0f66 7261 6d65  ....rY...Z.frame
-00000fe0: 5f68 6973 745f 7061 7468 7219 0000 0072  _hist_pathr....r
-00000ff0: 1900 0000 721a 0000 0072 4a00 0000 a400  ....r....rJ.....
-00001000: 0000 7308 0000 000c 0110 0110 0114 017a  ..s............z
-00001010: 2156 6964 656f 5265 636f 7264 6572 2e73  !VideoRecorder.s
-00001020: 746f 7265 5f66 7261 6d65 5f68 6973 746f  tore_frame_histo
-00001030: 7279 6301 0000 0000 0000 0000 0000 0001  ryc.............
-00001040: 0000 0001 0000 0043 0000 0073 0400 0000  .......C...s....
-00001050: 6400 5300 a901 4e72 1900 0000 a901 7216  d.S...Nr......r.
-00001060: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00001070: 0000 da13 7374 6f72 655f 6163 7469 7665  ....store_active
-00001080: 5f63 6f6e 6669 67aa 0000 0073 0200 0000  _config....s....
-00001090: 0401 7a21 5669 6465 6f52 6563 6f72 6465  ..z!VideoRecorde
-000010a0: 722e 7374 6f72 655f 6163 7469 7665 5f63  r.store_active_c
-000010b0: 6f6e 6669 6754 4672 1f00 0000 6305 0000  onfigTFr....c...
-000010c0: 0000 0000 0000 0000 0007 0000 0005 0000  ................
-000010d0: 0043 0000 0073 9800 0000 7400 a001 6401  .C...s....t...d.
-000010e0: 7c01 9b00 9d02 a101 0100 7c01 7c00 5f02  |.........|.|._.
-000010f0: 7c00 6a02 6a03 6402 6402 6403 8d02 0100  |.j.j.d.d.d.....
-00001100: 7c00 6a02 6a04 6a05 6404 6b02 7223 7406  |.j.j.j.d.k.r#t.
-00001110: 7c00 6a02 6a04 6a04 6405 8302 7d05 6e07  |.j.j.j.d...}.n.
-00001120: 7406 7c00 6a02 6a04 6405 8302 7d05 7406  t.|.j.j.d...}.t.
-00001130: 7c00 6a02 6405 8302 7d06 7407 a008 7c05  |.j.d...}.t...|.
-00001140: 7c06 a102 0100 6402 7c00 5f09 740a 7c00  |.....d.|._.t.|.
-00001150: 6a0b 7c02 7c03 7c04 6703 6402 6406 8d03  j.|.|.|.g.d.d...
-00001160: 7c00 5f0c 7c00 6a0c a00d a100 0100 6407  |._.|.j.......d.
-00001170: 5300 2908 61f5 0100 000a 2020 2020 2020  S.).a.....      
-00001180: 2020 4f70 7469 6f6e 2065 7869 7374 7320    Option exists 
-00001190: 746f 206e 6f74 2073 746f 7265 2076 6964  to not store vid
-000011a0: 656f 2069 6620 6f6e 6c79 2069 6e74 6572  eo if only inter
-000011b0: 6573 7465 6420 696e 2067 6574 7469 6e67  ested in getting
-000011c0: 2070 6f69 6e74 7320 6672 6f6d 206f 7269   points from ori
-000011d0: 6769 6e61 6c20 7669 6465 6f0a 2020 2020  ginal video.    
-000011e0: 2020 2020 0a20 2020 2020 2020 2050 6172      .        Par
-000011f0: 656e 7420 6f66 2064 6573 7469 6e61 7469  ent of destinati
-00001200: 6f6e 2066 6f6c 6465 7220 7769 6c6c 2062  on folder will b
-00001210: 6520 7468 6520 736f 7572 6365 206f 6620  e the source of 
-00001220: 7468 6520 636f 6e66 6967 2066 696c 6520  the config file 
-00001230: 7468 6174 2077 696c 6c20 6265 2073 746f  that will be sto
-00001240: 7265 6420 7769 7468 2074 6865 2076 6964  red with the vid
-00001250: 656f 0a20 2020 2020 2020 2054 6869 7320  eo.        This 
-00001260: 656e 6162 6c65 7320 7468 6520 6e65 7374  enables the nest
-00001270: 6564 2070 726f 6365 7373 696e 6720 6f66  ed processing of
-00001280: 2076 6964 656f 7320 2869 2e65 2e20 5265   videos (i.e. Re
-00001290: 636f 7264 696e 675f 3120 7769 6c6c 2073  cording_1 will s
-000012a0: 746f 7265 2074 6865 206d 6169 6e20 636f  tore the main co
-000012b0: 6e66 6967 2e74 6f6d 6c2c 0a20 2020 2020  nfig.toml,.     
-000012c0: 2020 2074 6865 6e20 504f 5345 2073 7562     then POSE sub
-000012d0: 666f 6c64 6572 2077 696c 6c20 7374 6f72  folder will stor
-000012e0: 6520 636f 6e66 6967 2e74 6f6d 6c20 6672  e config.toml fr
-000012f0: 6f6d 2052 6563 6f72 6469 6e67 5f31 292e  om Recording_1).
-00001300: 2045 6163 6820 666f 6c64 6572 2073 686f   Each folder sho
-00001310: 756c 6420 6c61 7267 656c 7920 6265 636f  uld largely beco
-00001320: 6d65 2073 656c 660a 2020 2020 2020 2020  me self.        
-00001330: 636f 6e74 6169 6e65 6420 616e 6420 706f  contained and po
-00001340: 7274 6162 6c65 2066 6f72 2061 6e61 6c79  rtable for analy
-00001350: 7369 7320 2f20 7265 636f 6e73 7472 7563  sis / reconstruc
-00001360: 7469 6f6e 2e0a 2020 2020 2020 2020 7a1e  tion..        z.
-00001370: 416c 6c20 7669 6465 6f20 6461 7461 2074  All video data t
-00001380: 6f20 6265 2073 6176 6564 2074 6f20 5429  o be saved to T)
-00001390: 02da 0865 7869 7374 5f6f 6bda 0770 6172  ...exist_ok..par
-000013a0: 656e 7473 da0b 6361 6c69 6272 6174 696f  ents..calibratio
-000013b0: 6e7a 0b63 6f6e 6669 672e 746f 6d6c 2903  nz.config.toml).
-000013c0: da06 7461 7267 6574 da04 6172 6773 da06  ..target..args..
-000013d0: 6461 656d 6f6e 4e29 0e72 2000 0000 7221  daemonN).r ...r!
-000013e0: 0000 0072 1f00 0000 da05 6d6b 6469 72da  ...r......mkdir.
-000013f0: 0670 6172 656e 74da 0473 7465 6d72 0200  .parent..stemr..
-00001400: 0000 da06 7368 7574 696c da05 636f 7079  ....shutil..copy
-00001410: 3272 1200 0000 7204 0000 0072 5100 0000  2r....r....rQ...
-00001420: 5a10 7265 636f 7264 696e 675f 7468 7265  Z.recording_thre
-00001430: 6164 da05 7374 6172 7429 0772 1600 0000  ad..start).r....
-00001440: 721f 0000 0072 2e00 0000 722f 0000 0072  r....r....r/...r
-00001450: 3000 0000 5a12 736f 7572 6365 5f63 6f6e  0...Z.source_con
-00001460: 6669 675f 7061 7468 5a15 6475 706c 6963  fig_pathZ.duplic
-00001470: 6174 655f 636f 6e66 6967 5f70 6174 6872  ate_config_pathr
-00001480: 1900 0000 7219 0000 0072 1a00 0000 da0f  ....r....r......
-00001490: 7374 6172 745f 7265 636f 7264 696e 67ad  start_recording.
-000014a0: 0000 0073 1a00 0000 100f 0602 1002 0e04  ...s............
-000014b0: 1201 0e02 0c02 0c02 0602 0201 0e01 08ff  ................
-000014c0: 0e03 7a1d 5669 6465 6f52 6563 6f72 6465  ..z.VideoRecorde
-000014d0: 722e 7374 6172 745f 7265 636f 7264 696e  r.start_recordin
-000014e0: 6763 0100 0000 0000 0000 0000 0000 0100  gc..............
-000014f0: 0000 0300 0000 4300 0000 7322 0000 0074  ......C...s"...t
-00001500: 00a0 0164 01a1 0101 007c 006a 02a0 03a1  ...d.....|.j....
-00001510: 0001 0074 00a0 0164 02a1 0101 0064 0053  ...t...d.....d.S
-00001520: 0029 034e 7a36 6162 6f75 7420 746f 2053  .).Nz6about to S
-00001530: 746f 7020 7265 636f 7264 696e 6720 696e  top recording in
-00001540: 6974 6961 7465 6420 7769 7468 696e 2056  itiated within V
-00001550: 6964 656f 5265 636f 7264 6572 7a2d 5374  ideoRecorderz-St
-00001560: 6f70 2072 6563 6f72 6469 6e67 2069 6e69  op recording ini
-00001570: 7469 6174 6564 2077 6974 6869 6e20 5669  tiated within Vi
-00001580: 6465 6f52 6563 6f72 6465 7229 0472 2000  deoRecorder).r .
-00001590: 0000 7221 0000 0072 1400 0000 da03 7365  ..r!...r......se
-000015a0: 7472 5c00 0000 7219 0000 0072 1900 0000  tr\...r....r....
-000015b0: 721a 0000 00da 0e73 746f 705f 7265 636f  r......stop_reco
-000015c0: 7264 696e 67d3 0000 0073 0600 0000 0a01  rding....s......
-000015d0: 0a01 0e01 7a1c 5669 6465 6f52 6563 6f72  ....z.VideoRecor
-000015e0: 6465 722e 7374 6f70 5f72 6563 6f72 6469  der.stop_recordi
-000015f0: 6e67 725b 0000 0029 0354 4654 2910 da08  ngr[...).TFT)...
-00001600: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00001610: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00001620: 5f5f 7206 0000 0072 1e00 0000 7211 0000  __r....r....r...
-00001630: 0072 2d00 0000 da04 626f 6f6c 7251 0000  .r-.....boolrQ..
-00001640: 0072 3000 0000 724a 0000 0072 5d00 0000  .r0...rJ...r]...
-00001650: 7202 0000 0072 6a00 0000 726c 0000 00da  r....rj...rl....
-00001660: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7219  .__classcell__r.
-00001670: 0000 0072 1900 0000 7217 0000 0072 1a00  ...r....r....r..
-00001680: 0000 720a 0000 0013 0000 0073 1c00 0000  ..r........s....
-00001690: 0800 1802 0812 1610 0867 0806 0806 0206  .........g......
-000016a0: 0201 0201 04fb 0202 0afe 1026 720a 0000  ...........&r...
-000016b0: 0029 19da 0d70 7978 7933 642e 6c6f 6767  .)...pyxy3d.logg
-000016c0: 6572 da06 7079 7879 3364 7220 0000 0072  er..pyxy3dr ...r
-000016d0: 3e00 0000 726d 0000 00da 0770 6174 686c  >...rm.....pathl
-000016e0: 6962 7202 0000 00da 0571 7565 7565 7203  ibr......queuer.
-000016f0: 0000 00da 0974 6872 6561 6469 6e67 7204  .....threadingr.
-00001700: 0000 0072 0500 0000 7222 0000 00da 0373  ...r....r".....s
-00001710: 7973 da06 7061 6e64 6173 7256 0000 0072  ys..pandasrV...r
-00001720: 6700 0000 da1b 7079 7879 3364 2e63 616d  g.....pyxy3d.cam
-00001730: 6572 6173 2e73 796e 6368 726f 6e69 7a65  eras.synchronize
-00001740: 7272 0600 0000 da1a 7079 7879 3364 2e63  rr......pyxy3d.c
-00001750: 616d 6572 6173 2e6c 6976 655f 7374 7265  ameras.live_stre
-00001760: 616d 7207 0000 00da 1070 7978 7933 642e  amr......pyxy3d.
-00001770: 696e 7465 7266 6163 6572 0800 0000 7209  interfacer....r.
-00001780: 0000 0072 0a00 0000 7219 0000 0072 1900  ...r....r....r..
-00001790: 0000 7219 0000 0072 1a00 0000 da08 3c6d  ..r....r......<m
-000017a0: 6f64 756c 653e 0100 0000 731a 0000 0008  odule>....s.....
-000017b0: 000c 020c 030c 0110 0108 0108 0108 0108  ................
-000017c0: 010c 020c 0110 0112 03                   .........
+00000990: 0100 0000 7a1d 4765 7474 696e 6720 7369  ....z.Getting si
+000009a0: 7a65 206f 6620 7379 6e63 2070 6163 6b65  ze of sync packe
+000009b0: 7420 71e9 1900 0000 7a31 5369 7a65 206f  t q.....z1Size o
+000009c0: 6620 756e 7361 7665 6420 6672 616d 6573  f unsaved frames
+000009d0: 206f 6e20 7468 6520 7265 636f 7264 696e   on the recordin
+000009e0: 6720 7175 6575 6520 6973 207a 3345 6e64  g queue is z3End
+000009f0: 206f 6620 7379 6e63 2070 6163 6b65 7473   of sync packets
+00000a00: 2073 6967 6e61 6c65 642e 2e2e 6272 6561   signaled...brea
+00000a10: 6b69 6e67 2072 6563 6f72 6420 6c6f 6f70  king record loop
+00000a20: 7a1b 5072 6f63 6573 7369 6f6e 6720 6672  z.Processiong fr
+00000a30: 616d 6520 7061 636b 6574 2e2e 2e7a 0d57  ame packet...z.W
+00000a40: 7269 7469 6e67 2066 7261 6d65 7213 0000  riting framer...
+00000a50: 0072 2800 0000 7231 0000 0072 3200 0000  .r(...r1...r2...
+00000a60: 7a25 4578 7465 6e64 696e 6720 7469 6479  z%Extending tidy
+00000a70: 2074 6162 6c65 206f 6620 706f 696e 7420   table of point 
+00000a80: 6869 7374 6f72 797a 2153 6176 6520 6672  historyz!Save fr
+00000a90: 616d 6520 776f 726b 6572 2077 696e 6469  ame worker windi
+00000aa0: 6e67 2064 6f77 6e2e 2e2e 547a 1a72 656c  ng down...Tz.rel
+00000ab0: 6561 7369 6e67 2076 6964 656f 2077 7269  easing video wri
+00000ac0: 7465 7273 2e2e 2e7a 2149 6e69 7469 6174  ters...z!Initiat
+00000ad0: 6520 7374 6f72 696e 6720 6f66 2066 7261  e storing of fra
+00000ae0: 6d65 2068 6973 746f 7279 7a21 496e 6974  me historyz!Init
+00000af0: 6961 7465 2073 746f 7269 6e67 206f 6620  iate storing of 
+00000b00: 706f 696e 7420 6869 7374 6f72 797a 2741  point historyz'A
+00000b10: 626f 7574 2074 6f20 656d 6974 2060 616c  bout to emit `al
+00000b20: 6c20 6672 616d 6573 2073 6176 6564 6020  l frames saved` 
+00000b30: 7369 676e 616c 2921 722d 0000 00da 0d66  signal)!r-.....f
+00000b40: 7261 6d65 5f68 6973 746f 7279 da12 706f  rame_history..po
+00000b50: 696e 745f 6461 7461 5f68 6973 746f 7279  int_data_history
+00000b60: 720b 0000 00da 1973 7562 7363 7269 6265  r......subscribe
+00000b70: 5f74 6f5f 7379 6e63 5f70 6163 6b65 7473  _to_sync_packets
+00000b80: 7215 0000 0072 2000 0000 7221 0000 00da  r....r ...r!....
+00000b90: 0571 7369 7a65 7214 0000 00da 0669 735f  .qsizer......is_
+00000ba0: 7365 74da 0367 6574 da05 6465 6275 6772  set..get..debugr
+00000bb0: 1300 0000 da0d 6672 616d 655f 7061 636b  ......frame_pack
+00000bc0: 6574 7372 1d00 0000 da11 6672 616d 655f  etsr......frame_
+00000bd0: 7769 7468 5f70 6f69 6e74 73da 0566 7261  with_points..fra
+00000be0: 6d65 7231 0000 0072 3200 0000 721b 0000  mer1...r2...r...
+00000bf0: 00da 0577 7269 7465 da06 6170 7065 6e64  ...write..append
+00000c00: da0d 746f 5f74 6964 795f 7461 626c 65da  ..to_tidy_table.
+00000c10: 0463 6f70 79da 0665 7874 656e 64da 1572  .copy..extend..r
+00000c20: 656c 6561 7365 5f73 796e 635f 7061 636b  elease_sync_pack
+00000c30: 6574 5f71 da05 706f 7274 73da 0772 656c  et_q..ports..rel
+00000c40: 6561 7365 da13 7374 6f72 655f 6672 616d  ease..store_fram
+00000c50: 655f 6869 7374 6f72 7972 3000 0000 da05  e_historyr0.....
+00000c60: 636c 6561 7272 1200 0000 290f 7216 0000  clearr....).r...
+00000c70: 0072 2e00 0000 722f 0000 0072 3000 0000  .r....r/...r0...
+00000c80: 5a21 7379 6e63 726f 6e69 7a65 725f 7375  Z!syncronizer_su
+00000c90: 6273 6372 6970 7469 6f6e 5f72 656c 6561  bscription_relea
+00000ca0: 7365 64da 0b73 796e 635f 7061 636b 6574  sed..sync_packet
+00000cb0: da07 6261 636b 6c6f 6772 2800 0000 da0c  ..backlogr(.....
+00000cc0: 6672 616d 655f 7061 636b 6574 7242 0000  frame_packetrB..
+00000cd0: 0072 3100 0000 7232 0000 005a 0e6e 6577  .r1...r2...Z.new
+00000ce0: 5f74 6964 795f 7461 626c 65da 036b 6579  _tidy_table..key
+00000cf0: da05 7661 6c75 6572 1900 0000 7219 0000  ..valuer....r...
+00000d00: 0072 1a00 0000 da10 7361 7665 5f64 6174  .r......save_dat
+00000d10: 615f 776f 726b 6572 3700 0000 7388 0000  a_worker7...s...
+00000d20: 0004 0208 0102 0402 0102 0102 0108 fc02  ................
+00000d30: 0802 0102 0102 0102 0102 0102 0102 0102  ................
+00000d40: 0108 f70e 0d04 010a 0318 010a 010a 030a  ................
+00000d50: 0114 0116 0108 020a 0202 0108 0212 0208  ................
+00000d60: 010a 0104 0208 0106 0206 0206 0104 020a  ................
+00000d70: 0210 0112 0310 0110 0110 010c 0208 0116  ................
+00000d80: 010a 0116 0102 800e 020a 0104 010e 0118  ................
+00000d90: d006 350a 010c 0112 010a 0408 010a 0206  ..5.............
+00000da0: 0108 010a 0106 010e 017a 1e56 6964 656f  .........z.Video
+00000db0: 5265 636f 7264 6572 2e73 6176 655f 6461  Recorder.save_da
+00000dc0: 7461 5f77 6f72 6b65 7263 0100 0000 0000  ta_workerc......
+00000dd0: 0000 0000 0000 0300 0000 0600 0000 4300  ..............C.
+00000de0: 0000 734a 0000 0074 00a0 017c 006a 02a1  ..sJ...t...|.j..
+00000df0: 017d 0174 0374 047c 006a 0564 017c 006a  .}.t.t.|.j.d.|.j
+00000e00: 069b 0064 029d 0383 0283 017d 0274 07a0  ...d.......}.t..
+00000e10: 0864 037c 029b 009d 02a1 0101 007c 016a  .d.|.........|.j
+00000e20: 097c 0264 0464 0564 068d 0301 0064 0053  .|.d.d.d.....d.S
+00000e30: 0029 074e da02 7879 7a04 2e63 7376 7a16  .).N..xyz..csvz.
+00000e40: 5374 6f72 696e 6720 706f 696e 7420 6461  Storing point da
+00000e50: 7461 2069 6e20 4654 a902 da05 696e 6465  ta in FT....inde
+00000e60: 78da 0668 6561 6465 7229 0ada 0270 64da  x..header)...pd.
+00000e70: 0944 6174 6146 7261 6d65 723a 0000 0072  .DataFramer:...r
+00000e80: 1e00 0000 7202 0000 0072 1f00 0000 720c  ....r....r....r.
+00000e90: 0000 0072 2000 0000 7221 0000 00da 0674  ...r ...r!.....t
+00000ea0: 6f5f 6373 7629 0372 1600 0000 da02 6466  o_csv).r......df
+00000eb0: da0f 706f 696e 745f 6461 7461 5f70 6174  ..point_data_pat
+00000ec0: 6872 1900 0000 7219 0000 0072 1a00 0000  hr....r....r....
+00000ed0: 7230 0000 009e 0000 0073 0800 0000 0c01  r0.......s......
+00000ee0: 1a01 1001 1401 7a21 5669 6465 6f52 6563  ......z!VideoRec
+00000ef0: 6f72 6465 722e 7374 6f72 655f 706f 696e  order.store_poin
+00000f00: 745f 6869 7374 6f72 7963 0100 0000 0000  t_historyc......
+00000f10: 0000 0000 0000 0300 0000 0500 0000 4300  ..............C.
+00000f20: 0000 7340 0000 0074 00a0 017c 006a 02a1  ..s@...t...|.j..
+00000f30: 017d 0174 0374 047c 006a 0564 0183 0283  .}.t.t.|.j.d....
+00000f40: 017d 0274 06a0 0764 027c 029b 009d 02a1  .}.t...d.|......
+00000f50: 0101 007c 016a 087c 0264 0364 0464 058d  ...|.j.|.d.d.d..
+00000f60: 0301 0064 0053 0029 064e 7a16 6672 616d  ...d.S.).Nz.fram
+00000f70: 655f 7469 6d65 5f68 6973 746f 7279 2e63  e_time_history.c
+00000f80: 7376 7a19 5374 6f72 696e 6720 6672 616d  svz.Storing fram
+00000f90: 6520 6869 7374 6f72 7920 746f 2046 5472  e history to FTr
+00000fa0: 5400 0000 2909 7257 0000 0072 5800 0000  T...).rW...rX...
+00000fb0: 7239 0000 0072 1e00 0000 7202 0000 0072  r9...r....r....r
+00000fc0: 1f00 0000 7220 0000 0072 2100 0000 7259  ....r ...r!...rY
+00000fd0: 0000 0029 0372 1600 0000 725a 0000 005a  ...).r....rZ...Z
+00000fe0: 0f66 7261 6d65 5f68 6973 745f 7061 7468  .frame_hist_path
+00000ff0: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
+00001000: 4b00 0000 a400 0000 7308 0000 000c 0110  K.......s.......
+00001010: 0110 0114 017a 2156 6964 656f 5265 636f  .....z!VideoReco
+00001020: 7264 6572 2e73 746f 7265 5f66 7261 6d65  rder.store_frame
+00001030: 5f68 6973 746f 7279 6301 0000 0000 0000  _historyc.......
+00001040: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00001050: 0073 0400 0000 6400 5300 a901 4e72 1900  .s....d.S...Nr..
+00001060: 0000 a901 7216 0000 0072 1900 0000 7219  ....r....r....r.
+00001070: 0000 0072 1a00 0000 da13 7374 6f72 655f  ...r......store_
+00001080: 6163 7469 7665 5f63 6f6e 6669 67aa 0000  active_config...
+00001090: 0073 0200 0000 0401 7a21 5669 6465 6f52  .s......z!VideoR
+000010a0: 6563 6f72 6465 722e 7374 6f72 655f 6163  ecorder.store_ac
+000010b0: 7469 7665 5f63 6f6e 6669 6754 4672 1f00  tive_configTFr..
+000010c0: 0000 6305 0000 0000 0000 0000 0000 0007  ..c.............
+000010d0: 0000 0005 0000 0043 0000 0073 9800 0000  .......C...s....
+000010e0: 7400 a001 6401 7c01 9b00 9d02 a101 0100  t...d.|.........
+000010f0: 7c01 7c00 5f02 7c00 6a02 6a03 6402 6402  |.|._.|.j.j.d.d.
+00001100: 6403 8d02 0100 7c00 6a02 6a04 6a05 6404  d.....|.j.j.j.d.
+00001110: 6b02 7223 7406 7c00 6a02 6a04 6a04 6405  k.r#t.|.j.j.j.d.
+00001120: 8302 7d05 6e07 7406 7c00 6a02 6a04 6405  ..}.n.t.|.j.j.d.
+00001130: 8302 7d05 7406 7c00 6a02 6405 8302 7d06  ..}.t.|.j.d...}.
+00001140: 7407 a008 7c05 7c06 a102 0100 6402 7c00  t...|.|.....d.|.
+00001150: 5f09 740a 7c00 6a0b 7c02 7c03 7c04 6703  _.t.|.j.|.|.|.g.
+00001160: 6402 6406 8d03 7c00 5f0c 7c00 6a0c a00d  d.d...|._.|.j...
+00001170: a100 0100 6407 5300 2908 61f5 0100 000a  ....d.S.).a.....
+00001180: 2020 2020 2020 2020 4f70 7469 6f6e 2065          Option e
+00001190: 7869 7374 7320 746f 206e 6f74 2073 746f  xists to not sto
+000011a0: 7265 2076 6964 656f 2069 6620 6f6e 6c79  re video if only
+000011b0: 2069 6e74 6572 6573 7465 6420 696e 2067   interested in g
+000011c0: 6574 7469 6e67 2070 6f69 6e74 7320 6672  etting points fr
+000011d0: 6f6d 206f 7269 6769 6e61 6c20 7669 6465  om original vide
+000011e0: 6f0a 2020 2020 2020 2020 0a20 2020 2020  o.        .     
+000011f0: 2020 2050 6172 656e 7420 6f66 2064 6573     Parent of des
+00001200: 7469 6e61 7469 6f6e 2066 6f6c 6465 7220  tination folder 
+00001210: 7769 6c6c 2062 6520 7468 6520 736f 7572  will be the sour
+00001220: 6365 206f 6620 7468 6520 636f 6e66 6967  ce of the config
+00001230: 2066 696c 6520 7468 6174 2077 696c 6c20   file that will 
+00001240: 6265 2073 746f 7265 6420 7769 7468 2074  be stored with t
+00001250: 6865 2076 6964 656f 0a20 2020 2020 2020  he video.       
+00001260: 2054 6869 7320 656e 6162 6c65 7320 7468   This enables th
+00001270: 6520 6e65 7374 6564 2070 726f 6365 7373  e nested process
+00001280: 696e 6720 6f66 2076 6964 656f 7320 2869  ing of videos (i
+00001290: 2e65 2e20 5265 636f 7264 696e 675f 3120  .e. Recording_1 
+000012a0: 7769 6c6c 2073 746f 7265 2074 6865 206d  will store the m
+000012b0: 6169 6e20 636f 6e66 6967 2e74 6f6d 6c2c  ain config.toml,
+000012c0: 0a20 2020 2020 2020 2074 6865 6e20 504f  .        then PO
+000012d0: 5345 2073 7562 666f 6c64 6572 2077 696c  SE subfolder wil
+000012e0: 6c20 7374 6f72 6520 636f 6e66 6967 2e74  l store config.t
+000012f0: 6f6d 6c20 6672 6f6d 2052 6563 6f72 6469  oml from Recordi
+00001300: 6e67 5f31 292e 2045 6163 6820 666f 6c64  ng_1). Each fold
+00001310: 6572 2073 686f 756c 6420 6c61 7267 656c  er should largel
+00001320: 7920 6265 636f 6d65 2073 656c 660a 2020  y become self.  
+00001330: 2020 2020 2020 636f 6e74 6169 6e65 6420        contained 
+00001340: 616e 6420 706f 7274 6162 6c65 2066 6f72  and portable for
+00001350: 2061 6e61 6c79 7369 7320 2f20 7265 636f   analysis / reco
+00001360: 6e73 7472 7563 7469 6f6e 2e0a 2020 2020  nstruction..    
+00001370: 2020 2020 7a1e 416c 6c20 7669 6465 6f20      z.All video 
+00001380: 6461 7461 2074 6f20 6265 2073 6176 6564  data to be saved
+00001390: 2074 6f20 5429 02da 0865 7869 7374 5f6f   to T)...exist_o
+000013a0: 6bda 0770 6172 656e 7473 da0b 6361 6c69  k..parents..cali
+000013b0: 6272 6174 696f 6e7a 0b63 6f6e 6669 672e  brationz.config.
+000013c0: 746f 6d6c 2903 da06 7461 7267 6574 da04  toml)...target..
+000013d0: 6172 6773 da06 6461 656d 6f6e 4e29 0e72  args..daemonN).r
+000013e0: 2000 0000 7221 0000 0072 1f00 0000 da05   ...r!...r......
+000013f0: 6d6b 6469 72da 0670 6172 656e 74da 0473  mkdir..parent..s
+00001400: 7465 6d72 0200 0000 da06 7368 7574 696c  temr......shutil
+00001410: da05 636f 7079 3272 1200 0000 7204 0000  ..copy2r....r...
+00001420: 0072 5200 0000 5a10 7265 636f 7264 696e  .rR...Z.recordin
+00001430: 675f 7468 7265 6164 da05 7374 6172 7429  g_thread..start)
+00001440: 0772 1600 0000 721f 0000 0072 2e00 0000  .r....r....r....
+00001450: 722f 0000 0072 3000 0000 5a12 736f 7572  r/...r0...Z.sour
+00001460: 6365 5f63 6f6e 6669 675f 7061 7468 5a15  ce_config_pathZ.
+00001470: 6475 706c 6963 6174 655f 636f 6e66 6967  duplicate_config
+00001480: 5f70 6174 6872 1900 0000 7219 0000 0072  _pathr....r....r
+00001490: 1a00 0000 da0f 7374 6172 745f 7265 636f  ......start_reco
+000014a0: 7264 696e 67ad 0000 0073 1a00 0000 100f  rding....s......
+000014b0: 0602 1002 0e04 1201 0e02 0c02 0c02 0602  ................
+000014c0: 0201 0e01 08ff 0e03 7a1d 5669 6465 6f52  ........z.VideoR
+000014d0: 6563 6f72 6465 722e 7374 6172 745f 7265  ecorder.start_re
+000014e0: 636f 7264 696e 6763 0100 0000 0000 0000  cordingc........
+000014f0: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
+00001500: 7322 0000 0074 00a0 0164 01a1 0101 007c  s"...t...d.....|
+00001510: 006a 02a0 03a1 0001 0074 00a0 0164 02a1  .j.......t...d..
+00001520: 0101 0064 0053 0029 034e 7a36 6162 6f75  ...d.S.).Nz6abou
+00001530: 7420 746f 2053 746f 7020 7265 636f 7264  t to Stop record
+00001540: 696e 6720 696e 6974 6961 7465 6420 7769  ing initiated wi
+00001550: 7468 696e 2056 6964 656f 5265 636f 7264  thin VideoRecord
+00001560: 6572 7a2d 5374 6f70 2072 6563 6f72 6469  erz-Stop recordi
+00001570: 6e67 2069 6e69 7469 6174 6564 2077 6974  ng initiated wit
+00001580: 6869 6e20 5669 6465 6f52 6563 6f72 6465  hin VideoRecorde
+00001590: 7229 0472 2000 0000 7221 0000 0072 1400  r).r ...r!...r..
+000015a0: 0000 da03 7365 7472 5d00 0000 7219 0000  ....setr]...r...
+000015b0: 0072 1900 0000 721a 0000 00da 0e73 746f  .r....r......sto
+000015c0: 705f 7265 636f 7264 696e 67d3 0000 0073  p_recording....s
+000015d0: 0600 0000 0a01 0a01 0e01 7a1c 5669 6465  ..........z.Vide
+000015e0: 6f52 6563 6f72 6465 722e 7374 6f70 5f72  oRecorder.stop_r
+000015f0: 6563 6f72 6469 6e67 725c 0000 0029 0354  ecordingr\...).T
+00001600: 4654 2910 da08 5f5f 6e61 6d65 5f5f da0a  FT)...__name__..
+00001610: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00001620: 616c 6e61 6d65 5f5f 7206 0000 0072 1e00  alname__r....r..
+00001630: 0000 7211 0000 0072 2d00 0000 da04 626f  ..r....r-.....bo
+00001640: 6f6c 7252 0000 0072 3000 0000 724b 0000  olrR...r0...rK..
+00001650: 0072 5e00 0000 7202 0000 0072 6b00 0000  .r^...r....rk...
+00001660: 726d 0000 00da 0d5f 5f63 6c61 7373 6365  rm.....__classce
+00001670: 6c6c 5f5f 7219 0000 0072 1900 0000 7217  ll__r....r....r.
+00001680: 0000 0072 1a00 0000 720a 0000 0013 0000  ...r....r.......
+00001690: 0073 1c00 0000 0800 1802 0812 1610 0867  .s.............g
+000016a0: 0806 0806 0206 0201 0201 04fb 0202 0afe  ................
+000016b0: 1026 720a 0000 0029 19da 0d70 7978 7933  .&r....)...pyxy3
+000016c0: 642e 6c6f 6767 6572 da06 7079 7879 3364  d.logger..pyxy3d
+000016d0: 7220 0000 0072 3e00 0000 726e 0000 00da  r ...r>...rn....
+000016e0: 0770 6174 686c 6962 7202 0000 00da 0571  .pathlibr......q
+000016f0: 7565 7565 7203 0000 00da 0974 6872 6561  ueuer......threa
+00001700: 6469 6e67 7204 0000 0072 0500 0000 7222  dingr....r....r"
+00001710: 0000 00da 0373 7973 da06 7061 6e64 6173  .....sys..pandas
+00001720: 7257 0000 0072 6800 0000 da1b 7079 7879  rW...rh.....pyxy
+00001730: 3364 2e63 616d 6572 6173 2e73 796e 6368  3d.cameras.synch
+00001740: 726f 6e69 7a65 7272 0600 0000 da1a 7079  ronizerr......py
+00001750: 7879 3364 2e63 616d 6572 6173 2e6c 6976  xy3d.cameras.liv
+00001760: 655f 7374 7265 616d 7207 0000 00da 1070  e_streamr......p
+00001770: 7978 7933 642e 696e 7465 7266 6163 6572  yxy3d.interfacer
+00001780: 0800 0000 7209 0000 0072 0a00 0000 7219  ....r....r....r.
+00001790: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+000017a0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000017b0: 731a 0000 0008 000c 020c 030c 0110 0108  s...............
+000017c0: 0108 0108 0108 010c 020c 0110 0112 03    ...............
```

### Comparing `pyxy3d-0.1.4/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/recording/recorded_stream.py` & `pyxy3d-0.1.5/pyxy3d/recording/recorded_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/recording/video_recorder.py` & `pyxy3d-0.1.5/pyxy3d/recording/video_recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         
         # this is where the issue is... need to figure out when the queue is empty...
         logger.info("Entering Save data worker loop entered")
         while self.sync_packet_in_q.qsize() > 0 or not self.trigger_stop.is_set(): 
             sync_packet: SyncPacket = self.sync_packet_in_q.get()
 
             # provide periodic updates of recording queue
-            logger.info("Getting sidze of sync packet q")
+            logger.debug("Getting size of sync packet q")
             backlog = self.sync_packet_in_q.qsize()
             if backlog % 25 == 0 and backlog !=0:
                 logger.info(f"Size of unsaved frames on the recording queue is {self.sync_packet_in_q.qsize()}")
 
             if sync_packet is None:
                 # relenvant when 
                 logger.info("End of sync packets signaled...breaking record loop")
```

### Comparing `pyxy3d-0.1.4/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/session/__pycache__/session.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/session/__pycache__/session.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jun 23 17:47:59 2023 UTC, .py size: 21689 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 cfda 9564 b954 0000  o..........d.T..
+00000000: 6f0d 0d0a 0000 0000 6b24 9764 b954 0000  o.......k$.d.T..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e01 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6502  d.l.Z.d.d.l.Z.e.
 00000040: 6a03 a004 6505 a101 5a03 6400 6402 6c06  j...e...Z.d.d.l.
 00000050: 6d07 5a07 6d08 5a08 0100 6400 6403 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6405 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
@@ -307,734 +307,734 @@
 00001320: 0072 5600 0000 7257 0000 0072 5200 0000  .rV...rW...rR...
 00001330: 723b 0000 0072 4800 0000 da06 6967 6e6f  r;...rH.....igno
 00001340: 7265 725c 0000 0072 5d00 0000 725e 0000  rer\...r]...r^..
 00001350: 0072 5f00 0000 2904 722d 0000 0072 5300  .r_...).r-...rS.
 00001360: 0000 724d 0000 00da 0663 616d 6572 6172  ..rM.....camerar
 00001370: 2500 0000 7225 0000 0072 2600 0000 da15  %...r%...r&.....
 00001380: 6973 5f72 6563 6f72 6469 6e67 5f65 6c69  is_recording_eli
-00001390: 6769 626c 65a1 0000 0073 2400 0000 0a07  gible....s$.....
-000013a0: 0c01 0403 1001 0401 1402 0a01 1401 0402  ................
-000013b0: 0401 0a01 04ff 0280 0403 0401 0404 04fe  ................
-000013c0: 0402 7a1d 5365 7373 696f 6e2e 6973 5f72  ..z.Session.is_r
-000013d0: 6563 6f72 6469 6e67 5f65 6c69 6769 626c  ecording_eligibl
-000013e0: 6563 0100 0000 0000 0000 0000 0000 0500  ec..............
-000013f0: 0000 0500 0000 4300 0000 7346 0000 0064  ......C...sF...d
-00001400: 017d 017c 006a 00a0 01a1 0044 005d 197d  .}.|.j.....D.].}
-00001410: 027c 02a0 02a1 0072 2074 037c 02a0 0464  .|.....r t.|...d
-00001420: 02a1 0183 017d 037c 0264 031b 007d 047c  .....}.|.d...}.|
-00001430: 0372 207c 04a0 05a1 0072 2064 047d 0171  .r |.....r d.}.q
-00001440: 077c 0153 0029 057a a60a 2020 2020 2020  .|.S.).z..      
-00001450: 2020 506f 7374 2070 726f 6365 7373 696e    Post processin
-00001460: 6720 6361 6e20 6f6e 6c79 2062 6520 7065  g can only be pe
-00001470: 7266 6f72 6d65 6420 6966 2072 6563 6f72  rformed if recor
-00001480: 6469 6e67 7320 286d 7034 2066 696c 6573  dings (mp4 files
-00001490: 2920 6578 6973 7420 616e 6420 6578 7472  ) exist and extr
-000014a0: 696e 7369 6373 200a 2020 2020 2020 2020  insics .        
-000014b0: 2863 6f6e 6669 672e 746f 6d6c 2920 6172  (config.toml) ar
-000014c0: 6520 6361 6c69 6272 6174 6564 2069 6e20  e calibrated in 
-000014d0: 7468 6520 2772 6563 6f72 6427 2064 6972  the 'record' dir
-000014e0: 6563 746f 7279 0a20 2020 2020 2020 2046  ectory.        F
-000014f0: 7a05 2a2e 6d70 347a 0b63 6f6e 6669 672e  z.*.mp4z.config.
-00001500: 746f 6d6c 5429 0672 3900 0000 da07 6974  tomlT).r9.....it
-00001510: 6572 6469 72da 0669 735f 6469 72da 046c  erdir..is_dir..l
-00001520: 6973 74da 0467 6c6f 62da 0665 7869 7374  ist..glob..exist
-00001530: 7329 0572 2d00 0000 7253 0000 00da 0563  s).r-...rS.....c
-00001540: 6869 6c64 5a09 6d70 345f 6669 6c65 735a  hildZ.mp4_filesZ
-00001550: 0b63 6f6e 6669 675f 6669 6c65 7225 0000  .config_filer%..
-00001560: 0072 2500 0000 7226 0000 00da 1b69 735f  .r%...r&.....is_
-00001570: 706f 7374 5f70 726f 6365 7373 696e 675f  post_processing_
-00001580: 656c 6967 6962 6c65 bf00 0000 7312 0000  eligible....s...
-00001590: 0004 060e 0108 010e 0108 010c 0104 0102  ................
-000015a0: 8004 027a 2353 6573 7369 6f6e 2e69 735f  ...z#Session.is_
-000015b0: 706f 7374 5f70 726f 6365 7373 696e 675f  post_processing_
-000015c0: 656c 6967 6962 6c65 7247 0000 0063 0200  eligiblerG...c..
-000015d0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000015e0: 0000 4300 0000 73bc 0100 007c 017c 005f  ..C...s....|.|._
-000015f0: 007c 00a0 01a1 0001 007c 006a 0004 0074  .|.......|.j...t
-00001600: 026a 036b 0272 1f01 007c 006a 0472 1d7c  .j.k.r...|.j.r.|
-00001610: 006a 05a0 06a1 0001 007c 00a0 07a1 0001  .j.......|......
-00001620: 0064 0953 0064 0953 0004 0074 026a 086b  .d.S.d.S...t.j.k
-00001630: 0272 3501 007c 006a 0472 337c 006a 05a0  .r5..|.j.r3|.j..
-00001640: 06a1 0001 007c 00a0 07a1 0001 0064 0953  .....|.......d.S
-00001650: 0064 0953 0004 0074 026a 096b 0272 6201  .d.S...t.j.k.rb.
-00001660: 0074 0a7c 006a 0b83 017c 005f 0c7c 006a  .t.|.j...|._.|.j
-00001670: 0473 487c 00a0 0da1 0001 007c 006a 05a0  .sH|.......|.j..
-00001680: 06a1 0001 007c 00a0 07a1 0001 007c 00a0  .....|.......|..
-00001690: 0ea1 0001 007c 00a0 0f64 01a1 0101 007c  .....|...d.....|
-000016a0: 00a0 107c 006a 11a1 0101 0064 0953 0004  ...|.j.....d.S..
-000016b0: 0074 026a 126b 0272 8901 0074 0a7c 006a  .t.j.k.r...t.|.j
-000016c0: 0b83 017c 005f 0c7c 006a 0473 757c 00a0  ...|._.|.j.su|..
-000016d0: 0da1 0001 007c 00a0 07a1 0001 007c 00a0  .....|.......|..
-000016e0: 0ea1 0001 007c 00a0 0f64 01a1 0101 007c  .....|...d.....|
-000016f0: 006a 05a0 13a1 0001 0064 0953 0004 0074  .j.......d.S...t
-00001700: 026a 146b 0272 9f01 007c 006a 0472 9d7c  .j.k.r...|.j.r.|
-00001710: 00a0 07a1 0001 007c 006a 05a0 06a1 0001  .......|.j......
-00001720: 0064 0953 0064 0953 0074 026a 156b 0272  .d.S.d.S.t.j.k.r
-00001730: dc74 16a0 1764 02a1 0101 007c 006a 0473  .t...d.....|.j.s
-00001740: b474 16a0 1764 03a1 0101 007c 00a0 0da1  .t...d.....|....
-00001750: 0001 0074 16a0 1764 04a1 0101 007c 00a0  ...t...d.....|..
-00001760: 07a1 0001 0074 16a0 1764 05a1 0101 007c  .....t...d.....|
-00001770: 00a0 0f64 06a1 0101 0074 16a0 1764 07a1  ...d.....t...d..
-00001780: 0101 007c 00a0 01a1 0001 0074 16a0 1764  ...|.......t...d
-00001790: 08a1 0101 007c 006a 05a0 13a1 0001 0064  .....|.j.......d
-000017a0: 0953 0064 0953 0029 0a7a af0a 2020 2020  .S.d.S.).z..    
-000017b0: 2020 2020 5669 6120 7468 6973 206d 6574      Via this met
-000017c0: 686f 642c 2074 6865 2066 7261 6d65 2072  hod, the frame r
-000017d0: 6561 6469 6e67 2062 6568 6176 696f 7220  eading behavior 
-000017e0: 7769 6c6c 2062 6520 6368 616e 6765 6420  will be changed 
-000017f0: 6279 2074 6865 2047 5549 2e20 4966 2073  by the GUI. If s
-00001800: 6f6d 6520 7072 6f70 6572 7469 6573 2061  ome properties a
-00001810: 7265 0a20 2020 2020 2020 206e 6f74 2061  re.        not a
-00001820: 7661 696c 6162 6c65 2028 692e 652e 2073  vailable (i.e. s
-00001830: 796e 6368 726f 6e69 7a65 7229 2074 6865  ynchronizer) the
-00001840: 7920 7769 6c6c 2062 6520 6372 6561 7465  y will be create
-00001850: 640a 2020 2020 2020 2020 547a 2041 7474  d.        Tz Att
-00001860: 656d 7074 696e 6720 746f 2073 6574 2072  empting to set r
-00001870: 6563 6f72 6469 6e67 206d 6f64 657a 2e53  ecording modez.S
-00001880: 7472 6561 6d20 746f 6f6c 7320 6e6f 7420  tream tools not 
-00001890: 6c6f 6164 6564 2c20 736f 206c 6f61 6469  loaded, so loadi
-000018a0: 6e67 2074 6865 6d20 7570 2e2e 2e7a 2850  ng them up...z(P
-000018b0: 6175 7369 6e67 206d 6f6e 6f63 616c 7320  ausing monocals 
-000018c0: 746f 2065 6e74 6572 2072 6563 6f72 6469  to enter recordi
-000018d0: 6e67 206d 6f64 657a 2053 746f 7020 7472  ng modez Stop tr
-000018e0: 6163 6b69 6e67 2066 6f72 2072 6563 6f72  acking for recor
-000018f0: 6469 6e67 206d 6f64 6546 7a22 5570 6461  ding modeFz"Upda
-00001900: 7465 2073 7472 6561 6d20 6670 7320 746f  te stream fps to
-00001910: 2072 6563 6f72 6469 6e67 2066 7073 7a3e   recording fpsz>
-00001920: 5375 6273 6372 6962 6520 7379 6e63 6872  Subscribe synchr
-00001930: 6f6e 697a 6572 2074 6f20 7374 7265 616d  onizer to stream
-00001940: 7320 736f 2076 6964 656f 2072 6563 6f72  s so video recor
-00001950: 6465 7220 6361 6e20 6d61 6e61 6765 4e29  der can manageN)
-00001960: 1872 4700 0000 da12 7570 6461 7465 5f73  .rG.....update_s
-00001970: 7472 6561 6d73 5f66 7073 7219 0000 0072  treams_fpsr....r
-00001980: 1f00 0000 723e 0000 0072 4b00 0000 da18  ....r>...rK.....
-00001990: 756e 7375 6273 6372 6962 655f 6672 6f6d  unsubscribe_from
-000019a0: 5f73 7472 6561 6d73 da19 7061 7573 655f  _streams..pause_
-000019b0: 616c 6c5f 6d6f 6e6f 6361 6c69 6272 6174  all_monocalibrat
-000019c0: 6f72 7372 2400 0000 7220 0000 0072 0900  orsr$...r ...r..
-000019d0: 0000 7245 0000 0072 4600 0000 da11 6c6f  ..rE...rF.....lo
-000019e0: 6164 5f73 7472 6561 6d5f 746f 6f6c 73da  ad_stream_tools.
-000019f0: 1373 6574 5f73 7472 6561 6d73 5f63 6861  .set_streams_cha
-00001a00: 7275 636f da14 7365 745f 7374 7265 616d  ruco..set_stream
-00001a10: 735f 7472 6163 6b69 6e67 da17 6163 7469  s_tracking..acti
-00001a20: 7661 7465 5f6d 6f6e 6f63 616c 6962 7261  vate_monocalibra
-00001a30: 746f 7272 4000 0000 7221 0000 00da 1473  torr@...r!.....s
-00001a40: 7562 7363 7269 6265 5f74 6f5f 7374 7265  ubscribe_to_stre
-00001a50: 616d 7372 2200 0000 7223 0000 0072 5e00  amsr"...r#...r^.
-00001a60: 0000 725f 0000 0029 0272 2d00 0000 7247  ..r_...).r-...rG
-00001a70: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00001a80: 0000 da08 7365 745f 6d6f 6465 cf00 0000  ....set_mode....
-00001a90: 7362 0000 0006 0508 0104 020c 0106 010a  sb..............
-00001aa0: 010c 0104 fe0c 0406 010a 010c 0104 fe0c  ................
-00001ab0: 040c 0206 0208 010a 0108 0108 010a 0110  ................
-00001ac0: 010c 020c 0206 0108 0108 0208 010a 010e  ................
-00001ad0: 020c 0206 0108 010e 0104 fe08 040a 0106  ................
-00001ae0: 010a 0108 010a 0208 010a 020a 010a 0108  ................
-00001af0: 010a 020e 0104 f17a 1053 6573 7369 6f6e  .......z.Session
-00001b00: 2e73 6574 5f6d 6f64 65da 0a66 7073 5f74  .set_mode..fps_t
-00001b10: 6172 6765 7463 0200 0000 0000 0000 0000  argetc..........
-00001b20: 0000 0200 0000 0300 0000 4300 0000 7386  ..........C...s.
-00001b30: 0000 007c 006a 0004 0074 016a 026b 0272  ...|.j...t.j.k.r
-00001b40: 0901 006e 3404 0074 016a 036b 0272 1001  ...n4..t.j.k.r..
-00001b50: 006e 2d04 0074 016a 046b 0272 2001 007c  .n-..t.j.k.r ..|
-00001b60: 017c 005f 057c 006a 06a0 077c 01a1 0101  .|._.|.j...|....
-00001b70: 006e 1d04 0074 016a 086b 0272 3001 007c  .n...t.j.k.r0..|
-00001b80: 017c 005f 097c 006a 06a0 0a7c 01a1 0101  .|._.|.j...|....
-00001b90: 006e 0d74 016a 0b6b 0272 3d7c 017c 005f  .n.t.j.k.r=|.|._
-00001ba0: 0c7c 006a 06a0 0d7c 01a1 0101 007c 00a0  .|.j...|.....|..
-00001bb0: 0ea1 0001 0064 0153 0029 027a 780a 2020  .....d.S.).zx.  
-00001bc0: 2020 2020 2020 5570 6461 7465 7320 7468        Updates th
-00001bd0: 6520 4650 5320 7573 6564 2062 7920 7468  e FPS used by th
-00001be0: 6520 6375 7272 656e 746c 7920 6163 7469  e currently acti
-00001bf0: 7665 2073 6573 7369 6f6e 206d 6f64 650a  ve session mode.
-00001c00: 2020 2020 2020 2020 5468 6973 2075 7064          This upd
-00001c10: 6174 6520 696e 636c 7564 6573 2074 6865  ate includes the
-00001c20: 2063 6f6e 6669 672e 746f 6d6c 0a20 2020   config.toml.   
-00001c30: 2020 2020 204e 290f 7247 0000 0072 1900       N).rG...r..
-00001c40: 0000 721f 0000 0072 2400 0000 7220 0000  ..r....r$...r ..
-00001c50: 0072 4300 0000 7236 0000 005a 1e73 6176  .rC...r6...Z.sav
-00001c60: 655f 6670 735f 696e 7472 696e 7369 635f  e_fps_intrinsic_
-00001c70: 6361 6c69 6272 6174 696f 6e72 2100 0000  calibrationr!...
-00001c80: 7242 0000 005a 1e73 6176 655f 6670 735f  rB...Z.save_fps_
-00001c90: 6578 7472 696e 7369 635f 6361 6c69 6272  extrinsic_calibr
-00001ca0: 6174 696f 6e72 2300 0000 7241 0000 005a  ationr#...rA...Z
-00001cb0: 1273 6176 655f 6670 735f 7265 636f 7264  .save_fps_record
-00001cc0: 696e 6772 6c00 0000 2902 722d 0000 0072  ingrl...).r-...r
-00001cd0: 7500 0000 7225 0000 0072 2500 0000 7226  u...r%...r%...r&
-00001ce0: 0000 00da 1373 6574 5f61 6374 6976 655f  .....set_active_
-00001cf0: 6d6f 6465 5f66 7073 1001 0000 731e 0000  mode_fps....s...
-00001d00: 0004 050c 0102 010c 0102 010c 0106 010e  ................
-00001d10: 010c 0106 010e 0108 0106 010c 010c 027a  ...............z
-00001d20: 1b53 6573 7369 6f6e 2e73 6574 5f61 6374  .Session.set_act
-00001d30: 6976 655f 6d6f 6465 5f66 7073 7228 0000  ive_mode_fpsr(..
-00001d40: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00001d50: 0000 0300 0000 4300 0000 736e 0000 0064  ......C...sn...d
-00001d60: 007d 017c 006a 0004 0074 016a 026b 0272  .}.|.j...t.j.k.r
-00001d70: 0d01 0009 007c 0153 0004 0074 016a 036b  .....|.S...t.j.k
-00001d80: 0272 1601 0009 007c 0153 0004 0074 016a  .r.....|.S...t.j
-00001d90: 046b 0272 2101 007c 006a 057d 017c 0153  .k.r!..|.j.}.|.S
-00001da0: 0004 0074 016a 066b 0272 2c01 007c 006a  ...t.j.k.r,..|.j
-00001db0: 077d 017c 0153 0074 016a 086b 0272 357c  .}.|.S.t.j.k.r5|
-00001dc0: 006a 097d 017c 0153 007c 0153 0072 2900  .j.}.|.S.|.S.r).
-00001dd0: 0000 290a 7247 0000 0072 1900 0000 721f  ..).rG...r....r.
-00001de0: 0000 0072 2400 0000 7220 0000 0072 4300  ...r$...r ...rC.
-00001df0: 0000 7221 0000 0072 4200 0000 7223 0000  ..r!...rB...r#..
-00001e00: 0072 4100 0000 2902 722d 0000 005a 0366  .rA...).r-...Z.f
-00001e10: 7073 7225 0000 0072 2500 0000 7226 0000  psr%...r%...r&..
-00001e20: 00da 1367 6574 5f61 6374 6976 655f 6d6f  ...get_active_mo
-00001e30: 6465 5f66 7073 2601 0000 7322 0000 0004  de_fps&...s"....
-00001e40: 0104 010c 0102 0104 090c f802 0104 070c  ................
-00001e50: fa06 0104 050c fc06 0104 0308 fe06 0108  ................
-00001e60: 017a 1b53 6573 7369 6f6e 2e67 6574 5f61  .z.Session.get_a
-00001e70: 6374 6976 655f 6d6f 6465 5f66 7073 6301  ctive_mode_fpsc.
-00001e80: 0000 0000 0000 0000 0000 0004 0000 0004  ................
-00001e90: 0000 0043 0000 0073 3600 0000 7c00 a000  ...C...s6...|...
-00001ea0: a100 7d01 7c01 6400 7501 7217 7c00 6a01  ..}.|.d.u.r.|.j.
-00001eb0: a002 a100 4400 5d0b 5c02 7d02 7d03 7c03  ....D.].\.}.}.|.
-00001ec0: a003 7c01 a101 0100 710d 6400 5300 6400  ..|.....q.d.S.d.
-00001ed0: 5300 7229 0000 0029 0472 7700 0000 723c  S.r)...).rw...r<
-00001ee0: 0000 0072 4800 0000 5a0e 7365 745f 6670  ...rH...Z.set_fp
-00001ef0: 735f 7461 7267 6574 2904 722d 0000 005a  s_target).r-...Z
-00001f00: 0f61 6374 6976 655f 6d6f 6465 5f66 7073  .active_mode_fps
-00001f10: 724d 0000 0072 4e00 0000 7225 0000 0072  rM...rN...r%...r
-00001f20: 2500 0000 7226 0000 0072 6c00 0000 3501  %...r&...rl...5.
-00001f30: 0000 730c 0000 0008 0108 0112 010c 0104  ..s.............
-00001f40: fe04 017a 1a53 6573 7369 6f6e 2e75 7064  ...z.Session.upd
-00001f50: 6174 655f 7374 7265 616d 735f 6670 73da  ate_streams_fps.
-00001f60: 0b74 7261 636b 696e 675f 6f6e 6302 0000  .tracking_onc...
-00001f70: 0000 0000 0000 0000 0004 0000 0004 0000  ................
-00001f80: 0043 0000 0073 2200 0000 7c00 6a00 a001  .C...s"...|.j...
-00001f90: a100 4400 5d09 5c02 7d02 7d03 7c03 a002  ..D.].\.}.}.|...
-00001fa0: 7c01 a101 0100 7105 6400 5300 7229 0000  |.....q.d.S.r)..
-00001fb0: 0029 0372 3c00 0000 7248 0000 005a 0f73  .).r<...rH...Z.s
-00001fc0: 6574 5f74 7261 636b 696e 675f 6f6e 2904  et_tracking_on).
-00001fd0: 722d 0000 0072 7800 0000 724d 0000 0072  r-...rx...rM...r
-00001fe0: 4e00 0000 7225 0000 0072 2500 0000 7226  N...r%...r%...r&
-00001ff0: 0000 0072 7100 0000 3b01 0000 7306 0000  ...rq...;...s...
-00002000: 0012 010c 0104 ff7a 1c53 6573 7369 6f6e  .......z.Session
-00002010: 2e73 6574 5f73 7472 6561 6d73 5f74 7261  .set_streams_tra
-00002020: 636b 696e 6763 0100 0000 0000 0000 0000  ckingc..........
-00002030: 0000 0300 0000 0400 0000 4300 0000 733a  ..........C...s:
-00002040: 0000 0074 00a0 0164 01a1 0101 0074 027c  ...t...d.....t.|
-00002050: 006a 0383 017c 005f 047c 006a 05a0 06a1  .j...|._.|.j....
-00002060: 0044 005d 0a5c 027d 017d 027c 02a0 077c  .D.].\.}.}.|...|
-00002070: 006a 04a1 0101 0071 1064 0053 0029 024e  .j.....q.d.S.).N
-00002080: 7a22 7570 6461 7469 6e67 2063 6861 7275  z"updating charu
-00002090: 636f 2069 6e20 6361 7365 206e 6563 6573  co in case neces
-000020a0: 7361 7279 2908 725e 0000 0072 5f00 0000  sary).r^...r_...
-000020b0: 7209 0000 0072 4500 0000 7246 0000 0072  r....rE...rF...r
-000020c0: 3c00 0000 7248 0000 005a 0e75 7064 6174  <...rH...Z.updat
-000020d0: 655f 7472 6163 6b65 7229 0372 2d00 0000  e_tracker).r-...
-000020e0: 724d 0000 0072 4e00 0000 7225 0000 0072  rM...rN...r%...r
-000020f0: 2500 0000 7226 0000 0072 7000 0000 3f01  %...r&...rp...?.
-00002100: 0000 730a 0000 000a 010c 0112 010e 0104  ..s.............
-00002110: ff7a 1b53 6573 7369 6f6e 2e73 6574 5f73  .z.Session.set_s
-00002120: 7472 6561 6d73 5f63 6861 7275 636f 6301  treams_charucoc.
-00002130: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00002140: 0000 0043 0000 0073 1800 0000 7400 a001  ...C...s....t...
-00002150: 6401 a101 0100 7c00 6a02 a003 a100 0100  d.....|.j.......
-00002160: 6400 5300 2902 4e7a 1470 6175 7369 6e67  d.S.).Nz.pausing
-00002170: 2073 796e 6368 726f 6e69 7a65 7229 0472   synchronizer).r
-00002180: 5e00 0000 725f 0000 0072 4b00 0000 726d  ^...r_...rK...rm
-00002190: 0000 0072 2c00 0000 7225 0000 0072 2500  ...r,...r%...r%.
-000021a0: 0000 7226 0000 00da 1270 6175 7365 5f73  ..r&.....pause_s
-000021b0: 796e 6368 726f 6e69 7a65 7245 0100 0073  ynchronizerE...s
-000021c0: 0400 0000 0a01 0e01 7a1a 5365 7373 696f  ........z.Sessio
-000021d0: 6e2e 7061 7573 655f 7379 6e63 6872 6f6e  n.pause_synchron
-000021e0: 697a 6572 6301 0000 0000 0000 0000 0000  izerc...........
-000021f0: 0001 0000 0003 0000 0043 0000 0073 1e00  .........C...s..
-00002200: 0000 7c00 6a00 a001 a100 0100 7c00 6a00  ..|.j.......|.j.
-00002210: a002 7c00 6a00 6a03 a101 0100 6400 5300  ..|.j.j.....d.S.
-00002220: 7229 0000 0029 0472 4b00 0000 7273 0000  r)...).rK...rs..
-00002230: 005a 0e73 6574 5f73 7472 6561 6d5f 6670  .Z.set_stream_fp
-00002240: 7372 7500 0000 722c 0000 0072 2500 0000  sru...r,...r%...
-00002250: 7225 0000 0072 2600 0000 da14 756e 7061  r%...r&.....unpa
-00002260: 7573 655f 7379 6e63 6872 6f6e 697a 6572  use_synchronizer
-00002270: 4901 0000 7304 0000 000a 0114 017a 1c53  I...s........z.S
-00002280: 6573 7369 6f6e 2e75 6e70 6175 7365 5f73  ession.unpause_s
-00002290: 796e 6368 726f 6e69 7a65 7263 0100 0000  ynchronizerc....
-000022a0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
-000022b0: 4300 0000 7334 0000 0064 017d 017c 006a  C...s4...d.}.|.j
-000022c0: 006a 01a0 02a1 00a0 03a1 0044 005d 0d5c  .j.........D.].\
-000022d0: 027d 027d 037c 02a0 0464 02a1 0172 177c  .}.}.|...d...r.|
-000022e0: 0164 0337 007d 0171 0a7c 0153 0029 044e  .d.7.}.q.|.S.).N
-000022f0: 7201 0000 0072 4f00 0000 e901 0000 0029  r....rO........)
-00002300: 0572 3600 0000 da04 6469 6374 da04 636f  .r6.....dict..co
-00002310: 7079 7248 0000 00da 0a73 7461 7274 7377  pyrH.....startsw
-00002320: 6974 6829 0472 2d00 0000 da05 636f 756e  ith).r-.....coun
-00002330: 74da 036b 6579 da06 7061 7261 6d73 7225  t..key..paramsr%
-00002340: 0000 0072 2500 0000 7226 0000 00da 1b67  ...r%...r&.....g
-00002350: 6574 5f63 6f6e 6669 6775 7265 645f 6361  et_configured_ca
-00002360: 6d65 7261 5f63 6f75 6e74 4d01 0000 730c  mera_countM...s.
-00002370: 0000 0004 0118 010a 0108 0102 8004 017a  ...............z
-00002380: 2353 6573 7369 6f6e 2e67 6574 5f63 6f6e  #Session.get_con
-00002390: 6669 6775 7265 645f 6361 6d65 7261 5f63  figured_camera_c
-000023a0: 6f75 6e74 6301 0000 0000 0000 0000 0000  ountc...........
-000023b0: 0005 0000 0008 0000 0003 0000 0073 8c00  .............s..
-000023c0: 0000 8700 6601 6401 6402 8408 7d01 7400  ....f.d.d...}.t.
-000023d0: 8300 8f1e 7d02 7401 6403 7402 8302 4400  ....}.t.d.t...D.
-000023e0: 5d10 7d03 7c03 8800 6a03 a004 a100 7600  ].}.|...j.....v.
-000023f0: 7219 710f 7c02 a005 7c01 7c03 a102 0100  r.q.|...|.|.....
-00002400: 710f 5700 6404 0400 0400 8303 0100 6e08  q.W.d.........n.
-00002410: 3100 732a 7701 0100 0100 0100 5900 0100  1.s*w.......Y...
-00002420: 8800 6a06 6a07 a008 a100 a004 a100 4400  ..j.j.........D.
-00002430: 5d0c 7d04 7c04 a009 6405 a101 7243 8800  ].}.|...d...rC..
-00002440: 6a06 6a07 7c04 3d00 7137 6404 5300 2906  j.j.|.=.q7d.S.).
-00002450: 7aa3 0a20 2020 2020 2020 2043 616c 6c65  z..        Calle
-00002460: 6420 6279 206c 6f61 645f 7374 7265 616d  d by load_stream
-00002470: 7320 696e 2074 6865 2065 7665 6e74 2074  s in the event t
-00002480: 6861 7420 6e6f 2063 616d 6572 6173 2061  hat no cameras a
-00002490: 7265 2072 6574 7572 6e65 6420 6279 2074  re returned by t
-000024a0: 6865 2063 6f6e 6669 6775 7261 746f 722e  he configurator.
-000024b0: 2e2e 0a20 2020 2020 2020 2057 696c 6c20  ...        Will 
-000024c0: 706f 7075 6c61 7465 2073 656c 662e 6361  populate self.ca
-000024d0: 6d65 7261 7320 7573 696e 6720 6d75 6c74  meras using mult
-000024e0: 6970 6c65 2074 6872 6561 6473 0a20 2020  iple threads.   
-000024f0: 2020 2020 2063 0100 0000 0000 0000 0000       c..........
-00002500: 0000 0200 0000 0700 0000 1300 0000 738c  ..............s.
-00002510: 0000 007a 3774 00a0 0164 017c 009b 009d  ...z7t...d.|....
-00002520: 02a1 0101 0074 027c 0083 017d 0174 00a0  .....t.|...}.t..
-00002530: 0164 027c 009b 009d 02a1 0101 007c 0188  .d.|.........|..
-00002540: 006a 037c 003c 0088 006a 04a0 057c 01a1  .j.|.<...j...|..
-00002550: 0101 0074 00a0 0164 037c 009b 0064 049d  ...t...d.|...d..
-00002560: 03a1 0101 0074 067c 0174 0788 006a 0883  .....t.|.t...j..
-00002570: 0164 058d 0288 006a 097c 003c 0057 0064  .d.....j.|.<.W.d
-00002580: 0053 0001 0001 0001 0074 00a0 0164 067c  .S.......t...d.|
-00002590: 009b 009d 02a1 0101 0059 0064 0053 0029  .........Y.d.S.)
-000025a0: 074e 7a0c 5472 7969 6e67 2070 6f72 7420  .Nz.Trying port 
-000025b0: 7a10 5375 6363 6573 7320 6174 2070 6f72  z.Success at por
-000025c0: 7420 7a17 4c6f 6164 696e 6720 7374 7265  t z.Loading stre
-000025d0: 616d 2061 7420 706f 7274 207a 2520 7769  am at port z% wi
-000025e0: 7468 2063 6861 7275 636f 2074 7261 636b  th charuco track
-000025f0: 6572 2066 6f72 2063 616c 6962 7261 7469  er for calibrati
-00002600: 6f6e a901 5a07 7472 6163 6b65 727a 124e  on..Z.trackerz.N
-00002610: 6f20 6361 6d65 7261 2061 7420 706f 7274  o camera at port
-00002620: 2029 0a72 5e00 0000 725f 0000 0072 0b00   ).r^...r_...r..
-00002630: 0000 723b 0000 0072 3600 0000 5a0b 7361  ..r;...r6...Z.sa
-00002640: 7665 5f63 616d 6572 6172 1600 0000 7209  ve_camerar....r.
-00002650: 0000 0072 4500 0000 723c 0000 0029 0272  ...rE...r<...).r
-00002660: 4d00 0000 724f 0000 0072 2c00 0000 7225  M...rO...r,...r%
-00002670: 0000 0072 2600 0000 da07 6164 645f 6361  ...r&.....add_ca
-00002680: 6d5a 0100 0073 1c00 0000 0201 1001 0801  mZ...s..........
-00002690: 1001 0a01 0c01 0401 0a01 04ff 0203 0a01  ................
-000026a0: 12ff 0603 1601 7a26 5365 7373 696f 6e2e  ......z&Session.
-000026b0: 5f66 696e 645f 6361 6d65 7261 732e 3c6c  _find_cameras.<l
-000026c0: 6f63 616c 733e 2e61 6464 5f63 616d 7201  ocals>.add_camr.
-000026d0: 0000 004e da06 7374 6572 656f 290a 7204  ...N..stereo).r.
-000026e0: 0000 00da 0572 616e 6765 da15 4d41 585f  .....range..MAX_
-000026f0: 4341 4d45 5241 5f50 4f52 545f 4348 4543  CAMERA_PORT_CHEC
-00002700: 4b72 3b00 0000 da04 6b65 7973 da06 7375  Kr;.....keys..su
-00002710: 626d 6974 7236 0000 0072 7c00 0000 727d  bmitr6...r|...r}
-00002720: 0000 0072 7e00 0000 2905 722d 0000 0072  ...r~...).r-...r
-00002730: 8400 0000 da08 6578 6563 7574 6f72 da01  ......executor..
-00002740: 6972 8000 0000 7225 0000 0072 2c00 0000  ir....r%...r,...
-00002750: 7226 0000 00da 0d5f 6669 6e64 5f63 616d  r&....._find_cam
-00002760: 6572 6173 5401 0000 731a 0000 000c 0608  erasT...s.......
-00002770: 100e 010e 0102 020e 0202 fb1c ff14 090a  ................
-00002780: 010a 0102 8004 fe7a 1553 6573 7369 6f6e  .......z.Session
-00002790: 2e5f 6669 6e64 5f63 616d 6572 6173 6301  ._find_camerasc.
-000027a0: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-000027b0: 0000 0043 0000 0073 dc00 0000 6401 7c00  ...C...s....d.|.
-000027c0: 5f00 7c00 6a01 a002 a100 7c00 5f03 7404  _.|.j.....|._.t.
-000027d0: 7c00 6a03 8301 6402 6b02 7214 7c00 a005  |.j...d.k.r.|...
-000027e0: a100 0100 7c00 6a03 a006 a100 4400 5d1e  ....|.j.....D.].
-000027f0: 5c02 7d01 7d02 7c01 7c00 6a07 a008 a100  \.}.}.|.|.j.....
-00002800: 7600 7225 7119 7409 a00a 6403 7c01 9b00  v.r%q.t...d.|...
-00002810: 9d02 a101 0100 740b 7c02 7c00 6a0c 6404  ......t.|.|.j.d.
-00002820: 8d02 7c00 6a07 7c01 3c00 7119 7c00 a00d  ..|.j.|.<.q.|...
-00002830: a100 0100 7c00 a00e a100 0100 740f 7c00  ....|.......t.|.
-00002840: 6a10 a008 a100 8301 7c00 5f11 7412 7c00  j.......|._.t.|.
-00002850: 6a07 8301 7c00 5f13 6401 7c00 5f14 6405  j...|._.d.|._.d.
-00002860: 7c00 5f00 7409 a00a 6406 a101 0100 7c00  |._.t...d.....|.
-00002870: a015 a100 0100 7c00 a016 a100 0100 7409  ......|.......t.
-00002880: a00a 6407 a101 0100 7c00 6a17 6a18 a019  ..d.....|.j.j...
-00002890: a100 0100 6408 5300 2909 7aad 0a20 2020  ....d.S.).z..   
-000028a0: 2020 2020 2043 6f6e 6e65 6374 7320 746f       Connects to
-000028b0: 2073 746f 7265 6420 6361 6d65 7261 7320   stored cameras 
-000028c0: 616e 6420 6372 6561 7465 7320 7374 7265  and creates stre
-000028d0: 616d 7320 7769 7468 2070 726f 7669 6465  ams with provide
-000028e0: 6420 7472 6163 6b69 6e67 0a20 2020 2020  d tracking.     
-000028f0: 2020 2042 6563 6175 7365 2074 6865 7365     Because these
-00002900: 2073 7472 6561 6d73 2061 7265 2061 7661   streams are ava
-00002910: 696c 6162 6c65 2c20 7468 6520 7379 6e63  ilable, the sync
-00002920: 6872 6f6e 697a 6572 2063 616e 2074 6865  hronizer can the
-00002930: 6e20 6265 2069 6e69 7469 616c 697a 6564  n be initialized
-00002940: 0a20 2020 2020 2020 2054 7201 0000 007a  .        Tr....z
-00002950: 184c 6f61 6469 6e67 2053 7472 6561 6d20  .Loading Stream 
-00002960: 666f 7220 706f 7274 2072 8300 0000 467a  for port r....Fz
-00002970: 3350 6175 7369 6e67 2073 7472 6561 6d20  3Pausing stream 
-00002980: 746f 6f6c 7320 7369 6e63 6520 6465 6661  tools since defa
-00002990: 756c 7420 6c6f 6164 7320 746f 2063 6861  ult loads to cha
-000029a0: 7275 636f 7a2d 5369 676e 616c 6c69 6e67  rucoz-Signalling
-000029b0: 2073 7563 6365 7373 6675 6c20 6c6f 6164   successful load
-000029c0: 696e 6720 6f66 2073 7472 6561 6d20 746f  ing of stream to
-000029d0: 6f6c 734e 291a 723d 0000 0072 3600 0000  olsN).r=...r6...
-000029e0: 5a0b 6765 745f 6361 6d65 7261 7372 3b00  Z.get_camerasr;.
-000029f0: 0000 7252 0000 0072 8c00 0000 7248 0000  ..rR...r....rH..
-00002a00: 0072 3c00 0000 7288 0000 0072 5e00 0000  .r<...r....r^...
-00002a10: 725f 0000 0072 1600 0000 7246 0000 00da  r_...r....rF....
-00002a20: 135f 6164 6a75 7374 5f72 6573 6f6c 7574  ._adjust_resolut
-00002a30: 696f 6e73 da15 5f6c 6f61 645f 6d6f 6e6f  ions.._load_mono
-00002a40: 6361 6c69 6272 6174 6f72 73da 036d 696e  calibrators..min
-00002a50: 723f 0000 0072 4000 0000 720c 0000 0072  r?...r@...r....r
-00002a60: 4b00 0000 723e 0000 0072 6e00 0000 7279  K...r>...rn...ry
-00002a70: 0000 0072 3700 0000 7230 0000 0072 4c00  ...r7...r0...rL.
-00002a80: 0000 a903 722d 0000 0072 4d00 0000 724f  ....r-...rM...rO
-00002a90: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00002aa0: 0000 726f 0000 0077 0100 0073 2c00 0000  ..ro...w...s,...
-00002ab0: 0605 0c02 0e02 0801 1202 0e01 0201 1002  ................
-00002ac0: 1601 0802 0801 1003 0202 0401 06ff 0605  ................
-00002ad0: 0601 0a02 0801 0801 0a02 1001 7a19 5365  ............z.Se
-00002ae0: 7373 696f 6e2e 6c6f 6164 5f73 7472 6561  ssion.load_strea
-00002af0: 6d5f 746f 6f6c 7363 0100 0000 0000 0000  m_toolsc........
-00002b00: 0000 0000 0300 0000 0600 0000 4300 0000  ............C...
-00002b10: 735e 0000 007c 006a 00a0 01a1 0044 005d  s^...|.j.....D.]
-00002b20: 275c 027d 017d 027c 017c 006a 02a0 03a1  '\.}.}.|.|.j....
-00002b30: 0076 0072 1a74 04a0 0564 017c 019b 0064  .v.r.t...d.|...d
-00002b40: 029d 03a1 0101 0071 0574 04a0 0564 037c  .......q.t...d.|
-00002b50: 019b 009d 02a1 0101 0074 067c 006a 077c  .........t.|.j.|
-00002b60: 0119 0083 017c 006a 027c 013c 0071 0564  .....|.j.|.<.q.d
-00002b70: 0053 0029 044e 7a2f 536b 6970 7069 6e67  .S.).Nz/Skipping
-00002b80: 206f 7665 7220 6d6f 6e6f 6361 6c69 6272   over monocalibr
-00002b90: 6174 6f72 2063 7265 6174 696f 6e20 666f  ator creation fo
-00002ba0: 7220 706f 7274 207a 1b20 6265 6361 7573  r port z. becaus
-00002bb0: 6520 6974 2061 6c72 6561 6479 2065 7869  e it already exi
-00002bc0: 7374 732e 7a20 4c6f 6164 696e 6720 4d6f  sts.z Loading Mo
-00002bd0: 6e6f 6361 6c69 6272 6174 6f72 2066 6f72  nocalibrator for
-00002be0: 2070 6f72 7420 2908 723b 0000 0072 4800   port ).r;...rH.
-00002bf0: 0000 723f 0000 0072 8800 0000 725e 0000  ..r?...r....r^..
-00002c00: 0072 5f00 0000 720a 0000 0072 3c00 0000  .r_...r....r<...
-00002c10: 7290 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
-00002c20: 2600 0000 728e 0000 009f 0100 0073 1200  &...r........s..
-00002c30: 0000 1201 0e01 0401 0a01 04ff 0203 1002  ................
-00002c40: 1601 04f8 7a1d 5365 7373 696f 6e2e 5f6c  ....z.Session._l
-00002c50: 6f61 645f 6d6f 6e6f 6361 6c69 6272 6174  oad_monocalibrat
-00002c60: 6f72 734e da0b 6163 7469 7665 5f70 6f72  orsN..active_por
-00002c70: 7463 0200 0000 0000 0000 0000 0000 0200  tc..............
-00002c80: 0000 0500 0000 4300 0000 7346 0000 007c  ......C...sF...|
-00002c90: 0164 0175 0172 0f74 00a0 0164 027c 019b  .d.u.r.t...d.|..
-00002ca0: 009d 02a1 0101 007c 017c 005f 0274 00a0  .......|.|._.t..
-00002cb0: 0164 037c 006a 029b 0064 049d 03a1 0101  .d.|.j...d......
-00002cc0: 007c 006a 037c 006a 0219 00a0 04a1 0001  .|.j.|.j........
-00002cd0: 0064 0153 0029 057a 7e0a 2020 2020 2020  .d.S.).z~.      
-00002ce0: 2020 5573 6564 2074 6f20 6d61 6b65 2073    Used to make s
-00002cf0: 7572 6520 7468 6174 206f 6e6c 7920 7468  ure that only th
-00002d00: 6520 6163 7469 7665 2063 616d 6572 6120  e active camera 
-00002d10: 7461 6220 6973 2072 6561 6469 6e67 2066  tab is reading f
-00002d20: 7261 6d65 7320 6475 7269 6e67 2074 6865  rames during the
-00002d30: 2069 6e74 7269 6e73 6963 2063 616c 6962   intrinsic calib
-00002d40: 7261 7469 6f6e 2070 726f 6365 7373 0a20  ration process. 
-00002d50: 2020 2020 2020 204e 7a29 5365 7474 696e         Nz)Settin
-00002d60: 6720 7365 7373 696f 6e20 6163 7469 7665  g session active
-00002d70: 206d 6f6e 6f63 616c 6962 7261 746f 7220   monocalibrator 
-00002d80: 746f 207a 1a41 6374 6976 6174 6520 7472  to z.Activate tr
-00002d90: 6163 6b69 6e67 206f 6e20 706f 7274 207a  acking on port z
-00002da0: 1620 616e 6420 6465 6163 7469 7661 7465  . and deactivate
-00002db0: 206f 7468 6572 7329 0572 5e00 0000 725f   others).r^...r_
-00002dc0: 0000 0072 4000 0000 723f 0000 005a 1373  ...r@...r?...Z.s
-00002dd0: 7562 7363 7269 6265 5f74 6f5f 7374 7265  ubscribe_to_stre
-00002de0: 616d 2902 722d 0000 0072 9100 0000 7225  am).r-...r....r%
-00002df0: 0000 0072 2500 0000 7226 0000 0072 7200  ...r%...r&...rr.
-00002e00: 0000 aa01 0000 730e 0000 0008 0510 0106  ......s.........
-00002e10: 0104 010c 0104 ff14 037a 1f53 6573 7369  .........z.Sessi
-00002e20: 6f6e 2e61 6374 6976 6174 655f 6d6f 6e6f  on.activate_mono
-00002e30: 6361 6c69 6272 6174 6f72 6301 0000 0000  calibratorc.....
-00002e40: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-00002e50: 0000 0073 2a00 0000 7400 a001 6401 a101  ...s*...t...d...
-00002e60: 0100 7c00 6a02 a003 a100 4400 5d08 5c02  ..|.j.....D.].\.
-00002e70: 7d01 7d02 7c02 a004 a100 0100 710a 6402  }.}.|.......q.d.
-00002e80: 5300 2903 7a8b 0a20 2020 2020 2020 2075  S.).z..        u
-00002e90: 7365 6420 7768 656e 206e 6f74 2061 6374  sed when not act
-00002ea0: 6976 656c 7920 6f6e 2074 6865 2063 616d  ively on the cam
-00002eb0: 6572 6120 6361 6c69 6272 6174 696f 6e20  era calibration 
-00002ec0: 7461 620a 2020 2020 2020 2020 6f72 2077  tab.        or w
-00002ed0: 6865 6e20 7369 6c65 6e63 696e 6720 616c  hen silencing al
-00002ee0: 6c20 696e 2070 7265 7061 7261 7469 6f6e  l in preparation
-00002ef0: 2066 6f72 2061 6374 6976 6174 696e 6720   for activating 
-00002f00: 6f6e 6c79 206f 6e65 0a20 2020 2020 2020  only one.       
-00002f10: 207a 2550 6175 7369 6e67 2061 6c6c 206d   z%Pausing all m
-00002f20: 6f6e 6f63 616c 6962 7261 746f 7220 6c6f  onocalibrator lo
-00002f30: 6f70 696e 672e 2e2e 4e29 0572 5e00 0000  oping...N).r^...
-00002f40: 725f 0000 0072 3f00 0000 7248 0000 005a  r_...r?...rH...Z
-00002f50: 1575 6e73 7562 7363 7269 6265 5f74 6f5f  .unsubscribe_to_
-00002f60: 7374 7265 616d 2903 722d 0000 0072 4d00  stream).r-...rM.
-00002f70: 0000 7250 0000 0072 2500 0000 7225 0000  ..rP...r%...r%..
-00002f80: 0072 2600 0000 726e 0000 00b7 0100 0073  .r&...rn.......s
-00002f90: 0800 0000 0a05 1201 0a01 04ff 7a21 5365  ............z!Se
-00002fa0: 7373 696f 6e2e 7061 7573 655f 616c 6c5f  ssion.pause_all_
-00002fb0: 6d6f 6e6f 6361 6c69 6272 6174 6f72 7346  monocalibratorsF
-00002fc0: da15 6465 7374 696e 6174 696f 6e5f 6469  ..destination_di
-00002fd0: 7265 6374 6f72 79da 1373 746f 7265 5f70  rectory..store_p
-00002fe0: 6f69 6e74 5f68 6973 746f 7279 6303 0000  oint_historyc...
-00002ff0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00003000: 0043 0000 0073 3e00 0000 7400 a001 6401  .C...s>...t...d.
-00003010: a101 0100 7c01 6a02 6402 6402 6403 8d02  ....|.j.d.d.d...
-00003020: 0100 7403 7c00 6a04 8301 7c00 5f05 7c00  ..t.|.j...|._.|.
-00003030: 6a05 6a06 7c01 7c02 6404 8d02 0100 6402  j.j.|.|.d.....d.
-00003040: 7c00 5f07 6400 5300 2905 4e7a 1749 6e69  |._.d.S.).Nz.Ini
-00003050: 7469 6174 696e 6720 7265 636f 7264 696e  tiating recordin
-00003060: 672e 2e2e 5429 02da 0770 6172 656e 7473  g...T)...parents
-00003070: da08 6578 6973 745f 6f6b 2901 7293 0000  ..exist_ok).r...
-00003080: 0029 0872 5e00 0000 725f 0000 00da 056d  .).r^...r_.....m
-00003090: 6b64 6972 7217 0000 0072 4b00 0000 da0e  kdirr....rK.....
-000030a0: 7669 6465 6f5f 7265 636f 7264 6572 da0f  video_recorder..
-000030b0: 7374 6172 745f 7265 636f 7264 696e 6772  start_recordingr
-000030c0: 4400 0000 2903 722d 0000 0072 9200 0000  D...).r-...r....
-000030d0: 7293 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
-000030e0: 2600 0000 7298 0000 00c0 0100 0073 0e00  &...r........s..
-000030f0: 0000 0a03 0e01 0c02 0601 0401 06ff 0a03  ................
-00003100: 7a17 5365 7373 696f 6e2e 7374 6172 745f  z.Session.start_
-00003110: 7265 636f 7264 696e 6763 0100 0000 0000  recordingc......
-00003120: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00003130: 0000 736e 0000 0074 00a0 0164 01a1 0101  ..sn...t...d....
-00003140: 007c 006a 02a0 03a1 0001 007c 006a 026a  .|.j.......|.j.j
-00003150: 0472 1b74 00a0 0164 02a1 0101 0074 0564  .r.t...d.....t.d
-00003160: 0383 0101 007c 006a 026a 0473 0e64 047c  .....|.j.j.s.d.|
-00003170: 005f 0674 00a0 0164 05a1 0101 007c 006a  ._.t...d.....|.j
-00003180: 076a 08a0 09a1 0001 007c 00a0 0aa1 0072  .j.......|.....r
-00003190: 357c 006a 076a 0ba0 09a1 0001 0064 0053  5|.j.j.......d.S
-000031a0: 0064 0053 0029 064e 7a15 5374 6f70 7069  .d.S.).Nz.Stoppi
-000031b0: 6e67 2072 6563 6f72 6469 6e67 2e2e 2e7a  ng recording...z
-000031c0: 2e57 6169 7469 6e67 2066 6f72 2076 6964  .Waiting for vid
-000031d0: 656f 2072 6563 6f72 6465 7220 746f 2073  eo recorder to s
-000031e0: 6176 6520 6f75 7420 6461 7461 2e2e 2e67  ave out data...g
-000031f0: 0000 0000 0000 e03f 467a 3d52 6563 6f72  .......?Fz=Recor
-00003200: 6469 6e67 206f 6620 6672 616d 6573 2069  ding of frames i
-00003210: 7320 636f 6d70 6c65 7465 2e2e 2e73 6967  s complete...sig
-00003220: 6e61 6c6c 696e 6720 6368 616e 6765 2069  nalling change i
-00003230: 6e20 7374 6174 7573 290c 725e 0000 0072  n status).r^...r
-00003240: 5f00 0000 7297 0000 00da 0e73 746f 705f  _...r......stop_
-00003250: 7265 636f 7264 696e 675a 0972 6563 6f72  recordingZ.recor
-00003260: 6469 6e67 7206 0000 0072 4400 0000 7237  dingr....rD...r7
-00003270: 0000 0072 3300 0000 724c 0000 0072 6b00  ...r3...rL...rk.
-00003280: 0000 7232 0000 0072 2c00 0000 7225 0000  ..r2...r,...r%..
-00003290: 0072 2500 0000 7226 0000 0072 9900 0000  .r%...r&...r....
-000032a0: cc01 0000 7318 0000 000a 010a 0108 010a  ....s...........
-000032b0: 0108 0108 fe06 040a 020c 0108 0210 0104  ................
-000032c0: ff7a 1653 6573 7369 6f6e 2e73 746f 705f  .z.Session.stop_
-000032d0: 7265 636f 7264 696e 6763 0100 0000 0000  recordingc......
-000032e0: 0000 0000 0000 0400 0000 0800 0000 0300  ................
-000032f0: 0000 7354 0000 0087 0066 0164 0164 0284  ..sT.....f.d.d..
-00003300: 087d 0174 0083 008f 177d 0288 006a 01a0  .}.t.....}...j..
-00003310: 02a1 0044 005d 087d 037c 02a0 037c 017c  ...D.].}.|...|.|
-00003320: 03a1 0201 0071 0f57 0064 0304 0004 0083  .....q.W.d......
-00003330: 0301 0064 0353 0031 0073 2377 0101 0001  ...d.S.1.s#w....
-00003340: 0001 0059 0001 0064 0353 0029 047a 8243  ...Y...d.S.).z.C
-00003350: 6861 6e67 6573 2074 6865 2063 616d 6572  hanges the camer
-00003360: 6120 7265 736f 6c75 7469 6f6e 2074 6f20  a resolution to 
-00003370: 7468 6520 7661 6c75 6520 696e 2074 6865  the value in the
-00003380: 2063 6f6e 6669 6775 7261 7469 6f6e 2c20   configuration, 
-00003390: 6173 0a20 2020 2020 2020 206c 6f67 2061  as.        log a
-000033a0: 7320 6974 2069 7320 6e6f 7420 636f 6e66  s it is not conf
-000033b0: 6967 7572 6564 2066 6f72 2074 6865 2064  igured for the d
-000033c0: 6566 6175 6c74 2072 6573 6f6c 7574 696f  efault resolutio
-000033d0: 6e63 0100 0000 0000 0000 0000 0000 0400  nc..............
-000033e0: 0000 0a00 0000 1300 0000 73b6 0000 0088  ..........s.....
-000033f0: 006a 007c 0019 007d 0188 006a 016a 0264  .j.|...}...j.j.d
-00003400: 017c 009b 009d 0219 0064 0219 007d 0288  .|.......d...}..
-00003410: 006a 037c 0019 006a 047d 037c 0264 0319  .j.|...j.}.|.d..
-00003420: 007c 0364 0319 006b 0373 267c 0264 0419  .|.d...k.s&|.d..
-00003430: 007c 0364 0419 006b 0372 5974 05a0 0664  .|.d...k.rYt...d
-00003440: 057c 009b 0064 067c 0364 0364 0785 0219  .|...d.|.d.d....
-00003450: 009b 0064 087c 0264 0364 0785 0219 009b  ...d.|.d.d......
-00003460: 009d 06a1 0101 007c 01a0 077c 02a1 0101  .......|...|....
-00003470: 0074 05a0 0664 097c 009b 0064 067c 0364  .t...d.|...d.|.d
-00003480: 0364 0785 0219 009b 0064 087c 0264 0364  .d.......d.|.d.d
-00003490: 0785 0219 009b 009d 06a1 0101 0064 0053  .............d.S
-000034a0: 0064 0053 0029 0a4e 5a04 6361 6d5f da04  .d.S.).NZ.cam_..
-000034b0: 7369 7a65 7201 0000 0072 7b00 0000 7a27  sizer....r{...z'
-000034c0: 4265 6769 6e6e 696e 6720 746f 2063 6861  Beginning to cha
-000034d0: 6e67 6520 7265 736f 6c75 7469 6f6e 2061  nge resolution a
-000034e0: 7420 706f 7274 207a 0620 6672 6f6d 2072  t port z. from r
-000034f0: 5b00 0000 7a04 2074 6f20 7a27 436f 6d70  [...z. to z'Comp
-00003500: 6c65 7465 6420 6368 616e 6765 206f 6620  leted change of 
-00003510: 7265 736f 6c75 7469 6f6e 2061 7420 706f  resolution at po
-00003520: 7274 2029 0872 3c00 0000 7236 0000 0072  rt ).r<...r6...r
-00003530: 7c00 0000 723b 0000 005a 1264 6566 6175  |...r;...Z.defau
-00003540: 6c74 5f72 6573 6f6c 7574 696f 6e72 5e00  lt_resolutionr^.
-00003550: 0000 725f 0000 005a 1163 6861 6e67 655f  ..r_...Z.change_
-00003560: 7265 736f 6c75 7469 6f6e 2904 724d 0000  resolution).rM..
-00003570: 0072 4e00 0000 729a 0000 005a 0c64 6566  .rN...r....Z.def
-00003580: 6175 6c74 5f73 697a 6572 2c00 0000 7225  ault_sizer,...r%
-00003590: 0000 0072 2600 0000 da11 6164 6a75 7374  ...r&.....adjust
-000035a0: 5f72 6573 5f77 6f72 6b65 72df 0100 0073  _res_worker....s
-000035b0: 1800 0000 0a01 1601 0c01 2002 0401 2401  .......... ...$.
-000035c0: 04ff 0a03 0401 2401 08ff 04fb 7a36 5365  ......$.....z6Se
-000035d0: 7373 696f 6e2e 5f61 646a 7573 745f 7265  ssion._adjust_re
-000035e0: 736f 6c75 7469 6f6e 732e 3c6c 6f63 616c  solutions.<local
-000035f0: 733e 2e61 646a 7573 745f 7265 735f 776f  s>.adjust_res_wo
-00003600: 726b 6572 4e29 0472 0400 0000 723b 0000  rkerN).r....r;..
-00003610: 0072 8800 0000 7289 0000 0029 0472 2d00  .r....r....).r-.
-00003620: 0000 729b 0000 0072 8a00 0000 724d 0000  ..r....r....rM..
-00003630: 0072 2500 0000 722c 0000 0072 2600 0000  .r%...r,...r&...
-00003640: 728d 0000 00db 0100 0073 0c00 0000 0c04  r........s......
-00003650: 080e 0e01 0e01 02ff 22ff 7a1b 5365 7373  ........".z.Sess
-00003660: 696f 6e2e 5f61 646a 7573 745f 7265 736f  ion._adjust_reso
-00003670: 6c75 7469 6f6e 7363 0100 0000 0000 0000  lutionsc........
-00003680: 0000 0000 0100 0000 0400 0000 4300 0000  ............C...
-00003690: 737a 0000 007c 006a 00a0 01a1 007c 005f  sz...|.j.....|._
-000036a0: 027c 006a 00a0 03a1 007c 005f 0474 057c  .|.j.....|._.t.|
-000036b0: 006a 047c 006a 0283 027c 005f 067c 006a  .j.|.j...|._.|.j
-000036c0: 006a 0764 0119 0064 0219 007c 006a 065f  .j.d...d...|.j._
-000036d0: 0864 037c 006a 006a 0764 0119 00a0 09a1  .d.|.j.j.d......
-000036e0: 0076 0072 327c 006a 006a 0764 0119 0064  .v.r2|.j.j.d...d
-000036f0: 0319 007c 006a 065f 0a74 0b7c 006a 067c  ...|.j._.t.|.j.|
-00003700: 006a 0c64 048d 027c 005f 0d64 0553 0029  .j.d...|._.d.S.)
-00003710: 067a f30a 2020 2020 2020 2020 466f 6c6c  .z..        Foll
-00003720: 6f77 696e 6720 6361 7074 7572 6520 766f  owing capture vo
-00003730: 6c75 6d65 206f 7074 696d 697a 6174 696f  lume optimizatio
-00003740: 6e20 7669 6120 6275 6e64 6c65 2061 646a  n via bundle adj
-00003750: 7573 746d 656e 742c 206f 7220 616c 7465  ustment, or alte
-00003760: 7261 7469 6f6e 0a20 2020 2020 2020 2076  ration.        v
-00003770: 6961 2061 2074 7261 6e73 666f 726d 206f  ia a transform o
-00003780: 6620 7468 6520 6f72 6967 696e 2c20 7468  f the origin, th
-00003790: 6520 656e 7469 7265 2063 6170 7475 7265  e entire capture
-000037a0: 2076 6f6c 756d 6520 6361 6e20 6265 2072   volume can be r
-000037b0: 656c 6f61 6465 640a 2020 2020 2020 2020  eloaded.        
-000037c0: 6672 6f6d 2074 6865 2063 6f6e 6669 6720  from the config 
-000037d0: 6461 7461 2077 6974 686f 7574 206e 6565  data without nee
-000037e0: 6469 6e67 2074 6f20 676f 2074 6872 6f75  ding to go throu
-000037f0: 6768 2074 6865 2073 7465 7073 0a0a 2020  gh the steps..  
-00003800: 2020 2020 2020 da0e 6361 7074 7572 655f        ..capture_
-00003810: 766f 6c75 6d65 da05 7374 6167 65da 116f  volume..stage..o
-00003820: 7269 6769 6e5f 7379 6e63 5f69 6e64 6578  rigin_sync_index
-00003830: 2901 7245 0000 004e 290e 7236 0000 0072  ).rE...N).r6...r
-00003840: 1400 0000 da0f 706f 696e 745f 6573 7469  ......point_esti
-00003850: 6d61 7465 7372 5600 0000 7257 0000 0072  matesrV...rW...r
-00003860: 1100 0000 729c 0000 0072 7c00 0000 729d  ....r....r|...r.
-00003870: 0000 0072 8800 0000 729e 0000 0072 1200  ...r....r....r..
-00003880: 0000 7245 0000 00da 1271 7561 6c69 7479  ..rE.....quality
-00003890: 5f63 6f6e 7472 6f6c 6c65 7272 2c00 0000  _controllerr,...
-000038a0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-000038b0: 1d6c 6f61 645f 6573 7469 6d61 7465 645f  .load_estimated_
-000038c0: 6361 7074 7572 655f 766f 6c75 6d65 f101  capture_volume..
-000038d0: 0000 7316 0000 000c 070c 0110 0114 0214  ..s.............
-000038e0: 010a 0102 0108 ff02 0508 010c ff7a 2553  .............z%S
-000038f0: 6573 7369 6f6e 2e6c 6f61 645f 6573 7469  ession.load_esti
-00003900: 6d61 7465 645f 6361 7074 7572 655f 766f  mated_capture_vo
-00003910: 6c75 6d65 6301 0000 0000 0000 0000 0000  lumec...........
-00003920: 0002 0000 0005 0000 0043 0000 0073 a600  .........C...s..
-00003930: 0000 7400 7c00 6a01 6a02 7c00 6a03 8302  ..t.|.j.j.|.j...
-00003940: 7d01 7c01 6a04 6401 6402 8d01 0100 7405  }.|.j.d.d.....t.
-00003950: 7c00 6a01 6a02 8301 a006 a100 7c00 5f07  |.j.j.......|._.
-00003960: 7408 7c00 6a07 7c00 6a03 8302 7c00 5f09  t.|.j.|.j...|._.
-00003970: 740a 7c00 6a07 7c00 6a09 8302 7c00 5f0b  t.|.j.|.j...|._.
-00003980: 7c00 6a0b a00c a100 0100 740d 7c00 6a0b  |.j.......t.|.j.
-00003990: 7c00 6a0e 8302 7c00 5f0f 7410 a011 6403  |.j...|._.t...d.
-000039a0: 7412 6404 1400 9b00 6405 9d03 a101 0100  t.d.....d.......
-000039b0: 7c00 6a0f a013 7412 a101 0100 7c00 6a0b  |.j...t.....|.j.
-000039c0: a00c a100 0100 7c00 6a01 a014 7c00 6a0b  ......|.j...|.j.
-000039d0: a101 0100 6406 5300 2907 7ad7 0a20 2020  ....d.S.).z..   
-000039e0: 2020 2020 2054 6869 7320 6973 2077 6865       This is whe
-000039f0: 7265 2074 6865 2063 616d 6572 6120 6172  re the camera ar
-00003a00: 7261 7920 3620 446f 4620 6973 2073 6574  ray 6 DoF is set
-00003a10: 2e20 4d61 6e79 2c20 6d61 6e79 2074 6869  . Many, many thi
-00003a20: 6e67 7320 6172 6520 6861 7070 656e 696e  ngs are happenin
-00003a30: 670a 2020 2020 2020 2020 6865 7265 2c20  g.        here, 
-00003a40: 6275 7420 7468 6579 2061 7265 2061 6c6c  but they are all
-00003a50: 206e 6563 6573 7361 7279 2073 7465 7073   necessary steps
-00003a60: 206f 6620 7468 6520 7072 6f63 6573 7320   of the process 
-00003a70: 736f 2049 2064 6964 6e27 7420 7761 6e74  so I didn't want
-00003a80: 2074 6f0a 2020 2020 2020 2020 7472 7920   to.        try 
-00003a90: 746f 2065 6e63 6170 7375 6c61 7465 2061  to encapsulate a
-00003aa0: 6e79 2066 7572 7468 6572 0a20 2020 2020  ny further.     
-00003ab0: 2020 2072 1800 0000 2901 5a0e 626f 6172     r....).Z.boar
-00003ac0: 6473 5f73 616d 706c 6564 7a1b 5265 6d6f  ds_sampledz.Remo
-00003ad0: 7669 6e67 2074 6865 2077 6f72 7374 2066  ving the worst f
-00003ae0: 6974 7469 6e67 20e9 6400 0000 7a21 2070  itting .d...z! p
-00003af0: 6572 6365 6e74 206f 6620 706f 696e 7473  ercent of points
-00003b00: 2066 726f 6d20 7468 6520 6d6f 6465 6c4e   from the modelN
-00003b10: 2915 720f 0000 0072 3600 0000 5a09 746f  ).r....r6...Z.to
-00003b20: 6d6c 5f70 6174 6872 3a00 0000 5a14 7374  ml_pathr:...Z.st
-00003b30: 6572 656f 5f63 616c 6962 7261 7465 5f61  ereo_calibrate_a
-00003b40: 6c6c 720d 0000 005a 1567 6574 5f62 6573  llr....Z.get_bes
-00003b50: 745f 6361 6d65 7261 5f61 7272 6179 7257  t_camera_arrayrW
-00003b60: 0000 0072 1400 0000 729f 0000 0072 1100  ...r....r....r..
-00003b70: 0000 729c 0000 00da 086f 7074 696d 697a  ..r......optimiz
-00003b80: 6572 1200 0000 7245 0000 0072 a000 0000  er....rE...r....
-00003b90: 725e 0000 0072 5f00 0000 da11 4649 4c54  r^...r_.....FILT
-00003ba0: 4552 4544 5f46 5241 4354 494f 4e5a 1666  ERED_FRACTIONZ.f
-00003bb0: 696c 7465 725f 706f 696e 745f 6573 7469  ilter_point_esti
-00003bc0: 6d61 7465 735a 1373 6176 655f 6361 7074  matesZ.save_capt
-00003bd0: 7572 655f 766f 6c75 6d65 2902 722d 0000  ure_volume).r-..
-00003be0: 005a 1073 7465 7265 6f63 616c 6962 7261  .Z.stereocalibra
-00003bf0: 746f 7272 2500 0000 7225 0000 0072 2600  torr%...r%...r&.
-00003c00: 0000 da13 6573 7469 6d61 7465 5f65 7874  ....estimate_ext
-00003c10: 7269 6e73 6963 7307 0200 0073 2a00 0000  rinsics....s*...
-00003c20: 0206 0a01 04ff 0c03 0202 0601 02ff 0402  ................
-00003c30: 04fe 0204 0801 06ff 1004 0a01 1002 0402  ................
-00003c40: 0e01 04ff 0c03 0a01 1202 7a1b 5365 7373  ..........z.Sess
-00003c50: 696f 6e2e 6573 7469 6d61 7465 5f65 7874  ion.estimate_ext
-00003c60: 7269 6e73 6963 7372 2900 0000 2901 4629  rinsicsr)...).F)
-00003c70: 2272 1b00 0000 721c 0000 0072 1d00 0000  "r....r....r....
-00003c80: 7215 0000 0072 2b00 0000 7251 0000 0072  r....r+...rQ...r
-00003c90: 5400 0000 725a 0000 0072 6100 0000 7264  T...rZ...ra...rd
-00003ca0: 0000 0072 6b00 0000 7219 0000 0072 7400  ...rk...r....rt.
-00003cb0: 0000 da03 696e 7472 7600 0000 7277 0000  ....intrv...rw..
-00003cc0: 0072 6c00 0000 da04 626f 6f6c 7271 0000  .rl.....boolrq..
-00003cd0: 0072 7000 0000 7279 0000 0072 7a00 0000  .rp...ry...rz...
-00003ce0: 7282 0000 0072 8c00 0000 726f 0000 0072  r....r....ro...r
-00003cf0: 8e00 0000 7272 0000 0072 6e00 0000 7205  ....rr...rn...r.
-00003d00: 0000 0072 9800 0000 7299 0000 0072 8d00  ...r....r....r..
-00003d10: 0000 72a1 0000 0072 a500 0000 7225 0000  ..r....r....r%..
-00003d20: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00003d30: 7235 0000 003b 0000 0073 4000 0000 0800  r5...;...s@.....
-00003d40: 0e01 0824 0812 0807 080b 081d 081e 0e10  ...$............
-00003d50: 0e41 0e16 080f 0e06 0804 0806 0804 0804  .A..............
-00003d60: 0807 0823 0828 100b 080d 020a 04ff 0201  ...#.(..........
-00003d70: 02ff 0201 0aff 080c 080f 0816 0c16 7235  ..............r5
-00003d80: 0000 0029 35da 0674 7970 696e 67da 0d70  ...)5..typing..p
-00003d90: 7978 7933 642e 6c6f 6767 6572 da06 7079  yxy3d.logger..py
-00003da0: 7879 3364 725e 0000 00da 0367 6574 721b  xy3dr^.....getr.
-00003db0: 0000 00da 0c50 7951 7436 2e51 7443 6f72  .....PyQt6.QtCor
-00003dc0: 6572 0200 0000 7203 0000 005a 1263 6f6e  er....r....Z.con
-00003dd0: 6375 7272 656e 742e 6675 7475 7265 7372  current.futuresr
-00003de0: 0400 0000 da07 7061 7468 6c69 6272 0500  ......pathlibr..
-00003df0: 0000 da04 7469 6d65 7206 0000 00da 0465  ....timer......e
-00003e00: 6e75 6d72 0700 0000 7208 0000 005a 1f70  numr....r....Z.p
-00003e10: 7978 7933 642e 7472 6163 6b65 7273 2e63  yxy3d.trackers.c
-00003e20: 6861 7275 636f 5f74 7261 636b 6572 7209  haruco_trackerr.
-00003e30: 0000 005a 2170 7978 7933 642e 6361 6c69  ...Z!pyxy3d.cali
-00003e40: 6272 6174 696f 6e2e 6d6f 6e6f 6361 6c69  bration.monocali
-00003e50: 6272 6174 6f72 720a 0000 005a 1570 7978  bratorr....Z.pyx
-00003e60: 7933 642e 6361 6d65 7261 732e 6361 6d65  y3d.cameras.came
-00003e70: 7261 720b 0000 00da 1b70 7978 7933 642e  rar......pyxy3d.
-00003e80: 6361 6d65 7261 732e 7379 6e63 6872 6f6e  cameras.synchron
-00003e90: 697a 6572 720c 0000 005a 2770 7978 7933  izerr....Z'pyxy3
-00003ea0: 642e 6361 6d65 7261 732e 6361 6d65 7261  d.cameras.camera
-00003eb0: 5f61 7272 6179 5f69 6e69 7469 616c 697a  _array_initializ
-00003ec0: 6572 720d 0000 005a 1070 7978 7933 642e  err....Z.pyxy3d.
-00003ed0: 696e 7465 7266 6163 6572 0e00 0000 5a23  interfacer....Z#
-00003ee0: 7079 7879 3364 2e63 616c 6962 7261 7469  pyxy3d.calibrati
-00003ef0: 6f6e 2e73 7465 7265 6f63 616c 6962 7261  on.stereocalibra
-00003f00: 746f 7272 0f00 0000 5a31 7079 7879 3364  torr....Z1pyxy3d
-00003f10: 2e63 616c 6962 7261 7469 6f6e 2e63 6170  .calibration.cap
-00003f20: 7475 7265 5f76 6f6c 756d 652e 706f 696e  ture_volume.poin
-00003f30: 745f 6573 7469 6d61 7465 7372 1000 0000  t_estimatesr....
-00003f40: 5a30 7079 7879 3364 2e63 616c 6962 7261  Z0pyxy3d.calibra
-00003f50: 7469 6f6e 2e63 6170 7475 7265 5f76 6f6c  tion.capture_vol
-00003f60: 756d 652e 6361 7074 7572 655f 766f 6c75  ume.capture_volu
-00003f70: 6d65 7211 0000 005a 3470 7978 7933 642e  mer....Z4pyxy3d.
-00003f80: 6361 6c69 6272 6174 696f 6e2e 6361 7074  calibration.capt
-00003f90: 7572 655f 766f 6c75 6d65 2e71 7561 6c69  ure_volume.quali
-00003fa0: 7479 5f63 6f6e 7472 6f6c 6c65 7272 1200  ty_controllerr..
-00003fb0: 0000 5a1b 7079 7879 3364 2e63 616d 6572  ..Z.pyxy3d.camer
-00003fc0: 6173 2e63 616d 6572 615f 6172 7261 7972  as.camera_arrayr
-00003fd0: 1300 0000 5a46 7079 7879 3364 2e63 616c  ....ZFpyxy3d.cal
-00003fe0: 6962 7261 7469 6f6e 2e63 6170 7475 7265  ibration.capture
-00003ff0: 5f76 6f6c 756d 652e 6865 6c70 6572 5f66  _volume.helper_f
-00004000: 756e 6374 696f 6e73 2e67 6574 5f70 6f69  unctions.get_poi
-00004010: 6e74 5f65 7374 696d 6174 6573 7214 0000  nt_estimatesr...
-00004020: 00da 1370 7978 7933 642e 636f 6e66 6967  ...pyxy3d.config
-00004030: 7572 6174 6f72 7215 0000 005a 1a70 7978  uratorr....Z.pyx
-00004040: 7933 642e 6361 6d65 7261 732e 6c69 7665  y3d.cameras.live
-00004050: 5f73 7472 6561 6d72 1600 0000 da1f 7079  _streamr......py
-00004060: 7879 3364 2e72 6563 6f72 6469 6e67 2e76  xy3d.recording.v
-00004070: 6964 656f 5f72 6563 6f72 6465 7272 1700  ideo_recorderr..
-00004080: 0000 7287 0000 0072 a400 0000 7219 0000  ..r....r....r...
-00004090: 0072 2700 0000 7235 0000 0072 2500 0000  .r'...r5...r%...
-000040a0: 7225 0000 0072 2500 0000 7226 0000 00da  r%...r%...r&....
-000040b0: 083c 6d6f 6475 6c65 3e01 0000 0073 3800  .<module>....s8.
-000040c0: 0000 0801 0801 0c02 1002 0c01 0c01 0c01  ................
-000040d0: 1001 0c02 0c01 0c01 0c01 0c01 0c01 0c02  ................
-000040e0: 0c01 0c01 0c01 0c02 0c01 0c03 0c01 0c01  ................
-000040f0: 0403 0401 1003 100a 120b                 ..........
+00001390: 6769 626c 65a1 0000 0073 2a00 0000 0a07  gible....s*.....
+000013a0: 0c01 0403 1001 0401 1402 0a01 0801 02ff  ................
+000013b0: 0801 02ff 0403 0401 0a01 04ff 0280 0403  ................
+000013c0: 0401 0404 04fe 0402 7a1d 5365 7373 696f  ........z.Sessio
+000013d0: 6e2e 6973 5f72 6563 6f72 6469 6e67 5f65  n.is_recording_e
+000013e0: 6c69 6769 626c 6563 0100 0000 0000 0000  ligiblec........
+000013f0: 0000 0000 0500 0000 0500 0000 4300 0000  ............C...
+00001400: 7346 0000 0064 017d 017c 006a 00a0 01a1  sF...d.}.|.j....
+00001410: 0044 005d 197d 027c 02a0 02a1 0072 2074  .D.].}.|.....r t
+00001420: 037c 02a0 0464 02a1 0183 017d 037c 0264  .|...d.....}.|.d
+00001430: 031b 007d 047c 0372 207c 04a0 05a1 0072  ...}.|.r |.....r
+00001440: 2064 047d 0171 077c 0153 0029 057a a60a   d.}.q.|.S.).z..
+00001450: 2020 2020 2020 2020 506f 7374 2070 726f          Post pro
+00001460: 6365 7373 696e 6720 6361 6e20 6f6e 6c79  cessing can only
+00001470: 2062 6520 7065 7266 6f72 6d65 6420 6966   be performed if
+00001480: 2072 6563 6f72 6469 6e67 7320 286d 7034   recordings (mp4
+00001490: 2066 696c 6573 2920 6578 6973 7420 616e   files) exist an
+000014a0: 6420 6578 7472 696e 7369 6373 200a 2020  d extrinsics .  
+000014b0: 2020 2020 2020 2863 6f6e 6669 672e 746f        (config.to
+000014c0: 6d6c 2920 6172 6520 6361 6c69 6272 6174  ml) are calibrat
+000014d0: 6564 2069 6e20 7468 6520 2772 6563 6f72  ed in the 'recor
+000014e0: 6427 2064 6972 6563 746f 7279 0a20 2020  d' directory.   
+000014f0: 2020 2020 2046 7a05 2a2e 6d70 347a 0b63       Fz.*.mp4z.c
+00001500: 6f6e 6669 672e 746f 6d6c 5429 0672 3900  onfig.tomlT).r9.
+00001510: 0000 da07 6974 6572 6469 72da 0669 735f  ....iterdir..is_
+00001520: 6469 72da 046c 6973 74da 0467 6c6f 62da  dir..list..glob.
+00001530: 0665 7869 7374 7329 0572 2d00 0000 7253  .exists).r-...rS
+00001540: 0000 00da 0563 6869 6c64 5a09 6d70 345f  .....childZ.mp4_
+00001550: 6669 6c65 735a 0b63 6f6e 6669 675f 6669  filesZ.config_fi
+00001560: 6c65 7225 0000 0072 2500 0000 7226 0000  ler%...r%...r&..
+00001570: 00da 1b69 735f 706f 7374 5f70 726f 6365  ...is_post_proce
+00001580: 7373 696e 675f 656c 6967 6962 6c65 bf00  ssing_eligible..
+00001590: 0000 7312 0000 0004 060e 0108 010e 0108  ..s.............
+000015a0: 010c 0104 0102 8004 027a 2353 6573 7369  .........z#Sessi
+000015b0: 6f6e 2e69 735f 706f 7374 5f70 726f 6365  on.is_post_proce
+000015c0: 7373 696e 675f 656c 6967 6962 6c65 7247  ssing_eligiblerG
+000015d0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000015e0: 0200 0000 0300 0000 4300 0000 73bc 0100  ........C...s...
+000015f0: 007c 017c 005f 007c 00a0 01a1 0001 007c  .|.|._.|.......|
+00001600: 006a 0004 0074 026a 036b 0272 1f01 007c  .j...t.j.k.r...|
+00001610: 006a 0472 1d7c 006a 05a0 06a1 0001 007c  .j.r.|.j.......|
+00001620: 00a0 07a1 0001 0064 0953 0064 0953 0004  .......d.S.d.S..
+00001630: 0074 026a 086b 0272 3501 007c 006a 0472  .t.j.k.r5..|.j.r
+00001640: 337c 006a 05a0 06a1 0001 007c 00a0 07a1  3|.j.......|....
+00001650: 0001 0064 0953 0064 0953 0004 0074 026a  ...d.S.d.S...t.j
+00001660: 096b 0272 6201 0074 0a7c 006a 0b83 017c  .k.rb..t.|.j...|
+00001670: 005f 0c7c 006a 0473 487c 00a0 0da1 0001  ._.|.j.sH|......
+00001680: 007c 006a 05a0 06a1 0001 007c 00a0 07a1  .|.j.......|....
+00001690: 0001 007c 00a0 0ea1 0001 007c 00a0 0f64  ...|.......|...d
+000016a0: 01a1 0101 007c 00a0 107c 006a 11a1 0101  .....|...|.j....
+000016b0: 0064 0953 0004 0074 026a 126b 0272 8901  .d.S...t.j.k.r..
+000016c0: 0074 0a7c 006a 0b83 017c 005f 0c7c 006a  .t.|.j...|._.|.j
+000016d0: 0473 757c 00a0 0da1 0001 007c 00a0 07a1  .su|.......|....
+000016e0: 0001 007c 00a0 0ea1 0001 007c 00a0 0f64  ...|.......|...d
+000016f0: 01a1 0101 007c 006a 05a0 13a1 0001 0064  .....|.j.......d
+00001700: 0953 0004 0074 026a 146b 0272 9f01 007c  .S...t.j.k.r...|
+00001710: 006a 0472 9d7c 00a0 07a1 0001 007c 006a  .j.r.|.......|.j
+00001720: 05a0 06a1 0001 0064 0953 0064 0953 0074  .......d.S.d.S.t
+00001730: 026a 156b 0272 dc74 16a0 1764 02a1 0101  .j.k.r.t...d....
+00001740: 007c 006a 0473 b474 16a0 1764 03a1 0101  .|.j.s.t...d....
+00001750: 007c 00a0 0da1 0001 0074 16a0 1764 04a1  .|.......t...d..
+00001760: 0101 007c 00a0 07a1 0001 0074 16a0 1764  ...|.......t...d
+00001770: 05a1 0101 007c 00a0 0f64 06a1 0101 0074  .....|...d.....t
+00001780: 16a0 1764 07a1 0101 007c 00a0 01a1 0001  ...d.....|......
+00001790: 0074 16a0 1764 08a1 0101 007c 006a 05a0  .t...d.....|.j..
+000017a0: 13a1 0001 0064 0953 0064 0953 0029 0a7a  .....d.S.d.S.).z
+000017b0: af0a 2020 2020 2020 2020 5669 6120 7468  ..        Via th
+000017c0: 6973 206d 6574 686f 642c 2074 6865 2066  is method, the f
+000017d0: 7261 6d65 2072 6561 6469 6e67 2062 6568  rame reading beh
+000017e0: 6176 696f 7220 7769 6c6c 2062 6520 6368  avior will be ch
+000017f0: 616e 6765 6420 6279 2074 6865 2047 5549  anged by the GUI
+00001800: 2e20 4966 2073 6f6d 6520 7072 6f70 6572  . If some proper
+00001810: 7469 6573 2061 7265 0a20 2020 2020 2020  ties are.       
+00001820: 206e 6f74 2061 7661 696c 6162 6c65 2028   not available (
+00001830: 692e 652e 2073 796e 6368 726f 6e69 7a65  i.e. synchronize
+00001840: 7229 2074 6865 7920 7769 6c6c 2062 6520  r) they will be 
+00001850: 6372 6561 7465 640a 2020 2020 2020 2020  created.        
+00001860: 547a 2041 7474 656d 7074 696e 6720 746f  Tz Attempting to
+00001870: 2073 6574 2072 6563 6f72 6469 6e67 206d   set recording m
+00001880: 6f64 657a 2e53 7472 6561 6d20 746f 6f6c  odez.Stream tool
+00001890: 7320 6e6f 7420 6c6f 6164 6564 2c20 736f  s not loaded, so
+000018a0: 206c 6f61 6469 6e67 2074 6865 6d20 7570   loading them up
+000018b0: 2e2e 2e7a 2850 6175 7369 6e67 206d 6f6e  ...z(Pausing mon
+000018c0: 6f63 616c 7320 746f 2065 6e74 6572 2072  ocals to enter r
+000018d0: 6563 6f72 6469 6e67 206d 6f64 657a 2053  ecording modez S
+000018e0: 746f 7020 7472 6163 6b69 6e67 2066 6f72  top tracking for
+000018f0: 2072 6563 6f72 6469 6e67 206d 6f64 6546   recording modeF
+00001900: 7a22 5570 6461 7465 2073 7472 6561 6d20  z"Update stream 
+00001910: 6670 7320 746f 2072 6563 6f72 6469 6e67  fps to recording
+00001920: 2066 7073 7a3e 5375 6273 6372 6962 6520   fpsz>Subscribe 
+00001930: 7379 6e63 6872 6f6e 697a 6572 2074 6f20  synchronizer to 
+00001940: 7374 7265 616d 7320 736f 2076 6964 656f  streams so video
+00001950: 2072 6563 6f72 6465 7220 6361 6e20 6d61   recorder can ma
+00001960: 6e61 6765 4e29 1872 4700 0000 da12 7570  nageN).rG.....up
+00001970: 6461 7465 5f73 7472 6561 6d73 5f66 7073  date_streams_fps
+00001980: 7219 0000 0072 1f00 0000 723e 0000 0072  r....r....r>...r
+00001990: 4b00 0000 da18 756e 7375 6273 6372 6962  K.....unsubscrib
+000019a0: 655f 6672 6f6d 5f73 7472 6561 6d73 da19  e_from_streams..
+000019b0: 7061 7573 655f 616c 6c5f 6d6f 6e6f 6361  pause_all_monoca
+000019c0: 6c69 6272 6174 6f72 7372 2400 0000 7220  libratorsr$...r 
+000019d0: 0000 0072 0900 0000 7245 0000 0072 4600  ...r....rE...rF.
+000019e0: 0000 da11 6c6f 6164 5f73 7472 6561 6d5f  ....load_stream_
+000019f0: 746f 6f6c 73da 1373 6574 5f73 7472 6561  tools..set_strea
+00001a00: 6d73 5f63 6861 7275 636f da14 7365 745f  ms_charuco..set_
+00001a10: 7374 7265 616d 735f 7472 6163 6b69 6e67  streams_tracking
+00001a20: da17 6163 7469 7661 7465 5f6d 6f6e 6f63  ..activate_monoc
+00001a30: 616c 6962 7261 746f 7272 4000 0000 7221  alibratorr@...r!
+00001a40: 0000 00da 1473 7562 7363 7269 6265 5f74  .....subscribe_t
+00001a50: 6f5f 7374 7265 616d 7372 2200 0000 7223  o_streamsr"...r#
+00001a60: 0000 0072 5e00 0000 725f 0000 0029 0272  ...r^...r_...).r
+00001a70: 2d00 0000 7247 0000 0072 2500 0000 7225  -...rG...r%...r%
+00001a80: 0000 0072 2600 0000 da08 7365 745f 6d6f  ...r&.....set_mo
+00001a90: 6465 cf00 0000 7362 0000 0006 0508 0104  de....sb........
+00001aa0: 020c 0106 010a 010c 0104 fe0c 0406 010a  ................
+00001ab0: 010c 0104 fe0c 040c 0206 0208 010a 0108  ................
+00001ac0: 0108 010a 0110 010c 020c 0206 0108 0108  ................
+00001ad0: 0208 010a 010e 020c 0206 0108 010e 0104  ................
+00001ae0: fe08 040a 0106 010a 0108 010a 0208 010a  ................
+00001af0: 020a 010a 0108 010a 020e 0104 f17a 1053  .............z.S
+00001b00: 6573 7369 6f6e 2e73 6574 5f6d 6f64 65da  ession.set_mode.
+00001b10: 0a66 7073 5f74 6172 6765 7463 0200 0000  .fps_targetc....
+00001b20: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001b30: 4300 0000 7386 0000 007c 006a 0004 0074  C...s....|.j...t
+00001b40: 016a 026b 0272 0901 006e 3404 0074 016a  .j.k.r...n4..t.j
+00001b50: 036b 0272 1001 006e 2d04 0074 016a 046b  .k.r...n-..t.j.k
+00001b60: 0272 2001 007c 017c 005f 057c 006a 06a0  .r ..|.|._.|.j..
+00001b70: 077c 01a1 0101 006e 1d04 0074 016a 086b  .|.....n...t.j.k
+00001b80: 0272 3001 007c 017c 005f 097c 006a 06a0  .r0..|.|._.|.j..
+00001b90: 0a7c 01a1 0101 006e 0d74 016a 0b6b 0272  .|.....n.t.j.k.r
+00001ba0: 3d7c 017c 005f 0c7c 006a 06a0 0d7c 01a1  =|.|._.|.j...|..
+00001bb0: 0101 007c 00a0 0ea1 0001 0064 0153 0029  ...|.......d.S.)
+00001bc0: 027a 780a 2020 2020 2020 2020 5570 6461  .zx.        Upda
+00001bd0: 7465 7320 7468 6520 4650 5320 7573 6564  tes the FPS used
+00001be0: 2062 7920 7468 6520 6375 7272 656e 746c   by the currentl
+00001bf0: 7920 6163 7469 7665 2073 6573 7369 6f6e  y active session
+00001c00: 206d 6f64 650a 2020 2020 2020 2020 5468   mode.        Th
+00001c10: 6973 2075 7064 6174 6520 696e 636c 7564  is update includ
+00001c20: 6573 2074 6865 2063 6f6e 6669 672e 746f  es the config.to
+00001c30: 6d6c 0a20 2020 2020 2020 204e 290f 7247  ml.        N).rG
+00001c40: 0000 0072 1900 0000 721f 0000 0072 2400  ...r....r....r$.
+00001c50: 0000 7220 0000 0072 4300 0000 7236 0000  ..r ...rC...r6..
+00001c60: 005a 1e73 6176 655f 6670 735f 696e 7472  .Z.save_fps_intr
+00001c70: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
+00001c80: 6e72 2100 0000 7242 0000 005a 1e73 6176  nr!...rB...Z.sav
+00001c90: 655f 6670 735f 6578 7472 696e 7369 635f  e_fps_extrinsic_
+00001ca0: 6361 6c69 6272 6174 696f 6e72 2300 0000  calibrationr#...
+00001cb0: 7241 0000 005a 1273 6176 655f 6670 735f  rA...Z.save_fps_
+00001cc0: 7265 636f 7264 696e 6772 6c00 0000 2902  recordingrl...).
+00001cd0: 722d 0000 0072 7500 0000 7225 0000 0072  r-...ru...r%...r
+00001ce0: 2500 0000 7226 0000 00da 1373 6574 5f61  %...r&.....set_a
+00001cf0: 6374 6976 655f 6d6f 6465 5f66 7073 1001  ctive_mode_fps..
+00001d00: 0000 731e 0000 0004 050c 0102 010c 0102  ..s.............
+00001d10: 010c 0106 010e 010c 0106 010e 0108 0106  ................
+00001d20: 010c 010c 027a 1b53 6573 7369 6f6e 2e73  .....z.Session.s
+00001d30: 6574 5f61 6374 6976 655f 6d6f 6465 5f66  et_active_mode_f
+00001d40: 7073 7228 0000 0063 0100 0000 0000 0000  psr(...c........
+00001d50: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+00001d60: 736e 0000 0064 007d 017c 006a 0004 0074  sn...d.}.|.j...t
+00001d70: 016a 026b 0272 0d01 0009 007c 0153 0004  .j.k.r.....|.S..
+00001d80: 0074 016a 036b 0272 1601 0009 007c 0153  .t.j.k.r.....|.S
+00001d90: 0004 0074 016a 046b 0272 2101 007c 006a  ...t.j.k.r!..|.j
+00001da0: 057d 017c 0153 0004 0074 016a 066b 0272  .}.|.S...t.j.k.r
+00001db0: 2c01 007c 006a 077d 017c 0153 0074 016a  ,..|.j.}.|.S.t.j
+00001dc0: 086b 0272 357c 006a 097d 017c 0153 007c  .k.r5|.j.}.|.S.|
+00001dd0: 0153 0072 2900 0000 290a 7247 0000 0072  .S.r)...).rG...r
+00001de0: 1900 0000 721f 0000 0072 2400 0000 7220  ....r....r$...r 
+00001df0: 0000 0072 4300 0000 7221 0000 0072 4200  ...rC...r!...rB.
+00001e00: 0000 7223 0000 0072 4100 0000 2902 722d  ..r#...rA...).r-
+00001e10: 0000 005a 0366 7073 7225 0000 0072 2500  ...Z.fpsr%...r%.
+00001e20: 0000 7226 0000 00da 1367 6574 5f61 6374  ..r&.....get_act
+00001e30: 6976 655f 6d6f 6465 5f66 7073 2601 0000  ive_mode_fps&...
+00001e40: 7322 0000 0004 0104 010c 0102 0104 090c  s"..............
+00001e50: f802 0104 070c fa06 0104 050c fc06 0104  ................
+00001e60: 0308 fe06 0108 017a 1b53 6573 7369 6f6e  .......z.Session
+00001e70: 2e67 6574 5f61 6374 6976 655f 6d6f 6465  .get_active_mode
+00001e80: 5f66 7073 6301 0000 0000 0000 0000 0000  _fpsc...........
+00001e90: 0004 0000 0004 0000 0043 0000 0073 3600  .........C...s6.
+00001ea0: 0000 7c00 a000 a100 7d01 7c01 6400 7501  ..|.....}.|.d.u.
+00001eb0: 7217 7c00 6a01 a002 a100 4400 5d0b 5c02  r.|.j.....D.].\.
+00001ec0: 7d02 7d03 7c03 a003 7c01 a101 0100 710d  }.}.|...|.....q.
+00001ed0: 6400 5300 6400 5300 7229 0000 0029 0472  d.S.d.S.r)...).r
+00001ee0: 7700 0000 723c 0000 0072 4800 0000 5a0e  w...r<...rH...Z.
+00001ef0: 7365 745f 6670 735f 7461 7267 6574 2904  set_fps_target).
+00001f00: 722d 0000 005a 0f61 6374 6976 655f 6d6f  r-...Z.active_mo
+00001f10: 6465 5f66 7073 724d 0000 0072 4e00 0000  de_fpsrM...rN...
+00001f20: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
+00001f30: 6c00 0000 3501 0000 730c 0000 0008 0108  l...5...s.......
+00001f40: 0112 010c 0104 fe04 017a 1a53 6573 7369  .........z.Sessi
+00001f50: 6f6e 2e75 7064 6174 655f 7374 7265 616d  on.update_stream
+00001f60: 735f 6670 73da 0b74 7261 636b 696e 675f  s_fps..tracking_
+00001f70: 6f6e 6302 0000 0000 0000 0000 0000 0004  onc.............
+00001f80: 0000 0004 0000 0043 0000 0073 2200 0000  .......C...s"...
+00001f90: 7c00 6a00 a001 a100 4400 5d09 5c02 7d02  |.j.....D.].\.}.
+00001fa0: 7d03 7c03 a002 7c01 a101 0100 7105 6400  }.|...|.....q.d.
+00001fb0: 5300 7229 0000 0029 0372 3c00 0000 7248  S.r)...).r<...rH
+00001fc0: 0000 005a 0f73 6574 5f74 7261 636b 696e  ...Z.set_trackin
+00001fd0: 675f 6f6e 2904 722d 0000 0072 7800 0000  g_on).r-...rx...
+00001fe0: 724d 0000 0072 4e00 0000 7225 0000 0072  rM...rN...r%...r
+00001ff0: 2500 0000 7226 0000 0072 7100 0000 3b01  %...r&...rq...;.
+00002000: 0000 7306 0000 0012 010c 0104 ff7a 1c53  ..s..........z.S
+00002010: 6573 7369 6f6e 2e73 6574 5f73 7472 6561  ession.set_strea
+00002020: 6d73 5f74 7261 636b 696e 6763 0100 0000  ms_trackingc....
+00002030: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00002040: 4300 0000 733a 0000 0074 00a0 0164 01a1  C...s:...t...d..
+00002050: 0101 0074 027c 006a 0383 017c 005f 047c  ...t.|.j...|._.|
+00002060: 006a 05a0 06a1 0044 005d 0a5c 027d 017d  .j.....D.].\.}.}
+00002070: 027c 02a0 077c 006a 04a1 0101 0071 1064  .|...|.j.....q.d
+00002080: 0053 0029 024e 7a22 7570 6461 7469 6e67  .S.).Nz"updating
+00002090: 2063 6861 7275 636f 2069 6e20 6361 7365   charuco in case
+000020a0: 206e 6563 6573 7361 7279 2908 725e 0000   necessary).r^..
+000020b0: 0072 5f00 0000 7209 0000 0072 4500 0000  .r_...r....rE...
+000020c0: 7246 0000 0072 3c00 0000 7248 0000 005a  rF...r<...rH...Z
+000020d0: 0e75 7064 6174 655f 7472 6163 6b65 7229  .update_tracker)
+000020e0: 0372 2d00 0000 724d 0000 0072 4e00 0000  .r-...rM...rN...
+000020f0: 7225 0000 0072 2500 0000 7226 0000 0072  r%...r%...r&...r
+00002100: 7000 0000 3f01 0000 730a 0000 000a 010c  p...?...s.......
+00002110: 0112 010e 0104 ff7a 1b53 6573 7369 6f6e  .......z.Session
+00002120: 2e73 6574 5f73 7472 6561 6d73 5f63 6861  .set_streams_cha
+00002130: 7275 636f 6301 0000 0000 0000 0000 0000  rucoc...........
+00002140: 0001 0000 0003 0000 0043 0000 0073 1800  .........C...s..
+00002150: 0000 7400 a001 6401 a101 0100 7c00 6a02  ..t...d.....|.j.
+00002160: a003 a100 0100 6400 5300 2902 4e7a 1470  ......d.S.).Nz.p
+00002170: 6175 7369 6e67 2073 796e 6368 726f 6e69  ausing synchroni
+00002180: 7a65 7229 0472 5e00 0000 725f 0000 0072  zer).r^...r_...r
+00002190: 4b00 0000 726d 0000 0072 2c00 0000 7225  K...rm...r,...r%
+000021a0: 0000 0072 2500 0000 7226 0000 00da 1270  ...r%...r&.....p
+000021b0: 6175 7365 5f73 796e 6368 726f 6e69 7a65  ause_synchronize
+000021c0: 7245 0100 0073 0400 0000 0a01 0e01 7a1a  rE...s........z.
+000021d0: 5365 7373 696f 6e2e 7061 7573 655f 7379  Session.pause_sy
+000021e0: 6e63 6872 6f6e 697a 6572 6301 0000 0000  nchronizerc.....
+000021f0: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
+00002200: 0000 0073 1e00 0000 7c00 6a00 a001 a100  ...s....|.j.....
+00002210: 0100 7c00 6a00 a002 7c00 6a00 6a03 a101  ..|.j...|.j.j...
+00002220: 0100 6400 5300 7229 0000 0029 0472 4b00  ..d.S.r)...).rK.
+00002230: 0000 7273 0000 005a 0e73 6574 5f73 7472  ..rs...Z.set_str
+00002240: 6561 6d5f 6670 7372 7500 0000 722c 0000  eam_fpsru...r,..
+00002250: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
+00002260: da14 756e 7061 7573 655f 7379 6e63 6872  ..unpause_synchr
+00002270: 6f6e 697a 6572 4901 0000 7304 0000 000a  onizerI...s.....
+00002280: 0114 017a 1c53 6573 7369 6f6e 2e75 6e70  ...z.Session.unp
+00002290: 6175 7365 5f73 796e 6368 726f 6e69 7a65  ause_synchronize
+000022a0: 7263 0100 0000 0000 0000 0000 0000 0400  rc..............
+000022b0: 0000 0400 0000 4300 0000 7334 0000 0064  ......C...s4...d
+000022c0: 017d 017c 006a 006a 01a0 02a1 00a0 03a1  .}.|.j.j........
+000022d0: 0044 005d 0d5c 027d 027d 037c 02a0 0464  .D.].\.}.}.|...d
+000022e0: 02a1 0172 177c 0164 0337 007d 0171 0a7c  ...r.|.d.7.}.q.|
+000022f0: 0153 0029 044e 7201 0000 0072 4f00 0000  .S.).Nr....rO...
+00002300: e901 0000 0029 0572 3600 0000 da04 6469  .....).r6.....di
+00002310: 6374 da04 636f 7079 7248 0000 00da 0a73  ct..copyrH.....s
+00002320: 7461 7274 7377 6974 6829 0472 2d00 0000  tartswith).r-...
+00002330: da05 636f 756e 74da 036b 6579 da06 7061  ..count..key..pa
+00002340: 7261 6d73 7225 0000 0072 2500 0000 7226  ramsr%...r%...r&
+00002350: 0000 00da 1b67 6574 5f63 6f6e 6669 6775  .....get_configu
+00002360: 7265 645f 6361 6d65 7261 5f63 6f75 6e74  red_camera_count
+00002370: 4d01 0000 730c 0000 0004 0118 010a 0108  M...s...........
+00002380: 0102 8004 017a 2353 6573 7369 6f6e 2e67  .....z#Session.g
+00002390: 6574 5f63 6f6e 6669 6775 7265 645f 6361  et_configured_ca
+000023a0: 6d65 7261 5f63 6f75 6e74 6301 0000 0000  mera_countc.....
+000023b0: 0000 0000 0000 0005 0000 0008 0000 0003  ................
+000023c0: 0000 0073 8c00 0000 8700 6601 6401 6402  ...s......f.d.d.
+000023d0: 8408 7d01 7400 8300 8f1e 7d02 7401 6403  ..}.t.....}.t.d.
+000023e0: 7402 8302 4400 5d10 7d03 7c03 8800 6a03  t...D.].}.|...j.
+000023f0: a004 a100 7600 7219 710f 7c02 a005 7c01  ....v.r.q.|...|.
+00002400: 7c03 a102 0100 710f 5700 6404 0400 0400  |.....q.W.d.....
+00002410: 8303 0100 6e08 3100 732a 7701 0100 0100  ....n.1.s*w.....
+00002420: 0100 5900 0100 8800 6a06 6a07 a008 a100  ..Y.....j.j.....
+00002430: a004 a100 4400 5d0c 7d04 7c04 a009 6405  ....D.].}.|...d.
+00002440: a101 7243 8800 6a06 6a07 7c04 3d00 7137  ..rC..j.j.|.=.q7
+00002450: 6404 5300 2906 7aa3 0a20 2020 2020 2020  d.S.).z..       
+00002460: 2043 616c 6c65 6420 6279 206c 6f61 645f   Called by load_
+00002470: 7374 7265 616d 7320 696e 2074 6865 2065  streams in the e
+00002480: 7665 6e74 2074 6861 7420 6e6f 2063 616d  vent that no cam
+00002490: 6572 6173 2061 7265 2072 6574 7572 6e65  eras are returne
+000024a0: 6420 6279 2074 6865 2063 6f6e 6669 6775  d by the configu
+000024b0: 7261 746f 722e 2e2e 0a20 2020 2020 2020  rator....       
+000024c0: 2057 696c 6c20 706f 7075 6c61 7465 2073   Will populate s
+000024d0: 656c 662e 6361 6d65 7261 7320 7573 696e  elf.cameras usin
+000024e0: 6720 6d75 6c74 6970 6c65 2074 6872 6561  g multiple threa
+000024f0: 6473 0a20 2020 2020 2020 2063 0100 0000  ds.        c....
+00002500: 0000 0000 0000 0000 0200 0000 0700 0000  ................
+00002510: 1300 0000 738c 0000 007a 3774 00a0 0164  ....s....z7t...d
+00002520: 017c 009b 009d 02a1 0101 0074 027c 0083  .|.........t.|..
+00002530: 017d 0174 00a0 0164 027c 009b 009d 02a1  .}.t...d.|......
+00002540: 0101 007c 0188 006a 037c 003c 0088 006a  ...|...j.|.<...j
+00002550: 04a0 057c 01a1 0101 0074 00a0 0164 037c  ...|.....t...d.|
+00002560: 009b 0064 049d 03a1 0101 0074 067c 0174  ...d.......t.|.t
+00002570: 0788 006a 0883 0164 058d 0288 006a 097c  ...j...d.....j.|
+00002580: 003c 0057 0064 0053 0001 0001 0001 0074  .<.W.d.S.......t
+00002590: 00a0 0164 067c 009b 009d 02a1 0101 0059  ...d.|.........Y
+000025a0: 0064 0053 0029 074e 7a0c 5472 7969 6e67  .d.S.).Nz.Trying
+000025b0: 2070 6f72 7420 7a10 5375 6363 6573 7320   port z.Success 
+000025c0: 6174 2070 6f72 7420 7a17 4c6f 6164 696e  at port z.Loadin
+000025d0: 6720 7374 7265 616d 2061 7420 706f 7274  g stream at port
+000025e0: 207a 2520 7769 7468 2063 6861 7275 636f   z% with charuco
+000025f0: 2074 7261 636b 6572 2066 6f72 2063 616c   tracker for cal
+00002600: 6962 7261 7469 6f6e a901 5a07 7472 6163  ibration..Z.trac
+00002610: 6b65 727a 124e 6f20 6361 6d65 7261 2061  kerz.No camera a
+00002620: 7420 706f 7274 2029 0a72 5e00 0000 725f  t port ).r^...r_
+00002630: 0000 0072 0b00 0000 723b 0000 0072 3600  ...r....r;...r6.
+00002640: 0000 5a0b 7361 7665 5f63 616d 6572 6172  ..Z.save_camerar
+00002650: 1600 0000 7209 0000 0072 4500 0000 723c  ....r....rE...r<
+00002660: 0000 0029 0272 4d00 0000 724f 0000 0072  ...).rM...rO...r
+00002670: 2c00 0000 7225 0000 0072 2600 0000 da07  ,...r%...r&.....
+00002680: 6164 645f 6361 6d5a 0100 0073 1c00 0000  add_camZ...s....
+00002690: 0201 1001 0801 1001 0a01 0c01 0401 0a01  ................
+000026a0: 04ff 0203 0a01 12ff 0603 1601 7a26 5365  ............z&Se
+000026b0: 7373 696f 6e2e 5f66 696e 645f 6361 6d65  ssion._find_came
+000026c0: 7261 732e 3c6c 6f63 616c 733e 2e61 6464  ras.<locals>.add
+000026d0: 5f63 616d 7201 0000 004e da06 7374 6572  _camr....N..ster
+000026e0: 656f 290a 7204 0000 00da 0572 616e 6765  eo).r......range
+000026f0: da15 4d41 585f 4341 4d45 5241 5f50 4f52  ..MAX_CAMERA_POR
+00002700: 545f 4348 4543 4b72 3b00 0000 da04 6b65  T_CHECKr;.....ke
+00002710: 7973 da06 7375 626d 6974 7236 0000 0072  ys..submitr6...r
+00002720: 7c00 0000 727d 0000 0072 7e00 0000 2905  |...r}...r~...).
+00002730: 722d 0000 0072 8400 0000 da08 6578 6563  r-...r......exec
+00002740: 7574 6f72 da01 6972 8000 0000 7225 0000  utor..ir....r%..
+00002750: 0072 2c00 0000 7226 0000 00da 0d5f 6669  .r,...r&....._fi
+00002760: 6e64 5f63 616d 6572 6173 5401 0000 731a  nd_camerasT...s.
+00002770: 0000 000c 0608 100e 010e 0102 020e 0202  ................
+00002780: fb1c ff14 090a 010a 0102 8004 fe7a 1553  .............z.S
+00002790: 6573 7369 6f6e 2e5f 6669 6e64 5f63 616d  ession._find_cam
+000027a0: 6572 6173 6301 0000 0000 0000 0000 0000  erasc...........
+000027b0: 0003 0000 0005 0000 0043 0000 0073 dc00  .........C...s..
+000027c0: 0000 6401 7c00 5f00 7c00 6a01 a002 a100  ..d.|._.|.j.....
+000027d0: 7c00 5f03 7404 7c00 6a03 8301 6402 6b02  |._.t.|.j...d.k.
+000027e0: 7214 7c00 a005 a100 0100 7c00 6a03 a006  r.|.......|.j...
+000027f0: a100 4400 5d1e 5c02 7d01 7d02 7c01 7c00  ..D.].\.}.}.|.|.
+00002800: 6a07 a008 a100 7600 7225 7119 7409 a00a  j.....v.r%q.t...
+00002810: 6403 7c01 9b00 9d02 a101 0100 740b 7c02  d.|.........t.|.
+00002820: 7c00 6a0c 6404 8d02 7c00 6a07 7c01 3c00  |.j.d...|.j.|.<.
+00002830: 7119 7c00 a00d a100 0100 7c00 a00e a100  q.|.......|.....
+00002840: 0100 740f 7c00 6a10 a008 a100 8301 7c00  ..t.|.j.......|.
+00002850: 5f11 7412 7c00 6a07 8301 7c00 5f13 6401  _.t.|.j...|._.d.
+00002860: 7c00 5f14 6405 7c00 5f00 7409 a00a 6406  |._.d.|._.t...d.
+00002870: a101 0100 7c00 a015 a100 0100 7c00 a016  ....|.......|...
+00002880: a100 0100 7409 a00a 6407 a101 0100 7c00  ....t...d.....|.
+00002890: 6a17 6a18 a019 a100 0100 6408 5300 2909  j.j.......d.S.).
+000028a0: 7aad 0a20 2020 2020 2020 2043 6f6e 6e65  z..        Conne
+000028b0: 6374 7320 746f 2073 746f 7265 6420 6361  cts to stored ca
+000028c0: 6d65 7261 7320 616e 6420 6372 6561 7465  meras and create
+000028d0: 7320 7374 7265 616d 7320 7769 7468 2070  s streams with p
+000028e0: 726f 7669 6465 6420 7472 6163 6b69 6e67  rovided tracking
+000028f0: 0a20 2020 2020 2020 2042 6563 6175 7365  .        Because
+00002900: 2074 6865 7365 2073 7472 6561 6d73 2061   these streams a
+00002910: 7265 2061 7661 696c 6162 6c65 2c20 7468  re available, th
+00002920: 6520 7379 6e63 6872 6f6e 697a 6572 2063  e synchronizer c
+00002930: 616e 2074 6865 6e20 6265 2069 6e69 7469  an then be initi
+00002940: 616c 697a 6564 0a20 2020 2020 2020 2054  alized.        T
+00002950: 7201 0000 007a 184c 6f61 6469 6e67 2053  r....z.Loading S
+00002960: 7472 6561 6d20 666f 7220 706f 7274 2072  tream for port r
+00002970: 8300 0000 467a 3350 6175 7369 6e67 2073  ....Fz3Pausing s
+00002980: 7472 6561 6d20 746f 6f6c 7320 7369 6e63  tream tools sinc
+00002990: 6520 6465 6661 756c 7420 6c6f 6164 7320  e default loads 
+000029a0: 746f 2063 6861 7275 636f 7a2d 5369 676e  to charucoz-Sign
+000029b0: 616c 6c69 6e67 2073 7563 6365 7373 6675  alling successfu
+000029c0: 6c20 6c6f 6164 696e 6720 6f66 2073 7472  l loading of str
+000029d0: 6561 6d20 746f 6f6c 734e 291a 723d 0000  eam toolsN).r=..
+000029e0: 0072 3600 0000 5a0b 6765 745f 6361 6d65  .r6...Z.get_came
+000029f0: 7261 7372 3b00 0000 7252 0000 0072 8c00  rasr;...rR...r..
+00002a00: 0000 7248 0000 0072 3c00 0000 7288 0000  ..rH...r<...r...
+00002a10: 0072 5e00 0000 725f 0000 0072 1600 0000  .r^...r_...r....
+00002a20: 7246 0000 00da 135f 6164 6a75 7374 5f72  rF....._adjust_r
+00002a30: 6573 6f6c 7574 696f 6e73 da15 5f6c 6f61  esolutions.._loa
+00002a40: 645f 6d6f 6e6f 6361 6c69 6272 6174 6f72  d_monocalibrator
+00002a50: 73da 036d 696e 723f 0000 0072 4000 0000  s..minr?...r@...
+00002a60: 720c 0000 0072 4b00 0000 723e 0000 0072  r....rK...r>...r
+00002a70: 6e00 0000 7279 0000 0072 3700 0000 7230  n...ry...r7...r0
+00002a80: 0000 0072 4c00 0000 a903 722d 0000 0072  ...rL.....r-...r
+00002a90: 4d00 0000 724f 0000 0072 2500 0000 7225  M...rO...r%...r%
+00002aa0: 0000 0072 2600 0000 726f 0000 0077 0100  ...r&...ro...w..
+00002ab0: 0073 2c00 0000 0605 0c02 0e02 0801 1202  .s,.............
+00002ac0: 0e01 0201 1002 1601 0802 0801 1003 0202  ................
+00002ad0: 0401 06ff 0605 0601 0a02 0801 0801 0a02  ................
+00002ae0: 1001 7a19 5365 7373 696f 6e2e 6c6f 6164  ..z.Session.load
+00002af0: 5f73 7472 6561 6d5f 746f 6f6c 7363 0100  _stream_toolsc..
+00002b00: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00002b10: 0000 4300 0000 735e 0000 007c 006a 00a0  ..C...s^...|.j..
+00002b20: 01a1 0044 005d 275c 027d 017d 027c 017c  ...D.]'\.}.}.|.|
+00002b30: 006a 02a0 03a1 0076 0072 1a74 04a0 0564  .j.....v.r.t...d
+00002b40: 017c 019b 0064 029d 03a1 0101 0071 0574  .|...d.......q.t
+00002b50: 04a0 0564 037c 019b 009d 02a1 0101 0074  ...d.|.........t
+00002b60: 067c 006a 077c 0119 0083 017c 006a 027c  .|.j.|.....|.j.|
+00002b70: 013c 0071 0564 0053 0029 044e 7a2f 536b  .<.q.d.S.).Nz/Sk
+00002b80: 6970 7069 6e67 206f 7665 7220 6d6f 6e6f  ipping over mono
+00002b90: 6361 6c69 6272 6174 6f72 2063 7265 6174  calibrator creat
+00002ba0: 696f 6e20 666f 7220 706f 7274 207a 1b20  ion for port z. 
+00002bb0: 6265 6361 7573 6520 6974 2061 6c72 6561  because it alrea
+00002bc0: 6479 2065 7869 7374 732e 7a20 4c6f 6164  dy exists.z Load
+00002bd0: 696e 6720 4d6f 6e6f 6361 6c69 6272 6174  ing Monocalibrat
+00002be0: 6f72 2066 6f72 2070 6f72 7420 2908 723b  or for port ).r;
+00002bf0: 0000 0072 4800 0000 723f 0000 0072 8800  ...rH...r?...r..
+00002c00: 0000 725e 0000 0072 5f00 0000 720a 0000  ..r^...r_...r...
+00002c10: 0072 3c00 0000 7290 0000 0072 2500 0000  .r<...r....r%...
+00002c20: 7225 0000 0072 2600 0000 728e 0000 009f  r%...r&...r.....
+00002c30: 0100 0073 1200 0000 1201 0e01 0401 0a01  ...s............
+00002c40: 04ff 0203 1002 1601 04f8 7a1d 5365 7373  ..........z.Sess
+00002c50: 696f 6e2e 5f6c 6f61 645f 6d6f 6e6f 6361  ion._load_monoca
+00002c60: 6c69 6272 6174 6f72 734e da0b 6163 7469  libratorsN..acti
+00002c70: 7665 5f70 6f72 7463 0200 0000 0000 0000  ve_portc........
+00002c80: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
+00002c90: 7346 0000 007c 0164 0175 0172 0f74 00a0  sF...|.d.u.r.t..
+00002ca0: 0164 027c 019b 009d 02a1 0101 007c 017c  .d.|.........|.|
+00002cb0: 005f 0274 00a0 0164 037c 006a 029b 0064  ._.t...d.|.j...d
+00002cc0: 049d 03a1 0101 007c 006a 037c 006a 0219  .......|.j.|.j..
+00002cd0: 00a0 04a1 0001 0064 0153 0029 057a 7e0a  .......d.S.).z~.
+00002ce0: 2020 2020 2020 2020 5573 6564 2074 6f20          Used to 
+00002cf0: 6d61 6b65 2073 7572 6520 7468 6174 206f  make sure that o
+00002d00: 6e6c 7920 7468 6520 6163 7469 7665 2063  nly the active c
+00002d10: 616d 6572 6120 7461 6220 6973 2072 6561  amera tab is rea
+00002d20: 6469 6e67 2066 7261 6d65 7320 6475 7269  ding frames duri
+00002d30: 6e67 2074 6865 2069 6e74 7269 6e73 6963  ng the intrinsic
+00002d40: 2063 616c 6962 7261 7469 6f6e 2070 726f   calibration pro
+00002d50: 6365 7373 0a20 2020 2020 2020 204e 7a29  cess.        Nz)
+00002d60: 5365 7474 696e 6720 7365 7373 696f 6e20  Setting session 
+00002d70: 6163 7469 7665 206d 6f6e 6f63 616c 6962  active monocalib
+00002d80: 7261 746f 7220 746f 207a 1a41 6374 6976  rator to z.Activ
+00002d90: 6174 6520 7472 6163 6b69 6e67 206f 6e20  ate tracking on 
+00002da0: 706f 7274 207a 1620 616e 6420 6465 6163  port z. and deac
+00002db0: 7469 7661 7465 206f 7468 6572 7329 0572  tivate others).r
+00002dc0: 5e00 0000 725f 0000 0072 4000 0000 723f  ^...r_...r@...r?
+00002dd0: 0000 005a 1373 7562 7363 7269 6265 5f74  ...Z.subscribe_t
+00002de0: 6f5f 7374 7265 616d 2902 722d 0000 0072  o_stream).r-...r
+00002df0: 9100 0000 7225 0000 0072 2500 0000 7226  ....r%...r%...r&
+00002e00: 0000 0072 7200 0000 aa01 0000 730e 0000  ...rr.......s...
+00002e10: 0008 0510 0106 0104 010c 0104 ff14 037a  ...............z
+00002e20: 1f53 6573 7369 6f6e 2e61 6374 6976 6174  .Session.activat
+00002e30: 655f 6d6f 6e6f 6361 6c69 6272 6174 6f72  e_monocalibrator
+00002e40: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
+00002e50: 0003 0000 0043 0000 0073 2a00 0000 7400  .....C...s*...t.
+00002e60: a001 6401 a101 0100 7c00 6a02 a003 a100  ..d.....|.j.....
+00002e70: 4400 5d08 5c02 7d01 7d02 7c02 a004 a100  D.].\.}.}.|.....
+00002e80: 0100 710a 6402 5300 2903 7a8b 0a20 2020  ..q.d.S.).z..   
+00002e90: 2020 2020 2075 7365 6420 7768 656e 206e       used when n
+00002ea0: 6f74 2061 6374 6976 656c 7920 6f6e 2074  ot actively on t
+00002eb0: 6865 2063 616d 6572 6120 6361 6c69 6272  he camera calibr
+00002ec0: 6174 696f 6e20 7461 620a 2020 2020 2020  ation tab.      
+00002ed0: 2020 6f72 2077 6865 6e20 7369 6c65 6e63    or when silenc
+00002ee0: 696e 6720 616c 6c20 696e 2070 7265 7061  ing all in prepa
+00002ef0: 7261 7469 6f6e 2066 6f72 2061 6374 6976  ration for activ
+00002f00: 6174 696e 6720 6f6e 6c79 206f 6e65 0a20  ating only one. 
+00002f10: 2020 2020 2020 207a 2550 6175 7369 6e67         z%Pausing
+00002f20: 2061 6c6c 206d 6f6e 6f63 616c 6962 7261   all monocalibra
+00002f30: 746f 7220 6c6f 6f70 696e 672e 2e2e 4e29  tor looping...N)
+00002f40: 0572 5e00 0000 725f 0000 0072 3f00 0000  .r^...r_...r?...
+00002f50: 7248 0000 005a 1575 6e73 7562 7363 7269  rH...Z.unsubscri
+00002f60: 6265 5f74 6f5f 7374 7265 616d 2903 722d  be_to_stream).r-
+00002f70: 0000 0072 4d00 0000 7250 0000 0072 2500  ...rM...rP...r%.
+00002f80: 0000 7225 0000 0072 2600 0000 726e 0000  ..r%...r&...rn..
+00002f90: 00b7 0100 0073 0800 0000 0a05 1201 0a01  .....s..........
+00002fa0: 04ff 7a21 5365 7373 696f 6e2e 7061 7573  ..z!Session.paus
+00002fb0: 655f 616c 6c5f 6d6f 6e6f 6361 6c69 6272  e_all_monocalibr
+00002fc0: 6174 6f72 7346 da15 6465 7374 696e 6174  atorsF..destinat
+00002fd0: 696f 6e5f 6469 7265 6374 6f72 79da 1373  ion_directory..s
+00002fe0: 746f 7265 5f70 6f69 6e74 5f68 6973 746f  tore_point_histo
+00002ff0: 7279 6303 0000 0000 0000 0000 0000 0003  ryc.............
+00003000: 0000 0004 0000 0043 0000 0073 3e00 0000  .......C...s>...
+00003010: 7400 a001 6401 a101 0100 7c01 6a02 6402  t...d.....|.j.d.
+00003020: 6402 6403 8d02 0100 7403 7c00 6a04 8301  d.d.....t.|.j...
+00003030: 7c00 5f05 7c00 6a05 6a06 7c01 7c02 6404  |._.|.j.j.|.|.d.
+00003040: 8d02 0100 6402 7c00 5f07 6400 5300 2905  ....d.|._.d.S.).
+00003050: 4e7a 1749 6e69 7469 6174 696e 6720 7265  Nz.Initiating re
+00003060: 636f 7264 696e 672e 2e2e 5429 02da 0770  cording...T)...p
+00003070: 6172 656e 7473 da08 6578 6973 745f 6f6b  arents..exist_ok
+00003080: 2901 7293 0000 0029 0872 5e00 0000 725f  ).r....).r^...r_
+00003090: 0000 00da 056d 6b64 6972 7217 0000 0072  .....mkdirr....r
+000030a0: 4b00 0000 da0e 7669 6465 6f5f 7265 636f  K.....video_reco
+000030b0: 7264 6572 da0f 7374 6172 745f 7265 636f  rder..start_reco
+000030c0: 7264 696e 6772 4400 0000 2903 722d 0000  rdingrD...).r-..
+000030d0: 0072 9200 0000 7293 0000 0072 2500 0000  .r....r....r%...
+000030e0: 7225 0000 0072 2600 0000 7298 0000 00c0  r%...r&...r.....
+000030f0: 0100 0073 0e00 0000 0a03 0e01 0c02 0601  ...s............
+00003100: 0401 06ff 0a03 7a17 5365 7373 696f 6e2e  ......z.Session.
+00003110: 7374 6172 745f 7265 636f 7264 696e 6763  start_recordingc
+00003120: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00003130: 0300 0000 4300 0000 736e 0000 0074 00a0  ....C...sn...t..
+00003140: 0164 01a1 0101 007c 006a 02a0 03a1 0001  .d.....|.j......
+00003150: 007c 006a 026a 0472 1b74 00a0 0164 02a1  .|.j.j.r.t...d..
+00003160: 0101 0074 0564 0383 0101 007c 006a 026a  ...t.d.....|.j.j
+00003170: 0473 0e64 047c 005f 0674 00a0 0164 05a1  .s.d.|._.t...d..
+00003180: 0101 007c 006a 076a 08a0 09a1 0001 007c  ...|.j.j.......|
+00003190: 00a0 0aa1 0072 357c 006a 076a 0ba0 09a1  .....r5|.j.j....
+000031a0: 0001 0064 0053 0064 0053 0029 064e 7a15  ...d.S.d.S.).Nz.
+000031b0: 5374 6f70 7069 6e67 2072 6563 6f72 6469  Stopping recordi
+000031c0: 6e67 2e2e 2e7a 2e57 6169 7469 6e67 2066  ng...z.Waiting f
+000031d0: 6f72 2076 6964 656f 2072 6563 6f72 6465  or video recorde
+000031e0: 7220 746f 2073 6176 6520 6f75 7420 6461  r to save out da
+000031f0: 7461 2e2e 2e67 0000 0000 0000 e03f 467a  ta...g.......?Fz
+00003200: 3d52 6563 6f72 6469 6e67 206f 6620 6672  =Recording of fr
+00003210: 616d 6573 2069 7320 636f 6d70 6c65 7465  ames is complete
+00003220: 2e2e 2e73 6967 6e61 6c6c 696e 6720 6368  ...signalling ch
+00003230: 616e 6765 2069 6e20 7374 6174 7573 290c  ange in status).
+00003240: 725e 0000 0072 5f00 0000 7297 0000 00da  r^...r_...r.....
+00003250: 0e73 746f 705f 7265 636f 7264 696e 675a  .stop_recordingZ
+00003260: 0972 6563 6f72 6469 6e67 7206 0000 0072  .recordingr....r
+00003270: 4400 0000 7237 0000 0072 3300 0000 724c  D...r7...r3...rL
+00003280: 0000 0072 6b00 0000 7232 0000 0072 2c00  ...rk...r2...r,.
+00003290: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
+000032a0: 0072 9900 0000 cc01 0000 7318 0000 000a  .r........s.....
+000032b0: 010a 0108 010a 0108 0108 fe06 040a 020c  ................
+000032c0: 0108 0210 0104 ff7a 1653 6573 7369 6f6e  .......z.Session
+000032d0: 2e73 746f 705f 7265 636f 7264 696e 6763  .stop_recordingc
+000032e0: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+000032f0: 0800 0000 0300 0000 7354 0000 0087 0066  ........sT.....f
+00003300: 0164 0164 0284 087d 0174 0083 008f 177d  .d.d...}.t.....}
+00003310: 0288 006a 01a0 02a1 0044 005d 087d 037c  ...j.....D.].}.|
+00003320: 02a0 037c 017c 03a1 0201 0071 0f57 0064  ...|.|.....q.W.d
+00003330: 0304 0004 0083 0301 0064 0353 0031 0073  .........d.S.1.s
+00003340: 2377 0101 0001 0001 0059 0001 0064 0353  #w.......Y...d.S
+00003350: 0029 047a 8243 6861 6e67 6573 2074 6865  .).z.Changes the
+00003360: 2063 616d 6572 6120 7265 736f 6c75 7469   camera resoluti
+00003370: 6f6e 2074 6f20 7468 6520 7661 6c75 6520  on to the value 
+00003380: 696e 2074 6865 2063 6f6e 6669 6775 7261  in the configura
+00003390: 7469 6f6e 2c20 6173 0a20 2020 2020 2020  tion, as.       
+000033a0: 206c 6f67 2061 7320 6974 2069 7320 6e6f   log as it is no
+000033b0: 7420 636f 6e66 6967 7572 6564 2066 6f72  t configured for
+000033c0: 2074 6865 2064 6566 6175 6c74 2072 6573   the default res
+000033d0: 6f6c 7574 696f 6e63 0100 0000 0000 0000  olutionc........
+000033e0: 0000 0000 0400 0000 0a00 0000 1300 0000  ................
+000033f0: 73b6 0000 0088 006a 007c 0019 007d 0188  s......j.|...}..
+00003400: 006a 016a 0264 017c 009b 009d 0219 0064  .j.j.d.|.......d
+00003410: 0219 007d 0288 006a 037c 0019 006a 047d  ...}...j.|...j.}
+00003420: 037c 0264 0319 007c 0364 0319 006b 0373  .|.d...|.d...k.s
+00003430: 267c 0264 0419 007c 0364 0419 006b 0372  &|.d...|.d...k.r
+00003440: 5974 05a0 0664 057c 009b 0064 067c 0364  Yt...d.|...d.|.d
+00003450: 0364 0785 0219 009b 0064 087c 0264 0364  .d.......d.|.d.d
+00003460: 0785 0219 009b 009d 06a1 0101 007c 01a0  .............|..
+00003470: 077c 02a1 0101 0074 05a0 0664 097c 009b  .|.....t...d.|..
+00003480: 0064 067c 0364 0364 0785 0219 009b 0064  .d.|.d.d.......d
+00003490: 087c 0264 0364 0785 0219 009b 009d 06a1  .|.d.d..........
+000034a0: 0101 0064 0053 0064 0053 0029 0a4e 5a04  ...d.S.d.S.).NZ.
+000034b0: 6361 6d5f da04 7369 7a65 7201 0000 0072  cam_..sizer....r
+000034c0: 7b00 0000 7a27 4265 6769 6e6e 696e 6720  {...z'Beginning 
+000034d0: 746f 2063 6861 6e67 6520 7265 736f 6c75  to change resolu
+000034e0: 7469 6f6e 2061 7420 706f 7274 207a 0620  tion at port z. 
+000034f0: 6672 6f6d 2072 5b00 0000 7a04 2074 6f20  from r[...z. to 
+00003500: 7a27 436f 6d70 6c65 7465 6420 6368 616e  z'Completed chan
+00003510: 6765 206f 6620 7265 736f 6c75 7469 6f6e  ge of resolution
+00003520: 2061 7420 706f 7274 2029 0872 3c00 0000   at port ).r<...
+00003530: 7236 0000 0072 7c00 0000 723b 0000 005a  r6...r|...r;...Z
+00003540: 1264 6566 6175 6c74 5f72 6573 6f6c 7574  .default_resolut
+00003550: 696f 6e72 5e00 0000 725f 0000 005a 1163  ionr^...r_...Z.c
+00003560: 6861 6e67 655f 7265 736f 6c75 7469 6f6e  hange_resolution
+00003570: 2904 724d 0000 0072 4e00 0000 729a 0000  ).rM...rN...r...
+00003580: 005a 0c64 6566 6175 6c74 5f73 697a 6572  .Z.default_sizer
+00003590: 2c00 0000 7225 0000 0072 2600 0000 da11  ,...r%...r&.....
+000035a0: 6164 6a75 7374 5f72 6573 5f77 6f72 6b65  adjust_res_worke
+000035b0: 72df 0100 0073 1800 0000 0a01 1601 0c01  r....s..........
+000035c0: 2002 0401 2401 04ff 0a03 0401 2401 08ff   ...$.......$...
+000035d0: 04fb 7a36 5365 7373 696f 6e2e 5f61 646a  ..z6Session._adj
+000035e0: 7573 745f 7265 736f 6c75 7469 6f6e 732e  ust_resolutions.
+000035f0: 3c6c 6f63 616c 733e 2e61 646a 7573 745f  <locals>.adjust_
+00003600: 7265 735f 776f 726b 6572 4e29 0472 0400  res_workerN).r..
+00003610: 0000 723b 0000 0072 8800 0000 7289 0000  ..r;...r....r...
+00003620: 0029 0472 2d00 0000 729b 0000 0072 8a00  .).r-...r....r..
+00003630: 0000 724d 0000 0072 2500 0000 722c 0000  ..rM...r%...r,..
+00003640: 0072 2600 0000 728d 0000 00db 0100 0073  .r&...r........s
+00003650: 0c00 0000 0c04 080e 0e01 0e01 02ff 22ff  ..............".
+00003660: 7a1b 5365 7373 696f 6e2e 5f61 646a 7573  z.Session._adjus
+00003670: 745f 7265 736f 6c75 7469 6f6e 7363 0100  t_resolutionsc..
+00003680: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00003690: 0000 4300 0000 737a 0000 007c 006a 00a0  ..C...sz...|.j..
+000036a0: 01a1 007c 005f 027c 006a 00a0 03a1 007c  ...|._.|.j.....|
+000036b0: 005f 0474 057c 006a 047c 006a 0283 027c  ._.t.|.j.|.j...|
+000036c0: 005f 067c 006a 006a 0764 0119 0064 0219  ._.|.j.j.d...d..
+000036d0: 007c 006a 065f 0864 037c 006a 006a 0764  .|.j._.d.|.j.j.d
+000036e0: 0119 00a0 09a1 0076 0072 327c 006a 006a  .......v.r2|.j.j
+000036f0: 0764 0119 0064 0319 007c 006a 065f 0a74  .d...d...|.j._.t
+00003700: 0b7c 006a 067c 006a 0c64 048d 027c 005f  .|.j.|.j.d...|._
+00003710: 0d64 0553 0029 067a f30a 2020 2020 2020  .d.S.).z..      
+00003720: 2020 466f 6c6c 6f77 696e 6720 6361 7074    Following capt
+00003730: 7572 6520 766f 6c75 6d65 206f 7074 696d  ure volume optim
+00003740: 697a 6174 696f 6e20 7669 6120 6275 6e64  ization via bund
+00003750: 6c65 2061 646a 7573 746d 656e 742c 206f  le adjustment, o
+00003760: 7220 616c 7465 7261 7469 6f6e 0a20 2020  r alteration.   
+00003770: 2020 2020 2076 6961 2061 2074 7261 6e73       via a trans
+00003780: 666f 726d 206f 6620 7468 6520 6f72 6967  form of the orig
+00003790: 696e 2c20 7468 6520 656e 7469 7265 2063  in, the entire c
+000037a0: 6170 7475 7265 2076 6f6c 756d 6520 6361  apture volume ca
+000037b0: 6e20 6265 2072 656c 6f61 6465 640a 2020  n be reloaded.  
+000037c0: 2020 2020 2020 6672 6f6d 2074 6865 2063        from the c
+000037d0: 6f6e 6669 6720 6461 7461 2077 6974 686f  onfig data witho
+000037e0: 7574 206e 6565 6469 6e67 2074 6f20 676f  ut needing to go
+000037f0: 2074 6872 6f75 6768 2074 6865 2073 7465   through the ste
+00003800: 7073 0a0a 2020 2020 2020 2020 da0e 6361  ps..        ..ca
+00003810: 7074 7572 655f 766f 6c75 6d65 da05 7374  pture_volume..st
+00003820: 6167 65da 116f 7269 6769 6e5f 7379 6e63  age..origin_sync
+00003830: 5f69 6e64 6578 2901 7245 0000 004e 290e  _index).rE...N).
+00003840: 7236 0000 0072 1400 0000 da0f 706f 696e  r6...r......poin
+00003850: 745f 6573 7469 6d61 7465 7372 5600 0000  t_estimatesrV...
+00003860: 7257 0000 0072 1100 0000 729c 0000 0072  rW...r....r....r
+00003870: 7c00 0000 729d 0000 0072 8800 0000 729e  |...r....r....r.
+00003880: 0000 0072 1200 0000 7245 0000 00da 1271  ...r....rE.....q
+00003890: 7561 6c69 7479 5f63 6f6e 7472 6f6c 6c65  uality_controlle
+000038a0: 7272 2c00 0000 7225 0000 0072 2500 0000  rr,...r%...r%...
+000038b0: 7226 0000 00da 1d6c 6f61 645f 6573 7469  r&.....load_esti
+000038c0: 6d61 7465 645f 6361 7074 7572 655f 766f  mated_capture_vo
+000038d0: 6c75 6d65 f101 0000 7316 0000 000c 070c  lume....s.......
+000038e0: 0110 0114 0214 010a 0102 0108 ff02 0508  ................
+000038f0: 010c ff7a 2553 6573 7369 6f6e 2e6c 6f61  ...z%Session.loa
+00003900: 645f 6573 7469 6d61 7465 645f 6361 7074  d_estimated_capt
+00003910: 7572 655f 766f 6c75 6d65 6301 0000 0000  ure_volumec.....
+00003920: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00003930: 0000 0073 a600 0000 7400 7c00 6a01 6a02  ...s....t.|.j.j.
+00003940: 7c00 6a03 8302 7d01 7c01 6a04 6401 6402  |.j...}.|.j.d.d.
+00003950: 8d01 0100 7405 7c00 6a01 6a02 8301 a006  ....t.|.j.j.....
+00003960: a100 7c00 5f07 7408 7c00 6a07 7c00 6a03  ..|._.t.|.j.|.j.
+00003970: 8302 7c00 5f09 740a 7c00 6a07 7c00 6a09  ..|._.t.|.j.|.j.
+00003980: 8302 7c00 5f0b 7c00 6a0b a00c a100 0100  ..|._.|.j.......
+00003990: 740d 7c00 6a0b 7c00 6a0e 8302 7c00 5f0f  t.|.j.|.j...|._.
+000039a0: 7410 a011 6403 7412 6404 1400 9b00 6405  t...d.t.d.....d.
+000039b0: 9d03 a101 0100 7c00 6a0f a013 7412 a101  ......|.j...t...
+000039c0: 0100 7c00 6a0b a00c a100 0100 7c00 6a01  ..|.j.......|.j.
+000039d0: a014 7c00 6a0b a101 0100 6406 5300 2907  ..|.j.....d.S.).
+000039e0: 7ad7 0a20 2020 2020 2020 2054 6869 7320  z..        This 
+000039f0: 6973 2077 6865 7265 2074 6865 2063 616d  is where the cam
+00003a00: 6572 6120 6172 7261 7920 3620 446f 4620  era array 6 DoF 
+00003a10: 6973 2073 6574 2e20 4d61 6e79 2c20 6d61  is set. Many, ma
+00003a20: 6e79 2074 6869 6e67 7320 6172 6520 6861  ny things are ha
+00003a30: 7070 656e 696e 670a 2020 2020 2020 2020  ppening.        
+00003a40: 6865 7265 2c20 6275 7420 7468 6579 2061  here, but they a
+00003a50: 7265 2061 6c6c 206e 6563 6573 7361 7279  re all necessary
+00003a60: 2073 7465 7073 206f 6620 7468 6520 7072   steps of the pr
+00003a70: 6f63 6573 7320 736f 2049 2064 6964 6e27  ocess so I didn'
+00003a80: 7420 7761 6e74 2074 6f0a 2020 2020 2020  t want to.      
+00003a90: 2020 7472 7920 746f 2065 6e63 6170 7375    try to encapsu
+00003aa0: 6c61 7465 2061 6e79 2066 7572 7468 6572  late any further
+00003ab0: 0a20 2020 2020 2020 2072 1800 0000 2901  .        r....).
+00003ac0: 5a0e 626f 6172 6473 5f73 616d 706c 6564  Z.boards_sampled
+00003ad0: 7a1b 5265 6d6f 7669 6e67 2074 6865 2077  z.Removing the w
+00003ae0: 6f72 7374 2066 6974 7469 6e67 20e9 6400  orst fitting .d.
+00003af0: 0000 7a21 2070 6572 6365 6e74 206f 6620  ..z! percent of 
+00003b00: 706f 696e 7473 2066 726f 6d20 7468 6520  points from the 
+00003b10: 6d6f 6465 6c4e 2915 720f 0000 0072 3600  modelN).r....r6.
+00003b20: 0000 5a09 746f 6d6c 5f70 6174 6872 3a00  ..Z.toml_pathr:.
+00003b30: 0000 5a14 7374 6572 656f 5f63 616c 6962  ..Z.stereo_calib
+00003b40: 7261 7465 5f61 6c6c 720d 0000 005a 1567  rate_allr....Z.g
+00003b50: 6574 5f62 6573 745f 6361 6d65 7261 5f61  et_best_camera_a
+00003b60: 7272 6179 7257 0000 0072 1400 0000 729f  rrayrW...r....r.
+00003b70: 0000 0072 1100 0000 729c 0000 00da 086f  ...r....r......o
+00003b80: 7074 696d 697a 6572 1200 0000 7245 0000  ptimizer....rE..
+00003b90: 0072 a000 0000 725e 0000 0072 5f00 0000  .r....r^...r_...
+00003ba0: da11 4649 4c54 4552 4544 5f46 5241 4354  ..FILTERED_FRACT
+00003bb0: 494f 4e5a 1666 696c 7465 725f 706f 696e  IONZ.filter_poin
+00003bc0: 745f 6573 7469 6d61 7465 735a 1373 6176  t_estimatesZ.sav
+00003bd0: 655f 6361 7074 7572 655f 766f 6c75 6d65  e_capture_volume
+00003be0: 2902 722d 0000 005a 1073 7465 7265 6f63  ).r-...Z.stereoc
+00003bf0: 616c 6962 7261 746f 7272 2500 0000 7225  alibratorr%...r%
+00003c00: 0000 0072 2600 0000 da13 6573 7469 6d61  ...r&.....estima
+00003c10: 7465 5f65 7874 7269 6e73 6963 7307 0200  te_extrinsics...
+00003c20: 0073 2a00 0000 0206 0a01 04ff 0c03 0202  .s*.............
+00003c30: 0601 02ff 0402 04fe 0204 0801 06ff 1004  ................
+00003c40: 0a01 1002 0402 0e01 04ff 0c03 0a01 1202  ................
+00003c50: 7a1b 5365 7373 696f 6e2e 6573 7469 6d61  z.Session.estima
+00003c60: 7465 5f65 7874 7269 6e73 6963 7372 2900  te_extrinsicsr).
+00003c70: 0000 2901 4629 2272 1b00 0000 721c 0000  ..).F)"r....r...
+00003c80: 0072 1d00 0000 7215 0000 0072 2b00 0000  .r....r....r+...
+00003c90: 7251 0000 0072 5400 0000 725a 0000 0072  rQ...rT...rZ...r
+00003ca0: 6100 0000 7264 0000 0072 6b00 0000 7219  a...rd...rk...r.
+00003cb0: 0000 0072 7400 0000 da03 696e 7472 7600  ...rt.....intrv.
+00003cc0: 0000 7277 0000 0072 6c00 0000 da04 626f  ..rw...rl.....bo
+00003cd0: 6f6c 7271 0000 0072 7000 0000 7279 0000  olrq...rp...ry..
+00003ce0: 0072 7a00 0000 7282 0000 0072 8c00 0000  .rz...r....r....
+00003cf0: 726f 0000 0072 8e00 0000 7272 0000 0072  ro...r....rr...r
+00003d00: 6e00 0000 7205 0000 0072 9800 0000 7299  n...r....r....r.
+00003d10: 0000 0072 8d00 0000 72a1 0000 0072 a500  ...r....r....r..
+00003d20: 0000 7225 0000 0072 2500 0000 7225 0000  ..r%...r%...r%..
+00003d30: 0072 2600 0000 7235 0000 003b 0000 0073  .r&...r5...;...s
+00003d40: 4000 0000 0800 0e01 0824 0812 0807 080b  @........$......
+00003d50: 081d 081e 0e10 0e41 0e16 080f 0e06 0804  .......A........
+00003d60: 0806 0804 0804 0807 0823 0828 100b 080d  .........#.(....
+00003d70: 020a 04ff 0201 02ff 0201 0aff 080c 080f  ................
+00003d80: 0816 0c16 7235 0000 0029 35da 0674 7970  ....r5...)5..typ
+00003d90: 696e 67da 0d70 7978 7933 642e 6c6f 6767  ing..pyxy3d.logg
+00003da0: 6572 da06 7079 7879 3364 725e 0000 00da  er..pyxy3dr^....
+00003db0: 0367 6574 721b 0000 00da 0c50 7951 7436  .getr......PyQt6
+00003dc0: 2e51 7443 6f72 6572 0200 0000 7203 0000  .QtCorer....r...
+00003dd0: 005a 1263 6f6e 6375 7272 656e 742e 6675  .Z.concurrent.fu
+00003de0: 7475 7265 7372 0400 0000 da07 7061 7468  turesr......path
+00003df0: 6c69 6272 0500 0000 da04 7469 6d65 7206  libr......timer.
+00003e00: 0000 00da 0465 6e75 6d72 0700 0000 7208  .....enumr....r.
+00003e10: 0000 005a 1f70 7978 7933 642e 7472 6163  ...Z.pyxy3d.trac
+00003e20: 6b65 7273 2e63 6861 7275 636f 5f74 7261  kers.charuco_tra
+00003e30: 636b 6572 7209 0000 005a 2170 7978 7933  ckerr....Z!pyxy3
+00003e40: 642e 6361 6c69 6272 6174 696f 6e2e 6d6f  d.calibration.mo
+00003e50: 6e6f 6361 6c69 6272 6174 6f72 720a 0000  nocalibratorr...
+00003e60: 005a 1570 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
+00003e70: 732e 6361 6d65 7261 720b 0000 00da 1b70  s.camerar......p
+00003e80: 7978 7933 642e 6361 6d65 7261 732e 7379  yxy3d.cameras.sy
+00003e90: 6e63 6872 6f6e 697a 6572 720c 0000 005a  nchronizerr....Z
+00003ea0: 2770 7978 7933 642e 6361 6d65 7261 732e  'pyxy3d.cameras.
+00003eb0: 6361 6d65 7261 5f61 7272 6179 5f69 6e69  camera_array_ini
+00003ec0: 7469 616c 697a 6572 720d 0000 005a 1070  tializerr....Z.p
+00003ed0: 7978 7933 642e 696e 7465 7266 6163 6572  yxy3d.interfacer
+00003ee0: 0e00 0000 5a23 7079 7879 3364 2e63 616c  ....Z#pyxy3d.cal
+00003ef0: 6962 7261 7469 6f6e 2e73 7465 7265 6f63  ibration.stereoc
+00003f00: 616c 6962 7261 746f 7272 0f00 0000 5a31  alibratorr....Z1
+00003f10: 7079 7879 3364 2e63 616c 6962 7261 7469  pyxy3d.calibrati
+00003f20: 6f6e 2e63 6170 7475 7265 5f76 6f6c 756d  on.capture_volum
+00003f30: 652e 706f 696e 745f 6573 7469 6d61 7465  e.point_estimate
+00003f40: 7372 1000 0000 5a30 7079 7879 3364 2e63  sr....Z0pyxy3d.c
+00003f50: 616c 6962 7261 7469 6f6e 2e63 6170 7475  alibration.captu
+00003f60: 7265 5f76 6f6c 756d 652e 6361 7074 7572  re_volume.captur
+00003f70: 655f 766f 6c75 6d65 7211 0000 005a 3470  e_volumer....Z4p
+00003f80: 7978 7933 642e 6361 6c69 6272 6174 696f  yxy3d.calibratio
+00003f90: 6e2e 6361 7074 7572 655f 766f 6c75 6d65  n.capture_volume
+00003fa0: 2e71 7561 6c69 7479 5f63 6f6e 7472 6f6c  .quality_control
+00003fb0: 6c65 7272 1200 0000 5a1b 7079 7879 3364  lerr....Z.pyxy3d
+00003fc0: 2e63 616d 6572 6173 2e63 616d 6572 615f  .cameras.camera_
+00003fd0: 6172 7261 7972 1300 0000 5a46 7079 7879  arrayr....ZFpyxy
+00003fe0: 3364 2e63 616c 6962 7261 7469 6f6e 2e63  3d.calibration.c
+00003ff0: 6170 7475 7265 5f76 6f6c 756d 652e 6865  apture_volume.he
+00004000: 6c70 6572 5f66 756e 6374 696f 6e73 2e67  lper_functions.g
+00004010: 6574 5f70 6f69 6e74 5f65 7374 696d 6174  et_point_estimat
+00004020: 6573 7214 0000 00da 1370 7978 7933 642e  esr......pyxy3d.
+00004030: 636f 6e66 6967 7572 6174 6f72 7215 0000  configuratorr...
+00004040: 005a 1a70 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
+00004050: 732e 6c69 7665 5f73 7472 6561 6d72 1600  s.live_streamr..
+00004060: 0000 da1f 7079 7879 3364 2e72 6563 6f72  ....pyxy3d.recor
+00004070: 6469 6e67 2e76 6964 656f 5f72 6563 6f72  ding.video_recor
+00004080: 6465 7272 1700 0000 7287 0000 0072 a400  derr....r....r..
+00004090: 0000 7219 0000 0072 2700 0000 7235 0000  ..r....r'...r5..
+000040a0: 0072 2500 0000 7225 0000 0072 2500 0000  .r%...r%...r%...
+000040b0: 7226 0000 00da 083c 6d6f 6475 6c65 3e01  r&.....<module>.
+000040c0: 0000 0073 3800 0000 0801 0801 0c02 1002  ...s8...........
+000040d0: 0c01 0c01 0c01 1001 0c02 0c01 0c01 0c01  ................
+000040e0: 0c01 0c01 0c02 0c01 0c01 0c01 0c02 0c01  ................
+000040f0: 0c03 0c01 0c01 0403 0401 1003 100a 120b  ................
```

### Comparing `pyxy3d-0.1.4/pyxy3d/session/session.py` & `pyxy3d-0.1.5/pyxy3d/session/session.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/charuco_tracker.py` & `pyxy3d-0.1.5/pyxy3d/trackers/charuco_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/hand_tracker.py` & `pyxy3d-0.1.5/pyxy3d/trackers/hand_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/helper.py` & `pyxy3d-0.1.5/pyxy3d/trackers/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/holistic_opensim_tracker.py` & `pyxy3d-0.1.5/pyxy3d/trackers/holistic_opensim_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/holistic_tracker.py` & `pyxy3d-0.1.5/pyxy3d/trackers/holistic_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/pose_tracker.py` & `pyxy3d-0.1.5/pyxy3d/trackers/pose_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/trackers/tracker_enum.py` & `pyxy3d-0.1.5/pyxy3d/trackers/tracker_enum.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc` & `pyxy3d-0.1.5/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/array_stereo_triangulator.py` & `pyxy3d-0.1.5/pyxy3d/triangulate/array_stereo_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/stereo_points_builder.py` & `pyxy3d-0.1.5/pyxy3d/triangulate/stereo_points_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/pyxy3d/triangulate/sync_packet_triangulator.py` & `pyxy3d-0.1.5/pyxy3d/triangulate/sync_packet_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.4/README.md` & `pyxy3d-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 
 <div align="center"><img src = "pyxy3d/gui/icons/pyxy_logo.svg" width = "150"></div>
 
 <div align="center">
 
-[Quick Start](#quick-start) | [Key Features](#key-features) | [Limitations](#limitations) | [Known Issues](#known-issues)
-
+[Quick Start](#quick-start) | [Key Features](#key-features) | [Limitations](#limitations)
 </div>
 
 
 ---
 ## About
 
 Pyxy3D (*pixie-3d*) is an open-source **Py**thon package for converting 2D **(x,y)** point data to **3D** estimates. It is intended to serve as the calibration and triangulation workhorse of a low-cost DIY motion capture studio. It's core functionality includes: 
@@ -41,15 +40,15 @@
 ```
 2. Navigate into that directory
 ```powershell
 cd pyxy3d_demo
 ```
 3. Create a virtual environment with [Python 3.10](https://www.python.org/downloads/release/python-3100/) or later:
 ```powershell
-python3.10 -m venv .venv
+C:\Python310\python.exe -m venv .venv
 ```
 4. Activate the environment
 ```powershell
 .\.venv\Scripts\activate
 ```
 
 5. Install Pyxy3D
@@ -87,17 +86,15 @@
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
 - It does not support anything other than standard webcams at the moment 
 - The frame capture backend presents a primary bottleneck that will limit the number of cameras/resolution/frame rates that can be used, which ultimately limits the size and precision of the capture volume.
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
-## Known Issues
-### Seg Faults on Windows 10
-[June 23, 2023] The most recent version of the package on PyPI (0.1.3) has been updated to allow it to run on MacOS 12. This update did not change any code, but did change which versions of the underlying dependencies were configured to install. Segmentation faults during recording emerged after this update and are currently being addressed as a top priority.
+
 
 ## Reporting Issues and Requesting Features
 
 To report a bug or request a feature, please [open an issue](https://github.com/mprib/pyxy3d/issues). Please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
 
 ## General Questions and Conversation
```

### Comparing `pyxy3d-0.1.4/PKG-INFO` & `pyxy3d-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxy3d
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for calibrating standard webcams to enable 3d motion tracking
 License: AGPL-3.0-only
 Author: Mac Prible
 Author-email: prible@gmail.com
 Requires-Python: >=3.10,<3.10.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -23,16 +23,15 @@
 
 
 
 <div align="center"><img src = "pyxy3d/gui/icons/pyxy_logo.svg" width = "150"></div>
 
 <div align="center">
 
-[Quick Start](#quick-start) | [Key Features](#key-features) | [Limitations](#limitations) | [Known Issues](#known-issues)
-
+[Quick Start](#quick-start) | [Key Features](#key-features) | [Limitations](#limitations)
 </div>
 
 
 ---
 ## About
 
 Pyxy3D (*pixie-3d*) is an open-source **Py**thon package for converting 2D **(x,y)** point data to **3D** estimates. It is intended to serve as the calibration and triangulation workhorse of a low-cost DIY motion capture studio. It's core functionality includes: 
@@ -64,15 +63,15 @@
 ```
 2. Navigate into that directory
 ```powershell
 cd pyxy3d_demo
 ```
 3. Create a virtual environment with [Python 3.10](https://www.python.org/downloads/release/python-3100/) or later:
 ```powershell
-python3.10 -m venv .venv
+C:\Python310\python.exe -m venv .venv
 ```
 4. Activate the environment
 ```powershell
 .\.venv\Scripts\activate
 ```
 
 5. Install Pyxy3D
@@ -110,17 +109,15 @@
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
 - It does not support anything other than standard webcams at the moment 
 - The frame capture backend presents a primary bottleneck that will limit the number of cameras/resolution/frame rates that can be used, which ultimately limits the size and precision of the capture volume.
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
-## Known Issues
-### Seg Faults on Windows 10
-[June 23, 2023] The most recent version of the package on PyPI (0.1.3) has been updated to allow it to run on MacOS 12. This update did not change any code, but did change which versions of the underlying dependencies were configured to install. Segmentation faults during recording emerged after this update and are currently being addressed as a top priority.
+
 
 ## Reporting Issues and Requesting Features
 
 To report a bug or request a feature, please [open an issue](https://github.com/mprib/pyxy3d/issues). Please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
 
 ## General Questions and Conversation
```

