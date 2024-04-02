# Comparing `tmp/flashcam-1.8.5.tar.gz` & `tmp/flashcam-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.8.5.tar", last modified: Tue Apr  2 04:03:01 2024, max compression
+gzip compressed data, was "flashcam-1.8.6.tar", last modified: Tue Apr  2 04:38:59 2024, max compression
```

## Comparing `flashcam-1.8.5.tar` & `flashcam-1.8.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.761471 flashcam-1.8.5/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 04:03:01.761471 flashcam-1.8.5/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-02 04:02:58.000000 flashcam-1.8.5/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.753471 flashcam-1.8.5/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29232 2024-03-17 02:07:58.000000 flashcam-1.8.5/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.8.5/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.8.5/bin/flashcam_org
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.8.5/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.8.5/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.757471 flashcam-1.8.5/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.8.5/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.8.5/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.761471 flashcam-1.8.5/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/digital-7.regular.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/pattern_acircles.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/pattern_chessboard.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/small_pixel.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.8.5/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.8.5/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50031 2024-04-02 04:02:11.000000 flashcam-1.8.5/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    43919 2024-04-02 03:57:37.000000 flashcam-1.8.5/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   114843 2024-03-22 13:59:53.000000 flashcam-1.8.5/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13417 2024-04-02 03:26:49.000000 flashcam-1.8.5/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.8.5/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40698 2024-04-02 03:34:28.000000 flashcam-1.8.5/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:03:01.761471 flashcam-1.8.5/flashcam.egg-info/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      975 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-02 04:03:01.000000 flashcam-1.8.5/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-02 04:03:01.761471 flashcam-1.8.5/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.8.5/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.231082 flashcam-1.8.6/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 04:38:59.231082 flashcam-1.8.6/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-02 04:38:54.000000 flashcam-1.8.6/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.223082 flashcam-1.8.6/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29232 2024-03-17 02:07:58.000000 flashcam-1.8.6/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.8.6/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.8.6/bin/flashcam_org
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.8.6/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.8.6/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.227082 flashcam-1.8.6/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.8.6/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.8.6/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.227082 flashcam-1.8.6/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/digital-7.regular.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/pattern_acircles.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/pattern_chessboard.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/small_pixel.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.8.6/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50061 2024-04-02 04:32:39.000000 flashcam-1.8.6/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    43977 2024-04-02 04:35:37.000000 flashcam-1.8.6/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   114843 2024-03-22 13:59:53.000000 flashcam-1.8.6/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13417 2024-04-02 03:26:49.000000 flashcam-1.8.6/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.8.6/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40700 2024-04-02 04:28:28.000000 flashcam-1.8.6/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.231082 flashcam-1.8.6/flashcam.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      975 2024-04-02 04:38:59.000000 flashcam-1.8.6/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-02 04:38:59.231082 flashcam-1.8.6/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.8.6/setup.py
```

### Comparing `flashcam-1.8.5/PKG-INFO` & `flashcam-1.8.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.8.5
+Version: 1.8.6
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.8.5/README.md` & `flashcam-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/bin/flashcam` & `flashcam-1.8.6/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/bin/flashcam_org` & `flashcam-1.8.6/bin/flashcam_org`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/bin/flashcam_rep` & `flashcam-1.8.6/bin/flashcam_rep`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/bin/flashcamg` & `flashcam-1.8.6/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/base_camera2.py` & `flashcam-1.8.6/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/config.py` & `flashcam-1.8.6/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.8.6/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.8.6/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/DET_NRDY.jpg` & `flashcam-1.8.6/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/DET_RDY_.jpg` & `flashcam-1.8.6/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/digital-7.mono.ttf` & `flashcam-1.8.6/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/digital-7.regular.ttf` & `flashcam-1.8.6/flashcam/data/digital-7.regular.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/monoskop.jpg` & `flashcam-1.8.6/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/pattern_acircles.png` & `flashcam-1.8.6/flashcam/data/pattern_acircles.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/pattern_chessboard.png` & `flashcam-1.8.6/flashcam/data/pattern_chessboard.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/small_pixel.ttf` & `flashcam-1.8.6/flashcam/data/small_pixel.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/win_rain.jpg` & `flashcam-1.8.6/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/win_skull.jpg` & `flashcam-1.8.6/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/win_storm.jpg` & `flashcam-1.8.6/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/win_winter.jpg` & `flashcam-1.8.6/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/data/windows.jpg` & `flashcam-1.8.6/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/direct.py` & `flashcam-1.8.6/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/izmq_receiver.py` & `flashcam-1.8.6/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/mmapwr.py` & `flashcam-1.8.6/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/real_camera.py` & `flashcam-1.8.6/flashcam/real_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1002,15 +1002,15 @@
                         #-----------exposure in capa
                     # ______________________ section with capa for camera _____________________
 
 
                     #--------------- now apply labels ------i cannot get rid in DETM---
                     #--------- all this will be on all rames histo,detect,direct,delta
                     senh.setbox(" ", senh.TIME, kompr=config.CONFIG['kompress'])
-                    if switch_res:
+                    if config.CONFIG['resolution'] != "640x480":
                         senh.setbox("xzoom", senh.xzoom)
 
                     #senh.setbox(" ", senh.TIME, kompr= frame.shape[1])
 
                     if framekind in ["detect","delta","histo"]:
                         senh.setbox(f"DISP {framekind}",senh.DISP)
                     if average>0:
```

### Comparing `flashcam-1.8.5/flashcam/stream_enhancer.py` & `flashcam-1.8.6/flashcam/stream_enhancer.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         if (row,col) == self.gamma: return (80,80,80) #
 
         if (row,col) == self.speedx: return (180,80,80) #
         if (row,col) == self.speedy: return (80,180,80) #
         if (row,col) == self.avi:    return (30,30,210) # FOR UNI only
         if (row,col) == self.jpg:    return (0,0,250)   # FOR UNI only
         if (row,col) == self.scale:  return (250,0,250)   # zoom scale
-        if (row,col) == self.xzoom:  return (250,100,250)   # xperimental zoom
+        if (row,col) == self.xzoom:  return (0,100,250)   # xperimental zoom
 
         t=[255,255,255]
         while (t[0]+t[1]+t[2]>400) or  (t[0]+t[1]+t[2]<200) :
             t =  (randint(5,255),randint(5,255),randint(5,255) )
         #print(t[0]+t[1]+t[2])
         return t
 
@@ -372,17 +372,18 @@
 
         if (row==6)and(col==0):  side="left"
         if (row==7)and(col==0):  side="left"
         if (row==8)and(col==0):  side="left"
         if (row==9)and(col==0):  side="left"
 
         if (row==10)and(col==0):  side="left"
+        if (row==11)and(col==0):  side="left" # xzoom
 
         if side=="" and row>2:
-            print("X... Too many rows, (0,1,2 only)")
+            print("X... SENH: Too many rows or undef.row ")
             return
 
         #------sides
         if side=="left" or side=="right":
             #print("D.. SIDES", self.maxrow, self.maxcol)
             if row>self.maxrow:
                 print("X... {} rows {} cols allowed".format(self.maxrow,self.maxcol) )
```

### Comparing `flashcam-1.8.5/flashcam/uniwrec.py` & `flashcam-1.8.6/flashcam/uniwrec.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/usbcheck.py` & `flashcam-1.8.6/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/v4lc.py` & `flashcam-1.8.6/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/flashcam/web.py` & `flashcam-1.8.6/flashcam/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1126,17 +1126,17 @@
 
 
     while True:
         time.sleep(0.1)
         framecnt+=1
         #print("D... get_frame (gen)")
 
-        print("D...  gen() - getframe ... ")
+        #print("D...  gen() - getframe ... ")
         frame,b_nframes,b_capture_time = camera.get_frame() # This is BaseCamera method, inherited in Camera
-        print("D...  gen() - gotframe  ")
+        #print("D...  gen() - gotframe  ")
 
         #print("i... got_frame (gen)", frame.shape )
         start = dt.datetime.now()
         blackframe = np.zeros((480,640,3), np.uint8)
         #frame = blackframe
         if blend:
             frame = 0.5*frame + 0.5*imgs[ random.randint(0,len(imgs)-1) ]
```

### Comparing `flashcam-1.8.5/flashcam.egg-info/PKG-INFO` & `flashcam-1.8.6/flashcam.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.8.5
+Version: 1.8.6
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.8.5/flashcam.egg-info/SOURCES.txt` & `flashcam-1.8.6/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.5/setup.py` & `flashcam-1.8.6/setup.py`

 * *Files identical despite different names*

