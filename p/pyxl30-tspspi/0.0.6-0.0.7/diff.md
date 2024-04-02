# Comparing `tmp/pyxl30-tspspi-0.0.6.tar.gz` & `tmp/pyxl30-tspspi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxl30-tspspi-0.0.6.tar", last modified: Tue Jan 23 14:48:55 2024, max compression
+gzip compressed data, was "pyxl30-tspspi-0.0.7.tar", last modified: Tue Apr  2 16:16:34 2024, max compression
```

## Comparing `pyxl30-tspspi-0.0.6.tar` & `pyxl30-tspspi-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-01-23 14:48:55.843006 pyxl30-tspspi-0.0.6/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1410 2024-01-23 14:48:15.000000 pyxl30-tspspi-0.0.6/LICENSE.md
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2587 2024-01-23 14:48:55.842943 pyxl30-tspspi-0.0.6/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2048 2024-01-23 14:48:15.000000 pyxl30-tspspi-0.0.6/README.md
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      183 2024-01-23 14:48:15.000000 pyxl30-tspspi-0.0.6/pyproject.toml
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      652 2024-01-23 14:48:55.843463 pyxl30-tspspi-0.0.6/setup.cfg
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-01-23 14:48:55.840179 pyxl30-tspspi-0.0.6/src/
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-01-23 14:48:55.842693 pyxl30-tspspi-0.0.6/src/pyxl30_tspspi.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2587 2024-01-23 14:48:55.000000 pyxl30-tspspi-0.0.6/src/pyxl30_tspspi.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)      350 2024-01-23 14:48:55.000000 pyxl30-tspspi-0.0.6/src/pyxl30_tspspi.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)        1 2024-01-23 14:48:55.000000 pyxl30-tspspi-0.0.6/src/pyxl30_tspspi.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)       39 2024-01-23 14:48:55.000000 pyxl30-tspspi-0.0.6/src/pyxl30_tspspi.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)       11 2024-01-23 14:48:55.000000 pyxl30-tspspi-0.0.6/src/pyxl30_tspspi.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-01-23 14:48:55.842432 pyxl30-tspspi-0.0.6/src/xl30serial/
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)        0 2024-01-23 14:48:15.000000 pyxl30-tspspi-0.0.6/src/xl30serial/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)    10020 2024-01-23 14:48:15.000000 pyxl30-tspspi-0.0.6/src/xl30serial/scanningelectronmicroscope.py
--rw-r--r--   0 jenkins   (1002) jenkins   (1002)    51375 2024-01-23 14:48:15.000000 pyxl30-tspspi-0.0.6/src/xl30serial/xl30serial.py
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:34.137574 pyxl30-tspspi-0.0.7/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     1410 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/LICENSE.md
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2588 2024-04-02 16:16:34.137519 pyxl30-tspspi-0.0.7/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2049 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/README.md
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      183 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/pyproject.toml
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      652 2024-04-02 16:16:34.138064 pyxl30-tspspi-0.0.7/setup.cfg
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:34.134713 pyxl30-tspspi-0.0.7/src/
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:34.137236 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)     2588 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)      350 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)        1 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)       39 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)       11 2024-04-02 16:16:34.000000 pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:34.136954 pyxl30-tspspi-0.0.7/src/xl30serial/
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)        0 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/src/xl30serial/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)    10020 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/src/xl30serial/scanningelectronmicroscope.py
+-rw-r--r--   0 jenkins   (1002) jenkins   (1002)    56070 2024-04-02 16:16:16.000000 pyxl30-tspspi-0.0.7/src/xl30serial/xl30serial.py
```

### Comparing `pyxl30-tspspi-0.0.6/LICENSE.md` & `pyxl30-tspspi-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyxl30-tspspi-0.0.6/PKG-INFO` & `pyxl30-tspspi-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxl30-tspspi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Control libraries and utilities for the XL30 ESEM (unofficial)
 Home-page: https://github.com/tspspi/pyxl30
 Author: Thomas Spielauer
 Author-email: pypipackages01@tspi.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -64,8 +64,9 @@
    xl._set_imagefilter_mode(ScanningElectronMicroscope_ImageFilterMode.INTEGRATE, 1)
    while(xl._get_imagefilter_mode()['mode'] != ScanningElectronMicroscope_ImageFilterMode.FREEZE):
       sleep(0.5)
    xl._write_tiff_image("c:\\temp\\IMAGE.TIF")
 
    xl._set_scanmode(ScanningElectronMicroscope_ScanMode.FULL_FRAME)
    xl._set_hightension(0)
+
 ```
```

### Comparing `pyxl30-tspspi-0.0.6/README.md` & `pyxl30-tspspi-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,9 @@
    xl._set_imagefilter_mode(ScanningElectronMicroscope_ImageFilterMode.INTEGRATE, 1)
    while(xl._get_imagefilter_mode()['mode'] != ScanningElectronMicroscope_ImageFilterMode.FREEZE):
       sleep(0.5)
    xl._write_tiff_image("c:\\temp\\IMAGE.TIF")
 
    xl._set_scanmode(ScanningElectronMicroscope_ScanMode.FULL_FRAME)
    xl._set_hightension(0)
+
 ```
```

### Comparing `pyxl30-tspspi-0.0.6/setup.cfg` & `pyxl30-tspspi-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyxl30-tspspi-0.0.6/src/pyxl30_tspspi.egg-info/PKG-INFO` & `pyxl30-tspspi-0.0.7/src/pyxl30_tspspi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxl30-tspspi
-Version: 0.0.6
+Version: 0.0.7
 Summary: Control libraries and utilities for the XL30 ESEM (unofficial)
 Home-page: https://github.com/tspspi/pyxl30
 Author: Thomas Spielauer
 Author-email: pypipackages01@tspi.at
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -64,8 +64,9 @@
    xl._set_imagefilter_mode(ScanningElectronMicroscope_ImageFilterMode.INTEGRATE, 1)
    while(xl._get_imagefilter_mode()['mode'] != ScanningElectronMicroscope_ImageFilterMode.FREEZE):
       sleep(0.5)
    xl._write_tiff_image("c:\\temp\\IMAGE.TIF")
 
    xl._set_scanmode(ScanningElectronMicroscope_ScanMode.FULL_FRAME)
    xl._set_hightension(0)
+
 ```
```

### Comparing `pyxl30-tspspi-0.0.6/src/xl30serial/scanningelectronmicroscope.py` & `pyxl30-tspspi-0.0.7/src/xl30serial/scanningelectronmicroscope.py`

 * *Files identical despite different names*

### Comparing `pyxl30-tspspi-0.0.6/src/xl30serial/xl30serial.py` & `pyxl30-tspspi-0.0.7/src/xl30serial/xl30serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -683,14 +683,157 @@
         if resp['error']:
             self._logger.error(f"Failed to set detector to {detectorId}")
             return False
 
         self._logger.info(f"New detector: {detectorId} ({self._detectorIds[detectorId]['shortname']}: {self._detectorIds[detectorId]['name']})")
         return True
 
+    @onlyconnected()
+    @retrylooped()
+    def _set_linetime(self, lt):
+        supportedLts = {
+            0 : 1.25,
+            1 : 1.87
+            2 : 3.43,
+            3 : 6.86,
+            4 : 20.0,
+            5 : 40.0,
+            6 : 60.0,
+            7 : 120.0,
+            8 : 240.0,
+            9 : 360.0,
+            10 : 1020.0,
+            100 : "TV"
+        }
+
+        setval = None
+        for l in supportedLts:
+            if lt == supportedLts[l]:
+                setval = l
+                break
+        if setval is None:
+            raise ValueError("Unsupported line time {lt} ms, only supporting {supportedLts}")
+
+        self._msg_tx(21, bytes([ setval, 0, 0, 0 ]))
+        resp = self._msg_rx(fmt = "i")
+        if resp['error']:
+            self._logger.error("Failed to set line time {lt} ms")
+            return False
+        self._logger.info("Set line time {lt} ms")
+        return True
+
+    @onlyconnected()
+    @retrylooped()
+    def _get_linetime(self):
+        supportedLts = {
+            0 : 1.25,
+            1 : 1.87
+            2 : 3.43,
+            3 : 6.86,
+            4 : 20.0,
+            5 : 40.0,
+            6 : 60.0,
+            7 : 120.0,
+            8 : 240.0,
+            9 : 360.0,
+            10 : 1020.0,
+            100 : "TV"
+        }
+
+        self._msg_tx(21, fill = 4)
+        resp = self._msg_rx(fmt = "i")
+        if resp['error']:
+            self._logger.error(f"Failed to query line time from XL30")
+            return None
+        v = resp['data'][0]
+
+        for lt in supportedLts:
+            if lt == v:
+                rv = supportedLts[v]
+                self._logger.info(f"Queried line time {rv} ms")
+                return rv
+        self._logger.error(f"Unknown queried line time value {v}")
+        return None
+
+
+
+
+
+    @onlyconnected()
+    @retrylooped()
+    def _set_linesperframe(self, lines):
+        supportedLines = {
+            0 : 121,
+            1 : 242,
+            2 : 484,
+            3 : 968,
+            4 : 1452,
+            5 : 1936,
+            6 : 2420,
+            7 : 2904,
+            8 : 3388,
+            9 : 3872,
+            10 : 180,
+            11 : 360,
+            12 : 720,
+            100 : "TV"
+        }
+
+        setValue = None
+        for l in supportedLines:
+            if lines == supportedLines[l]:
+                setValue = l
+                break
+        if setValue is None:
+            raise ValueError(f"Unspported number of lines {lines}, supporting only {supportedLines}")
+
+        self._msg_tx(19, bytes([ setValue, 0, 0, 0 ]))
+        resp = self._msg_rx(fmt = "i")
+        if resp['error']:
+            self._logger.error(f"Failed to set number of lines to {lines} (value {setValue})")
+            return False
+        else:
+            self._logger.info(f"Set number of lines to {lines}")
+            return True
+
+    @onlyconnected()
+    @retrylooped()
+    def _get_linesperframe(self):
+        supportedLines = {
+            0 : 121,
+            1 : 242,
+            2 : 484,
+            3 : 968,
+            4 : 1452,
+            5 : 1936,
+            6 : 2420,
+            7 : 2904,
+            8 : 3388,
+            9 : 3872,
+            10 : 180,
+            11 : 360,
+            12 : 720,
+            100 : "TV"
+        }
+
+        self._msg_tx(18, fill = 4)
+        resp = self._msg_rx(fmt = "i")
+        if resp['error']:
+            self._logger.error(f"Failed to query number of lines per frame")
+            return None
+        v = resp['data'][0]
+
+        for l in supportedLines:
+            if v == l:
+                self._logger.info(f"Queried {supportedLines[l]} per frame")
+                return supportedLines[l]
+
+        self._logger.error(f"Unknown value for lines per frame: {v}")
+        return None
+
     @tested()
     @onlyconnected()
     @retrylooped()
     def _set_scanmode(self, mode):
         if not isinstance(mode, ScanningElectronMicroscope_ScanMode):
             raise ValueError("Scan mode has to be a ScanningElectronMicroscope_ScanMode")
 
@@ -1058,14 +1201,43 @@
         if resp['error']:
             self._logger.error("Failed to set beamshift")
             return False
 
         self._logger.info(f"New beamshift x={x}mm, y={y}mm")
         return True
 
+    @onlyconnected()
+    @untested()
+    @retrylooped()
+    def _get_scanrotation(self):
+        self._msg_tx(98, fill = 1*4)
+        resp = self._msg_rx(fmt = "f")
+        if resp['error']:
+            self._logger.error("Failed to query scan rotation")
+            return None
+        self._logger.debug(f"Queried scan rotation: {resp['data'][0]} deg")
+        return resp['data'][0]
+
+    @onlyconnected()
+    @untested()
+    @retrylooped()
+    def _set_scanrotation(self, rot = None):
+        rot = float(rot)
+        if (rot < 90) or (rot > 90):
+            self._logger.error("Scan rotation has to be in range +- 90 deg")
+            return False
+        self._msg_tx(99, struct.pack('<f', rot))
+        resp = self._msg_rx(fmt = "f")
+        if resp['error']:
+            self._logger.error("Failed to set scan rotation")
+            return False
+
+        self._logger.info(f"New scan rotation rot={rot}deg")
+        return True
+
     @tested()
     @onlyconnected()
     @retrylooped()
     def _get_area_or_dot_shift(self):
         self._msg_tx(26, fill = 4)
         res = self._msg_rx(fmt = 'f')
         if res['error']:
```

