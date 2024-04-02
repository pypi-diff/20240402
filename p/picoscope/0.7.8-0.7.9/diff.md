# Comparing `tmp/picoscope-0.7.8.tar.gz` & `tmp/picoscope-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/picoscope-0.7.8.tar", last modified: Mon Dec  2 15:05:18 2019, max compression
+gzip compressed data, was "dist/picoscope-0.7.9.tar", last modified: Fri Feb 28 15:25:49 2020, max compression
```

## Comparing `picoscope-0.7.8.tar` & `picoscope-0.7.9.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-02 15:05:18.000000 picoscope-0.7.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)      111 2019-12-02 15:04:47.000000 picoscope-0.7.8/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-02 15:05:18.000000 picoscope-0.7.8/examples/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1835 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/test_ps3000a.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5540 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/dualview_time_fft.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/specgram_plot.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2176 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/freqmeasure.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/garbageCollectorTest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2764 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/awgdemo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6164 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/radar_capture_functions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1279 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/just_get_connected.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      957 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/test_ps5000a.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      617 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/discover_devices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1085 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/test_ps4000a.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2811 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/ps2000_demo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2275 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/sigGetBuiltIndemo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      954 2019-12-02 15:04:47.000000 picoscope-0.7.8/examples/openUnitAsyncDemo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68611 2019-12-02 15:04:47.000000 picoscope-0.7.8/versioneer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2019-12-02 15:04:47.000000 picoscope-0.7.8/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      751 2019-12-02 15:05:18.000000 picoscope-0.7.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5176 2019-12-02 15:04:47.000000 picoscope-0.7.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-02 15:05:18.000000 picoscope-0.7.8/picoscope.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      751 2019-12-02 15:05:18.000000 picoscope-0.7.8/picoscope.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-12-02 15:05:18.000000 picoscope-0.7.8/picoscope.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-12-02 15:05:18.000000 picoscope-0.7.8/picoscope.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      898 2019-12-02 15:05:18.000000 picoscope-0.7.8/picoscope.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-12-02 15:05:18.000000 picoscope-0.7.8/picoscope.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2019-12-02 15:05:18.000000 picoscope-0.7.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1100 2019-12-02 15:04:47.000000 picoscope-0.7.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-12-02 15:05:18.000000 picoscope-0.7.8/picoscope/
--rw-rw-r--   0 travis    (2000) travis    (2000)    22756 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/ps5000a.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2019-12-02 15:05:18.000000 picoscope-0.7.8/picoscope/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12147 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/error_codes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2410 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/darwin_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24421 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/ps4000a.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23998 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/ps6000.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19237 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/ps2000a.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24475 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/ps4000.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12357 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/ps2000.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19113 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/ps3000a.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      335 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    36660 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/picobase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12035 2019-12-02 15:04:47.000000 picoscope-0.7.8/picoscope/ps3000.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 15:25:49.000000 picoscope-0.7.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      111 2020-02-28 15:25:24.000000 picoscope-0.7.9/MANIFEST.in
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 15:25:49.000000 picoscope-0.7.9/examples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1835 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/test_ps3000a.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5540 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/dualview_time_fft.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/specgram_plot.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2176 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/freqmeasure.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/garbageCollectorTest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2764 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/awgdemo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6164 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/radar_capture_functions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1279 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/just_get_connected.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      957 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/test_ps5000a.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      617 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/discover_devices.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1085 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/test_ps4000a.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2811 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/ps2000_demo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2275 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/sigGetBuiltIndemo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      954 2020-02-28 15:25:24.000000 picoscope-0.7.9/examples/openUnitAsyncDemo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68611 2020-02-28 15:25:24.000000 picoscope-0.7.9/versioneer.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1407 2020-02-28 15:25:24.000000 picoscope-0.7.9/LICENSE.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      751 2020-02-28 15:25:49.000000 picoscope-0.7.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5176 2020-02-28 15:25:24.000000 picoscope-0.7.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 15:25:49.000000 picoscope-0.7.9/picoscope.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      751 2020-02-28 15:25:49.000000 picoscope-0.7.9/picoscope.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-02-28 15:25:49.000000 picoscope-0.7.9/picoscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       10 2020-02-28 15:25:49.000000 picoscope-0.7.9/picoscope.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      918 2020-02-28 15:25:49.000000 picoscope-0.7.9/picoscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2020-02-28 15:25:49.000000 picoscope-0.7.9/picoscope.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      246 2020-02-28 15:25:49.000000 picoscope-0.7.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1100 2020-02-28 15:25:24.000000 picoscope-0.7.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-02-28 15:25:49.000000 picoscope-0.7.9/picoscope/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22756 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/ps5000a.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2020-02-28 15:25:49.000000 picoscope-0.7.9/picoscope/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23761 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/ps5000.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12147 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/error_codes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2410 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/darwin_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24421 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/ps4000a.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23998 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/ps6000.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19237 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/ps2000a.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24475 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/ps4000.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12357 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/ps2000.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19339 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/ps3000a.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      335 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    36660 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/picobase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12035 2020-02-28 15:25:24.000000 picoscope-0.7.9/picoscope/ps3000.py
```

### Comparing `picoscope-0.7.8/examples/test_ps3000a.py` & `picoscope-0.7.9/examples/test_ps3000a.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/dualview_time_fft.py` & `picoscope-0.7.9/examples/dualview_time_fft.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/specgram_plot.py` & `picoscope-0.7.9/examples/specgram_plot.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/freqmeasure.py` & `picoscope-0.7.9/examples/freqmeasure.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/garbageCollectorTest.py` & `picoscope-0.7.9/examples/garbageCollectorTest.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/awgdemo.py` & `picoscope-0.7.9/examples/awgdemo.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/radar_capture_functions.py` & `picoscope-0.7.9/examples/radar_capture_functions.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/just_get_connected.py` & `picoscope-0.7.9/examples/just_get_connected.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/test_ps5000a.py` & `picoscope-0.7.9/examples/test_ps5000a.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/discover_devices.py` & `picoscope-0.7.9/examples/discover_devices.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/test_ps4000a.py` & `picoscope-0.7.9/examples/test_ps4000a.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/ps2000_demo.py` & `picoscope-0.7.9/examples/ps2000_demo.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/sigGetBuiltIndemo.py` & `picoscope-0.7.9/examples/sigGetBuiltIndemo.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/examples/openUnitAsyncDemo.py` & `picoscope-0.7.9/examples/openUnitAsyncDemo.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/versioneer.py` & `picoscope-0.7.9/versioneer.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/LICENSE.md` & `picoscope-0.7.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/PKG-INFO` & `picoscope-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: picoscope
-Version: 0.7.8
+Version: 0.7.9
 Summary: Unofficial python wrapper for the PicoScope devices.
 Home-page: https://github.com/colinoflynn/pico-python/
 Author: Colin O'Flynn, Mark Harfouche
 Author-email: coflynn@newae.com, mark.harfouche@gmail.com
 License: BSD
 Description: UNKNOWN
 Keywords: picoscope peripherals hardware oscilloscope ATE
```

### Comparing `picoscope-0.7.8/README.md` & `picoscope-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope.egg-info/PKG-INFO` & `picoscope-0.7.9/picoscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: picoscope
-Version: 0.7.8
+Version: 0.7.9
 Summary: Unofficial python wrapper for the PicoScope devices.
 Home-page: https://github.com/colinoflynn/pico-python/
 Author: Colin O'Flynn, Mark Harfouche
 Author-email: coflynn@newae.com, mark.harfouche@gmail.com
 License: BSD
 Description: UNKNOWN
 Keywords: picoscope peripherals hardware oscilloscope ATE
```

### Comparing `picoscope-0.7.8/picoscope.egg-info/SOURCES.txt` & `picoscope-0.7.9/picoscope.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 picoscope/picobase.py
 picoscope/ps2000.py
 picoscope/ps2000a.py
 picoscope/ps3000.py
 picoscope/ps3000a.py
 picoscope/ps4000.py
 picoscope/ps4000a.py
+picoscope/ps5000.py
 picoscope/ps5000a.py
 picoscope/ps6000.py
 picoscope.egg-info/PKG-INFO
 picoscope.egg-info/SOURCES.txt
 picoscope.egg-info/dependency_links.txt
 picoscope.egg-info/requires.txt
 picoscope.egg-info/top_level.txt
```

### Comparing `picoscope-0.7.8/setup.py` & `picoscope-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/ps5000a.py` & `picoscope-0.7.9/picoscope/ps5000a.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/error_codes.py` & `picoscope-0.7.9/picoscope/error_codes.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/darwin_utils.py` & `picoscope-0.7.9/picoscope/darwin_utils.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/ps4000a.py` & `picoscope-0.7.9/picoscope/ps4000a.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/ps6000.py` & `picoscope-0.7.9/picoscope/ps6000.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/ps2000a.py` & `picoscope-0.7.9/picoscope/ps2000a.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/ps4000.py` & `picoscope-0.7.9/picoscope/ps4000.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/ps2000.py` & `picoscope-0.7.9/picoscope/ps2000.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/ps3000a.py` & `picoscope-0.7.9/picoscope/ps3000a.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,14 +198,19 @@
     def _lowLevelSetChannel(self, chNum, enabled, coupling, VRange, VOffset,
                             BWLimited):
         m = self.lib.ps3000aSetChannel(c_int16(self.handle), c_enum(chNum),
                                        c_int16(enabled), c_enum(coupling),
                                        c_enum(VRange), c_float(VOffset))
         self.checkResult(m)
 
+        m = self.lib.ps3000aSetBandwidthFilter(c_int16(self.handle),
+                                               c_enum(chNum),
+                                               c_enum(BWLimited))
+        self.checkResult(m)
+
     def _lowLevelStop(self):
         m = self.lib.ps3000aStop(c_int16(self.handle))
         self.checkResult(m)
 
     def _lowLevelGetUnitInfo(self, info):
         s = create_string_buffer(256)
         requiredSize = c_int16(0)
```

### Comparing `picoscope-0.7.8/picoscope/picobase.py` & `picoscope-0.7.9/picoscope/picobase.py`

 * *Files identical despite different names*

### Comparing `picoscope-0.7.8/picoscope/ps3000.py` & `picoscope-0.7.9/picoscope/ps3000.py`

 * *Files identical despite different names*

