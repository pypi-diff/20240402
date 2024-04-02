# Comparing `tmp/yasfpy-0.0.8.tar.gz` & `tmp/yasfpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yasfpy-0.0.8.tar", max compression
+gzip compressed data, was "yasfpy-0.0.9.tar", max compression
```

## Comparing `yasfpy-0.0.8.tar` & `yasfpy-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1083 2024-03-19 10:46:44.110679 yasfpy-0.0.8/LICENSE
--rw-r--r--   0        0        0     3137 2024-03-19 10:46:44.110679 yasfpy-0.0.8/README.md
--rw-r--r--   0        0        0     1051 2024-03-19 10:46:44.134679 yasfpy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/functions/__init__.py
--rw-r--r--   0        0        0    26539 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/functions/cpu_numba.py
--rw-r--r--   0        0        0    16482 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/functions/cuda_numba.py
--rw-r--r--   0        0        0     5074 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/functions/legendre_normalized_trigon.py
--rw-r--r--   0        0        0     6013 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/functions/material_handler.py
--rw-r--r--   0        0        0     8972 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/functions/misc.py
--rw-r--r--   0        0        0     3178 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/functions/spherical_functions_trigon.py
--rw-r--r--   0        0        0     2455 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/functions/t_entry.py
--rw-r--r--   0        0        0     4855 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/initial_field.py
--rw-r--r--   0        0        0     2542 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/log.py
--rw-r--r--   0        0        0    14235 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/numerics.py
--rwxr-xr-x   0        0        0    19384 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/optics.py
--rw-r--r--   0        0        0     4608 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/parameters.py
--rw-r--r--   0        0        0     6655 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/particles.py
--rw-r--r--   0        0        0    27944 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/simulation.py
--rw-r--r--   0        0        0     5549 2024-03-19 10:46:44.146679 yasfpy-0.0.8/yasfpy/solver.py
--rw-r--r--   0        0        0     4004 1970-01-01 00:00:00.000000 yasfpy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-02 14:54:04.831789 yasfpy-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3137 2024-04-02 14:54:04.831789 yasfpy-0.0.9/README.md
+-rw-r--r--   0        0        0     1051 2024-04-02 14:54:04.855789 yasfpy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 14:54:04.863789 yasfpy-0.0.9/yasfpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 14:54:04.863789 yasfpy-0.0.9/yasfpy/functions/__init__.py
+-rw-r--r--   0        0        0    26539 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/functions/cpu_numba.py
+-rw-r--r--   0        0        0    16482 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/functions/cuda_numba.py
+-rw-r--r--   0        0        0     5074 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/functions/legendre_normalized_trigon.py
+-rw-r--r--   0        0        0     5955 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/functions/material_handler.py
+-rw-r--r--   0        0        0    10364 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/functions/misc.py
+-rw-r--r--   0        0        0     3178 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/functions/spherical_functions_trigon.py
+-rw-r--r--   0        0        0     2455 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/functions/t_entry.py
+-rw-r--r--   0        0        0     4855 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/initial_field.py
+-rw-r--r--   0        0        0     2542 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/log.py
+-rw-r--r--   0        0        0    14235 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/numerics.py
+-rwxr-xr-x   0        0        0    44791 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/optics.py
+-rw-r--r--   0        0        0     4677 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/parameters.py
+-rw-r--r--   0        0        0     6685 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/particles.py
+-rw-r--r--   0        0        0    27944 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/simulation.py
+-rw-r--r--   0        0        0     5460 2024-04-02 14:54:04.867789 yasfpy-0.0.9/yasfpy/solver.py
+-rw-r--r--   0        0        0     4004 1970-01-01 00:00:00.000000 yasfpy-0.0.9/PKG-INFO
```

### Comparing `yasfpy-0.0.8/LICENSE` & `yasfpy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/README.md` & `yasfpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/pyproject.toml` & `yasfpy-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yasfpy"
-version = "0.0.8"
+version = "0.0.9"
 description = "Light scattering code using T-Matrix"
 authors = ["Mirza Arnaut <mirza.arnaut@tu-dortmund.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `yasfpy-0.0.8/yasfpy/functions/cpu_numba.py` & `yasfpy-0.0.9/yasfpy/functions/cpu_numba.py`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/yasfpy/functions/cuda_numba.py` & `yasfpy-0.0.9/yasfpy/functions/cuda_numba.py`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/yasfpy/functions/legendre_normalized_trigon.py` & `yasfpy-0.0.9/yasfpy/functions/legendre_normalized_trigon.py`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/yasfpy/functions/material_handler.py` & `yasfpy-0.0.9/yasfpy/functions/material_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         else:
             if ".csv" in link:
                 df, material = handle_csv(link)
                 data["ref_idx"] = pd.concat([data["ref_idx"], df])
                 data["material"] = material
             else:
                 print("No matching handler found for file type")
-    # data['ref_idx'] = data['ref_idx'].sort_values(by=['wavelength'])
+    data["ref_idx"] = data["ref_idx"].sort_values(by=["wavelength"])
     return data
 
 
 def handle_refractiveindex_info(url):
     """
     Retrieves refractive index data from a given URL and processes it.
 
@@ -105,17 +105,15 @@
                 coefficients = np.array(
                     [float(c) for c in line["coefficients"].split()]
                 )
                 ref_idx = lambda x: np.sqrt(
                     1
                     + np.sum(
                         [
-                            coefficients[i]
-                            * x**2
-                            / (x**2 - coefficients[i + 1] ** 2)
+                            coefficients[i] * x**2 / (x**2 - coefficients[i + 1] ** 2)
                             for i in range(1, len(coefficients), 2)
                         ],
                         axis=0,
                     )
                 )
                 df = pd.DataFrame(columns=["wavelength", "n", "k"])
                 df["wavelength"] = wavelengths
```

### Comparing `yasfpy-0.0.8/yasfpy/functions/misc.py` & `yasfpy-0.0.9/yasfpy/functions/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import numpy as np
+from yasfpy.particles import Particles
+from yasfpy.functions.legendre_normalized_trigon import legendre_normalized_trigon
 
+import numpy as np
 from scipy.special import spherical_jn
 from scipy.special import hankel1, lpmv
 
-from yasfpy.functions.legendre_normalized_trigon import legendre_normalized_trigon
-
 
 def jmult_max(num_part, lmax):
     """
     Calculate the maximum value of jmult.
 
     Parameters:
     num_part (int): The number of particles.
@@ -164,15 +164,15 @@
     sine_theta = np.sqrt(1 - cosine_theta**2)
     phi = np.arctan2(differences[:, :, 1], differences[:, :, 0])
     e_theta = np.stack(
         [cosine_theta * np.cos(phi), cosine_theta * np.sin(phi), -sine_theta], axis=-1
     )
     e_phi = np.stack([-np.sin(phi), np.cos(phi), np.zeros_like(phi)], axis=-1)
 
-    size_parameter = distances * refractive_index[np.newaxis, np.newaxis, :]
+    size_parameter = distances * np.array(refractive_index)[np.newaxis, np.newaxis, :]
 
     if parallel:
         from yasfpy.functions.cpu_numba import compute_lookup_tables
 
         spherical_bessel, spherical_hankel, e_j_dm_phi, p_lm = compute_lookup_tables(
             lmax, size_parameter, phi, cosine_theta
         )
@@ -247,7 +247,46 @@
         e_theta,
         e_phi,
         cosine_theta,
         sine_theta,
         size_parameter,
         spherical_hankel_derivative,
     )
+
+
+def interpolate_refractive_index_from_table(
+    wavelengths: np.ndarray, materials: list, species_idx: np.ndarray
+) -> np.ndarray:
+    """Interpolates the refractive index values from a table for different wavelengths.
+
+    Returns:
+        refractive_index_interpolated (np.array): An array that contains the interpolated refractive index values for the particles
+            at different wavelengths.
+    """
+
+    refractive_index_table = Particles.generate_refractive_index_table(materials)
+
+    unique_refractive_indices, _ = np.unique(species_idx, return_inverse=True, axis=0)
+    num_unique_refractive_indices = unique_refractive_indices.shape[0]
+
+    refractive_index_interpolated = np.zeros(
+        (num_unique_refractive_indices, wavelengths.size),
+        dtype=complex,
+    )
+    for idx, data in enumerate(refractive_index_table):
+        table = data["ref_idx"].to_numpy().astype(float)
+        n = np.interp(
+            wavelengths,
+            table[:, 0],
+            table[:, 1],
+            left=table[0, 1],
+            right=table[-1, 1],
+        )
+        k = np.interp(
+            wavelengths,
+            table[:, 0],
+            table[:, 2],
+            left=table[0, 2],
+            right=table[-1, 2],
+        )
+        refractive_index_interpolated[idx, :] = n + 1j * k
+    return refractive_index_interpolated
```

### Comparing `yasfpy-0.0.8/yasfpy/functions/spherical_functions_trigon.py` & `yasfpy-0.0.9/yasfpy/functions/spherical_functions_trigon.py`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/yasfpy/functions/t_entry.py` & `yasfpy-0.0.9/yasfpy/functions/t_entry.py`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/yasfpy/initial_field.py` & `yasfpy-0.0.9/yasfpy/initial_field.py`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/yasfpy/log.py` & `yasfpy-0.0.9/yasfpy/log.py`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/yasfpy/numerics.py` & `yasfpy-0.0.9/yasfpy/numerics.py`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/yasfpy/parameters.py` & `yasfpy-0.0.9/yasfpy/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import numpy as np
-
 from yasfpy.particles import Particles
 from yasfpy.initial_field import InitialField
 
 
 import numpy as np
 
 
@@ -12,16 +10,16 @@
     The Parameters class represents the parameters for a simulation, including wavelength, refractive
     indices, scattering particles, and initial field, and provides methods for computing angular
     frequency and wave vectors.
     """
 
     def __init__(
         self,
-        wavelength: np.array,
-        medium_refractive_index: np.array,
+        wavelength: np.ndarray,
+        medium_refractive_index: np.ndarray,
         particles: Particles,
         initial_field: InitialField,
     ):
         """Initializes the class with the given parameters and sets up the necessary variables.
 
         Args:
             wavelength (np.array): An array that represents the wavelengths of the light being used.
@@ -30,15 +28,15 @@
                 medium in which the particles are located. It contains the refractive index values at different
                 wavelengths.
             particles (Particles): An instance of the "Particles" class. It represents the particles
                 present in the medium.
             initial_field (InitialField): An object of the `InitialField` class. It represents the
                 initial field configuration for the simulation.
         """
-        self.wavelength = wavelength
+        self.wavelength = np.array(wavelength)
         self.medium_refractive_index = medium_refractive_index
         self.wavelengths_number = wavelength.size
         self.particles = particles
         self.initial_field = initial_field
 
         self.__setup()
 
@@ -61,22 +59,22 @@
         refractive_index_interpolated = np.zeros(
             (self.particles.num_unique_refractive_indices, self.wavelength.size),
             dtype=complex,
         )
         for idx, data in enumerate(self.particles.refractive_index_table):
             table = data["ref_idx"].to_numpy().astype(float)
             n = np.interp(
-                self.wavelength / 1e3,
+                self.wavelength,
                 table[:, 0],
                 table[:, 1],
                 left=table[0, 1],
                 right=table[-1, 1],
             )
             k = np.interp(
-                self.wavelength / 1e3,
+                self.wavelength,
                 table[:, 0],
                 table[:, 2],
                 left=table[0, 2],
                 right=table[-1, 2],
             )
             refractive_index_interpolated[idx, :] = n + 1j * k
         return refractive_index_interpolated
@@ -90,32 +88,33 @@
 
     def __compute_ks(self):
         """Computes the values of k_medium and k_particle based on the refractive index of the
         medium and particles.
         """
         self.k_medium = self.omega * self.medium_refractive_index
         if self.particles.refractive_index_table is None:
+            self.ref_idx_table = None
             self.k_particle = np.outer(self.particles.refractive_index, self.omega)
         else:
-            table = self.__interpolate_refractive_index_from_table()
+            self.ref_idx_table = self.__interpolate_refractive_index_from_table()
             self.k_particle = (
-                np.take(table, self.particles.refractive_index, axis=0)
-                * self.omega[np.newaxis, :]
+                np.take(self.ref_idx_table, self.particles.refractive_index, axis=0)
+                * np.array(self.omega)[np.newaxis, :]
             )
 
             unique_radius_index_pairs = np.zeros(
                 (
                     self.particles.unique_radius_index_pairs.shape[0],
                     self.wavelength.size + 1,
                 ),
                 dtype=complex,
             )
             unique_radius_index_pairs[:, 0] = self.particles.unique_radius_index_pairs[
                 :, 0
             ]
             unique_radius_index_pairs[:, 1:] = np.take(
-                table,
+                self.ref_idx_table,
                 self.particles.unique_radius_index_pairs[:, 1].astype(int),
                 axis=0,
             )
 
             self.particles.unique_radius_index_pairs = unique_radius_index_pairs
```

### Comparing `yasfpy-0.0.8/yasfpy/particles.py` & `yasfpy-0.0.9/yasfpy/particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     """The `Particles` class represents a collection of particles with various properties such as position,
     radius, and refractive index, and provides methods for computing unique properties and
     characteristics of the particles.
     """
 
     def __init__(
         self,
-        position: np.array,
-        r: np.array,
-        refractive_index: np.array,
+        position: np.ndarray,
+        r: np.ndarray,
+        refractive_index: np.ndarray,
         refractive_index_table: list = None,
         shape_type: str = "sphere",
     ):
         """Initializes an object with position, radius, refractive index, refractive index table, and shape type attributes.
 
         Args:
             position (np.array): A numpy array representing the position of the shape.
@@ -45,27 +45,27 @@
         self.refractive_index_table = refractive_index_table
 
         if refractive_index_table is None:
             if self.refractive_index.shape[1] == 2:
                 self.refractive_index = (
                     self.refractive_index[:, 0] + 1j * self.refractive_index[:, 1]
                 )
-        elif self.refractive_index.shape[1] > 2:
-            self.log.error(
-                "Refractive index should be either complex or a two column matrix!"
-            )
+            elif self.refractive_index.shape[1] > 2:
+                self.log.error(
+                    "Refractive index should be either complex or a two column matrix!"
+                )
         else:
             self.refractive_index = refractive_index.astype(int)
             self.refractive_index_table = refractive_index_table
 
         self.number = r.shape[0]
         self.__setup_impl()
 
     @staticmethod
-    def generate_refractive_index_table(urls: list):
+    def generate_refractive_index_table(urls: list) -> list:
         """The function `generate_refractive_index_table` takes a list of URLs, retrieves data from each
         URL using the `material_handler` function, and returns a list of the retrieved data.
 
         Args:
             urls (list): A list of URLs representing different materials.
 
         Returns:
```

### Comparing `yasfpy-0.0.8/yasfpy/simulation.py` & `yasfpy-0.0.9/yasfpy/simulation.py`

 * *Files identical despite different names*

### Comparing `yasfpy-0.0.8/yasfpy/solver.py` & `yasfpy-0.0.9/yasfpy/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import yasfpy.log as log
 
 import numpy as np
 from scipy.sparse.linalg import LinearOperator, gmres, lgmres, bicgstab
-
-
-import numpy as np
-from scipy.sparse.linalg import LinearOperator, bicgstab, gmres, lgmres
 from . import log
 
 
 class Solver:
     """
     The Solver class provides a generic interface for solving linear systems of equations using
     different iterative solvers such as GMRES, BiCGSTAB, and LGMRES, and the GMResCounter class is used
@@ -17,16 +13,16 @@
     solver.
     """
 
     def __init__(
         self,
         solver_type: str = "gmres",
         tolerance: float = 1e-4,
-        max_iter: int = 1e4,
-        restart: int = 1e2,
+        max_iter: float = 1e4,
+        restart: float = 1e2,
     ):
         """Initializes a solver object with specified parameters and creates a logger object.
 
         Args:
             solver_type (str, optional): The type of solver to be used. Defaults to "gmres".
             tolerance (float): The desired accuracy of the solver.
             max_iter (int): The maximum number of iterations that the solver will perform.
```

### Comparing `yasfpy-0.0.8/PKG-INFO` & `yasfpy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yasfpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Light scattering code using T-Matrix
 License: MIT
 Author: Mirza Arnaut
 Author-email: mirza.arnaut@tu-dortmund.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

