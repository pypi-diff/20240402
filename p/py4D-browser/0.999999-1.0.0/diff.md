# Comparing `tmp/py4D_browser-0.999999.tar.gz` & `tmp/py4D_browser-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4D_browser-0.999999.tar", last modified: Wed Feb  7 16:09:13 2024, max compression
+gzip compressed data, was "py4D_browser-1.0.0.tar", last modified: Tue Apr  2 15:40:37 2024, max compression
```

## Comparing `py4D_browser-0.999999.tar` & `py4D_browser-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 sez       (1001) sez       (1001)        0 2024-02-07 16:09:13.416011 py4D_browser-0.999999/
--rw-rw-r--   0 sez       (1001) sez       (1001)    35135 2023-02-15 14:51:18.000000 py4D_browser-0.999999/LICENSE.txt
--rw-r--r--   0 sez       (1001) sez       (1001)     3887 2024-02-07 16:09:13.416011 py4D_browser-0.999999/PKG-INFO
--rw-rw-r--   0 sez       (1001) sez       (1001)     3174 2024-02-06 14:28:27.000000 py4D_browser-0.999999/README.md
--rw-rw-r--   0 sez       (1001) sez       (1001)      983 2024-02-05 19:07:22.000000 py4D_browser-0.999999/pyproject.toml
--rw-rw-r--   0 sez       (1001) sez       (1001)       38 2024-02-07 16:09:13.416011 py4D_browser-0.999999/setup.cfg
-drwxrwxr-x   0 sez       (1001) sez       (1001)        0 2024-02-07 16:09:13.408011 py4D_browser-0.999999/src/
-drwxrwxr-x   0 sez       (1001) sez       (1001)        0 2024-02-07 16:09:13.416011 py4D_browser-0.999999/src/py4D_browser/
--rw-rw-r--   0 sez       (1001) sez       (1001)       48 2023-05-12 19:43:52.000000 py4D_browser-0.999999/src/py4D_browser/__init__.py
--rw-rw-r--   0 sez       (1001) sez       (1001)     2318 2024-02-02 20:24:56.000000 py4D_browser-0.999999/src/py4D_browser/empad2_reader.py
--rw-rw-r--   0 sez       (1001) sez       (1001)     1212 2024-02-02 17:07:05.000000 py4D_browser-0.999999/src/py4D_browser/help_menu.py
--rw-rw-r--   0 sez       (1001) sez       (1001)   140395 2023-05-12 19:43:52.000000 py4D_browser-0.999999/src/py4D_browser/logo.png
--rw-rw-r--   0 sez       (1001) sez       (1001)    21240 2024-02-06 14:35:36.000000 py4D_browser-0.999999/src/py4D_browser/main_window.py
--rw-rw-r--   0 sez       (1001) sez       (1001)     9057 2024-02-05 19:13:47.000000 py4D_browser-0.999999/src/py4D_browser/menu_actions.py
--rw-rw-r--   0 sez       (1001) sez       (1001)   161818 2024-02-02 16:03:15.000000 py4D_browser-0.999999/src/py4D_browser/py4DGUI-keymap.png
--rw-rw-r--   0 sez       (1001) sez       (1001)      271 2023-05-12 19:43:52.000000 py4D_browser-0.999999/src/py4D_browser/runGUI.py
--rw-rw-r--   0 sez       (1001) sez       (1001)     3167 2024-01-17 19:07:55.000000 py4D_browser-0.999999/src/py4D_browser/scalebar.py
--rw-rw-r--   0 sez       (1001) sez       (1001)    17651 2024-02-06 14:15:33.000000 py4D_browser-0.999999/src/py4D_browser/update_views.py
--rw-rw-r--   0 sez       (1001) sez       (1001)     3764 2024-02-05 18:23:21.000000 py4D_browser-0.999999/src/py4D_browser/utils.py
-drwxrwxr-x   0 sez       (1001) sez       (1001)        0 2024-02-07 16:09:13.416011 py4D_browser-0.999999/src/py4D_browser.egg-info/
--rw-r--r--   0 sez       (1001) sez       (1001)     3887 2024-02-07 16:09:13.000000 py4D_browser-0.999999/src/py4D_browser.egg-info/PKG-INFO
--rw-rw-r--   0 sez       (1001) sez       (1001)      613 2024-02-07 16:09:13.000000 py4D_browser-0.999999/src/py4D_browser.egg-info/SOURCES.txt
--rw-rw-r--   0 sez       (1001) sez       (1001)        1 2024-02-07 16:09:13.000000 py4D_browser-0.999999/src/py4D_browser.egg-info/dependency_links.txt
--rw-rw-r--   0 sez       (1001) sez       (1001)       55 2024-02-07 16:09:13.000000 py4D_browser-0.999999/src/py4D_browser.egg-info/entry_points.txt
--rw-rw-r--   0 sez       (1001) sez       (1001)      103 2024-02-07 16:09:13.000000 py4D_browser-0.999999/src/py4D_browser.egg-info/requires.txt
--rw-rw-r--   0 sez       (1001) sez       (1001)       13 2024-02-07 16:09:13.000000 py4D_browser-0.999999/src/py4D_browser.egg-info/top_level.txt
+drwxrwxr-x   0 sez       (1001) sez       (1001)        0 2024-04-02 15:40:37.002447 py4D_browser-1.0.0/
+-rw-rw-r--   0 sez       (1001) sez       (1001)    35134 2024-03-06 18:46:28.000000 py4D_browser-1.0.0/LICENSE.txt
+-rw-r--r--   0 sez       (1001) sez       (1001)     3876 2024-04-02 15:40:37.002447 py4D_browser-1.0.0/PKG-INFO
+-rw-rw-r--   0 sez       (1001) sez       (1001)     3166 2024-03-06 18:46:28.000000 py4D_browser-1.0.0/README.md
+-rw-rw-r--   0 sez       (1001) sez       (1001)      981 2024-03-06 19:04:11.000000 py4D_browser-1.0.0/pyproject.toml
+-rw-rw-r--   0 sez       (1001) sez       (1001)       38 2024-04-02 15:40:37.002447 py4D_browser-1.0.0/setup.cfg
+drwxrwxr-x   0 sez       (1001) sez       (1001)        0 2024-04-02 15:40:36.998447 py4D_browser-1.0.0/src/
+drwxrwxr-x   0 sez       (1001) sez       (1001)        0 2024-04-02 15:40:37.002447 py4D_browser-1.0.0/src/py4D_browser/
+-rw-rw-r--   0 sez       (1001) sez       (1001)       48 2023-05-12 19:43:52.000000 py4D_browser-1.0.0/src/py4D_browser/__init__.py
+-rw-rw-r--   0 sez       (1001) sez       (1001)     2821 2024-04-02 15:33:15.000000 py4D_browser-1.0.0/src/py4D_browser/empad2_reader.py
+-rw-rw-r--   0 sez       (1001) sez       (1001)     1212 2024-02-02 17:07:05.000000 py4D_browser-1.0.0/src/py4D_browser/help_menu.py
+-rw-rw-r--   0 sez       (1001) sez       (1001)   140395 2023-05-12 19:43:52.000000 py4D_browser-1.0.0/src/py4D_browser/logo.png
+-rw-rw-r--   0 sez       (1001) sez       (1001)    22452 2024-03-17 15:06:14.000000 py4D_browser-1.0.0/src/py4D_browser/main_window.py
+-rw-rw-r--   0 sez       (1001) sez       (1001)    11439 2024-03-17 15:09:20.000000 py4D_browser-1.0.0/src/py4D_browser/menu_actions.py
+-rw-rw-r--   0 sez       (1001) sez       (1001)   161818 2024-02-02 16:03:15.000000 py4D_browser-1.0.0/src/py4D_browser/py4DGUI-keymap.png
+-rw-rw-r--   0 sez       (1001) sez       (1001)      271 2023-05-12 19:43:52.000000 py4D_browser-1.0.0/src/py4D_browser/runGUI.py
+-rw-rw-r--   0 sez       (1001) sez       (1001)     3167 2024-01-17 19:07:55.000000 py4D_browser-1.0.0/src/py4D_browser/scalebar.py
+-rw-rw-r--   0 sez       (1001) sez       (1001)    19284 2024-03-06 18:35:52.000000 py4D_browser-1.0.0/src/py4D_browser/update_views.py
+-rw-rw-r--   0 sez       (1001) sez       (1001)     7326 2024-03-17 14:48:23.000000 py4D_browser-1.0.0/src/py4D_browser/utils.py
+drwxrwxr-x   0 sez       (1001) sez       (1001)        0 2024-04-02 15:40:37.002447 py4D_browser-1.0.0/src/py4D_browser.egg-info/
+-rw-r--r--   0 sez       (1001) sez       (1001)     3876 2024-04-02 15:40:36.000000 py4D_browser-1.0.0/src/py4D_browser.egg-info/PKG-INFO
+-rw-rw-r--   0 sez       (1001) sez       (1001)      613 2024-04-02 15:40:36.000000 py4D_browser-1.0.0/src/py4D_browser.egg-info/SOURCES.txt
+-rw-rw-r--   0 sez       (1001) sez       (1001)        1 2024-04-02 15:40:36.000000 py4D_browser-1.0.0/src/py4D_browser.egg-info/dependency_links.txt
+-rw-rw-r--   0 sez       (1001) sez       (1001)       55 2024-04-02 15:40:36.000000 py4D_browser-1.0.0/src/py4D_browser.egg-info/entry_points.txt
+-rw-rw-r--   0 sez       (1001) sez       (1001)      103 2024-04-02 15:40:36.000000 py4D_browser-1.0.0/src/py4D_browser.egg-info/requires.txt
+-rw-rw-r--   0 sez       (1001) sez       (1001)       13 2024-04-02 15:40:36.000000 py4D_browser-1.0.0/src/py4D_browser.egg-info/top_level.txt
```

### Comparing `py4D_browser-0.999999/LICENSE.txt` & `py4D_browser-1.0.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -668,8 +668,7 @@
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
 <https://www.gnu.org/licenses/why-not-lgpl.html>.
-
```

### Comparing `py4D_browser-0.999999/PKG-INFO` & `py4D_browser-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4D_browser
-Version: 0.999999
+Version: 1.0.0
 Summary: A 4D-STEM data browser built on py4DSTEM.
 Author-email: Steven Zeltmann <steven.zeltmann@lbl.gov>
 Project-URL: Homepage, https://github.com/py4dstem/py4D-browser
 Project-URL: Bug Tracker, https://github.com/py4dstem/py4D-browser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -18,41 +18,41 @@
 Requires-Dist: PyQt5>=5.10
 Requires-Dist: pyqtgraph>=0.11
 Requires-Dist: sigfig
 
 
 # The `py4DSTEM` GUI
 
-This repository hosts the `pyqt` based graphical 4D--STEM data browser that was originally part of **py4DSTEM** until version 0.13.11. 
+This repository hosts the `pyqt` based graphical 4D--STEM data browser that was originally part of **py4DSTEM** until version 0.13.11.
 
-## Installation 
-The GUI is available on PyPI and conda-forge: 
+## Installation
+The GUI is available on PyPI and conda-forge:
 
 `pip install py4D-browser`
 
 `conda install -c conda-forge py4d-browser`
 
 
 ## Usage
 Run `py4DGUI` in your terminal to open the GUI. Then just drag and drop a 4D-STEM dataset into the window!
 
 ### Controls
-* Move the virtual detector and the real-space selector using the mouse or using the keyboard shortcuts: WASD moves the detector and IJKL moves the selector, and holding down shift moves 5 pixels at a time. 
-* Auto scaling of both views is on by default. Press the "Autoscale" buttons in the bottom right to disable. Press either button to apply automatic scaling once, or Shift + click to lock autoscaling back on. 
+* Move the virtual detector and the real-space selector using the mouse or using the keyboard shortcuts: WASD moves the detector and IJKL moves the selector, and holding down shift moves 5 pixels at a time.
+* Auto scaling of both views is on by default. Press the "Autoscale" buttons in the bottom right to disable. Press either button to apply automatic scaling once, or Shift + click to lock autoscaling back on.
 * Different shapes of virtual detector are available in the "Detector Shape" menu, and different detector responses are available in the "Detector Response" menu.
-* The information in the bottom bar contains the details of the virtual detector used to generate the images, and can be entered into py4DSTEM to generate the same image. 
+* The information in the bottom bar contains the details of the virtual detector used to generate the images, and can be entered into py4DSTEM to generate the same image.
 * The FFT pane can be switched between displaying the FFT of the virtual image and displaying the [exit wave power cepstrum](https://doi.org/10.1016/j.ultramic.2020.112994).
 * Virtual images can be exported either as the scaled and clipped displays shown in the GUI or as raw data. The exact datatype stored in the raw TIFF image depends on both the datatype of the dataset and the type of virtual image being displayed (in particular, integer datatypes are converted internally to floating point to prevent overflows when generating any synthesized virtual images).
-* If the [EMPAD-G2 Raw Reader](https://github.com/sezelt/empad2) is installed in the same environment, an extra menu will appear that allows the concatenated binary format data to be background subtracted and calibrated in the GUI. You can also save the calibrated data as an HDF5 file for later analysis. 
+* If the [EMPAD-G2 Raw Reader](https://github.com/sezelt/empad2) is installed in the same environment, an extra menu will appear that allows the concatenated binary format data to be background subtracted and calibrated in the GUI. You can also save the calibrated data as an HDF5 file for later analysis.
 
 ![Demonstration](/images/demo.gif)
 
 The keyboard map in the Help menu was made using [this tool](https://archie-adams.github.io/keyboard-shortcut-map-maker/) and the map file is in the top level of this repo.
 
-## About 
+## About
 
 ![py4DSTEM logo](/images/py4DSTEM_logo.png)
 
 **py4DSTEM** is an open source set of python tools for processing and analysis of four-dimensional scanning transmission electron microscopy (4D-STEM) data. Additional information:
 
 - [Our open access py4DSTEM publication in Microscopy and Microanalysis](https://doi.org/10.1017/S1431927621000477) describing this project and demonstrating a variety of applications.
 - [The py4DSTEM documentation pages](https://py4dstem.readthedocs.io/en/latest/index.html).
```

### Comparing `py4D_browser-0.999999/README.md` & `py4D_browser-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 
 # The `py4DSTEM` GUI
 
-This repository hosts the `pyqt` based graphical 4D--STEM data browser that was originally part of **py4DSTEM** until version 0.13.11. 
+This repository hosts the `pyqt` based graphical 4D--STEM data browser that was originally part of **py4DSTEM** until version 0.13.11.
 
-## Installation 
-The GUI is available on PyPI and conda-forge: 
+## Installation
+The GUI is available on PyPI and conda-forge:
 
 `pip install py4D-browser`
 
 `conda install -c conda-forge py4d-browser`
 
 
 ## Usage
 Run `py4DGUI` in your terminal to open the GUI. Then just drag and drop a 4D-STEM dataset into the window!
 
 ### Controls
-* Move the virtual detector and the real-space selector using the mouse or using the keyboard shortcuts: WASD moves the detector and IJKL moves the selector, and holding down shift moves 5 pixels at a time. 
-* Auto scaling of both views is on by default. Press the "Autoscale" buttons in the bottom right to disable. Press either button to apply automatic scaling once, or Shift + click to lock autoscaling back on. 
+* Move the virtual detector and the real-space selector using the mouse or using the keyboard shortcuts: WASD moves the detector and IJKL moves the selector, and holding down shift moves 5 pixels at a time.
+* Auto scaling of both views is on by default. Press the "Autoscale" buttons in the bottom right to disable. Press either button to apply automatic scaling once, or Shift + click to lock autoscaling back on.
 * Different shapes of virtual detector are available in the "Detector Shape" menu, and different detector responses are available in the "Detector Response" menu.
-* The information in the bottom bar contains the details of the virtual detector used to generate the images, and can be entered into py4DSTEM to generate the same image. 
+* The information in the bottom bar contains the details of the virtual detector used to generate the images, and can be entered into py4DSTEM to generate the same image.
 * The FFT pane can be switched between displaying the FFT of the virtual image and displaying the [exit wave power cepstrum](https://doi.org/10.1016/j.ultramic.2020.112994).
 * Virtual images can be exported either as the scaled and clipped displays shown in the GUI or as raw data. The exact datatype stored in the raw TIFF image depends on both the datatype of the dataset and the type of virtual image being displayed (in particular, integer datatypes are converted internally to floating point to prevent overflows when generating any synthesized virtual images).
-* If the [EMPAD-G2 Raw Reader](https://github.com/sezelt/empad2) is installed in the same environment, an extra menu will appear that allows the concatenated binary format data to be background subtracted and calibrated in the GUI. You can also save the calibrated data as an HDF5 file for later analysis. 
+* If the [EMPAD-G2 Raw Reader](https://github.com/sezelt/empad2) is installed in the same environment, an extra menu will appear that allows the concatenated binary format data to be background subtracted and calibrated in the GUI. You can also save the calibrated data as an HDF5 file for later analysis.
 
 ![Demonstration](/images/demo.gif)
 
 The keyboard map in the Help menu was made using [this tool](https://archie-adams.github.io/keyboard-shortcut-map-maker/) and the map file is in the top level of this repo.
 
-## About 
+## About
 
 ![py4DSTEM logo](/images/py4DSTEM_logo.png)
 
 **py4DSTEM** is an open source set of python tools for processing and analysis of four-dimensional scanning transmission electron microscopy (4D-STEM) data. Additional information:
 
 - [Our open access py4DSTEM publication in Microscopy and Microanalysis](https://doi.org/10.1017/S1431927621000477) describing this project and demonstrating a variety of applications.
 - [The py4DSTEM documentation pages](https://py4dstem.readthedocs.io/en/latest/index.html).
```

### Comparing `py4D_browser-0.999999/pyproject.toml` & `py4D_browser-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py4D_browser"
-version = "0.999999"
+version = "1.0.0"
 authors = [
   { name="Steven Zeltmann", email="steven.zeltmann@lbl.gov" },
 ]
 description = "A 4D-STEM data browser built on py4DSTEM."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -39,8 +39,8 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-py4D_browser = ["*.png"]
+py4D_browser = ["*.png"]
```

### Comparing `py4D_browser-0.999999/src/py4D_browser/empad2_reader.py` & `py4D_browser-1.0.0/src/py4D_browser/empad2_reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 import empad2
-from PyQt5.QtWidgets import QFileDialog, QMessageBox
+from PyQt5.QtWidgets import QFileDialog, QMessageBox, QApplication
 import numpy as np
 
 
+class StatusBarWriter:
+    def __init__(self, statusBar):
+        self.statusBar = statusBar
+        self.app = app = QApplication.instance()
+
+    def write(self, message):
+        self.statusBar.showMessage(message, 1_000)
+        self.app.processEvents()
+
+    def flush(self):
+        pass
+
+
 def set_empad2_sensor(self, sensor_name):
     self.empad2_calibrations = empad2.load_calibration_data(sensor=sensor_name)
     self.statusBar().showMessage(f"{sensor_name} calibrations loaded", 5_000)
 
 
 def load_empad2_background(self):
     if self.empad2_calibrations is not None:
@@ -37,15 +50,22 @@
                     "even": np.zeros((128, 128), dtype=np.float32),
                     "odd": np.zeros((128, 128), dtype=np.float32),
                 }
                 dummy_data = True
 
         filename = raw_file_dialog(self)
         self.datacube = empad2.load_dataset(
-            filename, self.empad2_background, self.empad2_calibrations
+            filename,
+            self.empad2_background,
+            self.empad2_calibrations,
+            _tqdm_args={
+                "desc": "Loading",
+                "file": StatusBarWriter(self.statusBar()),
+                "mininterval": 1.0,
+            },
         )
 
         if dummy_data:
             self.empad2_background = None
 
         self.update_diffraction_space_view(reset=True)
         self.update_real_space_view(reset=True)
```

### Comparing `py4D_browser-0.999999/src/py4D_browser/help_menu.py` & `py4D_browser-1.0.0/src/py4D_browser/help_menu.py`

 * *Files identical despite different names*

### Comparing `py4D_browser-0.999999/src/py4D_browser/logo.png` & `py4D_browser-1.0.0/src/py4D_browser/logo.png`

 * *Files identical despite different names*

### Comparing `py4D_browser-0.999999/src/py4D_browser/main_window.py` & `py4D_browser-1.0.0/src/py4D_browser/main_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,22 +30,24 @@
         app.exec_()
     """
 
     LOG_SCALE_MIN_VALUE = 1e-6
 
     from py4D_browser.menu_actions import (
         load_file,
+        load_data_arina,
         load_data_auto,
         load_data_bin,
         load_data_mmap,
         show_file_dialog,
         get_savefile_name,
         export_datacube,
         export_virtual_image,
         show_keyboard_map,
+        reshape_data,
     )
 
     from py4D_browser.update_views import (
         update_diffraction_space_view,
         update_real_space_view,
         update_realspace_detector,
         update_diffraction_detector,
@@ -111,14 +113,22 @@
         self.load_mmap_action.triggered.connect(self.load_data_mmap)
         self.file_menu.addAction(self.load_mmap_action)
 
         self.load_binned_action = QAction("Load Data &Binned...", self)
         self.load_binned_action.triggered.connect(self.load_data_bin)
         self.file_menu.addAction(self.load_binned_action)
 
+        self.load_arina_action = QAction("Load &Arina Data...", self)
+        self.load_arina_action.triggered.connect(self.load_data_arina)
+        self.file_menu.addAction(self.load_arina_action)
+
+        self.reshape_data_action = QAction("&Reshape Data...", self)
+        self.reshape_data_action.triggered.connect(self.reshape_data)
+        self.file_menu.addAction(self.reshape_data_action)
+
         self.file_menu.addSeparator()
 
         export_label = QAction("Export", self)
         export_label.setDisabled(True)
         self.file_menu.addAction(export_label)
 
         # Submenu to export datacube
@@ -356,21 +366,30 @@
         self.menu_bar.addMenu(self.fft_menu)
 
         self.fft_source_action_group = QActionGroup(self)
         self.fft_source_action_group.setExclusive(True)
         img_fft_action = QAction("Virtual Image FFT", self)
         img_fft_action.setCheckable(True)
         img_fft_action.setChecked(True)
+        img_fft_action.triggered.connect(partial(self.update_real_space_view, False))
         self.fft_menu.addAction(img_fft_action)
         self.fft_source_action_group.addAction(img_fft_action)
+
+        img_complex_fft_action = QAction("Virtual Image FFT (complex)", self)
+        img_complex_fft_action.setCheckable(True)
+        self.fft_menu.addAction(img_complex_fft_action)
+        self.fft_source_action_group.addAction(img_complex_fft_action)
+        img_complex_fft_action.triggered.connect(
+            partial(self.update_real_space_view, False)
+        )
+
         img_ewpc_action = QAction("EWPC", self)
         img_ewpc_action.setCheckable(True)
         self.fft_menu.addAction(img_ewpc_action)
         self.fft_source_action_group.addAction(img_ewpc_action)
-        img_fft_action.triggered.connect(partial(self.update_real_space_view, False))
         img_ewpc_action.triggered.connect(
             partial(self.update_diffraction_space_view, False)
         )
 
         self.help_menu = QMenu("&Help", self)
         self.menu_bar.addMenu(self.help_menu)
 
@@ -462,14 +481,20 @@
         self.setCentralWidget(widget)
 
         self.diffraction_space_widget.getView().setMenuEnabled(False)
         self.real_space_widget.getView().setMenuEnabled(False)
         self.fft_widget.getView().setMenuEnabled(False)
 
         # Setup Status Bar
+        self.realspace_statistics_text = QLabel("Image Stats")
+        self.diffraction_statistics_text = QLabel("Diffraction Stats")
+        self.statusBar().addPermanentWidget(VLine())
+        self.statusBar().addPermanentWidget(self.realspace_statistics_text)
+        self.statusBar().addPermanentWidget(VLine())
+        self.statusBar().addPermanentWidget(self.diffraction_statistics_text)
         self.statusBar().addPermanentWidget(VLine())
         self.statusBar().addPermanentWidget(self.diffraction_space_view_text)
         self.statusBar().addPermanentWidget(VLine())
         self.statusBar().addPermanentWidget(self.real_space_view_text)
         self.statusBar().addPermanentWidget(VLine())
         self.diffraction_rescale_button = LatchingButton(
             "Autoscale Diffraction",
```

### Comparing `py4D_browser-0.999999/src/py4D_browser/menu_actions.py` & `py4D_browser-1.0.0/src/py4D_browser/menu_actions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from numbers import Real
 import py4DSTEM
 from PyQt5.QtWidgets import QFileDialog, QMessageBox
 import h5py
 import os
 import numpy as np
 import matplotlib.pyplot as plt
 from py4D_browser.help_menu import KeyboardMapMenu
+from py4D_browser.utils import ResizeDialog
+from py4DSTEM.io.filereaders import read_arina
 
 
 def load_data_auto(self):
     filename = self.show_file_dialog()
     self.load_file(filename)
 
 
@@ -19,20 +22,56 @@
 
 def load_data_bin(self):
     # TODO: Ask user for binning level
     filename = self.show_file_dialog()
     self.load_file(filename, mmap=False, binning=4)
 
 
+def load_data_arina(self):
+    filename = self.show_file_dialog()
+    dataset = read_arina(filename)
+
+    # Try to reshape the data to be square
+    N_patterns = dataset.data.shape[1]
+    Nxy = np.sqrt(N_patterns)
+    if np.abs(Nxy - np.round(Nxy)) <= 1e-10:
+        Nxy = int(Nxy)
+        dataset.data = dataset.data.reshape(
+            Nxy, Nxy, dataset.data.shape[2], dataset.data.shape[3]
+        )
+    else:
+        self.statusBar().showMessage(
+            f"The scan appears to not be square! Found {N_patterns} patterns", 5_000
+        )
+
+    self.datacube = dataset
+    self.diffraction_scale_bar.pixel_size = self.datacube.calibration.get_Q_pixel_size()
+    self.diffraction_scale_bar.units = self.datacube.calibration.get_Q_pixel_units()
+
+    self.real_space_scale_bar.pixel_size = self.datacube.calibration.get_R_pixel_size()
+    self.real_space_scale_bar.units = self.datacube.calibration.get_R_pixel_units()
+
+    self.fft_scale_bar.pixel_size = (
+        1.0 / self.datacube.calibration.get_R_pixel_size() / self.datacube.R_Ny
+    )
+    self.fft_scale_bar.units = f"1/{self.datacube.calibration.get_R_pixel_units()}"
+
+    self.update_diffraction_space_view(reset=True)
+    self.update_real_space_view(reset=True)
+
+    self.setWindowTitle(filename)
+
+
 def load_file(self, filepath, mmap=False, binning=1):
     print(f"Loading file {filepath}")
     extension = os.path.splitext(filepath)[-1].lower()
     print(f"Type: {extension}")
-    if extension in (".h5", ".hdf5", ".py4dstem", ".emd"):
-        datacubes = get_4D(h5py.File(filepath, "r"))
+    if extension in (".h5", ".hdf5", ".py4dstem", ".emd", ".mat"):
+        file = h5py.File(filepath, "r")
+        datacubes = get_ND(file)
         print(f"Found {len(datacubes)} 4D datasets inside the HDF5 file...")
         if len(datacubes) >= 1:
             # Read the first datacube in the HDF5 file into RAM
             print(f"Reading dataset at location {datacubes[0].name}")
             self.datacube = py4DSTEM.DataCube(
                 datacubes[0] if mmap else datacubes[0][()]
             )
@@ -41,15 +80,25 @@
 
             self.datacube.calibration.set_R_pixel_size(R_size)
             self.datacube.calibration.set_R_pixel_units(R_units)
             self.datacube.calibration.set_Q_pixel_size(Q_size)
             self.datacube.calibration.set_Q_pixel_units(Q_units)
 
         else:
-            raise ValueError("No 4D data detected in the H5 file!")
+            # if no 4D data was found, look for 3D data
+            datacubes = get_ND(file, N=3)
+            print(f"Found {len(datacubes)} 3D datasets inside the HDF5 file...")
+            if len(datacubes) >= 1:
+                array = datacubes[0] if mmap else datacubes[0][()]
+                new_shape = ResizeDialog.get_new_size([1, array.shape[0]], parent=self)
+                self.datacube = py4DSTEM.DataCube(
+                    array.reshape(*new_shape, *array.shape[1:])
+                )
+            else:
+                raise ValueError("No 4D (or even 3D) data detected in the H5 file!")
     elif extension in [".npy"]:
         self.datacube = py4DSTEM.DataCube(np.load(filepath))
     else:
         self.datacube = py4DSTEM.import_file(
             filepath,
             mem="MEMMAP" if mmap else "RAM",
             binfactor=binning,
@@ -68,14 +117,26 @@
 
     self.update_diffraction_space_view(reset=True)
     self.update_real_space_view(reset=True)
 
     self.setWindowTitle(filepath)
 
 
+def reshape_data(self):
+    new_shape = ResizeDialog.get_new_size(self.datacube.shape[:2], parent=self)
+    self.datacube.data = self.datacube.data.reshape(
+        *new_shape, *self.datacube.data.shape[2:]
+    )
+
+    print(f"Reshaping data to {new_shape}")
+
+    self.update_diffraction_space_view(reset=True)
+    self.update_real_space_view(reset=True)
+
+
 def export_datacube(self, save_format: str):
     assert save_format in [
         "Raw float32",
         "py4DSTEM HDF5",
         "Plain HDF5",
     ], f"unrecognized format {format}"
     assert self.datacube is not None, "No datacube!"
@@ -152,15 +213,15 @@
 
 
 def show_file_dialog(self) -> str:
     filename = QFileDialog.getOpenFileName(
         self,
         "Open 4D-STEM Data",
         "",
-        "4D-STEM Data (*.dm3 *.dm4 *.raw *.mib *.gtg *.h5 *.hdf5 *.emd *.py4dstem *.npy *.npz);;Any file (*)",
+        "4D-STEM Data (*.dm3 *.dm4 *.raw *.mib *.gtg *.h5 *.hdf5 *.emd *.py4dstem *.npy *.npz *.mat);;Any file (*)",
     )
     if filename is not None and len(filename[0]) > 0:
         return filename[0]
     else:
         print("File was invalid, or something?")
         raise ValueError("Could not read file")
 
@@ -203,24 +264,25 @@
         return fname
     else:
         print("File was invalid, or something?")
         print(f"QFileDialog returned {filename}")
         raise ValueError("Could get save file")
 
 
-def get_4D(f, datacubes=None):
+def get_ND(f, datacubes=None, N=4):
+    # Traverse an h5py.File and look for Datasets with N dimensions
     if datacubes is None:
         datacubes = []
     for k in f.keys():
         if isinstance(f[k], h5py.Dataset):
             # we found data
-            if len(f[k].shape) == 4:
+            if len(f[k].shape) == N:
                 datacubes.append(f[k])
         elif isinstance(f[k], h5py.Group):
-            get_4D(f[k], datacubes)
+            get_ND(f[k], datacubes)
     return datacubes
 
 
 def find_calibrations(dset: h5py.Dataset):
     # Attempt to find calibrations from an H5 file
     R_size, R_units, Q_size, Q_units = 1.0, "pixels", 1.0, "pixels"
```

### Comparing `py4D_browser-0.999999/src/py4D_browser/py4DGUI-keymap.png` & `py4D_browser-1.0.0/src/py4D_browser/py4DGUI-keymap.png`

 * *Files identical despite different names*

### Comparing `py4D_browser-0.999999/src/py4D_browser/scalebar.py` & `py4D_browser-1.0.0/src/py4D_browser/scalebar.py`

 * *Files identical despite different names*

### Comparing `py4D_browser-0.999999/src/py4D_browser/update_views.py` & `py4D_browser-1.0.0/src/py4D_browser/update_views.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pyqtgraph as pg
 import numpy as np
 import py4DSTEM
 from functools import partial
 
-from py4D_browser.utils import pg_point_roi, make_detector
+from py4D_browser.utils import pg_point_roi, make_detector, complex_to_Lab
 
 
 def update_real_space_view(self, reset=False):
     scaling_mode = self.vimg_scaling_group.checkedAction().text().replace("&", "")
     assert scaling_mode in ["Linear", "Log", "Square Root"], scaling_mode
 
     detector_shape = self.detector_shape_group.checkedAction().text().replace("&", "")
@@ -170,17 +170,28 @@
     elif scaling_mode == "Square Root":
         new_view = np.sqrt(np.maximum(vimg, 0))
     else:
         raise ValueError("Mode not recognized")
 
     self.unscaled_realspace_image = vimg
 
+    self.realspace_statistics_text.setToolTip(
+        f"min\t{vimg.min():.5g}\nmax\t{vimg.max():.5g}\nmean\t{vimg.mean():.5g}\nsum\t{vimg.sum():.5g}\nstd\t{np.std(vimg):.5g}"
+    )
+
+    auto_level = reset or self.realspace_rescale_button.latched
+
     self.real_space_widget.setImage(
         new_view.T,
-        autoLevels=reset or self.realspace_rescale_button.latched,
+        autoLevels=False,
+        levels=(
+            (np.percentile(new_view, 2), np.percentile(new_view, 98))
+            if auto_level
+            else None
+        ),
         autoRange=reset,
     )
 
     # Update FFT view
     if self.fft_source_action_group.checkedAction().text() == "Virtual Image FFT":
         fft = np.abs(np.fft.fftshift(np.fft.fft2(new_view))) ** 0.5
         levels = (np.min(fft), np.percentile(fft, 99.9))
@@ -189,14 +200,40 @@
         self.fft_widget.setImage(
             fft.T, autoLevels=False, levels=levels, autoRange=mode_switch
         )
         self.fft_widget.getImageItem().setRect(0, 0, fft.shape[1], fft.shape[1])
         if mode_switch:
             # Need to autorange after setRect
             self.fft_widget.autoRange()
+    elif (
+        self.fft_source_action_group.checkedAction().text()
+        == "Virtual Image FFT (complex)"
+    ):
+        fft = np.fft.fftshift(np.fft.fft2(new_view))
+        levels = (np.min(np.abs(fft)), np.percentile(np.abs(fft), 99.9))
+        mode_switch = self.fft_widget_text.textItem.toPlainText() != "Virtual Image FFT"
+        self.fft_widget_text.setText("Virtual Image FFT")
+        fft_img = complex_to_Lab(
+            fft.T,
+            amin=levels[0],
+            amax=levels[1],
+            ab_scale=128,
+            gamma=0.5,
+        )
+        self.fft_widget.setImage(
+            fft_img,
+            autoLevels=False,
+            autoRange=mode_switch,
+            levels=(0, 1),
+        )
+
+        self.fft_widget.getImageItem().setRect(0, 0, fft.shape[1], fft.shape[1])
+        if mode_switch:
+            # Need to autorange after setRect
+            self.fft_widget.autoRange()
 
 
 def update_diffraction_space_view(self, reset=False):
     scaling_mode = self.diff_scaling_group.checkedAction().text().replace("&", "")
     assert scaling_mode in ["Linear", "Log", "Square Root"]
 
     if self.datacube is None:
@@ -247,17 +284,28 @@
     elif scaling_mode == "Log":
         new_view = np.log2(np.maximum(DP, self.LOG_SCALE_MIN_VALUE))
     elif scaling_mode == "Square Root":
         new_view = np.sqrt(np.maximum(DP, 0))
     else:
         raise ValueError("Mode not recognized")
 
+    self.diffraction_statistics_text.setToolTip(
+        f"min\t{DP.min():.5g}\nmax\t{DP.max():.5g}\nmean\t{DP.mean():.5g}\nsum\t{DP.sum():.5g}\nstd\t{np.std(DP):.5g}"
+    )
+
+    auto_level = reset or self.diffraction_rescale_button.latched
+
     self.diffraction_space_widget.setImage(
         new_view.T,
-        autoLevels=reset or self.diffraction_rescale_button.latched,
+        autoLevels=False,
+        levels=(
+            (np.percentile(new_view, 2), np.percentile(new_view, 98))
+            if auto_level
+            else None
+        ),
         autoRange=reset,
     )
 
     if self.fft_source_action_group.checkedAction().text() == "EWPC":
         log_clip = np.maximum(1e-10, np.percentile(np.maximum(DP, 0.0), 0.1))
         fft = np.abs(np.fft.fftshift(np.fft.fft2(np.log(np.maximum(DP, log_clip)))))
         levels = (np.min(fft), np.percentile(fft, 99.9))
@@ -275,15 +323,15 @@
         self.rs_detector_shape_group.checkedAction().text().replace("&", "")
     )
     assert detector_shape in ["Point", "Rectangular"], detector_shape
 
     if self.datacube is None:
         return
 
-    x, y = self.datacube.shape[2:]
+    x, y = self.datacube.data.shape[:2]
     x0, y0 = x / 2, y / 2
     xr, yr = x / 10, y / 10
 
     # Remove existing detector
     if hasattr(self, "real_space_point_selector"):
         self.real_space_widget.view.scene().removeItem(self.real_space_point_selector)
         self.real_space_point_selector = None
@@ -318,15 +366,15 @@
 
     detector_shape = self.detector_shape_group.checkedAction().text().strip("&")
     assert detector_shape in ["Point", "Rectangular", "Circle", "Annulus"]
 
     if self.datacube is None:
         return
 
-    x, y = self.datacube.shape[2:]
+    x, y = self.datacube.data.shape[2:]
     x0, y0 = x / 2, y / 2
     xr, yr = x / 10, y / 10
 
     # Remove existing detector
     if hasattr(self, "virtual_detector_point"):
         self.diffraction_space_widget.view.scene().removeItem(
             self.virtual_detector_point
```

### Comparing `py4D_browser-0.999999/src/py4D_browser.egg-info/PKG-INFO` & `py4D_browser-1.0.0/src/py4D_browser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4D_browser
-Version: 0.999999
+Version: 1.0.0
 Summary: A 4D-STEM data browser built on py4DSTEM.
 Author-email: Steven Zeltmann <steven.zeltmann@lbl.gov>
 Project-URL: Homepage, https://github.com/py4dstem/py4D-browser
 Project-URL: Bug Tracker, https://github.com/py4dstem/py4D-browser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -18,41 +18,41 @@
 Requires-Dist: PyQt5>=5.10
 Requires-Dist: pyqtgraph>=0.11
 Requires-Dist: sigfig
 
 
 # The `py4DSTEM` GUI
 
-This repository hosts the `pyqt` based graphical 4D--STEM data browser that was originally part of **py4DSTEM** until version 0.13.11. 
+This repository hosts the `pyqt` based graphical 4D--STEM data browser that was originally part of **py4DSTEM** until version 0.13.11.
 
-## Installation 
-The GUI is available on PyPI and conda-forge: 
+## Installation
+The GUI is available on PyPI and conda-forge:
 
 `pip install py4D-browser`
 
 `conda install -c conda-forge py4d-browser`
 
 
 ## Usage
 Run `py4DGUI` in your terminal to open the GUI. Then just drag and drop a 4D-STEM dataset into the window!
 
 ### Controls
-* Move the virtual detector and the real-space selector using the mouse or using the keyboard shortcuts: WASD moves the detector and IJKL moves the selector, and holding down shift moves 5 pixels at a time. 
-* Auto scaling of both views is on by default. Press the "Autoscale" buttons in the bottom right to disable. Press either button to apply automatic scaling once, or Shift + click to lock autoscaling back on. 
+* Move the virtual detector and the real-space selector using the mouse or using the keyboard shortcuts: WASD moves the detector and IJKL moves the selector, and holding down shift moves 5 pixels at a time.
+* Auto scaling of both views is on by default. Press the "Autoscale" buttons in the bottom right to disable. Press either button to apply automatic scaling once, or Shift + click to lock autoscaling back on.
 * Different shapes of virtual detector are available in the "Detector Shape" menu, and different detector responses are available in the "Detector Response" menu.
-* The information in the bottom bar contains the details of the virtual detector used to generate the images, and can be entered into py4DSTEM to generate the same image. 
+* The information in the bottom bar contains the details of the virtual detector used to generate the images, and can be entered into py4DSTEM to generate the same image.
 * The FFT pane can be switched between displaying the FFT of the virtual image and displaying the [exit wave power cepstrum](https://doi.org/10.1016/j.ultramic.2020.112994).
 * Virtual images can be exported either as the scaled and clipped displays shown in the GUI or as raw data. The exact datatype stored in the raw TIFF image depends on both the datatype of the dataset and the type of virtual image being displayed (in particular, integer datatypes are converted internally to floating point to prevent overflows when generating any synthesized virtual images).
-* If the [EMPAD-G2 Raw Reader](https://github.com/sezelt/empad2) is installed in the same environment, an extra menu will appear that allows the concatenated binary format data to be background subtracted and calibrated in the GUI. You can also save the calibrated data as an HDF5 file for later analysis. 
+* If the [EMPAD-G2 Raw Reader](https://github.com/sezelt/empad2) is installed in the same environment, an extra menu will appear that allows the concatenated binary format data to be background subtracted and calibrated in the GUI. You can also save the calibrated data as an HDF5 file for later analysis.
 
 ![Demonstration](/images/demo.gif)
 
 The keyboard map in the Help menu was made using [this tool](https://archie-adams.github.io/keyboard-shortcut-map-maker/) and the map file is in the top level of this repo.
 
-## About 
+## About
 
 ![py4DSTEM logo](/images/py4DSTEM_logo.png)
 
 **py4DSTEM** is an open source set of python tools for processing and analysis of four-dimensional scanning transmission electron microscopy (4D-STEM) data. Additional information:
 
 - [Our open access py4DSTEM publication in Microscopy and Microanalysis](https://doi.org/10.1017/S1431927621000477) describing this project and demonstrating a variety of applications.
 - [The py4DSTEM documentation pages](https://py4dstem.readthedocs.io/en/latest/index.html).
```

### Comparing `py4D_browser-0.999999/src/py4D_browser.egg-info/SOURCES.txt` & `py4D_browser-1.0.0/src/py4D_browser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

