# Comparing `tmp/subradar-1.1.3.tar.gz` & `tmp/subradar-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subradar-1.1.3.tar", last modified: Thu Mar  7 15:02:24 2024, max compression
+gzip compressed data, was "subradar-1.1.4.tar", last modified: Tue Apr  2 16:30:38 2024, max compression
```

## Comparing `subradar-1.1.3.tar` & `subradar-1.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-03-07 15:02:24.733894 subradar-1.1.3/
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     1102 2024-01-25 21:22:47.000000 subradar-1.1.3/LICENSE.md
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     1151 2024-03-07 15:02:24.732895 subradar-1.1.3/PKG-INFO
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)      689 2024-01-25 21:22:47.000000 subradar-1.1.3/README.md
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)       38 2024-03-07 15:02:24.733894 subradar-1.1.3/setup.cfg
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     1205 2024-01-25 21:22:47.000000 subradar-1.1.3/setup.py
-drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-03-07 15:02:24.732895 subradar-1.1.3/subradar/
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     2418 2024-01-25 21:22:47.000000 subradar-1.1.3/subradar/Classdef.py
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)      745 2024-03-07 14:59:36.000000 subradar-1.1.3/subradar/__init__.py
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)      976 2024-01-25 21:22:47.000000 subradar-1.1.3/subradar/filtering.py
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     7040 2024-01-25 21:22:47.000000 subradar-1.1.3/subradar/fractal.py
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     6137 2024-01-25 21:22:47.000000 subradar-1.1.3/subradar/iem.py
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     3830 2024-01-25 21:22:47.000000 subradar-1.1.3/subradar/invert.py
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)      391 2024-01-25 21:22:47.000000 subradar-1.1.3/subradar/roughness.py
-drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-03-07 15:02:24.732895 subradar-1.1.3/subradar/simulation/
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)      101 2024-01-25 21:22:47.000000 subradar-1.1.3/subradar/simulation/__init__.py
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)    10213 2024-03-07 14:52:09.000000 subradar-1.1.3/subradar/simulation/trento.py
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     7394 2024-01-25 21:22:47.000000 subradar-1.1.3/subradar/surface.py
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     4987 2024-01-25 21:22:47.000000 subradar-1.1.3/subradar/utils.py
-drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-03-07 15:02:24.732895 subradar-1.1.3/subradar.egg-info/
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)     1151 2024-03-07 15:02:24.000000 subradar-1.1.3/subradar.egg-info/PKG-INFO
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)      453 2024-03-07 15:02:24.000000 subradar-1.1.3/subradar.egg-info/SOURCES.txt
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)        1 2024-03-07 15:02:24.000000 subradar-1.1.3/subradar.egg-info/dependency_links.txt
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)       73 2024-03-07 15:02:24.000000 subradar-1.1.3/subradar.egg-info/requires.txt
--rw-r--r--   0 cgrima    (1000) cgrima    (1000)        9 2024-03-07 15:02:24.000000 subradar-1.1.3/subradar.egg-info/top_level.txt
-drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-03-07 15:02:24.732895 subradar-1.1.3/tests/
--rwxr-xr-x   0 cgrima    (1000) cgrima    (1000)     5627 2024-01-25 21:22:47.000000 subradar-1.1.3/tests/test_subradar1.py
+drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-04-02 16:30:38.781779 subradar-1.1.4/
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     1102 2024-01-25 21:22:47.000000 subradar-1.1.4/LICENSE.md
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     1003 2024-04-02 16:30:38.781779 subradar-1.1.4/PKG-INFO
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)      689 2024-01-25 21:22:47.000000 subradar-1.1.4/README.md
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)       38 2024-04-02 16:30:38.781779 subradar-1.1.4/setup.cfg
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     1205 2024-01-25 21:22:47.000000 subradar-1.1.4/setup.py
+drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-04-02 16:30:38.781779 subradar-1.1.4/subradar/
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     2418 2024-01-25 21:22:47.000000 subradar-1.1.4/subradar/Classdef.py
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)      745 2024-04-02 15:52:24.000000 subradar-1.1.4/subradar/__init__.py
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)      976 2024-01-25 21:22:47.000000 subradar-1.1.4/subradar/filtering.py
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     7029 2024-04-02 16:03:50.000000 subradar-1.1.4/subradar/fractal.py
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     6137 2024-01-25 21:22:47.000000 subradar-1.1.4/subradar/iem.py
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     3830 2024-01-25 21:22:47.000000 subradar-1.1.4/subradar/invert.py
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)      391 2024-01-25 21:22:47.000000 subradar-1.1.4/subradar/roughness.py
+drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-04-02 16:30:38.781779 subradar-1.1.4/subradar/simulation/
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)      101 2024-01-25 21:22:47.000000 subradar-1.1.4/subradar/simulation/__init__.py
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)    10230 2024-03-26 21:34:20.000000 subradar-1.1.4/subradar/simulation/trento.py
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     7394 2024-01-25 21:22:47.000000 subradar-1.1.4/subradar/surface.py
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     4987 2024-01-25 21:22:47.000000 subradar-1.1.4/subradar/utils.py
+drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-04-02 16:30:38.781779 subradar-1.1.4/subradar.egg-info/
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)     1003 2024-04-02 16:30:38.000000 subradar-1.1.4/subradar.egg-info/PKG-INFO
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)      453 2024-04-02 16:30:38.000000 subradar-1.1.4/subradar.egg-info/SOURCES.txt
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)        1 2024-04-02 16:30:38.000000 subradar-1.1.4/subradar.egg-info/dependency_links.txt
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)       73 2024-04-02 16:30:38.000000 subradar-1.1.4/subradar.egg-info/requires.txt
+-rw-r--r--   0 cgrima    (1000) cgrima    (1000)        9 2024-04-02 16:30:38.000000 subradar-1.1.4/subradar.egg-info/top_level.txt
+drwxr-xr-x   0 cgrima    (1000) cgrima    (1000)        0 2024-04-02 16:30:38.781779 subradar-1.1.4/tests/
+-rwxr-xr-x   0 cgrima    (1000) cgrima    (1000)     5627 2024-01-25 21:22:47.000000 subradar-1.1.4/tests/test_subradar1.py
```

### Comparing `subradar-1.1.3/LICENSE.md` & `subradar-1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `subradar-1.1.3/README.md` & `subradar-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `subradar-1.1.3/setup.py` & `subradar-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `subradar-1.1.3/subradar/Classdef.py` & `subradar-1.1.4/subradar/Classdef.py`

 * *Files identical despite different names*

### Comparing `subradar-1.1.3/subradar/__init__.py` & `subradar-1.1.4/subradar/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 theta, th : angle
 T : Transmission coefficient
 wf : Wave frequency
 wk : Wave number
 wl : Wavelength
 """
 
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 __author__ = "Cyril Grima"
 
 __all__ = ["iem", "invert", "roughness", "surface", "utils", "filtering", "simulation", "fractal"]
 
 from . import iem, invert, roughness, surface, utils, filtering, simulation, fractal
```

### Comparing `subradar-1.1.3/subradar/filtering.py` & `subradar-1.1.4/subradar/filtering.py`

 * *Files identical despite different names*

### Comparing `subradar-1.1.3/subradar/fractal.py` & `subradar-1.1.4/subradar/fractal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import rsr
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from scipy import signal 
 from scipy import fft
 import scipy.constants as ct
 from scipy import integrate
```

### Comparing `subradar-1.1.3/subradar/iem.py` & `subradar-1.1.4/subradar/iem.py`

 * *Files identical despite different names*

### Comparing `subradar-1.1.3/subradar/invert.py` & `subradar-1.1.4/subradar/invert.py`

 * *Files identical despite different names*

### Comparing `subradar-1.1.3/subradar/simulation/trento.py` & `subradar-1.1.4/subradar/simulation/trento.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import numpy as np
 import scipy
 import glob
-import rsr
+#import rsr
 import matplotlib.pyplot as plt
 import h5py
 import hdf5storage
 from .. import filtering, surface
 
 
 class Results:
@@ -286,26 +286,26 @@
         
         # Spatial Coordinates
         coord = self.xy()
         
         return {'y':ys, 'val':val, 'coord':coord}
         
         
-    def surface_rsr(self, fit_model='hk', lim=None, **kwargs):
-        """RSR
-        """
-        if 'compression' in kwargs:
-            compression = kwargs['compression']
-        else:
-            compression = None
+#    def surface_rsr(self, fit_model='hk', lim=None, **kwargs):
+#        """RSR
+#        """
+#        if 'compression' in kwargs:
+#            compression = kwargs['compression']
+#        else:
+#            compression = None
             
-        srf = self.surface(compression=compression, absolute=True)
-        amp = np.array(srf['val'])
+#        srf = self.surface(compression=compression, absolute=True)
+#        amp = np.array(srf['val'])
         
-        if lim:
-            y = srf['coord'][1]
-            idx = [i for i, val in enumerate(y) if (val > lim[0]) and (val < lim[1])]
-            amp2 = [amp[i] for i in idx]
-            amp = np.array(amp2)
+#        if lim:
+#            y = srf['coord'][1]
+#            idx = [i for i, val in enumerate(y) if (val > lim[0]) and (val < lim[1])]
+#            amp2 = [amp[i] for i in idx]
+#            amp = np.array(amp2)
             
-        f = rsr.run.processor(amp, fit_model=fit_model)
-        return f
+#        f = rsr.run.processor(amp, fit_model=fit_model)
+#        return f
```

### Comparing `subradar-1.1.3/subradar/surface.py` & `subradar-1.1.4/subradar/surface.py`

 * *Files identical despite different names*

### Comparing `subradar-1.1.3/subradar/utils.py` & `subradar-1.1.4/subradar/utils.py`

 * *Files identical despite different names*

### Comparing `subradar-1.1.3/tests/test_subradar1.py` & `subradar-1.1.4/tests/test_subradar1.py`

 * *Files identical despite different names*

