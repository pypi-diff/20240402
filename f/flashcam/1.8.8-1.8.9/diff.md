# Comparing `tmp/flashcam-1.8.8.tar.gz` & `tmp/flashcam-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashcam-1.8.8.tar", last modified: Tue Apr  2 12:15:14 2024, max compression
+gzip compressed data, was "flashcam-1.8.9.tar", last modified: Tue Apr  2 12:30:20 2024, max compression
```

## Comparing `flashcam-1.8.8.tar` & `flashcam-1.8.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:15:14.025523 flashcam-1.8.8/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 12:15:14.021523 flashcam-1.8.8/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-02 12:15:11.000000 flashcam-1.8.8/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:15:14.017523 flashcam-1.8.8/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29232 2024-03-17 02:07:58.000000 flashcam-1.8.8/bin/flashcam
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.8.8/bin/flashcam_join
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.8.8/bin/flashcam_org
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.8.8/bin/flashcam_rep
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.8.8/bin/flashcamg
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:15:14.021523 flashcam-1.8.8/flashcam/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.8.8/flashcam/base_camera2.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.8.8/flashcam/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:15:14.021523 flashcam-1.8.8/flashcam/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/BEAM_OFF.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/BEAM_ON_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/DET_NRDY.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/DET_RDY_.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/digital-7.mono.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/digital-7.regular.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/monoskop.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/pattern_acircles.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/pattern_chessboard.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/small_pixel.ttf
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/win_rain.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/win_skull.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/win_storm.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/win_winter.jpg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/data/windows.jpg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/direct.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.8.8/flashcam/izmq_receiver.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.8.8/flashcam/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50103 2024-04-02 12:10:00.000000 flashcam-1.8.8/flashcam/real_camera.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    43977 2024-04-02 04:35:37.000000 flashcam-1.8.8/flashcam/stream_enhancer.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)   114843 2024-03-22 13:59:53.000000 flashcam-1.8.8/flashcam/uniwrec.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13650 2024-04-02 12:14:08.000000 flashcam-1.8.8/flashcam/usbcheck.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.8.8/flashcam/v4lc.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-02 12:15:13.000000 flashcam-1.8.8/flashcam/version.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40700 2024-04-02 04:28:28.000000 flashcam-1.8.8/flashcam/web.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:15:14.021523 flashcam-1.8.8/flashcam.egg-info/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 12:15:13.000000 flashcam-1.8.8/flashcam.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      975 2024-04-02 12:15:13.000000 flashcam-1.8.8/flashcam.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-02 12:15:13.000000 flashcam-1.8.8/flashcam.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-02 12:15:13.000000 flashcam-1.8.8/flashcam.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-02 12:15:13.000000 flashcam-1.8.8/flashcam.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-02 12:15:14.025523 flashcam-1.8.8/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.8.8/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.153960 flashcam-1.8.9/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 12:30:20.153960 flashcam-1.8.9/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      901 2024-04-02 12:30:17.000000 flashcam-1.8.9/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.141960 flashcam-1.8.9/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    29232 2024-03-17 02:07:58.000000 flashcam-1.8.9/bin/flashcam
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      150 2023-11-02 08:34:00.000000 flashcam-1.8.9/bin/flashcam_join
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3406 2023-11-02 08:34:00.000000 flashcam-1.8.9/bin/flashcam_org
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      865 2023-11-02 08:34:00.000000 flashcam-1.8.9/bin/flashcam_rep
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      679 2024-02-27 15:50:11.000000 flashcam-1.8.9/bin/flashcamg
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.145959 flashcam-1.8.9/flashcam/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      249 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5401 2024-03-11 10:00:57.000000 flashcam-1.8.9/flashcam/base_camera2.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8850 2024-03-08 14:33:40.000000 flashcam-1.8.9/flashcam/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.153960 flashcam-1.8.9/flashcam/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    24159 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/BEAM_OFF.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27944 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/BEAM_ON_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27715 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/DET_NRDY.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27483 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/DET_RDY_.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34404 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/digital-7.mono.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    34360 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/digital-7.regular.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    19991 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/monoskop.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     7865 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/pattern_acircles.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    22255 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/pattern_chessboard.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    12496 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/small_pixel.ttf
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59930 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/win_rain.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    91079 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/win_skull.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    76270 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/win_storm.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    61604 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/win_winter.jpg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    72731 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/data/windows.jpg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4173 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/direct.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4572 2023-11-02 08:34:00.000000 flashcam-1.8.9/flashcam/izmq_receiver.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4635 2024-03-08 14:33:40.000000 flashcam-1.8.9/flashcam/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    50217 2024-04-02 12:28:54.000000 flashcam-1.8.9/flashcam/real_camera.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    43977 2024-04-02 04:35:37.000000 flashcam-1.8.9/flashcam/stream_enhancer.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)   114843 2024-03-22 13:59:53.000000 flashcam-1.8.9/flashcam/uniwrec.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13650 2024-04-02 12:14:08.000000 flashcam-1.8.9/flashcam/usbcheck.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    36471 2023-11-02 08:59:16.000000 flashcam-1.8.9/flashcam/v4lc.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam/version.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    40773 2024-04-02 12:27:03.000000 flashcam-1.8.9/flashcam/web.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-02 12:30:20.153960 flashcam-1.8.9/flashcam.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     1582 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      975 2024-04-02 12:30:20.000000 flashcam-1.8.9/flashcam.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      165 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        9 2024-04-02 12:30:19.000000 flashcam-1.8.9/flashcam.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-02 12:30:20.153960 flashcam-1.8.9/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2275 2023-11-02 08:34:00.000000 flashcam-1.8.9/setup.py
```

### Comparing `flashcam-1.8.8/PKG-INFO` & `flashcam-1.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.8.8
+Version: 1.8.9
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.8.8/README.md` & `flashcam-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/bin/flashcam` & `flashcam-1.8.9/bin/flashcam`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/bin/flashcam_org` & `flashcam-1.8.9/bin/flashcam_org`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/bin/flashcam_rep` & `flashcam-1.8.9/bin/flashcam_rep`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/bin/flashcamg` & `flashcam-1.8.9/bin/flashcamg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/base_camera2.py` & `flashcam-1.8.9/flashcam/base_camera2.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/config.py` & `flashcam-1.8.9/flashcam/config.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/BEAM_OFF.jpg` & `flashcam-1.8.9/flashcam/data/BEAM_OFF.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/BEAM_ON_.jpg` & `flashcam-1.8.9/flashcam/data/BEAM_ON_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/DET_NRDY.jpg` & `flashcam-1.8.9/flashcam/data/DET_NRDY.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/DET_RDY_.jpg` & `flashcam-1.8.9/flashcam/data/DET_RDY_.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/digital-7.mono.ttf` & `flashcam-1.8.9/flashcam/data/digital-7.mono.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/digital-7.regular.ttf` & `flashcam-1.8.9/flashcam/data/digital-7.regular.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/monoskop.jpg` & `flashcam-1.8.9/flashcam/data/monoskop.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/pattern_acircles.png` & `flashcam-1.8.9/flashcam/data/pattern_acircles.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/pattern_chessboard.png` & `flashcam-1.8.9/flashcam/data/pattern_chessboard.png`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/small_pixel.ttf` & `flashcam-1.8.9/flashcam/data/small_pixel.ttf`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/win_rain.jpg` & `flashcam-1.8.9/flashcam/data/win_rain.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/win_skull.jpg` & `flashcam-1.8.9/flashcam/data/win_skull.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/win_storm.jpg` & `flashcam-1.8.9/flashcam/data/win_storm.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/win_winter.jpg` & `flashcam-1.8.9/flashcam/data/win_winter.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/data/windows.jpg` & `flashcam-1.8.9/flashcam/data/windows.jpg`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/direct.py` & `flashcam-1.8.9/flashcam/direct.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/izmq_receiver.py` & `flashcam-1.8.9/flashcam/izmq_receiver.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/mmapwr.py` & `flashcam-1.8.9/flashcam/mmapwr.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/real_camera.py` & `flashcam-1.8.9/flashcam/real_camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,33 +174,35 @@
         #
 
         if len(vids)>0:
             if vids[0]==-1:
                 return config.CONFIG["product"] , -1, None
 
             vidnum = vids[0]
+            print("D... asking VideoCapture", vidnum )
             cap = cv2.VideoCapture(vidnum,  cv2.CAP_V4L2)
+            print("D... got    VideoCapture", vidnum )
 
             # config.CONFIG["camera_on"] = True
 
             # - with C270 - it showed corrupt jpeg
             # - it allowed to use try: except: and not stuck@!!!
             #cap = cv2.VideoCapture(vidnum)
             #   70% stucks even with timeout
 
 
             #pixelformat = "MJPG"
 
             pixelformat = "YUYV" # I use lossless format for camera readout
             pixelformat = config.CONFIG['PIXELFORMAT']
 
-            time.sleep(1)
+            time.sleep(0.6)
             fourcc = cv2.VideoWriter_fourcc(*pixelformat) # for capture device
             cap.set(cv2.CAP_PROP_FOURCC, fourcc)
-            time.sleep(1)
+            time.sleep(0.6)
 
             w,h =  int(res.split("x")[0]), int(res.split("x")[1])
             print(f"i... {fg.green}   RESOLUTIONwh= {w} x {h}, PIXELFORMAT {pixelformat}  {fg.default}")
             cap.set(cv2.CAP_PROP_FRAME_WIDTH,   w )
             time.sleep(0.5)
             cap.set(cv2.CAP_PROP_FRAME_HEIGHT,  h )
             print(f"i... {fg.green}   RESOLUTIONwh= {w} x {h}, PIXELFORMAT {pixelformat}  {fg.default}")
```

### Comparing `flashcam-1.8.8/flashcam/stream_enhancer.py` & `flashcam-1.8.9/flashcam/stream_enhancer.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/uniwrec.py` & `flashcam-1.8.9/flashcam/uniwrec.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/usbcheck.py` & `flashcam-1.8.9/flashcam/usbcheck.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/v4lc.py` & `flashcam-1.8.9/flashcam/v4lc.py`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/flashcam/web.py` & `flashcam-1.8.9/flashcam/web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1087,15 +1087,16 @@
 # windows  webcamxp ...   jpg  only
 ##### @app.route('/cam_5.cgi')
 @app.route('/video')
 @app.route('/cam_5.jpg')
 @auth.login_required
 def video():
     remote_ip=request.environ.get('HTTP_X_REAL_IP', request.remote_addr)
-    print("W... web is asking VIDEO",request.remote_addr, "(",remote_ip,")")
+    now = dt.datetime.now().strftime("%m/%d %H:%M:%S")
+    print(f"W... {now} web is asking VIDEO",request.remote_addr, "(",remote_ip,")", end="\r")
     logthis( " /video remote      = "+request.remote_addr )
     logthis( " /video remote xreal= "+remote_ip )
     # i return JPG TO AXIS CAMERA....
     #---------------this is MJPEG-------------------------
     #config.CONFIG["product"] = "Webcam C270"
     # return Response(gen(Camera(config.CONFIG["product"], "640x480"),remote_ip),
     # --- i send here the CLASS ?????
@@ -1114,15 +1115,15 @@
 def gen(camera, remote_ip, blend=False, bigtext=True):
     """ returns jpeg;
     MAY do modifications per USER ! BUT any fraME MOD => IS SENT TO ALL!
     can send only some frames
     """
     global  save_bg, frame_bg, frame_bg2, save_fg, frame_fg, frame_fg2, frame_mask, frame_mask_inv #, BGFILE
 
-    print("D... entered gen(), camera = ", camera)
+    #print("D... entered gen(), camera = ", camera)
     framecnt = 0
     framecnttrue = 0
     ss_time = 0
 
 
 
     while True:
```

### Comparing `flashcam-1.8.8/flashcam.egg-info/PKG-INFO` & `flashcam-1.8.9/flashcam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flashcam
-Version: 1.8.8
+Version: 1.8.9
 Summary: Composition of scripts to control a web camera
 Home-page: https://gitlab.com/jaromrax/flashcam
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `flashcam-1.8.8/flashcam.egg-info/SOURCES.txt` & `flashcam-1.8.9/flashcam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashcam-1.8.8/setup.py` & `flashcam-1.8.9/setup.py`

 * *Files identical despite different names*

