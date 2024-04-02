# Comparing `tmp/curvey-0.0.1.tar.gz` & `tmp/curvey-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Mar 27 12:45:19 2024, max compression
+gzip compressed data, last modified: Tue Apr  2 21:23:34 2024, max compression
```

## Comparing `curvey-0.0.1.tar` & `curvey-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0     1102 2024-03-27 12:45:19.000000 curvey-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      306 2024-03-27 12:45:19.000000 curvey-0.0.1/environment.yml
--rw-r--r--   0        0        0     3023 2024-03-27 12:45:19.000000 curvey-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0       47 2024-03-27 12:45:19.000000 curvey-0.0.1/requirements.txt
--rw-r--r--   0        0        0      587 2024-03-27 12:45:19.000000 curvey-0.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0      801 2024-03-27 12:45:19.000000 curvey-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1203 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/bibliography.md
--rw-r--r--   0        0        0      358 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/index.md
--rw-r--r--   0        0        0       36 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/api/blend.md
--rw-r--r--   0        0        0     3143 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/api/curve.md
--rw-r--r--   0        0        0       38 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/api/curves.md
--rw-r--r--   0        0        0       34 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/api/flow.md
--rw-r--r--   0        0        0      410 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/api/index.md
--rw-r--r--   0        0        0       69 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/api/shape_structure_dataset.md
--rw-r--r--   0        0        0       18 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/api/util.md
--rw-r--r--   0        0        0      308 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/javascripts/katex.js
--rw-r--r--   0        0        0      384 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0     9221 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/tutorial/blend.ipynb
--rw-r--r--   0        0        0    10269 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/tutorial/flow.ipynb
--rw-r--r--   0        0        0      625 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/tutorial/index.md
--rw-r--r--   0        0        0    10970 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/tutorial/introduction.ipynb
--rw-r--r--   0        0        0     3307 2024-03-27 12:45:19.000000 curvey-0.0.1/docs/tutorial/shape_structure_dataset.ipynb
--rw-r--r--   0        0        0      296 2024-03-27 12:45:19.000000 curvey-0.0.1/src/conftest.py
--rw-r--r--   0        0        0      119 2024-03-27 12:45:19.000000 curvey-0.0.1/src/curvey/__init__.py
--rw-r--r--   0        0        0    12306 2024-03-27 12:45:19.000000 curvey-0.0.1/src/curvey/blend.py
--rw-r--r--   0        0        0    57732 2024-03-27 12:45:19.000000 curvey-0.0.1/src/curvey/curve.py
--rw-r--r--   0        0        0    20807 2024-03-27 12:45:19.000000 curvey-0.0.1/src/curvey/curves.py
--rw-r--r--   0        0        0    27476 2024-03-27 12:45:19.000000 curvey-0.0.1/src/curvey/flow.py
--rw-r--r--   0        0        0        0 2024-03-27 12:45:19.000000 curvey-0.0.1/src/curvey/py.typed
--rw-r--r--   0        0        0     5633 2024-03-27 12:45:19.000000 curvey-0.0.1/src/curvey/shape_structure_dataset.py
--rw-r--r--   0        0        0     8099 2024-03-27 12:45:19.000000 curvey-0.0.1/src/curvey/util.py
--rw-r--r--   0        0        0    23917 2024-03-27 12:45:19.000000 curvey-0.0.1/static/curv_interp.png
--rw-r--r--   0        0        0    39468 2024-03-27 12:45:19.000000 curvey-0.0.1/static/curve_plot.png
--rw-r--r--   0        0        0    40234 2024-03-27 12:45:19.000000 curvey-0.0.1/static/willmore_flow.png
--rw-r--r--   0        0        0     1164 2024-03-27 12:45:19.000000 curvey-0.0.1/tests/test_blend.py
--rw-r--r--   0        0        0     5685 2024-03-27 12:45:19.000000 curvey-0.0.1/tests/test_curve.py
--rw-r--r--   0        0        0      968 2024-03-27 12:45:19.000000 curvey-0.0.1/tests/test_curves.py
--rw-r--r--   0        0        0     1092 2024-03-27 12:45:19.000000 curvey-0.0.1/tests/test_flow.py
--rw-r--r--   0        0        0      739 2024-03-27 12:45:19.000000 curvey-0.0.1/tests/test_shape_structure_dataset.py
--rw-r--r--   0        0        0       77 2024-03-27 12:45:19.000000 curvey-0.0.1/.gitignore
--rw-r--r--   0        0        0     7651 2024-03-27 12:45:19.000000 curvey-0.0.1/LICENSE
--rw-r--r--   0        0        0     1034 2024-03-27 12:45:19.000000 curvey-0.0.1/README.md
--rw-r--r--   0        0        0     3525 2024-03-27 12:45:19.000000 curvey-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    11964 2024-03-27 12:45:19.000000 curvey-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-02 21:23:34.000000 curvey-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      335 2024-04-02 21:23:34.000000 curvey-0.0.2/environment.yml
+-rw-r--r--   0        0        0     3023 2024-04-02 21:23:34.000000 curvey-0.0.2/mkdocs.yml
+-rw-r--r--   0        0        0       47 2024-04-02 21:23:34.000000 curvey-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      588 2024-04-02 21:23:34.000000 curvey-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      801 2024-04-02 21:23:34.000000 curvey-0.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1203 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/bibliography.md
+-rw-r--r--   0        0        0      358 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/index.md
+-rw-r--r--   0        0        0       36 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/blend.md
+-rw-r--r--   0        0        0     3177 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/curve.md
+-rw-r--r--   0        0        0       38 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/curves.md
+-rw-r--r--   0        0        0       34 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/flow.md
+-rw-r--r--   0        0        0      410 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/index.md
+-rw-r--r--   0        0        0       69 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/shape_structure_dataset.md
+-rw-r--r--   0        0        0       18 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/api/util.md
+-rw-r--r--   0        0        0      308 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/javascripts/katex.js
+-rw-r--r--   0        0        0      384 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0     9221 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/blend.ipynb
+-rw-r--r--   0        0        0    10269 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/flow.ipynb
+-rw-r--r--   0        0        0      625 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/index.md
+-rw-r--r--   0        0        0    10970 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/introduction.ipynb
+-rw-r--r--   0        0        0     3307 2024-04-02 21:23:34.000000 curvey-0.0.2/docs/tutorial/shape_structure_dataset.ipynb
+-rw-r--r--   0        0        0      296 2024-04-02 21:23:34.000000 curvey-0.0.2/src/conftest.py
+-rw-r--r--   0        0        0      119 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/__init__.py
+-rw-r--r--   0        0        0    12306 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/blend.py
+-rw-r--r--   0        0        0    54814 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/curve.py
+-rw-r--r--   0        0        0    20807 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/curves.py
+-rw-r--r--   0        0        0    27476 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/flow.py
+-rw-r--r--   0        0        0     6498 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/plot.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/py.typed
+-rw-r--r--   0        0        0     5633 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/shape_structure_dataset.py
+-rw-r--r--   0        0        0     5818 2024-04-02 21:23:34.000000 curvey-0.0.2/src/curvey/util.py
+-rw-r--r--   0        0        0    23917 2024-04-02 21:23:34.000000 curvey-0.0.2/static/curv_interp.png
+-rw-r--r--   0        0        0    39468 2024-04-02 21:23:34.000000 curvey-0.0.2/static/curve_plot.png
+-rw-r--r--   0        0        0    40234 2024-04-02 21:23:34.000000 curvey-0.0.2/static/willmore_flow.png
+-rw-r--r--   0        0        0     1164 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_blend.py
+-rw-r--r--   0        0        0     6207 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_curve.py
+-rw-r--r--   0        0        0      968 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_curves.py
+-rw-r--r--   0        0        0     1092 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_flow.py
+-rw-r--r--   0        0        0      739 2024-04-02 21:23:34.000000 curvey-0.0.2/tests/test_shape_structure_dataset.py
+-rw-r--r--   0        0        0       62 2024-04-02 21:23:34.000000 curvey-0.0.2/.gitignore
+-rw-r--r--   0        0        0     7651 2024-04-02 21:23:34.000000 curvey-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1105 2024-04-02 21:23:34.000000 curvey-0.0.2/README.md
+-rw-r--r--   0        0        0     3555 2024-04-02 21:23:34.000000 curvey-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    12089 2024-04-02 21:23:34.000000 curvey-0.0.2/PKG-INFO
```

### Comparing `curvey-0.0.1/.pre-commit-config.yaml` & `curvey-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/mkdocs.yml` & `curvey-0.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/.github/workflows/release.yml` & `curvey-0.0.2/.github/workflows/release.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
     if: github.event_name == 'release' && github.event.action == 'published'
     steps:
       - uses: actions/download-artifact@v4
         with:
           name: Packages
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@release/v1
+      - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `curvey-0.0.1/.github/workflows/test.yml` & `curvey-0.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/docs/bibliography.md` & `curvey-0.0.2/docs/bibliography.md`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/docs/api/curve.md` & `curvey-0.0.2/docs/api/curve.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,20 @@
 
 These are special cases and have length `n + 1`
 ### ::: curvey.curve.Curve.closed_arclength
 ### ::: curvey.curve.Curve.closed_points
 
 ## Edge-valued properties
 The following properties have length `n`:
+### ::: curvey.curve.Curve.cum_edge_length
 ### ::: curvey.curve.Curve.edge
 ### ::: curvey.curve.Curve.edge_length
-### ::: curvey.curve.Curve.unit_edge
 ### ::: curvey.curve.Curve.edge_normal
-### ::: curvey.curve.Curve.cum_edge_length
+### ::: curvey.curve.Curve.edges
+### ::: curvey.curve.Curve.unit_edge
 
 ## Transformations
 All transformations return a new `Curve`; nothing modifies a `Curve` inplace.
 
 ## Basic transformations
 ### ::: curvey.curve.Curve.with_points
 ### ::: curvey.curve.Curve.with_data
@@ -95,9 +96,9 @@
 ## Special
 ### ::: curvey.curve.Curve.check_same_n_vertices
 ### ::: curvey.curve.Curve.deriv
 ### ::: curvey.curve.Curve.edge_intersections
 ### ::: curvey.curve.Curve.interpolator
 
 ## Library interface
+### ::: curvey.curve.Curve.from_shapely
 ### ::: curvey.curve.Curve.to_shapely
-### ::: curvey.curve.Curve.triangulate
```

### Comparing `curvey-0.0.1/docs/tutorial/blend.ipynb` & `curvey-0.0.2/docs/tutorial/blend.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/docs/tutorial/flow.ipynb` & `curvey-0.0.2/docs/tutorial/flow.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/docs/tutorial/index.md` & `curvey-0.0.2/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/docs/tutorial/introduction.ipynb` & `curvey-0.0.2/docs/tutorial/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/docs/tutorial/shape_structure_dataset.ipynb` & `curvey-0.0.2/docs/tutorial/shape_structure_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/src/curvey/blend.py` & `curvey-0.0.2/src/curvey/blend.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/src/curvey/curve.py` & `curvey-0.0.2/src/curvey/curve.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 from types import MappingProxyType
 from typing import Any, Callable, Literal, NamedTuple, cast, overload
 
 import numpy as np
 import scipy
 import shapely
 import sortedcontainers
-from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.collections import LineCollection, PathCollection
 from matplotlib.lines import Line2D
 from matplotlib.quiver import Quiver
 from numpy import (
     append,
     arange,
     arctan2,
     argmin,
     array,
+    array_equal,
     asanyarray,
     asarray,
     ceil,
     concatenate,
     cos,
     cross,
     cumsum,
@@ -48,19 +48,18 @@
     where,
     zeros,
 )
 from numpy.linalg import norm
 from numpy.typing import ArrayLike
 from typing_extensions import Self
 
+from .plot import _get_ax, _VariableColorSpec, quiver, segments
 from .util import (
     InterpType,
-    _get_ax,
     _rescale,
-    _VariableColorSpec,
     align_edges,
     angle_to_points,
     periodic_interpolator,
     reflection_matrix,
     rotation_matrix,
 )
 
@@ -122,14 +121,23 @@
         #   3) Assume a lot of curve construction happens from fluent chaining like
         #      `curve.scale(2).translate([3, 3]).to_length(1) where the public `points` array is
         #       never touched
         pts = self._pts.view()
         pts.flags["WRITEABLE"] = False
         return pts
 
+    @property
+    def edges(self) -> ndarray:
+        """A `(n, 2)` array of vertex indices
+
+        The integer valued vertex connectivity array `[(0, 1), (1, 2), ..., (n-2, n-1), (n-1, 0)]`.
+        """
+        idx = arange(self.n)
+        return stack([idx, roll(idx, -1)], axis=1)
+
     def __getitem__(self, item: str) -> Any:
         """Get curve metadata value by key name
 
         `curve['foo']` returns the value of the metadata parameter 'foo'.
 
         """
         return self._data[item]
@@ -855,66 +863,41 @@
         -------
         : matplotlib.quiver.Quiver
             If `directed` is True.
 
         : matplotlib.collections.LineCollection
             If `directed` is False.
         """
-        ax = _get_ax(ax)
-        width = _rescale(width, scale_width)
-        colorspec = _VariableColorSpec.parse(
-            n_data=self.n, supplied=color, default_varied=self.arclength
-        )
 
         if directed:
             if isinstance(width, (collections.abc.Sequence, ndarray)):
                 msg = (
                     "`width` was supplied as a sequence but "
                     "matplotlib.pyplot.Quiver doesn't support scaling individual arrows. "
                     "Use directed=False to scale edge width."
                 )
                 raise ValueError(msg)
 
-            x, y = self._pts.T
-            dx, dy = self.edge.T
-            return ax.quiver(
-                x,
-                y,
-                dx,
-                dy,
-                *colorspec.maybe_varied,
-                color=colorspec.fixed,
-                angles="xy",
-                scale_units="xy",
-                scale=1.0,
-                width=width,
-                **kwargs,
-            )
-
-        # not directed
-        pts = self.closed_points.reshape((-1, 1, 2))
-        segments = concatenate([pts[:-1], pts[1:]], axis=1)
-
-        if colorspec.varied is not None:
-            lc = LineCollection(
-                segments=segments,
-                cmap="viridis",
-                norm=plt.Normalize(),
-                linewidths=width,
+            return quiver(
+                points=self._pts,
+                vectors=self.edge,
+                color=color,
+                ax=ax,
                 **kwargs,
             )
-            lc.set_array(colorspec.varied)
-        else:
-            lc = LineCollection(segments=segments, color=colorspec.fixed, linewidths=width)
-        ax.add_collection(lc)
 
-        # Adding a line collection doesn't update limits so do it here
-        ax.update_datalim(self._pts)
-        ax.autoscale_view()
-        return lc
+        return segments(
+            points=self._pts,
+            edges=self.edges,
+            color=color,
+            width=width,
+            scale_width=scale_width,
+            ax=ax,
+            **kwargs,
+        )
 
     def plot_vectors(
         self,
         vectors: ndarray | None = None,
         scale: ndarray | None = None,
         color=None,
         scale_length: tuple[float, float] | None = None,
@@ -942,43 +925,21 @@
 
         ax
             The axes to plot in. Defaults to the current axes.
 
         **kwargs
             additional kwargs passed to `matplotlib.pyplot.quiver`
         """
-        ax = _get_ax(ax)
-
-        _vectors = self.normal if vectors is None else vectors
-
-        if scale is not None:
-            _vectors = scale.reshape(-1, 1) * _vectors
-
-        if scale_length is not None:
-            length = norm(_vectors, axis=1, keepdims=True)
-            scaled_length = _rescale(length, scale_length)
-            _vectors = _vectors / length * scaled_length
-
-        colorspec = _VariableColorSpec.parse(self.n, color, default_fixed="black")
-
-        # By default quiver doesn't include vector endpoints in x/y lim calculations
-        ax.update_datalim(self._pts + _vectors)
-
-        x, y = self._pts.T
-        dx, dy = _vectors.T
-        return ax.quiver(
-            x,
-            y,
-            dx,
-            dy,
-            *colorspec.maybe_varied,
-            color=colorspec.fixed,
-            angles="xy",
-            scale_units="xy",
-            scale=1.0,
+        return quiver(
+            points=self._pts,
+            vectors=self.normal if vectors is None else vectors,
+            scale=scale,
+            color=color,
+            scale_length=scale_length,
+            ax=ax,
             **kwargs,
         )
 
     def plot_points(
         self,
         color: ndarray | Any | None = None,
         size: ndarray | float | None = None,
@@ -1005,79 +966,19 @@
             Matplotlib axes to plot in. Defaults to the current axes.
 
         **kwargs
             additional kwargs passed to `matplotlib.pyplot.scatter`
 
         """
         ax = _get_ax(ax)
-
         if color is None:
             color = self.dual_edge_length
-
         size = _rescale(size, scale_sz)
-
-        return ax.scatter(self.x, self.y, s=size, c=color, **kwargs)
-
-    def triangulate(
-        self,
-        max_tri_area: float | None = None,
-        min_angle: float | None = None,
-        extra_params: str | None = None,
-    ) -> tuple[ndarray, ndarray, ndarray]:
-        """Triangulate the polygon enclosed by the curve with Shewchuck's triangulation library
-
-        The python bindings [triangle](https://rufat.be/triangle/index.html) must be importable.
-        They can be installed with `pip install triangle`.
-
-        Parameters
-        ----------
-        max_tri_area: float, optional
-            A global maximum triangle area constraint.
-
-        min_angle: float, optional
-            Minimum angle constraint, in degrees.
-
-        extra_params: str, optional
-            See the [API documentation](https://rufat.be/triangle/API.html).
-            E.g. `extra_params='S10X' specifies a maximum number of 10 Steiner points and suppresses
-            exact arithmetic.
-
-        Returns
-        -------
-        points :
-            The `(n, 2)` vertex coordinates of the triangulation. If `max_tri_area=None`,
-            this is probably equal to `self.points`
-
-        tris :
-            `(n_tris, 3)` array of integer vertex indices.
-
-        is_border :
-            Length `n` vector of booleans, true for vertices on the border of the triangulation.
-
-        """
-        try:
-            import triangle
-        except ImportError as e:
-            msg = "Cannot import `triangle`. Use `pip install triangle` to install."
-            raise ValueError(msg) from e
-
-        idx = arange(self.n)
-        segments = stack([idx, roll(idx, -1)], axis=1)
-        params = "p"  # Constrained polygon triangulation
-        if max_tri_area is not None:
-            params += f"a{max_tri_area: f}"
-        if min_angle is not None:
-            params += f"q{min_angle: f}"
-        if extra_params is not None:
-            params += extra_params
-
-        d = triangle.triangulate({"vertices": self._pts, "segments": segments}, params)
-        verts, tris, is_border = d["vertices"], d["triangles"], d["vertex_markers"]
-        is_border = is_border.astype(bool).squeeze()
-        return verts, tris, is_border
+        cspec = _VariableColorSpec.parse(self.n, color)
+        return ax.scatter(self.x, self.y, s=size, c=cspec.varied, **kwargs)
 
     def transform(self, transform: ndarray) -> Curve:
         """Apply a 2x2 or 3x3 transform matrix to the vertex positions"""
         pts = self._pts
         if transform.shape not in ((2, 2), (3, 3)):
             msg = f"Expected transform to have shape (2, 2) or (3, 3), got {transform.shape}"
             raise ValueError(msg)
@@ -1144,15 +1045,15 @@
         edge_idx = repeat(arange(self.n), n)
         edge_frac = concatenate([arange(ni) / ni for ni in n])
         pts = self._pts[edge_idx] + edge_frac[:, newaxis] * self.edge[edge_idx]
         return self.with_points(pts)
 
     def split_long_edges(self, thresh: float) -> Curve:
         """Split edges evenly so all edge lengths are below `thresh`"""
-        n_split = ceil(self.edge_length / thresh)
+        n_split = ceil(self.edge_length / thresh).astype("int")
         return self.split_edges(n_split)
 
     def split_longest_edges(self, n: int) -> Curve:
         """Insert `n` new vertices by uniform edge subdivision
 
         Edges are split in priority of their length, so very long edges may be split into
         thirds, fourths, etc. before very short edges are split in half.
@@ -1172,21 +1073,27 @@
 
         orig_edges = (
             Edge(split_length=length, n_subdivide=1, idx=i, orig_length=length)
             for (i, length) in enumerate(self.edge_length)
         )
 
         # Priority queue -- break length ties by the less split edge
-        queue = sortedcontainers.SortedList(orig_edges, key=lambda e: (e.length, -e.n_subdivide))
+        queue = sortedcontainers.SortedList(
+            orig_edges, key=lambda e: (e.split_length, -e.n_subdivide)
+        )
 
         for _ in range(n):
-            edge = queue.pop()
-            edge.n_subdivide += 1
-            edge.split_length = edge.orig_length / edge.n_subdivide
-            queue.add(edge)
+            e = queue.pop()
+            e = Edge(
+                split_length=e.orig_length / (e.n_subdivide + 1),
+                n_subdivide=e.n_subdivide + 1,
+                idx=e.idx,
+                orig_length=e.orig_length,
+            )
+            queue.add(e)
 
         edges = sorted(queue, key=lambda e: e.idx)
         n_subdivide = array([e.n_subdivide for e in edges])
         return self.split_edges(n_subdivide)
 
     def collapse_shortest_edges(
         self,
@@ -1298,14 +1205,24 @@
                 -l_next[:-1],  # upper diag = edge lengths (0, 1), (1, 2), (2, 3), ...
                 -l_next[[-1]],  # upper corner = the single edge length (n-1, 0)
             ],
             offsets=(-(n - 1), -1, 0, 1, n - 1),
         ).tocsc()
 
     @classmethod
+    def from_shapely(cls, ring: shapely.LinearRing) -> Self:
+        """Convert a `shapely.LinearRing` to a `curvey.Curve`"""
+        pts = array(ring.coords)
+        if array_equal(pts[0], pts[-1]):
+            # Shapely likes to explicitly close points
+            pts = pts[:-1]
+
+        return cls(pts)
+
+    @classmethod
     def from_curvature(
         cls,
         curvature: ndarray,
         edge_lengths: ndarray,
         solve_vertices: bool = True,
         theta0: float | None = None,
         pt0: ndarray | Sequence[float] | None = None,
```

### Comparing `curvey-0.0.1/src/curvey/curves.py` & `curvey-0.0.2/src/curvey/curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.lines import Line2D
 from numpy import arange, array, asanyarray, asarray, ceil, nan, ndarray, sqrt
 from numpy.typing import ArrayLike
 
 from .curve import Curve
-from .util import _get_ax
+from .plot import _get_ax
 
 NamedMetadata = Union[tuple[str, Sequence], tuple[str, Callable[[Curve], Any]]]
 BareMetadata = Union["str", Sequence, Callable[[Curve], Any]]
 Metadata = Union[NamedMetadata, BareMetadata]
 
 
 class Curves:
```

### Comparing `curvey-0.0.1/src/curvey/flow.py` & `curvey-0.0.2/src/curvey/flow.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/src/curvey/shape_structure_dataset.py` & `curvey-0.0.2/src/curvey/shape_structure_dataset.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/src/curvey/util.py` & `curvey-0.0.2/src/curvey/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Literal, NamedTuple, Union, cast, overload
+from typing import Callable, Literal, overload
 
 import scipy
 from matplotlib import pyplot as plt
-from matplotlib.axes import Axes
-from numpy import arctan2, array, asarray, concatenate, cos, cross, eye, ndarray, sin, stack
-from numpy.typing import ArrayLike
+from numpy import arctan2, array, concatenate, cos, cross, eye, ndarray, sin, stack
 
 
 def angle_to_points(theta: ndarray) -> ndarray:
     return stack([cos(theta), sin(theta)], axis=1)
 
 
 def rotation_matrix(theta: float) -> ndarray:
@@ -208,84 +206,14 @@
     if typ == "pchip":
         return _periodic_pchip(x, f)
 
     msg = f"Unrecognized interpolator type {typ}"
     raise ValueError(msg)
 
 
-# A way of typing the extra *args to quiver
-# Might be the empty tuple, or a single element tuple
-_SingleColorOrNothing = Union[tuple[()], tuple[Any]]
-
-
-class _VariableColorSpec(NamedTuple):
-    """Interpret a colorspec that could be either a constant color or an array of scalars
-
-    The reason we return both variables instead of an enum is for convenience with e.g.
-    matplotlibs quiver, which takes two disjoint arguments, `c` (varied) and `color` (fixed)
-
-    """
-
-    fixed: Any = None
-    varied: ArrayLike | None = None
-
-    @property
-    def maybe_varied(self) -> tuple[()] | tuple[ArrayLike]:
-        # Quiver doesn't allow named parameter for the varied color argument,
-        # so we need a little splatting magic
-        if self.varied is None:
-            return ()
-
-        return (self.varied,)
-
-    @staticmethod
-    def parse(
-        n_data: int | None,
-        supplied: Any,
-        default_varied=None,
-        default_fixed=None,
-    ) -> _VariableColorSpec:
-        if supplied is None:
-            return _VariableColorSpec(fixed=default_fixed, varied=default_varied)
-
-        if isinstance(supplied, str):  # e.g. color='black'
-            return _VariableColorSpec(fixed=supplied, varied=None)
-
-        try:
-            supplied_len = len(supplied)
-        except TypeError as e:
-            msg = "Expected `color` to have a length"
-            raise NotImplementedError(msg) from e
-
-        if n_data == supplied_len == 3:
-            # This is ambiguous and hopefully rare
-            # Could raise a warning or something but whatever
-            return _VariableColorSpec(fixed=None, varied=asarray(supplied))
-
-        if n_data == supplied_len:
-            return _VariableColorSpec(fixed=None, varied=asarray(supplied))
-
-        msg = f"Expected color to be of length {n_data}, got {supplied_len}"
-        raise ValueError(msg)
-
-
-def _get_ax(ax: Axes | None) -> Axes:
-    if ax:
-        return ax
-
-    if len(plt.get_fignums()) == 0:
-        # making a new axes so don't feel bad about setting some defaults
-        _fig, ax = plt.subplots()
-        ax = cast(Axes, ax)
-        ax.axis("equal")
-        return ax
-
-    return plt.gca()
-
-
 def _rescale(v, vout: tuple[float, float] | None = None) -> ndarray | None:
     if v is None:
         return None
 
     if vout is None:
         return v
     v1 = plt.Normalize()(v)  # Scale to 0, 1
```

### Comparing `curvey-0.0.1/static/curv_interp.png` & `curvey-0.0.2/static/curv_interp.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/static/curve_plot.png` & `curvey-0.0.2/static/curve_plot.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/static/willmore_flow.png` & `curvey-0.0.2/static/willmore_flow.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/tests/test_blend.py` & `curvey-0.0.2/tests/test_blend.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/tests/test_curve.py` & `curvey-0.0.2/tests/test_curve.py`

 * *Files 8% similar despite different names*

```diff
@@ -200,7 +200,27 @@
 
 def test_optimize_edge_lengths_to(circle, star):
     star = star.interpolate_n(circle.n).to_length(circle.length)
     err0 = ((star.edge_length - circle.edge_length) ** 2).sum()
     star = star.optimize_edge_lengths_to(circle)
     err1 = ((star.edge_length - circle.edge_length) ** 2).sum()
     assert err1 < err0
+
+
+def test_split_longest_edges(tri):
+    tri1 = tri.split_longest_edges(1)
+    assert tri1.n == 4
+
+
+def test_split_long_edges(tri):
+    tri1 = tri.split_long_edges(thresh=1.1)
+    assert tri1.n == 4
+
+
+def test_shapely_roundtrip(tri):
+    ring = tri.to_shapely("ring")
+    tri1 = Curve.from_shapely(ring)
+    assert_array_equal(tri.points, tri1.points)
+    tri_rev = tri.reverse()
+    ring_rev = tri_rev.to_shapely("ring")
+    tri1_rev = Curve.from_shapely(ring_rev)
+    assert_array_equal(tri_rev.points, tri1_rev.points)
```

### Comparing `curvey-0.0.1/tests/test_curves.py` & `curvey-0.0.2/tests/test_curves.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/tests/test_flow.py` & `curvey-0.0.2/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/tests/test_shape_structure_dataset.py` & `curvey-0.0.2/tests/test_shape_structure_dataset.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/LICENSE` & `curvey-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `curvey-0.0.1/pyproject.toml` & `curvey-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "curvey"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Darik Gamble", email = "darik.gamble@gmail.com"},
 ]
 maintainers = [
     {name = "Darik Gamble", email = "darik.gamble@gmail.com"}
 ]
 description = "Pythonic geometric processing of discrete planar closed curves"
@@ -53,14 +53,15 @@
 ]
 
 [project.optional-dependencies]
 dev = [
     "precommit",
     "mypy",
     "ruff",
+    "sortedcontainers-stubs",
     "sybil",
 ]
 docs = [
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings[python]>=0.18",
     "mkdocs-jupyter",
```

### Comparing `curvey-0.0.1/PKG-INFO` & `curvey-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: curvey
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pythonic geometric processing of discrete planar closed curves
 Project-URL: Homepage, https://github.com/darikg/curvey/
 Project-URL: Documentation, https://darikg.github.io/curvey/
 Project-URL: Source Code, https://github.com/darikg/curvey/
 Author-email: Darik Gamble <darik.gamble@gmail.com>
 Maintainer-email: Darik Gamble <darik.gamble@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
@@ -194,14 +194,15 @@
 Requires-Dist: shapely
 Requires-Dist: sortedcontainers
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: precommit; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: sortedcontainers-stubs; extra == 'dev'
 Requires-Dist: sybil; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-jupyter; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings[python]>=0.18; extra == 'docs'
 Provides-Extra: test
@@ -220,25 +221,25 @@
 ## Documentation
 Tutorials and API documentation hosted [here](https://darikg.github.io/curvey/)
 
 ## Highlights
 
 ### Quick visualizations
 
-<img src="https://github.com/darikg/curvey/blob/main/static/curve_plot.png" alt="drawing" width="400"/>
+<img src="https://raw.githubusercontent.com/darikg/curvey/main/static/curve_plot.png" alt="curve plotting" width="400"/>
 
 Everything's numpy-, scipy-, and matplotlib-based.
 
 ### Curvature flows
 
-<img src="https://github.com/darikg/curvey/blob/main/static/willmore_flow.png" alt="drawing" width="400"/>
+<img src="https://raw.githubusercontent.com/darikg/curvey/main/static/willmore_flow.png" alt="willmore flow" width="400"/>
 
 Implementations of curve-shortening flow, [singularity free mean curvature flow](
 https://arxiv.org/abs/1203.6819), and [Willmore flow](
 https://www.cs.cmu.edu/~kmcrane/Projects/ConformalWillmoreFlow/paper.pdf).
 
 ### Shape blending
 
-<img src="https://github.com/darikg/curvey/blob/main/static/curv_interp.png" alt="drawing" width="500"/>
+<img src="https://raw.githubusercontent.com/darikg/curvey/main/static/curv_interp.png" alt="curvature based shape interpolation" width="500"/>
 
 Implementations of linear shape blending and [curvature flow shape blending](
 https://www.sciencedirect.com/science/article/pii/S016783961730016X).
```

