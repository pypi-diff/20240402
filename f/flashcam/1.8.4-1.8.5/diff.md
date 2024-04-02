# Comparing `tmp/flashcam-1.8.4.tar.gz` & `tmp/flashcam-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.8.4.tar", last modified: Mon Mar 18 09:01:38 2024, max compression
+gzip compressed data, was "flashcam-1.8.5.tar", last modified: Tue Apr  2 04:03:01 2024, max compression
```

## Comparing `flashcam-1.8.4.tar` & `flashcam-1.8.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-18 09:01:38.212507 flashcam-1.8.4/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1182 2024-03-18 09:01:38.212507 flashcam-1.8.4/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-03-18 09:01:35.000000 flashcam-1.8.4/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-18 09:01:38.208507 flashcam-1.8.4/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29232 2024-03-17 02:07:58.000000 flashcam-1.8.4/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.8.4/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.8.4/bin/flashcam_org
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.8.4/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.8.4/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-18 09:01:38.208507 flashcam-1.8.4/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.8.4/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.8.4/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-18 09:01:38.212507 flashcam-1.8.4/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/digital-7.regular.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/pattern_acircles.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/pattern_chessboard.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/small_pixel.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.8.4/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50988 2024-03-18 09:00:55.000000 flashcam-1.8.4/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    43179 2023-11-02 08:34:00.000000 flashcam-1.8.4/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   113386 2024-03-17 02:07:44.000000 flashcam-1.8.4/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12892 2024-03-18 09:00:03.000000 flashcam-1.8.4/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.8.4/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-03-18 09:01:37.000000 flashcam-1.8.4/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40594 2024-03-17 02:07:44.000000 flashcam-1.8.4/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-03-18 09:01:38.208507 flashcam-1.8.4/flashcam.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1182 2024-03-18 09:01:38.000000 flashcam-1.8.4/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      975 2024-03-18 09:01:38.000000 flashcam-1.8.4/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-03-18 09:01:38.000000 flashcam-1.8.4/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-03-18 09:01:38.000000 flashcam-1.8.4/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-03-18 09:01:38.000000 flashcam-1.8.4/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-03-18 09:01:38.212507 flashcam-1.8.4/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.8.4/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.761471 flashcam-1.8.5/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 04:03:01.761471 flashcam-1.8.5/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-02 04:02:58.000000 flashcam-1.8.5/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.753471 flashcam-1.8.5/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29232 2024-03-17 02:07:58.000000 flashcam-1.8.5/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.8.5/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.8.5/bin/flashcam_org
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.8.5/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.8.5/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.757471 flashcam-1.8.5/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.8.5/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.8.5/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.761471 flashcam-1.8.5/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/digital-7.regular.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/pattern_acircles.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/pattern_chessboard.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/small_pixel.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.8.5/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50031 2024-04-02 04:02:11.000000 flashcam-1.8.5/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    43919 2024-04-02 03:57:37.000000 flashcam-1.8.5/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   114843 2024-03-22 13:59:53.000000 flashcam-1.8.5/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13417 2024-04-02 03:26:49.000000 flashcam-1.8.5/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.8.5/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40698 2024-04-02 03:34:28.000000 flashcam-1.8.5/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.761471 flashcam-1.8.5/flashcam.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      975 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-02 04:03:01.761471 flashcam-1.8.5/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.8.5/setup.py
```

### Comparing `flashcam-1.8.4/PKG-INFO` & `flashcam-1.8.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: flashcam
-Version: 1.8.4
-Summary: Composition of scripts to control a web camera
-Home-page: https://gitlab.com/jaromrax/flashcam
-Author: jaromrax
-Author-email: jaromrax@gmail.com
-License: GPL2
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 Project flashcam
 ================
 
 `FLASk supported webCAM`
 
 *IN DEVELOPMENT*
 
@@ -43,9 +32,7 @@
 ===============
 
 <https://longervision.github.io/2017/03/12/ComputerVision/OpenCV/opencv-external-posture-estimation-ArUco-board/>
 
 <https://github.com/LongerVision/Examples_OpenCV/blob/master/01_internal_camera_calibration/chessboard.py>
 
 <https://markhedleyjones.com/projects/calibration-checkerboard-collection>
-
-
```

### Comparing `flashcam-1.8.4/bin/flashcam` & `flashcam-1.8.5/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/bin/flashcam_org` & `flashcam-1.8.5/bin/flashcam_org`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/bin/flashcam_rep` & `flashcam-1.8.5/bin/flashcam_rep`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/bin/flashcamg` & `flashcam-1.8.5/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/base_camera2.py` & `flashcam-1.8.5/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/config.py` & `flashcam-1.8.5/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.8.5/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.8.5/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/DET_NRDY.jpg` & `flashcam-1.8.5/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/DET_RDY_.jpg` & `flashcam-1.8.5/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/digital-7.mono.ttf` & `flashcam-1.8.5/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/digital-7.regular.ttf` & `flashcam-1.8.5/flashcam/data/digital-7.regular.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/monoskop.jpg` & `flashcam-1.8.5/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/pattern_acircles.png` & `flashcam-1.8.5/flashcam/data/pattern_acircles.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/pattern_chessboard.png` & `flashcam-1.8.5/flashcam/data/pattern_chessboard.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/small_pixel.ttf` & `flashcam-1.8.5/flashcam/data/small_pixel.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/win_rain.jpg` & `flashcam-1.8.5/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/win_skull.jpg` & `flashcam-1.8.5/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/win_storm.jpg` & `flashcam-1.8.5/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/win_winter.jpg` & `flashcam-1.8.5/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/data/windows.jpg` & `flashcam-1.8.5/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/direct.py` & `flashcam-1.8.5/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/izmq_receiver.py` & `flashcam-1.8.5/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/mmapwr.py` & `flashcam-1.8.5/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/real_camera.py` & `flashcam-1.8.5/flashcam/real_camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,17 @@
     for i in lines:
         posx = int(640/2 - len( str(i) )*32/2)
         if posx<minx:
             minx = posx
     return minx
 
 def force_text( frame, overtext , posy = 400, bg_bgra = (255,0,255,0) , fg_bgra = (0,255,255,255) ):
-
+    """
+    7segment LCD text in the middle
+    """
     posx = leftmost_txt_wid( overtext )# int(640/2 - len( str(overtext) )*32/2)
     if posx<0: posx=10
     position = ( posx ,posy)
     fontpath = os.path.expanduser("~/.config/flashcam/digital-7.mono.ttf")
     font = ImageFont.truetype(fontpath, 2*32)
 
     img_pil = Image.fromarray(frame).convert("RGBA")  # base img
@@ -139,18 +141,18 @@
     frame = np.array(composite)
     return frame
 
 # -----------------------------------------------------------------
 
 class Camera(BaseCamera):
 
-    video_source = 0
+    # video_source = 0
     histomean = 50
     #nfrm = 0 # number frame.... nonono
-    capdevice = None # global
+    # capdevice = None # global
 
     @staticmethod
     def init_cam(  ):
         """
         should return videocapture device
         but also sould set Camerare.video_source
         """
@@ -794,15 +796,15 @@
 
                         #
                         # PROBLEM TO SOLVE
                         #    i wait for re-demand from client........ seem to work.....
                         #
                         if expression == "switch_res":
                             switch_res = value #not(switch_res)
-                            print("i...              XEPERIMENTTAL SWITCH RESOLUTION now=", switch_res)
+                            print("i...              EXPERIMENTAL SWITCH RESOLUTION now=", switch_res)
                             if switch_res:
                                 maxres = get_resolutions( vidnum )[-1] # from usb_check
                                 config.CONFIG['resolution'] = maxres
                                 print("D.... resolution to MAX", maxres)
                                 # cap.close()
                                 #cap, vidnum, s9009 = camera.init_cam()
 
@@ -1000,14 +1002,17 @@
                         #-----------exposure in capa
                     # ______________________ section with capa for camera _____________________
 
 
                     #--------------- now apply labels ------i cannot get rid in DETM---
                     #--------- all this will be on all rames histo,detect,direct,delta
                     senh.setbox(" ", senh.TIME, kompr=config.CONFIG['kompress'])
+                    if switch_res:
+                        senh.setbox("xzoom", senh.xzoom)
+
                     #senh.setbox(" ", senh.TIME, kompr= frame.shape[1])
 
                     if framekind in ["detect","delta","histo"]:
                         senh.setbox(f"DISP {framekind}",senh.DISP)
                     if average>0:
                         senh.setbox(f"a {average}",  senh.avg)
                     if blur>0:
@@ -1134,35 +1139,14 @@
 
                     # debug info on final resolution
                     #print(f"  FIN{fg.yellow}{frame.shape}{fg.default} ", end = "" )
 
                     # --- here I can touch frame:
                     if overtext is not None:
                         frame = force_text( frame, overtext, posy = 400, fg_bgra= (0,255, 0, 255-int(overtextalpha)) )
-                        # posx = int(640/2 - len( str(overtext) )*32/2)
-                        # if posx<0: posx=10
-                        # position = ( posx ,400)
-                        # fontpath = os.path.expanduser("~/.config/flashcam/digital-7.mono.ttf")
-                        # font = ImageFont.truetype(fontpath, 2*32)
-
-                        # img_pil = Image.fromarray(frame).convert("RGBA")  # base img
-                        # txt_img = Image.new("RGBA", img_pil.size, (255,255,255,0))
-
-                        # #draw = ImageDraw.Draw(img_pil)
-                        # draw = ImageDraw.Draw(txt_img)
-                        # drtext =  f"{overtext}"# {overtextalpha}" # to be sure
-                        # b,g,r,a = 0,255, 0, 255-int(overtextalpha)
-                        # draw.text( position,  drtext, font = font, fill = (b, g, r, a))
-
-                        # composite = Image.alpha_composite(img_pil, txt_img)
-                        # #composite.save(output_path)
-
-
-                        # #frame = np.array(img_pil)
-                        # frame = np.array(composite)
                         if overtextalpha<255:
                             overtextalpha+=0.2
                         else:
                             overtext = None
```

### Comparing `flashcam-1.8.4/flashcam/stream_enhancer.py` & `flashcam-1.8.5/flashcam/stream_enhancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     hist= (6,0) # side
     rot = (7,0) # side  /otate in bin...
     # ------ more (with/for uni)
     avi = (8,0) #
     jpg = (9,0) #
 
     scale = (10,0) #? see
+    xzoom = (11,0) #? see
 
     delta_frame = None
     detect_frame = None
     frame_area = 1
 
     frame_number = 0
 
@@ -138,14 +139,15 @@
         if (row,col) == self.gamma: return (80,80,80) #
 
         if (row,col) == self.speedx: return (180,80,80) #
         if (row,col) == self.speedy: return (80,180,80) #
         if (row,col) == self.avi:    return (30,30,210) # FOR UNI only
         if (row,col) == self.jpg:    return (0,0,250)   # FOR UNI only
         if (row,col) == self.scale:  return (250,0,250)   # zoom scale
+        if (row,col) == self.xzoom:  return (250,100,250)   # xperimental zoom
 
         t=[255,255,255]
         while (t[0]+t[1]+t[2]>400) or  (t[0]+t[1]+t[2]<200) :
             t =  (randint(5,255),randint(5,255),randint(5,255) )
         #print(t[0]+t[1]+t[2])
         return t
 
@@ -516,19 +518,18 @@
         T = np.float32([[1, 0, dwidth], [0, 1, dheight]])
         shifted = cv2.warpAffine(self.frame, T, (self.frame.shape[1], self.frame.shape[0]))
         # print( T )
         self.frame = shifted
 
 
 
-    def crosson(self,  dix, diy, color = "g"):
+    def crosson(self,  dix, diy, color = "g", box_small = True, box_large = False):
         """
         two types  g (just cross, r boxed cross)
         """
-        crotype = 'box'
         #if color == 'r': crotype = 'line'
         #
         RADIUS=63
         y = int(self.frame.shape[0]/2)
         x = int(self.frame.shape[1]/2)
 
         ix = x+dix
@@ -539,42 +540,54 @@
         elif (color=="r"):
             lcolor=(55,0,255) #BGR
         else:
             lcolor=(0,255,55)
 
         crscal = 4
         crnx,crny = int(64/crscal),int(48/crscal)
-        if crotype == "box":
-            midskip = crnx
-            midskipy = crny
-        else:
-            midskip = 7
-            midskipy = 7
+        #if crotype == "box":
+        midskip = crnx
+        midskipy = crny
+        #else:
+        #    midskip = 7
+        #    midskipy = 7
 
 
         i2=cv2.circle( self.frame, (ix,iy), RADIUS, lcolor, 1)
         i2=cv2.line(i2, (ix-RADIUS+midskip,iy), (ix-midskip,iy), lcolor, thickness=1, lineType=8)
         i2=cv2.line(i2, (ix+RADIUS-midskip,iy), (ix+midskip,iy), lcolor, thickness=1, lineType=8)
 
         i2=cv2.line(i2, (ix,iy-RADIUS+midskipy), (ix,iy-midskipy), lcolor, thickness=1, lineType=8)
         i2=cv2.line(i2, (ix,iy+RADIUS-midskipy), (ix,iy+midskipy), lcolor, thickness=1, lineType=8)
 
         # mid
         i2=cv2.line(i2, (ix,iy), (ix,iy), lcolor, thickness=1, lineType=8)
 
-        if crotype == "box":
+        #if crotype == "box":
+        if box_small:
             #corners  #  position 0.5deg from 11 deg. OK
-            crscal = 4
+            crscal = 4 # normal original box
+            crscal = 3.2 # normal original box
             crnx,crny = int(64/crscal),int(48/crscal)
 
             i2=cv2.line(i2, (ix-crnx,iy-crny), (ix+crnx,iy-crny), lcolor, thickness=1, lineType=8)
             i2=cv2.line(i2, (ix+crnx,iy-crny), (ix+crnx,iy+crny), lcolor, thickness=1, lineType=8)
             i2=cv2.line(i2, (ix+crnx,iy+crny), (ix-crnx,iy+crny), lcolor, thickness=1, lineType=8)
             i2=cv2.line(i2, (ix-crnx,iy+crny), (ix-crnx,iy-crny), lcolor, thickness=1, lineType=8)
 
+        if box_large:
+            #corners  #  position 0.5deg from 11 deg. OK
+            crscal = 1.4 # normal original box
+            crnx,crny = int(64/crscal),int(48/crscal)
+
+            i2=cv2.line(i2, (ix-crnx,iy-crny), (ix+crnx,iy-crny), lcolor, thickness=1 )
+            i2=cv2.line(i2, (ix+crnx,iy-crny), (ix+crnx,iy+crny), lcolor, thickness=1 )
+            i2=cv2.line(i2, (ix+crnx,iy+crny), (ix-crnx,iy+crny), lcolor, thickness=1 )
+            i2=cv2.line(i2, (ix-crnx,iy+crny), (ix-crnx,iy-crny), lcolor, thickness=1 )
+
         #return self.frame
 
 
     #---------- for motion detect i need a second processing line frame2
     # to keep the camera on
 
     def setblur(self, blur=0, dmblur = 0):
```

### Comparing `flashcam-1.8.4/flashcam/uniwrec.py` & `flashcam-1.8.5/flashcam/uniwrec.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
 from flashcam.stream_enhancer import Stream_Enhancer
 import webbrowser
 
 import math
 
 import requests  # crosson=CROSSON
+from PIL import ImageFont, ImageDraw, Image
 
 # ------------------problem with SHIFT
 # from pynput.keyboard import Key, Listener
 
 
 global SHIFT, CTRL
 SHIFT = CTRL = False
@@ -1214,15 +1215,15 @@
                 # ------------------------redcross here: before zoom--------------------------------------
                 # print(f" ... cross == {cross}")
                 if not (cross is None):
                     if senh.add_frame(frame):
                         w, h, c = frame.shape
                         # print(w-centerY1, h-centerX1)
                         # print(f" ... cross {w} {h} /2")
-                        senh.crosson(cross[0], cross[1], color="r")  # dx dy
+                        senh.crosson(cross[0], cross[1], color="r" , box_large = True)  # dx dy
                         # senh.setbox(f"CROS",  senh.jpg)
                         frame = senh.get_frame()
                     else:
                         print("X... senh did not accept frame (in redcross)")
 
                 # =========================== ZOOM ME and OTHERS =======
 
@@ -1656,14 +1657,36 @@
                 #                     now = datetime.datetime.now()
                 #                     delta = now - datetime.datetime(1970, 1, 1)
                 #                     if delta < countdown_s:
                 #                         TEXT = """scanning exposure
                 # in progress"""
                 #                         frame = disp_mutext(frame, TEXT)
 
+                # ANY chnges to imge BEFORE IMSHOW!!
+                if cross is not None:
+                    overtext = f"({cross[0]},{cross[1]})"
+                    fontpath = os.path.expanduser("~/.config/flashcam/small_pixel.ttf")
+                    #fontpath = os.path.expanduser("~/.config/flashcam/digital-7.mono.ttf")
+                    position = ( 320+15+cross[0],240-40+cross[1] ) # 480 on x
+                    font = ImageFont.truetype(fontpath, 8)
+                    img_pil = Image.fromarray(frame).convert("RGBA")
+                    draw = ImageDraw.Draw(img_pil)
+                    #draw.line((0, 0) + img_pil.size, fill=128)
+                    draw.fontmode = "1" # NO ANTIALIASING
+                    #overtext = ' '.join(overtext[i:i+1] for i in range(0, len(overtext), 1))
+                    drtext =  str(overtext) # to be sure
+                    print(drtext, end=" ")
+                    b,g,r,a = 0,0,255,0
+                    draw.text( position,  drtext, font = font, fill = (b, g, r, a))
+                    composite = img_pil #Image.alpha_composite(img_pil, img_pil)
+                    frame = np.array(composite)
+                    #print(frame.shape)
+
+
+
                 # ======================================================== IMSHOW
                 # ======================================================== IMSHOW
                 # ======================================================== IMSHOW
                 # ======================================================== IMSHOW
 
 
                 apply_distortion = False
@@ -1683,14 +1706,18 @@
                     dst = cv2.undistort(frame, mtx, dist, None, newcameramtx)
                     ## crop the image
                     #x, y, w, h = roi
                     frame = dst#[y:y+h, x:x+w]
 
 
 
+                # IMSHOW #############
+                # IMSHOW #############
+                # IMSHOW #############
+                # IMSHOW #############
                 cv2.imshow(rpi_name, frame)  # 1 window for each RPi
                 ##########cv2.moveWindow(rpi_name, int(xy1), int(xy2))
                # ======================================================== IMSHOW
                 if save_decor:
                     saviout.write(frame)
                 # ======================================================== IMSHOW
                 # ======================================================== IMSHOW
@@ -1997,14 +2024,15 @@
                         (frame is not None) and (rpi_name != "") and (key == ord("K") and not CTRL)
                     ):  # ^
                         cross[1] -= 17
                     if (
                         (frame is not None) and (rpi_name != "") and (key == ord("L") and not CTRL)
                     ):  # >
                         cross[0] += 17
+                    #print(frame.shape)
 
                 if (
                     (measure > 0)
                     and (frame is not None)
                     and (rpi_name != "")
                     and (key == ord("N"))
                 ):
```

### Comparing `flashcam-1.8.4/flashcam/usbcheck.py` & `flashcam-1.8.5/flashcam/usbcheck.py`

 * *Files 8% similar despite different names*

```diff
@@ -283,51 +283,75 @@
             id_path = ":".join( id_path.split(":")[2:] )
             ok = True
         except  Exception as ex:
             print("X... udevadm error...", ex, vid, end="\r")
             ok = False
     return f"{vendor}:{model}:{revision}"
 
+
+
+def is_int(n):
+    try:
+        float_n = float(n)
+        int_n = int(float_n)
+    except ValueError:
+        return False
+    else:
+        return float_n == int_n
+
+
+
+
 def recommend_video( prefname=None ):
     """
     glob through /dev/video*
     recommend video device:  without paramenter - the list is returned, else if string matches
 
     0     001 006 2.0 	0458:708c 	 Genius WideCam F100 	 14.0-usb-0:9:1.0 	 12e
     ./usbcheck.py "Genius W"
     """
     usb_hubs = usbroot()
 
     if not(prefname is None) and ( prefname.find(".jpg")>=0  or prefname.find("clock")==0   ):
         return [-1] # if image is required
 
-    devices=serial.tools.list_ports.comports()
-    print("____________________serial  devices _______"+"_"*37)
-    for i in devices:
-        print(i)
-    #print("D... this was serial devices")
+    # ====================== nice BUT NOT NEEDED HERE
+    # devices=serial.tools.list_ports.comports()
+    # print("____________________serial  devices _______"+"_"*37)
+    # for i in devices:
+    #     print(i)
+    # #print("D... this was serial devices")
 
     recommvid=[]
     vids=glob.glob("/dev/video*")
     print(f"{bg.cyan}____________________video   devices _______"+"_"*37+f"{bg.default}")
     print(f"video bus dev UsbTyp vendor:model:revision   product            IDpath       capa")
     recomvid = []
+
+    # it all takes very long.... I remove all videos above 9
+    for vid in vids[:]: # the trick to take a copy
+        if is_int(vid[-2]):
+            vids.remove(vid)
+
+    # ======== loop over remaining....
     for vid in sorted(vids):
         CMD = f"udevadm info --name={vid}"
+        #time.sleep(0.7)
 
         # print(f"D... cmd={CMD}")
         res = ""
         ok=False
         try:
             res=sp.check_output( CMD, shell=True ).decode("utf8")
             ok=True
         except:
             print("X... ... ERROR "+CMD)
             # TRYING TO ADDRES ISSUE #6
-            return []
+            # no return from here ---- I think -----
+            #return []
 
 
         if ok:
             #print(res)
             try: # I saw there was no result...when reconnecting camera....
                 vendor = [x for x in res.split() if x.find("ID_VENDOR_ID=")>=0][0]
                 vendor = vendor.split("=")[1]
```

### Comparing `flashcam-1.8.4/flashcam/v4lc.py` & `flashcam-1.8.5/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/flashcam/web.py` & `flashcam-1.8.5/flashcam/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -1087,15 +1087,15 @@
 # windows  webcamxp ...   jpg  only
 ##### @app.route('/cam_5.cgi')
 @app.route('/video')
 @app.route('/cam_5.jpg')
 @auth.login_required
 def video():
     remote_ip=request.environ.get('HTTP_X_REAL_IP', request.remote_addr)
-    print("W... asking VIDEO",request.remote_addr, remote_ip)
+    print("W... web is asking VIDEO",request.remote_addr, "(",remote_ip,")")
     logthis( " /video remote      = "+request.remote_addr )
     logthis( " /video remote xreal= "+remote_ip )
     # i return JPG TO AXIS CAMERA....
     #---------------this is MJPEG-------------------------
     #config.CONFIG["product"] = "Webcam C270"
     # return Response(gen(Camera(config.CONFIG["product"], "640x480"),remote_ip),
     # --- i send here the CLASS ?????
@@ -1114,27 +1114,29 @@
 def gen(camera, remote_ip, blend=False, bigtext=True):
     """ returns jpeg;
     MAY do modifications per USER ! BUT any fraME MOD => IS SENT TO ALL!
     can send only some frames
     """
     global  save_bg, frame_bg, frame_bg2, save_fg, frame_fg, frame_fg2, frame_mask, frame_mask_inv #, BGFILE
 
-    print("D... entered gen, camera = ", camera)
+    print("D... entered gen(), camera = ", camera)
     framecnt = 0
     framecnttrue = 0
     ss_time = 0
 
 
 
     while True:
         time.sleep(0.1)
         framecnt+=1
         #print("D... get_frame (gen)")
 
+        print("D...  gen() - getframe ... ")
         frame,b_nframes,b_capture_time = camera.get_frame() # This is BaseCamera method, inherited in Camera
+        print("D...  gen() - gotframe  ")
 
         #print("i... got_frame (gen)", frame.shape )
         start = dt.datetime.now()
         blackframe = np.zeros((480,640,3), np.uint8)
         #frame = blackframe
         if blend:
             frame = 0.5*frame + 0.5*imgs[ random.randint(0,len(imgs)-1) ]
```

### Comparing `flashcam-1.8.4/flashcam.egg-info/SOURCES.txt` & `flashcam-1.8.5/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.4/setup.py` & `flashcam-1.8.5/setup.py`

 * *Files identical despite different names*

