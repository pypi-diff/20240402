# Comparing `tmp/jax-scipy-spatial-0.2.1.tar.gz` & `tmp/jax-scipy-spatial-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-scipy-spatial-0.2.1.tar", last modified: Thu Jan 11 17:51:20 2024, max compression
+gzip compressed data, was "jax-scipy-spatial-0.2.2.tar", last modified: Tue Apr  2 13:22:58 2024, max compression
```

## Comparing `jax-scipy-spatial-0.2.1.tar` & `jax-scipy-spatial-0.2.2.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-01-11 17:51:20.111315 jax-scipy-spatial-0.2.1/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-01-11 17:51:20.107315 jax-scipy-spatial-0.2.1/.github/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-01-11 17:51:20.107315 jax-scipy-spatial-0.2.1/.github/workflows/
--rw-rw-r--   0 chris     (1000) chris     (1000)      527 2023-10-23 01:28:45.000000 jax-scipy-spatial-0.2.1/.github/workflows/run_tests.yml
--rw-rw-r--   0 chris     (1000) chris     (1000)    11358 2023-10-23 01:28:45.000000 jax-scipy-spatial-0.2.1/LICENSE
--rw-r--r--   0 chris     (1000) chris     (1000)     1673 2024-01-11 17:51:20.111315 jax-scipy-spatial-0.2.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      541 2024-01-10 17:42:08.000000 jax-scipy-spatial-0.2.1/README.md
--rw-rw-r--   0 chris     (1000) chris     (1000)     1219 2024-01-11 17:51:13.000000 jax-scipy-spatial-0.2.1/pyproject.toml
--rw-rw-r--   0 chris     (1000) chris     (1000)       31 2023-10-23 01:28:45.000000 jax-scipy-spatial-0.2.1/pytest.ini
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2024-01-11 17:51:20.111315 jax-scipy-spatial-0.2.1/setup.cfg
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-01-11 17:51:20.107315 jax-scipy-spatial-0.2.1/src/
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-01-11 17:51:20.107315 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial/
--rw-rw-r--   0 chris     (1000) chris     (1000)        0 2023-10-25 01:33:42.000000 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     5125 2023-10-25 02:33:17.000000 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial/distance.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    24489 2024-01-11 13:45:00.000000 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial/transform.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-01-11 17:51:20.111315 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial.egg-info/
--rw-r--r--   0 chris     (1000) chris     (1000)     1673 2024-01-11 17:51:20.000000 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      485 2024-01-11 17:51:20.000000 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2024-01-11 17:51:20.000000 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       28 2024-01-11 17:51:20.000000 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial.egg-info/requires.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       18 2024-01-11 17:51:20.000000 jax-scipy-spatial-0.2.1/src/jax_scipy_spatial.egg-info/top_level.txt
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2024-01-11 17:51:20.111315 jax-scipy-spatial-0.2.1/tests/
--rw-rw-r--   0 chris     (1000) chris     (1000)     3534 2024-01-10 17:42:08.000000 jax-scipy-spatial-0.2.1/tests/scipy_spatial_distance_test.py
--rw-rw-r--   0 chris     (1000) chris     (1000)    17127 2024-01-10 17:46:55.000000 jax-scipy-spatial-0.2.1/tests/scipy_spatial_transform_test.py
--rw-rw-r--   0 chris     (1000) chris     (1000)      111 2023-10-23 01:28:45.000000 jax-scipy-spatial-0.2.1/tox.ini
+drwxrwx---   0 chris     (1000) chris     (1000)        0 2024-04-02 13:22:58.372560 jax-scipy-spatial-0.2.2/
+drwxrwx---   0 chris     (1000) chris     (1000)        0 2024-04-02 13:22:58.372560 jax-scipy-spatial-0.2.2/.github/
+drwxrwx---   0 chris     (1000) chris     (1000)        0 2024-04-02 13:22:58.372560 jax-scipy-spatial-0.2.2/.github/workflows/
+-rw-rw----   0 chris     (1000) chris     (1000)      527 2024-04-02 12:44:30.000000 jax-scipy-spatial-0.2.2/.github/workflows/run_tests.yml
+-rw-rw----   0 chris     (1000) chris     (1000)    11358 2024-04-02 12:44:30.000000 jax-scipy-spatial-0.2.2/LICENSE
+-rw-r--r--   0 chris     (1000) chris     (1000)     1732 2024-04-02 13:22:58.372560 jax-scipy-spatial-0.2.2/PKG-INFO
+-rw-rw----   0 chris     (1000) chris     (1000)      600 2024-04-02 13:21:35.000000 jax-scipy-spatial-0.2.2/README.md
+-rw-rw----   0 chris     (1000) chris     (1000)     1219 2024-04-02 13:21:35.000000 jax-scipy-spatial-0.2.2/pyproject.toml
+-rw-rw----   0 chris     (1000) chris     (1000)       31 2024-04-02 12:44:30.000000 jax-scipy-spatial-0.2.2/pytest.ini
+-rw-rw----   0 chris     (1000) chris     (1000)       38 2024-04-02 13:22:58.372560 jax-scipy-spatial-0.2.2/setup.cfg
+drwxrwx---   0 chris     (1000) chris     (1000)        0 2024-04-02 13:22:58.372560 jax-scipy-spatial-0.2.2/src/
+drwxrwx---   0 chris     (1000) chris     (1000)        0 2024-04-02 13:22:58.372560 jax-scipy-spatial-0.2.2/src/jax_scipy_spatial/
+-rw-rw----   0 chris     (1000) chris     (1000)     5125 2024-04-02 12:44:30.000000 jax-scipy-spatial-0.2.2/src/jax_scipy_spatial/distance.py
+-rw-rw----   0 chris     (1000) chris     (1000)    24135 2024-04-02 13:21:35.000000 jax-scipy-spatial-0.2.2/src/jax_scipy_spatial/transform.py
+drwxrwx---   0 chris     (1000) chris     (1000)        0 2024-04-02 13:22:58.372560 jax-scipy-spatial-0.2.2/src/jax_scipy_spatial.egg-info/
+-rw-r--r--   0 chris     (1000) chris     (1000)     1732 2024-04-02 13:22:58.000000 jax-scipy-spatial-0.2.2/src/jax_scipy_spatial.egg-info/PKG-INFO
+-rw-rw----   0 chris     (1000) chris     (1000)      451 2024-04-02 13:22:58.000000 jax-scipy-spatial-0.2.2/src/jax_scipy_spatial.egg-info/SOURCES.txt
+-rw-rw----   0 chris     (1000) chris     (1000)        1 2024-04-02 13:22:58.000000 jax-scipy-spatial-0.2.2/src/jax_scipy_spatial.egg-info/dependency_links.txt
+-rw-rw----   0 chris     (1000) chris     (1000)       28 2024-04-02 13:22:58.000000 jax-scipy-spatial-0.2.2/src/jax_scipy_spatial.egg-info/requires.txt
+-rw-rw----   0 chris     (1000) chris     (1000)       18 2024-04-02 13:22:58.000000 jax-scipy-spatial-0.2.2/src/jax_scipy_spatial.egg-info/top_level.txt
+drwxrwx---   0 chris     (1000) chris     (1000)        0 2024-04-02 13:22:58.372560 jax-scipy-spatial-0.2.2/tests/
+-rw-rw----   0 chris     (1000) chris     (1000)     3534 2024-04-02 12:44:30.000000 jax-scipy-spatial-0.2.2/tests/scipy_spatial_distance_test.py
+-rw-rw----   0 chris     (1000) chris     (1000)    17127 2024-04-02 13:11:23.000000 jax-scipy-spatial-0.2.2/tests/scipy_spatial_transform_test.py
+-rw-rw----   0 chris     (1000) chris     (1000)      111 2024-04-02 12:44:30.000000 jax-scipy-spatial-0.2.2/tox.ini
```

### Comparing `jax-scipy-spatial-0.2.1/.github/workflows/run_tests.yml` & `jax-scipy-spatial-0.2.2/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `jax-scipy-spatial-0.2.1/LICENSE` & `jax-scipy-spatial-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jax-scipy-spatial-0.2.1/PKG-INFO` & `jax-scipy-spatial-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-scipy-spatial
-Version: 0.2.1
+Version: 0.2.2
 Summary: Scipy spatial API for JAX
 Author-email: Chris Flesher <chris.flesher@gmail.com>
 Project-URL: Homepage, https://github.com/chrisflesher/jax-scipy-spatial
 Project-URL: Bug Tracker, https://github.com/chrisflesher/jax-scipy-spatial/issues
 Keywords: jax,scipy,spatial,rotation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -45,15 +45,15 @@
 import jax_scipy_spatial.transform as jtr
 
 rotation = jtr.Rotation.from_euler('xyz', jnp.array([0., 0., 180.]), degrees=True)
 print(rotation)
 ```
 
 ## Documentation
-Please refer to scipy documentation.
+Please refer to [scipy documentation](https://docs.scipy.org/doc/scipy/reference/spatial.html).
 
 ## Contributing
 
 To run unit tests on your local machine:
 ```
 tox
 ```
```

### Comparing `jax-scipy-spatial-0.2.1/README.md` & `jax-scipy-spatial-0.2.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import jax_scipy_spatial.transform as jtr
 
 rotation = jtr.Rotation.from_euler('xyz', jnp.array([0., 0., 180.]), degrees=True)
 print(rotation)
 ```
 
 ## Documentation
-Please refer to scipy documentation.
+Please refer to [scipy documentation](https://docs.scipy.org/doc/scipy/reference/spatial.html).
 
 ## Contributing
 
 To run unit tests on your local machine:
 ```
 tox
 ```
```

### Comparing `jax-scipy-spatial-0.2.1/pyproject.toml` & `jax-scipy-spatial-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jax-scipy-spatial"
-version = "0.2.1"
+version = "0.2.2"
 description = "Scipy spatial API for JAX"
 readme = "README.md"
 authors = [
     { name = "Chris Flesher", email = "chris.flesher@gmail.com" }
 ]
 keywords = ["jax", "scipy", "spatial", "rotation"]
 classifiers = [
```

### Comparing `jax-scipy-spatial-0.2.1/src/jax_scipy_spatial/distance.py` & `jax-scipy-spatial-0.2.2/src/jax_scipy_spatial/distance.py`

 * *Files identical despite different names*

### Comparing `jax-scipy-spatial-0.2.1/src/jax_scipy_spatial/transform.py` & `jax-scipy-spatial-0.2.2/src/jax_scipy_spatial/transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,39 +17,41 @@
 import re
 import typing
 
 import scipy.spatial.transform
 
 import jax
 import jax.numpy as jnp
-from jax._src.numpy.util import _wraps
 from scipy.constants import golden
 
+try:
+  from jax._src.numpy.util import implements
+except ImportError:
+  from jax._src.numpy.util import _wraps as implements  # for jax < 0.4.25
 
-@_wraps(scipy.spatial.transform.Rotation)
+
+@implements(scipy.spatial.transform.Rotation)
 class Rotation:
   """Rotation in 3 dimensions."""
 
   _quat: jax.Array
 
   def __init__(self, quat: jax.Array):
     """Initialize."""
     self._quat = quat
 
   @classmethod
   def align_vectors(cls, a: jax.Array, b: jax.Array, weights: typing.Optional[jax.Array] = None, return_sensitivity: bool = False):
     """Estimate a rotation to optimally align two sets of vectors."""
     a = jnp.asarray(a)
     if a.ndim < 2 or a.shape[-1] != 3:
-      raise ValueError("Expected input `a` to have shape (..., 3), "
-                       "got {}".format(a.shape))
+      raise ValueError(f"Expected input `a` to have shape (..., 3), got {a.shape}")
     b = jnp.asarray(b)
     if b.ndim < 2 or b.shape[-1] != 3:
-      raise ValueError("Expected input `b` to have shape (..., 3), "
-                       "got {}.".format(b.shape))
+      raise ValueError(f"Expected input `b` to have shape (..., 3), got {b.shape}")
     if weights is None:
       weights = jnp.ones(b.shape[-2], dtype=b.dtype)
     else:
       weights = jnp.asarray(weights, dtype=b.dtype)
       # if jnp.any(weights < 0):  # this causes a concretization error...
       #   raise ValueError("`weights` may not contain negative values")
     matrix, rssd, sensitivity = _align_vectors(a, b, weights)
@@ -97,29 +99,23 @@
     return cls(jnp.concatenate([rotation._quat for rotation in rotations]))
 
   @classmethod
   def from_euler(cls, seq: str, angles: jax.Array, degrees: bool = False):
     """Initialize from Euler angles."""
     num_axes = len(seq)
     if num_axes < 1 or num_axes > 3:
-      raise ValueError("Expected axis specification to be a non-empty "
-                       "string of upto 3 characters, got {}".format(seq))
+      raise ValueError(f"Expected axis specification to be a non-empty string of upto 3 characters, got {seq}")
     intrinsic = (re.match(r'^[XYZ]{1,3}$', seq) is not None)
     extrinsic = (re.match(r'^[xyz]{1,3}$', seq) is not None)
     if not (intrinsic or extrinsic):
-      raise ValueError("Expected axes from `seq` to be from ['x', 'y', "
-                       "'z'] or ['X', 'Y', 'Z'], got {}".format(seq))
+      raise ValueError(f"Expected axes from `seq` to be from ['x', 'y', 'z'] or ['X', 'Y', 'Z'], got {seq}")
     if any(seq[i] == seq[i+1] for i in range(num_axes - 1)):
-      raise ValueError("Expected consecutive axes to be different, "
-                       "got {}".format(seq))
-    angles = jnp.atleast_1d(angles)
-    if len(seq) == 1 and angles.ndim == 1:
-      angles = angles[:, jnp.newaxis]
+      raise ValueError(f"Expected consecutive axes to be different, got {seq}")
     axes = jnp.array([_elementary_basis_index(x) for x in seq.lower()])
-    quat = _elementary_quat_compose(angles, axes, intrinsic, degrees)
+    quat = _elementary_quat_compose(angles.reshape(-1, axes.size), axes, intrinsic, degrees)
     return cls(quat)
 
   @classmethod
   def from_matrix(cls, matrix: jax.Array):
     """Initialize from rotation matrix."""
     return cls(_from_matrix(matrix))
 
@@ -171,24 +167,21 @@
   def apply(self, vectors: jax.Array, inverse: bool = False) -> jax.Array:
     """Apply this rotation to one or more vectors."""
     return _apply(self.as_matrix(), vectors, inverse)
 
   def as_euler(self, seq: str, degrees: bool = False):
     """Represent as Euler angles."""
     if len(seq) != 3:
-      raise ValueError("Expected 3 axes, got {}.".format(seq))
+      raise ValueError(f"Expected 3 axes, got {seq}.")
     intrinsic = (re.match(r'^[XYZ]{1,3}$', seq) is not None)
     extrinsic = (re.match(r'^[xyz]{1,3}$', seq) is not None)
     if not (intrinsic or extrinsic):
-      raise ValueError("Expected axes from `seq` to be from "
-                       "['x', 'y', 'z'] or ['X', 'Y', 'Z'], "
-                       "got {}".format(seq))
+      raise ValueError(f"Expected axes from `seq` to be from ['x', 'y', 'z'] or ['X', 'Y', 'Z'], got {seq}")
     if any(seq[i] == seq[i+1] for i in range(2)):
-      raise ValueError("Expected consecutive axes to be different, "
-                       "got {}".format(seq))
+      raise ValueError(f"Expected consecutive axes to be different, got {seq}")
     axes = jnp.array([_elementary_basis_index(x) for x in seq.lower()])
     return _compute_euler_from_quat(self._quat, axes, extrinsic, degrees)
 
   def as_matrix(self) -> jax.Array:
     """Represent as rotation matrix."""
     return _as_matrix(self._quat)
 
@@ -212,19 +205,17 @@
     """Get the magnitude(s) of the rotation(s)."""
     return _magnitude(self._quat)
 
   def mean(self, weights: typing.Optional[jax.Array] = None):
     """Get the mean of the rotations."""
     weights = jnp.where(weights is None, jnp.ones(self._quat.shape[0], dtype=self._quat.dtype), jnp.asarray(weights, dtype=self._quat.dtype))
     if weights.ndim != 1:
-      raise ValueError("Expected `weights` to be 1 dimensional, got "
-                       "shape {}.".format(weights.shape))
+      raise ValueError(f"Expected `weights` to be 1 dimensional, got shape {weights.shape}.")
     if weights.shape[0] != len(self):
-      raise ValueError("Expected `weights` to have number of values "
-                       "equal to number of rotations, got "
+      raise ValueError("Expected `weights` to have number of values equal to number of rotations, got "
                        "{} values and {} rotations.".format(weights.shape[0], len(self)))
     K = jnp.dot(weights[jnp.newaxis, :] * self._quat.T, self._quat)
     _, v = jnp.linalg.eigh(K)
     return Rotation(v[:, -1])
 
   def reduce(self, left=None, right=None, return_indices=False):
     """Reduce this rotation with the provided rotation groups."""
@@ -251,32 +242,29 @@
 jax.tree_util.register_pytree_node(
   Rotation,
   lambda obj: ((obj._quat,), None),
   lambda aux, children: Rotation(*children),
 )
 
 
-@_wraps(scipy.spatial.transform.Slerp)
+@implements(scipy.spatial.transform.Slerp)
 class Slerp:
   """Spherical Linear Interpolation of Rotations."""
 
   def __init__(self, times: jax.Array, rotations: Rotation):
     if not isinstance(rotations, Rotation):
       raise TypeError("`rotations` must be a `Rotation` instance.")
     if rotations.single or len(rotations) == 1:
       raise ValueError("`rotations` must be a sequence of at least 2 rotations.")
     times = jnp.asarray(times, dtype=rotations.as_quat().dtype)
     if times.ndim != 1:
-      raise ValueError("Expected times to be specified in a 1 "
-                       "dimensional array, got {} "
-                       "dimensions.".format(times.ndim))
+      raise ValueError(f"Expected times to be specified in a 1 dimensional array, got {times.ndim} dimensions.")
     if times.shape[0] != len(rotations):
-      raise ValueError("Expected number of rotations to be equal to "
-                       "number of timestamps given, got {} rotations "
-                       "and {} timestamps.".format(len(rotations), times.shape[0]))
+      raise ValueError("Expected number of rotations to be equal to number of timestamps given, got "
+                       "{} rotations and {} timestamps.".format(len(rotations), times.shape[0]))
     timedelta = jnp.diff(times)
     # if jnp.any(timedelta <= 0):  # this causes a concretization error...
     #   raise ValueError("Times must be in strictly increasing order.")
     new_rotations = Rotation(rotations.as_quat()[:-1])
     self._times = times
     self._timedelta = timedelta
     self._rotations = new_rotations
@@ -318,15 +306,15 @@
   zeta = (s[0] + s[1]) * (s[1] + s[2]) * (s[2] + s[0])
   kappa = s[0] * s[1] + s[1] * s[2] + s[2] * s[0]
   # with jnp.errstate(divide='ignore', invalid='ignore'):
   sensitivity = jnp.mean(weights) / zeta * (kappa * jnp.eye(3, dtype=B.dtype) + jnp.dot(B, B.T))
   return C, rssd, sensitivity
 
 
-@functools.partial(jnp.vectorize, signature='(m,m),(m),()->(m)')
+@functools.partial(jnp.vectorize, signature='(m,m),(m)->(m)', excluded=(2,))
 def _apply(matrix: jax.Array, vector: jax.Array, inverse: bool) -> jax.Array:
   return jnp.where(inverse, matrix.T, matrix) @ vector
 
 
 @functools.partial(jnp.vectorize, signature='(m)->(n,n)')
 def _as_matrix(quat: jax.Array) -> jax.Array:
   x = quat[0]
@@ -351,15 +339,15 @@
 @functools.partial(jnp.vectorize, signature='(m)->(n)')
 def _as_mrp(quat: jax.Array) -> jax.Array:
   sign = jnp.where(quat[3] < 0, -1., 1.)
   denominator = 1. + sign * quat[3]
   return sign * quat[:3] / denominator
 
 
-@functools.partial(jnp.vectorize, signature='(m),()->(n)')
+@functools.partial(jnp.vectorize, signature='(m)->(n)', excluded=(1,))
 def _as_rotvec(quat: jax.Array, degrees: bool) -> jax.Array:
   quat = jnp.where(quat[3] < 0, -quat, quat)  # w > 0 to ensure 0 <= angle <= pi
   angle = 2. * jnp.arctan2(_vector_norm(quat[:3]), quat[3])
   angle2 = angle * angle
   small_scale = 2 + angle2 / 12 + 7 * angle2 * angle2 / 2880
   large_scale = angle / jnp.sin(angle / 2)
   scale = jnp.where(angle <= 1e-3, small_scale, large_scale)
@@ -372,15 +360,15 @@
   cross = jnp.cross(p[:3], q[:3])
   return jnp.array([p[3]*q[0] + q[3]*p[0] + cross[0],
                     p[3]*q[1] + q[3]*p[1] + cross[1],
                     p[3]*q[2] + q[3]*p[2] + cross[2],
                     p[3]*q[3] - p[0]*q[0] - p[1]*q[1] - p[2]*q[2]])
 
 
-@functools.partial(jnp.vectorize, signature='(m),(l),(),()->(n)')
+@functools.partial(jnp.vectorize, signature='(m),(l)->(n)', excluded=(2, 3))
 def _compute_euler_from_quat(quat: jax.Array, axes: jax.Array, extrinsic: bool, degrees: bool) -> jax.Array:
   angle_first = jnp.where(extrinsic, 0, 2)
   angle_third = jnp.where(extrinsic, 2, 0)
   axes = jnp.where(extrinsic, axes, axes[::-1])
   i = axes[0]
   j = axes[1]
   k = axes[2]
@@ -512,39 +500,39 @@
 def _elementary_basis_index(axis: str) -> int:
   if axis == 'x':
     return 0
   elif axis == 'y':
     return 1
   elif axis == 'z':
     return 2
-  raise ValueError("Expected axis to be from ['x', 'y', 'z'], got {}".format(axis))
+  raise ValueError(f"Expected axis to be from ['x', 'y', 'z'], got {axis}")
 
 
-@functools.partial(jnp.vectorize, signature=('(m),(m),(),()->(n)'))
+@functools.partial(jnp.vectorize, signature='(m),(m)->(n)', excluded=(2, 3))
 def _elementary_quat_compose(angles: jax.Array, axes: jax.Array, intrinsic: bool, degrees: bool) -> jax.Array:
   angles = jnp.where(degrees, jnp.deg2rad(angles), angles)
   result = _make_elementary_quat(axes[0], angles[0])
   for idx in range(1, len(axes)):
     quat = _make_elementary_quat(axes[idx], angles[idx])
     result = jnp.where(intrinsic, _compose_quat(result, quat), _compose_quat(quat, result))
   return result
 
 
-@functools.partial(jnp.vectorize, signature=('(m),()->(n)'))
+@functools.partial(jnp.vectorize, signature='(m)->(n)', excluded=(1,))
 def _from_rotvec(rotvec: jax.Array, degrees: bool) -> jax.Array:
   rotvec = jnp.where(degrees, jnp.deg2rad(rotvec), rotvec)
   angle = _vector_norm(rotvec)
   angle2 = angle * angle
   small_scale = scale = 0.5 - angle2 / 48 + angle2 * angle2 / 3840
   large_scale = jnp.sin(angle / 2) / angle
   scale = jnp.where(angle <= 1e-3, small_scale, large_scale)
   return jnp.hstack([scale * rotvec, jnp.cos(angle / 2)])
 
 
-@functools.partial(jnp.vectorize, signature=('(m,m)->(n)'))
+@functools.partial(jnp.vectorize, signature='(m,m)->(n)')
 def _from_matrix(matrix: jax.Array) -> jax.Array:
   matrix_trace = matrix[0, 0] + matrix[1, 1] + matrix[2, 2]
   decision = jnp.array([matrix[0, 0], matrix[1, 1], matrix[2, 2], matrix_trace], dtype=matrix.dtype)
   choice = jnp.argmax(decision)
   i = choice
   j = (i + 1) % 3
   k = (j + 1) % 3
```

### Comparing `jax-scipy-spatial-0.2.1/src/jax_scipy_spatial.egg-info/PKG-INFO` & `jax-scipy-spatial-0.2.2/src/jax_scipy_spatial.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jax-scipy-spatial
-Version: 0.2.1
+Version: 0.2.2
 Summary: Scipy spatial API for JAX
 Author-email: Chris Flesher <chris.flesher@gmail.com>
 Project-URL: Homepage, https://github.com/chrisflesher/jax-scipy-spatial
 Project-URL: Bug Tracker, https://github.com/chrisflesher/jax-scipy-spatial/issues
 Keywords: jax,scipy,spatial,rotation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -45,15 +45,15 @@
 import jax_scipy_spatial.transform as jtr
 
 rotation = jtr.Rotation.from_euler('xyz', jnp.array([0., 0., 180.]), degrees=True)
 print(rotation)
 ```
 
 ## Documentation
-Please refer to scipy documentation.
+Please refer to [scipy documentation](https://docs.scipy.org/doc/scipy/reference/spatial.html).
 
 ## Contributing
 
 To run unit tests on your local machine:
 ```
 tox
 ```
```

### Comparing `jax-scipy-spatial-0.2.1/tests/scipy_spatial_distance_test.py` & `jax-scipy-spatial-0.2.2/tests/scipy_spatial_distance_test.py`

 * *Files identical despite different names*

### Comparing `jax-scipy-spatial-0.2.1/tests/scipy_spatial_transform_test.py` & `jax-scipy-spatial-0.2.2/tests/scipy_spatial_transform_test.py`

 * *Files identical despite different names*

