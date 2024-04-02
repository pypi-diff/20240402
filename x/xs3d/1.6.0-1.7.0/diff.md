# Comparing `tmp/xs3d-1.6.0.tar.gz` & `tmp/xs3d-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xs3d-1.6.0.tar", last modified: Wed Feb 21 22:41:12 2024, max compression
+gzip compressed data, was "xs3d-1.7.0.tar", last modified: Tue Apr  2 05:00:12 2024, max compression
```

## Comparing `xs3d-1.6.0.tar` & `xs3d-1.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-21 22:41:12.818468 xs3d-1.6.0/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-21 22:41:12.811201 xs3d-1.6.0/.github/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-21 22:41:12.814969 xs3d-1.6.0/.github/workflows/
--rw-r--r--   0 wms        (501) staff       (20)     1075 2024-02-21 18:59:31.000000 xs3d-1.6.0/.github/workflows/build_wheel.yml
--rw-r--r--   0 wms        (501) staff       (20)      926 2024-02-21 18:59:07.000000 xs3d-1.6.0/.github/workflows/tests.yml
--rw-r--r--   0 wms        (501) staff       (20)       52 2024-02-21 22:41:12.000000 xs3d-1.6.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)     4694 2024-02-21 22:41:12.000000 xs3d-1.6.0/ChangeLog
--rw-r--r--   0 wms        (501) staff       (20)    35149 2024-01-23 23:28:25.000000 xs3d-1.6.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       39 2024-01-28 04:58:07.000000 xs3d-1.6.0/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)     3921 2024-02-21 22:41:12.818366 xs3d-1.6.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)     2936 2024-02-21 19:00:51.000000 xs3d-1.6.0/README.md
--rw-r--r--   0 wms        (501) staff       (20)    11810 2024-02-21 19:00:37.000000 xs3d-1.6.0/automated_test.py
--rw-r--r--   0 wms        (501) staff       (20)      124 2024-02-21 18:59:07.000000 xs3d-1.6.0/pyproject.toml
--rw-r--r--   0 wms        (501) staff       (20)     1041 2024-02-21 22:41:12.818893 xs3d-1.6.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)      612 2024-02-21 18:59:07.000000 xs3d-1.6.0/setup.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-21 22:41:12.815585 xs3d-1.6.0/src/
--rw-r--r--   0 wms        (501) staff       (20)     4564 2024-02-21 19:00:51.000000 xs3d-1.6.0/src/fastxs3d.cpp
--rw-r--r--   0 wms        (501) staff       (20)    19535 2024-02-21 19:00:51.000000 xs3d-1.6.0/src/xs3d.hpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-21 22:41:12.816452 xs3d-1.6.0/xs3d/
--rw-r--r--   0 wms        (501) staff       (20)     5840 2024-02-21 19:00:37.000000 xs3d-1.6.0/xs3d/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)     3396 2024-02-21 19:00:37.000000 xs3d-1.6.0/xs3d/twod.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-21 22:41:12.818001 xs3d-1.6.0/xs3d.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)     3921 2024-02-21 22:41:12.000000 xs3d-1.6.0/xs3d.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      383 2024-02-21 22:41:12.000000 xs3d-1.6.0/xs3d.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2024-02-21 22:41:12.000000 xs3d-1.6.0/xs3d.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2024-01-26 22:08:11.000000 xs3d-1.6.0/xs3d.egg-info/not-zip-safe
--rw-r--r--   0 wms        (501) staff       (20)       46 2024-02-21 22:41:12.000000 xs3d-1.6.0/xs3d.egg-info/pbr.json
--rw-r--r--   0 wms        (501) staff       (20)       14 2024-02-21 22:41:12.000000 xs3d-1.6.0/xs3d.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-04-02 05:00:12.660604 xs3d-1.7.0/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-04-02 05:00:12.652896 xs3d-1.7.0/.github/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-04-02 05:00:12.656572 xs3d-1.7.0/.github/workflows/
+-rw-r--r--   0 wms        (501) staff       (20)     1075 2024-02-21 18:59:31.000000 xs3d-1.7.0/.github/workflows/build_wheel.yml
+-rw-r--r--   0 wms        (501) staff       (20)      926 2024-02-21 18:59:07.000000 xs3d-1.7.0/.github/workflows/tests.yml
+-rw-r--r--   0 wms        (501) staff       (20)       52 2024-04-02 05:00:12.000000 xs3d-1.7.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)     4810 2024-04-02 05:00:12.000000 xs3d-1.7.0/ChangeLog
+-rw-r--r--   0 wms        (501) staff       (20)    35149 2024-01-23 23:28:25.000000 xs3d-1.7.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       39 2024-01-28 04:58:07.000000 xs3d-1.7.0/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)     3921 2024-04-02 05:00:12.660500 xs3d-1.7.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)     2936 2024-02-21 19:00:51.000000 xs3d-1.7.0/README.md
+-rw-r--r--   0 wms        (501) staff       (20)    11810 2024-03-04 23:44:46.000000 xs3d-1.7.0/automated_test.py
+-rw-r--r--   0 wms        (501) staff       (20)      124 2024-02-21 18:59:07.000000 xs3d-1.7.0/pyproject.toml
+-rw-r--r--   0 wms        (501) staff       (20)     1041 2024-04-02 05:00:12.661038 xs3d-1.7.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)      612 2024-02-21 18:59:07.000000 xs3d-1.7.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-04-02 05:00:12.657259 xs3d-1.7.0/src/
+-rw-r--r--   0 wms        (501) staff       (20)     4617 2024-03-13 04:54:31.000000 xs3d-1.7.0/src/fastxs3d.cpp
+-rw-r--r--   0 wms        (501) staff       (20)    19687 2024-03-13 04:54:30.000000 xs3d-1.7.0/src/xs3d.hpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-04-02 05:00:12.658235 xs3d-1.7.0/xs3d/
+-rw-r--r--   0 wms        (501) staff       (20)     6454 2024-03-13 04:49:23.000000 xs3d-1.7.0/xs3d/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)     3396 2024-02-21 19:00:37.000000 xs3d-1.7.0/xs3d/twod.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-04-02 05:00:12.660081 xs3d-1.7.0/xs3d.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)     3921 2024-04-02 05:00:12.000000 xs3d-1.7.0/xs3d.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      383 2024-04-02 05:00:12.000000 xs3d-1.7.0/xs3d.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2024-04-02 05:00:12.000000 xs3d-1.7.0/xs3d.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2024-01-26 22:08:11.000000 xs3d-1.7.0/xs3d.egg-info/not-zip-safe
+-rw-r--r--   0 wms        (501) staff       (20)       46 2024-04-02 05:00:12.000000 xs3d-1.7.0/xs3d.egg-info/pbr.json
+-rw-r--r--   0 wms        (501) staff       (20)       14 2024-04-02 05:00:12.000000 xs3d-1.7.0/xs3d.egg-info/top_level.txt
```

### Comparing `xs3d-1.6.0/.github/workflows/build_wheel.yml` & `xs3d-1.7.0/.github/workflows/build_wheel.yml`

 * *Files identical despite different names*

### Comparing `xs3d-1.6.0/.github/workflows/tests.yml` & `xs3d-1.7.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `xs3d-1.6.0/ChangeLog` & `xs3d-1.7.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+1.7.0
+-----
+
+* feat: add return\_contact feature to cross\_section
+* fix: cross\_section array order was incorrect
+
 1.6.0
 -----
 
 * perf: lift repetitive calculations out of check\_intersections
 * perf: pre-calculate inverses
 * perf: lift max distance to plane to constexpr
 * perf: convert /2 into \*0.5
```

### Comparing `xs3d-1.6.0/LICENSE` & `xs3d-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xs3d-1.6.0/PKG-INFO` & `xs3d-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xs3d
-Version: 1.6.0
+Version: 1.7.0
 Summary: Compute cross sectional area of 3d shapes.
 Home-page: https://github.com/seung-lab/igneous/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xs3d-1.6.0/README.md` & `xs3d-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `xs3d-1.6.0/automated_test.py` & `xs3d-1.7.0/automated_test.py`

 * *Files identical despite different names*

### Comparing `xs3d-1.6.0/setup.cfg` & `xs3d-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `xs3d-1.6.0/setup.py` & `xs3d-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `xs3d-1.6.0/src/fastxs3d.cpp` & `xs3d-1.7.0/src/fastxs3d.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 		: binimg.shape()[1];
 	const uint64_t sz = binimg.ndim() < 3 
 		? 1 
 		: binimg.shape()[2];
 
 	const uint64_t voxels = sx * sy * sz;
 
-	py::array_t arr = py::array_t<float, py::array::f_style>(voxels);
+	py::array_t arr = py::array_t<float, py::array::f_style>({ sx, sy, sz });
     float* data = static_cast<float*>(arr.request().ptr);
     std::fill(data, data + voxels, 0.0f);
 
-	xs3d::cross_section(
+	std::tuple<float*, uint8_t> tup = xs3d::cross_section(
 		binimg.data(),
 		sx, sy, sz,
 		point.at(0), point.at(1), point.at(2),
 		normal.at(0), normal.at(1), normal.at(2),
 		anisotropy.at(0), anisotropy.at(1), anisotropy.at(2),
 		data
 	);
 
-	return arr.reshape({ sx, sy, sz });
+	return std::make_tuple(arr, std::get<1>(tup));
 }
 
 auto area(
 	const py::array_t<uint8_t> &binimg,
 	const py::array_t<float> &point,
 	const py::array_t<float> &normal,
 	const py::array_t<float> &anisotropy
```

### Comparing `xs3d-1.6.0/src/xs3d.hpp` & `xs3d-1.7.0/src/xs3d.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -661,60 +661,61 @@
 		binimg, 
 		sx, sy, sz, 
 		pos, normal, anisotropy,
 		contact, /*plane_visualization=*/NULL
 	);
 }
 
-float* cross_section(
+std::tuple<float*, uint8_t> cross_section(
 	const uint8_t* binimg,
 	const uint64_t sx, const uint64_t sy, const uint64_t sz,
 	
 	const float px, const float py, const float pz,
 	const float nx, const float ny, const float nz,
 	const float wx, const float wy, const float wz,
 	float* plane_visualization = NULL
 ) {
 	if (plane_visualization == NULL) {
 		plane_visualization = new float[sx * sy * sz]();
 	}
 
+	uint8_t contact = 0;
+
 	if (px < 0 || px >= sx) {
-		return plane_visualization;
+		return std::make_tuple(plane_visualization, contact);
 	}
 	else if (py < 0 || py >= sy) {
-		return plane_visualization;
+		return std::make_tuple(plane_visualization, contact);
 	}
 	else if (pz < 0 || pz >= sz) {
-		return plane_visualization;
+		return std::make_tuple(plane_visualization, contact);
 	}
 
 	uint64_t loc = static_cast<uint64_t>(px) + sx * (
 		static_cast<uint64_t>(py) + sy * static_cast<uint64_t>(pz)
 	);
 
 	if (!binimg[loc]) {
-		return plane_visualization;
+		return std::make_tuple(plane_visualization, contact);
 	}
 
 	const Vec3 pos(px, py, pz);
 	const Vec3 anisotropy(wx, wy, wz);
 	Vec3 normal(nx, ny, nz);
 	normal /= normal.norm();
 
-	uint8_t contact = 0;
 
 	cross_sectional_area_helper(
 		binimg, 
 		sx, sy, sz, 
 		pos, normal, anisotropy,
 		contact, plane_visualization
 	);
 
-	return plane_visualization;
+	return std::make_tuple(plane_visualization, contact);
 }
 
 std::tuple<Vec3, Vec3> create_orthonormal_basis(
 	const Vec3& normal, const bool positive_basis
 ) {
 	Vec3 basis1 = normal.cross(jhat);
 	if (basis1.is_null()) {
```

### Comparing `xs3d-1.6.0/xs3d/__init__.py` & `xs3d-1.7.0/xs3d/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     return area
 
 def cross_section(
   binimg:np.ndarray,
   pos:Sequence[int],
   normal:Sequence[float],
   anisotropy:Optional[Sequence[float]] = None,
+  return_contact:bool = False,
 ) -> np.ndarray:
   """
   Compute which voxels are intercepted by a section plane
   (defined by a normal vector).
 
   binimg: a binary 2d or 3d numpy image (e.g. a bool datatype)
   pos: the point in the image from which to extract the section
@@ -87,14 +88,25 @@
     e.g. [5,10,2]
   normal: a vector normal to the section plane, does not
     need to be a unit vector. e.g. [sqrt(2)/2. sqrt(2)/2, 0]
   anisotropy: resolution of the x, y, and z axis
     e.g. [4,4,40] for an electron microscope image with 
     4nm XY resolution with a 40nm cutting plane in 
     serial sectioning.
+  return_contact: if true, return a tuple of (area, contact)
+    where area is the usual output and contact is non-zero if
+    the section plane has contacted the edge of the image
+    indicating the area may be an underestimate if you are
+    working with a cutout of a larger image.
+
+    Contact is an 8-bit bitfield that represents which image faces
+    have been touched. The bits are organized as follows.
+
+    0: 0 X     2: 0 Y     4: 0 Z      6: Unused
+    1: Max X   3: Max Y   5: Max Z    7: Unused
 
   Returns: float32 volume where each voxel's value is its
     contribution to the cross sectional area
   """
   if anisotropy is None:
     anisotropy = [ 1.0 ] * binimg.ndim
 
@@ -109,18 +121,23 @@
     raise ValueError(f"anisotropy values must be > 0. Got: {anisotropy}")
 
   if np.all(normal == 0):
     raise ValueError("normal vector must not be a null vector (all zeros).")
 
   binimg = np.asfortranarray(binimg)
 
-  if binimg.ndim == 3:
-    return fastxs3d.section(binimg, pos, normal, anisotropy)
-  else:
+  if binimg.ndim != 3:
     raise ValueError("dimensions not supported")
+  
+  section, contact = fastxs3d.section(binimg, pos, normal, anisotropy)
+
+  if return_contact:
+    return (section, contact)
+
+  return section
 
 def slice(
   labels:np.ndarray,
   pos:Sequence[int],
   normal:Sequence[float],
   anisotropy:Optional[Sequence[float]] = None,
   standardize_basis:bool = True,
```

### Comparing `xs3d-1.6.0/xs3d/twod.py` & `xs3d-1.7.0/xs3d/twod.py`

 * *Files identical despite different names*

### Comparing `xs3d-1.6.0/xs3d.egg-info/PKG-INFO` & `xs3d-1.7.0/xs3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xs3d
-Version: 1.6.0
+Version: 1.7.0
 Summary: Compute cross sectional area of 3d shapes.
 Home-page: https://github.com/seung-lab/igneous/
 Author: William Silversmith
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

