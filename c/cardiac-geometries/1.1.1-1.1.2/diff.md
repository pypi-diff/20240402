# Comparing `tmp/cardiac_geometries-1.1.1.tar.gz` & `tmp/cardiac_geometries-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardiac_geometries-1.1.1.tar", last modified: Sat Mar 30 10:11:48 2024, max compression
+gzip compressed data, was "cardiac_geometries-1.1.2.tar", last modified: Tue Apr  2 19:43:46 2024, max compression
```

## Comparing `cardiac_geometries-1.1.1.tar` & `cardiac_geometries-1.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 10:11:48.531957 cardiac_geometries-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1072 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3096 2024-03-30 10:11:48.531957 cardiac_geometries-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1730 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)     2983 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-30 10:11:48.531957 cardiac_geometries-1.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 10:11:48.523957 cardiac_geometries-1.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 10:11:48.527957 cardiac_geometries-1.1.1/src/cardiac_geometries/
--rw-r--r--   0 root         (0) root         (0)     1508 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/__main__.py
--rw-r--r--   0 root         (0) root         (0)      620 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/_import_checks.py
--rw-r--r--   0 root         (0) root         (0)    27628 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/_mesh.py
--rw-r--r--   0 root         (0) root         (0)     4247 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/aha.py
--rw-r--r--   0 root         (0) root         (0)     4165 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/calculus.py
--rw-r--r--   0 root         (0) root         (0)    23522 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/cli.py
--rw-r--r--   0 root         (0) root         (0)     5070 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/dolfin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 10:11:48.527957 cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/
--rw-r--r--   0 root         (0) root         (0)      133 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4517 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     6592 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py
--rw-r--r--   0 root         (0) root         (0)     5783 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/_slab.py
--rw-r--r--   0 root         (0) root         (0)     2104 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/_utils.py
--rw-r--r--   0 root         (0) root         (0)    16869 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/geometry.py
--rw-r--r--   0 root         (0) root         (0)      254 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/utils.py
--rw-r--r--   0 root         (0) root         (0)    10038 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/src/cardiac_geometries/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 10:11:48.531957 cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3096 2024-03-30 10:11:48.000000 cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      986 2024-03-30 10:11:48.000000 cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-30 10:11:48.000000 cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2024-03-30 10:11:48.000000 cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-30 10:11:40.000000 cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      234 2024-03-30 10:11:48.000000 cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-30 10:11:48.000000 cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 10:11:48.531957 cardiac_geometries-1.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)     3396 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     4553 2024-03-30 10:11:38.000000 cardiac_geometries-1.1.1/tests/test_geometry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.004398 cardiac_geometries-1.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.008398 cardiac_geometries-1.1.2/src/cardiac_geometries/
+-rw-r--r--   0 root         (0) root         (0)     1650 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/_import_checks.py
+-rw-r--r--   0 root         (0) root         (0)    28768 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/aha.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/calculus.py
+-rw-r--r--   0 root         (0) root         (0)    23522 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/cli.py
+-rw-r--r--   0 root         (0) root         (0)     5070 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/dolfin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/
+-rw-r--r--   0 root         (0) root         (0)      133 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4517 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_biv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     6592 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_lv_ellipsoid.py
+-rw-r--r--   0 root         (0) root         (0)     5783 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_slab.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_utils.py
+-rw-r--r--   0 root         (0) root         (0)    16869 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/utils.py
+-rw-r--r--   0 root         (0) root         (0)    10038 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/src/cardiac_geometries/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3096 2024-04-02 19:43:45.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-02 19:43:46.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 19:43:45.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-04-02 19:43:46.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 19:43:36.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-02 19:43:46.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-02 19:43:46.000000 cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 19:43:46.012398 cardiac_geometries-1.1.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     3396 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2024-04-02 19:43:34.000000 cardiac_geometries-1.1.2/tests/test_geometry.py
```

### Comparing `cardiac_geometries-1.1.1/LICENSE` & `cardiac_geometries-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/PKG-INFO` & `cardiac_geometries-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac_geometries
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python library for cardiac geometries
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://github.com/ComputationalPhysiology/cardiac_geometries
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cardiac_geometries-1.1.1/README.md` & `cardiac_geometries-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/pyproject.toml` & `cardiac_geometries-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cardiac_geometries"
-version = "1.1.1"
+version = "1.1.2"
 description = "A python library for cardiac geometries"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -136,14 +136,14 @@
 allow_dirty = false
 commit = true
 message = "Bump version: {current_version} → {new_version}"
 tag = true
 sign_tags = false
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
-current_version = "1.1.1"
+current_version = "1.1.2"
 
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/__init__.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,24 +19,26 @@
     from .aha import lv_aha, biv_aha
     from . import _mesh as mesh
     from ._mesh import (
         create_biv_ellipsoid,
         create_lv_ellipsoid,
         create_slab,
         create_biv_ellipsoid_torso,
+        create_benchmark_geometry_land15,
     )
 else:
     gmsh2dolfin = None  # type: ignore
     slab_fibers = None  # type: ignore
     lv_ellipsoid_fibers = None  # type:ignore
     biv_ellipsoid_fibers = None  # type: ignore
     create_biv_ellipsoid = None  # type: ignore
     create_lv_ellipsoid = None  # type: ignore
     create_slab = None  # type: ignore
     create_biv_ellipsoid_torso = None  # type: ignore
+    create_benchmark_geometry_land15 = None  # type: ignore
     lv_aha = None  # type: ignore
     biv_aha = None  # type: ignore
 
 
 __all__ = [
     "has_dolfin",
     "has_gmsh",
@@ -51,8 +53,9 @@
     "create_biv_ellipsoid",
     "create_biv_ellipsoid_torso",
     "create_lv_ellipsoid",
     "create_slab",
     "mesh",
     "lv_aha",
     "biv_aha",
+    "create_benchmark_geometry_land15",
 ]
```

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/_import_checks.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/_import_checks.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/_mesh.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/_mesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -592,15 +592,19 @@
 
     with open(outdir / "markers.json", "w") as f:
         json.dump(geometry.markers, f, default=json_serial)
 
     if create_fibers:
         from .fibers._lv_ellipsoid import create_microstructure
 
-        ffun = geometry.marker_functions.efun if axisymmetric else geometry.marker_functions.ffun
+        ffun = (
+            geometry.marker_functions.efun
+            if axisymmetric
+            else geometry.marker_functions.ffun
+        )
         create_microstructure(
             mesh=geometry.mesh,
             ffun=ffun,
             markers=geometry.markers,
             function_space=fiber_space,
             r_short_endo=r_short_endo,
             r_short_epi=r_short_epi,
@@ -622,14 +626,52 @@
 
     if _tmpfile is not None:
         _tmpfile.__exit__(None, None, None)
 
     return geo
 
 
+def create_benchmark_geometry_land15(
+    outdir: Optional[Union[Path, str]] = None,
+    psize: float = 3.0,
+    ndiv: float = 1.0,
+    axisymmetric: bool = False,
+    fiber_space: str = "Quadrature_4",
+):
+    r_short_endo = 7.0
+    r_short_epi = 10.0
+    r_long_endo = 17.0
+    r_long_epi = 20.0
+    quota_base = 5.0
+    fiber_angle_endo = 90
+    fiber_angle_epi = -90
+
+    mu_base_endo = -math.acos(quota_base / r_long_endo)
+    mu_base_epi = -math.acos(quota_base / r_long_epi)
+    mu_apex_endo = mu_apex_epi = -math.pi
+    psize_ref = psize / ndiv
+    return create_lv_ellipsoid(
+        outdir=outdir,
+        r_short_endo=r_short_endo,
+        r_short_epi=r_short_epi,
+        r_long_endo=r_long_endo,
+        r_long_epi=r_long_epi,
+        mu_base_endo=mu_base_endo,
+        mu_base_epi=mu_base_epi,
+        mu_apex_endo=mu_apex_endo,
+        mu_apex_epi=mu_apex_epi,
+        psize_ref=psize_ref,
+        create_fibers=True,
+        fiber_angle_endo=fiber_angle_endo,
+        fiber_angle_epi=fiber_angle_epi,
+        fiber_space=fiber_space,
+        axisymmetric=axisymmetric,
+    )
+
+
 def create_slab(
     outdir: Optional[Union[Path, str]] = None,
     lx: float = 20.0,
     ly: float = 7.0,
     lz: float = 3.0,
     dx: float = 1.0,
     create_fibers: bool = True,
```

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/aha.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/aha.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/calculus.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/calculus.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/cli.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/cli.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/dolfin_utils.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/dolfin_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/_biv_ellipsoid.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_biv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/_lv_ellipsoid.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_lv_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/_slab.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_slab.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/fibers/_utils.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/fibers/_utils.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/geometry.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/geometry.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries/viz.py` & `cardiac_geometries-1.1.2/src/cardiac_geometries/viz.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/PKG-INFO` & `cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardiac_geometries
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python library for cardiac geometries
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://github.com/ComputationalPhysiology/cardiac_geometries
 Keywords: cardiac,geometry,mesh,gmsh
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cardiac_geometries-1.1.1/src/cardiac_geometries.egg-info/SOURCES.txt` & `cardiac_geometries-1.1.2/src/cardiac_geometries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/tests/test_cli.py` & `cardiac_geometries-1.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `cardiac_geometries-1.1.1/tests/test_geometry.py` & `cardiac_geometries-1.1.2/tests/test_geometry.py`

 * *Files identical despite different names*

