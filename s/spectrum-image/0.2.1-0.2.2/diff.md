# Comparing `tmp/spectrum_image-0.2.1.tar.gz` & `tmp/spectrum_image-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_image-0.2.1.tar", last modified: Mon Apr  1 16:55:30 2024, max compression
+gzip compressed data, was "spectrum_image-0.2.2.tar", last modified: Tue Apr  2 20:19:10 2024, max compression
```

## Comparing `spectrum_image-0.2.1.tar` & `spectrum_image-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-01 16:55:30.615615 spectrum_image-0.2.1/
--rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.2.1/LICENSE
--rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-01 16:55:30.615414 spectrum_image-0.2.1/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      977 2024-03-18 03:44:13.000000 spectrum_image-0.2.1/README.md
--rw-r--r--   0 sung       (501) staff       (20)      864 2024-04-01 16:55:11.000000 spectrum_image-0.2.1/pyproject.toml
--rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-01 16:55:30.615653 spectrum_image-0.2.1/setup.cfg
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-01 16:55:30.612489 spectrum_image-0.2.1/src/
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-01 16:55:30.614435 spectrum_image-0.2.1/src/spectrum_image/
--rw-r--r--   0 sung       (501) staff       (20)    34207 2024-04-01 16:51:54.000000 spectrum_image-0.2.1/src/spectrum_image/SI.py
--rw-r--r--   0 sung       (501) staff       (20)    69473 2024-03-30 23:57:52.000000 spectrum_image-0.2.1/src/spectrum_image/SI_bckup.py
--rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.2.1/src/spectrum_image/SI_lineshapes.py
--rw-r--r--   0 sung       (501) staff       (20)     7848 2024-03-25 18:18:26.000000 spectrum_image-0.2.1/src/spectrum_image/SI_util.py
--rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.2.1/src/spectrum_image/__init__.py
-drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-01 16:55:30.615208 spectrum_image-0.2.1/src/spectrum_image.egg-info/
--rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/PKG-INFO
--rw-r--r--   0 sung       (501) staff       (20)      394 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/SOURCES.txt
--rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/dependency_links.txt
--rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/requires.txt
--rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-01 16:55:30.000000 spectrum_image-0.2.1/src/spectrum_image.egg-info/top_level.txt
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-02 20:19:10.998503 spectrum_image-0.2.2/
+-rw-r--r--   0 sung       (501) staff       (20)    35149 2024-03-12 18:53:01.000000 spectrum_image-0.2.2/LICENSE
+-rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-02 20:19:10.998308 spectrum_image-0.2.2/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      977 2024-03-18 03:44:13.000000 spectrum_image-0.2.2/README.md
+-rw-r--r--   0 sung       (501) staff       (20)      864 2024-04-02 20:18:57.000000 spectrum_image-0.2.2/pyproject.toml
+-rw-r--r--   0 sung       (501) staff       (20)       38 2024-04-02 20:19:10.998540 spectrum_image-0.2.2/setup.cfg
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-02 20:19:10.994705 spectrum_image-0.2.2/src/
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-02 20:19:10.997400 spectrum_image-0.2.2/src/spectrum_image/
+-rw-r--r--   0 sung       (501) staff       (20)    22598 2024-04-02 20:15:16.000000 spectrum_image-0.2.2/src/spectrum_image/SI.py
+-rw-r--r--   0 sung       (501) staff       (20)    69473 2024-03-30 23:57:52.000000 spectrum_image-0.2.2/src/spectrum_image/SI_bckup.py
+-rw-r--r--   0 sung       (501) staff       (20)     1466 2024-03-26 23:43:32.000000 spectrum_image-0.2.2/src/spectrum_image/SI_lineshapes.py
+-rw-r--r--   0 sung       (501) staff       (20)     7796 2024-04-02 17:57:16.000000 spectrum_image-0.2.2/src/spectrum_image/SI_util.py
+-rw-r--r--   0 sung       (501) staff       (20)      280 2024-03-12 18:53:01.000000 spectrum_image-0.2.2/src/spectrum_image/__init__.py
+-rw-r--r--   0 sung       (501) staff       (20)    11571 2024-04-02 20:08:45.000000 spectrum_image-0.2.2/src/spectrum_image/eels_bgsub.py
+drwxr-xr-x   0 sung       (501) staff       (20)        0 2024-04-02 20:19:10.998092 spectrum_image-0.2.2/src/spectrum_image.egg-info/
+-rw-r--r--   0 sung       (501) staff       (20)     1781 2024-04-02 20:19:10.000000 spectrum_image-0.2.2/src/spectrum_image.egg-info/PKG-INFO
+-rw-r--r--   0 sung       (501) staff       (20)      427 2024-04-02 20:19:10.000000 spectrum_image-0.2.2/src/spectrum_image.egg-info/SOURCES.txt
+-rw-r--r--   0 sung       (501) staff       (20)        1 2024-04-02 20:19:10.000000 spectrum_image-0.2.2/src/spectrum_image.egg-info/dependency_links.txt
+-rw-r--r--   0 sung       (501) staff       (20)       52 2024-04-02 20:19:10.000000 spectrum_image-0.2.2/src/spectrum_image.egg-info/requires.txt
+-rw-r--r--   0 sung       (501) staff       (20)       15 2024-04-02 20:19:10.000000 spectrum_image-0.2.2/src/spectrum_image.egg-info/top_level.txt
```

### Comparing `spectrum_image-0.2.1/LICENSE` & `spectrum_image-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.1/PKG-INFO` & `spectrum_image-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum_image
 Project-URL: Repository, https://github.com/sukhsung/spectrum_image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum_image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spectrum_image-0.2.1/README.md` & `spectrum_image-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.1/pyproject.toml` & `spectrum_image-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spectrum_image"
-version = "0.2.1"
+version = "0.2.2"
 dependencies = [
   "numpy",
   "matplotlib",
   "jupyterlab",
   "ipympl",
   "scipy",
   "tqdm",
```

### Comparing `spectrum_image-0.2.1/src/spectrum_image/SI_bckup.py` & `spectrum_image-0.2.2/src/spectrum_image/SI_bckup.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.1/src/spectrum_image/SI_lineshapes.py` & `spectrum_image-0.2.2/src/spectrum_image/SI_lineshapes.py`

 * *Files identical despite different names*

### Comparing `spectrum_image-0.2.1/src/spectrum_image/SI_util.py` & `spectrum_image-0.2.2/src/spectrum_image/SI_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import matplotlib.pyplot as plt
 import numpy as np
-import copy
-from scipy.optimize import curve_fit
 from scipy.ndimage import affine_transform
-from sklearn.decomposition import PCA
 from tqdm import tqdm, tqdm_notebook
 import spectrum_image.SI_lineshapes as ls
 
-from lmfit import Parameters, Minimizer
+
+from sklearn.decomposition import PCA
+from tqdm import tqdm, tqdm_notebook
+
 
 def remove_outlier( si, threshold_multiplier=5, remove_nn=True):
     # remove outliers that are larger than threshold_multiplier*std + median of each spectrum
     # remove_nn also remove two nearest neighbor pixels
     # Outliers are replaced by medians
     (ny,nx,ne) = si.shape
     si_cleaned = si.copy()
@@ -99,16 +99,14 @@
     if angle == 0:
         return img
     a = np.tan( angle*np.pi/180 )
     shear_matrix_ADF = [[1, a],[0, 1]]
     img_shear =affine_transform(img, shear_matrix_ADF, order=1)
     return img_shear
     
-
-
 def fit_zeroloss_si( si, es, pk_func=ls.gaussian, e_bound=(-10,10), d_func=ls.d_gaussian, ftol = 1e-5 ):
     (ny, nx, ne) = si.shape
 
     e_bound_ind = ( np.argmin( np.abs( es-e_bound[0] )),np.argmin( np.abs( es-e_bound[1] )) )
 
     e_fit = es[  e_bound_ind[0]:e_bound_ind[1] ]
     si_fit = si[ :,:, e_bound_ind[0]:e_bound_ind[1] ].copy()
@@ -161,15 +159,14 @@
             
             pbar.update(1)
     pbar.close()
 
 
     return A0s, e0s, sgs
 
-
 def shift_zeroloss_SI( si, es, shifts ):
     (ny, nx, ne) = si.shape
     si_shifted = si.copy()
 
     dispersion = es[1]-es[0]
     shifts_ind = shifts/dispersion
 
@@ -241,8 +238,8 @@
     pca = PCA(n_components=n_components).fit(data)
     components = pca.transform(data)
     filtered = pca.inverse_transform(components).T
     si_pca = np.reshape(filtered, (ny,nx,ne))
 
     si_pca = si_pca*data_range + data_min
 
-    return si_pca, components
+    return si_pca, components
```

### Comparing `spectrum_image-0.2.1/src/spectrum_image.egg-info/PKG-INFO` & `spectrum_image-0.2.2/src/spectrum_image.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrum_image
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Package for EELS (Electron Energy Loss Spectroscopy) Analysis
 Author-email: Suk Hyun Sung <sukhsung@umich.edu>
 Project-URL: Homepage, https://github.com/sukhsung/spectrum_image
 Project-URL: Repository, https://github.com/sukhsung/spectrum_image
 Project-URL: Bug Tracker, https://github.com/sukhsung/spectrum_image/issues
 Keywords: Electron Microscopy,EELS,TEM,STEM,Electron Energy Loss Spectroscopy
 Classifier: Development Status :: 3 - Alpha
```

