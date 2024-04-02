# Comparing `tmp/scipion-em-tomotwin-3.4.tar.gz` & `tmp/scipion-em-tomotwin-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-tomotwin-3.4.tar", last modified: Thu Dec 21 15:29:19 2023, max compression
+gzip compressed data, was "scipion-em-tomotwin-3.5.tar", last modified: Tue Apr  2 14:05:19 2024, max compression
```

## Comparing `scipion-em-tomotwin-3.4.tar` & `scipion-em-tomotwin-3.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:29:19.804396 scipion-em-tomotwin-3.4/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-12-21 15:29:19.804396 scipion-em-tomotwin-3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:29:19.800397 scipion-em-tomotwin-3.4/scipion_em_tomotwin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-12-21 15:29:19.000000 scipion-em-tomotwin-3.4/scipion_em_tomotwin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-12-21 15:29:19.000000 scipion-em-tomotwin-3.4/scipion_em_tomotwin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 15:29:19.000000 scipion-em-tomotwin-3.4/scipion_em_tomotwin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-21 15:29:19.000000 scipion-em-tomotwin-3.4/scipion_em_tomotwin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-21 15:29:19.000000 scipion-em-tomotwin-3.4/scipion_em_tomotwin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-21 15:29:19.000000 scipion-em-tomotwin-3.4/scipion_em_tomotwin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-21 15:29:19.804396 scipion-em-tomotwin-3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8493 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:29:19.804396 scipion-em-tomotwin-3.4/tomotwin/
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:29:19.804396 scipion-em-tomotwin-3.4/tomotwin/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_create_masks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_picking_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_picking_cluster_umap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_picking_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:29:19.804396 scipion-em-tomotwin-3.4/tomotwin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/tests/test_protocols_tomotwin.py
--rw-r--r--   0 runner    (1001) docker     (127)   130513 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/tomotwin_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 15:29:19.804396 scipion-em-tomotwin-3.4/tomotwin/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/viewers/viewers_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/viewers/views_tkinter_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2023-12-21 15:28:55.000000 scipion-em-tomotwin-3.4/tomotwin/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:05:19.691259 scipion-em-tomotwin-3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-02 14:05:19.691259 scipion-em-tomotwin-3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:05:19.687259 scipion-em-tomotwin-3.5/scipion_em_tomotwin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-02 14:05:19.000000 scipion-em-tomotwin-3.5/scipion_em_tomotwin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 14:05:19.000000 scipion-em-tomotwin-3.5/scipion_em_tomotwin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:05:19.000000 scipion-em-tomotwin-3.5/scipion_em_tomotwin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 14:05:19.000000 scipion-em-tomotwin-3.5/scipion_em_tomotwin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 14:05:19.000000 scipion-em-tomotwin-3.5/scipion_em_tomotwin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 14:05:19.000000 scipion-em-tomotwin-3.5/scipion_em_tomotwin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:05:19.691259 scipion-em-tomotwin-3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:05:19.691259 scipion-em-tomotwin-3.5/tomotwin/
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:05:19.691259 scipion-em-tomotwin-3.5/tomotwin/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13913 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_create_masks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_picking_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_picking_cluster_umap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_picking_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:05:19.691259 scipion-em-tomotwin-3.5/tomotwin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/tests/test_protocols_tomotwin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130513 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/tomotwin_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:05:19.691259 scipion-em-tomotwin-3.5/tomotwin/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/viewers/viewers_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/viewers/views_tkinter_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-02 14:04:53.000000 scipion-em-tomotwin-3.5/tomotwin/wizards.py
```

### Comparing `scipion-em-tomotwin-3.4/CHANGES.txt` & `scipion-em-tomotwin-3.5/CHANGES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+3.5:
+    - add v0.9.0b1
+    - change test data to tomotwin tutorial
+    - use 2 GPUs by default
 3.4: add v0.8.0
 3.3:
     - fix napari viewer args
     - add v0.6.1, v0.7.0
     - add new model
     - update create mask protocol
 3.2:
```

### Comparing `scipion-em-tomotwin-3.4/LICENSE` & `scipion-em-tomotwin-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/PKG-INFO` & `scipion-em-tomotwin-3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-tomotwin
-Version: 3.4
+Version: 3.5
 Summary: Plugin to use TomoTwin within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomotwin
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomotwin/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomotwin/
@@ -67,15 +67,15 @@
         -----------------------
         *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
         PATH (not recommended), which can lead to execution problems mixing scipion
         python with conda ones. One example of this could can be seen below but
         depending on your conda version and shell you will need something different:
         CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
         
-        *TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.8.0):
+        *TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.9.0b1):
         Command to activate the TomoTwin environment. Tomotwin uses cuda-11.8, so you might want to activate specific CUDA libs via e.g. `TOMOTWIN_ENV_ACTIVATION = . /etc/profile.d/lmod.sh && module load cuda/11.8 && conda activate tomotwin-0.8.0`
         
         *TOMOTWIN_MODEL* (default = software/em/tomotwin_model-092023/tomotwin_model_p120_092023_loss.pth):
         Path to the pre-trained model.
         
         *NAPARI_ENV_ACTIVATION* (default = conda activate napari-0.4.17):
         Command to activate the Napari viewer environment.
@@ -86,15 +86,15 @@
         
         * ``scipion tests tomotwin.tests.test_protocols_tomotwin.TestTomoTwinRefBased``
         * ``scipion tests tomotwin.tests.test_protocols_tomotwin.TestTomoTwinClusterBased``
         
         Supported versions
         ------------------
         
-        0.6.1, 0.7.0, 0.8.0
+        0.7.0, 0.8.0, 0.9.0b1
         
         Protocols
         ----------
         
         * clustering-based picking (step 1)
         * clustering-based picking (step 2)
         * create tomo masks
```

### Comparing `scipion-em-tomotwin-3.4/README.rst` & `scipion-em-tomotwin-3.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 -----------------------
 *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
 PATH (not recommended), which can lead to execution problems mixing scipion
 python with conda ones. One example of this could can be seen below but
 depending on your conda version and shell you will need something different:
 CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
 
-*TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.8.0):
+*TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.9.0b1):
 Command to activate the TomoTwin environment. Tomotwin uses cuda-11.8, so you might want to activate specific CUDA libs via e.g. `TOMOTWIN_ENV_ACTIVATION = . /etc/profile.d/lmod.sh && module load cuda/11.8 && conda activate tomotwin-0.8.0`
 
 *TOMOTWIN_MODEL* (default = software/em/tomotwin_model-092023/tomotwin_model_p120_092023_loss.pth):
 Path to the pre-trained model.
 
 *NAPARI_ENV_ACTIVATION* (default = conda activate napari-0.4.17):
 Command to activate the Napari viewer environment.
@@ -76,15 +76,15 @@
 
 * ``scipion tests tomotwin.tests.test_protocols_tomotwin.TestTomoTwinRefBased``
 * ``scipion tests tomotwin.tests.test_protocols_tomotwin.TestTomoTwinClusterBased``
 
 Supported versions
 ------------------
 
-0.6.1, 0.7.0, 0.8.0
+0.7.0, 0.8.0, 0.9.0b1
 
 Protocols
 ----------
 
 * clustering-based picking (step 1)
 * clustering-based picking (step 2)
 * create tomo masks
```

### Comparing `scipion-em-tomotwin-3.4/scipion_em_tomotwin.egg-info/PKG-INFO` & `scipion-em-tomotwin-3.5/scipion_em_tomotwin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-tomotwin
-Version: 3.4
+Version: 3.5
 Summary: Plugin to use TomoTwin within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-tomotwin
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-tomotwin/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-tomotwin/
@@ -67,15 +67,15 @@
         -----------------------
         *CONDA_ACTIVATION_CMD*: If undefined, it will rely on conda command being in the
         PATH (not recommended), which can lead to execution problems mixing scipion
         python with conda ones. One example of this could can be seen below but
         depending on your conda version and shell you will need something different:
         CONDA_ACTIVATION_CMD = eval "$(/extra/miniconda3/bin/conda shell.bash hook)"
         
-        *TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.8.0):
+        *TOMOTWIN_ENV_ACTIVATION* (default = conda activate tomotwin-0.9.0b1):
         Command to activate the TomoTwin environment. Tomotwin uses cuda-11.8, so you might want to activate specific CUDA libs via e.g. `TOMOTWIN_ENV_ACTIVATION = . /etc/profile.d/lmod.sh && module load cuda/11.8 && conda activate tomotwin-0.8.0`
         
         *TOMOTWIN_MODEL* (default = software/em/tomotwin_model-092023/tomotwin_model_p120_092023_loss.pth):
         Path to the pre-trained model.
         
         *NAPARI_ENV_ACTIVATION* (default = conda activate napari-0.4.17):
         Command to activate the Napari viewer environment.
@@ -86,15 +86,15 @@
         
         * ``scipion tests tomotwin.tests.test_protocols_tomotwin.TestTomoTwinRefBased``
         * ``scipion tests tomotwin.tests.test_protocols_tomotwin.TestTomoTwinClusterBased``
         
         Supported versions
         ------------------
         
-        0.6.1, 0.7.0, 0.8.0
+        0.7.0, 0.8.0, 0.9.0b1
         
         Protocols
         ----------
         
         * clustering-based picking (step 1)
         * clustering-based picking (step 2)
         * create tomo masks
```

### Comparing `scipion-em-tomotwin-3.4/scipion_em_tomotwin.egg-info/SOURCES.txt` & `scipion-em-tomotwin-3.5/scipion_em_tomotwin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/setup.py` & `scipion-em-tomotwin-3.5/setup.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/__init__.py` & `scipion-em-tomotwin-3.5/tomotwin/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import pwem
 import pyworkflow.utils as pwutils
 from pyworkflow import Config
 
 from .constants import *
 
 
-__version__ = '3.4'
+__version__ = '3.5'
 _references = ['Rice2022']
 _logo = "tomotwin_logo.png"
 
 
 class Plugin(pwem.Plugin):
     _pathVars = [TOMOTWIN_MODEL]
     _url = "https://github.com/scipion-em/scipion-em-tomotwin"
@@ -94,23 +94,24 @@
                                       getModelName(ver))],
                            neededProgs=["wget"],
                            default=ver == DEFAULT_MODEL)
 
     @classmethod
     def addTomoTwinPackage(cls, env, version, default=False):
         ENV_NAME = getTomoTwinEnvName(version)
-        git_version = f"v{version}" if version in ['0.6.1', '0.8.0'] else version
+        git_version = f"v{version}" if version != "0.7.0" else version
         installCmds = [
             f"cd .. && rmdir tomotwin-{version} &&",
-            f"git clone -b {git_version} https://github.com/MPI-Dortmund/tomotwin-cryoet.git {ENV_NAME} &&",
+            f"git clone https://github.com/MPI-Dortmund/tomotwin-cryoet.git {ENV_NAME} &&",
             f"cd {ENV_NAME} && {cls.getCondaActivationCmd()}",
+            f"git checkout {git_version} &&",
             f"conda create -y -n {ENV_NAME} -c nvidia -c pytorch -c rapidsai -c conda-forge",
             "'pytorch>=2.1' torchvision 'pandas<2' scipy numpy matplotlib",
-            "pytables cuML=23.04 cudatoolkit=11.8 'protobuf>3.20'",
-            "tensorboard optuna mysql-connector-python &&",
+            "pytables cuml=23.10 cuda-version=11.8 'protobuf>3.20'",
+            "tensorboard optuna mysql-connector-python pytorch-metric-learning &&",
             f"conda activate {ENV_NAME} &&",
             "pip install -e .",
         ]
 
         tomotwinCmds = [(" ".join(installCmds), "setup.py")]
 
         envPath = os.environ.get('PATH', "")
```

### Comparing `scipion-em-tomotwin-3.4/tomotwin/bibtex.py` & `scipion-em-tomotwin-3.5/tomotwin/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/constants.py` & `scipion-em-tomotwin-3.5/tomotwin/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     return f"tomotwin-{version}"
 
 
 def getModelName(version):
     return f"tomotwin_model_p120_{version}_loss.pth"
 
 
-VERSIONS = ['0.6.1', '0.7.0', '0.8.0']
+VERSIONS = ['0.7.0', '0.8.0', '0.9.0b1']
 TOMOTWIN_DEFAULT_VER_NUM = VERSIONS[-1]
 
 DEFAULT_ENV_NAME = getTomoTwinEnvName(TOMOTWIN_DEFAULT_VER_NUM)
 DEFAULT_ACTIVATION_CMD = 'conda activate ' + DEFAULT_ENV_NAME
 TOMOTWIN_ENV_ACTIVATION = 'TOMOTWIN_ENV_ACTIVATION'
 
 # Model vars
```

### Comparing `scipion-em-tomotwin-3.4/tomotwin/convert.py` & `scipion-em-tomotwin-3.5/tomotwin/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/protocols/__init__.py` & `scipion-em-tomotwin-3.5/tomotwin/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_base.py` & `scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             'output_tloc': self._getExtraPath("%(tomoId)s/locate/located.tloc")
         })
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineInputParams(self, form):
         form.addSection(label='Input')
         form.addHidden(params.GPU_LIST, params.StringParam,
-                       default='0', help="Choose GPU IDs")
+                       default='0,1', help="Choose GPU IDs")
         form.addParam('inputTomos', params.PointerParam,
                       pointerClass='SetOfTomograms',
                       label="Input tomograms", important=True,
                       help='Specify tomograms containing reference-like '
                            'particles to be extracted. It is recommended '
                            'to rescale tomograms to 10 A/px in advance. '
                            'Tomograms should be without denoising or '
@@ -73,17 +73,17 @@
                           label='Reference volumes', important=True,
                           help='Specify a set of 3D volumes. They *must have '
                                'the same pixel size as tomograms and 37 px dimensions*.')
 
         form.addParam('inputMasks', params.PointerParam,
                       pointerClass='SetOfTomoMasks',
                       label='Input masks', allowsNull=True,
-                      help='With TomoTwin >=0.5, the embedding command supports the '
-                           'use of masks. With masks you can define which regions '
-                           'of your tomogram get actually embedded and therefore '
+                      help='The embedding command supports the use of masks. '
+                           'With masks you can define which regions of your '
+                           'tomogram get actually embedded and therefore '
                            'speedup the embedding.')
 
     def _defineEmbedParams(self, form):
         form.addSection(label="Embedding params")
         line = form.addLine("Batch size for embedding",
                             help="To have your tomograms embedded as quick "
                                  "as possible, you should choose a batch size that "
```

### Comparing `scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_create_masks.py` & `scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_create_masks.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,30 +48,29 @@
         ProtCreateMask3D.__init__(self, **kwargs)
         self.stepsExecutionMode = params.STEPS_PARALLEL
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addHidden(params.GPU_LIST, params.StringParam,
-                       default='0', help="Choose GPU IDs")
+                       default='0,1', help="Choose GPU IDs")
         form.addParam('inputTomos', params.PointerParam,
                       pointerClass='SetOfTomograms',
                       label="Input tomograms", important=True,
                       help='It is recommended to rescale tomograms to '
                            '10 A/px in advance. Tomograms should be '
                            'without denoising or lowpass filtering.')
 
-        if Plugin.versionGE("0.7.0"):
-            form.addParam('roiEstimate', params.EnumParam,
-                          choices=['median', 'intensity'],
-                          default=0,
-                          display=params.EnumParam.DISPLAY_HLIST,
-                          label='ROI estimation based on:',
-                          help='Estimate potential ROIs based on median '
-                               'embedding (default) or intensity values.')
+        form.addParam('roiEstimate', params.EnumParam,
+                      choices=['median', 'intensity'],
+                      default=0,
+                      display=params.EnumParam.DISPLAY_HLIST,
+                      label='ROI estimation based on:',
+                      help='Estimate potential ROIs based on median '
+                           'embedding (default) or intensity values.')
 
         form.addParallelSection(threads=1)
 
     # --------------------------- INSERT steps functions ----------------------
     def _insertAllSteps(self):
         convertStepId = self._insertFunctionStep(self.convertInputStep)
         deps = []
@@ -91,26 +90,21 @@
         for tomo in self.inputTomos.get():
             inputFn = tomo.getFileName()
             tomoFn = self._getTmpPath(tomo.getTsId() + ".mrc")
             convertToMrc(inputFn, tomoFn)
 
     def createMaskStep(self, tomoId):
         """ Create mask for each tomo. """
-        args = ["embedding_mask"]
-
-        if Plugin.versionGE("0.7.0"):
-            args.extend([
-                f"{self.getEnumText('roiEstimate')}",
-                f"-m {Plugin.getVar(TOMOTWIN_MODEL)}"
-            ])
-
-        args.extend([
+        args = [
+            "embedding_mask",
+            self.getEnumText('roiEstimate'),
             f"-i {tomoId}.mrc",
+            f"-m {Plugin.getVar(TOMOTWIN_MODEL)}",
             "-o ../extra/"
-        ])
+        ]
 
         self.runJob(self.getProgram("tomotwin_tools.py"), " ".join(args),
                     env=Plugin.getEnviron(),
                     cwd=self._getTmpPath())
 
     def createOutputStep(self):
         inTomos = self.inputTomos.get()
```

### Comparing `scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_picking_cluster.py` & `scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_picking_cluster.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_picking_cluster_umap.py` & `scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_picking_cluster_umap.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/protocols/protocol_picking_ref.py` & `scipion-em-tomotwin-3.5/tomotwin/protocols/protocol_picking_ref.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/protocols.conf` & `scipion-em-tomotwin-3.5/tomotwin/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/tests/__init__.py` & `scipion-em-tomotwin-3.5/tomotwin/viewers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# -*- coding: utf-8 -*-
 # **************************************************************************
 # *
-# * Authors:     Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk)
+# * Authors:     David Herreros Calero (dherreros@cnb.csic.es)
 # *
-# * MRC Laboratory of Molecular Biology (MRC-LMB)
+# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -19,7 +20,9 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+
+from .viewers_data import NapariBoxManager
```

### Comparing `scipion-em-tomotwin-3.4/tomotwin/tests/test_protocols_tomotwin.py` & `scipion-em-tomotwin-3.5/tomotwin/tests/test_protocols_tomotwin.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,35 +35,36 @@
                          ProtTomoTwinClusterCreateUmaps)
 
 
 class TestTomoTwinBase(BaseTest):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
-        cls.dataset = DataSet.getDataSet("emd_10439")
-        cls.tomo = cls.dataset.getFile('tomoEmd10439')
-        cls.subtomos = cls.dataset.getFile('subtomograms/emd_10439-01*.mrc')
+        cls.dataset = DataSet.getDataSet("tomotwin")
+        cls.tomo = cls.dataset.getFile('tomo')
+        cls.subtomos = cls.dataset.getFile('reference')
 
     def runImportTomos(self):
         print(magentaStr("\n==> Importing data - tomograms:"))
         protImportTomo = self.newProtocol(ProtImportTomograms,
                                           filesPath=self.tomo,
-                                          samplingRate=10)
+                                          samplingRate=13.60)
         self.launchProtocol(protImportTomo)
         self.assertIsNotNone(protImportTomo.Tomograms,
                              msg="There was a problem with tomogram import")
 
         return protImportTomo
 
     def runImportVolumes(self):
         print(magentaStr("\n==> Importing data - volumes:"))
         protImportVols = self.newProtocol(ProtImportVolumes,
-                                          filesPath=self.subtomos, samplingRate=10)
+                                          filesPath=self.subtomos,
+                                          samplingRate=13.60)
         self.launchProtocol(protImportVols)
-        self.assertIsNotNone(protImportVols.outputVolumes,
+        self.assertIsNotNone(protImportVols.outputVolume,
                              "There was a problem with volumes import")
 
         return protImportVols
 
 
 class TestTomoTwinRefBased(TestTomoTwinBase):
     def test_run(self):
@@ -76,32 +77,37 @@
         self.launchProtocol(protCreateMasks)
         self.assertIsNotNone(protCreateMasks.outputMasks,
                              "Tomo mask creation has failed")
 
         print(magentaStr("\n==> Testing tomotwin - reference-based picking:"))
         protPicking = self.newProtocol(ProtTomoTwinRefPicking,
                                        inputTomos=protImportTomo.Tomograms,
-                                       inputRefs=protImportVols.outputVolumes,
+                                       inputRefs=protImportVols.outputVolume,
                                        inputMasks=protCreateMasks.outputMasks,
-                                       batchTomos=128,
-                                       batchRefs=12,
-                                       boxSize=44,
-                                       zMin=200, zMax=204)
+                                       batchTomos=400,
+                                       batchRefs=12)
         self.launchProtocol(protPicking)
         outputCoords = protPicking.output3DCoordinates
         self.assertIsNotNone(outputCoords, "Tomotwin reference-based picking has failed")
-        self.assertAlmostEqual(outputCoords.getSize(), 2250, delta=100)
-        self.assertEqual(outputCoords.getBoxSize(), 44)
+        self.assertAlmostEqual(outputCoords.getSize(), 976, delta=100)
+        self.assertEqual(outputCoords.getBoxSize(), 37)
 
 
 class TestTomoTwinClusterBased(TestTomoTwinBase):
     def test_run(self):
         protImportTomo = self.runImportTomos()
 
+        print(magentaStr("\n==> Testing tomotwin - create tomo masks:"))
+        protCreateMasks = self.newProtocol(ProtTomoTwinCreateMasks,
+                                           inputTomos=protImportTomo.Tomograms)
+        self.launchProtocol(protCreateMasks)
+        self.assertIsNotNone(protCreateMasks.outputMasks,
+                             "Tomo mask creation has failed")
+
         print(magentaStr("\n==> Testing tomotwin - clustering-based picking (step 1):"))
         protPicking = self.newProtocol(ProtTomoTwinClusterCreateUmaps,
                                        inputTomos=protImportTomo.Tomograms,
-                                       batchTomos=128,
-                                       zMin=200, zMax=204)
+                                       inputMasks=protCreateMasks.outputMasks,
+                                       batchTomos=400)
         self.launchProtocol(protPicking)
         self.assertTrue(protPicking.isFinished(),
                         "Tomotwin cluster-based embedding has failed")
```

### Comparing `scipion-em-tomotwin-3.4/tomotwin/tomotwin_logo.png` & `scipion-em-tomotwin-3.5/tomotwin/tomotwin_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/viewers/__init__.py` & `scipion-em-tomotwin-3.5/tomotwin/tests/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# -*- coding: utf-8 -*-
 # **************************************************************************
 # *
-# * Authors:     David Herreros Calero (dherreros@cnb.csic.es)
+# * Authors:     Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk)
 # *
-# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
+# * MRC Laboratory of Molecular Biology (MRC-LMB)
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -21,8 +20,15 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-from .viewers_data import NapariBoxManager
+from pyworkflow.tests import DataSet
+
+DataSet(name='tomotwin',
+        folder='tomotwin',
+        files={
+            'tomo': 'tomo.mrc',
+            'reference': 'reference_0.mrc'
+        })
```

### Comparing `scipion-em-tomotwin-3.4/tomotwin/viewers/viewers_data.py` & `scipion-em-tomotwin-3.5/tomotwin/viewers/viewers_data.py`

 * *Files identical despite different names*

### Comparing `scipion-em-tomotwin-3.4/tomotwin/viewers/views_tkinter_tree.py` & `scipion-em-tomotwin-3.5/tomotwin/viewers/views_tkinter_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,8 +65,9 @@
             proc = threading.Thread(target=self.launchNapari,
                                     args=(tomo_path, tloc_fn,))
             proc.start()
 
     def launchNapari(self, tomoFn, tlocFn):
         from tomotwin import Plugin, NAPARI_BOXMANAGER
         args = f"{tomoFn} {tlocFn}"
-        Plugin.runNapariBoxManager(self.prot.getProject().getPath(), NAPARI_BOXMANAGER, args)
+        Plugin.runNapariBoxManager(self.prot.getProject().getPath(),
+                                   NAPARI_BOXMANAGER, args)
```

### Comparing `scipion-em-tomotwin-3.4/tomotwin/wizards.py` & `scipion-em-tomotwin-3.5/tomotwin/wizards.py`

 * *Files identical despite different names*

