# Comparing `tmp/regularizepsf-0.2.3.tar.gz` & `tmp/regularizepsf-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regularizepsf-0.2.3.tar", last modified: Thu Nov  2 14:53:18 2023, max compression
+gzip compressed data, was "regularizepsf-0.3.1.tar", last modified: Tue Apr  2 21:02:15 2024, max compression
```

## Comparing `regularizepsf-0.2.3.tar` & `regularizepsf-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 14:53:18.093481 regularizepsf-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-11-02 14:53:18.093481 regularizepsf-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 14:53:18.089481 regularizepsf-0.2.3/regularizepsf/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/regularizepsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13386 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/regularizepsf/corrector.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/regularizepsf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24112 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/regularizepsf/fitter.py
--rw-r--r--   0 runner    (1001) docker     (127)   584237 2023-11-02 14:53:16.000000 regularizepsf-0.2.3/regularizepsf/helper.c
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/regularizepsf/helper.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     6080 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/regularizepsf/psf.py
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/regularizepsf/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 14:53:18.089481 regularizepsf-0.2.3/regularizepsf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-11-02 14:53:18.000000 regularizepsf-0.2.3/regularizepsf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-11-02 14:53:18.000000 regularizepsf-0.2.3/regularizepsf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 14:53:18.000000 regularizepsf-0.2.3/regularizepsf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-02 14:53:18.000000 regularizepsf-0.2.3/regularizepsf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-02 14:53:18.000000 regularizepsf-0.2.3/regularizepsf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-02 14:53:18.093481 regularizepsf-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 14:53:18.089481 regularizepsf-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/tests/test_corrector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9823 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/tests/test_fitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/tests/test_psf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2023-11-02 14:52:51.000000 regularizepsf-0.2.3/tests/test_visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:02:15.596476 regularizepsf-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    43114 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-02 21:02:15.596476 regularizepsf-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:02:15.596476 regularizepsf-0.3.1/regularizepsf/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/regularizepsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/regularizepsf/corrector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/regularizepsf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/regularizepsf/fitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)   584487 2024-04-02 21:02:14.000000 regularizepsf-0.3.1/regularizepsf/helper.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/regularizepsf/helper.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/regularizepsf/psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/regularizepsf/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:02:15.596476 regularizepsf-0.3.1/regularizepsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-02 21:02:15.000000 regularizepsf-0.3.1/regularizepsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-02 21:02:15.000000 regularizepsf-0.3.1/regularizepsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:02:15.000000 regularizepsf-0.3.1/regularizepsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 21:02:15.000000 regularizepsf-0.3.1/regularizepsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 21:02:15.000000 regularizepsf-0.3.1/regularizepsf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:02:15.596476 regularizepsf-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:02:15.596476 regularizepsf-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/tests/test_corrector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/tests/test_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/tests/test_psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-04-02 21:02:09.000000 regularizepsf-0.3.1/tests/test_visualize.py
```

### Comparing `regularizepsf-0.2.3/PKG-INFO` & `regularizepsf-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: regularizepsf
-Version: 0.2.3
+Version: 0.3.1
 Summary: Point spread function modeling and regularization
 Home-page: https://github.com/punch-mission/regularizepsf
 Author: J. Marcus Hughes
 Author-email: hughes.jmb@gmail.com
 License: MIT
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: dill
 Requires-Dist: h5py
 Requires-Dist: lmfit
 Requires-Dist: sep
@@ -35,27 +36,29 @@
 Below is an example of correcting model data using the package. An initial image of a simplified starfield (a) is synthetically observed with a slowly
 varying PSF (b), then regularized with this technique (c). The final image visually matches a direct convolution of
 the initial image with the target PSF (d). The panels are gamma-corrected to highlight the periphery of the model PSFs.
 ![Example result image](model_example.png)
 
 ## Getting started
 
-`pip install regularizepsf` and then follow along with the [Quickstart section](https://punch-mission.github.io/regularizepsf/quickstart.html). 
+`pip install regularizepsf` and then follow along with the [documentation](https://punch-mission.github.io/regularizepsf/concepts.html).
 
 ## Contributing
-We encourage all contributions. If you have a problem with the code or would like to see a new feature, please open an issue. Or you can submit a pull request. 
+We encourage all contributions. If you have a problem with the code or would like to see a new feature, please open an issue. Or you can submit a pull request.
+
+If you're contributing code please see [this package's development guide](https://punch-mission.github.io/regularizepsf/development.html).
 
 ## License
-See LICENSE for the MIT license
+See [LICENSE file](LICENSE)
 
 ## Need help?
-Please contact Marcus Hughes at [marcus.hughes@swri.org](mailto:marcus.hughes@swri.org).
+Please ask a question in our [discussions](https://github.com/punch-mission/regularizepsf/discussions)
 
 ## Citation
-Please cite the associated paper if you use this technique: 
+Please cite [the associated paper](https://iopscience.iop.org/article/10.3847/1538-3881/acc578) if you use this technique:
 
 ```
 @article{Hughes_2023,
 doi = {10.3847/1538-3881/acc578},
 url = {https://dx.doi.org/10.3847/1538-3881/acc578},
 year = {2023},
 month = {apr},
@@ -65,23 +68,8 @@
 pages = {204},
 author = {J. Marcus Hughes and Craig E. DeForest and Daniel B. Seaton},
 title = {Coma Off It: Regularizing Variable Point-spread Functions},
 journal = {The Astronomical Journal}
 }
 ```
 
-If you use this software, please also cite the package: 
-```
-@software{marcus_hughes_2023_8370994,
-  author       = {Marcus Hughes and
-                  Sam Van Kooten and
-                  Tania Varesano and
-                  Suman Chapai},
-  title        = {punch-mission/regularizepsf: 0.2.2},
-  month        = sep,
-  year         = 2023,
-  publisher    = {Zenodo},
-  version      = {0.2.2},
-  doi          = {10.5281/zenodo.8370994},
-  url          = {https://doi.org/10.5281/zenodo.8370994}
-}
-```
+If you use this software, please also cite the package with the specific version used. [Zenodo always has the most up-to-date citation](https://zenodo.org/records/10066960).
```

### Comparing `regularizepsf-0.2.3/README.md` & `regularizepsf-0.3.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 Below is an example of correcting model data using the package. An initial image of a simplified starfield (a) is synthetically observed with a slowly
 varying PSF (b), then regularized with this technique (c). The final image visually matches a direct convolution of
 the initial image with the target PSF (d). The panels are gamma-corrected to highlight the periphery of the model PSFs.
 ![Example result image](model_example.png)
 
 ## Getting started
 
-`pip install regularizepsf` and then follow along with the [Quickstart section](https://punch-mission.github.io/regularizepsf/quickstart.html). 
+`pip install regularizepsf` and then follow along with the [documentation](https://punch-mission.github.io/regularizepsf/concepts.html).
 
 ## Contributing
-We encourage all contributions. If you have a problem with the code or would like to see a new feature, please open an issue. Or you can submit a pull request. 
+We encourage all contributions. If you have a problem with the code or would like to see a new feature, please open an issue. Or you can submit a pull request.
+
+If you're contributing code please see [this package's development guide](https://punch-mission.github.io/regularizepsf/development.html).
 
 ## License
-See LICENSE for the MIT license
+See [LICENSE file](LICENSE)
 
 ## Need help?
-Please contact Marcus Hughes at [marcus.hughes@swri.org](mailto:marcus.hughes@swri.org).
+Please ask a question in our [discussions](https://github.com/punch-mission/regularizepsf/discussions)
 
 ## Citation
-Please cite the associated paper if you use this technique: 
+Please cite [the associated paper](https://iopscience.iop.org/article/10.3847/1538-3881/acc578) if you use this technique:
 
 ```
 @article{Hughes_2023,
 doi = {10.3847/1538-3881/acc578},
 url = {https://dx.doi.org/10.3847/1538-3881/acc578},
 year = {2023},
 month = {apr},
@@ -39,23 +41,8 @@
 pages = {204},
 author = {J. Marcus Hughes and Craig E. DeForest and Daniel B. Seaton},
 title = {Coma Off It: Regularizing Variable Point-spread Functions},
 journal = {The Astronomical Journal}
 }
 ```
 
-If you use this software, please also cite the package: 
-```
-@software{marcus_hughes_2023_8370994,
-  author       = {Marcus Hughes and
-                  Sam Van Kooten and
-                  Tania Varesano and
-                  Suman Chapai},
-  title        = {punch-mission/regularizepsf: 0.2.2},
-  month        = sep,
-  year         = 2023,
-  publisher    = {Zenodo},
-  version      = {0.2.2},
-  doi          = {10.5281/zenodo.8370994},
-  url          = {https://doi.org/10.5281/zenodo.8370994}
-}
-```
+If you use this software, please also cite the package with the specific version used. [Zenodo always has the most up-to-date citation](https://zenodo.org/records/10066960).
```

### Comparing `regularizepsf-0.2.3/regularizepsf/corrector.py` & `regularizepsf-0.3.1/regularizepsf/corrector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from __future__ import annotations
 
 import abc
+from typing import Any, Tuple, Optional
 from pathlib import Path
-from typing import Any, Tuple
 
-import dill
 import h5py
 import numpy as np
 from numpy.fft import fft2, ifft2, ifftshift
 
-from regularizepsf.exceptions import (
-    EvaluatedModelInconsistentSizeError,
-    InvalidSizeError,
-    UnevaluatedPointError,
-)
+from regularizepsf.exceptions import EvaluatedModelInconsistentSizeError, InvalidSizeError, UnevaluatedPointError
 from regularizepsf.helper import _correct_image, _precalculate_ffts
 from regularizepsf.psf import PointSpreadFunctionABC, SimplePSF, VariedPSF
 
 
 class CorrectorABC(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def save(self, path: str | Path) -> None:
@@ -54,18 +49,18 @@
         """PSF correct an image according to the model
 
         Parameters
         ----------
         image : 2D float np.ndarray
             image to be corrected
         size : int
-            how big to make the patches when correcting an image, 
+            how big to make the patches when correcting an image,
             only used for FunctionalCorrector
         alpha : float
-            controls the “hardness” of the transition from amplification 
+            controls the “hardness” of the transition from amplification
             to attenuation, see notes
         epsilon : float
             controls the maximum of the amplification, see notes
 
         Returns
         -------
         np.ndarray
@@ -87,15 +82,15 @@
             an image with the PSF applied
         """
 
 
 class FunctionalCorrector(CorrectorABC):
     """
     A version of the PSF corrector that stores the model as a set of functions.
-    For the actual correction, the functions must first 
+    For the actual correction, the functions must first
     be evaluated to an ArrayCorrector.
     """
     def __init__(self, psf: PointSpreadFunctionABC,
                  target_model: SimplePSF | None) -> None:
         """Initialize a FunctionalCorrector
 
         Parameters
@@ -111,22 +106,22 @@
 
     @property
     def is_variable(self) -> bool:
         """
         Returns
         -------
         bool
-            True if the PSF model is varied (changes across the field-of-view) 
+            True if the PSF model is varied (changes across the field-of-view)
             and False otherwise
         """
         return self._variable
 
-    def evaluate_to_array_form(self, 
+    def evaluate_to_array_form(self,
                                x: np.ndarray,
-                               y: np.ndarray, 
+                               y: np.ndarray,
                                size: int) -> ArrayCorrector:
         """Evaluates a FunctionalCorrector to an ArrayCorrector
 
         Parameters
         ----------
         x : np.ndarray
             the first dimension coordinates to evaluate over
@@ -151,30 +146,27 @@
 
         target_evaluation = self._target_model(image_x, image_y) if self._target_model else np.ones((size, size))
         return ArrayCorrector(evaluations, target_evaluation)
 
     def correct_image(self, image: np.ndarray, size: int,
                       alpha: float = 0.5, epsilon: float = 0.05) -> np.ndarray:
         corners = calculate_covering(image.shape, size)
-        array_corrector = self.evaluate_to_array_form(corners[:, 0], 
+        array_corrector = self.evaluate_to_array_form(corners[:, 0],
                                                       corners[:, 1], size)
-        return array_corrector.correct_image(image, 
-                                             size=size, 
-                                             alpha=alpha, 
+        return array_corrector.correct_image(image,
+                                             size=size,
+                                             alpha=alpha,
                                              epsilon=epsilon)
 
     def save(self, path: str) -> None:
-        with open(path, "wb") as f:
-            dill.dump(self, f)
+        raise NotImplementedError("You cannot save a FunctionalCorrector.")
 
     @classmethod
     def load(cls, path: str) -> FunctionalCorrector:
-        with open(path, "rb") as f:
-            return dill.load(f)
-
+        raise NotImplementedError("You cannot load a FunctionalCorrector.")
 
     def simulate_observation(self, image: np.ndarray, size: int) -> np.ndarray:
         """Simulates on a star field what an observation using this PSF looks like
 
         Parameters
         ----------
         image : 2D float np.ndarray
@@ -184,33 +176,33 @@
 
         Returns
         -------
         np.ndarray
             an image with the PSF applied
         """
         corners = calculate_covering(image.shape, size)
-        array_corrector = self.evaluate_to_array_form(corners[:, 0], 
-                                                      corners[:, 1], 
+        array_corrector = self.evaluate_to_array_form(corners[:, 0],
+                                                      corners[:, 1],
                                                       size)
         return array_corrector.simulate_observation(image)
 
 
 class ArrayCorrector(CorrectorABC):
     """ A PSF corrector that is evaluated as array patches
     """
-    def __init__(self, evaluations: dict[Any, np.ndarray], 
+    def __init__(self, evaluations: dict[Any, np.ndarray],
                  target_evaluation: np.ndarray) -> None:
         """Initialize an ArrayCorrector
 
         Parameters
         ----------
         evaluations : dict
-            evaluated version of the PSF as they vary over the image, 
+            evaluated version of the PSF as they vary over the image,
                 keys should be (x, y) of the lower left
-                pixel of each patch. values should be the `np.ndarray` 
+                pixel of each patch. values should be the `np.ndarray`
                 that corresponds to that patch
         target_evaluation : np.ndarray
             evaluated version of the target PSF
         """
         self._evaluation_points: list[Any] = list(evaluations.keys())
 
         if not isinstance(evaluations[self._evaluation_points[0]], np.ndarray):
@@ -237,50 +229,58 @@
 
         normalized_values = np.array(
                 [v / v.sum() for v in self._evaluations.values()], dtype=float)
         normalized_target = target_evaluation / target_evaluation.sum()
         self.target_fft, self.psf_i_fft = _precalculate_ffts(
                 normalized_target, normalized_values)
 
-    def correct_image(self, image: np.ndarray, size: int = None,  # noqa: ARG002, size used in FunctionalCorrector
+    @property
+    def evaluations(self) -> dict[Any, np.ndarray]:
+        return self._evaluations
+
+    @property
+    def evaluation_points(self) -> list:
+        return self._evaluation_points
+
+    def correct_image(self, image: np.ndarray, size: Optional[int] = None,  # noqa: ARG002
                       alpha: float = 0.5, epsilon: float = 0.05) -> np.ndarray:
-        if not all(img_dim_i >= psf_dim_i for img_dim_i, psf_dim_i in zip(image.shape, 
-                                                                          (self._size, 
+        if not all(img_dim_i >= psf_dim_i for img_dim_i, psf_dim_i in zip(image.shape,
+                                                                          (self._size,
                                                                            self._size))):
             msg = "The image must be at least as large as the PSFs in all dimensions"
             raise InvalidSizeError(msg)
 
         x = np.array([x for x, _ in self._evaluations], dtype=int)
         y = np.array([y for _, y in self._evaluations], dtype=int)
 
-        return _correct_image(image, 
-                              self.target_fft, 
-                              x, y, 
+        return _correct_image(image,
+                              self.target_fft,
+                              x, y,
                               self.psf_i_fft,  alpha, epsilon)
 
     def __getitem__(self, xy: Tuple[int, int]) -> np.ndarray:
         if xy in self._evaluation_points:
             return self._evaluations[xy]
         else:
             raise UnevaluatedPointError(f"Model not evaluated at {xy}.")
 
     def save(self, path: str) -> None:
-        with h5py.File(path, 'w') as f:
-            eval_grp = f.create_group('evaluations')
+        with h5py.File(path, "w") as f:
+            eval_grp = f.create_group("evaluations")
             for key, val in self._evaluations.items():
-                eval_grp.create_dataset(f'{key}', data=val)
-            f.create_dataset('target', data=self._target_evaluation)
+                eval_grp.create_dataset(f"{key}", data=val)
+            f.create_dataset("target", data=self._target_evaluation)
 
     @classmethod
     def load(cls, path: str) -> ArrayCorrector:
-        with h5py.File(path, 'r') as f:
-            target_evaluation = f['target'][:].copy()
+        with h5py.File(path, "r") as f:
+            target_evaluation = f["target"][:].copy()
 
-            evaluations = dict()
-            for key, val in f['evaluations'].items():
+            evaluations = {}
+            for key, val in f["evaluations"].items():
                 parsed_key = tuple(int(val) for val in key.replace("(", "").replace(")", "").split(","))
                 evaluations[parsed_key] = val[:].copy()
         return cls(evaluations, target_evaluation)
 
     def simulate_observation(self, image: np.ndarray) -> np.ndarray:
         psf_shape = (self._size, self._size)
         pad_shape = psf_shape
@@ -304,15 +304,15 @@
             xs, xe = x + psf_shape[0], x + 2 * psf_shape[0]
             ys, ye = y + psf_shape[1], y + 2 * psf_shape[1]
             observation_synthetic_p[xs:xe, ys:ye] = np.nansum(
                 [image, observation_synthetic_p[xs:xe, ys:ye]], axis=0)
 
         for (x, y), psf_i in self._evaluations.items():
             img_i = get_img_i(x, y)
-            out_i = np.real(ifftshift(ifft2(fft2(img_i * apodization_window) 
+            out_i = np.real(ifftshift(ifft2(fft2(img_i * apodization_window)
                                             * fft2(psf_i)))) * apodization_window
             set_synthetic_p(x, y, out_i)
 
         return observation_synthetic_p[psf_shape[0]:img_shape[0] + psf_shape[0],
                       psf_shape[1]:img_shape[1] + psf_shape[1]]
 
 
@@ -325,15 +325,15 @@
         shape of the image we plan to correct
     size : int
         size of the square patches we want to create
 
     Returns
     -------
     np.ndarray
-        an array of shape Nx2 where return[:, 0] 
+        an array of shape Nx2 where return[:, 0]
         are the x coordinate and return[:, 1] are the y coordinates
 
     """
     half_size = np.ceil(size / 2).astype(int)
 
     x1 = np.arange(0, image_shape[0], size)
     y1 = np.arange(0, image_shape[1], size)
```

### Comparing `regularizepsf-0.2.3/regularizepsf/fitter.py` & `regularizepsf-0.3.1/regularizepsf/fitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import abc
 import warnings
-from collections import namedtuple
-from collections.abc import Callable
+from typing import Any, Dict, List, Tuple, Optional, Generator
 from numbers import Real
-from typing import Any, Dict, Generator, List, Optional, Tuple
+from collections import namedtuple
 
 import h5py
 import numpy as np
 import sep
 from astropy.io import fits
 from lmfit import Parameters, minimize
 from lmfit.minimizer import MinimizerResult
@@ -33,27 +32,27 @@
             self.size = None
 
     def __len__(self) -> int:
         return len(self.patches)
 
     @classmethod
     @abc.abstractmethod
-    def extract(cls, 
-                images: list[np.ndarray], 
-                coordinates: list, 
+    def extract(cls,
+                images: list[np.ndarray],
+                coordinates: list,
                 size: int) -> PatchCollectionABC:
-        """Construct a PatchCollection from a set of images 
+        """Construct a PatchCollection from a set of images
         using the specified coordinates and patch size
 
         Parameters
         ----------
         images : list of np.ndarrays
             the images loaded
         coordinates : list
-            A list of coordinates for the lower left pixel of each patch, 
+            A list of coordinates for the lower left pixel of each patch,
                 specified in each type of PatchCollection
         size : int
             size of one side of the square patches extracted
 
         Returns
         -------
         np.ndarray
@@ -62,15 +61,15 @@
 
     def __getitem__(self, identifier: Any) -> np.ndarray:
         """Access a patch with square brackets
 
         Parameters
         ----------
         identifier : Any
-            identifier for a given patch, specifically implemented 
+            identifier for a given patch, specifically implemented
             for each PatchCollection
 
         Returns
         -------
         np.ndarray
             a patch's data
         """
@@ -82,35 +81,35 @@
 
     def __contains__(self, identifier: Any) -> bool:
         """Determines if a patch is in the collection
 
         Parameters
         ----------
         identifier : Any
-            identifier for a given patch, 
+            identifier for a given patch,
                 specifically implemented for each PatchCollection
 
         Returns
         -------
         bool
-            True if patch with specified identifier is in the collection, 
+            True if patch with specified identifier is in the collection,
                 False otherwise
         """
         return identifier in self.patches
 
     def add(self,
             identifier: Any,
             patch: np.ndarray,
             count: Optional[int] = None) -> None:
         """Add a new patch to the collection
 
         Parameters
         ----------
         identifier : Any
-            identifier for a given patch, 
+            identifier for a given patch,
                 specifically implemented for each PatchCollection
         patch : np.ndarray
             the data for a specific patch
         count : int
             Optionally, a corresponding item to add to the `counts` dictionary
 
         Returns
@@ -127,20 +126,20 @@
             self.counts[identifier] = count
 
         if self.size is None:
             self.size = patch.shape[0]
             # TODO : enforce square constraint
 
     @abc.abstractmethod
-    def average(self, 
-                corners: np.ndarray, 
-                step: int, 
+    def average(self,
+                corners: np.ndarray,
+                step: int,
                 size: int,
                 mode: str) -> PatchCollectionABC:
-        """Construct a new PatchCollection where patches 
+        """Construct a new PatchCollection where patches
         lying inside a new grid are averaged together
 
         Parameters
         ----------
         corners : np.ndarray
             an Nx2 `np.ndarray` of the lower left corners of the new patch grid
         step : int
@@ -153,16 +152,16 @@
         Returns
         -------
         PatchCollectionABC
             a PatchCollection where data is sampled at the new grid
         """
 
     @abc.abstractmethod
-    def fit(self, 
-            base_psf: SimplePSF, 
+    def fit(self,
+            base_psf: SimplePSF,
             is_varied: bool = False) -> PointSpreadFunctionABC:
         """
 
         Parameters
         ----------
         base_psf
         is_varied
@@ -211,16 +210,16 @@
         """Gets values of all patches"""
         return self.patches.values()
 
     def items(self) -> Dict:
         """A dictionary like iterator over the patches"""
         return self.patches.items()
 
-    def _fit_lmfit(self, 
-                   base_psf: SimplePSF, 
+    def _fit_lmfit(self,
+                   base_psf: SimplePSF,
                    initial_guesses: dict[str, Real]) -> dict[Any, MinimizerResult]:
         """Fit a patch using lmfit
 
         Parameters
         ----------
         base_psf : SimplePSF
             the PSF model to use in fitting
@@ -248,60 +247,60 @@
         return results
 
 
 CoordinateIdentifier = namedtuple("CoordinateIdentifier", "image_index, x, y")
 
 
 class CoordinatePatchCollection(PatchCollectionABC):
-    """A representation of a PatchCollection that operates 
+    """A representation of a PatchCollection that operates
     on pixel coordinates from a set of images"""
     @classmethod
     def extract(cls, images: list[np.ndarray],
                 coordinates: list[CoordinateIdentifier],
                 size: int) -> PatchCollectionABC:
         out = cls({})
 
         # pad in case someone selects a region on the edge of the image
         padding_shape = ((size, size), (size, size))
-        padded_images = [np.pad(image, padding_shape, mode="constant") 
+        padded_images = [np.pad(image, padding_shape, mode="constant")
                          for image in images]
 
         # TODO: prevent someone from selecting a region completing outside of the image
         for coordinate in coordinates:
             patch = padded_images[coordinate.image_index][coordinate.x+size:coordinate.x+2*size,
                                                           coordinate.y+size:coordinate.y+2*size]
             out.add(coordinate, patch)
         return out
 
     @classmethod
-    def find_stars_and_average(cls, 
+    def find_stars_and_average(cls,  # noqa: C901
                                images: list[str] | np.ndarray | Generator,
                                psf_size: int,
                                patch_size: int,
                                interpolation_scale: int = 1,
                                average_mode: str = "median",
                                percentile: float = 10,
                                star_threshold: int = 3,
                                star_mask: Optional[list[str] | np.ndarray | Generator] = None,
                                hdu_choice: int=0) -> CoordinatePatchCollection:
-        """Loads a series of images, finds stars in each, 
+        """Loads a series of images, finds stars in each,
             and builds a CoordinatePatchCollection with averaged stars
 
         Parameters
         ----------
         images : List[str] or np.ndarray or Generator
             The images to be processed. Can be a list of FITS filenames, a
             numpy array of shape (n_images, ny, nx), or a Generator that yields
             each data array in turn.
         psf_size : int
             size of the PSF model to use
         patch_size : int
             square size that each PSF model applies to
         interpolation_scale : int
-            if >1, the image are first scaled by this factor. 
+            if >1, the image are first scaled by this factor.
                 This results in stars being aligned at a subpixel scale
         average_mode : str
             "median", "percentile", or "mean": determines how patches are
             combined
         percentile : float
             If `average_mode` is `"percentile"`, use this percentile value
             (from 0 to 100)
@@ -313,63 +312,63 @@
             numpy array of shape (n_images, ny, nx), or a Generator that yields
             each mask array in turn. Where the mask pixel is `True`, the
             corresponding data array pixel will not be selected as a star. See
             `mask` in
             https://sep.readthedocs.io/en/v1.1.x/api/sep.extract.html#sep-extract
             for more details.
         hdu_choice : int
-            Which HDU from each image will be used, 
+            Which HDU from each image will be used,
                 default of 0 is most common but could be 1 for compressed images
 
         Returns
         -------
         CoordinatePatchCollection
             An averaged star model built from the provided images
 
         Notes
         ------
-        Using an `interpolation_scale` other than 1 
+        Using an `interpolation_scale` other than 1
             for large images can dramatically slow down the execution.
         """
         if isinstance(images, Generator):
             data_iterator = images
         elif isinstance(images, np.ndarray):
             if len(images.shape) == 3:
-                def generator():
+                def generator() -> np.ndarray:
                     for image in images:
                         yield image
                 data_iterator = generator()
             else:
                 raise ValueError("Image data array must be 3D")
         elif isinstance(images, List) and isinstance(images[0], str):
-            def generator():
+            def generator() -> np.ndarray:
                 for image_path in images:
                     with fits.open(image_path) as hdul:
                         yield hdul[hdu_choice].data.astype(float)
             data_iterator = generator()
         else:
-            raise ValueError("Unsupported type for `images`")
+            raise TypeError("Unsupported type for `images`")
 
         if star_mask is None:
-            def generator():
+            def generator() -> None:
                 while True:
                     yield None
             star_mask_iterator = generator()
         elif isinstance(star_mask, Generator):
             star_mask_iterator = star_mask
         elif isinstance(star_mask, np.ndarray):
             if len(star_mask.shape) == 3:
-                def generator():
+                def generator() -> np.ndarray:
                     for mask in star_mask:
                         yield mask
                 star_mask_iterator = generator()
             else:
                 raise ValueError("Star mask array must be 3D")
         elif isinstance(star_mask, List) and isinstance(star_mask[0], str):
-            def generator():
+            def generator() -> np.ndarray:
                 for mask_path in star_mask:
                     with fits.open(mask_path) as hdul:
                         yield hdul[hdu_choice].data.astype(bool)
             star_mask_iterator = generator()
         else:
             raise ValueError("Unsupported type for `star_mask`")
 
@@ -387,56 +386,56 @@
             elif image.shape != image_shape:
                 msg = ("Images must all be the same shape."
                       f"Found both {image_shape} and {image.shape}.")
                 raise ValueError(msg)
 
             # if the image should be scaled then, do the scaling before anything else
             if interpolation_scale != 1:
-                interpolator = RectBivariateSpline(np.arange(image.shape[0]), 
-                                                   np.arange(image.shape[1]), 
+                interpolator = RectBivariateSpline(np.arange(image.shape[0]),
+                                                   np.arange(image.shape[1]),
                                                    image)
                 image = interpolator(np.linspace(0,
                                                  image.shape[0] - 1,
                                                  1 + (image.shape[0] - 1) * interpolation_scale),
                                      np.linspace(0,
                                                  image.shape[1] - 1,
                                                  1 + (image.shape[1] - 1) * interpolation_scale))
 
             # find stars using SEP
             background = sep.Background(image)
             image_background_removed = image - background
-            image_star_coords = sep.extract(image_background_removed, 
-                                            star_threshold, 
+            image_star_coords = sep.extract(image_background_removed,
+                                            star_threshold,
                                             err=background.globalrms,
                                             mask=star_mask)
 
             coordinates = [CoordinateIdentifier(i,
                                                 int(round(y - psf_size * interpolation_scale / 2)),
                                                 int(round(x - psf_size * interpolation_scale / 2)))
                            for x, y in zip(image_star_coords["x"], image_star_coords["y"])]
 
             # pad in case someone selects a region on the edge of the image
             padding_shape = ((psf_size * interpolation_scale, psf_size * interpolation_scale),
                              (psf_size * interpolation_scale, psf_size * interpolation_scale))
             padded_image = np.pad(image_background_removed,
-                                  padding_shape, 
-                                  mode="constant", 
+                                  padding_shape,
+                                  mode="constant",
                                   constant_values=np.median(image))
 
             for coordinate in coordinates:
                 patch = padded_image[coordinate.x+interpolation_scale*psf_size:
                                      coordinate.x+2*interpolation_scale*psf_size,
                                      coordinate.y + interpolation_scale * psf_size:
                                      coordinate.y + 2 * interpolation_scale * psf_size]
                 this_collection.add(coordinate, patch)
 
-        corners = calculate_covering((image_shape[0] * interpolation_scale, 
+        corners = calculate_covering((image_shape[0] * interpolation_scale,
                                       image_shape[1] * interpolation_scale),
                                       patch_size * interpolation_scale)
-        averaged = this_collection.average(corners, 
+        averaged = this_collection.average(corners,
                                            patch_size * interpolation_scale, psf_size * interpolation_scale,
                                            mode=average_mode, percentile=percentile)
 
         if interpolation_scale != 1:
             for coordinate, _ in averaged.items():
                 averaged.patches[coordinate] = downscale_local_mean(averaged.patches[coordinate],
                                                                     (interpolation_scale, interpolation_scale))
@@ -450,15 +449,15 @@
                                             key.x // interpolation_scale,
                                             key.y // interpolation_scale),
                        patch,
                        count=count)
 
         return output
 
-    def average(self, corners: np.ndarray, patch_size: int, psf_size: int,  # noqa: ARG002, kept for consistency
+    def average(self, corners: np.ndarray, patch_size: int, psf_size: int,  # , kept for consistency
                 mode: str = "median", percentile: float = 10) -> PatchCollectionABC:
         CoordinatePatchCollection._validate_average_mode(mode, percentile)
 
         if mode == "mean":
             mean_stack = {tuple(corner): np.zeros((psf_size, psf_size))
                           for corner in corners}
             mean_counts = {tuple(corner): np.zeros((psf_size, psf_size))
@@ -486,23 +485,23 @@
             y_matches = (y_bounds[:, 0] <= center_y) * (center_y < y_bounds[:, 1])
             match_indices = np.where(x_matches * y_matches)[0]
 
             # add to averages and increment count
             for match_index in match_indices:
                 match_corner = tuple(corners[match_index])
                 if mode == "mean":
-                    mean_stack[match_corner] = np.nansum([mean_stack[match_corner], 
+                    mean_stack[match_corner] = np.nansum([mean_stack[match_corner],
                                                           patch], axis=0)
                     mean_counts[match_corner] += np.isfinite(patch)
                 else:
                     stack[match_corner].append(patch)
                 counts[match_corner] += 1
 
         if mode == "mean":
-            averages = {CoordinateIdentifier(None, corner[0], corner[1]): 
+            averages = {CoordinateIdentifier(None, corner[0], corner[1]):
                         mean_stack[corner] / mean_counts[corner]
                         for corner in mean_stack}
         elif mode == "median":
             averages = {CoordinateIdentifier(None, corner[0], corner[1]):
                             np.nanmedian(stack[corner], axis=0)
                                 if len(stack[corner]) > 0 else
                                 np.zeros((psf_size, psf_size))
@@ -532,24 +531,24 @@
             raise ValueError(msg)
         if mode == "percentile" and not (0 <= percentile <= 100):
             raise ValueError("`percentile` must be between 0 and 100, inclusive")
 
     def _calculate_pad_shape(self, size: int) -> Tuple[int, int]:
         pad_amount = size - self.size
         if pad_amount < 0:
-            raise InvalidSizeError(f"The average window size (found {size})" 
+            raise InvalidSizeError(f"The average window size (found {size})"
                                    "must be larger than the existing patch size"
                                    f"(found {self.size}).")
         if pad_amount % 2 != 0:
-            raise InvalidSizeError(f"The average window size (found {size})" 
+            raise InvalidSizeError(f"The average window size (found {size})"
                                    "must be the same parity as the existing patch size"
                                    f"(found {self.size}).")
         return ((pad_amount//2, pad_amount//2), (pad_amount//2, pad_amount//2))
 
-    def fit(self, base_psf: SimplePSF, 
+    def fit(self, base_psf: SimplePSF,
             is_varied: bool = False) -> PointSpreadFunctionABC:
         raise NotImplementedError("TODO")
 
     def to_array_corrector(self, target_evaluation: np.array) -> ArrayCorrector:
         """Converts a patch collection that has been averaged into an ArrayCorrector
 
         Parameters
@@ -578,16 +577,16 @@
         path : str
             where to save the patch collection
 
         Returns
         -------
         None
         """
-        with h5py.File(path, 'w') as f:
-            patch_grp = f.create_group('patches')
+        with h5py.File(path, "w") as f:
+            patch_grp = f.create_group("patches")
             for key, val in self.patches.items():
                 patch_grp.create_dataset(f"({key.image_index, key.x, key.y})", data=val)
 
     @classmethod
     def load(cls, path: str) -> PatchCollectionABC:
         """Load a PatchCollection from a file
 
@@ -597,14 +596,14 @@
             file path to load from
 
         Returns
         -------
         PatchCollectionABC
             the new patch collection
         """
-        patches = dict()
+        patches = {}
         with h5py.File(path, "r") as f:
-            for key, val in f['patches'].items():
+            for key, val in f["patches"].items():
                 parsed_key = tuple(int(val) for val in key.replace("(", "").replace(")", "").split(","))
                 coord_id = CoordinateIdentifier(image_index=parsed_key[0], x=parsed_key[1], y=parsed_key[2])
                 patches[coord_id] = val[:].copy()
         return cls(patches)
```

### Comparing `regularizepsf-0.2.3/regularizepsf/helper.c` & `regularizepsf-0.3.1/regularizepsf/helper.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* Generated by Cython 3.0.5 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/core/include"
+            "/tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "regularizepsf.helper",
         "sources": [
             "regularizepsf/helper.pyx"
         ]
     },
     "module_name": "regularizepsf.helper"
@@ -42,18 +42,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_5" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030005F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -137,14 +137,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -198,14 +200,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -259,60 +263,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -395,14 +422,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -587,26 +617,27 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
-        #endif
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -619,15 +650,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -652,15 +682,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -738,16 +768,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -947,15 +982,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1091,15 +1126,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1178,15 +1213,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1291,32 +1326,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1358,15 +1376,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1478,15 +1496,15 @@
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__) && !defined(_MSC_VER))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -1546,177 +1564,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1754,42 +1772,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2169,33 +2187,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
-    static CYTHON_UNUSED PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2225,30 +2244,30 @@
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_5
-#define __PYX_HAVE_RT_ImportType_proto_3_0_5
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_5(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_5(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_5 {
-   __Pyx_ImportType_CheckSize_Error_3_0_5 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_5 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_5 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_5(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_5 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2353,15 +2372,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -3190,261 +3209,261 @@
 #define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
 #define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
 #define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
 #define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
 #define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3453,29 +3472,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3486,15 +3505,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3503,29 +3522,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3536,15 +3555,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3553,29 +3572,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3586,15 +3605,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3603,29 +3622,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3636,15 +3655,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3653,29 +3672,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3686,217 +3705,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 969, __pyx_L1_error)
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3912,15 +3931,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3928,68 +3947,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 981, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 982, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 983, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 983, __pyx_L5_except_error)
+      __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -3997,15 +4016,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4020,15 +4039,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4044,15 +4063,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4060,68 +4079,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 987, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 988, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 989, __pyx_L5_except_error)
+      __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4129,15 +4148,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4152,15 +4171,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4176,15 +4195,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4192,68 +4211,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 993, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 994, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 995, __pyx_L5_except_error)
+      __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4261,15 +4280,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4284,170 +4303,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5914,24 +5933,24 @@
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_image)); if (unlikely(__pyx_t_1 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L1_error)
-  __pyx_t_15 = PyInt_FromSsize_t(((__pyx_t_1[0]) + (2 * __pyx_v_size))); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyInt_From_long(((__pyx_t_1[0]) + (2 * __pyx_v_size))); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __pyx_t_5 = PySlice_New(__pyx_t_2, __pyx_t_15, Py_None); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = __Pyx_PyInt_From_long((2 * __pyx_v_size)); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __pyx_t_1 = __pyx_f_5numpy_7ndarray_5shape_shape(((PyArrayObject *)__pyx_v_image)); if (unlikely(__pyx_t_1 == ((npy_intp *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L1_error)
-  __pyx_t_2 = PyInt_FromSsize_t(((__pyx_t_1[1]) + (2 * __pyx_v_size))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_long(((__pyx_t_1[1]) + (2 * __pyx_v_size))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PySlice_New(__pyx_t_15, __pyx_t_2, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -7693,44 +7712,44 @@
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 40, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 983, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 984, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 983, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-k38pf8bw/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-e4v6yjgg/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 989, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "regularizepsf/helper.pyx":11
  * @cython.wraparound(False)
  * @cython.cdivision(True)
  * cpdef _correct_image(np.ndarray[np.float_t, ndim=2] image,             # <<<<<<<<<<<<<<
@@ -7863,41 +7882,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_5(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 865, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -8104,15 +8123,15 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("helper", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to helper pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "helper" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -9779,17 +9798,18 @@
     PyErr_Format(PyExc_ValueError,
                  "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
                  index, (index == 1) ? "" : "s");
 }
 
 /* IterFinish */
   static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    PyObject* exc_type;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
         if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
         __Pyx_PyErr_Clear();
         return 0;
     }
     return 0;
@@ -9978,15 +9998,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_item(o, i);
         }
     }
 #else
-    if (is_list || PySequence_Check(o)) {
+    if (is_list || !PyMapping_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* PyObjectCallOneArg */
@@ -10240,22 +10260,22 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
-static CYTHON_UNUSED PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
         return NULL;
     for (i=0; i<nkwargs; i++) {
         PyObject *key = PyTuple_GET_ITEM(kwnames, i);
@@ -10357,15 +10377,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -10376,15 +10396,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -10408,15 +10428,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -10490,18 +10510,18 @@
         ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
     __Pyx_DECREF_TypeName(type_name);
     __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_5
-#define __PYX_HAVE_RT_ImportType_3_0_5
-static PyTypeObject *__Pyx_ImportType_3_0_5(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_5 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -10547,23 +10567,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_5 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_5 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -11857,15 +11877,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -12316,15 +12336,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
```

### Comparing `regularizepsf-0.2.3/regularizepsf/helper.pyx` & `regularizepsf-0.3.1/regularizepsf/helper.pyx`

 * *Files identical despite different names*

### Comparing `regularizepsf-0.2.3/regularizepsf/psf.py` & `regularizepsf-0.3.1/regularizepsf/psf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from __future__ import annotations
 
 import abc
 import inspect
-from functools import partial
+from typing import Any, Dict, List, Callable, cast
 from numbers import Real
-from typing import Any, Callable, Dict, List, cast
+from functools import partial
 
 import numpy as np
 
-from regularizepsf.exceptions import (
-    PSFParameterValidationError,
-    VariedPSFParameterMismatchError,
-)
+from regularizepsf.exceptions import PSFParameterValidationError, VariedPSFParameterMismatchError
 
 
 class PointSpreadFunctionABC(metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def __call__(self, x: Real | np.ndarary, y: Real | np.ndarray) -> Real | np.ndarray:
         """Evaluation of the point spread function
 
@@ -64,17 +61,17 @@
                 raise PSFParameterValidationError(msg)
             elif i == 1 and variable != "y":
                 msg = "y must be the second arguments in your model equation"
                 raise PSFParameterValidationError(msg)
             if i >= 2:
                 self._parameters.add(variable)
 
-    def __call__(self, 
+    def __call__(self,
                  x: Real | np.ndarray,
-                 y: Real | np.ndarray, 
+                 y: Real | np.ndarray,
                  **kwargs: Dict[str, Any]) -> Real | np.ndarray:
         return self._f(x, y, **kwargs)
 
     @property
     def parameters(self) -> set[str]:
         return self._parameters
 
@@ -85,17 +82,17 @@
     else:
         raise TypeError("psf decorator must have no arguments.")
 
 
 class VariedPSF(PointSpreadFunctionABC):
     """Model for a PSF that varies over the field of view"""
 
-    def __init__(self, 
+    def __init__(self,
                  vary_function: Callable,
-                 base_psf: SimplePSF, 
+                 base_psf: SimplePSF,
                  validate_at_call: bool = True) -> None:
         self._vary_function = vary_function
         self._base_psf = base_psf
         self.validate_at_call = validate_at_call
 
         self.parameterization_signature = inspect.signature(vary_function)
         if len(self.parameterization_signature.parameters) < 2:
@@ -117,15 +114,15 @@
                 raise PSFParameterValidationError(msg)
 
         # check the parameters at the origin
         origin_evaluation: dict[str, Any] = vary_function(0, 0)
         self._origin_parameters: set[str] = set(origin_evaluation.keys())
         if self._base_psf.parameters != self._origin_parameters:
             msg = (f"The base PSF model has parameters {self._base_psf.parameters} "
-                   f"while the varied psf supplies {self._origin_parameters}" 
+                   f"while the varied psf supplies {self._origin_parameters}"
                    "at the origin. These must match.")
             raise VariedPSFParameterMismatchError(msg)
 
     def __call__(self, x: Real | np.ndarray, y: Real | np.ndarray) -> Real | np.ndarray:
         variance = self._vary_function(x, y)
         if self.validate_at_call and set(variance.keys()) != self.parameters:
                 msg = (f"At (x, y) the varying parameters were {set(variance.keys())}"
@@ -138,15 +135,15 @@
         return self._base_psf.parameters
 
 
 def _varied_psf(base_psf: SimplePSF) -> VariedPSF:
     if base_psf is None:
         raise TypeError("A base_psf must be provided to the varied_psf decorator.")
 
-    def inner(__fn: Callable=None, *, check_at_call: bool = True) -> Callable:
+    def inner(__fn: Callable=None, *, check_at_call: bool = True) -> Callable:  # noqa: RUF013
         if __fn:
             return VariedPSF(__fn, base_psf, validate_at_call=check_at_call)
         else:
             return partial(inner, check_at_call=check_at_call)
 
     return inner
```

### Comparing `regularizepsf-0.2.3/regularizepsf/visualize.py` & `regularizepsf-0.3.1/regularizepsf/visualize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import copy
 import itertools
 from typing import Optional
 
-import matplotlib
+import matplotlib as mpl
+import matplotlib.colors
 import matplotlib.pyplot as plt
 import numpy as np
 
 from regularizepsf.corrector import ArrayCorrector
 from regularizepsf.fitter import CoordinateIdentifier, PatchCollectionABC
 from regularizepsf.helper import _regularize_array
 
 
 def visualize_patch_counts(patch_collection: PatchCollectionABC,
-                           ax: Optional[matplotlib.axes.Axes] = None,
-                           label_pixel_bounds: bool = False) -> matplotlib.axes.Axes:
+                           ax: Optional[mpl.axes.Axes] = None,
+                           label_pixel_bounds: bool = False) -> mpl.axes.Axes:
     """
     Utility to visualize the number of stars identified within each patch
 
     Parameters
     ----------
     patch_collection : PatchCollectionABC
         A patch collection, such as that returned by
@@ -32,30 +33,30 @@
     if patch_collection.counts is None or not len(patch_collection.counts):
         raise ValueError("This PatchCollection does not have any counts")
 
     if ax is None:
         fig = plt.figure()
         ax = fig.subplots()
 
-    rows = [k.x for k in patch_collection.counts.keys()]
-    columns = [k.y for k in patch_collection.counts.keys()]
+    rows = [k.x for k in patch_collection.counts]
+    columns = [k.y for k in patch_collection.counts]
     rows = np.unique(sorted(rows))
     columns = np.unique(sorted(columns))
     dr = rows[1] - rows[0]
     dc = columns[1] - columns[0]
 
     # Build an array containing all the patch counts
     counts = np.empty((len(rows), len(columns)))
     for k, count in patch_collection.counts.items():
         r, c = k.x, k.y
         r = int((r - rows.min()) / dr)
         c = int((c - columns.min()) / dc)
         counts[r, c] = count
 
-    m = ax.imshow(counts, origin='lower')
+    m = ax.imshow(counts, origin="lower")
     plt.colorbar(m).set_label(
             "Number of stars found in patch")
 
     if label_pixel_bounds:
         xticks = [xt for xt in plt.xticks()[0] if 0 <= xt < len(columns)]
         plt.xticks(
                 xticks,
@@ -73,36 +74,37 @@
     else:
         ax.set_xlabel("Patch number")
         ax.set_ylabel("Patch number")
 
     return ax
 
 
-def _generate_colormap():
+def _generate_colormap() -> matplotlib.colors.ListedColormap:
     a = np.linspace(0, 1, 1000)
     r = np.sqrt(a)
     g = a
     b = np.square(a)
     colors = np.stack([r, g, b], axis=-1)
-    return matplotlib.colors.ListedColormap(colors)
+    return mpl.colors.ListedColormap(colors)
 
 
 _colormap = _generate_colormap()
 
 
-def visualize_PSFs(psfs: ArrayCorrector,
-                   corrected: Optional[PatchCollectionABC] = None,
-                   all_patches: bool = False,
-                   region_size: int = 0,
-                   label_pixel_bounds: bool = False,
-                   fig: Optional[matplotlib.figure.Figure] = None,
-                   fig_scale: float = 1,
-                   colorbar_label: str = 'Normalized brightness',
-                   axis_border_color: str = 'white',
-                   imshow_args: dict = {}) -> matplotlib.figure.Figure:
+def visualize_PSFs(  # noqa: N802, C901
+        psfs: ArrayCorrector,
+        corrected: Optional[PatchCollectionABC] = None,
+        all_patches: bool = False,
+        region_size: int = 0,
+        label_pixel_bounds: bool = False,
+        fig: Optional[mpl.figure.Figure] = None,
+        fig_scale: float = 1,
+        colorbar_label: str = "Normalized brightness",
+        axis_border_color: str = "white",
+        imshow_args: Optional[dict] = None) -> mpl.figure.Figure:
     """
     Utility to visualize estimated PSFs.
 
     Accepts an `ArrayCorrector`, which contains the estimated PSFs across the
     image.
 
     This utility can also produce a "before and after" visualization. To do
@@ -145,30 +147,31 @@
 
     Returns
     -------
     fig : matplotlib.figure.Figure
         The generated figure
     """
     # Special-case vmin/vmax, and pass them to our PowerNorm
-    if 'norm' not in imshow_args:
-        vmin = imshow_args.pop('vmin', 0)
-        vmax = imshow_args.pop('vmax', 1)
+    imshow_args = {} if imshow_args is None else imshow_args
+    if "norm" not in imshow_args:
+        vmin = imshow_args.pop("vmin", 0)
+        vmax = imshow_args.pop("vmax", 1)
     else:
         # The default Norm will be overridden
         vmin, vmax = None, None
-    imshow_args_default = dict(
-        origin='lower',
-        cmap=_colormap,
-        norm=matplotlib.colors.PowerNorm(gamma=1/2.2, vmin=vmin, vmax=vmax)
-    )
+    imshow_args_default = {
+        "origin": "lower",
+        "cmap": _colormap,
+        "norm": mpl.colors.PowerNorm(gamma=1/2.2, vmin=vmin, vmax=vmax)
+    }
     imshow_args = imshow_args_default | imshow_args
 
     # Identify which patches we'll be plotting
-    rows = np.unique(sorted(r for r, c in psfs._evaluation_points))
-    columns = np.unique(sorted(c for r, c in psfs._evaluation_points))
+    rows = np.unique(sorted(r for r, c in psfs.evaluation_points))
+    columns = np.unique(sorted(c for r, c in psfs.evaluation_points))
     dr = rows[1] - rows[0]
     dc = columns[1] - columns[0]
     if not all_patches:
         rows = rows[1::2]
         columns = columns[1::2]
 
     if region_size:
@@ -197,15 +200,15 @@
                 [patches_width / len(columns)] * len(columns)
                 + [.2] + width_ratios)
 
     if fig is None:
         fig = plt.figure(
                 figsize=(total_width * fig_scale, patches_height * fig_scale))
 
-    gs = matplotlib.gridspec.GridSpec(
+    gs = mpl.gridspec.GridSpec(
             len(rows), n_columns, figure=fig,
             wspace=0, hspace=0,
             width_ratios=width_ratios)
 
     for i, j in itertools.product(range(len(rows)), range(len(columns))):
         ax = fig.add_subplot(gs[len(rows)-1-i, j])
         image = psfs[rows[i], columns[j]]
@@ -215,50 +218,50 @@
         # Ensure there's a thin line between subplots
         ax.spines[:].set_color(axis_border_color)
         ax.set_xticks([])
         ax.set_yticks([])
         if i == 0 and label_pixel_bounds:
             ax.set_xlabel(
                     f"{int(columns[j])} to\n{int(columns[j] + 2 * dc)} px",
-                    rotation='horizontal', ha='center')
+                    rotation="horizontal", ha="center")
         if j == 0 and label_pixel_bounds:
             ax.set_ylabel(
                     f"{int(rows[i])} to\n{int(rows[i] + 2 * dr)} px",
-                    rotation='horizontal', ha='right', va='center')
+                    rotation="horizontal", ha="right", va="center")
 
     cax = fig.add_subplot(gs[:, -1])
     fig.colorbar(im, cax=cax, label=colorbar_label)
 
     if corrected is not None:
         for i, j in itertools.product(range(len(rows)), range(len(columns))):
             ax = fig.add_subplot(gs[len(rows)-1-i, j + len(columns) + 1])
             image = corrected[CoordinateIdentifier(None, rows[i], columns[j])]
             if trim is not None:
                 image = image[trim:-trim, trim:-trim]
             im = ax.imshow(image, **imshow_args)
             # Ensure there's a thin white line between subplots
-            ax.spines[:].set_color('white')
+            ax.spines[:].set_color("white")
             ax.set_xticks([])
             ax.set_yticks([])
 
-        fig.text(0.31, 0.95, 'Uncorrected', ha='center', fontsize=15)
-        fig.text(0.7, 0.95, 'Corrected', ha='center', fontsize=15)
+        fig.text(0.31, 0.95, "Uncorrected", ha="center", fontsize=15)
+        fig.text(0.7, 0.95, "Corrected", ha="center", fontsize=15)
     return fig
 
 
 def visualize_transfer_kernels(psfs: ArrayCorrector,
                    alpha: float, epsilon: float,
                    all_patches: bool = False,
                    region_size: int = 0,
                    label_pixel_bounds: bool = False,
-                   fig: Optional[matplotlib.figure.Figure] = None,
+                   fig: Optional[mpl.figure.Figure] = None,
                    fig_scale: float = 1,
-                   colorbar_label: str = 'Transfer kernel amplitude',
-                   axis_border_color: str = 'black',
-                   imshow_args: dict = {}) -> matplotlib.figure.Figure:
+                   colorbar_label: str = "Transfer kernel amplitude",
+                   axis_border_color: str = "black",
+                   imshow_args: Optional[dict] = None) -> mpl.figure.Figure:
     """
     Utility to compute and visualize transfer kernels.
 
     Accepts an `ArrayCorrector`, which contains the estimated PSFs across the
     image. These PSFs, and the target PSF, will be used to compute each
     transfer kernel.
 
@@ -297,36 +300,38 @@
         Additional arguments to pass to each `plt.imshow()` call
 
     Returns
     -------
     fig : matplotlib.figure.Figure
         The generated figure
     """
+    imshow_args = {} if imshow_args is None else imshow_args
+
     # Copy the ArrayCorrector. We'll change each patch to store the transfer
     # kernel rather than the PSF
     tks = copy.deepcopy(psfs)
     extent = -np.inf
-    for i in range(len(tks._evaluations)):
+    for i in range(len(tks.evaluations)):
         psf_regularized_inverse = _regularize_array(
                 tks.psf_i_fft[i], alpha, epsilon, tks.target_fft)
         transfer_kernel = np.fft.ifft2(
                 psf_regularized_inverse * tks.target_fft).real
         # For some reason, the transfer kernel we get straddles the corners of
         # the image, rather than being centered. We must be picking up a phase
         # shift in Fourier space.
         transfer_kernel = np.fft.fftshift(transfer_kernel)
-        tks._evaluations[tks._evaluation_points[i]] = transfer_kernel
+        tks.evaluations[tks.evaluation_points[i]] = transfer_kernel
         extent = max(extent, np.max(np.abs(transfer_kernel)))
 
     # The plot we want is very similar to that produced by visualize_PSFs, so
     # we'll use that function and change some of the defaults.
-    imshow_args_default = dict(
-            norm=None,
-            cmap='bwr',
-            vmin=-extent,
-            vmax=extent)
+    imshow_args_default = {
+            "norm": None,
+            "cmap": "bwr",
+            "vmin": -extent,
+            "vmax": extent}
     imshow_args = imshow_args_default | imshow_args
     return visualize_PSFs(
             tks, all_patches=all_patches, region_size=region_size, fig=fig,
             fig_scale=fig_scale, colorbar_label=colorbar_label,
             axis_border_color=axis_border_color,
             label_pixel_bounds=label_pixel_bounds, imshow_args=imshow_args)
```

### Comparing `regularizepsf-0.2.3/regularizepsf.egg-info/PKG-INFO` & `regularizepsf-0.3.1/regularizepsf.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: regularizepsf
-Version: 0.2.3
+Version: 0.3.1
 Summary: Point spread function modeling and regularization
 Home-page: https://github.com/punch-mission/regularizepsf
 Author: J. Marcus Hughes
 Author-email: hughes.jmb@gmail.com
 License: MIT
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: dill
 Requires-Dist: h5py
 Requires-Dist: lmfit
 Requires-Dist: sep
@@ -35,27 +36,29 @@
 Below is an example of correcting model data using the package. An initial image of a simplified starfield (a) is synthetically observed with a slowly
 varying PSF (b), then regularized with this technique (c). The final image visually matches a direct convolution of
 the initial image with the target PSF (d). The panels are gamma-corrected to highlight the periphery of the model PSFs.
 ![Example result image](model_example.png)
 
 ## Getting started
 
-`pip install regularizepsf` and then follow along with the [Quickstart section](https://punch-mission.github.io/regularizepsf/quickstart.html). 
+`pip install regularizepsf` and then follow along with the [documentation](https://punch-mission.github.io/regularizepsf/concepts.html).
 
 ## Contributing
-We encourage all contributions. If you have a problem with the code or would like to see a new feature, please open an issue. Or you can submit a pull request. 
+We encourage all contributions. If you have a problem with the code or would like to see a new feature, please open an issue. Or you can submit a pull request.
+
+If you're contributing code please see [this package's development guide](https://punch-mission.github.io/regularizepsf/development.html).
 
 ## License
-See LICENSE for the MIT license
+See [LICENSE file](LICENSE)
 
 ## Need help?
-Please contact Marcus Hughes at [marcus.hughes@swri.org](mailto:marcus.hughes@swri.org).
+Please ask a question in our [discussions](https://github.com/punch-mission/regularizepsf/discussions)
 
 ## Citation
-Please cite the associated paper if you use this technique: 
+Please cite [the associated paper](https://iopscience.iop.org/article/10.3847/1538-3881/acc578) if you use this technique:
 
 ```
 @article{Hughes_2023,
 doi = {10.3847/1538-3881/acc578},
 url = {https://dx.doi.org/10.3847/1538-3881/acc578},
 year = {2023},
 month = {apr},
@@ -65,23 +68,8 @@
 pages = {204},
 author = {J. Marcus Hughes and Craig E. DeForest and Daniel B. Seaton},
 title = {Coma Off It: Regularizing Variable Point-spread Functions},
 journal = {The Astronomical Journal}
 }
 ```
 
-If you use this software, please also cite the package: 
-```
-@software{marcus_hughes_2023_8370994,
-  author       = {Marcus Hughes and
-                  Sam Van Kooten and
-                  Tania Varesano and
-                  Suman Chapai},
-  title        = {punch-mission/regularizepsf: 0.2.2},
-  month        = sep,
-  year         = 2023,
-  publisher    = {Zenodo},
-  version      = {0.2.2},
-  doi          = {10.5281/zenodo.8370994},
-  url          = {https://doi.org/10.5281/zenodo.8370994}
-}
-```
+If you use this software, please also cite the package with the specific version used. [Zenodo always has the most up-to-date citation](https://zenodo.org/records/10066960).
```

### Comparing `regularizepsf-0.2.3/regularizepsf.egg-info/SOURCES.txt` & `regularizepsf-0.3.1/regularizepsf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `regularizepsf-0.2.3/tests/test_corrector.py` & `regularizepsf-0.3.1/tests/test_corrector.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,16 @@
 
 import numpy as np
 import pytest
 from hypothesis import given, settings
 from hypothesis import strategies as st
 from pytest import fixture
 
-from regularizepsf.corrector import (
-    ArrayCorrector,
-    FunctionalCorrector,
-    calculate_covering,
-)
-from regularizepsf.exceptions import (
-    EvaluatedModelInconsistentSizeError,
-    InvalidSizeError,
-    UnevaluatedPointError,
-)
+from regularizepsf.corrector import ArrayCorrector, FunctionalCorrector, calculate_covering
+from regularizepsf.exceptions import EvaluatedModelInconsistentSizeError, InvalidSizeError, UnevaluatedPointError
 from regularizepsf.psf import simple_psf, varied_psf
 
 
 def confirm_full_four_covering(corners, img_shape, patch_size):
     counts = np.zeros(img_shape)
     for i, (x, y) in enumerate(corners):
         counts[np.max([0, x]):np.min([img_shape[0], x + patch_size]),
@@ -92,20 +84,14 @@
 
 def test_create_functional_corrector(tmp_path):
     example = FunctionalCorrector(example_psf, example_psf)
     assert example._psf == example_psf
     assert example.is_variable is False
     assert example._target_model == example_psf
 
-    fname = tmp_path / "test.psf"
-    example.save(fname)
-    assert os.path.isfile(fname)
-    loaded = example.load(fname)
-    assert isinstance(loaded, FunctionalCorrector)
-
 
 def test_evaluate_to_array_form_with_invalid_size_errors():
     @simple_psf
     def base(x, y):
         return np.ones_like(x)
 
     func_corrector = FunctionalCorrector(base, None)
```

### Comparing `regularizepsf-0.2.3/tests/test_fitter.py` & `regularizepsf-0.3.1/tests/test_fitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os.path
 import pathlib
 
-from astropy.io import fits
-import pytest
 import numpy as np
-from hypothesis import given, strategies as st, settings, HealthCheck
+import pytest
+from astropy.io import fits
+from hypothesis import HealthCheck, given, settings
+from hypothesis import strategies as st
 
-from regularizepsf.fitter import CoordinatePatchCollection, CoordinateIdentifier
 from regularizepsf.exceptions import InvalidSizeError
-
+from regularizepsf.fitter import CoordinateIdentifier, CoordinatePatchCollection
 
 TEST_DIR = pathlib.Path(__file__).parent.resolve()
 
 
 @pytest.fixture
 def incrementing_5_image_set_100x100():
     """ 5 images of size 100x100 that increment value from 0 to 4"""
@@ -235,8 +235,7 @@
             assert np.all(example_file[loc] == 0)
         elif loc.x <= 200 and loc.y <= 200:
             # This patch should be fully unmasked
             assert np.all(example_file[loc] == example_no_mask[loc])
         else:
             # This patche covers a mix of masked and non-masked areas
             assert np.any(example_file[loc] != 0)
-
```

### Comparing `regularizepsf-0.2.3/tests/test_psf.py` & `regularizepsf-0.3.1/tests/test_psf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
-from regularizepsf.psf import simple_psf, varied_psf, SimplePSF, VariedPSF
 from regularizepsf.exceptions import PSFParameterValidationError, VariedPSFParameterMismatchError
+from regularizepsf.psf import SimplePSF, VariedPSF, simple_psf, varied_psf
 
 
 def test_simple_psf_valid():
     """ Confirms that a psf with no extra parameters works"""
     func = lambda x, y: x + y
     eqn = simple_psf(func)
     assert isinstance(eqn, SimplePSF)
```

### Comparing `regularizepsf-0.2.3/tests/test_visualize.py` & `regularizepsf-0.3.1/tests/test_visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import pathlib
 
-from astropy.io import fits
 import numpy as np
 import pytest
+from astropy.io import fits
 
 import regularizepsf
 from regularizepsf.fitter import CoordinatePatchCollection
 
-
 TEST_DIR = pathlib.Path(__file__).parent.resolve()
 
 
 @pytest.mark.mpl_image_compare(style='mpl20', remove_text=True)
 def test_visualize_patch_counts():
     img_path = str(TEST_DIR / "data/DASH.fits")
     data = fits.getdata(img_path)
```

