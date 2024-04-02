# Comparing `tmp/periodicity_detection-0.1.1.tar.gz` & `tmp/periodicity_detection-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/periodicity_detection-0.1.1.tar", last modified: Thu Aug 24 12:10:19 2023, max compression
+gzip compressed data, was "dist/periodicity_detection-0.1.2.tar", last modified: Tue Apr  2 08:41:31 2024, max compression
```

## Comparing `periodicity_detection-0.1.1.tar` & `periodicity_detection-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (999)     1079 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       18 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     5639 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     4667 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection/
--rw-r--r--   0 runner    (1001) docker     (999)     3697 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6556 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)       27 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection/methods/
--rw-r--r--   0 runner    (1001) docker     (999)      302 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1347 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/methods/autocorrelation.py
--rw-r--r--   0 runner    (1001) docker     (999)    17872 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/methods/autoperiod.py
--rw-r--r--   0 runner    (1001) docker     (999)     1447 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/methods/fft.py
--rw-r--r--   0 runner    (1001) docker     (999)     1699 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/methods/find_length.py
--rw-r--r--   0 runner    (1001) docker     (999)    10761 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/methods/findfrequency.py
--rw-r--r--   0 runner    (1001) docker     (999)     2746 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/methods/number_peaks.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/periodicity_detection/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     5639 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      812 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       67 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)      294 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       22 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/periodicity_detection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      801 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-24 12:10:19.000000 periodicity_detection-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     4870 2023-08-24 12:09:49.000000 periodicity_detection-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/methods/autocorrelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/methods/autoperiod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/methods/fft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/methods/find_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10761 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/methods/findfrequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/methods/number_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/periodicity_detection/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/periodicity_detection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:41:31.000000 periodicity_detection-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-02 08:41:15.000000 periodicity_detection-0.1.2/setup.py
```

### Comparing `periodicity_detection-0.1.1/LICENSE` & `periodicity_detection-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/PKG-INFO` & `periodicity_detection-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodicity_detection
-Version: 0.1.1
+Version: 0.1.2
 Summary: Detect the dominant period in univariate, equidistant time series data.
 Home-page: https://github.com/CodeLionX/periodicity_detection
 Author: Sebastian Schmidl
 Author-email: sebastian.schmidl@hpi.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -50,14 +50,17 @@
 - Fast Fourier Transform (FFT)
 - `find_length`
 - Python-adaption of the R package `forecast`'s `findfrequency` function
 - Number of Peaks-method
 
 📖 Periodicity Detection's documentation is hosted at https://periodicity-detection.readthedocs.io.
 
+Recommended reading: [Window Size Selection In Unsupervised Time Series Analytics: A Review and Benchmark](https://project.inria.fr/aaltd22/files/2022/08/AALTD22_paper_3876.pdf):
+Workshop paper that compares the _Autocorrelation_, _FFT_ (_DFT_ in the paper), and _AutoPeriod_ methods to three other methods ([Code](https://github.com/ermshaua/window-size-selection)).
+
 # Installation
 
 You can install Periodicity Detection as a package or from source.
 
 ## Prerequisites
 
 - python >= 3.7, <= 3.11
```

### Comparing `periodicity_detection-0.1.1/README.md` & `periodicity_detection-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 - Fast Fourier Transform (FFT)
 - `find_length`
 - Python-adaption of the R package `forecast`'s `findfrequency` function
 - Number of Peaks-method
 
 📖 Periodicity Detection's documentation is hosted at https://periodicity-detection.readthedocs.io.
 
+Recommended reading: [Window Size Selection In Unsupervised Time Series Analytics: A Review and Benchmark](https://project.inria.fr/aaltd22/files/2022/08/AALTD22_paper_3876.pdf):
+Workshop paper that compares the _Autocorrelation_, _FFT_ (_DFT_ in the paper), and _AutoPeriod_ methods to three other methods ([Code](https://github.com/ermshaua/window-size-selection)).
+
 # Installation
 
 You can install Periodicity Detection as a package or from source.
 
 ## Prerequisites
 
 - python >= 3.7, <= 3.11
```

### Comparing `periodicity_detection-0.1.1/periodicity_detection/__init__.py` & `periodicity_detection-0.1.2/periodicity_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/periodicity_detection/__main__.py` & `periodicity_detection-0.1.2/periodicity_detection/__main__.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/periodicity_detection/methods/autocorrelation.py` & `periodicity_detection-0.1.2/periodicity_detection/methods/autocorrelation.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/periodicity_detection/methods/autoperiod.py` & `periodicity_detection-0.1.2/periodicity_detection/methods/autoperiod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import sys
 import warnings
-from typing import Any, List, Tuple, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import statsmodels.tsa.stattools
 from matplotlib.patches import Rectangle
 from scipy.optimize import minimize_scalar
 from scipy.signal import periodogram
@@ -263,23 +263,35 @@
         # print("frequency:", f)  # between 0 and 0.5
         # print("period:", N/k)
 
         self._print(
             f"inspecting periodogram between 2 and {N // 2} (frequencies 0 and 0.5)",
             level=2,
         )
-        period_hints = []
+        period_candidates: Dict[int, Tuple[int, float, float]] = {}
+        removed_hints = 0
         for i in np.arange(2, N // 2):
             if p_den[i] > p_threshold:
-                period_hints.append((k[i], f[i], p_den[i]))
-                self._print(
-                    f"detected hint at bin k={k[i]} (f={f[i]:.4f}, "
-                    f"power={p_den[i]:.2f})",
-                    level=3,
-                )
+                period = N // k[i]
+                if period not in period_candidates:
+                    period_candidates[period] = (k[i], f[i], p_den[i])
+                    self._print(
+                        f"detected hint at bin k={k[i]} (f={f[i]:.4f}, "
+                        f"power={p_den[i]:.2f})",
+                        level=3,
+                    )
+                else:
+                    removed_hints += 1
+                    self._print(
+                        f"detected hint at bin k={k[i]} (f={f[i]:.4f}, "
+                        f"power={p_den[i]:.2f}) - skipped due to duplicated "
+                        f"period ({period})",
+                        level=3,
+                    )
+        period_hints = list(period_candidates.values())
 
         # start with the highest power frequency:
         self._print("sorting hints by highest power first", level=2)
         period_hints = sorted(period_hints, key=lambda x: x[-1], reverse=True)
 
         if self._plot:
             plt.figure()
@@ -388,15 +400,17 @@
                 self._print(
                     f"insufficient steepness ({np.abs(slope[0].slope):.4f} and "
                     f"{np.abs(slope[1].slope):.4f}) --> INVALID",
                     level=3,
                 )
 
             elif lslope > 0 > rslope:
-                self._print("hill detected --> VALID", level=3)
+                self._print(
+                    f"hill detected (steepness={steepness:.4f}) --> VALID", level=3
+                )
                 period = begin + np.argmax(acf[begin : end + 1])
                 self._print(f"corrected period (from {N // k}): {period}", level=3)
                 ranges.append((begin, end, optimal_t, period, slope))
                 if self._return_multi <= 1:
                     break
 
             else:
@@ -405,20 +419,20 @@
         warnings.filterwarnings(
             action="default",
             category=RuntimeWarning,
             message=r".*invalid value encountered.*",
         )
 
         if self._plot:
-            n_plots = 3 if self._detrend and self._trend else 2
+            n_plots = 3 if self._detrend and self._trend is not None else 2
             fig, axs = plt.subplots(n_plots, 1, sharex="col")
             axs[0].set_title("Original time series")
             axs[0].set_xlabel("time")
 
-            if self._trend and self._orig_data:
+            if self._trend is not None and self._orig_data is not None:
                 axs[0].plot(self._orig_data, label="time series", color="blue")
                 axs[0].plot(self._trend, label="linear trend", color="black")
                 axs[1].set_title("Detrended time series")
                 axs[1].plot(data, label="time series", color="black")
                 axs[1].set_xlabel("time")
             else:
                 axs[0].plot(data, label="time series", color="black")
```

### Comparing `periodicity_detection-0.1.1/periodicity_detection/methods/fft.py` & `periodicity_detection-0.1.2/periodicity_detection/methods/fft.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/periodicity_detection/methods/find_length.py` & `periodicity_detection-0.1.2/periodicity_detection/methods/find_length.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/periodicity_detection/methods/findfrequency.py` & `periodicity_detection-0.1.2/periodicity_detection/methods/findfrequency.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/periodicity_detection/methods/number_peaks.py` & `periodicity_detection-0.1.2/periodicity_detection/methods/number_peaks.py`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/periodicity_detection.egg-info/PKG-INFO` & `periodicity_detection-0.1.2/periodicity_detection.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: periodicity-detection
-Version: 0.1.1
+Version: 0.1.2
 Summary: Detect the dominant period in univariate, equidistant time series data.
 Home-page: https://github.com/CodeLionX/periodicity_detection
 Author: Sebastian Schmidl
 Author-email: sebastian.schmidl@hpi.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -50,14 +50,17 @@
 - Fast Fourier Transform (FFT)
 - `find_length`
 - Python-adaption of the R package `forecast`'s `findfrequency` function
 - Number of Peaks-method
 
 📖 Periodicity Detection's documentation is hosted at https://periodicity-detection.readthedocs.io.
 
+Recommended reading: [Window Size Selection In Unsupervised Time Series Analytics: A Review and Benchmark](https://project.inria.fr/aaltd22/files/2022/08/AALTD22_paper_3876.pdf):
+Workshop paper that compares the _Autocorrelation_, _FFT_ (_DFT_ in the paper), and _AutoPeriod_ methods to three other methods ([Code](https://github.com/ermshaua/window-size-selection)).
+
 # Installation
 
 You can install Periodicity Detection as a package or from source.
 
 ## Prerequisites
 
 - python >= 3.7, <= 3.11
```

### Comparing `periodicity_detection-0.1.1/periodicity_detection.egg-info/SOURCES.txt` & `periodicity_detection-0.1.2/periodicity_detection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/pyproject.toml` & `periodicity_detection-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `periodicity_detection-0.1.1/setup.py` & `periodicity_detection-0.1.2/setup.py`

 * *Files identical despite different names*

