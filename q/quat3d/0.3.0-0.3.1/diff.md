# Comparing `tmp/quat3d-0.3.0.tar.gz` & `tmp/quat3d-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quat3d-0.3.0.tar", last modified: Tue Apr  2 09:15:01 2024, max compression
+gzip compressed data, was "quat3d-0.3.1.tar", last modified: Tue Apr  2 09:23:55 2024, max compression
```

## Comparing `quat3d-0.3.0.tar` & `quat3d-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 09:15:00.998511 quat3d-0.3.0/
--rw-rw-rw-   0        0        0       40 2024-04-02 08:28:06.000000 quat3d-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1709 2024-04-02 09:15:00.996508 quat3d-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-02 09:09:14.000000 quat3d-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 09:15:00.963478 quat3d-0.3.0/quat3d/
--rw-rw-rw-   0        0        0       21 2024-04-02 09:10:43.000000 quat3d-0.3.0/quat3d/__init__.py
--rw-rw-rw-   0        0        0     2310 2024-04-02 09:05:16.000000 quat3d-0.3.0/quat3d/quat.py
--rw-rw-rw-   0        0        0     7471 2024-04-02 08:15:36.000000 quat3d-0.3.0/quat3d/quaternion3d.py
-drwxrwxrwx   0        0        0        0 2024-04-02 09:15:00.994511 quat3d-0.3.0/quat3d.egg-info/
--rw-rw-rw-   0        0        0     1709 2024-04-02 09:15:00.000000 quat3d-0.3.0/quat3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2024-04-02 09:15:00.000000 quat3d-0.3.0/quat3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 09:15:00.000000 quat3d-0.3.0/quat3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-02 09:15:00.000000 quat3d-0.3.0/quat3d.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-02 09:15:00.000000 quat3d-0.3.0/quat3d.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       84 2024-04-02 09:15:00.000000 quat3d-0.3.0/quat3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 09:15:00.000000 quat3d-0.3.0/quat3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 09:15:00.998511 quat3d-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1050 2024-04-02 09:14:33.000000 quat3d-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:23:55.777253 quat3d-0.3.1/
+-rw-rw-rw-   0        0        0       40 2024-04-02 08:28:06.000000 quat3d-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1709 2024-04-02 09:23:55.776253 quat3d-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-02 09:09:14.000000 quat3d-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 09:23:55.741219 quat3d-0.3.1/quat3d/
+-rw-rw-rw-   0        0        0       21 2024-04-02 09:19:41.000000 quat3d-0.3.1/quat3d/__init__.py
+-rw-rw-rw-   0        0        0     2312 2024-04-02 09:20:40.000000 quat3d-0.3.1/quat3d/quat3d.py
+-rw-rw-rw-   0        0        0     7475 2024-04-02 09:23:49.000000 quat3d-0.3.1/quat3d/quaternion3d.py
+drwxrwxrwx   0        0        0        0 2024-04-02 09:23:55.774252 quat3d-0.3.1/quat3d.egg-info/
+-rw-rw-rw-   0        0        0     1709 2024-04-02 09:23:55.000000 quat3d-0.3.1/quat3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-04-02 09:23:55.000000 quat3d-0.3.1/quat3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 09:23:55.000000 quat3d-0.3.1/quat3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-02 09:23:55.000000 quat3d-0.3.1/quat3d.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-02 09:23:55.000000 quat3d-0.3.1/quat3d.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       84 2024-04-02 09:23:55.000000 quat3d-0.3.1/quat3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 09:23:55.000000 quat3d-0.3.1/quat3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 09:23:55.777253 quat3d-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1054 2024-04-02 09:21:51.000000 quat3d-0.3.1/setup.py
```

### Comparing `quat3d-0.3.0/PKG-INFO` & `quat3d-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quat3d
-Version: 0.3.0
+Version: 0.3.1
 Summary: This is an IMU quaternion data visualization tool for xkit.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: xkit,genlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quat3d-0.3.0/README.md` & `quat3d-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `quat3d-0.3.0/quat3d/quat.py` & `quat3d-0.3.1/quat3d/quat3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 
 import click
 import dotenv
 import genlib.ansiec as ansiec
 from PyQt6.QtWidgets import QApplication
 
-from quat.quaternion3d import Quaternion3D
+from quat3d.quaternion3d import Quaternion3D
 
 config = dotenv.find_dotenv(filename=".xnode", usecwd=True)
 if config:
     dotenv.load_dotenv(dotenv_path=config)
 
 @click.command()
 @click.option(
```

### Comparing `quat3d-0.3.0/quat3d/quaternion3d.py` & `quat3d-0.3.1/quat3d/quaternion3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         dlg.rejected.connect(lambda: self.gl_view.setBackgroundColor(self.bg_color))
 
         if dlg.exec():
             self.bg_color = dlg.currentColor()
 
     def onXnodeCode(self):
         msgbox = QMessageBox(self)        
-        msgbox.setIconPixmap(QPixmap(os.path.join(os.path.dirname(__file__), "quat_xnode_code.png")))
+        msgbox.setIconPixmap(QPixmap(os.path.join(os.path.dirname(__file__), "quat3d_xnode_code.png")))
         msgbox.setWindowTitle("The code below needs to be run on XNode.")
         copy_bt = msgbox.addButton("Copy", QMessageBox.ButtonRole.YesRole)
         copy_bt.clicked.connect(lambda : self.clipboard.setText(XNODE_CODE))
         msgbox.addButton("Ok", QMessageBox.ButtonRole.YesRole)        
         msgbox.exec()
 
     def onDraw(self, quat):    
@@ -144,15 +144,15 @@
 
         self.mesh_item.resetTransform()
         self.mesh_item.rotate(angle, axis.x(), axis.y(), axis.z())
         
     def initGUI(self):
         self.setWindowTitle("Quaternion 3D Viewer")
         self.resize(800, 600)
-        self.setWindowIcon(QIcon(os.path.join(os.path.dirname(__file__), "quat.png")))
+        self.setWindowIcon(QIcon(os.path.join(os.path.dirname(__file__), "quat3d.png")))
         
         self.initMenu()
             
         self.old_quat = (0.0, 0,0, 0,0, 0,0)        
         self.bg_color = QColor(0, 33, 50, 255) #RGBA
         self.object = self.SPHERE
```

### Comparing `quat3d-0.3.0/quat3d.egg-info/PKG-INFO` & `quat3d-0.3.1/quat3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quat3d
-Version: 0.3.0
+Version: 0.3.1
 Summary: This is an IMU quaternion data visualization tool for xkit.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: xkit,genlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quat3d-0.3.0/setup.py` & `quat3d-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name='quat3d',
-    version='0.3.0',
+    version='0.3.1',
     description='This is an IMU quaternion data visualization tool for xkit.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='chanmin.park',
     author_email='devcamp@gmail.com',
     url='https://github.com/planxstudio/xkit',
     install_requires=['click', 'python-dotenv', 'pyside6', 'pyqtgraph', 'pyopengl', 'pyopengl_accelerate', 'numpy-stl', 'genlib'],
@@ -22,11 +22,11 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     entry_points={
         'console_scripts': [
-            'quat = quat:main',            
+            'quat3d = quat3d:main',            
         ],
     },
 )
```

