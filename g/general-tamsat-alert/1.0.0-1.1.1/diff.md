# Comparing `tmp/general_tamsat_alert-1.0.0.tar.gz` & `tmp/general_tamsat_alert-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_tamsat_alert-1.0.0.tar", last modified: Sun Feb 18 17:51:49 2024, max compression
+gzip compressed data, was "general_tamsat_alert-1.1.1.tar", last modified: Tue Apr  2 15:23:03 2024, max compression
```

## Comparing `general_tamsat_alert-1.0.0.tar` & `general_tamsat_alert-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-02-18 17:51:49.936228 general_tamsat_alert-1.0.0/
--rw-r--r--   0 john      (1001) john      (1001)      761 2024-02-18 17:51:49.936228 general_tamsat_alert-1.0.0/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)      448 2024-02-18 17:35:53.000000 general_tamsat_alert-1.0.0/README.md
--rw-rw-r--   0 john      (1001) john      (1001)      536 2024-02-18 17:22:01.000000 general_tamsat_alert-1.0.0/pyproject.toml
--rw-rw-r--   0 john      (1001) john      (1001)       38 2024-02-18 17:51:49.936228 general_tamsat_alert-1.0.0/setup.cfg
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-02-18 17:51:49.936228 general_tamsat_alert-1.0.0/src/
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-02-18 17:51:49.936228 general_tamsat_alert-1.0.0/src/general_tamsat_alert/
--rw-rw-r--   0 john      (1001) john      (1001)      179 2023-12-29 14:08:34.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert/__init__.py
--rw-rw-r--   0 john      (1001) john      (1001)     5760 2023-12-29 14:10:03.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert/ensembles.py
--rw-rw-r--   0 john      (1001) john      (1001)     4842 2023-12-29 13:21:49.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert/periodicity.py
--rw-rw-r--   0 john      (1001) john      (1001)     1915 2023-12-29 14:10:03.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert/roc_auc.py
--rw-rw-r--   0 john      (1001) john      (1001)     3629 2023-09-09 16:55:53.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert/weighting_functions.py
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-02-18 17:51:49.936228 general_tamsat_alert-1.0.0/src/general_tamsat_alert.egg-info/
--rw-r--r--   0 john      (1001) john      (1001)      761 2024-02-18 17:51:49.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)      512 2024-02-18 17:51:49.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1001) john      (1001)        1 2024-02-18 17:51:49.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1001) john      (1001)       27 2024-02-18 17:51:49.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert.egg-info/requires.txt
--rw-rw-r--   0 john      (1001) john      (1001)       21 2024-02-18 17:51:49.000000 general_tamsat_alert-1.0.0/src/general_tamsat_alert.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-02-18 17:51:49.936228 general_tamsat_alert-1.0.0/tests/
--rw-rw-r--   0 john      (1001) john      (1001)        0 2023-12-29 18:10:31.000000 general_tamsat_alert-1.0.0/tests/test_ensembles.py
--rw-rw-r--   0 john      (1001) john      (1001)     1764 2023-12-29 19:04:08.000000 general_tamsat_alert-1.0.0/tests/test_periodicity.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/
+-rw-r--r--   0 john      (1001) john      (1001)      761 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)      448 2024-02-18 17:35:53.000000 general_tamsat_alert-1.1.1/README.md
+-rw-rw-r--   0 john      (1001) john      (1001)      536 2024-04-02 15:22:54.000000 general_tamsat_alert-1.1.1/pyproject.toml
+-rw-rw-r--   0 john      (1001) john      (1001)       38 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/setup.cfg
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/src/
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/src/general_tamsat_alert/
+-rw-rw-r--   0 john      (1001) john      (1001)     2904 2024-04-02 15:14:12.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/__init__.py
+-rw-rw-r--   0 john      (1001) john      (1001)     5898 2024-04-02 15:14:12.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/ensembles.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3269 2024-04-02 15:01:21.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/misc.py
+-rw-rw-r--   0 john      (1001) john      (1001)     4842 2023-12-29 13:21:49.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/periodicity.py
+-rw-rw-r--   0 john      (1001) john      (1001)     1881 2024-04-02 15:14:12.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/roc_auc.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3652 2024-04-02 15:06:02.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/weighting_functions.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/
+-rw-r--r--   0 john      (1001) john      (1001)      761 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)      545 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1001) john      (1001)        1 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1001) john      (1001)       27 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/requires.txt
+-rw-rw-r--   0 john      (1001) john      (1001)       21 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/tests/
+-rw-rw-r--   0 john      (1001) john      (1001)        0 2023-12-29 18:10:31.000000 general_tamsat_alert-1.1.1/tests/test_ensembles.py
+-rw-rw-r--   0 john      (1001) john      (1001)     1764 2023-12-29 19:04:08.000000 general_tamsat_alert-1.1.1/tests/test_periodicity.py
```

### Comparing `general_tamsat_alert-1.0.0/PKG-INFO` & `general_tamsat_alert-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general_tamsat_alert
-Version: 1.0.0
+Version: 1.1.1
 Author-email: John Ellis <12johnellis@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: scipy
```

### Comparing `general_tamsat_alert-1.0.0/pyproject.toml` & `general_tamsat_alert-1.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "general_tamsat_alert"
-version = "1.0.0"
+version = "1.1.1"
 dependencies = [
     "numpy",
     "xarray",
     "scipy",
     "fastroc",
 ]
 authors = [
```

### Comparing `general_tamsat_alert-1.0.0/src/general_tamsat_alert/ensembles.py` & `general_tamsat_alert-1.1.1/src/general_tamsat_alert/ensembles.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import xarray as xr
-import general_tamsat_alert.weighting_functions as wfs
 import numpy as np
 from typing import List, Tuple, Hashable
 
+from . import weighting_functions as wfs
+
+
 def get_ensembles(
-    da: xr.DataArray,
-    period: int,
-    ensemble_length: int,
-    initiation_index: int,
-    look_back: int = 0,
-    wf: wfs.WeightingFunctionType = wfs.no_weights,
-    time_label: str = "time",
+        da: xr.DataArray,
+        period: int,
+        ensemble_length: int,
+        initiation_index: int,
+        look_back: int = 0,
+        wf: wfs.WeightingFunctionType = wfs.no_weights,
+        time_label: str = "time",
+        do_increments: int = 1
 ) -> Tuple[xr.DataArray, xr.DataArray]:
     """Get an ensemble of the data in the data array.
 
     Given the most significant period of the data (usually annual),
     the index of the initiation date and the length of the ensemble in
     indices.
 
     The lookback is the number of indices of observation data required
 
+    TODO: Document inputs
+
+    :param do_increments:
     :param da:
     :param period:
     :param ensemble_length:
     :param initiation_index:
     :param look_back:
     :param wf:
     :param time_label:
@@ -52,19 +58,22 @@
 
     weight_data = np.empty([len(i) for i in coords])
     weights = xr.DataArray(weight_data, coords=coords, dims=dims, name="weights",)
     for index, start_time in enumerate(start_times):
         ensembles[look_back:, ..., index] = da.isel(
             {time_label: slice(start_time, start_time + ensemble_length)}
         ).values
-        weights[..., index] = wf(start_time, 1)
-    ensembles[...] -= ensembles[look_back, ...]
-    ensembles[...] += da.isel({time_label: initiation_index})
-    ensembles[:look_back, ...] = da.isel(
-        {time_label: slice(initiation_index - look_back, initiation_index)}
+        weights[..., index] = wf(start_time)
+
+    if do_increments == 1:
+        ensembles[...] -= ensembles[look_back, ...]
+        ensembles[...] += da.isel({time_label: initiation_index})
+
+    ensembles[:look_back+1, ...] = da.isel(
+        {time_label: slice(initiation_index - look_back, initiation_index+1)}
     ).values[..., np.newaxis]
 
     return ensembles, weights
 
 
 def get_ensemble_indices(
     da: xr.DataArray,
```

### Comparing `general_tamsat_alert-1.0.0/src/general_tamsat_alert/periodicity.py` & `general_tamsat_alert-1.1.1/src/general_tamsat_alert/periodicity.py`

 * *Files identical despite different names*

### Comparing `general_tamsat_alert-1.0.0/src/general_tamsat_alert/roc_auc.py` & `general_tamsat_alert-1.1.1/src/general_tamsat_alert/roc_auc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import xarray as xr
 import fastroc
 from typing import List
 from scipy.stats import norm
 import numpy as np
 
-from general_tamsat_alert.ensembles import get_ensemble_indices, get_hindcasts_observed
-import general_tamsat_alert.weighting_functions as wfs
+from .ensembles import get_ensemble_indices, get_hindcasts_observed
+from . import weighting_functions as wfs
 
 def get_roc_auc(
     da: xr.DataArray,
     prediction_date: str,
     start_dates: List[str],
     period: int,
     threshold_value: float = 0.2,
```

### Comparing `general_tamsat_alert-1.0.0/src/general_tamsat_alert/weighting_functions.py` & `general_tamsat_alert-1.1.1/src/general_tamsat_alert/weighting_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 import numpy as np
 import xarray as xr
 from typing import Callable, Union, Sequence, Tuple, Optional
 
-WeightingFunctionType = Union[Callable[[int, float], Union[float, np.ndarray, xr.DataArray]]]
+WeightingFunctionType = Callable[[int], Union[float, np.ndarray, xr.DataArray]]
 WeightingFunctionIntermediateType = Callable[[int], WeightingFunctionType]
 WeightingFunctionBuilderType = Callable[..., WeightingFunctionIntermediateType]
 
 
-def no_weights(member_index: int, weighting_strength: float = 1.0) -> float:
+def no_weights(member_index: int) -> float:
     return 1.0
 
 
 def no_weights_intermediate(initiation_index: int) -> WeightingFunctionType:
     return no_weights
 
 
-def no_weights_builder() -> WeightingFunctionIntermediateType:
+def no_weights_builder(weighting_strength: float = 1.0) -> WeightingFunctionIntermediateType:
     return no_weights_intermediate
 
 
-def weight_time_builder(period: int = 24) -> WeightingFunctionIntermediateType:
+def weight_time_builder(period: int = 24, weighting_strength: float = 1.0) -> WeightingFunctionIntermediateType:
     def weight_time_intermediate(initiation_index: int) -> WeightingFunctionType:
-        def weight_time(member_index: int, weighting_strength: float = 1.0) -> float:
+        def weight_time(member_index: int) -> float:
             if member_index == initiation_index:
                 return 0.0
             else:
                 return np.exp(-0.0001 * (weighting_strength * (member_index - initiation_index) * period/24) ** 2)
         return weight_time
     return weight_time_intermediate
 
 
 def weight_neighbour_error_builder(data: xr.DataArray,
                                    neighbour_shifts: Sequence[Tuple[int, int]] = ((1, 0), (0, 1), (-1, 0), (0, -1)),
                                    neighbour_weights: Optional[Sequence[Tuple[int, int]]] = None,
-                                   lat_label: str = "lat", lon_label: str = "lon") -> WeightingFunctionIntermediateType:
+                                   lat_label: str = "lat", lon_label: str = "lon",
+                                   weighting_strength: float = 1.0) -> WeightingFunctionIntermediateType:
     def weight_neighbor_error_intermediate(initiation_index: int) -> WeightingFunctionType:
         if neighbour_weights is None:
             internal_neighbour_weights = [1 / np.sqrt(x * x + y * y) for y,x in neighbour_shifts]
         else:
             internal_neighbour_weights = neighbour_weights
 
         shifts = np.arange(len(neighbour_shifts))
@@ -49,15 +50,15 @@
         error_values = np.empty((len(lat), len(lon), len(shifts)))
 
         errors = xr.DataArray(error_values, coords=[lat, lon, shifts], dims=["lat", "lon", "shift"])
         shifted_data = []
         for (y, x) in neighbour_shifts:
             shifted_data.append(data[initiation_index, :, :].shift(lat=y, lon=x).values)
 
-        def weight_neighbour_error(member_index: int, weighting_strength: float = 1.0) -> np.ndarray:
+        def weight_neighbour_error(member_index: int) -> np.ndarray:
             if member_index == initiation_index:
                 return np.zeros((len(lat), len(lon)))
 
             values = data[member_index, :, :]
             for index, (y, x) in enumerate(neighbour_shifts):
                 errors[:, :, index] = ((values.shift({lat_label: y, lon_label: x}) - shifted_data[index])**2).values
             mean = errors.weighted(weights).mean(dim="shift", skipna=True).values
@@ -65,15 +66,15 @@
             mean = 1/mean
             mean[(np.isnan(mean))] = 0
             return mean
         return weight_neighbour_error
     return weight_neighbor_error_intermediate
 
 
-def weight_value_builder(values: Sequence[float]) -> WeightingFunctionIntermediateType:
+def weight_value_builder(values: Sequence[float], weighting_strength: float = 1.0) -> WeightingFunctionIntermediateType:
     def weight_value_intermediate(initiation_index: int) -> WeightingFunctionType:
-        def weight_value(member_index: int, weighting_strength: float=1) -> float:
+        def weight_value(member_index: int) -> float:
             delta = values[member_index] - values[initiation_index]
             delta = np.abs(delta)
             return np.exp(-(weighting_strength*delta)**2)
         return weight_value
     return weight_value_intermediate
```

### Comparing `general_tamsat_alert-1.0.0/src/general_tamsat_alert.egg-info/PKG-INFO` & `general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general_tamsat_alert
-Version: 1.0.0
+Version: 1.1.1
 Author-email: John Ellis <12johnellis@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: scipy
```

### Comparing `general_tamsat_alert-1.0.0/src/general_tamsat_alert.egg-info/SOURCES.txt` & `general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 src/general_tamsat_alert/__init__.py
 src/general_tamsat_alert/ensembles.py
+src/general_tamsat_alert/misc.py
 src/general_tamsat_alert/periodicity.py
 src/general_tamsat_alert/roc_auc.py
 src/general_tamsat_alert/weighting_functions.py
 src/general_tamsat_alert.egg-info/PKG-INFO
 src/general_tamsat_alert.egg-info/SOURCES.txt
 src/general_tamsat_alert.egg-info/dependency_links.txt
 src/general_tamsat_alert.egg-info/requires.txt
```

### Comparing `general_tamsat_alert-1.0.0/tests/test_periodicity.py` & `general_tamsat_alert-1.1.1/tests/test_periodicity.py`

 * *Files identical despite different names*

