# Comparing `tmp/rportion-0.1.0.tar.gz` & `tmp/rportion-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rportion-0.1.0.tar", last modified: Tue Aug 16 20:37:22 2022, max compression
+gzip compressed data, was "rportion-0.2.0.tar", last modified: Tue Apr  2 12:25:08 2024, max compression
```

## Comparing `rportion-0.1.0.tar` & `rportion-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 20:37:22.021730 rportion-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-16 20:37:10.000000 rportion-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    14379 2022-08-16 20:37:22.021730 rportion-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13682 2022-08-16 20:37:10.000000 rportion-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-08-16 20:37:10.000000 rportion-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 20:37:22.021730 rportion-0.1.0/rportion/
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-08-16 20:37:10.000000 rportion-0.1.0/rportion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29623 2022-08-16 20:37:10.000000 rportion-0.1.0/rportion/rportion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 20:37:22.021730 rportion-0.1.0/rportion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14379 2022-08-16 20:37:22.000000 rportion-0.1.0/rportion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-08-16 20:37:22.000000 rportion-0.1.0/rportion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 20:37:22.000000 rportion-0.1.0/rportion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-08-16 20:37:22.000000 rportion-0.1.0/rportion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-16 20:37:22.000000 rportion-0.1.0/rportion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-16 20:37:22.021730 rportion-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-08-16 20:37:10.000000 rportion-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:25:08.715484 rportion-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-02 12:24:59.000000 rportion-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-04-02 12:25:08.715484 rportion-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-04-02 12:24:59.000000 rportion-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 12:24:59.000000 rportion-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:25:08.711484 rportion-0.2.0/rportion/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-02 12:24:59.000000 rportion-0.2.0/rportion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29733 2024-04-02 12:24:59.000000 rportion-0.2.0/rportion/rportion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:25:08.711484 rportion-0.2.0/rportion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14700 2024-04-02 12:25:08.000000 rportion-0.2.0/rportion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-02 12:25:08.000000 rportion-0.2.0/rportion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:25:08.000000 rportion-0.2.0/rportion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 12:25:08.000000 rportion-0.2.0/rportion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 12:25:08.000000 rportion-0.2.0/rportion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:25:08.715484 rportion-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-02 12:24:59.000000 rportion-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:25:08.711484 rportion-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    43803 2024-04-02 12:24:59.000000 rportion-0.2.0/tests/test_rportion.py
```

### Comparing `rportion-0.1.0/LICENSE` & `rportion-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rportion-0.1.0/PKG-INFO` & `rportion-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: rportion
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python data structure and operations for 2-dimensional rectilinear polygons
 Home-page: https://github.com/tilmann-bartsch/rportion
 Author: Tilmann Bartsch
 License: MIT
 Keywords: rectangle polygon interval-tree
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Requires-Python: ~= 3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sortedcontainers~=2.2
+Requires-Dist: portion~=2.4.2
 Provides-Extra: test
+Requires-Dist: pytest~=7.0; extra == "test"
+Requires-Dist: coverage~=6.0; extra == "test"
+Requires-Dist: numpy~=1.26.4; extra == "test"
 Provides-Extra: docu
-License-File: LICENSE
+Requires-Dist: numpy~=1.26.4; extra == "docu"
+Requires-Dist: matplotlib~=3.5.2; extra == "docu"
+Requires-Dist: imageio~=2.19.5; extra == "docu"
+Requires-Dist: pillow~=9.2.0; extra == "docu"
+Requires-Dist: tqdm~=4.64.0; extra == "docu"
 
 # rportion - data structure and operations for rectilinear polygons
 
 
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pytest-codeblocks.svg?branch=master)](https://test.pypi.org/project/rportion/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/rportion)](https://pypi.org/project/rportion/)
 [![Tests](https://github.com/tilmann-bartsch/rportion/actions/workflows/test.yaml/badge.svg?branch=master)](https://github.com/tilmann-bartsch/portion/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/tilmann-bartsch/rportion/badge.svg?branch=master)](https://coveralls.io/github/tilmann-bartsch/rportion?branch=master)
-[![LGTM](https://img.shields.io/lgtm/grade/python/github/tilmann-bartsch/rportion.svg?branch=master)](https://lgtm.com/projects/g/tilmann-bartsch/rportion)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Commits](https://img.shields.io/github/last-commit/tilmann-bartsch/rportion/master)](https://github.com/tilmann-bartsch/rportion/commits/master)
 
 The `rportion` library provides data structure to represent 
-2D [rectilinear polygons](https://en.wikipedia.org/wiki/Rectilinear_polygon) (unions of 2D-intervals) in Python 3.7+.
+2D [rectilinear polygons](https://en.wikipedia.org/wiki/Rectilinear_polygon) (unions of 2D-intervals) in Python 3.9+.
 It is built upon the library [`portion`](https://github.com/AlexandreDecan/portion) and follows its concepts.
 The following features are provided:
 
  - 2D-Intervals (rectangles) which can be open/closed and finite/infinite at every boundary
  - intersection, union, complement and difference of rectilinear polygons
  - iterator over all maximum rectangles inside and outside a given polygon
 
@@ -50,27 +59,37 @@
 
   * [Installation](#installation)
   * [Documentation & usage](#documentation--usage)
       * [Polygon creation](#polygon-creation)
       * [Polygon bounds & attributes](#polygon-bounds--attributes)
       * [Polygon operations](#polygon-operations)
       * [Rectangle partitioning iterator](#rectangle-partitioning-iterator)
-      * [Maximum rectangle iterator](#maximum-rectangle-iterators)
+      * [Maximum rectangle iterator](#maximum-rectangle-iterator)
       * [Boundary](#boundary)
       * [Internal data structure](#internal-data-structure)
   * [Changelog](#changelog)
   * [Contributions](#contributions)
   * [License](#license)
 
 ## Installation
 
-Install `rportion` from [PyPi-test](https://test.pypi.org/project/rportion/) with `pip` using 
-`pip install -i https://test.pypi.org/simple/ rportion`.
+`rportion` can be installed from [PyPi](https://pypi.org/project/rportion/) with `pip` using 
 
-Install `rportion` with the development environment using `pip install -e ".[test]"`.
+```bash
+pip install rportion
+```
+
+Alternatively, clone the repository and run
+
+```bash
+pip install -e ".[test]"
+python -m unittest discover -s tests
+```
+
+Note that `python
 
 ## Documentation & usage
 
 ### Polygon creation
 
 Atomic polygons (rectangles) can be created by one of the following:
 ```python
@@ -152,14 +171,16 @@
     the polygon.
     ```python
     >>> p = rp.rclosedopen(0, 2, 1, 3)
     >>> p.x_left, p.x_right, p.y_left, p.y_right
     (CLOSED, OPEN, CLOSED, OPEN)
     ```
 
+
+[&uparrow; back to top](#table-of-contents)
 ### Polygon operations
 
 `RPolygon` instances support the following operations:
  - `p.intersection(other)` and `p & other` return the intersection of two rectilinear polygons.
    ```python
    >>> rp.rclosed(0, 2, 0, 2) & rp.rclosed(1, 3, 0, 1)
    (x=[1,2], y=[0,1])
```

### Comparing `rportion-0.1.0/README.md` & `rportion-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # rportion - data structure and operations for rectilinear polygons
 
 
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pytest-codeblocks.svg?branch=master)](https://test.pypi.org/project/rportion/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/rportion)](https://pypi.org/project/rportion/)
 [![Tests](https://github.com/tilmann-bartsch/rportion/actions/workflows/test.yaml/badge.svg?branch=master)](https://github.com/tilmann-bartsch/portion/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/tilmann-bartsch/rportion/badge.svg?branch=master)](https://coveralls.io/github/tilmann-bartsch/rportion?branch=master)
-[![LGTM](https://img.shields.io/lgtm/grade/python/github/tilmann-bartsch/rportion.svg?branch=master)](https://lgtm.com/projects/g/tilmann-bartsch/rportion)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Commits](https://img.shields.io/github/last-commit/tilmann-bartsch/rportion/master)](https://github.com/tilmann-bartsch/rportion/commits/master)
 
 The `rportion` library provides data structure to represent 
-2D [rectilinear polygons](https://en.wikipedia.org/wiki/Rectilinear_polygon) (unions of 2D-intervals) in Python 3.7+.
+2D [rectilinear polygons](https://en.wikipedia.org/wiki/Rectilinear_polygon) (unions of 2D-intervals) in Python 3.9+.
 It is built upon the library [`portion`](https://github.com/AlexandreDecan/portion) and follows its concepts.
 The following features are provided:
 
  - 2D-Intervals (rectangles) which can be open/closed and finite/infinite at every boundary
  - intersection, union, complement and difference of rectilinear polygons
  - iterator over all maximum rectangles inside and outside a given polygon
 
@@ -30,27 +29,37 @@
 
   * [Installation](#installation)
   * [Documentation & usage](#documentation--usage)
       * [Polygon creation](#polygon-creation)
       * [Polygon bounds & attributes](#polygon-bounds--attributes)
       * [Polygon operations](#polygon-operations)
       * [Rectangle partitioning iterator](#rectangle-partitioning-iterator)
-      * [Maximum rectangle iterator](#maximum-rectangle-iterators)
+      * [Maximum rectangle iterator](#maximum-rectangle-iterator)
       * [Boundary](#boundary)
       * [Internal data structure](#internal-data-structure)
   * [Changelog](#changelog)
   * [Contributions](#contributions)
   * [License](#license)
 
 ## Installation
 
-Install `rportion` from [PyPi-test](https://test.pypi.org/project/rportion/) with `pip` using 
-`pip install -i https://test.pypi.org/simple/ rportion`.
+`rportion` can be installed from [PyPi](https://pypi.org/project/rportion/) with `pip` using 
 
-Install `rportion` with the development environment using `pip install -e ".[test]"`.
+```bash
+pip install rportion
+```
+
+Alternatively, clone the repository and run
+
+```bash
+pip install -e ".[test]"
+python -m unittest discover -s tests
+```
+
+Note that `python
 
 ## Documentation & usage
 
 ### Polygon creation
 
 Atomic polygons (rectangles) can be created by one of the following:
 ```python
@@ -132,14 +141,16 @@
     the polygon.
     ```python
     >>> p = rp.rclosedopen(0, 2, 1, 3)
     >>> p.x_left, p.x_right, p.y_left, p.y_right
     (CLOSED, OPEN, CLOSED, OPEN)
     ```
 
+
+[&uparrow; back to top](#table-of-contents)
 ### Polygon operations
 
 `RPolygon` instances support the following operations:
  - `p.intersection(other)` and `p & other` return the intersection of two rectilinear polygons.
    ```python
    >>> rp.rclosed(0, 2, 0, 2) & rp.rclosed(1, 3, 0, 1)
    (x=[1,2], y=[0,1])
```

### Comparing `rportion-0.1.0/rportion/rportion.py` & `rportion-0.2.0/rportion/rportion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from copy import copy
 from typing import Iterator, List, Tuple, Callable
 
 import portion as P
-from portion.interval import Interval, open, empty, closedopen, closed, openclosed, singleton
 from sortedcontainers import SortedList
 
 
-def _sub_contained_atomics(int_1: Interval, int_2: Interval) -> Interval:
+def _sub_contained_atomics(int_1: P.Interval, int_2: P.Interval) -> P.Interval:
     """
     Remove all atomic sectors from int_1 which are contained completely in int_2, i.e.
 
 
          int_1:     ---     ----
          int_2: ----------    ---------
         return:             ----
     """
-    ret_int = empty()
+    ret_int = P.empty()
     for y_atomic in int_1:
         if not int_2.contains(y_atomic):
             ret_int |= y_atomic
     return ret_int
 
 
 class RBoundary:
@@ -89,32 +88,32 @@
     def __copy__(self):
         return self.__class__(self.val, self.btype)
 
     def __repr__(self):
         return f"({self.val}, {self.btype})"
 
 
-def _extend_ranges_mat(mat: List[List[Interval]],
+def _extend_ranges_mat(mat: List[List[P.Interval]],
                        x_boundaries: 'SortedList[RBoundary]',
                        rbound: RBoundary):
     n = len(mat)
     index = x_boundaries.bisect_right(rbound)
     prev_y_int_row = mat[index - 1]
     mat.insert(index - 1, list(prev_y_int_row))
     for row in range(0, index):
         prev_y_int = mat[row][n - index]
         mat[row].insert(n - index, prev_y_int)
 
 
-def _y_interval_triangle_prunable(bound_index: int, y_interval_triangle: List[List[Interval]]) -> bool:
+def _y_interval_triangle_prunable(bound_index: int, y_interval_triangle: List[List[P.Interval]]) -> bool:
     """
     Test if the given bound can be removed from y_interval_triangle.
 
     :bound_index int:
-    :y_interval_triangle list[list[Interval]]:
+    :y_interval_triangle list[list[P.Interval]]:
     :return bool:
 
     For the following triangle the boundary 4 can be pruned, because
       - the y-intervals of row (Y) are contained in the corresponding
         y-intervals of row (X), and
       - the y-intervals of column (N) are contained in the corresponding
         y-intervals of column (M).
@@ -154,27 +153,27 @@
     for i in rows:
         if not tr[i][j - 1].contains(tr[i][j]):
             return False
 
     return True
 
 
-def _interval_triangle_prunable_indices(y_interval_triangle: List[List[Interval]]) -> List[int]:
+def _interval_triangle_prunable_indices(y_interval_triangle: List[List[P.Interval]]) -> List[int]:
     """Return a list of indices which can be removed from y_interval_triangle."""
     n = len(y_interval_triangle)
     return [b_index for b_index in range(1, n + 1)
             if _y_interval_triangle_prunable(b_index, y_interval_triangle)]
 
 
-def _remove_boundaries(bound_indices: List[int], y_interval_triangle: List[List[Interval]]):
+def _remove_boundaries(bound_indices: List[int], y_interval_triangle: List[List[P.Interval]]):
     """
     Remove rows and columnss from y_interval_triangle specified by bound_indices.
 
     :bound_indices list[int]:
-    :y_interval_triangle list[list[Interval]]: Data
+    :y_interval_triangle list[list[P.Interval]]: Data
 
     This function is meant to be performed if the boundary is prunable, see function
     `_y_interval_triangle_prunable`.
 
     I.e. for bound_indices == [1] we get
 
              old y-interval-triangle                         new y-interval-triangle
@@ -193,28 +192,28 @@
             y_interval_triangle[i].pop(n - bound_index)
         y_interval_triangle.pop(bound_index - n_removed)
         n_removed += 1
 
 
 def _update_x_boundaries_and_y_interval_triangles(
         x_boundaries: 'SortedList[RBoundary]',
-        y_interval_triangle_add: List[List[Interval]],
-        y_interval_triangle_sub: List[List[Interval]],
-        other_x_atom: Interval, other_y_interval: Interval):
+        y_interval_triangle_add: List[List[P.Interval]],
+        y_interval_triangle_sub: List[List[P.Interval]],
+        other_x_atom: P.Interval, other_y_interval: P.Interval):
     """
     Update
        - y_interval_triangle_add
                 such that it represents the union of the old polygon and the one provided as parameters
        - y_interval_triangle_sub
                 such that it represents the difference of the old polygon and the one provided as paramters
 
     :x_boundaries SortedList[RBoundary]:
-    :y_interval_triangle_add list[list[Interval]]:
-    :y_interval_triangle_sub list[list[Interval]]:
-    :new_x_atom Atomic, new_y_interval: Interval:
+    :y_interval_triangle_add list[list[P.Interval]]:
+    :y_interval_triangle_sub list[list[P.Interval]]:
+    :new_x_atom Atomic, new_y_interval: P.Interval:
     """
     assert other_x_atom.atomic
 
     # Left and right boundary of other_x_atom
     l_bound_type = ~other_x_atom.left
     x_b_left = RBoundary(other_x_atom.lower, l_bound_type)
     r_bound_type = other_x_atom.right
@@ -232,53 +231,53 @@
 
     # (b) Update y_interval_triangle_add
     n = len(y_interval_triangle_add)
     for i in range(n):
         for j in range(n - i):
             l_bound = x_boundaries[i]
             r_bound = x_boundaries[-j - 1]
-            x_interval = Interval.from_atomic(~l_bound.btype, l_bound.val, r_bound.val, r_bound.btype)
+            x_interval = P.Interval.from_atomic(~l_bound.btype, l_bound.val, r_bound.val, r_bound.btype)
 
             if other_x_atom.contains(x_interval):
                 y_interval_triangle_add[i][j] |= other_y_interval
             else:
                 adj_other_x_interval = other_x_atom
 
                 other_x_int_l_bound = ~RBoundary(other_x_atom.lower, other_x_atom.left)
                 other_y_int_r_bound = RBoundary(other_x_atom.upper, other_x_atom.right)
 
                 left_ind = x_boundaries.bisect_left(other_x_int_l_bound)
                 col = n - left_ind
                 if l_bound < other_x_int_l_bound and (0 < col < n - i):
-                    adj_other_x_interval |= Interval.from_atomic(~l_bound.btype, l_bound.val,
+                    adj_other_x_interval |= P.Interval.from_atomic(~l_bound.btype, l_bound.val,
                                                                  adj_other_x_interval.upper,
                                                                  adj_other_x_interval.right)
                     y_int_left = y_interval_triangle_add[i][col]
                 else:
-                    y_int_left = open(-P.inf, P.inf)
+                    y_int_left = P.open(-P.inf, P.inf)
 
                 right_ind = x_boundaries.bisect_left(other_y_int_r_bound)
                 if other_y_int_r_bound < r_bound and right_ind < n - j:
-                    adj_other_x_interval |= Interval.from_atomic(adj_other_x_interval.left,
+                    adj_other_x_interval |= P.Interval.from_atomic(adj_other_x_interval.left,
                                                                  adj_other_x_interval.lower,
                                                                  r_bound.val, r_bound.btype)
                     y_int_right = y_interval_triangle_add[right_ind][j]
                 else:
-                    y_int_right = open(-P.inf, P.inf)
+                    y_int_right = P.open(-P.inf, P.inf)
 
                 if adj_other_x_interval.contains(x_interval):
                     y_interval_triangle_add[i][j] |= y_int_left & other_y_interval & y_int_right
 
     # (c) Update y_interval_triangle_sub
     n = len(y_interval_triangle_sub)
     for i in range(n):
         for j in range(n - i):
             l_bound = ~x_boundaries[i]
             r_bound = x_boundaries[-j - 1]
-            x_interval = Interval.from_atomic(l_bound.btype, l_bound.val, r_bound.val, r_bound.btype)
+            x_interval = P.Interval.from_atomic(l_bound.btype, l_bound.val, r_bound.val, r_bound.btype)
             if other_x_atom.overlaps(x_interval):
                 y_interval_triangle_sub[i][j] -= other_y_interval
 
     # (d) Prune the y-interval-triangles if possible
     indices_add = _interval_triangle_prunable_indices(y_interval_triangle_add)
     indices_sub = _interval_triangle_prunable_indices(y_interval_triangle_sub)
     assert indices_add == indices_sub, (
@@ -287,29 +286,29 @@
     _remove_boundaries(indices_add, y_interval_triangle_add)
     _remove_boundaries(indices_add, y_interval_triangle_sub)
     for ind in sorted(indices_add, reverse=True):
         x_boundaries.pop(ind)
 
 
 def _traverse_diagonally(boundaries: List[RBoundary],
-                         interval_triangle: List[List[Interval]],
-                         next_accumulator: Callable[[Interval, Interval, Interval], Interval],
-                         adj_y_interval: Callable[[Interval, Interval, Interval], Interval]
-                         ) -> Iterator[Tuple[Interval, Interval]]:
+                         interval_triangle: List[List[P.Interval]],
+                         next_accumulator: Callable[[P.Interval, P.Interval, P.Interval], P.Interval],
+                         adj_y_interval: Callable[[P.Interval, P.Interval, P.Interval], P.Interval]
+                         ) -> Iterator[Tuple[P.Interval, P.Interval]]:
     """
     Traverse `interval_triangle` diagonally from the top left and yield rectangles specified by the parameters
     `asdf` and `next_accumulator`.
 
     The iterator *DOES NOT* return tuples where either the first or second interval is empty.
 
     :param boundaries: List[RBoundary]:
-    :param interval_triangle: List[List[Interval]]:
-    :param next_accumulator: Callable[[Interval, Interval, Interval], Interval]:
+    :param interval_triangle: List[List[P.Interval]]:
+    :param next_accumulator: Callable[[P.Interval, P.Interval, P.Interval], P.Interval]:
         Function determining how to accumulate values while traversing. See explanation below.
-    :param adj_y_interval: Callable[[Interval, Interval, Interval], Interval]:
+    :param adj_y_interval: Callable[[P.Interval, P.Interval, P.Interval], P.Interval]:
         Function determining which rectangles to return. See explanation below.
 
     `interval_triangle` represents an interval tree of the form
 
                     ┌─x─┐
                   ┌─x─┬─x─┐
                 ┌─x─┬─x─┬─x─┐
@@ -322,34 +321,34 @@
                             to obtain an interval which is the accumulator of this node.
       - `adj_y_interval`:   use the previous accumulators of both parent nodes and the current node value
                             to obtain an adjusted y_interval..
 
     All generated rectangles which are non-empty are returned.
     """
     n = len(interval_triangle)
-    next_parent_y_intervals = [empty(), empty()]
+    next_parent_y_intervals = [P.empty(), P.empty()]
     for start_row in range(n):
         parent_y_intervals = next_parent_y_intervals
-        next_parent_y_intervals = [empty()]
+        next_parent_y_intervals = [P.empty()]
         for row, col in enumerate(range(start_row, -1, -1)):
             curr_y_int = interval_triangle[row][col]
 
             adj_curr_y_int = adj_y_interval(curr_y_int, parent_y_intervals[row], parent_y_intervals[row + 1])
 
             l_bound = ~boundaries[row]
             r_bound = boundaries[-col - 1]
-            curr_x_int = Interval.from_atomic(l_bound.btype, l_bound.val,
+            curr_x_int = P.Interval.from_atomic(l_bound.btype, l_bound.val,
                                               r_bound.val, r_bound.btype)
             if not curr_x_int.empty and not adj_curr_y_int.empty:
                 yield curr_x_int, adj_curr_y_int
 
             next_parent_y_intervals.append(next_accumulator(curr_y_int,
                                                             parent_y_intervals[row],
                                                             parent_y_intervals[row + 1]))
-        next_parent_y_intervals.append(empty())
+        next_parent_y_intervals.append(P.empty())
 
 
 class RPolygon:
     """
     This class represents an orthogonal Polygon.
 
     An orthogonal polygon is a union of rectangles. A rectangle is represented by two
@@ -370,16 +369,16 @@
         #         | inf  bn  ... b2  b1
         #    -----+---------------------
         #    -inf |                 ___/
         #      b1 |             ___/
         #      b2 |         ___/
         #       : |      __/
         #      bn |_____/
-        self._used_y_ranges: List[List[Interval]] = [[empty()]]
-        self._free_y_ranges: List[List[Interval]] = [[open(-P.inf, P.inf)]]
+        self._used_y_ranges: List[List[P.Interval]] = [[P.empty()]]
+        self._free_y_ranges: List[List[P.Interval]] = [[P.open(-P.inf, P.inf)]]
 
     @property
     def x_left(self):
         """
         Lowest left boundary in x-dimension. Equal to either CLOSED or OPEN.
         """
         return self.x_enclosure_interval.left
@@ -452,44 +451,44 @@
             return True
 
     @property
     def enclosure(self) -> 'RPolygon':
         return self.__class__.from_interval_product(self.x_enclosure_interval, self.y_enclosure_interval)
 
     @property
-    def x_enclosure_interval(self) -> Interval:
+    def x_enclosure_interval(self) -> P.Interval:
         """
         smallest y_interval enclosing the y-dimension of the polygon.
         """
         n = len(self._free_y_ranges[0])
         for l_int in range(0, n):
-            if self._free_y_ranges[0][l_int] == open(-P.inf, P.inf):
+            if self._free_y_ranges[0][l_int] == P.open(-P.inf, P.inf):
                 break
         else:
             l_int += 1
         n = len(self._free_y_ranges)
         for r_int in range(0, n):
-            if self._free_y_ranges[r_int][0] == open(-P.inf, P.inf):
+            if self._free_y_ranges[r_int][0] == P.open(-P.inf, P.inf):
                 break
         else:
             r_int += 1
         l_bound = self._x_boundaries[n - l_int]
         r_bound = self._x_boundaries[r_int]
-        return Interval.from_atomic(~l_bound.btype, l_bound.val,
+        return P.Interval.from_atomic(~l_bound.btype, l_bound.val,
                                     r_bound.val, r_bound.btype)
 
     @property
-    def y_enclosure_interval(self) -> Interval:
+    def y_enclosure_interval(self) -> P.Interval:
         """
         smallest y_interval enclosing the y-dimension of the polygon.
         """
         return ~self._free_y_ranges[0][0]
 
     @classmethod
-    def from_interval_product(cls, x_interval: Interval, y_interval: Interval) -> 'RPolygon':
+    def from_interval_product(cls, x_interval: P.Interval, y_interval: P.Interval) -> 'RPolygon':
         """
         Create a (simple) rectangular polygon as the product of two intervals.
 
         :param x_interval:
         :param y_interval:
         :return RPolygon:
         """
@@ -558,37 +557,37 @@
 
     def boundary(self) -> 'RPolygon':
         """
         Return the boundary of this polygon.
 
         :return RPolygon: boundary of this polygon represented as another polygon
         """
-        def adj_y_interval(curr: Interval, l_parent: Interval, r_parent: Interval) -> Interval:
+        def adj_y_interval(curr: P.Interval, l_parent: P.Interval, r_parent: P.Interval) -> P.Interval:
             return curr - l_parent - r_parent
 
         iterator = _traverse_diagonally(list(self._x_boundaries), self._used_y_ranges,
                                         lambda curr, l_parent, r_parent: curr | l_parent | r_parent,
                                         adj_y_interval)
         x_boundary_poly = rempty()
         for x_atom, y_interval in iterator:
-            x_int = singleton(x_atom.lower) | singleton(x_atom.upper)
+            x_int = P.singleton(x_atom.lower) | P.singleton(x_atom.upper)
             x_boundary_poly |= self.__class__.from_interval_product(x_int, y_interval)
 
         # Traverse the leafs of the interval tree
         y_boundary_poly = rempty()
         n = len(self._used_y_ranges)
         for i in range(n):
             row = i
             col = n - i - 1
             l_bound = ~self._x_boundaries[i]
             r_bound = self._x_boundaries[i+1]
-            x_int = closed(l_bound.val, r_bound.val)
+            x_int = P.closed(l_bound.val, r_bound.val)
             leaf_y_int = self._used_y_ranges[row][col]
             for y_atom in leaf_y_int:
-                y_int = singleton(y_atom.lower) | singleton(y_atom.upper)
+                y_int = P.singleton(y_atom.lower) | P.singleton(y_atom.upper)
                 y_boundary_poly |= self.__class__.from_interval_product(x_int, y_int)
 
         return x_boundary_poly | y_boundary_poly
 
     def __copy__(self):
         poly_copy = self.__class__()
         poly_copy._x_boundaries = SortedList(copy(b) for b in self._x_boundaries)
@@ -644,67 +643,67 @@
         string = []
         for atomic_poly in self.maximal_rectangles():
             x_int = atomic_poly.x_enclosure_interval
             y_int = atomic_poly.y_enclosure_interval
             string.append(f"(x={repr(x_int)}, y={repr(y_int)})")
         return " | ".join(string)
 
-    def _atomic_x_rectangle_partitioning(self) -> Iterator[Tuple[Interval, Interval]]:
+    def _atomic_x_rectangle_partitioning(self) -> Iterator[Tuple[P.Interval, P.Interval]]:
         """Traverse `self._used_y_ranges` to obtain a rectangle partitioning of the polygon.
 
         This function *MUST NOT* return tuples where either the first or the second interval is empty.
         """
-        def adj_y_interval(curr: Interval, l_parent: Interval, r_parent: Interval) -> Interval:
+        def adj_y_interval(curr: P.Interval, l_parent: P.Interval, r_parent: P.Interval) -> P.Interval:
             return curr - l_parent - r_parent
 
         return _traverse_diagonally(list(self._x_boundaries), self._used_y_ranges,
                                     lambda curr, l_parent, r_parent: curr | l_parent | r_parent,
                                     adj_y_interval)
 
-    def _maximal_atomic_x_rectangles(self) -> Iterator[Tuple[Interval, Interval]]:
+    def _maximal_atomic_x_rectangles(self) -> Iterator[Tuple[P.Interval, P.Interval]]:
         """Traverse `self._used_y_ranges` to obtain the maximum contained rectangles.
 
         This function *MUST NOT* return tuples where either the first or the second interval is empty.
         """
-        def adj_y_interval(curr: Interval, l_parent: Interval, r_parent: Interval) -> Interval:
+        def adj_y_interval(curr: P.Interval, l_parent: P.Interval, r_parent: P.Interval) -> P.Interval:
             return _sub_contained_atomics(_sub_contained_atomics(curr, l_parent), r_parent)
 
         return _traverse_diagonally(list(self._x_boundaries), self._used_y_ranges,
                                     lambda curr, l_parent, r_parent: curr | l_parent | r_parent,
                                     adj_y_interval)
 
     def _invert(self):
         temp = self._used_y_ranges
         self._used_y_ranges = self._free_y_ranges
         self._free_y_ranges = temp
 
-    def _add_interval_product(self, x_interval: Interval, y_interval: Interval):
+    def _add_interval_product(self, x_interval: P.Interval, y_interval: P.Interval):
         if not x_interval.empty and not y_interval.empty:
             for x_atom in x_interval:
                 self._add_atomic(x_atom, y_interval)
 
-    def _sub_interval_product(self, x_interval: Interval, y_interval: Interval):
+    def _sub_interval_product(self, x_interval: P.Interval, y_interval: P.Interval):
         if not x_interval.empty and not y_interval.empty:
             for x_atom in x_interval:
                 self._sub_atomic(x_atom, y_interval)
 
-    def _add_atomic(self, add_x_atom: Interval, add_y_interval: Interval):
+    def _add_atomic(self, add_x_atom: P.Interval, add_y_interval: P.Interval):
         """
         Update self._used_y_ranges and self._free_y_ranges such that they represent the union of the old rectangular
         polygon and the provided interval product.
         """
         _update_x_boundaries_and_y_interval_triangles(
             self._x_boundaries,
             self._used_y_ranges,
             self._free_y_ranges,
             add_x_atom,
             add_y_interval,
         )
 
-    def _sub_atomic(self, sub_x_atom: Interval, sub_y_interval: Interval):
+    def _sub_atomic(self, sub_x_atom: P.Interval, sub_y_interval: P.Interval):
         """
         Update self._used_y_ranges and self._free_y_ranges such that they represent the set difference of the old
         rectangular polygon and the provided interval product.
         """
         _update_x_boundaries_and_y_interval_triangles(
             self._x_boundaries,
             self._free_y_ranges,
@@ -716,29 +715,29 @@
 
 def rempty() -> RPolygon:
     """
     Create an empty rectangular polygon.
 
     :return RPolygon:
     """
-    return RPolygon.from_interval_product(empty(), empty())
+    return RPolygon.from_interval_product(P.empty(), P.empty())
 
 
 def rsingleton(x, y) -> RPolygon:
     """
     Create a Polygon representing a single value.
 
     :param x: x-value of the singleton
     :param y: y-value of the singleton
     :return RPolygon:
     """
-    return RPolygon.from_interval_product(singleton(x), singleton(y))
+    return RPolygon.from_interval_product(P.singleton(x), P.singleton(y))
 
 
-def rproduct(x_interval: Interval, y_interval: Interval):
+def rproduct(x_interval: P.Interval, y_interval: P.Interval):
     """
     Create a polygon as the (cartesian) product of two intervals.
 
     :param x_interval: x-interval of the cartesian product
     :param y_interval: y-interval of the cartesian product
     :return RPolygon:
     """
@@ -751,49 +750,49 @@
 
     :param x_lower: value of the lower bound in x-dimension
     :param x_upper: value of the upper bound in x-dimension
     :param y_lower: value of the lower bound in y-dimension
     :param y_upper: value of the upper bound in y-dimension
     :return RPolygon:
     """
-    return RPolygon.from_interval_product(open(x_lower, x_upper), open(y_lower, y_upper))
+    return RPolygon.from_interval_product(P.open(x_lower, x_upper), P.open(y_lower, y_upper))
 
 
 def rclosed(x_lower, x_upper, y_lower, y_upper) -> RPolygon:
     """
     Create a closed rectangular polygon.
 
     :param x_lower: value of the lower bound in x-dimension
     :param x_upper: value of the upper bound in x-dimension
     :param y_lower: value of the lower bound in y-dimension
     :param y_upper: value of the upper bound in y-dimension
     :return RPolygon:
     """
-    return RPolygon.from_interval_product(closed(x_lower, x_upper), closed(y_lower, y_upper))
+    return RPolygon.from_interval_product(P.closed(x_lower, x_upper), P.closed(y_lower, y_upper))
 
 
 def ropenclosed(x_lower, x_upper, y_lower, y_upper) -> RPolygon:
     """
     Create a rectangular polygon which is open on both lower bounds
     and closed on both upper bounds.
 
     :param x_lower: value of the lower bound in x-dimension
     :param x_upper: value of the upper bound in x-dimension
     :param y_lower: value of the lower bound in y-dimension
     :param y_upper: value of the upper bound in y-dimension
     :return RPolygon:
     """
-    return RPolygon.from_interval_product(openclosed(x_lower, x_upper), openclosed(y_lower, y_upper))
+    return RPolygon.from_interval_product(P.openclosed(x_lower, x_upper), P.openclosed(y_lower, y_upper))
 
 
 def rclosedopen(x_lower, x_upper, y_lower, y_upper) -> RPolygon:
     """
     Create a rectangular polygon which is closed on both lower bounds
     and open on both upper bounds.
 
     :param x_lower: value of the lower bound in x-dimension
     :param x_upper: value of the upper bound in x-dimension
     :param y_lower: value of the lower bound in y-dimension
     :param y_upper: value of the upper bound in y-dimension
     :return RPolygon:
     """
-    return RPolygon.from_interval_product(closedopen(x_lower, x_upper), closedopen(y_lower, y_upper))
+    return RPolygon.from_interval_product(P.closedopen(x_lower, x_upper), P.closedopen(y_lower, y_upper))
```

### Comparing `rportion-0.1.0/rportion.egg-info/PKG-INFO` & `rportion-0.2.0/rportion.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,48 @@
 Metadata-Version: 2.1
 Name: rportion
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python data structure and operations for 2-dimensional rectilinear polygons
 Home-page: https://github.com/tilmann-bartsch/rportion
 Author: Tilmann Bartsch
 License: MIT
 Keywords: rectangle polygon interval-tree
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Requires-Python: ~= 3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: sortedcontainers~=2.2
+Requires-Dist: portion~=2.4.2
 Provides-Extra: test
+Requires-Dist: pytest~=7.0; extra == "test"
+Requires-Dist: coverage~=6.0; extra == "test"
+Requires-Dist: numpy~=1.26.4; extra == "test"
 Provides-Extra: docu
-License-File: LICENSE
+Requires-Dist: numpy~=1.26.4; extra == "docu"
+Requires-Dist: matplotlib~=3.5.2; extra == "docu"
+Requires-Dist: imageio~=2.19.5; extra == "docu"
+Requires-Dist: pillow~=9.2.0; extra == "docu"
+Requires-Dist: tqdm~=4.64.0; extra == "docu"
 
 # rportion - data structure and operations for rectilinear polygons
 
 
-[![PyPI pyversions](https://img.shields.io/pypi/pyversions/pytest-codeblocks.svg?branch=master)](https://test.pypi.org/project/rportion/)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/rportion)](https://pypi.org/project/rportion/)
 [![Tests](https://github.com/tilmann-bartsch/rportion/actions/workflows/test.yaml/badge.svg?branch=master)](https://github.com/tilmann-bartsch/portion/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/tilmann-bartsch/rportion/badge.svg?branch=master)](https://coveralls.io/github/tilmann-bartsch/rportion?branch=master)
-[![LGTM](https://img.shields.io/lgtm/grade/python/github/tilmann-bartsch/rportion.svg?branch=master)](https://lgtm.com/projects/g/tilmann-bartsch/rportion)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Commits](https://img.shields.io/github/last-commit/tilmann-bartsch/rportion/master)](https://github.com/tilmann-bartsch/rportion/commits/master)
 
 The `rportion` library provides data structure to represent 
-2D [rectilinear polygons](https://en.wikipedia.org/wiki/Rectilinear_polygon) (unions of 2D-intervals) in Python 3.7+.
+2D [rectilinear polygons](https://en.wikipedia.org/wiki/Rectilinear_polygon) (unions of 2D-intervals) in Python 3.9+.
 It is built upon the library [`portion`](https://github.com/AlexandreDecan/portion) and follows its concepts.
 The following features are provided:
 
  - 2D-Intervals (rectangles) which can be open/closed and finite/infinite at every boundary
  - intersection, union, complement and difference of rectilinear polygons
  - iterator over all maximum rectangles inside and outside a given polygon
 
@@ -50,27 +59,37 @@
 
   * [Installation](#installation)
   * [Documentation & usage](#documentation--usage)
       * [Polygon creation](#polygon-creation)
       * [Polygon bounds & attributes](#polygon-bounds--attributes)
       * [Polygon operations](#polygon-operations)
       * [Rectangle partitioning iterator](#rectangle-partitioning-iterator)
-      * [Maximum rectangle iterator](#maximum-rectangle-iterators)
+      * [Maximum rectangle iterator](#maximum-rectangle-iterator)
       * [Boundary](#boundary)
       * [Internal data structure](#internal-data-structure)
   * [Changelog](#changelog)
   * [Contributions](#contributions)
   * [License](#license)
 
 ## Installation
 
-Install `rportion` from [PyPi-test](https://test.pypi.org/project/rportion/) with `pip` using 
-`pip install -i https://test.pypi.org/simple/ rportion`.
+`rportion` can be installed from [PyPi](https://pypi.org/project/rportion/) with `pip` using 
 
-Install `rportion` with the development environment using `pip install -e ".[test]"`.
+```bash
+pip install rportion
+```
+
+Alternatively, clone the repository and run
+
+```bash
+pip install -e ".[test]"
+python -m unittest discover -s tests
+```
+
+Note that `python
 
 ## Documentation & usage
 
 ### Polygon creation
 
 Atomic polygons (rectangles) can be created by one of the following:
 ```python
@@ -152,14 +171,16 @@
     the polygon.
     ```python
     >>> p = rp.rclosedopen(0, 2, 1, 3)
     >>> p.x_left, p.x_right, p.y_left, p.y_right
     (CLOSED, OPEN, CLOSED, OPEN)
     ```
 
+
+[&uparrow; back to top](#table-of-contents)
 ### Polygon operations
 
 `RPolygon` instances support the following operations:
  - `p.intersection(other)` and `p & other` return the intersection of two rectilinear polygons.
    ```python
    >>> rp.rclosed(0, 2, 0, 2) & rp.rclosed(1, 3, 0, 1)
    (x=[1,2], y=[0,1])
```

### Comparing `rportion-0.1.0/setup.py` & `rportion-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(
     path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
 ) as f:
     long_description = f.read()
 
 setup(
     name="rportion",
-    version="0.1.0",
+    version="0.2.0",
     license="MIT",
     author="Tilmann Bartsch",
     url="https://github.com/tilmann-bartsch/rportion",
     description="Python data structure and operations for 2-dimensional rectilinear polygons",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
@@ -23,22 +23,22 @@
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
     ],
     keywords="rectangle polygon interval-tree",
     packages=find_packages(include=["rportion"]),
-    python_requires="~= 3.7",
+    python_requires=">=3.9",
     install_requires=[
-        "sortedcontainers ~= 2.2", "portion ~= 2.2.0"
+        "sortedcontainers ~= 2.2", "portion ~= 2.4.2"
     ],
     extras_require={
         "test": ["pytest ~= 7.0",
                  "coverage ~= 6.0",
-                 "numpy ~= 1.21.6"],
-        "docu": ["numpy ~= 1.21.6",
+                 "numpy ~= 1.26.4"],
+        "docu": ["numpy ~= 1.26.4",
                  "matplotlib ~= 3.5.2",
                  "imageio ~= 2.19.5",
                  "pillow ~= 9.2.0",
                  "tqdm ~= 4.64.0"]
     },
 )
```

