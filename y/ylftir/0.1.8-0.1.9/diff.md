# Comparing `tmp/ylftir-0.1.8.tar.gz` & `tmp/ylftir-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ylftir-0.1.8.tar", last modified: Fri Mar 29 07:11:54 2024, max compression
+gzip compressed data, was "ylftir-0.1.9.tar", last modified: Tue Apr  2 22:45:06 2024, max compression
```

## Comparing `ylftir-0.1.8.tar` & `ylftir-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 07:11:54.555153 ylftir-0.1.8/
--rw-rw-rw-   0        0        0       36 2024-01-05 08:06:39.000000 ylftir-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0      347 2024-03-29 07:11:54.555153 ylftir-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-02-28 23:41:39.000000 ylftir-0.1.8/README.md
--rw-rw-rw-   0        0        0      101 2024-02-28 23:51:54.000000 ylftir-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       92 2024-03-29 07:11:54.559710 ylftir-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      587 2024-02-28 23:39:07.000000 ylftir-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-29 07:11:54.491662 ylftir-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 07:11:54.526449 ylftir-0.1.8/src/ylftir/
--rw-rw-rw-   0        0        0       48 2024-03-29 07:11:41.000000 ylftir-0.1.8/src/ylftir/__init__.py
--rw-rw-rw-   0        0        0    12767 2024-03-29 07:11:35.000000 ylftir-0.1.8/src/ylftir/ylftir.py
-drwxrwxrwx   0        0        0        0 2024-03-29 07:11:54.553248 ylftir-0.1.8/src/ylftir.egg-info/
--rw-rw-rw-   0        0        0      347 2024-03-29 07:11:54.000000 ylftir-0.1.8/src/ylftir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-03-29 07:11:54.000000 ylftir-0.1.8/src/ylftir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 07:11:54.000000 ylftir-0.1.8/src/ylftir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2024-03-29 07:11:54.000000 ylftir-0.1.8/src/ylftir.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-29 07:11:54.000000 ylftir-0.1.8/src/ylftir.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 22:45:06.083325 ylftir-0.1.9/
+-rw-rw-rw-   0        0        0       36 2024-01-05 08:06:39.000000 ylftir-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      347 2024-04-02 22:45:06.083325 ylftir-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-02-28 23:41:39.000000 ylftir-0.1.9/README.md
+-rw-rw-rw-   0        0        0      101 2024-02-28 23:51:54.000000 ylftir-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       92 2024-04-02 22:45:06.089108 ylftir-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      587 2024-02-28 23:39:07.000000 ylftir-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:45:05.949643 ylftir-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 22:45:06.022037 ylftir-0.1.9/src/ylftir/
+-rw-rw-rw-   0        0        0       48 2024-04-02 22:44:56.000000 ylftir-0.1.9/src/ylftir/__init__.py
+-rw-rw-rw-   0        0        0    17614 2024-04-02 22:43:51.000000 ylftir-0.1.9/src/ylftir/ylftir.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:45:06.083325 ylftir-0.1.9/src/ylftir.egg-info/
+-rw-rw-rw-   0        0        0      347 2024-04-02 22:45:05.000000 ylftir-0.1.9/src/ylftir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-04-02 22:45:05.000000 ylftir-0.1.9/src/ylftir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 22:45:05.000000 ylftir-0.1.9/src/ylftir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-04-02 22:45:05.000000 ylftir-0.1.9/src/ylftir.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 22:45:05.000000 ylftir-0.1.9/src/ylftir.egg-info/top_level.txt
```

### Comparing `ylftir-0.1.8/setup.py` & `ylftir-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ylftir-0.1.8/src/ylftir/ylftir.py` & `ylftir-0.1.9/src/ylftir/ylftir.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import requests
 from scipy.signal import argrelextrema, savgol_filter
+from scipy.special import erf
 from scipy import interpolate
 from scipy.optimize import curve_fit
 import csv
 import numbers
 
 def import_data_url(url, guess=False):
   '''
@@ -66,15 +67,15 @@
           x, y = np.transpose(np.genfromtxt(file, delimiter=','))
         else:
           print(f'Error: Unrecognized filetype')
 
       if x is None or y is None:
         print(f'Error: Unable to parse data from {file}')
         return None, None
-      
+
       # sort y w.r.t. x
       # NOTE: if files are guaranteed to be in order (or reverse order) with respect to wavenumber, this is unnecessary
       x_ind = np.argsort(x)
       x, y = x[x_ind], y[x_ind]
       return x, y
 
 def normalize_data(x, y):
@@ -91,46 +92,75 @@
 
 def gaussian(x, position, amplitude, width):
   return amplitude * np.exp(-0.5 * ((x - position) / width) ** 2)
 
 def gaussian_area(position, amplitude, width):
   return amplitude * np.sqrt(2 * np.pi) * width
 
+def gaussian_area_cropped(position, amplitude, width, lower_bound, upper_bound):
+  return amplitude * width * np.sqrt(np.pi / 2) * (erf((position - lower_bound)/(width * np.sqrt(2))) - erf((position - upper_bound)/(width * np.sqrt(2))))
+
 def gaussian_fwhm(position, amplitude, width):
   ''' length of FWHM '''
   return 4 * width * np.sqrt(-np.log(0.5))
 
 class Optim_Gaussian:
   def __init__(self):
     pass
-  
+
   def __call__(self, x, *args):
     '''
     args should be in the form position, position, ..., amplitude, amplitude, ..., width, width, ... etc.
     '''
     positions, amplitudes, widths = np.array(args).reshape(3, -1)
     return sum([gaussian(x, positions[i], amplitudes[i], widths[i]) for i in range(len(positions))])
 
 def lorentzian(x, position, amplitude, width):
   return (amplitude * width**2) / (np.power(x - position, 2) + width**2)
 
 def lorentzian_area(position, amplitude, width):
   return amplitude * np.pi * width
 
+def lorentzian_area_cropped(position, amplitude, width, lower_bound, upper_bound):
+  return amplitude * width * (np.arctan((position - lower_bound)/width) - np.arctan((position - upper_bound)/width))
+
 class Optim_Lorentzian:
   def __init__(self):
     pass
 
   def __call__(self, x, *args):
     '''
     args should be in the form position, position, ..., amplitude, amplitude, ..., width, width, ... etc.
     '''
     positions, amplitudes, widths = np.array(args).reshape(3, -1)
     return sum([lorentzian(x, positions[i], amplitudes[i], widths[i]) for i in range(len(positions))])
 
+class Optim_Problem:
+  def __init__(self, types):
+    '''
+    types is a list of strings `'gaussian'` for gaussian peaks and `'lorentzian'` for lorentzian peaks
+    '''
+    self.types = types
+  
+  def __call__(self, x, *args):
+    '''
+    args should be in the form position, position, ..., amplitude, amplitude, ..., width, width, ... etc.
+    '''
+    positions, amplitudes, widths = np.array(args).reshape(3, -1)
+    
+    inter = np.zeros_like(x)
+    for i, t in enumerate(self.types):
+      if t == 'gaussian':
+        inter += gaussian(x, positions[i], amplitudes[i], widths[i])
+      elif t == 'lorentzian':
+        inter += lorentzian(x, positions[i], amplitudes[i], widths[i])
+      else:
+        raise Exception(f'Unrecognized peak type at i={i}: {t}')
+    return inter
+
 def linear_baseline_correction(x, y):
   slope = (y[-1] - y[0]) / (x[-1] - x[0])
   baseline = y[0] + slope * (x - x[0])
   return y - baseline, baseline
 
 def nearest(x, y, x0):
   idx = (np.abs(x-x0)).argmin()
@@ -251,15 +281,15 @@
     nodes_x=None, nodes_y=None,
     peak_window_size=35, smoothing_size=20
     ):
   '''
   Computes full deconvolution of input data given deconvolution parameters
   `x` - wavenumbers, sorted
   `y` - absorbance
-  `fit_func` - `'gaussian'` or `'lorentzian'`; the fitting function used. defaults to `'gaussian'`
+  `fit_func` - `'gaussian'` or `'lorentzian'`; the fitting function used. defaults to `'gaussian'`. alternatively, for each peak, provide a type
   `baseline` - `'nodal'`, `'linear'`, or `'cubic'`; baseline correction used. defaults to `'linear'`
   `peak_finder` - `'first_derivative'` or `'second_derivative'`; the method for finding peaks if `n` and `positions` is not provided
   `positions` - list of positions for each peak
   `vary_positions` - percentage by which to constrain the varying of positions as a decimal
   `constrain_width` - tuple of lower and upper bounds for width, defaults to (0, np.inf); to provide bounds for each peak, provide a tuple for each bound i.e. ((0, 0, 0), (np.inf, 1, 2))
   `constrain_amplitude` - tuple of lower and upper bounds for amplitude, defaults to (0, np.inf); to provide bounds for each peak, provide a tuple for each bound i.e. ((0, 0, 0), (np.inf, 1, 2))
   `nodes` - list of wavenumbers in x to consider as nodes for nodal baseline correction
@@ -286,67 +316,147 @@
     print(f'Using {n} peaks at {positions}')
   else:
     n = len(positions)
 
   # rescale so numerically feasible
   scale_x = np.max(x) - np.min(x)
   positions = positions / scale_x
-  
+
   # constraints
   pos_lb = [(1 - vary_positions) * pos for pos in positions]
   pos_ub = [(1 + vary_positions) * pos for pos in positions]
-  
+
   bw, tw = constrain_width
   ba, ta = constrain_amplitude
   if isinstance(bw, numbers.Number):
     bw = [bw] * n
   if isinstance(tw, numbers.Number):
     tw = [tw] * n
   if isinstance(ba, numbers.Number):
     ba = [ba] * n
   if isinstance(ta, numbers.Number):
     ta = [ta] * n
-  
+
   # rescale constraints
   bw = [bw[i] / scale_x for i in range(n)]
   tw = [tw[i] / scale_x for i in range(n)]
-  
+
   # problem
   if fit_func == 'gaussian':
     problem = Optim_Gaussian()
   elif fit_func == 'lorentzian':
     problem = Optim_Lorentzian()
   else:
-    print('Error: unrecognized fit function')
-    return None, None
-  
+    try:
+      _ = iter(fit_func)
+      problem = Optim_Problem(fit_func)
+    except:
+      raise Exception(f'Unrecognized fit function {fit_func}')
+      return None, None
+
   # setup and solve optimization problems
   init = [*positions, *[0.9*min(1, ta[i]) for i in range(n)], *[0.9*min(0.1, tw[i]) for i in range(n)]]
 
   solution, cov = curve_fit(problem, x / scale_x, y, init, maxfev=100000, bounds=([*pos_lb, *ba, *bw],[*pos_ub, *ta, *tw]))
 
   # return problem solution as numpy array of parameters
   positions, amplitudes, widths = np.array(solution).reshape(3, -1)
   widths *= scale_x
   positions *= scale_x
 
   return np.array([positions, amplitudes, widths]), residual
 
 def simulated_gaussians(x, gaussians):
   '''
-  Returns the sum of input gaussians along input x
+  Returns the sum of input gaussians along input x, and individual peaks
   `x` - wavenumbers, sorted
   `gaussians` - list in shape (3,N) where N is the number of gaussians, in the form [positions, amplitudes, widths]
   '''
   positions, amplitudes, widths = gaussians
   res = np.array([gaussian(x, positions[i], amplitudes[i], widths[i]) for i in range(len(positions))])
   return np.sum(res, axis=0), res
 
 def simulated_lorentzians(x, lorentzians):
   '''
-  Returns the sum of input lorentzians along input x
+  Returns the sum of input lorentzians along input x, and individual peaks
   `x` - wavenumbers, sorted
   `lorentzians` - list in shape (3,N) where N is the number of lorentzians, in the form [positions, amplitudes, widths]
   '''
   positions, amplitudes, widths = lorentzians
   res = np.array([lorentzian(x, positions[i], amplitudes[i], widths[i]) for i in range(len(positions))])
   return np.sum(res, axis=0), res
+
+def simulated(x, peaks, types):
+  '''
+  Returns the sum of input peaks along input x, and individual peaks
+  `x` - wavenumbers, sorted
+  `peaks` - list in shape (3,N) where N is the number of peaks, in the form [positions, amplitudes, widths]
+  `types` - either `'gaussian'`, `'lorentzian'`, or a list of these, one for each peak
+  '''
+  if types == 'gaussian':
+    return simulated_gaussians(x, peaks)
+  elif types == 'lorentzian':
+    return simulated_lorentzians(x, peaks)
+
+  positions, amplitudes, widths = peaks
+  res = np.zeros((len(types), len(x)))
+  for i, t in enumerate(types):
+    if t == 'gaussian':
+      res[i] = gaussian(x, positions[i], amplitudes[i], widths[i])
+    elif t == 'lorentzian':
+      res[i] = lorentzian(x, positions[i], amplitudes[i], widths[i])
+    else:
+      raise Exception(f'Unrecognized peak type at i={i}: {t}')
+  return np.sum(res, axis=0), res
+
+def get_areas(peaks, types):
+  '''
+  Get peak areas
+  `peaks` - list in shape (3,N) where N is the number of peaks, in the form [positions, amplitudes, widths]
+  `types` - either `'gaussian'`, `'lorentzian'`, or a list of these, one for each peak
+  '''
+  positions, amplitudes, widths = peaks
+
+  if types == 'gaussian':
+    return np.array([gaussian_area(positions[i], amplitudes[i], widths[i]) for i in range(len(positions))])
+  if types == 'lorentzian':
+    return np.array([lorentzian_area(positions[i], amplitudes[i], widths[i]) for i in range(len(positions))])
+  
+  areas = []
+  for i, t in enumerate(types):
+    if t == 'gaussian':
+      areas.append(gaussian_area(positions[i], amplitudes[i], widths[i]))
+    elif t == 'lorentzian':
+      areas.append(lorentzian_area(positions[i], amplitudes[i], widths[i]))
+    else:
+      raise Exception(f'Unrecognized peak type at i={i}: {t}')
+  return np.array(areas)
+
+def get_areas_cropped(peaks, types, crop_range):
+  '''
+  Get cropped peak areas
+  `peaks` - list in shape (3,N) where N is the number of peaks, in the form [positions, amplitudes, widths]
+  `types` - either `'gaussian'`, `'lorentzian'`, or a list of these, one for each peak
+  `crop_range` - tuple in the form `(lower_bounds, upper_bounds)` where `lower_bounds` and `upper_bounds` is either a number or a tuple corresponding to each peak
+  '''
+  positions, amplitudes, widths = peaks
+
+  lower_bounds, upper_bounds = crop_range
+  if isinstance(lower_bounds, numbers.Number):
+    lower_bounds = [lower_bounds] * len(positions)
+  if isinstance(upper_bounds, numbers.Number):
+    upper_bounds = [upper_bounds] * len(positions)
+
+  if types == 'gaussian':
+    return np.array([gaussian_area_cropped(positions[i], amplitudes[i], widths[i], lower_bounds[i], upper_bounds[i]) for i in range(len(positions))])
+  if types == 'lorentzian':
+    return np.array([lorentzian_area_cropped(positions[i], amplitudes[i], widths[i], lower_bounds[i], upper_bounds[i]) for i in range(len(positions))])
+  
+  areas = []
+  for i, t in enumerate(types):
+    if t == 'gaussian':
+      areas.append(gaussian_area_cropped(positions[i], amplitudes[i], widths[i], lower_bounds[i], upper_bounds[i]))
+    elif t == 'lorentzian':
+      areas.append(lorentzian_area_cropped(positions[i], amplitudes[i], widths[i], lower_bounds[i], upper_bounds[i]))
+    else:
+      raise Exception(f'Unrecognized peak type at i={i}: {t}')
+  return np.array(areas)
```

