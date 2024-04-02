# Comparing `tmp/diplomat_track-0.1.1.tar.gz` & `tmp/diplomat_track-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diplomat_track-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "diplomat_track-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `diplomat_track-0.1.1.tar` & `diplomat_track-0.1.2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0     5826 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/README.md
--rw-r--r--   0        0        0     2548 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/__init__.py
--rw-r--r--   0        0        0       45 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/__main__.py
--rw-r--r--   0        0        0     2456 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/_cli_runner.py
--rw-r--r--   0        0        0    22991 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/core_ops.py
--rw-r--r--   0        0        0     1432 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontend_ops.py
--rw-r--r--   0        0        0     7089 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/__init__.py
--rw-r--r--   0        0        0      901 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/csv/__init__.py
--rw-r--r--   0        0        0      475 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/csv/_verify_func.py
--rw-r--r--   0        0        0      938 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/csv/csv_utils.py
--rw-r--r--   0        0        0     5436 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/csv/label_videos.py
--rw-r--r--   0        0        0     3049 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/csv/tweak_results.py
--rw-r--r--   0        0        0     1428 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/deeplabcut/__init__.py
--rw-r--r--   0        0        0      980 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/deeplabcut/_verify_func.py
--rw-r--r--   0        0        0     2879 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/deeplabcut/convert_results_dlc.py
--rw-r--r--   0        0        0      679 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/deeplabcut/dlc_importer.py
--rw-r--r--   0        0        0    10254 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/deeplabcut/label_videos_dlc.py
--rw-r--r--   0        0        0    13430 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/deeplabcut/predict_frames_dlc.py
--rw-r--r--   0        0        0    19560 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/deeplabcut/predict_videos_dlc.py
--rw-r--r--   0        0        0     1806 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/deeplabcut/save_from_restore.py
--rw-r--r--   0        0        0     4185 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/deeplabcut/tweak_results.py
--rw-r--r--   0        0        0     1391 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/__init__.py
--rw-r--r--   0        0        0      458 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/_verify_func.py
--rw-r--r--   0        0        0     1704 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/convert_results_sleap.py
--rw-r--r--   0        0        0     5323 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/label_videos_sleap.py
--rw-r--r--   0        0        0     8744 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/predict_frames_sleap.py
--rw-r--r--   0        0        0     6413 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/predict_videos_sleap.py
--rw-r--r--   0        0        0     9260 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/run_utils.py
--rw-r--r--   0        0        0     1355 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/save_from_restore.py
--rw-r--r--   0        0        0      590 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/sleap_importer.py
--rw-r--r--   0        0        0    12331 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/sleap_providers.py
--rw-r--r--   0        0        0     2539 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/tweak_results_sleap.py
--rw-r--r--   0        0        0     2277 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/frontends/sleap/visual_settings.py
--rw-r--r--   0        0        0     5416 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictor_ops.py
--rw-r--r--   0        0        0        0 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/__init__.py
--rw-r--r--   0        0        0      699 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/argmax.py
--rw-r--r--   0        0        0    14516 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fastplotter.py
--rw-r--r--   0        0        0        0 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/__init__.py
--rw-r--r--   0        0        0     4917 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/arr_utils.py
--rw-r--r--   0        0        0     1319 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/fpe_help.py
--rw-r--r--   0        0        0     7374 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/fpe_math.py
--rw-r--r--   0        0        0    24838 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/fpe_test_data.py
--rw-r--r--   0        0        0     4284 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/frame_pass.py
--rw-r--r--   0        0        0    23031 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/frame_pass_engine.py
--rw-r--r--   0        0        0     1530 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/frame_pass_loader.py
--rw-r--r--   0        0        0        0 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/__init__.py
--rw-r--r--   0        0        0    11011 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/cluster_frames.py
--rw-r--r--   0        0        0     9363 2024-03-05 17:44:46.628008 diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/create_skeleton.py
--rw-r--r--   0        0        0    22849 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/fix_frame.py
--rw-r--r--   0        0        0    47968 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/mit_viterbi.py
--rw-r--r--   0        0        0     5120 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/optimize_std.py
--rw-r--r--   0        0        0    13500 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/fpe/skeleton_structures.py
--rw-r--r--   0        0        0    29594 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/fpe/sparse_storage.py
--rw-r--r--   0        0        0     5863 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/frame_exporter.py
--rw-r--r--   0        0        0    11920 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/plotter.py
--rw-r--r--   0        0        0        0 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/sfpe/__init__.py
--rw-r--r--   0        0        0      767 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/sfpe/assignment.py
--rw-r--r--   0        0        0    14995 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/sfpe/avl_tree.py
--rw-r--r--   0        0        0     9344 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/sfpe/disk_sparse_storage.py
--rw-r--r--   0        0        0    18778 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/sfpe/file_io.py
--rw-r--r--   0        0        0     1361 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/sfpe/growable_numpy_array.py
--rw-r--r--   0        0        0     4263 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/sfpe/segmentation.py
--rw-r--r--   0        0        0    63512 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/sfpe/segmented_frame_pass_engine.py
--rw-r--r--   0        0        0        0 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/supervised_fpe/__init__.py
--rw-r--r--   0        0        0    18822 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/supervised_fpe/labelers.py
--rw-r--r--   0        0        0     6622 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/supervised_fpe/scorers.py
--rw-r--r--   0        0        0    18822 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py
--rw-r--r--   0        0        0        0 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/supervised_sfpe/__init__.py
--rw-r--r--   0        0        0    28773 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py
--rw-r--r--   0        0        0     2168 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/processing/__init__.py
--rw-r--r--   0        0        0     3523 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/processing/containers.py
--rw-r--r--   0        0        0    11144 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/processing/pose.py
--rw-r--r--   0        0        0    13781 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/processing/predictor.py
--rw-r--r--   0        0        0     3749 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/processing/progress_bar.py
--rw-r--r--   0        0        0    18651 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/processing/track_data.py
--rw-r--r--   0        0        0    21853 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/processing/type_casters.py
--rw-r--r--   0        0        0       96 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/__init__.py
--rw-r--r--   0        0        0      360 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/_bit_or.py
--rw-r--r--   0        0        0      874 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/_function_tools.py
--rw-r--r--   0        0        0    11484 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/cli_tools.py
--rw-r--r--   0        0        0     3153 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/colormaps.py
--rw-r--r--   0        0        0    11695 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/extract_frames.py
--rw-r--r--   0        0        0    10794 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/frame_store_api.py
--rw-r--r--   0        0        0    28484 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/frame_store_fmt.py
--rw-r--r--   0        0        0     8442 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/graph_ops.py
--rw-r--r--   0        0        0     3980 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/lazy_import.py
--rw-r--r--   0        0        0     4284 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/pluginloader.py
--rw-r--r--   0        0        0     1690 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/pretty_printer.py
--rw-r--r--   0        0        0     6965 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/shapes.py
--rw-r--r--   0        0        0     2816 2024-03-05 17:44:46.632008 diplomat_track-0.1.1/diplomat/utils/track_formats.py
--rw-r--r--   0        0        0    11520 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/utils/tweak_ui.py
--rw-r--r--   0        0        0      925 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/utils/video_info.py
--rw-r--r--   0        0        0     1596 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/utils/video_io.py
--rw-r--r--   0        0        0     6823 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/utils/video_splitter.py
--rw-r--r--   0        0        0      403 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/__init__.py
--rw-r--r--   0        0        0    37702 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/fpe_editor.py
--rw-r--r--   0        0        0     4670 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/helpdialog.py
--rw-r--r--   0        0        0    14468 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/icons.py
--rw-r--r--   0        0        0    14402 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/id_swap_dialog.py
--rw-r--r--   0        0        0     2026 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/identity_swapper.py
--rw-r--r--   0        0        0    15199 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/labeler_lib.py
--rw-r--r--   0        0        0    46523 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/point_edit.py
--rw-r--r--   0        0        0    25981 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/probability_displayer.py
--rw-r--r--   0        0        0     7308 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/progress_bar.py
--rw-r--r--   0        0        0     2382 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/progress_dialog.py
--rw-r--r--   0        0        0     6002 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/score_lib.py
--rw-r--r--   0        0        0     8477 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/scroll_image_list.py
--rw-r--r--   0        0        0     4380 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/settings_dialog.py
--rw-r--r--   0        0        0    35348 2024-03-05 17:44:46.636008 diplomat_track-0.1.1/diplomat/wx_gui/video_player.py
--rw-r--r--   0        0        0     1119 2024-03-05 17:44:46.680008 diplomat_track-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7054 1970-01-01 00:00:00.000000 diplomat_track-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5836 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/README.md
+-rw-r--r--   0        0        0     2548 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/__main__.py
+-rw-r--r--   0        0        0     2456 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/_cli_runner.py
+-rw-r--r--   0        0        0    22991 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/core_ops.py
+-rw-r--r--   0        0        0     1432 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontend_ops.py
+-rw-r--r--   0        0        0     7089 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/csv/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/csv/_verify_func.py
+-rw-r--r--   0        0        0      938 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/csv/csv_utils.py
+-rw-r--r--   0        0        0     5436 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/csv/label_videos.py
+-rw-r--r--   0        0        0     3049 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/csv/tweak_results.py
+-rw-r--r--   0        0        0     1464 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/deeplabcut/__init__.py
+-rw-r--r--   0        0        0      980 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/deeplabcut/_verify_func.py
+-rw-r--r--   0        0        0     2879 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/deeplabcut/convert_results_dlc.py
+-rw-r--r--   0        0        0      679 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/deeplabcut/dlc_importer.py
+-rw-r--r--   0        0        0    10254 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/deeplabcut/label_videos_dlc.py
+-rw-r--r--   0        0        0    13430 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/deeplabcut/predict_frames_dlc.py
+-rw-r--r--   0        0        0    19560 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/deeplabcut/predict_videos_dlc.py
+-rw-r--r--   0        0        0     1806 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/deeplabcut/save_from_restore.py
+-rw-r--r--   0        0        0     4185 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/deeplabcut/tweak_results.py
+-rw-r--r--   0        0        0     1391 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/__init__.py
+-rw-r--r--   0        0        0      458 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/_verify_func.py
+-rw-r--r--   0        0        0     1704 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/convert_results_sleap.py
+-rw-r--r--   0        0        0     5323 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/label_videos_sleap.py
+-rw-r--r--   0        0        0     8744 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/predict_frames_sleap.py
+-rw-r--r--   0        0        0     6413 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/predict_videos_sleap.py
+-rw-r--r--   0        0        0     9260 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/run_utils.py
+-rw-r--r--   0        0        0     1355 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/save_from_restore.py
+-rw-r--r--   0        0        0      590 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/sleap_importer.py
+-rw-r--r--   0        0        0    12331 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/sleap_providers.py
+-rw-r--r--   0        0        0     2539 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/tweak_results_sleap.py
+-rw-r--r--   0        0        0     2277 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/frontends/sleap/visual_settings.py
+-rw-r--r--   0        0        0     5416 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictor_ops.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictors/__init__.py
+-rw-r--r--   0        0        0      699 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictors/argmax.py
+-rw-r--r--   0        0        0    14516 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictors/fastplotter.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictors/fpe/__init__.py
+-rw-r--r--   0        0        0     4917 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictors/fpe/arr_utils.py
+-rw-r--r--   0        0        0     1319 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictors/fpe/fpe_help.py
+-rw-r--r--   0        0        0     7374 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictors/fpe/fpe_math.py
+-rw-r--r--   0        0        0    24838 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictors/fpe/fpe_test_data.py
+-rw-r--r--   0        0        0     4284 2024-04-02 16:21:30.323031 diplomat_track-0.1.2/diplomat/predictors/fpe/frame_pass.py
+-rw-r--r--   0        0        0    23031 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/frame_pass_engine.py
+-rw-r--r--   0        0        0     1530 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/frame_pass_loader.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/__init__.py
+-rw-r--r--   0        0        0    11011 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/cluster_frames.py
+-rw-r--r--   0        0        0     9363 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/create_skeleton.py
+-rw-r--r--   0        0        0    26266 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/fix_frame.py
+-rw-r--r--   0        0        0    48985 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/mit_viterbi.py
+-rw-r--r--   0        0        0     5120 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/optimize_std.py
+-rw-r--r--   0        0        0    13500 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/skeleton_structures.py
+-rw-r--r--   0        0        0    29594 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/fpe/sparse_storage.py
+-rw-r--r--   0        0        0     5863 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/frame_exporter.py
+-rw-r--r--   0        0        0    11920 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/plotter.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/sfpe/__init__.py
+-rw-r--r--   0        0        0      767 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/sfpe/assignment.py
+-rw-r--r--   0        0        0    14995 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/sfpe/avl_tree.py
+-rw-r--r--   0        0        0     9344 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/sfpe/disk_sparse_storage.py
+-rw-r--r--   0        0        0    18778 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/sfpe/file_io.py
+-rw-r--r--   0        0        0     1361 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/sfpe/growable_numpy_array.py
+-rw-r--r--   0        0        0     4263 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/sfpe/segmentation.py
+-rw-r--r--   0        0        0    69969 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/sfpe/segmented_frame_pass_engine.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/supervised_fpe/__init__.py
+-rw-r--r--   0        0        0    20059 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/supervised_fpe/labelers.py
+-rw-r--r--   0        0        0     6622 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/supervised_fpe/scorers.py
+-rw-r--r--   0        0        0    18822 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py
+-rw-r--r--   0        0        0        0 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/supervised_sfpe/__init__.py
+-rw-r--r--   0        0        0    28291 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py
+-rw-r--r--   0        0        0     2168 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/processing/__init__.py
+-rw-r--r--   0        0        0     3523 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/processing/containers.py
+-rw-r--r--   0        0        0    11144 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/processing/pose.py
+-rw-r--r--   0        0        0    13781 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/processing/predictor.py
+-rw-r--r--   0        0        0     3749 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/processing/progress_bar.py
+-rw-r--r--   0        0        0    18651 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/processing/track_data.py
+-rw-r--r--   0        0        0    21853 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/processing/type_casters.py
+-rw-r--r--   0        0        0       96 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/utils/__init__.py
+-rw-r--r--   0        0        0      360 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/utils/_bit_or.py
+-rw-r--r--   0        0        0      874 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/utils/_function_tools.py
+-rw-r--r--   0        0        0    11484 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/utils/cli_tools.py
+-rw-r--r--   0        0        0     3153 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/utils/colormaps.py
+-rw-r--r--   0        0        0    11695 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/utils/extract_frames.py
+-rw-r--r--   0        0        0    10794 2024-04-02 16:21:30.327031 diplomat_track-0.1.2/diplomat/utils/frame_store_api.py
+-rw-r--r--   0        0        0    28484 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/frame_store_fmt.py
+-rw-r--r--   0        0        0     8442 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/graph_ops.py
+-rw-r--r--   0        0        0     3980 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/lazy_import.py
+-rw-r--r--   0        0        0     4284 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/pluginloader.py
+-rw-r--r--   0        0        0     1690 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/pretty_printer.py
+-rw-r--r--   0        0        0     6965 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/shapes.py
+-rw-r--r--   0        0        0     2816 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/track_formats.py
+-rw-r--r--   0        0        0    11520 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/tweak_ui.py
+-rw-r--r--   0        0        0      925 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/video_info.py
+-rw-r--r--   0        0        0     1596 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/video_io.py
+-rw-r--r--   0        0        0     6823 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/utils/video_splitter.py
+-rw-r--r--   0        0        0      403 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/__init__.py
+-rw-r--r--   0        0        0    37702 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/fpe_editor.py
+-rw-r--r--   0        0        0     4670 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/helpdialog.py
+-rw-r--r--   0        0        0    14468 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/icons.py
+-rw-r--r--   0        0        0    14402 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/id_swap_dialog.py
+-rw-r--r--   0        0        0     2026 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/identity_swapper.py
+-rw-r--r--   0        0        0    15199 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/labeler_lib.py
+-rw-r--r--   0        0        0    46523 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/point_edit.py
+-rw-r--r--   0        0        0    25981 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/probability_displayer.py
+-rw-r--r--   0        0        0     7308 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/progress_bar.py
+-rw-r--r--   0        0        0     2382 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/progress_dialog.py
+-rw-r--r--   0        0        0     6002 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/score_lib.py
+-rw-r--r--   0        0        0     8477 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/scroll_image_list.py
+-rw-r--r--   0        0        0     4380 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/settings_dialog.py
+-rw-r--r--   0        0        0    35348 2024-04-02 16:21:30.331031 diplomat_track-0.1.2/diplomat/wx_gui/video_player.py
+-rw-r--r--   0        0        0     1119 2024-04-02 16:21:30.375032 diplomat_track-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7064 1970-01-01 00:00:00.000000 diplomat_track-0.1.2/PKG-INFO
```

### Comparing `diplomat_track-0.1.1/README.md` & `diplomat_track-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # DIPLOMAT
 
 Deep learning-based Identity Preserving Labeled-Object Multi-Animal Tracking.
 
-**NOTE:** DIPLOMAT is currently alpha software, there may be minor bugs and issues.
+**NOTE:** DIPLOMAT is currently alpha software, there may be minor bugs and usability issues.
 
 ## About
 
 DIPLOMAT provides algorithms and tools for performing multi-animal identity preserving tracking on top of single animal and multi animal CNN based tracking packages. Currently, it supports running on both DeepLabCut and SLEAP projects.
 Unlike other multi-animal tracking packages, DIPLOMAT's algorithms work directly off confidence maps instead of running peak detection, allowing for more nuanced tracking results compared to other methods. 
 
 https://github.com/TravisWheelerLab/DIPLOMAT/assets/47544550/d805b673-4678-4297-b288-3fd08ad3cf62
```

### Comparing `diplomat_track-0.1.1/diplomat/__init__.py` & `diplomat_track-0.1.2/diplomat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A tool providing multi-animal tracking capabilities on top of other Deep learning based tracking software.
 """
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 # Can be used by functions to determine if diplomat was invoked through it's CLI interface.
 CLI_RUN = False
 
 from diplomat.predictor_ops import list_predictor_plugins, get_predictor_settings, test_predictor_plugin
 from diplomat.frontend_ops import list_all_frontends, list_loaded_frontends
 from diplomat.utils.video_splitter import split_videos
 from diplomat.core_ops import track_with, track, track_and_interact, annotate, tweak, yaml, convert, interact
```

### Comparing `diplomat_track-0.1.1/diplomat/_cli_runner.py` & `diplomat_track-0.1.2/diplomat/_cli_runner.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/core_ops.py` & `diplomat_track-0.1.2/diplomat/core_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontend_ops.py` & `diplomat_track-0.1.2/diplomat/frontend_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/__init__.py` & `diplomat_track-0.1.2/diplomat/frontends/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/csv/__init__.py` & `diplomat_track-0.1.2/diplomat/frontends/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/csv/csv_utils.py` & `diplomat_track-0.1.2/diplomat/frontends/csv/csv_utils.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/csv/label_videos.py` & `diplomat_track-0.1.2/diplomat/frontends/csv/label_videos.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/csv/tweak_results.py` & `diplomat_track-0.1.2/diplomat/frontends/csv/tweak_results.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/deeplabcut/__init__.py` & `diplomat_track-0.1.2/diplomat/frontends/deeplabcut/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 from diplomat.frontends import DIPLOMATFrontend, DIPLOMATCommands
-
+from diplomat.utils import colormaps
 
 class DEEPLABCUTFrontend(DIPLOMATFrontend):
     """
     The DEEPLABCUT frontend for DIPLOMAT. Contains functions for running DIPLOMAT on DEEPLABCUT projects.
     """
     @classmethod
     def init(cls) -> Optional[DIPLOMATCommands]:
```

### Comparing `diplomat_track-0.1.1/diplomat/frontends/deeplabcut/_verify_func.py` & `diplomat_track-0.1.2/diplomat/frontends/deeplabcut/_verify_func.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/deeplabcut/convert_results_dlc.py` & `diplomat_track-0.1.2/diplomat/frontends/deeplabcut/convert_results_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/deeplabcut/dlc_importer.py` & `diplomat_track-0.1.2/diplomat/frontends/deeplabcut/dlc_importer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/deeplabcut/label_videos_dlc.py` & `diplomat_track-0.1.2/diplomat/frontends/deeplabcut/label_videos_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/deeplabcut/predict_frames_dlc.py` & `diplomat_track-0.1.2/diplomat/frontends/deeplabcut/predict_frames_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/deeplabcut/predict_videos_dlc.py` & `diplomat_track-0.1.2/diplomat/frontends/deeplabcut/predict_videos_dlc.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/deeplabcut/save_from_restore.py` & `diplomat_track-0.1.2/diplomat/frontends/deeplabcut/save_from_restore.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/deeplabcut/tweak_results.py` & `diplomat_track-0.1.2/diplomat/frontends/deeplabcut/tweak_results.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/__init__.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/convert_results_sleap.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/convert_results_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/label_videos_sleap.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/label_videos_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/predict_frames_sleap.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/predict_frames_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/predict_videos_sleap.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/predict_videos_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/run_utils.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/run_utils.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/save_from_restore.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/save_from_restore.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/sleap_importer.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/sleap_importer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/sleap_providers.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/sleap_providers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/tweak_results_sleap.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/tweak_results_sleap.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/frontends/sleap/visual_settings.py` & `diplomat_track-0.1.2/diplomat/frontends/sleap/visual_settings.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictor_ops.py` & `diplomat_track-0.1.2/diplomat/predictor_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/argmax.py` & `diplomat_track-0.1.2/diplomat/predictors/argmax.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fastplotter.py` & `diplomat_track-0.1.2/diplomat/predictors/fastplotter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/arr_utils.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/arr_utils.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/fpe_help.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/fpe_help.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/fpe_math.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/fpe_math.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/fpe_test_data.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/fpe_test_data.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/frame_pass.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/frame_pass.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/frame_pass_engine.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/frame_pass_engine.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/frame_pass_loader.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/frame_pass_loader.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/cluster_frames.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/cluster_frames.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/create_skeleton.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/create_skeleton.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/fix_frame.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/fix_frame.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,14 +44,29 @@
 
     @classmethod
     def get_max_location(
         cls,
         frame: ForwardBackwardFrame,
         down_scaling: float
     ) -> Tuple[Optional[float], Optional[float], Optional[float]]:
+        """
+        Determines the maximum location within a frame after downscaling.
+
+        This method identifies the maximum probability location within a given frame and adjusts its coordinates
+        based on the provided downscaling factor. It returns the adjusted x and y coordinates along with the
+        maximum probability value.
+
+        Parameters:
+        - frame: ForwardBackwardFrame, the frame to analyze.
+        - down_scaling: float, the factor by which the frame's coordinates are downscaled.
+
+        Returns:
+        - Tuple[Optional[float], Optional[float], Optional[float]]: The adjusted x and y coordinates of the maximum
+          location and its probability. Returns None for each value if the probability data is not available.
+        """
         y, x, prob, x_off, y_off = frame.src_data.unpack()
 
         if(prob is None):
             return (None, None, None)
 
         max_idx = np.argmax(prob)
 
@@ -343,27 +358,46 @@
         frames: List[ForwardBackwardFrame],
         num_outputs: int,
         down_scaling: float,
         skeleton: Optional[StorageGraph],
         max_dist: float,
         progress_bar: Optional[ProgressBar] = None
     ) -> Tuple[float, float]:
+        """
+        Computes a single score for a given set of frames, considering the number of outputs, down scaling factor, 
+        an optional skeleton, and the maximum distance. This function aggregates the scores across all body part groupings, 
+        taking into account the minimum distance between body parts and their confidence levels. It returns a tuple 
+        containing two scores, which represent different aspects of the frame's quality or suitability for further processing.
+
+        Parameters:
+        - frames: List[ForwardBackwardFrame], a list of frames to be scored.
+        - num_outputs: int, the number of outputs or body parts to consider in each frame.
+        - down_scaling: float, the factor by which the frame dimensions have been scaled down.
+        - skeleton: Optional[StorageGraph], an optional graph representing the skeleton to be considered in scoring.
+        - max_dist: float, the maximum distance to consider when scoring body part pairs.
+        - progress_bar: Optional[ProgressBar], an optional progress bar to display processing progress.
+
+        Returns:
+        - Tuple[float, float]: A tuple containing two scores calculated based on the minimum distances and confidence levels 
+          of body part pairs across the given frames.
+        """
         num_bp = len(frames) // num_outputs
 
         score = 0
         score2 = 0
 
         for bp_group_off in range(num_bp):
 
             min_dist = np.inf
             total_conf = 0
             count = 0
 
             # For body part groupings...
             for i in range(num_outputs - 1):
+                #get the maximum probability location for the body part
                 f1_loc = cls.get_max_location(
                     frames[bp_group_off * num_outputs + i],
                     down_scaling
                 )
 
                 if (f1_loc[0] is None):
                     score = -np.inf
@@ -373,35 +407,41 @@
                     f2_loc = cls.get_max_location(
                         frames[bp_group_off * num_outputs + j], down_scaling
                     )
 
                     if (f2_loc[0] is None):
                         score = -np.inf
                         continue
-
+                    
+                    #mininum distance between the two body parts
                     min_dist = min(cls.dist(f1_loc, f2_loc), min_dist)
                     total_conf += f1_loc[2] * f2_loc[2]
                     count += 1
 
             if(np.isinf(min_dist)):
                 min_dist = 0
             if(min_dist == 0 or count == 0):
                 # BAD! We found a frame that failed to cluster properly...
+
+                #looks like this is the difference between score and score2? 
                 score = -np.inf
 
             # Minimum distance, weighted by average skeleton-pair confidence...
             if(count > 0):
                 score += min_dist * (total_conf / count)
                 score2 += min_dist * (total_conf / count)
+        
 
         # If skeleton is implemented...
         if (skeleton is not None):
             skel = skeleton
 
             for bp in range(len(frames)):
+
+                #what is this  ?
                 bp_group_off, bp_off = divmod(bp, num_outputs)
 
                 num_pairs = num_outputs * len(skel[bp_group_off])
                 f1_loc = cls.get_max_location(
                     frames[bp_group_off * num_outputs + bp_off], down_scaling
                 )
 
@@ -444,14 +484,15 @@
     ) -> np.ndarray:
         final_scores = np.zeros((len(frames), 2))
 
         if(progress_bar is not None):
             progress_bar.reset(len(frames))
 
         for i, frame in enumerate(frames):
+            #this will be a tuple of scores per frame 
             final_scores[i] = cls.compute_single_score(frame, num_outputs, down_scaling, skeleton, max_dist)
 
             if(progress_bar is not None):
                 progress_bar.update()
 
         return final_scores
 
@@ -459,14 +500,31 @@
     def compute_scores(
         cls,
         fb_data: ForwardBackwardData,
         prog_bar: ProgressBar,
         reset_bar: bool = False,
         thread_count: int = 0
     ) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Computes the scores for each frame in the ForwardBackwardData object.
+
+        This method calculates two scores for each frame based on the frame data provided. The scores are computed
+        by evaluating the frame against a set of criteria defined in the compute_single_score method. The scores
+        are intended to be used for determining the quality of the frame data and for further processing steps
+        such as segmentation.
+
+        Parameters:
+        - fb_data: ForwardBackwardData, the data containing frames to be scored.
+        - prog_bar: ProgressBar, a progress bar object for visual feedback during the scoring process.
+        - reset_bar: bool, a flag indicating whether to reset the progress bar before starting the scoring process.
+        - thread_count: int, the number of threads to use for parallel processing of the scoring.
+
+        Returns:
+        - Tuple[np.ndarray, np.ndarray], two arrays containing the computed scores for each frame.
+        """
         if("is_clustered" not in fb_data.metadata):
             raise PassOrderError(
                 "Clustering must be done before frame fixing!"
             )
 
         scores = np.zeros((fb_data.num_frames, 2))
```

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/mit_viterbi.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/mit_viterbi.py`

 * *Files 8% similar despite different names*

```diff
@@ -120,16 +120,16 @@
         self._skeleton_tables = None
 
     def _init_gaussian_table(self, metadata: AttributeDict):
         """
         Initialize the standard deviation and gaussian table.
 
         :param metadata: The metadata from the ForwardBackwardData object.
-                         Provides the optimized standard deviation if the
-                         standard_deviation is set to 'auto'.
+        Provides the optimized standard deviation if the
+        standard_deviation is set to 'auto'.
         """
         conf = self.config
         std = conf.standard_deviation
 
         if (std == "auto" and ("optimal_std" in metadata)):
             self._scaled_std = metadata.optimal_std[2]
         else:
@@ -195,72 +195,101 @@
                     ),
                     self.config.lowest_skeleton_score
                 )
         else:
             self.config.skeleton_weight = 0
 
     def _init_obscured_state(self, metadata: AttributeDict):
+        """Initialize probabilities relating to an obscured state"""
         metadata.obscured_prob = self.config.obscured_probability
         metadata.obscured_survival_max = self.config.obscured_survival_max
 
     def _init_edge_state(self, metadata: AttributeDict):
+        """Initialize probabilities relating to an edge / boundary state"""
         metadata.enter_prob = self.config.enter_state_probability
         metadata.enter_trans_prob = self.config.enter_state_exit_probability
 
     def run_pass(
         self,
         fb_data: ForwardBackwardData,
         prog_bar: Optional[ProgressBar] = None,
         in_place: bool = True,
         reset_bar: bool = True
     ) -> ForwardBackwardData:
         """
         This is the main function that orchestrates the forward and backward passes of the Viterbi algorithm. 
         It initializes the necessary tables and states, then runs the forward pass to calculate probabilities,
-        followed by a backtrace to determine the most probable paths."""
+        followed by a backtrace to determine the most probable paths.
+        
+        
+        fb_data: ForwardBackwardData object. I guess this comes from DLC or SLEAP (or i guess the edited data after supervision)
+
+        ****This is going to be for some segment of frames after segmentation with clustering 
+
+
+        The ForwardBackwardData object is a crucial component in the Viterbi algorithm's implementation for frame passes. It primarily contains the following:
+
+        - frames: A list of Frame objects, each representing a snapshot of the body parts' states at a specific time point. 
+        Each Frame object holds probabilities and other statistical data necessary for the forward and backward passes.
+        - metadata: An AttributeDict containing metadata related to the current processing, such as fixed_frame_index, 
+        obscured_probability, and other configuration parameters that influence the algorithm's behavior.
+        - num_frames: An integer representing the total number of frames to be processed.
+        - num_bodyparts: An integer indicating the number of body parts being tracked.
+
+        This object is typically generated as part of the preprocessing steps before running the Viterbi algorithm. 
+        It is constructed from the input data, which includes video frames, tracking configurations, 
+        and any precomputed probabilities or states necessary for the algorithm. 
+        The ForwardBackwardData object serves as a container for all the information needed to perform 
+        the forward and backward passes, facilitating the calculation of the most probable paths for body part movements across frames.
+        """
+
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore")
             if("fixed_frame_index" not in fb_data.metadata):
                 raise PassOrderError(f"Must run FixFrame before this pass!")
 
             self._init_gaussian_table(fb_data.metadata)
             self._init_skeleton(fb_data)
             self._init_obscured_state(fb_data.metadata)
             self._init_edge_state(fb_data.metadata)
 
-            fix_frame = fb_data.metadata.fixed_frame_index
+            #the index of the frame that marks the segment, in which animals are separable
+            fix_frame_index = fb_data.metadata.fixed_frame_index
 
             if(reset_bar and prog_bar is not None):
                 prog_bar.reset(fb_data.num_frames * 3)
 
             # Initialize fixed frame...
             if(not fb_data.metadata.get("is_pre_initialized", False)):
                 for bp_i in range(fb_data.num_bodyparts):
                     self._compute_init_frame(
-                        fb_data.frames[fb_data.metadata.fixed_frame_index][bp_i],
+                        fb_data.frames[fix_frame_index][bp_i],
                         fb_data.metadata
                     )
             else:
                 for bp_i in range(fb_data.num_bodyparts):
-                    frame = fb_data.frames[fb_data.metadata.fixed_frame_index][bp_i]
+                    frame = fb_data.frames[fix_frame_index][bp_i]
+                    #converting probabilities to log space 
                     frame.frame_probs = to_log_space(frame.frame_probs)
                     frame.occluded_probs = to_log_space(frame.occluded_probs)
                     frame.enter_state = to_log_space(frame.enter_state)
 
             fb_data = fb_data if(in_place) else fb_data.copy()
 
-            # Viterbi
-            super()._set_step_controls(fix_frame + 1, None, 1, -1)
+            # Viterbiwhi
+            super()._set_step_controls(fix_frame_index + 1, None, 1, -1) #starting from the frame after the fix_frame, going future
             self._run_forward(fb_data, prog_bar, True, False)
-            super()._set_step_controls(None, fix_frame, -1, 1)
+            super()._set_step_controls(None, fix_frame_index, -1, 1)
             self._run_backtrace(fb_data, prog_bar)
 
-            super()._set_step_controls(fix_frame - 1, None, -1, 1)
+
+            #TODO check if this is being run for any segment other than the first one
+            super()._set_step_controls(fix_frame_index - 1, None, -1, 1) #starting from the frame before the fix_frame, going past
             self._run_forward(fb_data, prog_bar, True, False)
-            super()._set_step_controls(None, fix_frame, 1, -1)
+            super()._set_step_controls(None, fix_frame_index, 1, -1)
             self._run_backtrace(fb_data, prog_bar)
 
             for f_i in range(fb_data.num_frames):
                 for bp_i in range(fb_data.num_bodyparts):
                     fix_frame = fb_data.frames[f_i][bp_i]
                     fix_frame.frame_probs = from_log_space(fix_frame.frame_probs)
                     fix_frame.occluded_probs = from_log_space(fix_frame.occluded_probs)
@@ -271,27 +300,38 @@
             return fb_data
 
     def _run_backtrace(
         self,
         fb_data: ForwardBackwardData,
         prog_bar: Optional[ProgressBar] = None,
     ) -> ForwardBackwardData:
+        
+        """
+        Executes the backtrace process for the Viterbi algorithm on the given data.
+
+        This method backtraces through the computed probabilities to determine the most likely path of states
+        that leads to the observed data. It utilizes the forward probabilities computed during the forward pass
+        and the transition probabilities to backtrack and identify the sequence of states that maximizes the
+        overall probability of the observed sequence.
+
+        Parameters:
+        - fb_data: ForwardBackwardData object containing the forward probabilities and other relevant data for backtracing.
+        - prog_bar: Optional ProgressBar instance for tracking progress of the backtrace operation.
+
+        Returns:
+        - ForwardBackwardData: The input data object updated with the backtraced path information.
+        """
         pool_cls = self._get_pool if(self.multi_threading_allowed and (fb_data.num_bodyparts // fb_data.metadata.num_outputs) > 2) else NotAPool
 
         backtrace_priors = [None for __ in range(fb_data.num_bodyparts)]
         backtrace_current = [None for __ in range(fb_data.num_bodyparts)]
 
         with pool_cls() as pool:
             exit_prob = fb_data.metadata.enter_trans_prob
             transition_function = ViterbiTransitionTable(self._gaussian_table, exit_prob, 1 - exit_prob)
-            resist_transition_func = (
-                ViterbiTransitionTable(self._gaussian_repel_table, exit_prob, 1 - exit_prob)
-                if (self._gaussian_repel_table is not None)
-                else None
-            )
 
             for frame_idx in RangeSlicer(fb_data.frames)[self._start:self._stop:self._step]:
                 if(not (0 <= (frame_idx + self._prior_off) < len(fb_data.frames))):
                     continue
 
                 # Compute the prior maximum locations for all body parts in
                 # the prior frame...
@@ -316,17 +356,19 @@
                     combined = np.asarray(combined)
 
                     prior_max_idxs = np.argmax(combined, axis=1)
                     max_of_maxes = np.argmax(
                         np.max(combined, axis=1))  # Is it in occluded or frame?
 
                     # If edge state is higher, select it over the actual frame coordinates...
+                    #TODO what is going on here
                     if(combined[max_of_maxes][prior_max_idxs[max_of_maxes]] < prior.enter_state):
                         prob, coords = prior.enter_state, [-np.inf, -np.inf]
                     else:
+                        #this is likely the general case 
                         prob = combined[max_of_maxes][prior_max_idxs[max_of_maxes]]
                         coords = combined_coords[max_of_maxes][prior_max_idxs[max_of_maxes]]
 
                     prior_data = [(
                         np.asarray([prob]),
                         np.asarray([coords]).T
                     )]
@@ -346,17 +388,15 @@
                     type(self)._compute_backtrace_step,
                     [(
                         backtrace_priors,
                         backtrace_current[bp_i],
                         bp_i,
                         fb_data.metadata,
                         transition_function,
-                        resist_transition_func,
                         self._skeleton_tables if (self.config.include_skeleton) else None,
-                        self.config.soft_domination_weight,
                         self.config.skeleton_weight
                     ) for bp_i in range(fb_data.num_bodyparts)]
                 )
 
                 # We stash the entire frame, the maximums are computed on
                 # the next step, and by the FramePassEngine at the end...
                 for bp_i, (frm_prob, occ_prob, enter_state) in enumerate(results):
@@ -391,33 +431,45 @@
     def _run_forward(
         self,
         fb_data: ForwardBackwardData,
         prog_bar: Optional[ProgressBar] = None,
         in_place: bool = True,
         reset_bar: bool = True
     ) -> ForwardBackwardData:
+        """
+        Executes the forward pass of the MIT Viterbi algorithm over the provided frame data.
+
+        This method orchestrates the forward pass computation by slicing the frame data according to the
+        configured step controls, setting up a multiprocessing pool if necessary, and applying the MIT Viterbi
+        algorithm to compute the probabilities and states for each body part in each frame. The results are
+        aggregated and updated in the provided ForwardBackwardData object.
+
+        Parameters:
+        - fb_data: ForwardBackwardData, the data structure containing frames and metadata for the forward-backward pass.
+        - prog_bar: Optional[ProgressBar], a progress bar object for visual feedback during processing (default is None).
+        - in_place: bool, flag indicating whether to update the fb_data object in place or to create a copy (default is True).
+        - reset_bar: bool, flag indicating whether to reset the progress bar if it is provided (default is True).
+
+        Returns:
+        - ForwardBackwardData: The updated data structure with computed probabilities and states for each frame.
+        """
         frame_iter = RangeSlicer(fb_data.frames)[self._start:self._stop:self._step]
         meta = fb_data.metadata
 
         fb_data = fb_data if(in_place) else fb_data.copy()
 
         if(prog_bar is not None and reset_bar):
             prog_bar.reset(total=fb_data.num_frames)
 
         # We only use a pool if the body part group is high enough...
         pool_cls = self._get_pool if(self.multi_threading_allowed and (fb_data.num_bodyparts // meta.num_outputs) > 2) else NotAPool
 
         with pool_cls() as pool:
             exit_prob = fb_data.metadata.enter_trans_prob
             transition_func = ViterbiTransitionTable(self._gaussian_table, exit_prob, 1 - exit_prob)
-            resist_transition_func = (
-                ViterbiTransitionTable(self._gaussian_repel_table, exit_prob, 1 - exit_prob)
-                if(self._gaussian_repel_table is not None)
-                else None
-            )
 
             for i in frame_iter:
                 prior_idx = i + self._prior_off
 
                 if (not (0 <= prior_idx < fb_data.num_frames)):
                     continue
                 prior = fb_data.frames[prior_idx]
@@ -428,17 +480,15 @@
                     MITViterbi._compute_normal_frame,
                     [(
                         prior,
                         current,
                         bp_grp_i,
                         meta,
                         transition_func,
-                        resist_transition_func,
                         self._skeleton_tables if (self.config.include_skeleton) else None,
-                        self.config.soft_domination_weight,
                         self.config.skeleton_weight
                     ) for bp_grp_i in range(fb_data.num_bodyparts // meta.num_outputs)]
                 )
 
                 for (bp_grp_i, res) in enumerate(results):
                     section = slice(bp_grp_i * meta.num_outputs, (bp_grp_i + 1) * meta.num_outputs)
                     current[section] = res[section]
@@ -454,17 +504,15 @@
     def _compute_backtrace_step(
         cls,
         prior: List[List[Tuple[np.ndarray, Tuple[np.ndarray, np.ndarray]]]],
         current: List[Tuple[np.ndarray, Tuple[np.ndarray, np.ndarray]]],
         bp_idx: int,
         metadata: AttributeDict,
         transition_function: TransitionFunction,
-        resist_transition_function: Optional[TransitionFunction] = None,
         skeleton_table: Optional[StorageGraph] = None,
-        soft_dom_weight: float = 0,
         skeleton_weight: float = 0
     ) -> List[np.ndarray]:
         """This method is responsible for computing the transition probabilities from the prior maximum locations 
         (highest probability states) of all body parts in the prior frame to the current frame's states. 
         It's where the algorithm determines the most probable path that leads to each pixel 
         in the current frame based on the accumulated probabilities from previous frames.
         
@@ -480,17 +528,14 @@
         bp_idx: The index of the body part being processed. This is used to identify which part of the data corresponds to the current body part in multi-body part tracking scenarios.
 
         metadata: The metadata from the ForwardBackwardData object. 
         An AttributeDict containing metadata that might be necessary for the computation, such as configuration parameters or additional data needed for probability calculations.
         
         transition_function:  A function or callable object that calculates the transition probabilities between states. This is crucial for determining how likely it is to move from one state to another.
 
-        resist_transition_function: A function or callable object that calculates the resistance to transitioning between states. 
-        Similar to transition_function, but used for calculating resistive transitions, which might be part of handling interactions between different tracked objects or body parts.
-
         skeleton_table: A StorageGraph object that stores the relationship between different body parts as defined in the skeleton data from the metadata.
         An optional parameter that, if provided, contains skeleton information that can be used to enhance the tracking by considering the structural relationships between different body parts.
 
         soft_dom_weight: A float representing the weight of the soft domination factor. 
 
         skeleton_weight: A float representing the weight of the skeleton factor.
 
@@ -503,27 +548,14 @@
             prior,
             current,
             bp_idx,
             metadata,
             skeleton_table
         )
 
-        #The method then calculates the effect of soft domination, 
-        # which is a technique used to handle the dominance relationship between different paths. 
-        # This step adjusts the probabilities to favor more likely paths and suppress less likely ones, 
-        # based on the configured soft domination weight.
-
-        from_soft_dom = cls._compute_soft_domination(
-            prior,
-            current,
-            bp_idx,
-            metadata,
-            resist_transition_function,
-        )
-
         #The core of the method involves calculating the transition probabilities from the prior states to the current states. 
         # This is done using the transition_function, which takes into account the distances between states and other factors 
         # to determine how likely it is to transition from one state to another.
         trans_res = cls.log_viterbi_between(
             current,
             prior[bp_idx],
             transition_function
@@ -533,28 +565,29 @@
         # and direct transitions are then combined to determine the overall probability of transitioning 
         # to each current state from the prior states. 
         # This involves weighting each component according to the configured weights and summing them up to get the final probabilities.
 
         #Normalization: Finally, the probabilities are normalized to ensure they are within a valid range 
         # and to facilitate comparison between different paths.
         return norm_together([
-            t + s * skeleton_weight + d * soft_dom_weight for t, s, d in zip(trans_res, skel_res, from_soft_dom)
+            t + s * skeleton_weight for t, s in zip(trans_res, skel_res)
         ])
 
     @classmethod
     def _compute_init_frame(
         cls,
         frame: ForwardBackwardFrame,
         metadata: AttributeDict
     ) -> ForwardBackwardFrame:
         y, x, probs, x_off, y_off = frame.src_data.unpack()
 
         if(y is None):
             print("Invalid frame to start on! Using enter state...")
             frame.enter_state = to_log_space(1)
+            #The enter_state is used when no good fix frame is found over the entire video (one where all parts are separable) the best scoring frame for the video (typically one with most parts separated) is picked and parts that weren't separated via clustering start in the enter state, which allows transitioning to the frame, but not back to the enter state
             frame.occluded_probs = to_log_space(np.array([0]))
             frame.occluded_coords = np.array([[0, 0]])
 
         # Occluded state for first frame...
         occ_coord = np.array([x, y]).T
         occ_probs = np.full(
             occ_coord.shape[0], to_log_space(metadata.obscured_prob)
@@ -607,14 +640,38 @@
         metadata: AttributeDict,
         skeleton_table: Optional[StorageGraph] = None,
         merge_arrays: Callable[[Iterable[np.ndarray]], np.ndarray] = np.maximum.reduce,
         merge_internal: Callable[[np.ndarray, int], np.ndarray] = np.max,
         merge_results: bool = True
     ) -> Union[List[Tuple[int, List[NumericArray]]], List[NumericArray]]:
         
+        """
+        Computes the transition probabilities between the prior and current data for a specific body part, 
+        considering the skeleton information, if available. This method integrates the transition probabilities 
+        from the prior state to the current state, leveraging the skeleton structure to inform the transition 
+        probabilities and ensure that the computed paths are anatomically plausible.
+
+        Parameters:
+        - prior: A union of lists containing either ForwardBackwardFrame objects or lists of tuples with numpy arrays 
+        and tuples of numpy arrays, representing the state of each body part in the previous frame.
+        - current_data: A list of tuples containing numpy arrays and tuples of numpy arrays, representing the current 
+                        state to be updated with new probabilities.
+        - bp_idx: An integer representing the index of the body part being processed.
+        - metadata: An AttributeDict containing configuration and metadata for the tracking process.
+        - skeleton_table: An optional StorageGraph containing skeleton information to inform tracking.
+        - merge_arrays: A callable that merges numpy arrays using a specified operation (e.g., np.maximum.reduce).
+        - merge_internal: A callable that merges internal numpy arrays using a specified operation (e.g., np.max).
+        - merge_results: A boolean indicating whether to merge the results into a single list or keep them separate.
+
+        Returns:
+        - A union of lists containing either tuples of integers and lists of NumericArray objects or lists of 
+          NumericArray objects, depending on the merge_results parameter. These lists represent the updated 
+          probabilities and states for the body part being processed.
+        """
+        
         #TODO: Add docstring and notes in coda
         if(skeleton_table is None):
             return [0] * len(current_data) if(merge_results) else []
 
         bp_group_idx = bp_idx // metadata.num_outputs
         bp_off = bp_idx % metadata.num_outputs
 
@@ -646,15 +703,15 @@
             transition_func = ViterbiTransitionTable(trans_table, 0.5, 0.5)
 
             results.append((
                 other_bp_group_idx * metadata.num_outputs + bp_off,
                 cls.log_viterbi_between(
                     current_data,
                     prior_data,
-                    transition_func,
+                    transition_func, #the skeleton data is likely incorporated in this transition function 
                     merge_arrays,
                     merge_internal
                 )
             ))
 
         if(not merge_results):
             return results
@@ -666,163 +723,72 @@
                 merged_result = current_total + bp_sub_res
                 final_result[i] = merged_result
 
             final_result = norm_together(final_result)
 
         return final_result
 
-    @classmethod
-    def _compute_soft_domination(
-        cls,
-        prior: Union[List[ForwardBackwardFrame], List[List[Tuple[np.ndarray, Tuple[np.ndarray, np.ndarray]]]]],
-        current_data: List[Tuple[np.ndarray, Tuple[np.ndarray, np.ndarray]]],
-        bp_idx: int,
-        metadata: AttributeDict,
-        transition_func: Optional[TransitionFunction] = None,
-        merge_arrays: Callable[[Iterable[np.ndarray]], np.ndarray] = np.maximum.reduce,
-        merge_internal: Callable[[np.ndarray, int], np.ndarray] = np.max,
-        merge_results: bool = True
-    ) -> Union[List[Tuple[int, List[NumericArray]]], List[NumericArray]]:
-        """
-        Computes the soft domination for a given body part across frames, considering prior and current data.
-
-        This method calculates the soft domination values by comparing the probabilities of a body part being in
-        a certain state in the current frame against its probabilities in the prior frames. It uses a transition
-        function to determine the likelihood of transitioning from each state in the prior frames to each state in
-        the current frame. The results are merged using specified merging functions to find the most probable state
-        transitions. This method can optionally merge the results across all body parts to find the overall most
-        probable states.
-
-        Parameters:
-        - prior: Union[List[ForwardBackwardFrame], List[List[Tuple[np.ndarray, Tuple[np.ndarray, np.ndarray]]]]]
-                 The prior frame data or computed probabilities and coordinates for each body part.
-        - current_data: List[Tuple[np.ndarray, Tuple[np.ndarray, np.ndarray]]]
-                        The current frame data including probabilities and coordinates for each body part.
-        - bp_idx: int
-                  The index of the body part being processed.
-        - metadata: AttributeDict
-                    Metadata containing configuration and state information for the current processing.
-        - transition_func: Optional[TransitionFunction]
-                           The function used to compute the transition probabilities between states.
-        - merge_arrays: Callable[[Iterable[np.ndarray]], np.ndarray]
-                        A function to merge arrays of probabilities from different transitions.
-        - merge_internal: Callable[[np.ndarray, int], np.ndarray]
-                          A function to merge probabilities within a single transition.
-        - merge_results: bool
-                         A flag indicating whether to merge the results across all body parts.
-
-        Returns:
-        - Union[List[Tuple[int, List[NumericArray]]], List[NumericArray]]:
-          The computed soft domination values for the specified body part, either as a list of numeric arrays
-          (if merge_results is False) or as a list of tuples containing the body part index and the list of
-          numeric arrays (if merge_results is True).
-
-        This method is crucial for optimizing the Viterbi path selection by considering not only the most probable
-        paths but also how these paths compare when considering potential transitions from prior states. It helps
-        in refining the selection of paths that are not only probable in isolation but also in the context of the
-        sequence of frames being analyzed.
-        """
-        if(transition_func is None or metadata.num_outputs <= 1):
-            return [0] * len(current_data) if(merge_results) else []
-
-        bp_group_idx = bp_idx // metadata.num_outputs
-
-        results = []
-        final_result = [0] * len(current_data)
-
-        for other_idx in range(bp_group_idx * metadata.num_outputs, (bp_group_idx + 1) * metadata.num_outputs):
-            if(other_idx == bp_idx):
-                continue
-
-            # Grab the prior frame...
-            prior_frame = prior[other_idx]
-            if(isinstance(prior_frame, ForwardBackwardFrame)):
-                py, px, __, __, __ = prior_frame.src_data.unpack()
-
-                # If wasn't found, don't include in the result.
-                if(prior_frame.frame_probs is None):
-                    continue
-
-                z_a = lambda: np.array([0])
-                nf_a = lambda: np.array([-np.inf])
-
-                prior_data = [
-                    (prior_frame.frame_probs, (px, py) if(py is not None) else (z_a(), z_a())),
-                    (prior_frame.occluded_probs, prior_frame.occluded_coords.T),
-                    (np.array([prior_frame.enter_state]), (nf_a(), nf_a()))
-                ]
-            else:
-                prior_data = prior_frame
-
-            results.append((
-                other_idx,
-                # Find the best paths from other parts, then take the complement. This optimizes for avoiding
-                # paths from other parts....
-                [log_prob_complement(v) for v in cls.log_viterbi_between(
-                    current_data,
-                    prior_data,
-                    transition_func,
-                    merge_arrays,
-                    merge_internal
-                )]
-            ))
-
-        if(not merge_results):
-            return results
-
-        for __, bp_res in results:
-            for i, (current_total, bp_sub_res) in enumerate(zip(final_result, bp_res)):
-                merged_result = current_total + bp_sub_res
-                if(np.all(np.isneginf(merged_result))):
-                    continue
-                final_result[i] = merged_result
-
-            final_result = norm_together(final_result)
-
-        return final_result
 
     @classmethod
     def _compute_normal_frame(
         cls,
         prior: List[ForwardBackwardFrame],
         current: List[ForwardBackwardFrame],
         bp_group: int,
         metadata: AttributeDict,
         transition_function: TransitionFunction,
-        resist_transition_function: Optional[TransitionFunction] = None,
         skeleton_table: Optional[StorageGraph] = None,
-        soft_dom_weight: float = 0,
         skeleton_weight: float = 0
     ) -> List[ForwardBackwardFrame]:
         
         """processes a single frame in the context of tracking multiple body parts or individuals, 
         calculating the probabilities of each body part being in each position based on prior information, 
         current observations, and various transition models.
         It integrates several key concepts, including handling occlusions, leveraging skeleton information, 
-        and applying soft domination to refine the tracking process."""
+        and applying soft domination to refine the tracking process.
+        
+        
+        prior: A list of ForwardBackwardFrame objects representing the state of each body part in the previous frame.
+
+        current: A list of ForwardBackwardFrame objects representing the current state to be updated with new probabilities.
+
+        bp_group: The index of the body part group being processed. This will be all the instances of some particular body part in the frame
+
+        metadata: An AttributeDict containing configuration and metadata for the tracking process.
+
+        transition_function: A callable that computes transition probabilities between states.
+
+        skeleton_table: Optional data structure containing skeleton information to inform tracking.
+
+        """
+
         group_range = range(
             bp_group * metadata.num_outputs,
             (bp_group + 1) * metadata.num_outputs
         )
 
         results = []
         result_coords = []
 
         # Looks like normal viterbi until domination step...
+        # iterates through each body part within the specified group, unpacking prior and current state information.
+
         for bp_i in group_range:
+            #the source data from deep lab cut or sleap
             py, px, pprob, p_occx, p_occy = prior[bp_i].src_data.unpack()
             cy, cx, cprob, c_occx, c_occy = current[bp_i].src_data.unpack()
 
             if((cprob is not None) and np.all(cprob <= 0)):
                 current[bp_i].src_data = SparseTrackingData()
                 cy = cx = cprob = None
 
             z_arr = lambda: np.array([0])
             neg_inf_arr = lambda: np.array([-np.inf])
 
+            #the data from running viterbi on the previous frame
             prior_data = [
                 (
                     prior[bp_i].frame_probs if(py is not None) else neg_inf_arr(),
                     (px, py) if(py is not None) else (z_arr(), z_arr())
                 ),
                 (
                     prior[bp_i].occluded_probs,
@@ -830,64 +796,70 @@
                 ),
                 (
                     np.array([prior[bp_i].enter_state]),
                     (neg_inf_arr(), neg_inf_arr())
                 )
             ]
 
+            #only have source data for the current frame
             c_frame_data = (
                 (norm(to_log_space(cprob)), (cx, cy))
                 if(cy is not None) else (to_log_space(z_arr()), (z_arr(), z_arr()))
             )
 
+            #occluded coordinates are constrained by the coordinate probabilities in the previous frame 
             c_occ_coords, c_occ_probs = cls.generate_occluded(
                 np.asarray(c_frame_data[1]).T,
                 prior[bp_i].occluded_coords,
-                metadata.obscured_prob,
+                metadata.obscured_prob, #obscured = occluded
                 current[bp_i].disable_occluded and (cy is not None)
             )
 
             current[bp_i].occluded_coords = c_occ_coords
 
             current_data = [
                 c_frame_data,
                 (c_occ_probs, c_occ_coords.T),
                 (np.array([to_log_space(metadata.enter_prob)]), (neg_inf_arr(), neg_inf_arr()))
             ]
 
+            #the skeleton_table has transition functions for each pair of body parts 
+            #we use those functions to calculate the transition probabilities between the prior and current states for each body part
+            #having incorporated information about how likely body parts are to be in some range of each other
             from_skel = cls._compute_from_skeleton(
                 prior,
                 current_data,
                 bp_i,
                 metadata,
                 skeleton_table
             )
 
-            from_soft_dom = cls._compute_soft_domination(
-                prior,
-                current_data,
-                bp_i,
-                metadata,
-                resist_transition_function,
-            )
-
             from_transition = cls.log_viterbi_between(
                 current_data,
                 prior_data,
                 transition_function
             )
 
             results.append([
-                t + s * skeleton_weight + d * soft_dom_weight
-                for t, s, d in zip(from_transition, from_skel, from_soft_dom)
+                t + s * skeleton_weight 
+                for t, s in zip(from_transition, from_skel)
             ])
 
             # Result coordinates, exclude the enter state...
             result_coords.append([c[1] for c in current_data[:-1]])
 
+            #TODO i want the coordinates of the source of each pixel in the current frame
+            #which would be the coordinate that has the highest transition probability
+            # source_coords = []*len(c_frame_data[:-1])
+            # for i, c in enumerate(current_data[:-1]):
+            #     if(np.all(np.isneginf(results[-1][i]))):
+            #         continue
+            #     best = np.argmax(results[-1][i])
+            #     source_coords[i] = c[1][best]
+
         # Pad all arrays so we can do element-wise comparisons between them...
         frm_probs, frm_coords, frm_idxs = arr_utils.pad_coordinates_and_probs(
             [r[0] for r in results],
             [np.asarray(r[0]).T for r in result_coords],
             -np.inf
         )
         occ_probs, occ_coords, occ_idxs = arr_utils.pad_coordinates_and_probs(
@@ -919,14 +891,21 @@
                 occ_dominators[best_occ] = 0  # Don't allow anyone else to take this spot.
 
             norm_val = np.nanmax([np.nanmax(frm_prob), np.nanmax(occ_prob), enter_prob])
 
             # Store the results...
             # Store the results...
             current[bp_i].frame_probs = frm_prob[frm_idx] - norm_val
+
+            #TODO 
+            #also store a mirror matrix for each coordinate, the source of that pixel in the preceding frame 
+            #which would be the coordinate that has the highest transition probability 
+
+
+
             # Filter occluded probabilities...
             c, p = cls.filter_occluded_probabilities(
                 current[bp_i].occluded_coords,
                 occ_prob[occ_idx],
                 metadata.obscured_survival_max
             )
             current[bp_i].occluded_coords = c
```

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/frame_passes/optimize_std.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/frame_passes/optimize_std.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/skeleton_structures.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/skeleton_structures.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/fpe/sparse_storage.py` & `diplomat_track-0.1.2/diplomat/predictors/fpe/sparse_storage.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/frame_exporter.py` & `diplomat_track-0.1.2/diplomat/predictors/frame_exporter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/plotter.py` & `diplomat_track-0.1.2/diplomat/predictors/plotter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/sfpe/assignment.py` & `diplomat_track-0.1.2/diplomat/predictors/sfpe/assignment.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/sfpe/avl_tree.py` & `diplomat_track-0.1.2/diplomat/predictors/sfpe/avl_tree.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/sfpe/disk_sparse_storage.py` & `diplomat_track-0.1.2/diplomat/predictors/sfpe/disk_sparse_storage.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/sfpe/file_io.py` & `diplomat_track-0.1.2/diplomat/predictors/sfpe/file_io.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/sfpe/growable_numpy_array.py` & `diplomat_track-0.1.2/diplomat/predictors/sfpe/growable_numpy_array.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/sfpe/segmentation.py` & `diplomat_track-0.1.2/diplomat/predictors/sfpe/segmentation.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/sfpe/segmented_frame_pass_engine.py` & `diplomat_track-0.1.2/diplomat/predictors/sfpe/segmented_frame_pass_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -449,14 +449,24 @@
         self._segment_bp_order = None
 
         self._restore_path = restore_path
 
         self._current_frame = 0
 
     def get_frame_holder(self):
+        """
+        Retrieves the frame holder object that manages frame data storage and access.
+
+        This method initializes and returns a DiskBackedForwardBackwardData object, which is responsible for holding
+        the frames data. It sets up the necessary file object, shared memory, and manager for inter-process communication
+        and data sharing. It also copies the original video data into a disk file for processing.
+
+        Returns:
+            DiskBackedForwardBackwardData: An object that holds and manages access to the frames data.
+        """
         output_path = Path(self.video_metadata["output-file-path"]).resolve()
         video_path = Path(self.video_metadata["orig-video-path"]).resolve()
         disk_path = output_path.parent / (output_path.stem + ".dipui")
 
         self._file_obj = disk_path.open("w+b")
 
         with video_path.open("rb") as f:
@@ -476,14 +486,22 @@
             lock=self._manager.RLock(),
             memory_backing=self._shared_memory
         )
 
         return _frame_holder
 
     def _open(self):
+        """
+        Opens the necessary resources and prepares the frame holder for processing.
+
+        This method is responsible for setting up the frame holder based on the specified storage mode in the settings.
+        If a restore path is provided, it initializes the frame holder with the data from the specified path. Otherwise,
+        it creates a new frame holder based on the current settings, which could be in-memory, disk-backed, or a hybrid
+        of both. It also initializes segments and segment scores if they are available in the frame holder's metadata.
+        """
         if(self._restore_path is not None):
             # Ignore everything else,
             self._restore_path = Path(self._restore_path).resolve()
             self.video_metadata["orig-video-path"] = self._restore_path
             orig_ext = Path(self.video_metadata["output-file-path"]).suffix
             self.video_metadata["output-file-path"] = self._restore_path.parent / (self._restore_path.stem + orig_ext)
             self.settings.storage_mode = "disk"
@@ -515,37 +533,71 @@
         self._frame_holder.metadata.video_metadata = dict(self.video_metadata)
         self._frame_holder.metadata.threshold = self.THRESHOLD
         self._frame_holder.metadata.bodyparts = self.bodyparts
         self._frame_holder.metadata.num_outputs = self.num_outputs
         self._frame_holder.metadata.project_skeleton = self.video_metadata.get("skeleton", None)
 
     def _close(self):
+        """
+        Closes all resources associated with the frame holder.
+
+        This method ensures that all resources such as file objects, shared memory, and the manager used for inter-process
+        communication are properly closed and, if applicable, unlinked. It is crucial for preventing resource leaks and ensuring
+        that the system resources are released back to the operating system. This method should be called when the frame holder
+        is no longer needed, typically at the end of processing or when an exception occurs.
+        """
         if(isinstance(self._frame_holder, DiskBackedForwardBackwardData)):
             self._frame_holder.close()
         if(self._file_obj is not None):
             self._file_obj.close()
         if(self._shared_memory is not None and hasattr(self._shared_memory, "close")):
             self._shared_memory.close()
             if(hasattr(self._shared_memory, "unlink")):
                 self._shared_memory.unlink()
         if(self._manager is not None):
             self._manager.shutdown()
 
     def _sparcify_and_store(self, fb_frame: ForwardBackwardFrame, scmap: TrackingData, frame_idx: int, bp_idx: int):
+        """
+        Sparsifies and stores the tracking data for a given frame and body part index.
+
+        This method takes the dense tracking data for a specific frame and body part index, sparsifies it according to the
+        threshold and maximum cells per frame settings, and then stores the sparsified data back into the frame. This process
+        helps in reducing the memory footprint and computational complexity for subsequent processing steps.
+
+        Parameters:
+            fb_frame (ForwardBackwardFrame): The frame object where the sparsified data will be stored.
+            scmap (TrackingData): The dense tracking data for the frame.
+            frame_idx (int): The index of the frame being processed.
+            bp_idx (int): The index of the body part being processed.
+        """
         fb_frame.orig_data = SparseTrackingData.sparsify(
             scmap,
             frame_idx,
             bp_idx,
             self.THRESHOLD,
             self.settings.max_cells_per_frame,
             SparseTrackingData.SparseModes[self.settings.sparsification_mode]
         )
         fb_frame.src_data = fb_frame.orig_data
 
     def _on_frames(self, scmap: TrackingData) -> Optional[Pose]:
+        """
+        Processes tracking data for each frame and updates the frame holder with sparsified data.
+
+        This method iterates through each frame provided by the tracking data, processes it by sparsifying
+        the tracking data for each body part, and updates the frame holder with the processed data. It ensures
+        that the metadata for width, height, and downscaling factor are updated based on the tracking data.
+
+        Parameters:
+            scmap (TrackingData): The tracking data containing dense tracking information for each frame.
+
+        Returns:
+            None: This method updates the frame holder in-place and does not return any value.
+        """
         if(self._width is None):
             self._width = scmap.get_frame_width()
             self._height = scmap.get_frame_height()
             self._frame_holder.metadata.down_scaling = scmap.get_down_scaling()
             self._frame_holder.metadata.width = scmap.get_frame_width()
             self._frame_holder.metadata.height = scmap.get_frame_height()
 
@@ -706,14 +758,30 @@
                 True
             )
 
     def _get_thread_count(self) -> int:
         return os.cpu_count() if(self.settings.thread_count is None) else self.settings.thread_count
 
     def _build_segments(self, progress_bar: Optional[ProgressBar], reset_bar: bool = True):
+        """
+        Builds segments for frame processing based on the current settings and progress bar status.
+
+        This method computes the scores for each frame using the current frame holder data and then segments
+        the frames based on these scores. The segments are determined using the EndPointSegmentor, which
+        optimizes the segments based on the computed scores and the specified segment size in the settings.
+
+        If the progress bar is enabled and the reset_bar flag is set to True, the progress bar is reset and
+        updated with messages reflecting the current stage of the segmentation process.
+
+        Parameters:
+        - progress_bar: Optional[ProgressBar], a progress bar instance for visual feedback.
+        - reset_bar: bool, a flag indicating whether to reset the progress bar at the beginning of the process.
+
+        The method updates the internal state with the computed segments and their corresponding scores.
+        """
         # Compute the scores...
         if(reset_bar and progress_bar is not None):
             progress_bar.message("Computing frame pose scores...")
             progress_bar.reset(self.num_frames)
 
         segment_size = self.settings.segment_size
 
@@ -865,14 +933,51 @@
         self._frame_holder.frames[start:end] = frame_data.frames
 
     def _iter_run_levels(
         self,
         segment_idxs: np.ndarray,
         run_level_data: Optional[Tuple[np.ndarray, np.ndarray, int]]
     ) -> Iterable[Tuple[bool, Sequence[int]]]:
+        """
+        Determines what segments should be run next 
+        For example if you have a segment without any fixed frames (frames with good separation, all segments are at most 200 frames)
+        It tries to always put the fixed frame at the beginning of the segment 
+        
+        Any segment that does have a fixed frame is returned immediately 
+
+        Then you have to do special logic for all of the segments where there is not a fixed frame 
+
+        Whcih is : take the nearest good segment (rightmost) and include the first frame into the given bad segment
+        and continue Viterbi from that good segment 
+
+        but you can only do that for the bad segment that is closest to a good segmentxxw
+        so you kind of have to run viterbi in 'tiers'
+        you run all of the ones that you can run, yield, and then you'll have updated the ones that are 'good' and then you rerun it 
+
+
+
+        Iterates through segments to run levels of processing based on the provided segment indices and run level data.
+
+        This method determines the correct order to run segments in. 
+        If a segment has no good fix frames in it (full separation of parts), instead of picking a poor fix frame 
+        the Viterbi will run for a neighboring good segment first, and then stitch across to the bad segment 
+        by just continuing the Viterbi from the good segment. This can happen recursively, 
+        to allow for long viterbi runs through difficult segments. 
+        
+        This figures out what segments can be run in parallel next, and what segments still have dependencies on other segments.
+
+        Parameters:
+        - segment_idxs: np.ndarray, an array of segment indices that are to be processed.
+        - run_level_data: Optional[Tuple[np.ndarray, np.ndarray, int]], a tuple containing arrays of level values and booleans indicating if a segment
+          is before the fixed frame, along with the maximum level value. If None, default values are used.
+
+        Yields:
+        - Tuple[bool, Sequence[int]], a tuple where the first element is a boolean indicating if the segment is before the fixed frame, and the second
+          element is a sequence of segment indices to be processed at the current level.
+        """
         segment_idxs = np.asarray(segment_idxs)
 
         if(run_level_data is None):
             d = np.zeros(len(segment_idxs), int)
             run_level_data = (d, d, 0)
 
         level_vals, is_before, max_levels = run_level_data
```

### Comparing `diplomat_track-0.1.1/diplomat/predictors/supervised_fpe/labelers.py` & `diplomat_track-0.1.2/diplomat/predictors/supervised_fpe/labelers.py`

 * *Files 10% similar despite different names*

```diff
@@ -271,14 +271,32 @@
             *self._frame_engine.get_maximum_with_defaults(temp_f),
             meta.down_scaling
         )
 
         return ((frame_idx, bp_idx, temp_f, (x, y)), (x, y, prob))
 
     def pose_change(self, new_state: Any) -> Any:
+        """
+        Handles the change in pose by updating the frame data with the new state.
+
+        This method is responsible for updating the frame data when there is a change in the pose. It checks if the
+        frame and body part index combination (frm, bp) has already been modified. If not, it marks the original frame
+        data for this combination as changed. Depending on whether a suggested frame is provided or not, it either
+        creates new tracking data from the suggested frame or from the provided coordinates. This new data is then
+        used to update the frame data for the given frame and body part index. The method returns a tuple containing
+        the frame index, body part index, a flag indicating if the original data was modified, and the old frame data.
+
+        Parameters:
+        - new_state (Any): A tuple containing the frame index, body part index, an optional suggested frame, and
+          coordinates. The suggested frame is None if not provided.
+
+        Returns:
+        - Tuple[Any, Any, bool, Any]: A tuple containing the frame index, body part index, a boolean indicating if the
+          original data was modified (is_orig), and the old frame data before the change.
+        """
         frm, bp, suggested_frame, coord = new_state
         changed_frames = self._frame_engine.changed_frames
         frames = self._frame_engine.frame_data.frames
 
         old_frame_data = frames[frm][bp]
         is_orig = False
```

### Comparing `diplomat_track-0.1.1/diplomat/predictors/supervised_fpe/scorers.py` & `diplomat_track-0.1.2/diplomat/predictors/supervised_fpe/scorers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py` & `diplomat_track-0.1.2/diplomat/predictors/supervised_fpe/supervised_frame_pass_engine.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py` & `diplomat_track-0.1.2/diplomat/predictors/supervised_sfpe/supervised_segmented_frame_pass_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -515,20 +515,14 @@
         changed_frames: Dict[Tuple[int, int], ForwardBackwardFrame],
         old_poses: Pose,
         progress_bar: ProgressBar
     ) -> Tuple[Pose, Iterable[int]]:
         
         #TODO : delete below lines, not doing as expected
         
-        # # For each changed frame and each body part, take the maximum probability coordinates and set them to one
-        # for (frame_idx, bp_idx), frame in changed_frames.items():
-        #     max_prob_coord = np.unravel_index(frame.frame_probs.argmax(), frame.frame_probs.shape)
-        #     new_frame_probs = np.zeros_like(frame.frame_probs) #copy because this is read only
-        #     new_frame_probs[max_prob_coord] = 1
-        #     frame.frame_probs = new_frame_probs
         # Determine what segments have been manipulated...
         segment_indexes = sorted({np.searchsorted(self._segments[:, 1], f_i, "right") for f_i, b_i in changed_frames})
 
         poses = old_poses.get_all().reshape((old_poses.get_frame_count(), old_poses.get_bodypart_count(), 3))
         # Restore poses to there original order....
         for (s_i, e_i, f_i), seg_rev in zip(self._segments, self._reverse_segment_bp_order):
             poses[s_i:e_i, :] = poses[s_i:e_i, seg_rev]
```

### Comparing `diplomat_track-0.1.1/diplomat/processing/__init__.py` & `diplomat_track-0.1.2/diplomat/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/processing/containers.py` & `diplomat_track-0.1.2/diplomat/processing/containers.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/processing/pose.py` & `diplomat_track-0.1.2/diplomat/processing/pose.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/processing/predictor.py` & `diplomat_track-0.1.2/diplomat/processing/predictor.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/processing/progress_bar.py` & `diplomat_track-0.1.2/diplomat/processing/progress_bar.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/processing/track_data.py` & `diplomat_track-0.1.2/diplomat/processing/track_data.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/processing/type_casters.py` & `diplomat_track-0.1.2/diplomat/processing/type_casters.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/_function_tools.py` & `diplomat_track-0.1.2/diplomat/utils/_function_tools.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/cli_tools.py` & `diplomat_track-0.1.2/diplomat/utils/cli_tools.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/colormaps.py` & `diplomat_track-0.1.2/diplomat/utils/colormaps.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/extract_frames.py` & `diplomat_track-0.1.2/diplomat/utils/extract_frames.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/frame_store_api.py` & `diplomat_track-0.1.2/diplomat/utils/frame_store_api.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/frame_store_fmt.py` & `diplomat_track-0.1.2/diplomat/utils/frame_store_fmt.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/graph_ops.py` & `diplomat_track-0.1.2/diplomat/utils/graph_ops.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/lazy_import.py` & `diplomat_track-0.1.2/diplomat/utils/lazy_import.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/pluginloader.py` & `diplomat_track-0.1.2/diplomat/utils/pluginloader.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/pretty_printer.py` & `diplomat_track-0.1.2/diplomat/utils/pretty_printer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/shapes.py` & `diplomat_track-0.1.2/diplomat/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/track_formats.py` & `diplomat_track-0.1.2/diplomat/utils/track_formats.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/tweak_ui.py` & `diplomat_track-0.1.2/diplomat/utils/tweak_ui.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/video_info.py` & `diplomat_track-0.1.2/diplomat/utils/video_info.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/video_io.py` & `diplomat_track-0.1.2/diplomat/utils/video_io.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/utils/video_splitter.py` & `diplomat_track-0.1.2/diplomat/utils/video_splitter.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/fpe_editor.py` & `diplomat_track-0.1.2/diplomat/wx_gui/fpe_editor.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/helpdialog.py` & `diplomat_track-0.1.2/diplomat/wx_gui/helpdialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/icons.py` & `diplomat_track-0.1.2/diplomat/wx_gui/icons.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/id_swap_dialog.py` & `diplomat_track-0.1.2/diplomat/wx_gui/id_swap_dialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/identity_swapper.py` & `diplomat_track-0.1.2/diplomat/wx_gui/identity_swapper.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/labeler_lib.py` & `diplomat_track-0.1.2/diplomat/wx_gui/labeler_lib.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/point_edit.py` & `diplomat_track-0.1.2/diplomat/wx_gui/point_edit.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/probability_displayer.py` & `diplomat_track-0.1.2/diplomat/wx_gui/probability_displayer.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/progress_bar.py` & `diplomat_track-0.1.2/diplomat/wx_gui/progress_bar.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/progress_dialog.py` & `diplomat_track-0.1.2/diplomat/wx_gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/score_lib.py` & `diplomat_track-0.1.2/diplomat/wx_gui/score_lib.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/scroll_image_list.py` & `diplomat_track-0.1.2/diplomat/wx_gui/scroll_image_list.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/settings_dialog.py` & `diplomat_track-0.1.2/diplomat/wx_gui/settings_dialog.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/diplomat/wx_gui/video_player.py` & `diplomat_track-0.1.2/diplomat/wx_gui/video_player.py`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/pyproject.toml` & `diplomat_track-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `diplomat_track-0.1.1/PKG-INFO` & `diplomat_track-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diplomat-track
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool providing multi-animal tracking capabilities on top of other Deep learning based tracking software.
 Author-email: Isaac Robinson <isaac.k.robinson2000@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 Provides-Extra: gui
 Provides-Extra: sleap
 
 # DIPLOMAT
 
 Deep learning-based Identity Preserving Labeled-Object Multi-Animal Tracking.
 
-**NOTE:** DIPLOMAT is currently alpha software, there may be minor bugs and issues.
+**NOTE:** DIPLOMAT is currently alpha software, there may be minor bugs and usability issues.
 
 ## About
 
 DIPLOMAT provides algorithms and tools for performing multi-animal identity preserving tracking on top of single animal and multi animal CNN based tracking packages. Currently, it supports running on both DeepLabCut and SLEAP projects.
 Unlike other multi-animal tracking packages, DIPLOMAT's algorithms work directly off confidence maps instead of running peak detection, allowing for more nuanced tracking results compared to other methods. 
 
 https://github.com/TravisWheelerLab/DIPLOMAT/assets/47544550/d805b673-4678-4297-b288-3fd08ad3cf62
```

