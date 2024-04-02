# Comparing `tmp/condynsate-0.5.7.tar.gz` & `tmp/condynsate-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condynsate-0.5.7.tar", last modified: Tue Mar  5 21:57:19 2024, max compression
+gzip compressed data, was "condynsate-0.6.0.tar", last modified: Tue Apr  2 20:16:51 2024, max compression
```

## Comparing `condynsate-0.5.7.tar` & `condynsate-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 21:57:19.821447 condynsate-0.5.7/
--rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.5.7/LICENSE
--rw-rw-rw-   0        0        0     4920 2024-03-05 21:57:19.821447 condynsate-0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     2436 2024-01-16 21:39:32.000000 condynsate-0.5.7/README.md
--rw-rw-rw-   0        0        0     1439 2024-03-05 21:56:32.000000 condynsate-0.5.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-05 21:57:19.821447 condynsate-0.5.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-05 21:57:19.779530 condynsate-0.5.7/src/
-drwxrwxrwx   0        0        0        0 2024-03-05 21:57:19.805818 condynsate-0.5.7/src/condynsate/
-drwxrwxrwx   0        0        0        0 2024-03-05 21:57:19.821447 condynsate-0.5.7/src/condynsate/__assets__/
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/arrow_ccw.stl
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/arrow_cw.stl
--rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/arrow_lin.stl
--rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/check.png
--rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/cube.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.5.7/src/condynsate/__assets__/cylinder.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.5.7/src/condynsate/__assets__/cylinder_lower_origin.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.5.7/src/condynsate/__assets__/gate_med.stl
--rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.5.7/src/condynsate/__assets__/gate_short.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.5.7/src/condynsate/__assets__/gate_tall.stl
--rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/plane_big.obj
--rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/plane_med.obj
--rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/plane_small.obj
--rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/pyramid.stl
--rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/__assets__/sphere.stl
--rw-rw-rw-   0        0        0      153 2024-03-05 21:56:41.000000 condynsate-0.5.7/src/condynsate/__init__.py
--rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.5.7/src/condynsate/animator.py
--rw-rw-rw-   0        0        0     8209 2024-02-06 15:55:34.000000 condynsate-0.5.7/src/condynsate/keyboard.py
--rw-rw-rw-   0        0        0   140818 2024-03-04 19:25:57.000000 condynsate-0.5.7/src/condynsate/simulator.py
--rw-rw-rw-   0        0        0     7902 2024-02-27 00:32:15.000000 condynsate-0.5.7/src/condynsate/utils.py
--rw-rw-rw-   0        0        0    22062 2023-11-24 19:50:22.000000 condynsate-0.5.7/src/condynsate/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-03-05 21:57:19.821447 condynsate-0.5.7/src/condynsate.egg-info/
--rw-rw-rw-   0        0        0     4920 2024-03-05 21:57:19.000000 condynsate-0.5.7/src/condynsate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2024-03-05 21:57:19.000000 condynsate-0.5.7/src/condynsate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 21:57:19.000000 condynsate-0.5.7/src/condynsate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-03-05 21:57:19.000000 condynsate-0.5.7/src/condynsate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-05 21:57:19.000000 condynsate-0.5.7/src/condynsate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.961443 condynsate-0.6.0/
+-rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     4875 2024-04-02 20:16:51.961443 condynsate-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.0/README.md
+-rw-rw-rw-   0        0        0     1439 2024-04-02 20:16:17.000000 condynsate-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 20:16:51.961443 condynsate-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.895143 condynsate-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.918182 condynsate-0.6.0/src/condynsate/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.961443 condynsate-0.6.0/src/condynsate/__assets__/
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/arrow_ccw.stl
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/arrow_cw.stl
+-rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/arrow_lin.stl
+-rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/check.png
+-rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/cube.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.0/src/condynsate/__assets__/cylinder.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.0/src/condynsate/__assets__/cylinder_lower_origin.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.0/src/condynsate/__assets__/gate_med.stl
+-rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.0/src/condynsate/__assets__/gate_short.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.0/src/condynsate/__assets__/gate_tall.stl
+-rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/plane_big.obj
+-rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/plane_med.obj
+-rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/plane_small.obj
+-rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/pyramid.stl
+-rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.0/src/condynsate/__assets__/sphere.stl
+-rw-rw-rw-   0        0        0      153 2024-04-02 20:16:17.000000 condynsate-0.6.0/src/condynsate/__init__.py
+-rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.0/src/condynsate/animator.py
+-rw-rw-rw-   0        0        0     8209 2024-02-06 15:55:34.000000 condynsate-0.6.0/src/condynsate/keyboard.py
+-rw-rw-rw-   0        0        0   144586 2024-04-02 19:53:04.000000 condynsate-0.6.0/src/condynsate/simulator.py
+-rw-rw-rw-   0        0        0    10335 2024-03-26 22:00:32.000000 condynsate-0.6.0/src/condynsate/utils.py
+-rw-rw-rw-   0        0        0    22362 2024-04-02 19:38:52.000000 condynsate-0.6.0/src/condynsate/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:16:51.961443 condynsate-0.6.0/src/condynsate.egg-info/
+-rw-rw-rw-   0        0        0     4875 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 20:16:51.000000 condynsate-0.6.0/src/condynsate.egg-info/top_level.txt
```

### Comparing `condynsate-0.5.7/LICENSE` & `condynsate-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/PKG-INFO` & `condynsate-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.5.7
+Version: 0.6.0
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,16 +51,14 @@
 Requires-Dist: pyside6
 Requires-Dist: sympy
 
 # condynsate
 
  [condynsate](https://github.com/GrayKS3248/condynsate) is a dynamic system simulation and visualization tool built with [PyBullet](https://pybullet.org/wordpress/) and [MeshCat](https://github.com/meshcat-dev/meshcat-python). It automatically simulates multiple objects and their interactions as described by [.urdf](http://wiki.ros.org/urdf), [.stl](https://en.wikipedia.org/wiki/STL_(file_format)), and [.obj](https://en.wikipedia.org/wiki/Wavefront_.obj_file) files and can render real time visualizations in a web browser.
 
-
-
 # Installation
 
 ## From Source
 
 condynsate requires python => 3.8
 
 ```bash
@@ -74,16 +72,14 @@
   * [Install Miniconda.](https://docs.conda.io/projects/miniconda/en/latest/)
   
   * To verify that Miniconda is installed properly, open **Anaconda Prompt (Miniconda3)** and run the command:
     
     ```bash
     conda --version
     ```
-    
-    
 
 * **Create a new virtual environment**
   
   * To create a new environment, open **Anaconda Prompt (Miniconda3)** and run the command:
     
     ```bash
     conda create -n ENVNAME
@@ -92,16 +88,14 @@
   * Next, activate the newly made environment: 
     
     ```bash
     conda activate ENVNAME
     ```
   
   * You can confirm the virtual environment is activated when environment name on the left side of the command line changes from ``(base)`` to``(ENVNAME)``
-    
-    
 
 * **Install dependencies from Conda-Forge:**
   
   * Configure the environment channels by running the commands:
     
     ```bash
     conda config --env --add channels conda-forge
@@ -110,16 +104,14 @@
     ```
   
   * Install dependencies available from Conda-Forge by running the command:
     
     ```bash
     conda install -y python=3 numpy pynput matplotlib pybullet control sympy notebook
     ```
-    
-    
 
 * **Install condynsate using pip**
   
   * To install condynsate run the commands:
     
     ```bash
     pip cache purge
@@ -130,12 +122,10 @@
     
     ```python
     python
     import condynsate
     condynsate.__version__ 
     ```
 
- 
-
 # Usage
 
 For examples of usage, see [examples](https://github.com/GrayKS3248/condynsate/tree/main/examples).
```

### Comparing `condynsate-0.5.7/README.md` & `condynsate-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # condynsate
 
  [condynsate](https://github.com/GrayKS3248/condynsate) is a dynamic system simulation and visualization tool built with [PyBullet](https://pybullet.org/wordpress/) and [MeshCat](https://github.com/meshcat-dev/meshcat-python). It automatically simulates multiple objects and their interactions as described by [.urdf](http://wiki.ros.org/urdf), [.stl](https://en.wikipedia.org/wiki/STL_(file_format)), and [.obj](https://en.wikipedia.org/wiki/Wavefront_.obj_file) files and can render real time visualizations in a web browser.
 
-
-
 # Installation
 
 ## From Source
 
 condynsate requires python => 3.8
 
 ```bash
@@ -21,16 +19,14 @@
   * [Install Miniconda.](https://docs.conda.io/projects/miniconda/en/latest/)
   
   * To verify that Miniconda is installed properly, open **Anaconda Prompt (Miniconda3)** and run the command:
     
     ```bash
     conda --version
     ```
-    
-    
 
 * **Create a new virtual environment**
   
   * To create a new environment, open **Anaconda Prompt (Miniconda3)** and run the command:
     
     ```bash
     conda create -n ENVNAME
@@ -39,16 +35,14 @@
   * Next, activate the newly made environment: 
     
     ```bash
     conda activate ENVNAME
     ```
   
   * You can confirm the virtual environment is activated when environment name on the left side of the command line changes from ``(base)`` to``(ENVNAME)``
-    
-    
 
 * **Install dependencies from Conda-Forge:**
   
   * Configure the environment channels by running the commands:
     
     ```bash
     conda config --env --add channels conda-forge
@@ -57,16 +51,14 @@
     ```
   
   * Install dependencies available from Conda-Forge by running the command:
     
     ```bash
     conda install -y python=3 numpy pynput matplotlib pybullet control sympy notebook
     ```
-    
-    
 
 * **Install condynsate using pip**
   
   * To install condynsate run the commands:
     
     ```bash
     pip cache purge
@@ -77,12 +69,10 @@
     
     ```python
     python
     import condynsate
     condynsate.__version__ 
     ```
 
- 
-
 # Usage
 
 For examples of usage, see [examples](https://github.com/GrayKS3248/condynsate/tree/main/examples).
```

### Comparing `condynsate-0.5.7/pyproject.toml` & `condynsate-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "condynsate"
-version = "0.5.7"
+version = "0.6.0"
 description = "Simulates and visualizes articulated systems in real time"
 readme = "README.md"
 authors = [{ name = "Grayson Schaer", email = "gschaer2@illinois.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/arrow_ccw.stl` & `condynsate-0.6.0/src/condynsate/__assets__/arrow_ccw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/arrow_cw.stl` & `condynsate-0.6.0/src/condynsate/__assets__/arrow_cw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/arrow_lin.stl` & `condynsate-0.6.0/src/condynsate/__assets__/arrow_lin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/check.png` & `condynsate-0.6.0/src/condynsate/__assets__/check.png`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/cylinder.stl` & `condynsate-0.6.0/src/condynsate/__assets__/cylinder.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/cylinder_lower_origin.stl` & `condynsate-0.6.0/src/condynsate/__assets__/cylinder_lower_origin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/gate_med.stl` & `condynsate-0.6.0/src/condynsate/__assets__/gate_med.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/gate_short.stl` & `condynsate-0.6.0/src/condynsate/__assets__/gate_short.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/gate_tall.stl` & `condynsate-0.6.0/src/condynsate/__assets__/gate_tall.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/__assets__/sphere.stl` & `condynsate-0.6.0/src/condynsate/__assets__/sphere.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/animator.py` & `condynsate-0.6.0/src/condynsate/animator.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/keyboard.py` & `condynsate-0.6.0/src/condynsate/keyboard.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.5.7/src/condynsate/simulator.py` & `condynsate-0.6.0/src/condynsate/simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy as np
 import time
 import pybullet
 from pybullet_utils import bullet_client as bc
 from condynsate.visualizer import Visualizer
 from condynsate.animator import Animator
 from condynsate.utils import format_path,format_RGB,wxyz_to_xyzw,xyzw_to_wxyz
-from condynsate.utils import xyzw_quat_mult, get_rot_from_2_vecs
+from condynsate.utils import get_rot_from_2_vecs, vc_inA_toB, RAB_to_RBA
 from condynsate.keyboard import Keys
 from matplotlib import colormaps as cmaps
 from pathlib import Path
 
 
 ###############################################################################
 #URDF OBJECT CLASS
@@ -56,14 +56,16 @@
 
         """
         self.urdf_id = urdf_id
         self.joint_map = joint_map
         self.link_map = link_map     
         self.update_vis = update_vis
         self.initial_conds = {}
+        self.geometries = []
+        self.textures = []
 
 
 ###############################################################################
 #SIMULATOR CLASS
 ###############################################################################
 class Simulator:
     """
@@ -134,15 +136,16 @@
         self.ccw_arr_map = {}
         
         # Create a visualizer
         if visualization:
             self.vis = Visualizer(grid_vis=False,axes_vis=False)
         else:
             self.vis=None
-            
+        self.vis_time_okay = True
+        
         # Create an animator
         if animation:
             self.ani = Animator(fr=animation_fr)
         else:
             self.ani=None
             
         # Start the keyboard listener
@@ -497,14 +500,73 @@
         # Set the max joint velocity
         if joint_name in joint_map:
             joint_id = joint_map[joint_name]
             self.engine.changeDynamics(urdf_id,
                                        joint_id,
                                        maxJointVelocity=max_vel)
             
+            
+    ###########################################################################
+    #CHANGE OF COORDINATE TOOLS
+    ###########################################################################      
+    def _v_inB_to_vinW(self,
+                       urdf_obj,
+                       v_inB):
+        """
+        Converts a vector in body coords to a vector in world coords
+    
+        Parameters
+        ----------
+        urdf_obj : URDF_Obj
+            A URDF_Obj whose base orientation describes the body frame.
+        v_inB : array-like, shape(3,)
+            A three vector in body coords.
+    
+        Returns
+        -------
+        v_inW : array-like, shape(3,)
+            The same three vector in world coords.
+    
+        """
+        v_inB = np.array(v_inB)
+        world_state = self.get_base_state(urdf_obj=urdf_obj,
+                                          body_coords=False)
+        R_ofW_inB = world_state['R of world in body']
+        R_ofB_inW = RAB_to_RBA(R_ofW_inB)
+        v_inW = vc_inA_toB(R_ofB_inW, v_inB)
+        return v_inW
+        
+    
+    def _v_inW_to_vinB(self,
+                       urdf_obj,
+                       v_inW):
+        """
+        Converts a vector in world coords to a vector in body coords
+    
+        Parameters
+        ----------
+        urdf_obj : URDF_Obj
+            A URDF_Obj whose base orientation describes the body frame.
+        v_inW : array-like, shape(3,)
+            A three vector in world coords.
+    
+        Returns
+        -------
+        v_inB : array-like, shape(3,)
+            The same three vector in body coords.
+    
+        """
+        v_inW = np.array(v_inW)
+        world_state = self.get_base_state(urdf_obj=urdf_obj,
+                                          body_coords=False)
+        R_ofW_inB = world_state['R of world in body']
+        v_inB = vc_inA_toB(R_ofW_inB, v_inW)
+        return v_inB
+            
+            
     ###########################################################################
     #JOINT SETTERS
     ###########################################################################
     def set_joint_force_sensor(self,
                                urdf_obj,
                                joint_name,
                                enable_sensor):
@@ -969,130 +1031,38 @@
         else:
             return
         
         # Ensure that we don't try to change a base joint
         if joint_id < 0:
             return
         
-        # If the arrow isn't meant to be visualized, hide it
-        vis_exists = isinstance(self.vis, Visualizer)
-        arr_exists = joint_name in self.ccw_arr_map
-        if (not show_arrow) and vis_exists and arr_exists:
-            arrow_name = str(self.ccw_arr_map[joint_name])
-            path = Path(__file__).parents[0]
-            path = path.absolute().as_posix()
-            path = path + "/__assets__/arrow_ccw.stl"
-            self.vis.set_link_color(urdf_name = "Torque Arrows",
-                                    link_name = arrow_name,
-                                    stl_path=path, 
-                                    color = [0, 0, 0],
-                                    transparent = True,
-                                    e = 0.0)
-        
-        # Handle torque arrow visualization
-        if show_arrow and isinstance(self.vis, Visualizer):
-            # Get the orientation, in body coordinates, of the arrow based
-            # on direction of torque
-            axis = self.get_joint_axis(urdf_obj=urdf_obj,
-                                       joint_name=joint_name)
-            if torque>=0.:
-                arrow_xyzw_in_body = get_rot_from_2_vecs([0,0,1], axis)
-            else:
-                arrow_xyzw_in_body = get_rot_from_2_vecs([0,0,-1], axis)
-                
-            # Get the child link of the joint to which torque is applied
-            joint_index = list(urdf_obj.link_map.values()).index(joint_id)
-            link_name = list(urdf_obj.link_map.keys())[joint_index]
-                
-            # Get the link state
-            state = self.get_link_state(urdf_obj=urdf_obj,
-                                        link_name=link_name)
-            body_xyzw_in_world = state['orientation']
-            body_xyzw_in_world = np.array(body_xyzw_in_world)
-            
-            # Get the arrow offset
-            body_wxyz_axis = np.insert(np.array(axis), 0, 0.)
-            wxyz_R = xyzw_to_wxyz(body_xyzw_in_world)
-            wxyz_R_prime = np.array([wxyz_R[0],
-                                     -wxyz_R[1],
-                                     -wxyz_R[2],
-                                     -wxyz_R[3]])
-            r1 = xyzw_quat_mult(wxyz_R,body_wxyz_axis)
-            world_wxyz_axis = -xyzw_quat_mult(r1, wxyz_R_prime)
-            world_axis = np.array([world_wxyz_axis[1],
-                                   world_wxyz_axis[2],
-                                   world_wxyz_axis[3]])
-            pos = state['position']
-            pos = np.array(pos) + arrow_offset*np.array(world_axis)
-            pos = tuple(pos.tolist())
-            
-            # Combine the two rotations
-            xyzw_ori = xyzw_quat_mult(arrow_xyzw_in_body, body_xyzw_in_world)
-            wxyz_ori = xyzw_to_wxyz(xyzw_ori)
-                
-            # Get the scale of the arrow based on the magnitude of the torque
-            scale = arrow_scale*abs(torque)*np.array([1., 1., 0.1])
-            scale = scale.tolist()
-            
-            # If the arrow already exists, only update its position and ori
-            if link_name in self.ccw_arr_map:
-                arrow_name = str(self.ccw_arr_map[link_name])
-                path = Path(__file__).parents[0]
-                path = path.absolute().as_posix()
-                path = path + "/__assets__/arrow_ccw.stl"
-                self.vis.set_link_color(urdf_name = "Torque Arrows",
-                                        link_name = arrow_name,
-                                        stl_path=path, 
-                                        color = [0, 0, 0],
-                                        transparent = False,
-                                        opacity = 1.0)
-                self.vis.apply_transform(urdf_name="Torque Arrows",
-                                         link_name=arrow_name,
-                                         scale=scale,
-                                         translate=pos,
-                                         wxyz_quaternion=wxyz_ori)
-            
-            # If the arrow is not already created, add it to the visualizer
-            else:
-                # Add the arrow to the linear arrow map
-                self.ccw_arr_map[link_name] = len(self.ccw_arr_map)
-                arrow_name = str(self.ccw_arr_map[link_name])
-                
-                # Add an arrow to the visualizer
-                path = Path(__file__).parents[0]
-                path = path.absolute().as_posix()
-                path = path + "/__assets__/arrow_ccw.stl"
-                self.vis.add_stl(urdf_name="Torque Arrows",
-                                 link_name=arrow_name,
-                                 stl_path=path,
-                                 color = [0, 0, 0],
-                                 transparent=False,
-                                 opacity = 1.0,
-                                 scale=scale,
-                                 translate=pos,
-                                 wxyz_quaternion=wxyz_ori)
-        
-        # Set the link color based on applied torque if option is selected.
-        if color and isinstance(self.vis, Visualizer):
-            self.set_color_from_torque(urdf_obj=urdf_obj,
-                                       joint_name=joint_name,
-                                       torque=torque,
-                                       min_torque=min_torque,
-                                       max_torque=max_torque)
-        
+        # Get the axis information about this joint so we can draw the 
+        # torque arrows in the correct directions
+        ax_inW, pos_inW, link_name = self.get_joint_axis(urdf_obj=urdf_obj,
+                                                         joint_name=joint_name)
+        
+        # Adjust the position of the arrow to get the desired offset
+        arr_pos_inW = pos_inW + arrow_offset*ax_inW
+        arr_pos_inW = arr_pos_inW.tolist()
+        
+        # Draw the torque arrow
+        self._draw_torque_arrow(urdf_obj=urdf_obj,
+                                torque_name=link_name,
+                                t_inW=torque*ax_inW,
+                                arr_pos_inW=arr_pos_inW,
+                                arr_scale=arrow_scale,
+                                show_arrow=show_arrow,
+                                force_update=False)
         
         # Set the joint torque
-        if joint_name in joint_map:
-            joint_id = [joint_map[joint_name]]
-            mode = self.engine.TORQUE_CONTROL
-            torque = [torque]
-            self.engine.setJointMotorControlArray(urdf_id,
-                                                  joint_id,
-                                                  mode,
-                                                  forces=torque)
+        self.engine.setJointMotorControlArray(urdf_id,
+                                              [joint_id],
+                                              self.engine.TORQUE_CONTROL,
+                                              forces=[torque])
+        
             
     ###########################################################################
     #JOINT GETTERS
     ###########################################################################
     def get_joint_state(self,
                         urdf_obj,
                         joint_name):
@@ -1161,41 +1131,73 @@
         return state
     
     
     def get_joint_axis(self,
                         urdf_obj,
                         joint_name):
         """
-        Get the joint axis in local frame.
+        Get the joint axis in the world frame.
 
         Parameters
         ----------
         urdf_obj : URDF_Obj
             A URDF_Obj that contains that joint whose axis is found.
         joint_name : string
             The name of the joint axis is returned.
 
         Returns
         -------
-        axis : array-like, shape(3,)
-            The joint axis in local frame.
+        axis_inW : array-like, shape(3,)
+            The joint axis in world frame.
+        pos_inW : array-like, shape(3,)
+            The (x,y,z) coords of the center of the child link in world coords.
+        link_name : string
+            The name of the child link of the joint.
 
         """
         # Gather information from urdf_obj
         urdf_id = urdf_obj.urdf_id
         joint_map = urdf_obj.joint_map
         
-        # Set the joint velocity
+        # If the joint exists
         if joint_name in joint_map:
+            
+            # Retrieve the joint axis in parent child coordinates
             joint_id = joint_map[joint_name]
             info = self.engine.getJointInfo(urdf_id,
                                             joint_id)
-            axis = info[13]
-            axis=np.array(axis).tolist()
-            return axis
+            axis_inC = np.array(info[13])
+            
+            # Get the child link
+            link_name = info[12].decode("utf-8")
+            link_id = urdf_obj.link_map[link_name]
+            
+            # Get the orientation of the child link if the child is the base
+            if link_id == -1:
+                child_state = self.get_base_state(urdf_obj=urdf_obj,
+                                                  body_coords=False)
+                R_ofW_inC = child_state['R of world in body']
+                pos_inW = child_state['position']
+                
+            # Get the orientation of the child link if the child is
+            # not the base
+            else:
+                child_state = self.get_link_state(urdf_obj=urdf_obj,
+                                                  link_name=link_name)
+                R_ofW_inC = child_state['R of world in link']
+                pos_inW = child_state['position']
+            
+            # Convert the child coord joint axis to world coords
+            R_ofC_inW = RAB_to_RBA(R_ofW_inC)
+            axis_inW = vc_inA_toB(R_ofC_inW, axis_inC)
+            return axis_inW, pos_inW, link_name
+        
+        # If the joint doesn't exist, return a default axis
+        else:
+            return np.array([0., 0., 1.]), "", np.array([0., 0., 0.])
             
             
     ###########################################################################
     #LINK SETTERS
     ###########################################################################
     def set_link_mass(self,
                       urdf_obj,
@@ -1257,53 +1259,90 @@
     ###########################################################################
     #LINK GETTERS
     ###########################################################################
     def get_link_state(self,
                        urdf_obj,
                        link_name):
         """
-        Gets the rigid body position and orientation of a link in world
-        cooridinates.
+        Gets the rigid body states (position and orientation) of a given
+        link of a given urdf. 
 
         Parameters
         ----------
         urdf_obj : URDF_Obj
-            A URDF_Obj that contrains the link whose state is being measured.
+            A URDF_Obj whose state is being measured.
         link_name : string
-            The name of the link to measure.
+            The name of the link whose state is measured. The link name is
+            specified in the .urdf file.
 
         Returns
         -------
-        state : dictionary with the following keys
+        state : a dictionary with the following keys:
             'position' : array-like, shape (3,)
-                Cartesian position of center of mass.
-            'orientation' : array-like, shape(4,)
-                Cartesian orientation of center of mass, in quaternion
-                [x,y,z,w]
+                The (x,y,z) world coordinates of the link.
+            'roll' : float
+                The Euler angle roll of the link
+                that defines the link's orientation in the world. Rotation
+                of the link about the world's x-axis.
+            'pitch' : float
+                The Euler angle pitch of the link
+                that defines the link's orientation in the world. Rotation
+                of the link about the world's y-axis.
+            'yaw' : float
+                The Euler angle yaw of the link
+                that defines the link's orientation in the world. Rotation
+                of the link about the world's z-axis.
+            'R of world in link' : array-like, shape(3,3):
+                The rotation matrix that takes vectors in world coordinates 
+                to link coordinates. For example, let V_inL be a 3vector
+                written in link coordinates. Let V_inW be a 3vector 
+                written in world coordinates. Then:
+                V_inL = R_ofWorld_inLink @ V_inW
 
         """
         # Get object id and link map
         urdf_id = urdf_obj.urdf_id
         link_map = urdf_obj.link_map
         
         # Get the link id
         if link_name in link_map:
-            link_id = [link_map[link_name]]
+            link_id = link_map[link_name]
         else:
             return
         
         # Retrieve the link states
-        link_states = self.engine.getLinkStates(urdf_id, link_id)
-        link_states = link_states[0]
-        pos_in_world = link_states[0]
-        ori_in_world = link_states[1]
-        
-        #  Make the dictionary
-        state = {'position' : pos_in_world,
-                 'orientation' : ori_in_world}
+        link_state = self.engine.getLinkState(urdf_id, link_id)
+        O_inW = link_state[0]
+        xyzw_ori = link_state[1]
+        
+        # Convert the orientation quaternion the Euler angles
+        rpy = self.engine.getEulerFromQuaternion(xyzw_ori)
+
+        # Get the rotation matrix of the link in world coords
+        # This rotation matrix takes vectors in link coordinates
+        # and places them in world coordinates.
+        R_ofL_inW = self.engine.getMatrixFromQuaternion(xyzw_ori)
+        R_ofL_inW = np.array(R_ofL_inW)
+        R_ofL_inW = np.reshape(R_ofL_inW, (3,3))
+        
+        # Get the rotation matrix of the world in body coords
+        # This rotation matrix takes vectors in world coordinates
+        # and places them in body coordinates.
+        R_ofW_inL = R_ofL_inW.T
+        
+        # Format the link state data
+        O_inW = np.array(O_inW)
+        rpy = np.array(rpy)
+        
+        # Make and return the state dictionary
+        state = {'position' : O_inW,
+                 'roll' : rpy[0],
+                 'pitch' : rpy[1],
+                 'yaw' : rpy[2],
+                 'R of world in link' : R_ofW_inL}
         return state
     
     
     def get_link_mass(self,
                       urdf_obj,
                       link_name):
         """
@@ -1410,29 +1449,25 @@
         
         # Return the set position and orientation
         return position, xyzw_ori
     
     
     def _set_base_vel(self,
                       urdf_obj,
-                      xyzw_ori,
                       velocity,
                       ang_velocity,
                       body_coords):
         """
         Sets the velocity and angular velocity of a urdf. Does not use physics.
 
         Parameters
         ----------
         urdf_path : string
             The path to the .urdf file that describes the urdf to be
             loaded into the simulation.
-        xyzw_ori : array-like, shape (4,)
-            A xyzw quaternion that describes the orientation of the
-            urdf.
         velocity : array-like, shape (3,)
             The velocity to be set in either world or body coords.
         ang_velocity : array-like, shape (3,)
             The angular velocity to be set in either world or body coords.
         body_coords : bool
             A boolean flag that indicates whether the passed velocities are in
             world coords or body coords.
@@ -1447,21 +1482,20 @@
         """
         # Get the urdf ID
         i = urdf_obj.urdf_id
         
         # If the velocities are passed in body coordinates, convert them
         # to world coordinates before setting them
         if body_coords:
-            R_ofB_inW = self.engine.getMatrixFromQuaternion(xyzw_ori)
-            R_ofB_inW = np.array(R_ofB_inW)
-            R_ofB_inW = np.reshape(R_ofB_inW, (3,3))
             v_inB = np.array(velocity)
             w_inB = np.array(ang_velocity)
-            v_inW = R_ofB_inW @ v_inB
-            w_inW = R_ofB_inW @ w_inB
+            v_inW = self._v_inB_to_vinW(urdf_obj=urdf_obj,
+                                        v_inB=v_inB)
+            w_inW = self._v_inB_to_vinW(urdf_obj=urdf_obj,
+                                        v_inB=w_inB)
         
         # If the velocities are already in world coords, do nothing
         else:
             v_inW = np.array(velocity)
             w_inW = np.array(ang_velocity)
             
         # Set the base velocity and angular velocity
@@ -1538,15 +1572,15 @@
         set_pitch = not (pitch is None)
         set_yaw = not (yaw is None)
         set_vel = not (velocity is None) 
         set_ang_vel = not (ang_velocity is None)
         
         # Get the current state
         current_state = self.get_base_state(urdf_obj=urdf_obj,
-                                            body_coords=False)
+                                            body_coords=body_coords)
         
         # If the position is not specified, set the current position
         if not set_pos:
             position = current_state['position']
     
         # If neither the orientation nor roll are specified,
         # set the current roll
@@ -1583,15 +1617,14 @@
                                                 wxyz_ori=wxyz_quaternion,
                                                 roll=roll,
                                                 pitch=pitch,
                                                 yaw=yaw)
         
         # Set linear and angular velocities
         v_inW, w_inW = self._set_base_vel(urdf_obj=urdf_obj,
-                                          xyzw_ori=xyzw_ori,
                                           velocity=velocity,
                                           ang_velocity=ang_velocity,
                                           body_coords=body_coords)
         
         # Handle the initial conditions
         if initial_cond:
             urdf_obj.initial_conds['position'] = position
@@ -1635,15 +1668,15 @@
             'yaw' : float
                 The Euler angle yaw of the base of the urdf
                 that define the body's orientation in the world. Rotation
                 of the body about the world's z-axis.
             'R of world in body' : array-like, shape(3,3):
                 The rotation matrix that takes vectors in world coordinates 
                 to body coordinates. For example, let V_inB be a 3vector
-                written in body coordinates. Let V_inW be a 2vector 
+                written in body coordinates. Let V_inW be a 3vector 
                 written in world coordinates. Then:
                 V_inB = R_ofWorld_inBody @ V_inW
             'velocity' : array-like, shape (3,)
                 The linear velocity of the base of the urdf in either world 
                 coords or body coords. Ordered as either
                 (vx_inW, vy_inW, vz_inW) or (vx_inB, vy_inB, vz_inB).
             'angular velocity' : array-like, shape (3,)
@@ -1765,90 +1798,118 @@
     ###########################################################################
     #EXTERNAL FORCE AND TORQUE APPLICATION
     ###########################################################################   
     def apply_force_to_link(self,
                             urdf_obj,
                             link_name,
                             force,
+                            link_coords=False,
                             show_arrow=False,
                             arrow_scale=0.4,
                             arrow_offset=0.0):
         """
         Applies an external force the to center of a specified link of a urdf.
 
         Parameters
         ----------
         urdf_obj : URDF_Obj
             A URDF_Obj that contains that link to which the force is applied.
         link_name : string
             The name of the link to which the force is applied.
             The link name is specified in the .urdf file.
         force : array-like, shape (3,)
-            The force vector in body coordinates to apply to the link.
+            The force vector in either world or link coordinates to apply to
+            the link.
+        link_coords : bool, optional
+            A boolean flag that indicates whether force is given in link
+            coords (True) or world coords (False). The default is False.
         show_arrow : bool, optional
             A boolean flag that indicates whether an arrow will be rendered
             on the link to visualize the applied force. The default is False.
         arrow_scale : float, optional
             The scaling factor that determines the size of the arrow. The
             default is 0.4.
         arrow_offset : float, optional
             The amount by which the drawn force arrow will be offset from the
             center of mass along the direction of the applied force. The 
             default is 0.0.
-            
+
         Returns
         -------
         None.
-
         """
+        
         # Do nothing if paused
         if self.paused:
             return
         
         # Gather information from urdf_obj
         urdf_id = urdf_obj.urdf_id
         link_map = urdf_obj.link_map
         
-        # Get the joint_id that defines the link
-        if link_name in link_map:
-            joint_id = link_map[link_name]
-        else:
-            return
+        # Get the center of the link in world cooridnates
+        link_state = self.get_link_state(urdf_obj=urdf_obj,
+                                         link_name=link_name)
+        link_inW = link_state['position']
+        
+        # Convert the force to the world frame
+        if link_coords:
+            f_inW = self._v_inB_to_vinW(urdf_obj, force)
+        else:
+            f_inW = np.array(force)
+        
+        # Apply the arrow offset to get the position of the base of the arrow
+        # in world coords
+        if np.linalg.norm(f_inW) != 0:
+            f_inW_dirn = f_inW / np.linalg.norm(f_inW)
+        else:
+            f_inW_dirn = np.array([0., 0., 0.])
+        arr_pos_inW = link_inW + arrow_offset*f_inW_dirn
+        arr_pos_inW = tuple(arr_pos_inW.tolist())
         
         # Draw the force arrow
-        self._apply_force_arrow(urdf_obj=urdf_obj,
-                                link_name=link_name,
-                                force=force,
+        self._draw_force_arrow(urdf_obj=urdf_obj,
+                                force_name=link_name,
+                                f_inW=f_inW,
+                                arr_pos_inW=arr_pos_inW,
+                                arr_scale=arrow_scale,
                                 show_arrow=show_arrow,
-                                arrow_scale=arrow_scale,
-                                arrow_offset=arrow_offset)
+                                force_update=False)
+        
+        # Get the link id to which force is applied
+        link_id = link_map[link_name]
         
-        # Apply the external force
+        # Apply a force to the highest link at the center of mass of the body
         self.engine.applyExternalForce(urdf_id,
-                                       joint_id,
-                                       force,
-                                       [0., 0., 0.],
-                                       flags=self.engine.LINK_FRAME)
+                                       link_id,
+                                       f_inW,
+                                       link_inW,
+                                       flags=self.engine.WORLD_FRAME)
                 
         
     def apply_force_to_com(self,
                            urdf_obj,
                            force,
+                           body_coords=False,
                            show_arrow=False,
                            arrow_scale=0.4,
                            arrow_offset=0.0):
         """
         Applies an external force to the center of mass of the body.
 
         Parameters
         ----------
         urdf_obj : URDF_Obj
             A URDF_Obj to which the force is applied.
         force : array-like, shape (3,)
-            The force vector in world coordinates to apply to the body.
+            The force vector in either world or body coordinates to apply to
+            the body.
+        body_coords : bool, optional
+            A boolean flag that indicates whether force is given in body
+            coords (True) or world coords (False). The default is False.
         show_arrow : bool, optional
             A boolean flag that indicates whether an arrow will be rendered
             on the com to visualize the applied force. The default is False.
         arrow_scale : float, optional
             The scaling factor that determines the size of the arrow. The
             default is 0.4.
         arrow_offset : float, optional
@@ -1865,100 +1926,56 @@
         if self.paused:
             return
         
         # Gather information from urdf_obj
         urdf_id = urdf_obj.urdf_id
         link_map = urdf_obj.link_map
         
-        # Get the highest link in the body tree
-        highest_link_id = min(link_map.values())
+        # Convert the force to the world frame
+        if body_coords:
+            f_inW = self._v_inB_to_vinW(urdf_obj, force)
+        else:
+            f_inW = np.array(force)
         
         # Get the center of mass of the body in world cooridnates
-        com = self.get_center_of_mass(urdf_obj)
-        if np.linalg.norm(force) != 0:
-            force_dirn = np.array(force) / np.linalg.norm(force)
-        else:
-            force_dirn = np.array([0., 0., 0.])
-        pos = com + arrow_offset*force_dirn
-        pos = tuple(pos.tolist())
+        com_inW = self.get_center_of_mass(urdf_obj)
         
-        # If the arrow isn't meant to be visualized, hide it
-        vis_exists = isinstance(self.vis, Visualizer)
-        arr_exists = 'COM' in self.lin_arr_map
-        if (not show_arrow) and vis_exists and arr_exists:
-            arrow_name = str(self.lin_arr_map['COM'])
-            path = Path(__file__).parents[0]
-            path = path.absolute().as_posix()
-            path = path + "/__assets__/arrow_lin.stl"
-            self.vis.set_link_color(urdf_name = "Force Arrows",
-                                    link_name = arrow_name,
-                                    stl_path=path, 
-                                    color = [0, 0, 0],
-                                    transparent = True,
-                                    opacity = 0.0)
+        # Apply the arrow offset to get the position of the base of the arrow
+        # in world coords
+        if np.linalg.norm(f_inW) != 0:
+            f_inW_dirn = f_inW / np.linalg.norm(f_inW)
+        else:
+            f_inW_dirn = np.array([0., 0., 0.])
+        arr_pos_inW = com_inW + arrow_offset*f_inW_dirn
+        arr_pos_inW = tuple(arr_pos_inW.tolist())
         
-        # Handle force arrow visualization
-        if show_arrow and isinstance(self.vis, Visualizer):
-            # Get the orientation of the force arrow
-            xyzw_ori = get_rot_from_2_vecs([0,0,1], force)
-            wxyz_ori = xyzw_to_wxyz(xyzw_ori)
-            
-            # Get the scale of the arrow based on the magnitude of the force
-            scale = arrow_scale*np.linalg.norm(force)*np.array([1., 1., 1.])
-            scale=scale.tolist()
-            
-            # If the arrow already exists, only update its position and ori
-            if 'COM' in self.lin_arr_map:
-                arrow_name = str(self.lin_arr_map['COM'])
-                path = Path(__file__).parents[0]
-                path = path.absolute().as_posix()
-                path = path + "/__assets__/arrow_lin.stl"
-                self.vis.set_link_color(urdf_name = "Force Arrows",
-                                        link_name = arrow_name,
-                                        stl_path=path, 
-                                        color = [0, 0, 0],
-                                        transparent = False,
-                                        opacity = 1.0)
-                self.vis.apply_transform(urdf_name="Force Arrows",
-                                         link_name=arrow_name,
-                                         scale=scale,
-                                         translate=pos,
-                                         wxyz_quaternion=wxyz_ori)
-            
-            # If the arrow is not already created, add it to the visualizer
-            else:
-                # Add the arrow to the linear arrow map
-                self.lin_arr_map['COM'] = len(self.lin_arr_map)
-                arrow_name = str(self.lin_arr_map['COM'])
-                path = Path(__file__).parents[0]
-                path = path.absolute().as_posix()
-                path = path + "/__assets__/arrow_lin.stl"
-                
-                # Add an arrow to the visualizer
-                self.vis.add_stl(urdf_name="Force Arrows",
-                                 link_name=arrow_name,
-                                 stl_path=path,
-                                 color = [0, 0, 0],
-                                 transparent=False,
-                                 opacity = 1.0,
-                                 scale=scale,
-                                 translate=pos,
-                                 wxyz_quaternion=wxyz_ori)
+        # Draw the force arrow
+        self._draw_force_arrow(urdf_obj=urdf_obj,
+                               force_name='Center_of_Mass',
+                               f_inW=f_inW,
+                               arr_pos_inW=arr_pos_inW,
+                               arr_scale=arrow_scale,
+                               show_arrow=show_arrow,
+                               force_update=False)
+        
+        # Get the highest link in the body tree
+        root_link_id = min(link_map.values())
         
         # Apply a force to the highest link at the center of mass of the body
         self.engine.applyExternalForce(urdf_id,
-                                       highest_link_id,
-                                       force,
-                                       com,
+                                       root_link_id,
+                                       f_inW,
+                                       com_inW,
                                        flags=self.engine.WORLD_FRAME)
-        
-        
+
+
     def apply_external_torque(self,
                               urdf_obj,
                               torque,
+                              body_coords=False,
                               show_arrow=False,
                               arrow_scale=0.1,
                               arrow_offset=0.0):
         """
         Applies an external torque to the center of mass of the body.
 
         Parameters
@@ -1987,208 +2004,314 @@
         if self.paused:
             return
         
         # Gather information from urdf_obj
         urdf_id = urdf_obj.urdf_id
         link_map = urdf_obj.link_map
         
-        # Get the highest link in the body tree
-        highest_link_id = min(link_map.values())
+        # Convert the torque to the world frame
+        if body_coords:
+            t_inW = self._v_inB_to_vinW(urdf_obj, torque)
+        else:
+            t_inW = np.array(torque)
         
         # Get the center of mass of the body in world cooridnates
-        com = self.get_center_of_mass(urdf_obj)
-        torque_dirn = np.array(torque) / np.linalg.norm(torque)
-        pos = com + arrow_offset*torque_dirn
-        pos = tuple(pos.tolist())
+        com_inW = self.get_center_of_mass(urdf_obj)
+        
+        # Apply the arrow offset to get the position of the base of the arrow
+        # in world coords
+        if np.linalg.norm(t_inW) != 0:
+            t_inW_dirn = t_inW / np.linalg.norm(t_inW)
+        else:
+            t_inW_dirn = np.array([0., 0., 0.])
+        arr_pos_inW = com_inW + arrow_offset*t_inW_dirn
+        arr_pos_inW = tuple(arr_pos_inW.tolist())
+        
+        # Draw the torque arrow
+        self._draw_torque_arrow(urdf_obj=urdf_obj,
+                                torque_name='Center_of_Mass',
+                                t_inW=t_inW,
+                                arr_pos_inW=arr_pos_inW,
+                                arr_scale=arrow_scale,
+                                show_arrow=show_arrow,
+                                force_update=False)
+        
+        # Get the highest link in the body tree
+        root_link_id = min(link_map.values())
         
-        # If the arrow isn't meant to be visualized, hide it
+        # Apply a force to the highest link at the center of mass of the body
+        self.engine.applyExternalTorque(urdf_id,
+                                        root_link_id,
+                                        t_inW,
+                                        flags=self.engine.WORLD_FRAME)
+
+
+    ###########################################################################
+    #DRAWING FOR AND TORQUE ARROWS
+    ########################################################################### 
+    def _draw_force_arrow(self,
+                          urdf_obj,
+                          force_name,
+                          f_inW,
+                          arr_pos_inW,
+                          arr_scale,
+                          show_arrow,
+                          force_update=False):
+        """
+        Draws a force arrow based on force applied at a location.
+
+        Parameters
+        ----------
+        urdf_obj : URDF_Obj
+            A URDF_Obj that contains that link to which the force is applied.
+        force_name : string
+            The name of the force applied.
+        f_inW : array-like, shape (3,)
+            The force vector in world coordinates to apply to the link.
+        arr_pos_inW : array-like, shape(3,)
+            The position of the base of the arrow in world coords.
+        arr_scale : float
+            The scaling factor that determines the size of the arrow.
+        show_arrow : bool
+            A boolean flag that indicates whether an arrow will be rendered
+            on the link to visualize the applied force
+        force_update : bool, optional
+            A boolean flag that indicates whether or not visualizer frame rate
+            will be ignored and the arrow will update immediately. The default
+            is False
+            
+        Returns
+        -------
+        None.
+
+        """
+        # If we cannot update the arrow, do nothing
+        if not self.vis_time_okay and not force_update:
+            return
+        
+        # Get the URDF ID and combine with link name to get the key to the 
+        # linear arrow map
+        urdf_id = str(urdf_obj.urdf_id)
+        urdf_force = urdf_id + "__" + force_name
+        
+        # Make sure the visualizer exists and check the current status of the 
+        # arrow
         vis_exists = isinstance(self.vis, Visualizer)
-        arr_exists = 'COM' in self.ccw_arr_map
-        if (not show_arrow) and vis_exists and arr_exists:
-            arrow_name = str(self.lin_arr_map['COM'])    
-            path = Path(__file__).parents[0]
-            path = path.absolute().as_posix()
-            path = path + "/__assets__/arrow_ccw.stl"
-            self.vis.set_link_color(urdf_name = "Torque Arrows",
-                                    link_name = arrow_name,
-                                    stl_path=path, 
+        arr_exists = urdf_force in self.lin_arr_map
+        
+        # If the visualizer doesn't exist, leave
+        if not vis_exists:
+            return
+        
+        # If show_arrow is set to false, and the visualizer and associated
+        # force arrow exist, set the arrows visibility to false
+        if (not show_arrow) and arr_exists:
+            arr_name = str(self.lin_arr_map[urdf_force])
+            self.vis.set_link_color(urdf_name = "Force Arrows",
+                                    link_name = arr_name,
+                                    link_geometry = self.lin_geom, 
                                     color = [0, 0, 0],
                                     transparent = True,
                                     opacity = 0.0)
         
-        # Handle force arrow visualization
-        if show_arrow and isinstance(self.vis, Visualizer):
-            # Get the orientation of the force arrow
-            xyzw_ori = get_rot_from_2_vecs([0,0,1], torque)
-            wxyz_ori = xyzw_to_wxyz(xyzw_ori)
+        # If show arrow is set to True and the visualizer exists, draw the
+        # arrow at the position and orientation listed.
+        if show_arrow:
+            
+            # Get the direction in which the force is applied
+            if np.linalg.norm(f_inW) != 0:
+                arr_dirn_inW = f_inW / np.linalg.norm(f_inW)
+            else:
+                arr_dirn_inW = np.array([0., 0., 0.])
+                
+            # Get the orientation of the force arrow based on the direction
+            # that it's pointing
+            arr_xyzw_inW = get_rot_from_2_vecs([0,0,1], arr_dirn_inW)
+            arr_wxyz_inW = xyzw_to_wxyz(arr_xyzw_inW)
             
             # Get the scale of the arrow based on the magnitude of the force
-            scale = arrow_scale*np.linalg.norm(torque)*np.array([1., 1., 0.1])
-            scale=scale.tolist()
+            scale = arr_scale*np.linalg.norm(f_inW)*np.array([1., 1., 1.])
+            scale = scale.tolist()
             
             # If the arrow already exists, only update its position and ori
-            if 'COM' in self.ccw_arr_map:
-                arrow_name = str(self.ccw_arr_map['COM'])
-                path = Path(__file__).parents[0]
-                path = path.absolute().as_posix()
-                path = path + "/__assets__/arrow_ccw.stl"
-                self.vis.set_link_color(urdf_name = "Torque Arrows",
-                                        link_name = arrow_name,
-                                        stl_path=path, 
+            if arr_exists:
+                # Get the arrow's name
+                arr_name = str(self.lin_arr_map[urdf_force])
+                
+                # Set the visibility of the arrow to True
+                self.vis.set_link_color(urdf_name = "Force Arrows",
+                                        link_name = arr_name,
+                                        link_geometry = self.lin_geom, 
                                         color = [0, 0, 0],
                                         transparent = False,
                                         opacity = 1.0)
-                self.vis.apply_transform(urdf_name="Torque Arrows",
-                                         link_name=arrow_name,
+                
+                # Set the position and orientation of the arrow
+                self.vis.apply_transform(urdf_name="Force Arrows",
+                                         link_name=arr_name,
                                          scale=scale,
-                                         translate=pos,
-                                         wxyz_quaternion=wxyz_ori)
+                                         translate=arr_pos_inW,
+                                         wxyz_quaternion=arr_wxyz_inW)
+            
             
             # If the arrow is not already created, add it to the visualizer
             else:
                 # Add the arrow to the linear arrow map
-                self.ccw_arr_map['COM'] = len(self.ccw_arr_map)
-                arrow_name = str(self.ccw_arr_map['COM'])
-                path = Path(__file__).parents[0]
-                path = path.absolute().as_posix()
-                path = path + "/__assets__/arrow_ccw.stl"
+                self.lin_arr_map[urdf_force] = force_name
+                
+                # Get the arrow's name
+                arr_name = self.lin_arr_map[urdf_force]
+                
+                # Get the path to the arrow asset
+                arr_path = Path(__file__).parents[0]
+                arr_path = arr_path.absolute().as_posix()
+                arr_path = arr_path + "/__assets__/arrow_lin.stl"
                 
                 # Add an arrow to the visualizer
-                self.vis.add_stl(urdf_name="Torque Arrows",
-                                 link_name=arrow_name,
-                                 stl_path=path,
-                                 color = [0, 0, 0],
-                                 transparent=False,
-                                 opacity = 1.0,
-                                 scale=scale,
-                                 translate=pos,
-                                 wxyz_quaternion=wxyz_ori)
-        
-        # Apply a force to the highest link at the center of mass of the body
-        self.engine.applyExternalTorque(urdf_id,
-                                        highest_link_id,
-                                        torque,
-                                        flags=self.engine.WORLD_FRAME)
-        
-        
-    def _apply_force_arrow(self,
+                self.lin_geom,_=self.vis.add_stl(urdf_name="Force Arrows",
+                                                 link_name=arr_name,
+                                                 stl_path=arr_path,
+                                                 color = [0, 0, 0],
+                                                 transparent=False,
+                                                 opacity = 1.0,
+                                                 scale=scale,
+                                                 translate=arr_pos_inW,
+                                                 wxyz_quaternion=arr_wxyz_inW)
+                
+                
+    def _draw_torque_arrow(self,
                            urdf_obj,
-                           link_name,
-                           force,
+                           torque_name,
+                           t_inW,
+                           arr_pos_inW,
+                           arr_scale,
                            show_arrow,
-                           arrow_scale,
-                           arrow_offset):
+                           force_update=False):
         """
-        Draws a body coordinate force arrow based on force applied to a link.
+        Draws a torque arrow based on torque applied at a location.
 
         Parameters
         ----------
         urdf_obj : URDF_Obj
-            A URDF_Obj that contains that link to which the force is applied.
-        link_name : string
-            The name of the link to which the force is applied.
-            The link name is specified in the .urdf file.
-        force : array-like, shape (3,)
-            The force vector in body coordinates to apply to the link.
+            A URDF_Obj that contains that link to which the torque is applied.
+        torque_name : string
+            The name of the torque applied.
+        t_inW : array-like, shape (3,)
+            The torque vector in world coordinates to apply to the link.
+        arr_pos_inW : array-like, shape(3,)
+            The position of the base of the arrow in world coords.
+        arr_scale : float
+            The scaling factor that determines the size of the arrow.
         show_arrow : bool
             A boolean flag that indicates whether an arrow will be rendered
-            on the link to visualize the applied force
-        arrow_scale : float
-            The scaling factor that determines the size of the arrow.
-        arrow_offset : float
-            The amount by which the drawn force arrow will be offset from the
-            center of mass along the direction of the applied force.
+            on the link to visualize the applied torque
+        force_update : bool, optional
+            A boolean flag that indicates whether or not visualizer frame rate
+            will be ignored and the arrow will update immediately. The default
+            is False
             
         Returns
         -------
         None.
 
         """
-        # If the arrow isn't meant to be visualized, hide it
+        # If we cannot update the arrow, do nothing
+        if not self.vis_time_okay and not force_update:
+            return
+        
+        # Get the URDF ID and combine with link name to get the key to the 
+        # ccw arrow map
+        urdf_id = str(urdf_obj.urdf_id)
+        urdf_torque = urdf_id + "__" + torque_name
+        
+        # Make sure the visualizer exists and check the current status of the 
+        # arrow
         vis_exists = isinstance(self.vis, Visualizer)
-        arr_exists = link_name in self.lin_arr_map
-        if (not show_arrow) and vis_exists and arr_exists:
-            arrow_name = str(self.lin_arr_map[link_name])
-            path = Path(__file__).parents[0]
-            path = path.absolute().as_posix()
-            path = path + "/__assets__/arrow_lin.stl"
-            self.vis.set_link_color(urdf_name = "Force Arrows",
-                                    link_name = arrow_name,
-                                    stl_path=path, 
+        arr_exists = urdf_torque in self.ccw_arr_map
+        
+        # If the visualizer doesn't exist, leave
+        if not vis_exists:
+            return
+        
+        # If show_arrow is set to false, and the visualizer and associated
+        # torque arrow exist, set the arrows visibility to false
+        if (not show_arrow) and arr_exists:
+            arr_name = str(self.ccw_arr_map[urdf_torque])
+            self.vis.set_link_color(urdf_name = "Torque Arrows",
+                                    link_name = arr_name,
+                                    link_geometry = self.ccw_geom, 
                                     color = [0, 0, 0],
                                     transparent = True,
                                     opacity = 0.0)
         
-        # Handle force arrow visualization
-        if show_arrow and isinstance(self.vis, Visualizer):
-            
-            # Get the orientation, in body coordinates, of the arrow based
-            # on direction of force
-            arrow_xyzw_in_body = get_rot_from_2_vecs([0,0,1], force)
-            
-            # Get the link state
-            state = self.get_link_state(urdf_obj=urdf_obj,
-                                        link_name=link_name)
-            pos = state['position']
-            if np.linalg.norm(force) != 0:
-                force_dirn = np.array(force) / np.linalg.norm(force)
+        # If show arrow is set to True and the visualizer exists, draw the
+        # arrow at the position and orientation listed.
+        if show_arrow:
+            
+            # Get the direction in which the torque is applied
+            if np.linalg.norm(t_inW) != 0:
+                arr_dirn_inW = t_inW / np.linalg.norm(t_inW)
             else:
-                force_dirn = np.array([0., 0., 0.])
-            pos = np.array(pos) + arrow_offset*force_dirn
-            pos = tuple(pos.tolist())
-            body_xyzw_in_world = state['orientation']
-            body_xyzw_in_world = np.array(body_xyzw_in_world)
-            
-            # Combine the two rotations
-            xyzw_ori = xyzw_quat_mult(arrow_xyzw_in_body, body_xyzw_in_world)
-            wxyz_ori = xyzw_to_wxyz(xyzw_ori)
+                arr_dirn_inW = np.array([0., 0., 0.])
+                
+            # Get the orientation of the torque arrow based on the direction
+            # that it's pointing
+            arr_xyzw_inW = get_rot_from_2_vecs([0,0,1], arr_dirn_inW)
+            arr_wxyz_inW = xyzw_to_wxyz(arr_xyzw_inW)
             
-            # Get the scale of the arrow based on the magnitude of the force
-            scale = arrow_scale*np.linalg.norm(force)*np.array([1., 1., 1.])
-            scale=scale.tolist()
+            # Get the scale of the arrow based on the magnitude of the torque
+            scale = arr_scale*np.linalg.norm(t_inW)*np.array([1., 1., 0.05])
+            scale = scale.tolist()
             
             # If the arrow already exists, only update its position and ori
-            if link_name in self.lin_arr_map:
-                arrow_name = str(self.lin_arr_map[link_name])
-                path = Path(__file__).parents[0]
-                path = path.absolute().as_posix()
-                path = path + "/__assets__/arrow_lin.stl"
-                self.vis.set_link_color(urdf_name = "Force Arrows",
-                                        link_name = arrow_name,
-                                        stl_path=path, 
+            if arr_exists:
+                # Get the arrow's name
+                arr_name = str(self.ccw_arr_map[urdf_torque])
+                
+                # Set the visibility of the arrow to True
+                self.vis.set_link_color(urdf_name = "Torque Arrows",
+                                        link_name = arr_name,
+                                        link_geometry = self.ccw_geom, 
                                         color = [0, 0, 0],
                                         transparent = False,
                                         opacity = 1.0)
-                self.vis.apply_transform(urdf_name="Force Arrows",
-                                         link_name=arrow_name,
+                
+                # Set the position and orientation of the arrow
+                self.vis.apply_transform(urdf_name="Torque Arrows",
+                                         link_name=arr_name,
                                          scale=scale,
-                                         translate=pos,
-                                         wxyz_quaternion=wxyz_ori)
+                                         translate=arr_pos_inW,
+                                         wxyz_quaternion=arr_wxyz_inW)
+            
             
             # If the arrow is not already created, add it to the visualizer
             else:
                 # Add the arrow to the linear arrow map
-                self.lin_arr_map[link_name] = len(self.lin_arr_map)
-                arrow_name = str(self.lin_arr_map[link_name])
-                path = Path(__file__).parents[0]
-                path = path.absolute().as_posix()
-                path = path + "/__assets__/arrow_lin.stl"
+                self.ccw_arr_map[urdf_torque] = torque_name
                 
-                # Add an arrow to the visualizer
-                self.vis.add_stl(urdf_name="Force Arrows",
-                                 link_name=arrow_name,
-                                 stl_path=path,
-                                 color = [0, 0, 0],
-                                 transparent=False,
-                                 opacity = 1.0,
-                                 scale=scale,
-                                 translate=pos,
-                                 wxyz_quaternion=wxyz_ori)
+                # Get the arrow's name
+                arr_name = self.ccw_arr_map[urdf_torque]
                 
+                # Get the path to the arrow asset
+                arr_path = Path(__file__).parents[0]
+                arr_path = arr_path.absolute().as_posix()
+                arr_path = arr_path + "/__assets__/arrow_ccw.stl"
                 
+                # Add an arrow to the visualizer
+                self.ccw_geom,_=self.vis.add_stl(urdf_name="Torque Arrows",
+                                                 link_name=arr_name,
+                                                 stl_path=arr_path,
+                                                 color = [0, 0, 0],
+                                                 transparent=False,
+                                                 opacity = 1.0,
+                                                 scale=scale,
+                                                 translate=arr_pos_inW,
+                                                 wxyz_quaternion=arr_wxyz_inW)
+    
+    
     ###########################################################################
     #URDF VISUALIZATION MANIPULATION
     ###########################################################################
     def add_urdf_to_visualizer(self,
                                urdf_obj,
                                tex_path=None):
         """
@@ -2230,38 +2353,46 @@
         tex_path = format_path(tex_path)
         
         # Loop through all the links
         for i in range(len(paths)):
             
             # If the current link is defined by an .obj file
             if paths[i][-4:] == ".obj":
-                self.vis.add_obj(urdf_name=urdf_name,
-                                 link_name=names[i],
-                                 obj_path=paths[i],
-                                 tex_path=tex_path,
-                                 scale=scales[i],
-                                 translate=poss[i],
-                                 wxyz_quaternion=oris[i])
+                geom, tex = self.vis.add_obj(urdf_name=urdf_name,
+                                             link_name=names[i],
+                                             obj_path=paths[i],
+                                             tex_path=tex_path,
+                                             scale=scales[i],
+                                             translate=poss[i],
+                                             wxyz_quaternion=oris[i])
+                
+                # Save the texture and geometry
+                urdf_obj.geometries.append(geom)
+                urdf_obj.textures.append(tex)
                 
             # If the current link is defined by an .stl file
             elif paths[i][-4:] == ".stl":
                 link_name = names[i]
                 rgb = format_RGB(colors[i][0:3],
                                   range_to_255=True)
                 opacity = colors[i][3]
                 transparent = opacity != 1.0
-                self.vis.add_stl(urdf_name=urdf_name,
-                                 link_name=link_name,
-                                 stl_path=paths[i],
-                                 color=rgb,
-                                 transparent=transparent,
-                                 opacity=opacity,
-                                 scale=scales[i],
-                                 translate=poss[i],
-                                 wxyz_quaternion=oris[i])
+                geom, tex = self.vis.add_stl(urdf_name=urdf_name,
+                                             link_name=link_name,
+                                             stl_path=paths[i],
+                                             color=rgb,
+                                             transparent=transparent,
+                                             opacity=opacity,
+                                             scale=scales[i],
+                                             translate=poss[i],
+                                             wxyz_quaternion=oris[i])
+
+                # Save the texture and geometry
+                urdf_obj.geometries.append(geom)
+                urdf_obj.textures.append(tex)
 
     
     def _update_urdf_visual(self,
                             urdf_obj):
         """
         Updates the positions of dynamic links in the Visualizer.
 
@@ -2345,15 +2476,15 @@
             scale = list(vis_datum[3])
             scales.append(scale)
             color = list(vis_datum[7])
             colors.append(color)
             
             # Extract link id
             link_id = vis_datum[1]
-            
+
             # Link id of -1 implies that the current link is the base
             # of a robot
             if link_id == -1:
                 base_link_name = self.engine.getBodyInfo(urdf_id)[0]
                 base_link_name = base_link_name.decode('UTF-8')
                 link_names.append(base_link_name)
                 pos_ori = self.engine.getBasePositionAndOrientation(urdf_id)
@@ -2430,35 +2561,27 @@
             return
     
         # Get name and id data from urdf_obj
         urdf_id = urdf_obj.urdf_id
         urdf_name = str(urdf_id)
         link_id = urdf_obj.link_map[link_name]
         
-        # Get current visual data for the requested link
-        vis_data = self.engine.getVisualShapeData(urdf_id)
-        stl_path = ""
-        for vis_datum in vis_data:
-            if vis_datum[1] == link_id:
-                stl_path = vis_datum[4]
-            
-        # Format stl path
-        stl_path = format_path(stl_path.decode('UTF-8'))
+        # Get the link's geometry
+        link_geometry = urdf_obj.geometries[link_id]
         
         # Ensure color is in proper format
-        color = format_RGB(color,
-                            range_to_255=False)
+        color = format_RGB(color, range_to_255=False)
         
         # Set the requested color
         self.vis.set_link_color(urdf_name = urdf_name,
-                                   link_name = link_name,
-                                   stl_path = stl_path, 
-                                   color = color,
-                                   transparent = transparent,
-                                   opacity = opacity)
+                                link_name = link_name,
+                                link_geometry = link_geometry, 
+                                color = color,
+                                transparent = transparent,
+                                opacity = opacity)
 
 
     def set_color_from_pos(self,
                            urdf_obj,
                            joint_name,
                            min_pos,
                            max_pos):
@@ -3380,14 +3503,15 @@
         if self.paused:
             return
         
         # Note the simulation is no longer done and reset the time
         self.is_done = False
         self.time = 0.
         self.last_step_time = time.time()
+        self.vis_time_okay = True
         
         # Reset each urdf
         for urdf_obj in self.urdf_objs:
             
             # Reset the base position and orientation of all urdfs
             i = urdf_obj.urdf_id
             p = urdf_obj.initial_conds['position']
@@ -3504,16 +3628,18 @@
         # Step the physics engine
         curr_step_time = time.time()
         self.engine.stepSimulation()
         self.time = self.time + self.dt
 
         # Update the visualizer if it exists
         time_since_last_vis = curr_step_time - self.last_vis_time
-        vis_time_okay =  time_since_last_vis >= (1. / self.visualization_fr)
-        if vis_time_okay and update_vis and isinstance(self.vis, Visualizer):
+        self.vis_time_okay=time_since_last_vis >= (1. / self.visualization_fr)
+        vis_exists = isinstance(self.vis, Visualizer)
+        if self.vis_time_okay and update_vis and vis_exists:
+            self.last_vis_time = curr_step_time
             for urdf_obj in self.urdf_objs:
                 if urdf_obj.update_vis:
                     self._update_urdf_visual(urdf_obj)
        
         # Update the animator if it exists
         if update_ani and isinstance(self.ani, Animator):
             self.ani.step()
```

### Comparing `condynsate-0.5.7/src/condynsate/utils.py` & `condynsate-0.6.0/src/condynsate/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -280,7 +280,111 @@
     if range_to_255:
         rgb_255 = np.round(rgb*255)
     else:
         rgb_255 = np.round(rgb)
     rgb_255_int = rgb_255.astype(int)
     list_rgb_255_int = rgb_255_int.tolist()
     return list_rgb_255_int
+
+
+def RAB_to_RBA(R_ofA_inB):
+    """
+    Takes a rotation cosine matrix of the A frame in B coords to the rotation
+    cosine of the B frame in A coords.
+
+    Parameters
+    ----------
+    R_ofA_inB : valid rotation matrix, shape(3,3)
+        The rotation cosine matrix of the A frame in B coords.
+
+    Returns
+    -------
+    R_ofB_inA : valid rotation matrix, shape(3,3)
+        The rotation cosine matrix of the B frame in A coords.
+
+    """
+    R_ofB_inA = np.array(R_ofA_inB).T
+    return R_ofB_inA
+    
+
+def OAB_to_OBA(R_ofA_inB, O_ofA_inB):
+    """
+    Takes the origin of frame A in B coords to the origin of frame B in A
+    coords.
+
+    Parameters
+    ----------
+    R_ofA_inB : valid rotation matrix, shape(3,3)
+        The rotation cosine matrix of the A frame in B coords.
+    O_ofA_inB : array, shape(3,)
+        The origin of frame A in B coords.
+
+    Returns
+    -------
+    O_ofB_inA : array, shape(3,)
+        The origin of frame B in A coords.
+
+    """
+    R_ofB_inA = RAB_to_RBA(R_ofA_inB)
+    O_ofB_inA = -R_ofB_inA @ np.array(O_ofA_inB)
+    return O_ofB_inA
+
+
+def vc_inA_toB(R_ofA_inB, vc_inA):
+    """
+    Based on a relative cosine matrix, takes vecotrs in frame A coords to 
+    frame B coords.
+    
+    Parameters
+    ----------
+    R_ofA_inB : valid rotation matrix, shape(3,3)
+        The rotation cosine matrix of the A frame in B coords.
+    vc_inA : array, shape(3,)
+        A 3 vector in frame A.
+
+    Returns
+    -------
+    vc_inB : array, shape(3,)
+        The same 3 vector in frame B coords.
+
+    """
+    vc_inB = np.array(R_ofA_inB) @ np.array(vc_inA)
+    return vc_inB
+    
+
+def pt_inA_toB(R_ofA_inB, O_ofA_inB, pt_inA):
+    """
+    Based on a relative cosine matrix and origin vector, takes a point in frame
+    A coords to frame B coords.
+
+    Parameters
+    ----------
+    R_ofA_inB : valid rotation matrix, shape(3,3)
+        The rotation cosine matrix of the A frame in B coords.
+    O_ofA_inB : array, shape(3,)
+        The origin of frame A in B coords.
+    pt_inA : array, shape(3,)
+        A 3D point in frame A.
+
+    Returns
+    -------
+    pt_inB : array, shape(3,)
+        The same 3D point in B coords.
+
+    """
+    pt_inB = np.array(R_ofA_inB) @ np.array(pt_inA) + np.array(O_ofA_inB)
+    return pt_inB
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+    
+
```

### Comparing `condynsate-0.5.7/src/condynsate/visualizer.py` & `condynsate-0.6.0/src/condynsate/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,16 +80,19 @@
             The default is [0., 0., 0.].
         wxyz_quaternion : array-like, size (4,), optional
             The wxyz quaternion that defines the initial rotation applied to
             the .obj. The default is [1., 0., 0., 0.].
 
         Returns
         -------
-        None.
-
+        obj_geometry : meshcat.geometry.ObjMeshGeometry
+            The object mesh.
+        obj_texture : meshcat.geometry.MeshPhongMaterial
+            The object texture.
+            
         """
         # Get geometry of object from the .obj file at obj_path
         obj_path = format_path(obj_path)
         obj_geometry = geo.ObjMeshGeometry.from_file(obj_path)
         
         # Get the texture of object from the .png file at tex_path
         tex_path = format_path(tex_path)
@@ -102,14 +105,17 @@
         # Calculate the transform
         transform = self._get_transform(scale, translate, wxyz_quaternion)
 
         # Add and transform the object to its orientation and position
         self.scene[urdf_name][link_name].set_object(obj_geometry, obj_texture)
         self.scene[urdf_name][link_name].set_transform(transform)
         
+        # Return the geometry and texture
+        return obj_geometry, obj_texture
+        
         
     def add_stl(self,
                 urdf_name,
                 link_name,
                 stl_path,
                 color = [91, 155, 213],
                 transparent=False,
@@ -146,15 +152,18 @@
             The default is [0., 0., 0.].
         wxyz_quaternion : array-like, size (4,), optional
             The wxyz quaternion that defines the initial rotation applied to
             the .stl. The default is [1., 0., 0., 0.].
 
         Returns
         -------
-        transform : None.
+        link_geometry : meshcat.geometry.StlMeshGeometry
+            The link mesh.
+        link_mat : meshcat.geometry.MeshPhongMaterial
+            The link material.
 
         """
         # Set the parts's geometry
         stl_path = format_path(stl_path)
         link_geometry = geo.StlMeshGeometry.from_file(stl_path)
         
         # Set the parts's color
@@ -169,54 +178,51 @@
         # Calculate the transform
         transform = self._get_transform(scale, translate, wxyz_quaternion)
 
         # Add and transform the link to its orientation and position
         self.scene[urdf_name][link_name].set_object(link_geometry, link_mat)
         self.scene[urdf_name][link_name].set_transform(transform)
         
+        # Return the geometry and material
+        return link_geometry, link_mat
+    
     
     def set_link_color(self,
                        urdf_name,
                        link_name,
-                       stl_path, 
+                       link_geometry,
                        color = [91, 155, 213],
                        transparent = False,
                        opacity = 1.0):
         """
         Set a link color by deleting it and then adding another copy of it.
 
         Parameters
         ----------
         urdf_name : string
             The name of the urdf that contains the link being refreshed.
             URDF objects define robots or assemblies.
         link_name : string
             The name of the link.
-        stl_path : string
-            The relative path pointing to the .stl description of the link that
-            is being refreshed.
+        link_geometry : meshcat.geometry.StlMeshGeometry
+            The link mesh.
         color : array-like, size (3,), optional
             The 0-255 RGB color of the link. The default is [91, 155, 213].
         transparent : boolean, optional
             A boolean that indicates if the link is transparent.
             The default is False.
         opacity : float, optional
             The opacity of the link. Can take float values between 0.0 and 1.0.
             The default is 1.0.
 
         Returns
         -------
         None.
 
-        """
-        
-        # Set the parts's geometry
-        stl_path = format_path(stl_path)
-        link_geometry = geo.StlMeshGeometry.from_file(stl_path)
-        
+        """        
         # Set the parts's color
         color_int = color[0]*256**2 + color[1]*256 + color[2]
         link_mat = geo.MeshPhongMaterial(color=color_int,
                                          transparent=transparent,
                                          opacity=opacity,
                                          reflectivity=0.3)
```

### Comparing `condynsate-0.5.7/src/condynsate.egg-info/PKG-INFO` & `condynsate-0.6.0/src/condynsate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.5.7
+Version: 0.6.0
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -51,16 +51,14 @@
 Requires-Dist: pyside6
 Requires-Dist: sympy
 
 # condynsate
 
  [condynsate](https://github.com/GrayKS3248/condynsate) is a dynamic system simulation and visualization tool built with [PyBullet](https://pybullet.org/wordpress/) and [MeshCat](https://github.com/meshcat-dev/meshcat-python). It automatically simulates multiple objects and their interactions as described by [.urdf](http://wiki.ros.org/urdf), [.stl](https://en.wikipedia.org/wiki/STL_(file_format)), and [.obj](https://en.wikipedia.org/wiki/Wavefront_.obj_file) files and can render real time visualizations in a web browser.
 
-
-
 # Installation
 
 ## From Source
 
 condynsate requires python => 3.8
 
 ```bash
@@ -74,16 +72,14 @@
   * [Install Miniconda.](https://docs.conda.io/projects/miniconda/en/latest/)
   
   * To verify that Miniconda is installed properly, open **Anaconda Prompt (Miniconda3)** and run the command:
     
     ```bash
     conda --version
     ```
-    
-    
 
 * **Create a new virtual environment**
   
   * To create a new environment, open **Anaconda Prompt (Miniconda3)** and run the command:
     
     ```bash
     conda create -n ENVNAME
@@ -92,16 +88,14 @@
   * Next, activate the newly made environment: 
     
     ```bash
     conda activate ENVNAME
     ```
   
   * You can confirm the virtual environment is activated when environment name on the left side of the command line changes from ``(base)`` to``(ENVNAME)``
-    
-    
 
 * **Install dependencies from Conda-Forge:**
   
   * Configure the environment channels by running the commands:
     
     ```bash
     conda config --env --add channels conda-forge
@@ -110,16 +104,14 @@
     ```
   
   * Install dependencies available from Conda-Forge by running the command:
     
     ```bash
     conda install -y python=3 numpy pynput matplotlib pybullet control sympy notebook
     ```
-    
-    
 
 * **Install condynsate using pip**
   
   * To install condynsate run the commands:
     
     ```bash
     pip cache purge
@@ -130,12 +122,10 @@
     
     ```python
     python
     import condynsate
     condynsate.__version__ 
     ```
 
- 
-
 # Usage
 
 For examples of usage, see [examples](https://github.com/GrayKS3248/condynsate/tree/main/examples).
```

### Comparing `condynsate-0.5.7/src/condynsate.egg-info/SOURCES.txt` & `condynsate-0.6.0/src/condynsate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

