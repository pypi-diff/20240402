# Comparing `tmp/onvif-gui-2.0.1.tar.gz` & `tmp/onvif-gui-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-2.0.1.tar", last modified: Fri Mar 29 01:54:08 2024, max compression
+gzip compressed data, was "onvif-gui-2.0.9.tar", last modified: Tue Apr  2 04:00:29 2024, max compression
```

## Comparing `onvif-gui-2.0.1.tar` & `onvif-gui-2.0.9.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.640648 onvif-gui-2.0.1/
--rw-rw-rw-   0        0        0    11558 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      221 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2410 2024-03-29 01:54:08.639692 onvif-gui-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1515 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.288542 onvif-gui-2.0.1/gui/
--rw-rw-rw-   0        0        0       28 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.335037 onvif-gui-2.0.1/gui/components/
--rw-rw-rw-   0        0        0      325 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/components/__init__.py
--rw-rw-rw-   0        0        0     1833 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/components/comboselector.py
--rw-rw-rw-   0        0        0     2693 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/components/directoryselector.py
--rw-rw-rw-   0        0        0     2429 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/components/fileselector.py
--rw-rw-rw-   0        0        0     4165 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/components/progress.py
--rw-rw-rw-   0        0        0     8691 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/components/target.py
--rw-rw-rw-   0        0        0     2723 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/components/thresholdslider.py
--rw-rw-rw-   0        0        0     3023 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/components/warningbar.py
--rw-rw-rw-   0        0        0    14860 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/glwidget.py
--rw-rw-rw-   0        0        0    37632 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/main.py
--rw-rw-rw-   0        0        0     9803 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/manager.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.382734 onvif-gui-2.0.1/gui/onvif/
--rw-rw-rw-   0        0        0      269 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/onvif/__init__.py
--rw-rw-rw-   0        0        0     9269 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/onvif/datastructures.py
--rw-rw-rw-   0        0        0     4012 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/onvif/imagetab.py
--rw-rw-rw-   0        0        0     2573 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/onvif/logindialog.py
--rw-rw-rw-   0        0        0     4928 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/onvif/networktab.py
--rw-rw-rw-   0        0        0     4990 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/onvif/ptztab.py
--rw-rw-rw-   0        0        0    13341 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/onvif/systemtab.py
--rw-rw-rw-   0        0        0    18638 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/onvif/videotab.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.420237 onvif-gui-2.0.1/gui/panels/
--rw-rw-rw-   0        0        0      184 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/panels/__init__.py
--rw-rw-rw-   0        0        0     3757 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/panels/audiopanel.py
--rw-rw-rw-   0        0        0    30511 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/panels/camerapanel.py
--rw-rw-rw-   0        0        0    25884 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/panels/filepanel.py
--rw-rw-rw-   0        0        0    26378 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/panels/settingspanel.py
--rw-rw-rw-   0        0        0     4718 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/panels/videopanel.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.526644 onvif-gui-2.0.1/gui/resources/
--rw-rw-rw-   0        0        0     2021 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/LICENSE
--rw-rw-rw-   0        0        0        0 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/__init__.py
--rw-rw-rw-   0        0        0      435 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/alarm_plain.png
--rw-rw-rw-   0        0        0      543 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/alarm_recording.gif
--rw-rw-rw-   0        0        0      256 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/apply.png
--rw-rw-rw-   0        0        0      267 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/apply_hi.png
--rw-rw-rw-   0        0        0      262 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/apply_lo.png
--rw-rw-rw-   0        0        0      911 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/audio.png
--rw-rw-rw-   0        0        0      536 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/audio_hi.png
--rw-rw-rw-   0        0        0      920 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/audio_lo.png
--rw-rw-rw-   0        0        0      203 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/branch_closed.png
--rw-rw-rw-   0        0        0      219 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/branch_closed_hi.png
--rw-rw-rw-   0        0        0      211 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/branch_closed_lo.png
--rw-rw-rw-   0        0        0      199 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/branch_open.png
--rw-rw-rw-   0        0        0      168 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/branch_open_hi.png
--rw-rw-rw-   0        0        0      172 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/branch_open_lo.png
--rw-rw-rw-   0        0        0      267 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/checked.png
--rw-rw-rw-   0        0        0      235 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/checked_hi.png
--rw-rw-rw-   0        0        0      246 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/checked_lo.png
--rw-rw-rw-   0        0        0    14172 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/darkstyle.qss
--rw-rw-rw-   0        0        0      910 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/discover.png
--rw-rw-rw-   0        0        0      849 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/discover_hi.png
--rw-rw-rw-   0        0        0      937 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/discover_lo.png
--rw-rw-rw-   0        0        0    75360 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/drops.mp3
--rw-rw-rw-   0        0        0      425 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/fast-forward.png
--rw-rw-rw-   0        0        0      253 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/fast-forward_hi.png
--rw-rw-rw-   0        0        0      433 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/fast-forward_lo.png
--rw-rw-rw-   0        0        0     4675 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/idle_lo.png
--rw-rw-rw-   0        0        0    29256 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/loud.mp3
--rw-rw-rw-   0        0        0      641 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/mute.png
--rw-rw-rw-   0        0        0      346 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/mute_hi.png
--rw-rw-rw-   0        0        0      618 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/mute_lo.png
--rw-rw-rw-   0        0        0      347 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/next.png
--rw-rw-rw-   0        0        0      225 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/next_hi.png
--rw-rw-rw-   0        0        0      348 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/next_lo.png
--rw-rw-rw-   0        0        0   207707 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/onvif-gui.ico
--rw-rw-rw-   0        0        0    46084 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/onvif-gui.png
--rw-rw-rw-   0        0        0      172 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/pause.png
--rw-rw-rw-   0        0        0      144 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/pause_hi.png
--rw-rw-rw-   0        0        0      149 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/pause_lo.png
--rw-rw-rw-   0        0        0    73660 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/ping.mp3
--rw-rw-rw-   0        0        0     1516 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/plain_recording.gif
--rw-rw-rw-   0        0        0      321 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/play.png
--rw-rw-rw-   0        0        0      209 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/play_hi.png
--rw-rw-rw-   0        0        0      316 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/play_lo.png
--rw-rw-rw-   0        0        0      349 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/previous.png
--rw-rw-rw-   0        0        0      232 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/previous_hi.png
--rw-rw-rw-   0        0        0      348 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/previous_lo.png
--rw-rw-rw-   0        0        0      324 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/radio-off.png
--rw-rw-rw-   0        0        0      250 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/radio-off_hi.png
--rw-rw-rw-   0        0        0      324 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/radio-off_lo.png
--rw-rw-rw-   0        0        0      350 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/radio-on.png
--rw-rw-rw-   0        0        0      263 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/radio-on_hi.png
--rw-rw-rw-   0        0        0      343 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/radio-on_lo.png
--rw-rw-rw-   0        0        0      395 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/record.png
--rw-rw-rw-   0        0        0     4377 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/record_hi.png
--rw-rw-rw-   0        0        0     4428 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/record_lo.png
--rw-rw-rw-   0        0        0      408 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/recording.png
--rw-rw-rw-   0        0        0      435 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/recording_hi.png
--rw-rw-rw-   0        0        0      532 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/recording_lo.png
--rw-rw-rw-   0        0        0      454 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/rewind.png
--rw-rw-rw-   0        0        0      250 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/rewind_hi.png
--rw-rw-rw-   0        0        0      457 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/rewind_lo.png
--rw-rw-rw-   0        0        0      187 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/small_arrow_left.png
--rw-rw-rw-   0        0        0      183 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/small_arrow_left_hi.png
--rw-rw-rw-   0        0        0      189 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/small_arrow_left_lo.png
--rw-rw-rw-   0        0        0      162 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/small_arrow_up.png
--rw-rw-rw-   0        0        0      160 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/small_arrow_up_hi.png
--rw-rw-rw-   0        0        0      161 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/small_arrow_up_lo.png
--rw-rw-rw-   0        0        0    19236 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/spinner.gif
--rw-rw-rw-   0        0        0      158 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/stop.png
--rw-rw-rw-   0        0        0      140 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/stop_hi.png
--rw-rw-rw-   0        0        0      151 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/stop_lo.png
--rw-rw-rw-   0        0        0      143 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/unchecked.png
--rw-rw-rw-   0        0        0      142 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/unchecked_hi.png
--rw-rw-rw-   0        0        0      143 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/gui/resources/unchecked_lo.png
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.527674 onvif-gui-2.0.1/modules/
--rw-rw-rw-   0        0        0        0 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.535656 onvif-gui-2.0.1/modules/audio/
--rw-rw-rw-   0        0        0        0 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/modules/audio/__init__.py
--rw-rw-rw-   0        0        0    27640 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/modules/audio/sample.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.549585 onvif-gui-2.0.1/modules/video/
--rw-rw-rw-   0        0        0        0 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/modules/video/__init__.py
--rw-rw-rw-   0        0        0     8041 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/modules/video/motion.py
--rw-rw-rw-   0        0        0    17303 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/modules/video/yolox.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.638653 onvif-gui-2.0.1/onvif_gui.egg-info/
--rw-rw-rw-   0        0        0     2410 2024-03-29 01:54:08.000000 onvif-gui-2.0.1/onvif_gui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3497 2024-03-29 01:54:08.000000 onvif-gui-2.0.1/onvif_gui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 01:54:08.000000 onvif-gui-2.0.1/onvif_gui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-03-29 01:54:08.000000 onvif-gui-2.0.1/onvif_gui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2024-03-29 01:54:08.000000 onvif-gui-2.0.1/onvif_gui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-29 01:54:08.000000 onvif-gui-2.0.1/onvif_gui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1772 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-29 01:54:08.640648 onvif-gui-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1586 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.572108 onvif-gui-2.0.1/yolox/
--rw-rw-rw-   0        0        0        0 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.627683 onvif-gui-2.0.1/yolox/models/
--rw-rw-rw-   0        0        0      961 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/models/__init__.py
--rw-rw-rw-   0        0        0     5019 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/models/build.py
--rw-rw-rw-   0        0        0     6840 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/models/darknet.py
--rw-rw-rw-   0        0        0     2372 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/models/losses.py
--rw-rw-rw-   0        0        0     6944 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/models/network_blocks.py
--rw-rw-rw-   0        0        0     3202 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/models/yolo_fpn.py
--rw-rw-rw-   0        0        0    26204 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/models/yolo_head.py
--rw-rw-rw-   0        0        0     4288 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/models/yolo_pafpn.py
--rw-rw-rw-   0        0        0     2054 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/models/yolox.py
-drwxrwxrwx   0        0        0        0 2024-03-29 01:54:08.637691 onvif-gui-2.0.1/yolox/utils/
--rw-rw-rw-   0        0        0      130 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/utils/__init__.py
--rw-rw-rw-   0        0        0     1628 2024-03-20 04:06:47.000000 onvif-gui-2.0.1/yolox/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.468036 onvif-gui-2.0.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0       62 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2521 2024-04-02 04:00:29.467038 onvif-gui-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1626 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.354023 onvif-gui-2.0.9/gui/
+-rw-rw-rw-   0        0        0       28 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.362018 onvif-gui-2.0.9/gui/components/
+-rw-rw-rw-   0        0        0      325 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/components/__init__.py
+-rw-rw-rw-   0        0        0     1833 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/components/comboselector.py
+-rw-rw-rw-   0        0        0     2693 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/components/directoryselector.py
+-rw-rw-rw-   0        0        0     2429 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/components/fileselector.py
+-rw-rw-rw-   0        0        0     4165 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/components/progress.py
+-rw-rw-rw-   0        0        0     8691 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/components/target.py
+-rw-rw-rw-   0        0        0     2723 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/components/thresholdslider.py
+-rw-rw-rw-   0        0        0     3023 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/components/warningbar.py
+-rw-rw-rw-   0        0        0    14860 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/glwidget.py
+-rw-rw-rw-   0        0        0    37632 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/main.py
+-rw-rw-rw-   0        0        0     9803 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/manager.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.369002 onvif-gui-2.0.9/gui/onvif/
+-rw-rw-rw-   0        0        0      269 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/onvif/__init__.py
+-rw-rw-rw-   0        0        0     9269 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/onvif/datastructures.py
+-rw-rw-rw-   0        0        0     4012 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/onvif/imagetab.py
+-rw-rw-rw-   0        0        0     2573 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/onvif/logindialog.py
+-rw-rw-rw-   0        0        0     4928 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/onvif/networktab.py
+-rw-rw-rw-   0        0        0     4990 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/onvif/ptztab.py
+-rw-rw-rw-   0        0        0    13341 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/onvif/systemtab.py
+-rw-rw-rw-   0        0        0    18638 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/onvif/videotab.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.374019 onvif-gui-2.0.9/gui/panels/
+-rw-rw-rw-   0        0        0      184 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/panels/__init__.py
+-rw-rw-rw-   0        0        0     3757 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/panels/audiopanel.py
+-rw-rw-rw-   0        0        0    30511 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/panels/camerapanel.py
+-rw-rw-rw-   0        0        0    25884 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/panels/filepanel.py
+-rw-rw-rw-   0        0        0    26380 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/panels/settingspanel.py
+-rw-rw-rw-   0        0        0     4718 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/panels/videopanel.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.438195 onvif-gui-2.0.9/gui/resources/
+-rw-rw-rw-   0        0        0     2021 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/__init__.py
+-rw-rw-rw-   0        0        0      435 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/alarm_plain.png
+-rw-rw-rw-   0        0        0      543 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/alarm_recording.gif
+-rw-rw-rw-   0        0        0      256 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/apply.png
+-rw-rw-rw-   0        0        0      267 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/apply_hi.png
+-rw-rw-rw-   0        0        0      262 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/apply_lo.png
+-rw-rw-rw-   0        0        0      911 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/audio.png
+-rw-rw-rw-   0        0        0      536 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/audio_hi.png
+-rw-rw-rw-   0        0        0      920 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/audio_lo.png
+-rw-rw-rw-   0        0        0      203 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/branch_closed.png
+-rw-rw-rw-   0        0        0      219 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/branch_closed_hi.png
+-rw-rw-rw-   0        0        0      211 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/branch_closed_lo.png
+-rw-rw-rw-   0        0        0      199 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/branch_open.png
+-rw-rw-rw-   0        0        0      168 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/branch_open_hi.png
+-rw-rw-rw-   0        0        0      172 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/branch_open_lo.png
+-rw-rw-rw-   0        0        0      267 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/checked.png
+-rw-rw-rw-   0        0        0      235 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/checked_hi.png
+-rw-rw-rw-   0        0        0      246 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/checked_lo.png
+-rw-rw-rw-   0        0        0    14172 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/darkstyle.qss
+-rw-rw-rw-   0        0        0      910 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/discover.png
+-rw-rw-rw-   0        0        0      849 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/discover_hi.png
+-rw-rw-rw-   0        0        0      937 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/discover_lo.png
+-rw-rw-rw-   0        0        0    75360 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/drops.mp3
+-rw-rw-rw-   0        0        0      425 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/fast-forward.png
+-rw-rw-rw-   0        0        0      253 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/fast-forward_hi.png
+-rw-rw-rw-   0        0        0      433 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/fast-forward_lo.png
+-rw-rw-rw-   0        0        0     4675 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/idle_lo.png
+-rw-rw-rw-   0        0        0    29256 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/loud.mp3
+-rw-rw-rw-   0        0        0      641 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/mute.png
+-rw-rw-rw-   0        0        0      346 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/mute_hi.png
+-rw-rw-rw-   0        0        0      618 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/mute_lo.png
+-rw-rw-rw-   0        0        0      347 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/next.png
+-rw-rw-rw-   0        0        0      225 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/next_hi.png
+-rw-rw-rw-   0        0        0      348 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/next_lo.png
+-rw-rw-rw-   0        0        0   207707 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/onvif-gui.ico
+-rw-rw-rw-   0        0        0    46084 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/onvif-gui.png
+-rw-rw-rw-   0        0        0      172 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/pause.png
+-rw-rw-rw-   0        0        0      144 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/pause_hi.png
+-rw-rw-rw-   0        0        0      149 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/pause_lo.png
+-rw-rw-rw-   0        0        0    73660 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/ping.mp3
+-rw-rw-rw-   0        0        0     1516 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/plain_recording.gif
+-rw-rw-rw-   0        0        0      321 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/play.png
+-rw-rw-rw-   0        0        0      209 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/play_hi.png
+-rw-rw-rw-   0        0        0      316 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/play_lo.png
+-rw-rw-rw-   0        0        0      349 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/previous.png
+-rw-rw-rw-   0        0        0      232 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/previous_hi.png
+-rw-rw-rw-   0        0        0      348 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/previous_lo.png
+-rw-rw-rw-   0        0        0      324 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/radio-off.png
+-rw-rw-rw-   0        0        0      250 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/radio-off_hi.png
+-rw-rw-rw-   0        0        0      324 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/radio-off_lo.png
+-rw-rw-rw-   0        0        0      350 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/radio-on.png
+-rw-rw-rw-   0        0        0      263 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/radio-on_hi.png
+-rw-rw-rw-   0        0        0      343 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/radio-on_lo.png
+-rw-rw-rw-   0        0        0      395 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/record.png
+-rw-rw-rw-   0        0        0     4377 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/record_hi.png
+-rw-rw-rw-   0        0        0     4428 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/record_lo.png
+-rw-rw-rw-   0        0        0      408 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/recording.png
+-rw-rw-rw-   0        0        0      435 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/recording_hi.png
+-rw-rw-rw-   0        0        0      532 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/recording_lo.png
+-rw-rw-rw-   0        0        0      454 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/rewind.png
+-rw-rw-rw-   0        0        0      250 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/rewind_hi.png
+-rw-rw-rw-   0        0        0      457 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/rewind_lo.png
+-rw-rw-rw-   0        0        0      187 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/small_arrow_left.png
+-rw-rw-rw-   0        0        0      183 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/small_arrow_left_hi.png
+-rw-rw-rw-   0        0        0      189 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/small_arrow_left_lo.png
+-rw-rw-rw-   0        0        0      162 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/small_arrow_up.png
+-rw-rw-rw-   0        0        0      160 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/small_arrow_up_hi.png
+-rw-rw-rw-   0        0        0      161 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/small_arrow_up_lo.png
+-rw-rw-rw-   0        0        0    19236 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/spinner.gif
+-rw-rw-rw-   0        0        0      158 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/stop.png
+-rw-rw-rw-   0        0        0      140 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/stop_hi.png
+-rw-rw-rw-   0        0        0      151 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/stop_lo.png
+-rw-rw-rw-   0        0        0      143 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/unchecked.png
+-rw-rw-rw-   0        0        0      142 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/unchecked_hi.png
+-rw-rw-rw-   0        0        0      143 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/gui/resources/unchecked_lo.png
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.439194 onvif-gui-2.0.9/modules/
+-rw-rw-rw-   0        0        0        0 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.441194 onvif-gui-2.0.9/modules/audio/
+-rw-rw-rw-   0        0        0        0 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/modules/audio/__init__.py
+-rw-rw-rw-   0        0        0    27640 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/modules/audio/sample.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.444193 onvif-gui-2.0.9/modules/video/
+-rw-rw-rw-   0        0        0        0 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/modules/video/__init__.py
+-rw-rw-rw-   0        0        0     8041 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/modules/video/motion.py
+-rw-rw-rw-   0        0        0    17067 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/modules/video/yolox.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.466041 onvif-gui-2.0.9/onvif_gui.egg-info/
+-rw-rw-rw-   0        0        0     2521 2024-04-02 04:00:29.000000 onvif-gui-2.0.9/onvif_gui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3497 2024-04-02 04:00:29.000000 onvif-gui-2.0.9/onvif_gui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 04:00:29.000000 onvif-gui-2.0.9/onvif_gui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-02 04:00:29.000000 onvif-gui-2.0.9/onvif_gui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2024-04-02 04:00:29.000000 onvif-gui-2.0.9/onvif_gui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-02 04:00:29.000000 onvif-gui-2.0.9/onvif_gui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1764 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 04:00:29.468036 onvif-gui-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1586 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.455155 onvif-gui-2.0.9/yolox/
+-rw-rw-rw-   0        0        0        0 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.463049 onvif-gui-2.0.9/yolox/models/
+-rw-rw-rw-   0        0        0      961 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/models/__init__.py
+-rw-rw-rw-   0        0        0     5019 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/models/build.py
+-rw-rw-rw-   0        0        0     6840 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/models/darknet.py
+-rw-rw-rw-   0        0        0     2372 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/models/losses.py
+-rw-rw-rw-   0        0        0     6944 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/models/network_blocks.py
+-rw-rw-rw-   0        0        0     3202 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/models/yolo_fpn.py
+-rw-rw-rw-   0        0        0    26204 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/models/yolo_head.py
+-rw-rw-rw-   0        0        0     4288 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/models/yolo_pafpn.py
+-rw-rw-rw-   0        0        0     2054 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/models/yolox.py
+drwxrwxrwx   0        0        0        0 2024-04-02 04:00:29.465043 onvif-gui-2.0.9/yolox/utils/
+-rw-rw-rw-   0        0        0      130 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/utils/__init__.py
+-rw-rw-rw-   0        0        0     1628 2024-04-02 03:54:50.000000 onvif-gui-2.0.9/yolox/utils/utils.py
```

### Comparing `onvif-gui-2.0.1/LICENSE` & `onvif-gui-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/PKG-INFO` & `onvif-gui-2.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 2.0.1
+Version: 2.0.9
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: libonvif==3.1.0
-Requires-Dist: avio==3.1.0
+Requires-Dist: libonvif==3.1.1
+Requires-Dist: avio==3.1.2
 Requires-Dist: PyQt6-Qt6==6.6.1
 Requires-Dist: pyqt6==6.6.1
 Requires-Dist: numpy
 Requires-Dist: loguru
 Requires-Dist: opencv-python
 
 
 onvif-gui
 ===
 
 Onvif GUI is an integrated camera management and NVR system with an intuitive user interface that can easily manage a fleet of cameras and create high resolution recordings based on alarm conditions. A best of breed YOLO detector is included with the system to facilitate accurate alarm signals without false detections. The system is designed to scale with available hardware and will run on simple configurations with minimal hardware requirements as well as high end multi core CPUs with NVIDIA GPU for maximum performance. The system can be configured with auto start settings and a user friendly icon so that non-technical users can feel comfortable working with the application without specialized training. File management is easy with an automated disk space manager and file playback controls.
 
-For a full description of the project, please visit [Onvif GUI](https://github.com/sr99622/libonvif).
+Please note that installation of this program may require some dependencies.
+
+For a full description of the project with installation instructions, please visit [Onvif GUI](https://github.com/sr99622/libonvif).
 
 Copyright (c) 2022, 2023, 2024  Stephen Rhodes
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `onvif-gui-2.0.1/README.md` & `onvif-gui-2.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 
 onvif-gui
 ===
 
 Onvif GUI is an integrated camera management and NVR system with an intuitive user interface that can easily manage a fleet of cameras and create high resolution recordings based on alarm conditions. A best of breed YOLO detector is included with the system to facilitate accurate alarm signals without false detections. The system is designed to scale with available hardware and will run on simple configurations with minimal hardware requirements as well as high end multi core CPUs with NVIDIA GPU for maximum performance. The system can be configured with auto start settings and a user friendly icon so that non-technical users can feel comfortable working with the application without specialized training. File management is easy with an automated disk space manager and file playback controls.
 
-For a full description of the project, please visit [Onvif GUI](https://github.com/sr99622/libonvif).
+Please note that installation of this program may require some dependencies.
+
+For a full description of the project with installation instructions, please visit [Onvif GUI](https://github.com/sr99622/libonvif).
 
 Copyright (c) 2022, 2023, 2024  Stephen Rhodes
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `onvif-gui-2.0.1/gui/components/comboselector.py` & `onvif-gui-2.0.9/gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/components/directoryselector.py` & `onvif-gui-2.0.9/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/components/fileselector.py` & `onvif-gui-2.0.9/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/components/progress.py` & `onvif-gui-2.0.9/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/components/target.py` & `onvif-gui-2.0.9/gui/components/target.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/components/thresholdslider.py` & `onvif-gui-2.0.9/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/components/warningbar.py` & `onvif-gui-2.0.9/gui/components/warningbar.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/glwidget.py` & `onvif-gui-2.0.9/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/main.py` & `onvif-gui-2.0.9/gui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from gui.glwidget import GLWidget
 from gui.manager import Manager
 from gui.onvif import StreamState
 from collections import deque
 import shutil
 import avio
 
-VERSION = "2.0.1"
+VERSION = "2.0.9"
 
 class PipeManager():
     def __init__(self, mw, uri):
         self.mw = mw
         self.uri = uri
 
 class PlayerSignals(QObject):
```

### Comparing `onvif-gui-2.0.1/gui/manager.py` & `onvif-gui-2.0.9/gui/manager.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/onvif/datastructures.py` & `onvif-gui-2.0.9/gui/onvif/datastructures.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/onvif/imagetab.py` & `onvif-gui-2.0.9/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/onvif/logindialog.py` & `onvif-gui-2.0.9/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/onvif/networktab.py` & `onvif-gui-2.0.9/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/onvif/ptztab.py` & `onvif-gui-2.0.9/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/onvif/systemtab.py` & `onvif-gui-2.0.9/gui/onvif/systemtab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/onvif/videotab.py` & `onvif-gui-2.0.9/gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/panels/audiopanel.py` & `onvif-gui-2.0.9/gui/panels/audiopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/panels/camerapanel.py` & `onvif-gui-2.0.9/gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/panels/filepanel.py` & `onvif-gui-2.0.9/gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/panels/settingspanel.py` & `onvif-gui-2.0.9/gui/panels/settingspanel.py`

 * *Files 0% similar despite different names*

```diff
@@ -452,24 +452,14 @@
         filename = ""
         if sys.platform == "win32":
             filename = os.environ['HOMEPATH'] + "/.cache/onvif-gui/logs.txt"
         else:
             filename = os.environ['HOME'] + "/.cache/onvif-gui/logs.txt"
         return filename
 
-    def getDirectorySize(self, d):
-        total_size = 0
-        for dirpath, dirnames, filenames in os.walk(d):
-            for f in filenames:
-                fp = os.path.join(dirpath, f)
-                if not os.path.islink(fp):
-                    total_size += os.path.getsize(fp)
-        
-        return total_size
-    
     def btnShowLogsClicked(self):
         filename = self.getLogFilename()
         if not self.dlgLog:
             self.dlgLog = LogDialog(self.mw)
         self.dlgLog.readLogFile(filename)
         self.dlgLog.exec()
 
@@ -566,7 +556,18 @@
             for f in filenames:
                 fp = os.path.join(dirpath, f)
                 if not os.path.islink(fp):
                     d_size += os.path.getsize(fp)
         total, used, free = shutil.disk_usage(d)
         max_available = (free + d_size - 10000000000) / 1000000000
         return max_available
+
+    def getDirectorySize(self, d):
+        total_size = 0
+        for dirpath, dirnames, filenames in os.walk(d):
+            for f in filenames:
+                fp = os.path.join(dirpath, f)
+                if not os.path.islink(fp):
+                    total_size += os.path.getsize(fp)
+        
+        return total_size
+
```

### Comparing `onvif-gui-2.0.1/gui/panels/videopanel.py` & `onvif-gui-2.0.9/gui/panels/videopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/LICENSE` & `onvif-gui-2.0.9/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/alarm_recording.gif` & `onvif-gui-2.0.9/gui/resources/alarm_recording.gif`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/audio.png` & `onvif-gui-2.0.9/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/audio_hi.png` & `onvif-gui-2.0.9/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/audio_lo.png` & `onvif-gui-2.0.9/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/darkstyle.qss` & `onvif-gui-2.0.9/gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/discover.png` & `onvif-gui-2.0.9/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/discover_hi.png` & `onvif-gui-2.0.9/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/discover_lo.png` & `onvif-gui-2.0.9/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/drops.mp3` & `onvif-gui-2.0.9/gui/resources/drops.mp3`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/idle_lo.png` & `onvif-gui-2.0.9/gui/resources/idle_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/loud.mp3` & `onvif-gui-2.0.9/gui/resources/loud.mp3`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/mute.png` & `onvif-gui-2.0.9/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/mute_lo.png` & `onvif-gui-2.0.9/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/onvif-gui.ico` & `onvif-gui-2.0.9/gui/resources/onvif-gui.ico`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/onvif-gui.png` & `onvif-gui-2.0.9/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/ping.mp3` & `onvif-gui-2.0.9/gui/resources/ping.mp3`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/plain_recording.gif` & `onvif-gui-2.0.9/gui/resources/plain_recording.gif`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/record_hi.png` & `onvif-gui-2.0.9/gui/resources/record_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/record_lo.png` & `onvif-gui-2.0.9/gui/resources/record_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/recording_lo.png` & `onvif-gui-2.0.9/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/gui/resources/spinner.gif` & `onvif-gui-2.0.9/gui/resources/spinner.gif`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/modules/audio/sample.py` & `onvif-gui-2.0.9/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/modules/video/motion.py` & `onvif-gui-2.0.9/modules/video/motion.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/modules/video/yolox.py` & `onvif-gui-2.0.9/modules/video/yolox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #/********************************************************************
-# libonvif/onvif-gui/modules/video/yolox.py 
+# onvif-gui/modules/video/yolox.py 
 #
 # Copyright (c) 2023  Stephen Rhodes
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -23,18 +23,18 @@
     import sys
     from loguru import logger
     import numpy as np
     from pathlib import Path
     from gui.components import ComboSelector, FileSelector, ThresholdSlider, TargetSelector
     from gui.onvif.datastructures import MediaSource
     from PyQt6.QtWidgets import QWidget, QGridLayout, QLabel, QCheckBox, QMessageBox, \
-        QGroupBox, QDialog
+        QGroupBox, QSlider, QDialog
     from PyQt6.QtCore import Qt, QSize, QObject, pyqtSignal
     from PyQt6.QtGui import QMovie
-    from time import sleep
+    import time
     import torch
     from torchvision.transforms import functional
     import torch.nn as nn
     from yolox.models import YOLOX, YOLOPAFPN, YOLOXHead
     from yolox.utils import postprocess
 
 except ModuleNotFoundError as ex:
@@ -144,22 +144,19 @@
             self.signals = YoloxSignals()
             self.signals.showWaitDialog.connect(self.showWaitDialog)
             self.signals.hideWaitDialog.connect(self.hideWaitDialog)
             
             self.chkAuto = QCheckBox("Automatically download model")
             self.chkAuto.setChecked(int(self.mw.settings.value(self.autoKey, 1)))
             self.chkAuto.stateChanged.connect(self.chkAutoClicked)
-
             self.txtFilename = FileSelector(mw, MODULE_NAME)
             self.txtFilename.setEnabled(not self.chkAuto.isChecked())
             self.cmbRes = ComboSelector(mw, "Model Size", ("320", "480", "640", "960", "1280", "1440"), "640", MODULE_NAME)
             self.cmbType = ComboSelector(mw, "Model Name", ("yolox_s", "yolox_m", "yolox_l", "yolox_x"), "yolox_s", MODULE_NAME)
 
-            self.txtFilename.setEnabled(not self.chkAuto.isChecked())
-
             self.sldConfThre = ThresholdSlider(mw, "Confidence", MODULE_NAME)
             self.selTargets = TargetSelector(self.mw, MODULE_NAME)
 
             grpSystem = QGroupBox("System wide model parameters")
             lytSystem = QGridLayout(grpSystem)
             lytSystem.addWidget(self.chkAuto,      0, 0, 1, 1)
             lytSystem.addWidget(self.cmbType,      1, 0, 1, 1)
@@ -251,14 +248,15 @@
 
             if self.mw.videoConfigure.name != MODULE_NAME or len(IMPORT_ERROR) > 0:
                 return
             
             device_name = "cpu"
             if torch.cuda.is_available():
                 device_name = "cuda"
+
             self.device = torch.device(device_name)
 
             self.mw.glWidget.model_loading = True
 
             self.num_classes = 80
 
             size = {'yolox_s': [0.33, 0.50], 
@@ -293,29 +291,28 @@
             res = int(self.mw.videoConfigure.cmbRes.currentText())
             self.model(torch.zeros(1, 3, res, res).to(self.device))
             self.mw.glWidget.model_loading = False
 
         except:
             logger.exception(MODULE_NAME + " initialization failure")
             self.mw.signals.error.emit(MODULE_NAME + " initialization failure, please check logs for details")
-            for player in self.mw.pm.players:
-                player.request_reconnect = False
-                player.running = False
-            self.mw.glWidget.model_loading = False
-                
+
     def __call__(self, F, player):
         try:
 
-            if not F or not player or self.mw.videoConfigure.name != MODULE_NAME:
+            if not F or not player:
                 self.mw.videoConfigure.selTargets.barLevel.setLevel(0)
                 self.mw.videoConfigure.selTargets.indAlarm.setState(0)
                 return
 
             img = np.array(F, copy=False)
 
+            if self.mw.videoConfigure.name != MODULE_NAME:
+                return
+            
             res = int(self.mw.videoConfigure.cmbRes.currentText())
             test_size = (res, res)
             ratio = min(test_size[0] / img.shape[0], test_size[1] / img.shape[1])
             inf_shape = (int(img.shape[0] * ratio), int(img.shape[1] * ratio))
             bottom = test_size[0] - inf_shape[0]
             side = test_size[1] - inf_shape[1]
             pad = (0, 0, side, bottom)
@@ -337,19 +334,20 @@
                     if not self.mw.videoConfigure.isModelSettings(self.mw.filePanel.videoModelSettings):
                         self.mw.filePanel.videoModelSettings = YoloxSettings(self.mw)
                     player.videoModelSettings = self.mw.filePanel.videoModelSettings
 
             if not player.videoModelSettings:
                 raise Exception("Unable to set video model parameters for player")
 
+
             confthre = player.videoModelSettings.confidence / 100
             nmsthre = 0.65
 
             while self.lock:
-                sleep(0.001)
+                time.sleep(0.001)
             
             self.lock = True
             with torch.no_grad():
                 outputs = self.model(timg)
                 outputs = postprocess(outputs, self.num_classes, confthre, nmsthre)
             self.lock = False
 
@@ -369,19 +367,20 @@
 
             gain = 1
             if frame_rate:
                 gain = player.videoModelSettings.gain / frame_rate
 
             alarmState = result * gain >= 1.0
 
-            if self.mw.glWidget.focused_uri == player.uri:
-                self.mw.videoConfigure.selTargets.barLevel.setLevel(result * gain)
-                if alarmState:
-                    self.mw.videoConfigure.selTargets.indAlarm.setState(1)
-                    
+            if camera:
+                if camera.isFocus():
+                    self.mw.videoConfigure.selTargets.barLevel.setLevel(result * gain)
+                    if alarmState:
+                        self.mw.videoConfigure.selTargets.indAlarm.setState(1)
+
             player.handleAlarm(alarmState)
 
             # restart the model if changed during run time
             tmp = None
             if self.mw.videoConfigure.chkAuto.isChecked():
                 tmp = self.get_auto_ckpt_filename()
             else:
```

### Comparing `onvif-gui-2.0.1/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-2.0.9/onvif_gui.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: onvif-gui
-Version: 2.0.1
+Version: 2.0.9
 Summary: A client gui for Onvif
 Author: Stephen Rhodes
 Author-email: Stephen Rhodes <sr99622@gmail.com>
 Project-URL: Homepage, https://github.com/sr99622/libonvif
 Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
 Keywords: sample,setuptools,development
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: libonvif==3.1.0
-Requires-Dist: avio==3.1.0
+Requires-Dist: libonvif==3.1.1
+Requires-Dist: avio==3.1.2
 Requires-Dist: PyQt6-Qt6==6.6.1
 Requires-Dist: pyqt6==6.6.1
 Requires-Dist: numpy
 Requires-Dist: loguru
 Requires-Dist: opencv-python
 
 
 onvif-gui
 ===
 
 Onvif GUI is an integrated camera management and NVR system with an intuitive user interface that can easily manage a fleet of cameras and create high resolution recordings based on alarm conditions. A best of breed YOLO detector is included with the system to facilitate accurate alarm signals without false detections. The system is designed to scale with available hardware and will run on simple configurations with minimal hardware requirements as well as high end multi core CPUs with NVIDIA GPU for maximum performance. The system can be configured with auto start settings and a user friendly icon so that non-technical users can feel comfortable working with the application without specialized training. File management is easy with an automated disk space manager and file playback controls.
 
-For a full description of the project, please visit [Onvif GUI](https://github.com/sr99622/libonvif).
+Please note that installation of this program may require some dependencies.
+
+For a full description of the project with installation instructions, please visit [Onvif GUI](https://github.com/sr99622/libonvif).
 
 Copyright (c) 2022, 2023, 2024  Stephen Rhodes
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `onvif-gui-2.0.1/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-2.0.9/onvif_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/pyproject.toml` & `onvif-gui-2.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "2.0.1"  
+version = "2.0.9"
 dynamic = ["gui-scripts"]
-description = "A client gui for Onvif"  
-readme = "README.md" 
+description = "A client gui for Onvif"
+readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
-keywords = ["sample", "setuptools", "development"]  
+keywords = ["sample", "setuptools", "development"]
 authors = [
-  {name = "Stephen Rhodes", email = "sr99622@gmail.com" } 
+  {name = "Stephen Rhodes", email = "sr99622@gmail.com" }
 ]
 classifiers = [ 
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Build Tools",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
 ]
 
 dependencies = [
-  "libonvif==3.1.0", "avio==3.1.0", "PyQt6-Qt6==6.6.1", "pyqt6==6.6.1", "numpy", "loguru", "opencv-python"
+  "libonvif==3.1.1", "avio==3.1.2", "PyQt6-Qt6==6.6.1", "pyqt6==6.6.1", "numpy", "loguru", "opencv-python"
 ]
 
 [project.urls]  
 "Homepage" = "https://github.com/sr99622/libonvif"
 "Bug Reports" = "https://github.com/sr99622/libonvif/issues"
 
 [tool.setuptools]
```

### Comparing `onvif-gui-2.0.1/setup.py` & `onvif-gui-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #from setuptools.command.install import install
 
 with open("README.md", "r", encoding = 'cp850') as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="2.0.1",
+    version="2.0.9",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-2.0.1/yolox/models/__init__.py` & `onvif-gui-2.0.9/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/yolox/models/build.py` & `onvif-gui-2.0.9/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/yolox/models/darknet.py` & `onvif-gui-2.0.9/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/yolox/models/losses.py` & `onvif-gui-2.0.9/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/yolox/models/network_blocks.py` & `onvif-gui-2.0.9/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/yolox/models/yolo_fpn.py` & `onvif-gui-2.0.9/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/yolox/models/yolo_head.py` & `onvif-gui-2.0.9/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/yolox/models/yolo_pafpn.py` & `onvif-gui-2.0.9/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/yolox/models/yolox.py` & `onvif-gui-2.0.9/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-2.0.1/yolox/utils/utils.py` & `onvif-gui-2.0.9/yolox/utils/utils.py`

 * *Files identical despite different names*

