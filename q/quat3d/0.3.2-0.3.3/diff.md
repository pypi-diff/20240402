# Comparing `tmp/quat3d-0.3.2.tar.gz` & `tmp/quat3d-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quat3d-0.3.2.tar", last modified: Tue Apr  2 12:38:08 2024, max compression
+gzip compressed data, was "quat3d-0.3.3.tar", last modified: Tue Apr  2 12:45:14 2024, max compression
```

## Comparing `quat3d-0.3.2.tar` & `quat3d-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:38:08.877694 quat3d-0.3.2/
--rw-rw-rw-   0        0        0       40 2024-04-02 08:28:06.000000 quat3d-0.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1709 2024-04-02 12:38:08.876694 quat3d-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-02 09:09:14.000000 quat3d-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 12:38:08.856694 quat3d-0.3.2/quat3d/
--rw-rw-rw-   0        0        0       21 2024-04-02 12:37:30.000000 quat3d-0.3.2/quat3d/__init__.py
--rw-rw-rw-   0        0        0     2312 2024-04-02 09:20:40.000000 quat3d-0.3.2/quat3d/quat3d.py
--rw-rw-rw-   0        0        0     7475 2024-04-02 09:23:49.000000 quat3d-0.3.2/quat3d/quaternion3d.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:38:08.876694 quat3d-0.3.2/quat3d.egg-info/
--rw-rw-rw-   0        0        0     1709 2024-04-02 12:38:08.000000 quat3d-0.3.2/quat3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2024-04-02 12:38:08.000000 quat3d-0.3.2/quat3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:38:08.000000 quat3d-0.3.2/quat3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-02 12:38:08.000000 quat3d-0.3.2/quat3d.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-04-02 12:38:08.000000 quat3d-0.3.2/quat3d.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       84 2024-04-02 12:38:08.000000 quat3d-0.3.2/quat3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 12:38:08.000000 quat3d-0.3.2/quat3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 12:38:08.877694 quat3d-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1061 2024-04-02 12:37:24.000000 quat3d-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:45:14.424215 quat3d-0.3.3/
+-rw-rw-rw-   0        0        0       40 2024-04-02 08:28:06.000000 quat3d-0.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1705 2024-04-02 12:45:14.423215 quat3d-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1027 2024-04-02 12:44:14.000000 quat3d-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 12:45:14.395730 quat3d-0.3.3/quat3d/
+-rw-rw-rw-   0        0        0       21 2024-04-02 12:44:32.000000 quat3d-0.3.3/quat3d/__init__.py
+-rw-rw-rw-   0        0        0     2312 2024-04-02 09:20:40.000000 quat3d-0.3.3/quat3d/quat3d.py
+-rw-rw-rw-   0        0        0     7473 2024-04-02 12:43:35.000000 quat3d-0.3.3/quat3d/quaternion3d.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:45:14.422215 quat3d-0.3.3/quat3d.egg-info/
+-rw-rw-rw-   0        0        0     1705 2024-04-02 12:45:14.000000 quat3d-0.3.3/quat3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2024-04-02 12:45:14.000000 quat3d-0.3.3/quat3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:45:14.000000 quat3d-0.3.3/quat3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-02 12:45:14.000000 quat3d-0.3.3/quat3d.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-02 12:38:08.000000 quat3d-0.3.3/quat3d.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       82 2024-04-02 12:45:14.000000 quat3d-0.3.3/quat3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 12:45:14.000000 quat3d-0.3.3/quat3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:45:14.424215 quat3d-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2024-04-02 12:44:21.000000 quat3d-0.3.3/setup.py
```

### Comparing `quat3d-0.3.2/PKG-INFO` & `quat3d-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: quat3d
-Version: 0.3.2
+Version: 0.3.3
 Summary: This is an IMU quaternion data visualization tool for xkit.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: xkit,genlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: python-dotenv
-Requires-Dist: pyside6
+Requires-Dist: pyqt6
 Requires-Dist: pyqtgraph
 Requires-Dist: pyopengl
 Requires-Dist: pyopengl_accelerate
 Requires-Dist: numpy-stl
 Requires-Dist: genlib
 
 This is an IMU quaternion data visualization tool for xkit.
@@ -30,15 +30,15 @@
 
 ### Install
 ```sh
 pip install quat
 ```
 
 ### Dependencies
-- PySide6
+- PyQt6
 - PyOpenGL
 - pyqtgraph
 - numpy-stl
 - genlib
 
 
 ### Running
```

### Comparing `quat3d-0.3.2/README.md` & `quat3d-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ### Install
 ```sh
 pip install quat
 ```
 
 ### Dependencies
-- PySide6
+- PyQt6
 - PyOpenGL
 - pyqtgraph
 - numpy-stl
 - genlib
 
 
 ### Running
```

### Comparing `quat3d-0.3.2/quat3d/quat3d.py` & `quat3d-0.3.3/quat3d/quat3d.py`

 * *Files identical despite different names*

### Comparing `quat3d-0.3.2/quat3d/quaternion3d.py` & `quat3d-0.3.3/quat3d/quaternion3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Uart.write(data, slip=True)
     
     # This is an optimized value for 
     # visualizations up to 65 frames.
     time.sleep_ms(20)
 """
 
-ABOUT = "Version: 1.0.0\n\nPySide6: 6.6.2\nPyOpenGL: 3.1.7\npyqtgraph: 0.13.4\n\n@PlanX Labs. 2024"
+ABOUT = "Version: 1.0.0\n\nPyQt6: 6.6.2\nPyOpenGL: 3.1.7\npyqtgraph: 0.13.4\n\n@PlanX Labs. 2024"
 
 
 class ReadThread(QThread):
     readSignal = pyqtSignal(object)
     
     def __init__(self, mainWindow, group, iport, mcast, log_name):
         super().__init__()
```

### Comparing `quat3d-0.3.2/quat3d.egg-info/PKG-INFO` & `quat3d-0.3.3/quat3d.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: quat3d
-Version: 0.3.2
+Version: 0.3.3
 Summary: This is an IMU quaternion data visualization tool for xkit.
 Home-page: https://github.com/planxstudio/xkit
 Author: chanmin.park
 Author-email: devcamp@gmail.com
 Keywords: xkit,genlib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: python-dotenv
-Requires-Dist: pyside6
+Requires-Dist: pyqt6
 Requires-Dist: pyqtgraph
 Requires-Dist: pyopengl
 Requires-Dist: pyopengl_accelerate
 Requires-Dist: numpy-stl
 Requires-Dist: genlib
 
 This is an IMU quaternion data visualization tool for xkit.
@@ -30,15 +30,15 @@
 
 ### Install
 ```sh
 pip install quat
 ```
 
 ### Dependencies
-- PySide6
+- PyQt6
 - PyOpenGL
 - pyqtgraph
 - numpy-stl
 - genlib
 
 
 ### Running
```

### Comparing `quat3d-0.3.2/setup.py` & `quat3d-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     
 setup(
     name='quat3d',
-    version='0.3.2',
+    version='0.3.3',
     description='This is an IMU quaternion data visualization tool for xkit.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='chanmin.park',
     author_email='devcamp@gmail.com',
     url='https://github.com/planxstudio/xkit',
-    install_requires=['click', 'python-dotenv', 'pyside6', 'pyqtgraph', 'pyopengl', 'pyopengl_accelerate', 'numpy-stl', 'genlib'],
+    install_requires=['click', 'python-dotenv', 'pyqt6', 'pyqtgraph', 'pyopengl', 'pyopengl_accelerate', 'numpy-stl', 'genlib'],
     packages=find_packages(exclude=[]),
     keywords=['xkit', 'genlib'],
     python_requires='>=3.11',
     package_data={},
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
```

