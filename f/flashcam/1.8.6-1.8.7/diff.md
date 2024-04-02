# Comparing `tmp/flashcam-1.8.6.tar.gz` & `tmp/flashcam-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.8.6.tar", last modified: Tue Apr  2 04:38:59 2024, max compression
+gzip compressed data, was "flashcam-1.8.7.tar", last modified: Tue Apr  2 12:11:07 2024, max compression
```

## Comparing `flashcam-1.8.6.tar` & `flashcam-1.8.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.231082 flashcam-1.8.6/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 04:38:59.231082 flashcam-1.8.6/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-02 04:38:54.000000 flashcam-1.8.6/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.223082 flashcam-1.8.6/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29232 2024-03-17 02:07:58.000000 flashcam-1.8.6/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.8.6/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.8.6/bin/flashcam_org
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.8.6/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.8.6/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.227082 flashcam-1.8.6/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.8.6/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.8.6/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.227082 flashcam-1.8.6/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/digital-7.regular.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/pattern_acircles.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/pattern_chessboard.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/small_pixel.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.8.6/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.8.6/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50061 2024-04-02 04:32:39.000000 flashcam-1.8.6/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    43977 2024-04-02 04:35:37.000000 flashcam-1.8.6/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   114843 2024-03-22 13:59:53.000000 flashcam-1.8.6/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13417 2024-04-02 03:26:49.000000 flashcam-1.8.6/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.8.6/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40700 2024-04-02 04:28:28.000000 flashcam-1.8.6/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 04:38:59.231082 flashcam-1.8.6/flashcam.egg-info/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      975 2024-04-02 04:38:59.000000 flashcam-1.8.6/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-02 04:38:58.000000 flashcam-1.8.6/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-02 04:38:59.231082 flashcam-1.8.6/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.8.6/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:11:07.330137 flashcam-1.8.7/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 12:11:07.330137 flashcam-1.8.7/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-02 12:10:30.000000 flashcam-1.8.7/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:11:07.326137 flashcam-1.8.7/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29232 2024-03-17 02:07:58.000000 flashcam-1.8.7/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.8.7/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.8.7/bin/flashcam_org
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.8.7/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.8.7/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:11:07.326137 flashcam-1.8.7/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.8.7/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.8.7/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:11:07.330137 flashcam-1.8.7/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/digital-7.regular.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/pattern_acircles.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/pattern_chessboard.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/small_pixel.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.8.7/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.8.7/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50103 2024-04-02 12:10:00.000000 flashcam-1.8.7/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    43977 2024-04-02 04:35:37.000000 flashcam-1.8.7/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   114843 2024-03-22 13:59:53.000000 flashcam-1.8.7/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13619 2024-04-02 12:09:15.000000 flashcam-1.8.7/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.8.7/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-02 12:11:06.000000 flashcam-1.8.7/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40700 2024-04-02 04:28:28.000000 flashcam-1.8.7/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:11:07.330137 flashcam-1.8.7/flashcam.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 12:11:07.000000 flashcam-1.8.7/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      975 2024-04-02 12:11:07.000000 flashcam-1.8.7/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-02 12:11:07.000000 flashcam-1.8.7/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-02 12:11:07.000000 flashcam-1.8.7/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-02 12:11:07.000000 flashcam-1.8.7/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-02 12:11:07.330137 flashcam-1.8.7/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.8.7/setup.py
```

### Comparing `flashcam-1.8.6/PKG-INFO` & `flashcam-1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.8.6
+Version: 1.8.7
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.8.6/README.md` & `flashcam-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/bin/flashcam` & `flashcam-1.8.7/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/bin/flashcam_org` & `flashcam-1.8.7/bin/flashcam_org`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/bin/flashcam_rep` & `flashcam-1.8.7/bin/flashcam_rep`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/bin/flashcamg` & `flashcam-1.8.7/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/base_camera2.py` & `flashcam-1.8.7/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/config.py` & `flashcam-1.8.7/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.8.7/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.8.7/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/DET_NRDY.jpg` & `flashcam-1.8.7/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/DET_RDY_.jpg` & `flashcam-1.8.7/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/digital-7.mono.ttf` & `flashcam-1.8.7/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/digital-7.regular.ttf` & `flashcam-1.8.7/flashcam/data/digital-7.regular.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/monoskop.jpg` & `flashcam-1.8.7/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/pattern_acircles.png` & `flashcam-1.8.7/flashcam/data/pattern_acircles.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/pattern_chessboard.png` & `flashcam-1.8.7/flashcam/data/pattern_chessboard.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/small_pixel.ttf` & `flashcam-1.8.7/flashcam/data/small_pixel.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/win_rain.jpg` & `flashcam-1.8.7/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/win_skull.jpg` & `flashcam-1.8.7/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/win_storm.jpg` & `flashcam-1.8.7/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/win_winter.jpg` & `flashcam-1.8.7/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/data/windows.jpg` & `flashcam-1.8.7/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/direct.py` & `flashcam-1.8.7/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/izmq_receiver.py` & `flashcam-1.8.7/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/mmapwr.py` & `flashcam-1.8.7/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/real_camera.py` & `flashcam-1.8.7/flashcam/real_camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,16 @@
         #print("D... init_cam caleld with res:", res )
         #print("i... init_cam caleld with prod:", res )
         #print("D... init_cam caleld with prod:",  config.CONFIG["product"] )
         print("i... init_cam caleld with prod:",  config.CONFIG["product"] )
 
         # here, I need to  wait until the correct video is reported.... ????
         #
-        vids = recommend_video( config.CONFIG["product"]  ) # if jpg => give -1
+        #### HACK ===
+        vids = recommend_video( config.CONFIG["product"] , slow_track = False ) # if jpg => give -1
         #
         # if error is lsusb=>>> return [-1] ??????? or [] ???? test it NONONOO
         #
 
         if len(vids)>0:
             if vids[0]==-1:
                 return config.CONFIG["product"] , -1, None
```

### Comparing `flashcam-1.8.6/flashcam/stream_enhancer.py` & `flashcam-1.8.7/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/uniwrec.py` & `flashcam-1.8.7/flashcam/uniwrec.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/usbcheck.py` & `flashcam-1.8.7/flashcam/usbcheck.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,21 +297,22 @@
         return False
     else:
         return float_n == int_n
 
 
 
 
-def recommend_video( prefname=None ):
+def recommend_video( prefname=None , slow_track = True):
     """
     glob through /dev/video*
     recommend video device:  without paramenter - the list is returned, else if string matches
 
     0     001 006 2.0 	0458:708c 	 Genius WideCam F100 	 14.0-usb-0:9:1.0 	 12e
     ./usbcheck.py "Genius W"
+    rpi with 2 cams...very tedious process - hack slow_track = False
     """
     usb_hubs = usbroot()
 
     if not(prefname is None) and ( prefname.find(".jpg")>=0  or prefname.find("clock")==0   ):
         return [-1] # if image is required
 
     # ====================== nice BUT NOT NEEDED HERE
@@ -367,22 +368,25 @@
                 ok = True
             except  Exception as ex:
                 print("X... udevadm error...", ex, vid, end="\r")
                 ok = False
 
             if ok:
                 # print(f"D...  getting capabilities", )
-                cc = V4L2_CTL( vid )
-                capa = cc.get_capbilities()
-                GE = ""
-                if "gain" in capa:
-                    GE = "g"
-                if "exposure_absolute" in capa:
-                    GE+= "e"
-                # print(   )
+                if slow_track:
+                    cc = V4L2_CTL( vid )
+                    capa = cc.get_capbilities()
+                    GE = ""
+                    if "gain" in capa:
+                        GE = "g"
+                    if "exposure_absolute" in capa:
+                        GE+= "e"
+                    # print(   )
+                else:
+                    capa = 1
 
                 if len(capa) > 0:
                     bus,dev,name = lsusbv(f"{vendor}:{model}")
                     #print(usb_hubs)
                     vidid = int(vid[vid.find('/dev/video')+10:])
                     pref = " "
                     if prefname is None:
```

### Comparing `flashcam-1.8.6/flashcam/v4lc.py` & `flashcam-1.8.7/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam/web.py` & `flashcam-1.8.7/flashcam/web.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/flashcam.egg-info/PKG-INFO` & `flashcam-1.8.7/flashcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.8.6
+Version: 1.8.7
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.8.6/flashcam.egg-info/SOURCES.txt` & `flashcam-1.8.7/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.6/setup.py` & `flashcam-1.8.7/setup.py`

 * *Files identical despite different names*

