# Comparing `tmp/DeCGR-1.0.3.tar.gz` & `tmp/DeCGR-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeCGR-1.0.3.tar", last modified: Tue Apr  2 07:28:20 2024, max compression
+gzip compressed data, was "DeCGR-1.0.4.tar", last modified: Tue Apr  2 14:08:36 2024, max compression
```

## Comparing `DeCGR-1.0.3.tar` & `DeCGR-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 07:28:20.149344 DeCGR-1.0.3/
-drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 07:28:20.145341 DeCGR-1.0.3/DeCGR.egg-info/
--rw-r--r--   0 desert     (501) staff       (20)      320 2024-04-02 07:28:20.000000 DeCGR-1.0.3/DeCGR.egg-info/PKG-INFO
--rw-r--r--   0 desert     (501) staff       (20)      427 2024-04-02 07:28:20.000000 DeCGR-1.0.3/DeCGR.egg-info/SOURCES.txt
--rw-r--r--   0 desert     (501) staff       (20)        1 2024-04-02 07:28:20.000000 DeCGR-1.0.3/DeCGR.egg-info/dependency_links.txt
--rw-r--r--   0 desert     (501) staff       (20)      169 2024-04-02 07:28:20.000000 DeCGR-1.0.3/DeCGR.egg-info/requires.txt
--rw-r--r--   0 desert     (501) staff       (20)        6 2024-04-02 07:28:20.000000 DeCGR-1.0.3/DeCGR.egg-info/top_level.txt
--rw-r--r--   0 desert     (501) staff       (20)     1107 2024-04-01 08:41:08.000000 DeCGR-1.0.3/LICENSE
--rw-r--r--   0 desert     (501) staff       (20)      320 2024-04-02 07:28:20.149200 DeCGR-1.0.3/PKG-INFO
-drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 07:28:20.147177 DeCGR-1.0.3/decgr/
--rwx------   0 desert     (501) staff       (20)    27458 2024-03-20 12:35:41.000000 DeCGR-1.0.3/decgr/DetermineFragment.py
--rwx------   0 desert     (501) staff       (20)      143 2024-04-01 02:10:06.000000 DeCGR-1.0.3/decgr/__init__.py
-drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 07:28:20.148505 DeCGR-1.0.3/decgr/cnv/
--rwx------   0 desert     (501) staff       (20)      135 2024-02-04 04:50:54.000000 DeCGR-1.0.3/decgr/cnv/__init__.py
--rwx------   0 desert     (501) staff       (20)     6600 2024-03-29 07:05:53.000000 DeCGR-1.0.3/decgr/cnv/correctcnv.py
--rwx------   0 desert     (501) staff       (20)     4092 2024-02-04 04:50:54.000000 DeCGR-1.0.3/decgr/cnv/loadcnv.py
--rwx------   0 desert     (501) staff       (20)     2155 2024-02-04 04:50:54.000000 DeCGR-1.0.3/decgr/cnv/runcnv.py
--rwx------   0 desert     (501) staff       (20)    12058 2024-04-01 02:45:20.000000 DeCGR-1.0.3/decgr/cnv/segcnv.py
--rwx------   0 desert     (501) staff       (20)    16319 2024-02-04 04:50:54.000000 DeCGR-1.0.3/decgr/cnv/util.py
--rwx------   0 desert     (501) staff       (20)     6287 2024-04-01 02:45:00.000000 DeCGR-1.0.3/decgr/correct.py
--rwx------   0 desert     (501) staff       (20)    10602 2024-04-01 02:44:19.000000 DeCGR-1.0.3/decgr/plot_reconstruct_map.py
--rwx------   0 desert     (501) staff       (20)    15674 2024-03-20 09:30:46.000000 DeCGR-1.0.3/decgr/simuProcess.py
--rwx------   0 desert     (501) staff       (20)     3334 2024-04-01 07:24:41.000000 DeCGR-1.0.3/decgr/utils.py
-drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 07:28:20.148739 DeCGR-1.0.3/scripts/
--rwx------   0 desert     (501) staff       (20)    41048 2024-04-02 07:28:19.000000 DeCGR-1.0.3/scripts/DeCGR
--rw-r--r--   0 desert     (501) staff       (20)       38 2024-04-02 07:28:20.149376 DeCGR-1.0.3/setup.cfg
--rw-r--r--   0 desert     (501) staff       (20)     1296 2024-04-02 07:10:11.000000 DeCGR-1.0.3/setup.py
+drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 14:08:36.288782 DeCGR-1.0.4/
+drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 14:08:36.288465 DeCGR-1.0.4/DeCGR.egg-info/
+-rw-r--r--   0 desert     (501) staff       (20)      639 2024-04-02 14:08:36.000000 DeCGR-1.0.4/DeCGR.egg-info/PKG-INFO
+-rw-r--r--   0 desert     (501) staff       (20)      427 2024-04-02 14:08:36.000000 DeCGR-1.0.4/DeCGR.egg-info/SOURCES.txt
+-rw-r--r--   0 desert     (501) staff       (20)        1 2024-04-02 14:08:36.000000 DeCGR-1.0.4/DeCGR.egg-info/dependency_links.txt
+-rw-r--r--   0 desert     (501) staff       (20)      169 2024-04-02 14:08:36.000000 DeCGR-1.0.4/DeCGR.egg-info/requires.txt
+-rw-r--r--   0 desert     (501) staff       (20)        6 2024-04-02 14:08:36.000000 DeCGR-1.0.4/DeCGR.egg-info/top_level.txt
+-rw-r--r--   0 desert     (501) staff       (20)     1107 2024-04-01 08:41:08.000000 DeCGR-1.0.4/LICENSE
+-rw-r--r--   0 desert     (501) staff       (20)      639 2024-04-02 14:08:36.288633 DeCGR-1.0.4/PKG-INFO
+drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 14:08:36.286014 DeCGR-1.0.4/decgr/
+-rwx------   0 desert     (501) staff       (20)    27458 2024-03-20 12:35:41.000000 DeCGR-1.0.4/decgr/DetermineFragment.py
+-rwx------   0 desert     (501) staff       (20)      143 2024-04-01 02:10:06.000000 DeCGR-1.0.4/decgr/__init__.py
+drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 14:08:36.287508 DeCGR-1.0.4/decgr/cnv/
+-rwx------   0 desert     (501) staff       (20)      135 2024-02-04 04:50:54.000000 DeCGR-1.0.4/decgr/cnv/__init__.py
+-rwx------   0 desert     (501) staff       (20)     6600 2024-03-29 07:05:53.000000 DeCGR-1.0.4/decgr/cnv/correctcnv.py
+-rwx------   0 desert     (501) staff       (20)     4092 2024-02-04 04:50:54.000000 DeCGR-1.0.4/decgr/cnv/loadcnv.py
+-rwx------   0 desert     (501) staff       (20)     2155 2024-02-04 04:50:54.000000 DeCGR-1.0.4/decgr/cnv/runcnv.py
+-rwx------   0 desert     (501) staff       (20)    12058 2024-04-01 02:45:20.000000 DeCGR-1.0.4/decgr/cnv/segcnv.py
+-rwx------   0 desert     (501) staff       (20)    16319 2024-02-04 04:50:54.000000 DeCGR-1.0.4/decgr/cnv/util.py
+-rwx------   0 desert     (501) staff       (20)     6287 2024-04-01 02:45:00.000000 DeCGR-1.0.4/decgr/correct.py
+-rwx------   0 desert     (501) staff       (20)    10602 2024-04-01 02:44:19.000000 DeCGR-1.0.4/decgr/plot_reconstruct_map.py
+-rwx------   0 desert     (501) staff       (20)    15674 2024-03-20 09:30:46.000000 DeCGR-1.0.4/decgr/simuProcess.py
+-rwx------   0 desert     (501) staff       (20)     3367 2024-04-02 14:05:52.000000 DeCGR-1.0.4/decgr/utils.py
+drwxr-xr-x   0 desert     (501) staff       (20)        0 2024-04-02 14:08:36.287819 DeCGR-1.0.4/scripts/
+-rwx------   0 desert     (501) staff       (20)    41236 2024-04-02 14:08:36.000000 DeCGR-1.0.4/scripts/DeCGR
+-rw-r--r--   0 desert     (501) staff       (20)       38 2024-04-02 14:08:36.288820 DeCGR-1.0.4/setup.cfg
+-rw-r--r--   0 desert     (501) staff       (20)     1297 2024-04-02 13:43:15.000000 DeCGR-1.0.4/setup.py
```

### Comparing `DeCGR-1.0.3/LICENSE` & `DeCGR-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/DetermineFragment.py` & `DeCGR-1.0.4/decgr/DetermineFragment.py`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/cnv/correctcnv.py` & `DeCGR-1.0.4/decgr/cnv/correctcnv.py`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/cnv/loadcnv.py` & `DeCGR-1.0.4/decgr/cnv/loadcnv.py`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/cnv/runcnv.py` & `DeCGR-1.0.4/decgr/cnv/runcnv.py`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/cnv/segcnv.py` & `DeCGR-1.0.4/decgr/cnv/segcnv.py`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/cnv/util.py` & `DeCGR-1.0.4/decgr/cnv/util.py`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/correct.py` & `DeCGR-1.0.4/decgr/correct.py`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/plot_reconstruct_map.py` & `DeCGR-1.0.4/decgr/plot_reconstruct_map.py`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/simuProcess.py` & `DeCGR-1.0.4/decgr/simuProcess.py`

 * *Files identical despite different names*

### Comparing `DeCGR-1.0.3/decgr/utils.py` & `DeCGR-1.0.4/decgr/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     sort_start = dict(sorted(start.items(), key=operator.itemgetter(0)))
     sort_end = dict(sorted(end.items(), key=operator.itemgetter(0)))
     return list(path.values()), list(orient.values()), list(sort_chrom.values()), list(sort_start.values()), list(
         sort_end.values())
 
 
 def runFitHiC(path, control_dict, chrom_list, chro_lens, resolution):
+    path = os.path.dirname(path)
     with open(path + '/tmp/fithic.bed', 'w+') as f:
         chr_first = {}
         index = 1
         for idx, chro_len in enumerate(chro_lens):
             chr = chrom_list[idx]
             chr_first[chr] = index
             start = 0
```

### Comparing `DeCGR-1.0.3/scripts/DeCGR` & `DeCGR-1.0.4/scripts/DeCGR`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/env python
-from PyQt5.QtWidgets import QMainWindow, QLabel, QToolBar, QAction, QWidget, QVBoxLayout, QStackedWidget, QPushButton, QToolButton, QSplitter, QHBoxLayout, QTextEdit, QFrame, QApplication, QSizePolicy
+
+from PyQt5.QtWidgets import (
+    QMainWindow, QLabel, QToolBar, QAction, QWidget, QVBoxLayout, QStackedWidget, QPushButton, QToolButton, QSplitter,
+    QHBoxLayout, QTextEdit, QFrame, QApplication, QSizePolicy
+)
 from PyQt5.QtGui import QPixmap, QTextOption, QFont, QPainter, QColor, QDesktopServices
 from PyQt5.QtCore import QUrl, Qt
 import sys
 from PyQt5 import QtCore, QtGui, QtWidgets
 from iced import normalization
 from decgr.DetermineFragment import FragmentAssembly
 from decgr.simuProcess import simulation, get_cut_pos, plot_simu_matrix
@@ -24,14 +28,15 @@
     def __init__(self, parent=None):
         super(Interface, self).__init__(parent)
         self.setupUi(self)
         self.stackedWidget = QStackedWidget()
         self.setCentralWidget(self.stackedWidget)
 
         self.path = os.path.split(os.path.abspath(__file__))[0]
+        self.path = os.path.dirname(self.path)
         if not os.path.exists(self.path + '/result'):
             os.mkdir(self.path + '/result')
         if not os.path.exists(self.path + '/tmp'):
             os.mkdir(self.path + '/tmp')
 
         self.setWindowTitle('')
         self.setWindowFlags(self.windowFlags() & ~QtCore.Qt.WindowMaximizeButtonHint)
@@ -441,15 +446,17 @@
         text_edit.setMaximumHeight(350)
         text_edit.setAlignment(QtCore.Qt.AlignJustify)
         text_edit.setWordWrapMode(QTextOption.WrapAtWordBoundaryOrAnywhere)
         left_layout.addLayout(buttons_layout)
         left_layout.addWidget(text_edit)
         right_layout = QVBoxLayout()
         image_label = QLabel()
-        pixmap = QPixmap("mainplot.jpg")
+        path = os.path.split(os.path.abspath(__file__))[0]
+        path = os.path.dirname(path)
+        pixmap = QPixmap(path+"/figure/mainplot.jpg")
         image_label.setPixmap(pixmap)
         image_label.setAlignment(QtCore.Qt.AlignCenter)
         right_layout.addWidget(image_label)
         main_layout = QHBoxLayout(self.inputPage)
         main_layout.addLayout(left_layout)
         main_layout.addLayout(right_layout)
         self.inputPage.setLayout(main_layout)
@@ -787,15 +794,15 @@
         self.page3SubmitButton.setText(_translate("Form", "Submit-->"))
         self.exportResult.setText(_translate("Form", "Export result"))
 
     def open_user_manual(self):
         QDesktopServices.openUrl(QUrl("https://github.com/GaoLabXDU/DeCGR"))
 
     def download_test_data(self):
-        QDesktopServices.openUrl(QUrl("https://github.com/GaoLabXDU/DeCGR"))
+        QDesktopServices.openUrl(QUrl("https://github.com/GaoLabXDU/DeCGR/tree/main/TestData"))
 
 
 if __name__ == "__main__":
     app = QApplication(sys.argv)
     w = Interface()
     w.show()
     sys.exit(app.exec_())
```

### Comparing `DeCGR-1.0.3/setup.py` & `DeCGR-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 """
-Setup script for HiSV.
+Setup script for DeCGR.
 
 """
 import os, sys, glob
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
@@ -16,15 +16,15 @@
 # Guarantee Unix Format
 for src in glob.glob('scripts/*'):
     text = open(src, 'r').read().replace('\r\n', '\n')
     open(src, 'w').write(text)
 
 setuptools.setup(
     name = 'DeCGR',
-    version = "1.0.3",
+    version = "1.0.4",
     author = "Li Junping",
     author_email = 'lijunping02@qq.com',
     url = 'https://github.com/GaoLabXDU/DeCGR',
     description = 'An interactive toolkit for deciphering CGRs from Hi-C data',
     keywords = ("Hi-C", "complex rearrangements", "3D genome"),
     scripts = glob.glob('scripts/*'),
     packages = setuptools.find_packages(),
```

