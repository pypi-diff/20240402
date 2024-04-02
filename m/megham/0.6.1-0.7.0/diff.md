# Comparing `tmp/megham-0.6.1.tar.gz` & `tmp/megham-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megham-0.6.1.tar", last modified: Sun Jan 28 20:18:24 2024, max compression
+gzip compressed data, was "megham-0.7.0.tar", last modified: Tue Apr  2 21:41:36 2024, max compression
```

## Comparing `megham-0.6.1.tar` & `megham-0.7.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:18:24.313410 megham-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-28 20:18:16.000000 megham-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-01-28 20:18:24.313410 megham-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-01-28 20:18:16.000000 megham-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:18:24.309410 megham-0.6.1/megham/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 20:18:16.000000 megham-0.6.1/megham/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-01-28 20:18:16.000000 megham-0.6.1/megham/mds.py
--rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-01-28 20:18:16.000000 megham-0.6.1/megham/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 20:18:24.309410 megham-0.6.1/megham.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-01-28 20:18:24.000000 megham-0.6.1/megham.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-28 20:18:24.000000 megham-0.6.1/megham.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 20:18:24.000000 megham-0.6.1/megham.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-01-28 20:18:24.000000 megham-0.6.1/megham.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 20:18:24.000000 megham-0.6.1/megham.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-28 20:18:16.000000 megham-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 20:18:24.313410 megham-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:41:36.396128 megham-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-02 21:41:32.000000 megham-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-02 21:41:36.396128 megham-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-02 21:41:32.000000 megham-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:41:36.392128 megham-0.7.0/megham/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:41:32.000000 megham-0.7.0/megham/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14727 2024-04-02 21:41:32.000000 megham-0.7.0/megham/mds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11820 2024-04-02 21:41:32.000000 megham-0.7.0/megham/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-02 21:41:32.000000 megham-0.7.0/megham/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:41:36.396128 megham-0.7.0/megham.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-02 21:41:36.000000 megham-0.7.0/megham.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 21:41:36.000000 megham-0.7.0/megham.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:41:36.000000 megham-0.7.0/megham.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 21:41:36.000000 megham-0.7.0/megham.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 21:41:36.000000 megham-0.7.0/megham.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-02 21:41:32.000000 megham-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:41:36.396128 megham-0.7.0/setup.cfg
```

### Comparing `megham-0.6.1/LICENSE` & `megham-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `megham-0.6.1/PKG-INFO` & `megham-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megham
-Version: 0.6.1
+Version: 0.7.0
 Summary: Tools for working with point clouds
 Author: Saianeesh Keshav Haridas
 License: GPLv3
 Keywords: point cloud,affine,rotations,mds,multidimensional scaling,point set registration,cpd,coherent point drift,mpd,guassian mixture model
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `megham-0.6.1/README.md` & `megham-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `megham-0.6.1/megham/mds.py` & `megham-0.7.0/megham/mds.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,39 +2,20 @@
 Functions for doing multidimensional scaling.
 """
 import logging
 from typing import Callable, Optional
 
 import numpy as np
 import scipy.optimize as opt
-import scipy.spatial.distance as dist
 from numpy.typing import NDArray
 from sklearn.isotonic import IsotonicRegression
 
-logger = logging.getLogger(__name__)
-
-
-def make_edm(coords: NDArray[np.floating]) -> NDArray[np.floating]:
-    """
-    Make an Euclidean distance matrix from a set of points.
+from megham.utils import make_edm
 
-    Parameters
-    ----------
-    coords : NDArray[np.floating]
-        The (npoint, ndim) array of input points.
-
-    Returns
-    -------
-    edm : NDArray[np.floating]
-        The (npoint, npoint) euclidean distance matrix.
-    """
-    dist_vec = dist.pdist(coords)
-    edm = dist.squareform(dist_vec)
-
-    return edm
+logger = logging.getLogger(__name__)
 
 
 def classic_mds(
     distance_matrix: NDArray[np.floating], ndim: int = 3
 ) -> NDArray[np.floating]:
     """
     Perform classical (Torgerson) MDS. This assumes a complete euclidean distance matrix.
```

### Comparing `megham-0.6.1/megham/transform.py` & `megham-0.7.0/megham/transform.py`

 * *Files identical despite different names*

### Comparing `megham-0.6.1/megham.egg-info/PKG-INFO` & `megham-0.7.0/megham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: megham
-Version: 0.6.1
+Version: 0.7.0
 Summary: Tools for working with point clouds
 Author: Saianeesh Keshav Haridas
 License: GPLv3
 Keywords: point cloud,affine,rotations,mds,multidimensional scaling,point set registration,cpd,coherent point drift,mpd,guassian mixture model
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `megham-0.6.1/pyproject.toml` & `megham-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "megham"
-version = "0.6.1"
+version = "0.7.0"
 authors = [{name="Saianeesh Keshav Haridas"}]
 description = "Tools for working with point clouds"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["point cloud", "affine", "rotations", "mds", "multidimensional scaling", "point set registration", "cpd", "coherent point drift", "mpd", "guassian mixture model"]
 license = {text = "GPLv3"}
 classifiers = [ "Programming Language :: Python" ]
```

