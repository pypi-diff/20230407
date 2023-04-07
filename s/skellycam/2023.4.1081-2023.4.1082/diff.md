# Comparing `tmp/skellycam-2023.4.1081.tar.gz` & `tmp/skellycam-2023.4.1082.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skellycam-2023.4.1081.tar", last modified: Fri Apr  7 16:55:42 2023, max compression
+gzip compressed data, was "skellycam-2023.4.1082.tar", last modified: Fri Apr  7 16:56:05 2023, max compression
```

## Comparing `skellycam-2023.4.1081.tar` & `skellycam-2023.4.1082.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0     1087 2023-04-07 16:55:34.008166 skellycam-2023.4.1081/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1280 2023-04-07 16:55:34.008166 skellycam-2023.4.1081/.gitignore
--rw-r--r--   0        0        0     3267 2023-04-07 16:55:34.008166 skellycam-2023.4.1081/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-04-07 16:55:34.008166 skellycam-2023.4.1081/LICENSE
--rw-r--r--   0        0        0        8 2023-04-07 16:55:34.008166 skellycam-2023.4.1081/MANIFEST.in
--rw-r--r--   0        0        0     5247 2023-04-07 16:55:34.008166 skellycam-2023.4.1081/README.md
--rw-r--r--   0        0        0  1243325 2023-04-07 16:55:34.012166 skellycam-2023.4.1081/assets/logo/skelly-cam-logo.ai
--rw-r--r--   0        0        0   159269 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/assets/logo/skelly-cam-logo.png
--rw-r--r--   0        0        0    12576 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/assets/logo/skelly-cam-logo.svg
--rw-r--r--   0        0        0     2922 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/pyproject.toml
--rw-r--r--   0        0        0       13 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/requirements-dev.txt
--rw-r--r--   0        0        0      224 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/requirements.txt
--rw-r--r--   0        0        0       50 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/setup.py
--rw-r--r--   0        0        0     1489 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/__init__.py
--rw-r--r--   0        0        0      899 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/__main__.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/detection/__init__.py
--rw-r--r--   0        0        0      593 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/detection/detect_cameras.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/detection/models/__init__.py
--rw-r--r--   0        0        0      468 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/detection/models/frame_payload.py
--rw-r--r--   0        0        0     2609 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/detection/private/detect_possible_cameras.py
--rw-r--r--   0        0        0      262 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/detection/private/found_camera_cache.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/diagnostics/__init__.py
--rw-r--r--   0        0        0     1940 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/diagnostics/create_diagnostic_plots.py
--rw-r--r--   0        0        0     2636 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/diagnostics/plot_first_middle_and_last_frames.py
--rw-r--r--   0        0        0     7874 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/diagnostics/plot_framerate_diagnostics.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/examples/__init__.py
--rw-r--r--   0        0        0      151 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/examples/example1_single_camera_connection.py
--rw-r--r--   0        0        0      683 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/examples/example2_record_synchronized_videos.py
--rw-r--r--   0        0        0     1287 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/examples/show_all_cameras_in_cv2_windows.py
--rw-r--r--   0        0        0       87 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/experiments/__init__.py
--rw-r--r--   0        0        0      256 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/experiments/cam_show.py
--rw-r--r--   0        0        0      535 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/experiments/imshow_tester.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/experiments/multi_camera_recorder/__init__.py
--rw-r--r--   0        0        0     7268 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/experiments/multi_camera_recorder/multicamera_video_recorder.py
--rw-r--r--   0        0        0      774 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/experiments/slider_widget.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/css/__init__.py
--rw-r--r--   0        0        0     2735 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/css/qt_css_stylesheet.py
--rw-r--r--   0        0        0      679 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/main.py
--rw-r--r--   0        0        0     6240 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/skelly_cam_main_window.py
--rw-r--r--   0        0        0    14467 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/skelly_cam_widget.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/utilities/__init__.py
--rw-r--r--   0        0        0      495 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/utilities/clear_layout.py
--rw-r--r--   0        0        0      189 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/utilities/get_qt_app.py
--rw-r--r--   0        0        0     2042 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/utilities/qt_label_strings.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/widgets/__init__.py
--rw-r--r--   0        0        0     3068 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/widgets/single_camera_view_widget.py
--rw-r--r--   0        0        0    13091 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/widgets/skelly_cam_config_parameter_tree_widget.py
--rw-r--r--   0        0        0     5909 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/widgets/skelly_cam_controller_widget.py
--rw-r--r--   0        0        0     3740 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/widgets/skelly_cam_directory_view_widget.py
--rw-r--r--   0        0        0     2179 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/widgets/welcome_to_skellycam_widget.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.016166 skellycam-2023.4.1081/skellycam/gui/qt/workers/__init__.py
--rw-r--r--   0        0        0    11268 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/gui/qt/workers/camera_group_process_worker.py
--rw-r--r--   0        0        0    10777 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/gui/qt/workers/camera_group_thread_worker.py
--rw-r--r--   0        0        0      532 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/gui/qt/workers/detect_cameras_worker.py
--rw-r--r--   0        0        0     1028 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/gui/qt/workers/save_videos_worker.py
--rw-r--r--   0        0        0     1452 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/gui/qt/workers/video_save_thread_worker.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/camera/__init__.py
--rw-r--r--   0        0        0      270 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/camera/attributes.py
--rw-r--r--   0        0        0     3319 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/camera/camera.py
--rw-r--r--   0        0        0     6228 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/camera/internal_camera_thread.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/camera/models/__init__.py
--rw-r--r--   0        0        0      389 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/camera/models/camera_config.py
--rw-r--r--   0        0        0       15 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/camera/types/camera_id.py
--rw-r--r--   0        0        0     1501 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/config/apply_config.py
--rw-r--r--   0        0        0      379 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/config/determine_backend.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/group/__init__.py
--rw-r--r--   0        0        0     6547 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/group/camera_group.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/group/strategies/__init__.py
--rw-r--r--   0        0        0     6787 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/group/strategies/cam_group_queue_process.py
--rw-r--r--   0        0        0     1732 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/group/strategies/cam_group_zeromq_process.py
--rw-r--r--   0        0        0     3357 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/group/strategies/grouped_process_strategy.py
--rw-r--r--   0        0        0      494 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/group/strategies/queue_communicator.py
--rw-r--r--   0        0        0       96 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/group/strategies/strategies.py
--rw-r--r--   0        0        0      874 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/simplest_opencv_webcam_display.py
--rw-r--r--   0        0        0     5660 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/video_recorder/save_synchronized_videos.py
--rw-r--r--   0        0        0     6560 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/opencv/video_recorder/video_recorder.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/system/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/system/environment/__init__.py
--rw-r--r--   0        0        0     3495 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/system/environment/default_paths.py
--rw-r--r--   0        0        0       86 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/system/environment/home_dir.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/system/log_config/__init__.py
--rw-r--r--   0        0        0     1458 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/system/log_config/logsetup.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/tests/__init__.py
--rw-r--r--   0        0        0      542 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/tests/test_frame_timestamp_synchronization.py
--rw-r--r--   0        0        0      749 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/tests/test_synchronized_video_frame_counts.py
--rw-r--r--   0        0        0       79 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/tests/test_test.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/tests/utilities/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0      476 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/utils/array_split_by.py
--rw-r--r--   0        0        0      251 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/utils/start_file.py
--rw-r--r--   0        0        0        0 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/viewers/__init__.py
--rw-r--r--   0        0        0     1000 2023-04-07 16:55:34.020166 skellycam-2023.4.1081/skellycam/viewers/cv_cam_viewer.py
--rw-r--r--   0        0        0     7699 1970-01-01 00:00:00.000000 skellycam-2023.4.1081/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-04-07 16:56:00.217410 skellycam-2023.4.1082/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1280 2023-04-07 16:56:00.217410 skellycam-2023.4.1082/.gitignore
+-rw-r--r--   0        0        0     3267 2023-04-07 16:56:00.217410 skellycam-2023.4.1082/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-04-07 16:56:00.217410 skellycam-2023.4.1082/LICENSE
+-rw-r--r--   0        0        0        8 2023-04-07 16:56:00.217410 skellycam-2023.4.1082/MANIFEST.in
+-rw-r--r--   0        0        0     5247 2023-04-07 16:56:00.217410 skellycam-2023.4.1082/README.md
+-rw-r--r--   0        0        0  1243325 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/assets/logo/skelly-cam-logo.ai
+-rw-r--r--   0        0        0   159269 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/assets/logo/skelly-cam-logo.png
+-rw-r--r--   0        0        0    12576 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/assets/logo/skelly-cam-logo.svg
+-rw-r--r--   0        0        0     2922 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/requirements-dev.txt
+-rw-r--r--   0        0        0      224 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/requirements.txt
+-rw-r--r--   0        0        0       50 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/setup.py
+-rw-r--r--   0        0        0     1489 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/__init__.py
+-rw-r--r--   0        0        0      899 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/detection/__init__.py
+-rw-r--r--   0        0        0      593 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/detection/detect_cameras.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/detection/models/__init__.py
+-rw-r--r--   0        0        0      468 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/detection/models/frame_payload.py
+-rw-r--r--   0        0        0     2609 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/detection/private/detect_possible_cameras.py
+-rw-r--r--   0        0        0      262 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/detection/private/found_camera_cache.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/diagnostics/__init__.py
+-rw-r--r--   0        0        0     1940 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/diagnostics/create_diagnostic_plots.py
+-rw-r--r--   0        0        0     2636 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/diagnostics/plot_first_middle_and_last_frames.py
+-rw-r--r--   0        0        0     7874 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/diagnostics/plot_framerate_diagnostics.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/examples/__init__.py
+-rw-r--r--   0        0        0      151 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/examples/example1_single_camera_connection.py
+-rw-r--r--   0        0        0      683 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/examples/example2_record_synchronized_videos.py
+-rw-r--r--   0        0        0     1287 2023-04-07 16:56:00.221410 skellycam-2023.4.1082/skellycam/examples/show_all_cameras_in_cv2_windows.py
+-rw-r--r--   0        0        0       87 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/experiments/__init__.py
+-rw-r--r--   0        0        0      256 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/experiments/cam_show.py
+-rw-r--r--   0        0        0      535 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/experiments/imshow_tester.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/experiments/multi_camera_recorder/__init__.py
+-rw-r--r--   0        0        0     7268 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/experiments/multi_camera_recorder/multicamera_video_recorder.py
+-rw-r--r--   0        0        0      774 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/experiments/slider_widget.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/css/__init__.py
+-rw-r--r--   0        0        0     2735 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/css/qt_css_stylesheet.py
+-rw-r--r--   0        0        0      679 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/main.py
+-rw-r--r--   0        0        0     6240 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/skelly_cam_main_window.py
+-rw-r--r--   0        0        0    14467 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/skelly_cam_widget.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/utilities/__init__.py
+-rw-r--r--   0        0        0      495 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/utilities/clear_layout.py
+-rw-r--r--   0        0        0      189 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/utilities/get_qt_app.py
+-rw-r--r--   0        0        0     2042 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/utilities/qt_label_strings.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/widgets/__init__.py
+-rw-r--r--   0        0        0     3068 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/widgets/single_camera_view_widget.py
+-rw-r--r--   0        0        0    13091 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/widgets/skelly_cam_config_parameter_tree_widget.py
+-rw-r--r--   0        0        0     5909 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/widgets/skelly_cam_controller_widget.py
+-rw-r--r--   0        0        0     3740 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/widgets/skelly_cam_directory_view_widget.py
+-rw-r--r--   0        0        0     2179 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/widgets/welcome_to_skellycam_widget.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/workers/__init__.py
+-rw-r--r--   0        0        0    11268 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/workers/camera_group_process_worker.py
+-rw-r--r--   0        0        0     9886 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/workers/camera_group_thread_worker.py
+-rw-r--r--   0        0        0      532 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/workers/detect_cameras_worker.py
+-rw-r--r--   0        0        0     1028 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/workers/save_videos_worker.py
+-rw-r--r--   0        0        0     1452 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/gui/qt/workers/video_save_thread_worker.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/camera/__init__.py
+-rw-r--r--   0        0        0      270 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/camera/attributes.py
+-rw-r--r--   0        0        0     3319 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/camera/camera.py
+-rw-r--r--   0        0        0     6228 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/camera/internal_camera_thread.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/camera/models/__init__.py
+-rw-r--r--   0        0        0      389 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/camera/models/camera_config.py
+-rw-r--r--   0        0        0       15 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/camera/types/camera_id.py
+-rw-r--r--   0        0        0     1501 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/config/apply_config.py
+-rw-r--r--   0        0        0      379 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/config/determine_backend.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/group/__init__.py
+-rw-r--r--   0        0        0     6574 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/group/camera_group.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/group/strategies/__init__.py
+-rw-r--r--   0        0        0     6787 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/group/strategies/cam_group_queue_process.py
+-rw-r--r--   0        0        0     1732 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/group/strategies/cam_group_zeromq_process.py
+-rw-r--r--   0        0        0     3357 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/group/strategies/grouped_process_strategy.py
+-rw-r--r--   0        0        0      494 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/group/strategies/queue_communicator.py
+-rw-r--r--   0        0        0       96 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/group/strategies/strategies.py
+-rw-r--r--   0        0        0      874 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/simplest_opencv_webcam_display.py
+-rw-r--r--   0        0        0     5660 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/video_recorder/save_synchronized_videos.py
+-rw-r--r--   0        0        0     6560 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/opencv/video_recorder/video_recorder.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/system/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/system/environment/__init__.py
+-rw-r--r--   0        0        0     3495 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/system/environment/default_paths.py
+-rw-r--r--   0        0        0       86 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/system/environment/home_dir.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/system/log_config/__init__.py
+-rw-r--r--   0        0        0     1458 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/system/log_config/logsetup.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/tests/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/tests/test_frame_timestamp_synchronization.py
+-rw-r--r--   0        0        0      749 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/tests/test_synchronized_video_frame_counts.py
+-rw-r--r--   0        0        0       79 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/tests/test_test.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/tests/utilities/__init__.py
+-rw-r--r--   0        0        0     1036 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0      476 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/utils/array_split_by.py
+-rw-r--r--   0        0        0      251 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/utils/start_file.py
+-rw-r--r--   0        0        0        0 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/viewers/__init__.py
+-rw-r--r--   0        0        0     1000 2023-04-07 16:56:00.225410 skellycam-2023.4.1082/skellycam/viewers/cv_cam_viewer.py
+-rw-r--r--   0        0        0     7699 1970-01-01 00:00:00.000000 skellycam-2023.4.1082/PKG-INFO
```

### Comparing `skellycam-2023.4.1081/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skellycam-2023.4.1082/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/.gitignore` & `skellycam-2023.4.1082/.gitignore`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/CONTRIBUTING.md` & `skellycam-2023.4.1082/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/LICENSE` & `skellycam-2023.4.1082/LICENSE`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/README.md` & `skellycam-2023.4.1082/README.md`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/assets/logo/skelly-cam-logo.ai` & `skellycam-2023.4.1082/assets/logo/skelly-cam-logo.ai`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/assets/logo/skelly-cam-logo.png` & `skellycam-2023.4.1082/assets/logo/skelly-cam-logo.png`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/assets/logo/skelly-cam-logo.svg` & `skellycam-2023.4.1082/assets/logo/skelly-cam-logo.svg`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/pyproject.toml` & `skellycam-2023.4.1082/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/freemocap/skellycam"
 
 [tool.bumpver]
-current_version = "v2023.04.1081"
+current_version = "v2023.04.1082"
 
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
```

### Comparing `skellycam-2023.4.1081/skellycam/__init__.py` & `skellycam-2023.4.1082/skellycam/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for skellycam."""
 
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
-__version__ = "v2023.04.1081"
+__version__ = "v2023.04.1082"
 
 __description__ = "A simple python API for efficiently connecting to and recording synchronized videos from one or multiple cameras 💀📸"
 __package_name__ = "skellycam"
 __repo_url__ = f"https://github.com/freemocap/{__package_name__}/"
 __repo_issues_url__ = f"{__repo_url__}issues"
 
 import sys
```

### Comparing `skellycam-2023.4.1081/skellycam/__main__.py` & `skellycam-2023.4.1082/skellycam/__main__.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/detection/detect_cameras.py` & `skellycam-2023.4.1082/skellycam/detection/detect_cameras.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/detection/private/detect_possible_cameras.py` & `skellycam-2023.4.1082/skellycam/detection/private/detect_possible_cameras.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/diagnostics/create_diagnostic_plots.py` & `skellycam-2023.4.1082/skellycam/diagnostics/create_diagnostic_plots.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/diagnostics/plot_first_middle_and_last_frames.py` & `skellycam-2023.4.1082/skellycam/diagnostics/plot_first_middle_and_last_frames.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/diagnostics/plot_framerate_diagnostics.py` & `skellycam-2023.4.1082/skellycam/diagnostics/plot_framerate_diagnostics.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/examples/example2_record_synchronized_videos.py` & `skellycam-2023.4.1082/skellycam/examples/example2_record_synchronized_videos.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/examples/show_all_cameras_in_cv2_windows.py` & `skellycam-2023.4.1082/skellycam/examples/show_all_cameras_in_cv2_windows.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/experiments/imshow_tester.py` & `skellycam-2023.4.1082/skellycam/experiments/imshow_tester.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/experiments/multi_camera_recorder/multicamera_video_recorder.py` & `skellycam-2023.4.1082/skellycam/experiments/multi_camera_recorder/multicamera_video_recorder.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/experiments/slider_widget.py` & `skellycam-2023.4.1082/skellycam/experiments/slider_widget.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/css/qt_css_stylesheet.py` & `skellycam-2023.4.1082/skellycam/gui/qt/css/qt_css_stylesheet.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/main.py` & `skellycam-2023.4.1082/skellycam/gui/qt/main.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/skelly_cam_main_window.py` & `skellycam-2023.4.1082/skellycam/gui/qt/skelly_cam_main_window.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/skelly_cam_widget.py` & `skellycam-2023.4.1082/skellycam/gui/qt/skelly_cam_widget.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/utilities/qt_label_strings.py` & `skellycam-2023.4.1082/skellycam/gui/qt/utilities/qt_label_strings.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/widgets/single_camera_view_widget.py` & `skellycam-2023.4.1082/skellycam/gui/qt/widgets/single_camera_view_widget.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/widgets/skelly_cam_config_parameter_tree_widget.py` & `skellycam-2023.4.1082/skellycam/gui/qt/widgets/skelly_cam_config_parameter_tree_widget.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/widgets/skelly_cam_controller_widget.py` & `skellycam-2023.4.1082/skellycam/gui/qt/widgets/skelly_cam_controller_widget.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/widgets/skelly_cam_directory_view_widget.py` & `skellycam-2023.4.1082/skellycam/gui/qt/widgets/skelly_cam_directory_view_widget.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/widgets/welcome_to_skellycam_widget.py` & `skellycam-2023.4.1082/skellycam/gui/qt/widgets/welcome_to_skellycam_widget.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/workers/camera_group_process_worker.py` & `skellycam-2023.4.1082/skellycam/gui/qt/workers/camera_group_process_worker.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/workers/camera_group_thread_worker.py` & `skellycam-2023.4.1082/skellycam/gui/qt/workers/camera_group_thread_worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -186,70 +186,47 @@
         if self._camera_group is None:
             self._camera_group = self._create_camera_group(
                 camera_ids=self.camera_ids,
                 camera_config_dictionary=camera_config_dictionary,
             )
             return
 
+        self._video_recorder_dictionary = self._initialize_video_recorder_dictionary()
         self._updating_camera_settings_bool = True
         self._updating_camera_settings_bool = not self._update_camera_settings(
             camera_config_dictionary
         )
 
     def _launch_save_video_thread_worker(self):
         logger.info("Launching save video thread worker")
 
         synchronized_videos_folder = self._synchronized_video_folder_path
         self._synchronized_video_folder_path = None
 
+
         self._video_save_thread_worker = VideoSaveThreadWorker(
             dictionary_of_video_recorders=deepcopy(self._video_recorder_dictionary),
             folder_to_save_videos=str(synchronized_videos_folder),
             create_diagnostic_plots_bool=True,
         )
         self._video_save_thread_worker.start()
         self._video_save_thread_worker.finished_signal.connect(
             self._handle_videos_save_thread_worker_finished
         )
 
     def _handle_videos_save_thread_worker_finished(self, folder_path: str):
         logger.debug(f"Emitting `videos_saved_to_this_folder_signal` with string: {folder_path}")
         self.videos_saved_to_this_folder_signal.emit(folder_path)
 
-    #
-    # def _launch_save_video_process(self):
-    #     logger.info("Launching save video process")
-    #     if self._video_save_process is not None:
-    #         while self._video_save_process.is_alive():
-    #             time.sleep(0.1)
-    #             logger.info(
-    #                 f"Waiting for video save process to finish: {self._video_save_process}"
-    #             )
-    #
-    #     synchronized_videos_folder = self._synchronized_video_folder_path
-    #     self._synchronized_video_folder_path = None
-    #     self._video_save_process = Process(
-    #         name=f"VideoSaveProcess",
-    #         target=save_synchronized_videos,
-    #         args=(
-    #             deepcopy(self._video_recorder_dictionary),
-    #             synchronized_videos_folder,
-    #             True,
-    #             self.videos_saved_to_this_folder_signal
-    #         ),
-    #     )
-    #     logger.info(f"Launching video save process: {self._video_save_process}")
-    #
-    #     self._video_save_process.start()
-    #     self._video_save_thread_worker.finished_signal.connect(
-    #         lambda: self.videos_saved_to_this_folder_signal.emit
-    #     )
-
     def _initialize_video_recorder_dictionary(self):
-        return {camera_id: VideoRecorder() for camera_id in self._camera_ids}
+        video_recorder_dictionary = {}
+        for camera_id, config in self._camera_group.camera_config_dictionary.items():
+            if config.use_this_camera:
+                video_recorder_dictionary[camera_id] = VideoRecorder()
+        return video_recorder_dictionary
 
     def _get_recorder_frame_count_dict(self):
         return {
             camera_id: recorder.number_of_frames
             for camera_id, recorder in self._video_recorder_dictionary.items()
         }
```

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/workers/detect_cameras_worker.py` & `skellycam-2023.4.1082/skellycam/gui/qt/workers/detect_cameras_worker.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/workers/save_videos_worker.py` & `skellycam-2023.4.1082/skellycam/gui/qt/workers/save_videos_worker.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/gui/qt/workers/video_save_thread_worker.py` & `skellycam-2023.4.1082/skellycam/gui/qt/workers/video_save_thread_worker.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/opencv/camera/camera.py` & `skellycam-2023.4.1082/skellycam/opencv/camera/camera.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/opencv/camera/internal_camera_thread.py` & `skellycam-2023.4.1082/skellycam/opencv/camera/internal_camera_thread.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/opencv/config/apply_config.py` & `skellycam-2023.4.1082/skellycam/opencv/config/apply_config.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/opencv/group/camera_group.py` & `skellycam-2023.4.1082/skellycam/opencv/group/camera_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         return self._exit_event
 
     @property
     def camera_ids(self):
         return self._camera_ids
 
     @property
-    def camera_config_dictionary(self):
+    def camera_config_dictionary(self) -> Dict[str, CameraConfig]:
         return self._camera_config_dictionary
 
     @property
     def queue_size(self) -> Dict[str, int]:
         return self._strategy_class.queue_size
 
     def update_camera_configs(self, camera_config_dictionary: Dict[str, CameraConfig]):
```

### Comparing `skellycam-2023.4.1081/skellycam/opencv/group/strategies/cam_group_queue_process.py` & `skellycam-2023.4.1082/skellycam/opencv/group/strategies/cam_group_queue_process.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/opencv/group/strategies/cam_group_zeromq_process.py` & `skellycam-2023.4.1082/skellycam/opencv/group/strategies/cam_group_zeromq_process.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/opencv/group/strategies/grouped_process_strategy.py` & `skellycam-2023.4.1082/skellycam/opencv/group/strategies/grouped_process_strategy.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/opencv/simplest_opencv_webcam_display.py` & `skellycam-2023.4.1082/skellycam/opencv/simplest_opencv_webcam_display.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/opencv/video_recorder/save_synchronized_videos.py` & `skellycam-2023.4.1082/skellycam/opencv/video_recorder/save_synchronized_videos.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/opencv/video_recorder/video_recorder.py` & `skellycam-2023.4.1082/skellycam/opencv/video_recorder/video_recorder.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/system/environment/default_paths.py` & `skellycam-2023.4.1082/skellycam/system/environment/default_paths.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/system/log_config/logsetup.py` & `skellycam-2023.4.1082/skellycam/system/log_config/logsetup.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/tests/test_frame_timestamp_synchronization.py` & `skellycam-2023.4.1082/skellycam/tests/test_frame_timestamp_synchronization.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/tests/test_synchronized_video_frame_counts.py` & `skellycam-2023.4.1082/skellycam/tests/test_synchronized_video_frame_counts.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skellycam-2023.4.1082/skellycam/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/skellycam/viewers/cv_cam_viewer.py` & `skellycam-2023.4.1082/skellycam/viewers/cv_cam_viewer.py`

 * *Files identical despite different names*

### Comparing `skellycam-2023.4.1081/PKG-INFO` & `skellycam-2023.4.1082/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skellycam
-Version: 2023.4.1081
+Version: 2023.4.1082
 Summary: Top-level package for skellycam.
 Keywords: camera,stream,video,image,opencv,skelly,freemocap,motion capture,synchronization,computer vision
 Author: Endurance Idehen, Jonathan Samir Matthis
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skellycam Version: 2023.4.1081 Summary: Top-level
+Metadata-Version: 2.1 Name: skellycam Version: 2023.4.1082 Summary: Top-level
 package for skellycam. Keywords:
 camera,stream,video,image,opencv,skelly,freemocap,motion
 capture,synchronization,computer vision Author: Endurance Idehen, Jonathan
 Samir Matthis Author-email: Skelly FreeMoCap
 freemocap.org> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: License :: OSI Approved
 :: GNU Affero General Public License v3 or later (AGPLv3+) Classifier: Intended
```

