# Comparing `tmp/genice2-svg-2.2.tar.gz` & `tmp/genice2_svg-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genice2-svg-2.2.tar", last modified: Thu Apr 21 04:05:41 2022, max compression
+gzip compressed data, was "genice2_svg-2.4.1.tar", max compression
```

## Comparing `genice2-svg-2.2.tar` & `genice2_svg-2.4.1.tar`

### file list

```diff
@@ -1,21 +1,10 @@
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2022-04-21 04:05:41.788242 genice2-svg-2.2/
--rw-r--r--   0 matto      (505) staff       (20)    24281 2022-04-21 04:05:41.788339 genice2-svg-2.2/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)    23805 2022-04-21 04:05:41.000000 genice2-svg-2.2/README.md
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2022-04-21 04:05:41.786954 genice2-svg-2.2/genice2_svg/
--rw-r--r--   0 matto      (505) staff       (20)       92 2022-04-21 04:03:06.000000 genice2-svg-2.2/genice2_svg/__init__.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2022-04-21 04:05:41.788127 genice2-svg-2.2/genice2_svg/formats/
--rw-r--r--   0 matto      (505) staff       (20)        0 2021-01-26 07:58:08.000000 genice2-svg-2.2/genice2_svg/formats/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)     1796 2021-05-05 04:50:23.000000 genice2-svg-2.2/genice2_svg/formats/png.py
--rw-r--r--   0 matto      (505) staff       (20)    18603 2022-04-21 04:01:21.000000 genice2-svg-2.2/genice2_svg/formats/svg.py
--rw-r--r--   0 matto      (505) staff       (20)     4730 2021-05-05 04:50:22.000000 genice2-svg-2.2/genice2_svg/render_png.py
--rw-r--r--   0 matto      (505) staff       (20)     6704 2022-02-08 02:57:13.000000 genice2-svg-2.2/genice2_svg/render_svg.py
--rw-r--r--   0 matto      (505) staff       (20)      491 2021-05-05 04:50:22.000000 genice2-svg-2.2/genice2_svg/theochem.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2022-04-21 04:05:41.787845 genice2-svg-2.2/genice2_svg.egg-info/
--rw-r--r--   0 matto      (505) staff       (20)    24281 2022-04-21 04:05:41.000000 genice2-svg-2.2/genice2_svg.egg-info/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)      426 2022-04-21 04:05:41.000000 genice2-svg-2.2/genice2_svg.egg-info/SOURCES.txt
--rw-r--r--   0 matto      (505) staff       (20)        1 2022-04-21 04:05:41.000000 genice2-svg-2.2/genice2_svg.egg-info/dependency_links.txt
--rw-r--r--   0 matto      (505) staff       (20)       77 2022-04-21 04:05:41.000000 genice2-svg-2.2/genice2_svg.egg-info/entry_points.txt
--rw-r--r--   0 matto      (505) staff       (20)       39 2022-04-21 04:05:41.000000 genice2-svg-2.2/genice2_svg.egg-info/requires.txt
--rw-r--r--   0 matto      (505) staff       (20)       12 2022-04-21 04:05:41.000000 genice2-svg-2.2/genice2_svg.egg-info/top_level.txt
--rw-r--r--   0 matto      (505) staff       (20)      108 2022-04-21 04:05:41.788621 genice2-svg-2.2/setup.cfg
--rw-r--r--   0 matto      (505) staff       (20)     1390 2021-03-19 15:19:50.000000 genice2-svg-2.2/setup.py
+-rw-r--r--   0        0        0   304008 2024-04-02 05:51:32.885626 genice2_svg-2.4.1/README.md
+-rw-r--r--   0        0        0      299 2024-04-01 03:36:42.231862 genice2_svg-2.4.1/genice2_svg/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 03:00:56.943806 genice2_svg-2.4.1/genice2_svg/formats/__init__.py
+-rw-r--r--   0        0        0     1787 2024-04-01 03:12:30.244780 genice2_svg-2.4.1/genice2_svg/formats/png.py
+-rw-r--r--   0        0        0    19166 2024-04-01 03:12:06.678499 genice2_svg-2.4.1/genice2_svg/formats/svg.py
+-rw-r--r--   0        0        0     4875 2024-04-01 03:03:37.353201 genice2_svg-2.4.1/genice2_svg/render_png.py
+-rw-r--r--   0        0        0     6642 2024-04-01 03:03:37.353402 genice2_svg-2.4.1/genice2_svg/render_svg.py
+-rw-r--r--   0        0        0      491 2024-04-01 03:00:56.944478 genice2_svg-2.4.1/genice2_svg/theochem.py
+-rw-r--r--   0        0        0     1067 2024-04-02 05:51:27.885932 genice2_svg-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0   304662 1970-01-01 00:00:00.000000 genice2_svg-2.4.1/PKG-INFO
```

### Comparing `genice2-svg-2.2/genice2_svg/formats/png.py` & `genice2_svg-2.4.1/genice2_svg/formats/png.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 """
 GenIce format plugin to generate a PNG file.
 
 Usage:
-    % genice CS2 -r 3 3 3 -f png[shadow:bg=#f00] > CS2.png
+    % genice2 CS2 -r 3 3 3 -f png[shadow:bg=#f00] > CS2.png
 
 Options:
     rotatex=30
     rotatey=30
     rotatez=30
     shadow         Draw shadows behind balls.
     bg=#f00        Specify the background color.
@@ -22,18 +22,20 @@
 
 import genice2_svg.formats.svg
 from genice2_svg.render_png import Render
 from logging import getLogger
 import numpy as np
 from math import sin, cos, pi
 import re
-desc = {"ref": {},
-        "brief": "PNG (Portable Network Graphics).",
-        "usage": __doc__,
-        }
+
+desc = {
+    "ref": {},
+    "brief": "PNG (Portable Network Graphics).",
+    "usage": __doc__,
+}
 
 
 class Format(genice2_svg.formats.svg.Format):
     """
     Format an ice structure into a PNG file.
 
     Options:
```

### Comparing `genice2-svg-2.2/genice2_svg/formats/svg.py` & `genice2_svg-2.4.1/genice2_svg/formats/svg.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 """
 GenIce format plugin to generate a SVG file.
 
 Usage:
-    % genice CS2 -r 3 3 3 -f svg[rotatex=30:shadow] > CS2.svg
+    % genice2 CS2 -r 3 3 3 -f svg[rotatex=30:shadow] > CS2.svg
 
 Options:
     rotatex=30
     rotatey=30
     rotatez=30
     polygon        Draw polygons instead of a ball and stick model.
     arrows         Draw the hydrogen bonds with arrows.
@@ -15,105 +15,129 @@
     bg=#f00        Specify the background color.
     O=0.06
     H=0            Size of the hydrogen atom (relative to that of oxygen)
     HB=0.4         Radius of HB relative to that of oxygem
     OH=0.5         Radius of OH colvalent bond relative to that of oxygem
     width=0        (Pixel)
     height=0       (Pixel)
+    margin=0       (Pixel)
 """
 
 from genice2.molecules import serialize
 from genice2.decorators import timeit, banner
 import genice2.formats
 from genice2_svg.render_svg import Render
 from cycless.cycles import cycles_iter
 import networkx as nx
 import numpy as np
 from collections import defaultdict
 from logging import getLogger
 from math import pi, cos, sin, radians
 import re
-desc = {"ref": {},
-        "brief": "SVG (Standard Vector Graphics).",
-        "usage": __doc__,
-        }
+
+desc = {
+    "ref": {},
+    "brief": "SVG (Standard Vector Graphics).",
+    "usage": __doc__,
+}
 
 
 def Normal(vs):
     """
     Normal vector (not normalized)
     """
     n = np.zeros(3)
     for i in range(vs.shape[0]):
         n += np.cross(vs[i - 1], vs[i])
     return n
 
 
-sun = np.array([-1., -1., 2.])
+sun = np.array([-1.0, -1.0, 2.0])
 sun /= np.linalg.norm(sun)
 
 
 # set of hue and saturation
-hue_sat = {3: (60., 0.8),
-           4: (120, 0.8),  # yellow-green
-           5: (180, 0.5),  # skyblue
-           6: (240, 0.5),  # blue
-           7: (300, 0.8),
-           8: (350, 0.5)}  # red-purple
+hue_sat = {
+    3: (60.0, 0.8),
+    4: (120, 0.8),  # yellow-green
+    5: (180, 0.5),  # skyblue
+    6: (240, 0.5),  # blue
+    7: (300, 0.8),
+    8: (350, 0.5),
+}  # red-purple
 
 
 def clip_cyl(v1, r1, v2, r2, rb):
-    r1c = (r1**2 - rb**2)**0.5
-    r2c = (r2**2 - rb**2)**0.5
+    r1c = (r1**2 - rb**2) ** 0.5
+    r2c = (r2**2 - rb**2) ** 0.5
     dv = v2 - v1
     Lv = np.linalg.norm(dv)
     if Lv < r1 + r2:
         return None
     newv1 = v1 + dv * r1c / Lv
     newv2 = v2 - dv * r2c / Lv
     c = (newv1 + newv2) / 2
     d = c - newv2
     return [c, "L2", d]
 
 
 def draw_cell(prims, cellmat, origin=np.zeros(3)):
-    for a in (0., 1.):
-        for b in (0., 1.):
-            v0 = np.array([0., a, b] + origin)
-            v1 = np.array([1., a, b] + origin)
+    for a in (0.0, 1.0):
+        for b in (0.0, 1.0):
+            v0 = np.array([0.0, a, b] + origin)
+            v1 = np.array([1.0, a, b] + origin)
             mid = (v0 + v1) / 2
-            prims.append([np.dot(mid, cellmat),
-                          "L",
-                          np.dot(v0, cellmat),
-                          np.dot(v1, cellmat), 0, {"stroke_width": 1,
-                                                   "stroke": "#888"}])
-            v0 = np.array([b, 0., a] + origin)
-            v1 = np.array([b, 1., a] + origin)
+            prims.append(
+                [
+                    np.dot(mid, cellmat),
+                    "L",
+                    np.dot(v0, cellmat),
+                    np.dot(v1, cellmat),
+                    0,
+                    {"stroke_width": 1, "stroke": "#888"},
+                ]
+            )
+            v0 = np.array([b, 0.0, a] + origin)
+            v1 = np.array([b, 1.0, a] + origin)
             mid = (v0 + v1) / 2
-            prims.append([np.dot(mid, cellmat),
-                          "L",
-                          np.dot(v0, cellmat),
-                          np.dot(v1, cellmat), 0, {"stroke_width": 1,
-                                                   "stroke": "#888"}])
-            v0 = np.array([a, b, 0.] + origin)
-            v1 = np.array([a, b, 1.] + origin)
+            prims.append(
+                [
+                    np.dot(mid, cellmat),
+                    "L",
+                    np.dot(v0, cellmat),
+                    np.dot(v1, cellmat),
+                    0,
+                    {"stroke_width": 1, "stroke": "#888"},
+                ]
+            )
+            v0 = np.array([a, b, 0.0] + origin)
+            v1 = np.array([a, b, 1.0] + origin)
             mid = (v0 + v1) / 2
-            prims.append([np.dot(mid, cellmat),
-                          "L",
-                          np.dot(v0, cellmat),
-                          np.dot(v1, cellmat), 0, {"stroke_width": 1,
-                                                   "stroke": "#888"}])
+            prims.append(
+                [
+                    np.dot(mid, cellmat),
+                    "L",
+                    np.dot(v0, cellmat),
+                    np.dot(v1, cellmat),
+                    0,
+                    {"stroke_width": 1, "stroke": "#888"},
+                ]
+            )
     corners = []
     for x in (np.zeros(3), cellmat[0]):
         for y in (np.zeros(3), cellmat[1]):
             for z in (np.zeros(3), cellmat[2]):
                 corners.append(x + y + z + origin)
     corners = np.array(corners)
-    return np.min(corners[:, 0]), np.max(corners[:, 0]), np.min(
-        corners[:, 1]), np.max(corners[:, 1])
+    return (
+        np.min(corners[:, 0]),
+        np.max(corners[:, 0]),
+        np.min(corners[:, 1]),
+        np.max(corners[:, 1]),
+    )
 
 
 class Format(genice2.formats.Format):
     """
     Format an ice structure into a SVG file.
 
     Options:
@@ -139,64 +163,69 @@
 
     @timeit
     @banner
     def __init__(self, **kwargs):
         "ArgParser (svg)."
         #
         # このparserだと、rotatexを二回指定できない。しかも、実行順序が安定しない。
-        # 
+        #
         #
         logger = getLogger()
         self.renderer = Render
         self.encode = True  # valid for png.
         self.poly = False
         self.shadow = None
         self.oxygen = 0.06  # absolute radius in nm
         self.HB = 0.4  # radius relative to the oxygen
         self.OH = 0.5  # radius relative to the oxygen
-        self.hydrogen = 0    # radius relative to the oxygen
+        self.hydrogen = 0  # radius relative to the oxygen
         self.arrows = False
         self.bgcolor = None
-        self.proj = np.array([[1., 0, 0], [0, 1, 0], [0, 0, 1]])
+        self.proj = np.array([[1.0, 0, 0], [0, 1, 0], [0, 0, 1]])
         self.width = 0
         self.height = 0
+        self.margin = 0  # margin around the cell cube
+        unprocessed = dict()
         for key, value in kwargs.items():
-            logger.info(
-                "  Option with arguments: {0} := {1}".format(
-                    key, value))
+            logger.info("  Option with arguments: {0} := {1}".format(key, value))
             if key == "rotmat":
                 value = re.search(r"\[([-0-9,.]+)\]", value).group(1)
-                self.proj = np.array([float(x)
-                                     for x in value.split(",")]).reshape(3, 3)
+                self.proj = np.array([float(x) for x in value.split(",")]).reshape(3, 3)
             elif key == "rotatex":
-                logger.warning("The rotatex option is deprecated. Use rotate option instead.")
+                logger.warning(
+                    "The rotatex option is deprecated. Use rotate option instead."
+                )
                 value = float(value) * pi / 180
                 cosx = cos(value)
                 sinx = sin(value)
                 R = np.array([[1, 0, 0], [0, cosx, sinx], [0, -sinx, cosx]])
                 self.proj = np.dot(self.proj, R)
             elif key == "rotatey":
-                logger.warning("The rotatey option is deprecated. Use rotate option instead.")
+                logger.warning(
+                    "The rotatey option is deprecated. Use rotate option instead."
+                )
                 value = float(value) * pi / 180
                 cosx = cos(value)
                 sinx = sin(value)
                 R = np.array([[cosx, 0, -sinx], [0, 1, 0], [sinx, 0, cosx]])
                 self.proj = np.dot(self.proj, R)
             elif key == "rotatez":
-                logger.warning("The rotatez option is deprecated. Use rotate option instead.")
+                logger.warning(
+                    "The rotatez option is deprecated. Use rotate option instead."
+                )
                 value = float(value) * pi / 180
                 cosx = cos(value)
                 sinx = sin(value)
                 R = np.array([[cosx, sinx, 0], [-sinx, cosx, 0], [0, 0, 1]])
                 self.proj = np.dot(self.proj, R)
             elif key == "rotate":
                 values = value.split(",")
                 for value in values:
                     axis = value[0]
-                    angle  = radians(float(value[1:]))
+                    angle = radians(float(value[1:]))
                     cosx = cos(angle)
                     sinx = sin(angle)
                     if axis in "xX":
                         R = np.array([[1, 0, 0], [0, cosx, sinx], [0, -sinx, cosx]])
                     elif axis in "yY":
                         R = np.array([[cosx, 0, -sinx], [0, 1, 0], [sinx, 0, cosx]])
                     elif axis in "zZ":
@@ -226,27 +255,34 @@
                     self.OH = float(value)
             elif key == "bg":
                 self.bgcolor = value
             elif key == "width":
                 self.width = int(value)
             elif key == "height":
                 self.height = int(value)
+            elif key == "margin":
+                self.margin = int(value)
             elif key == "encode":
                 self.encode = bool(value)
             elif value is True:
                 a = key
                 logger.info("  Flags: {0}".format(a))
                 if a == "polygon":
                     self.poly = True
                 elif a == "arrows":
                     self.arrows = True
                 else:
                     assert False, "  Wrong options."
             else:
-                assert False, "  Wrong options."
+                unprocessed[key] = value
+            self.width -= self.margin * 2
+            self.height -= self.margin * 2
+        kwargs.clear()
+        kwargs |= unprocessed
+        logger.info(kwargs)
 
     @timeit
     @banner
     def Hook2(self, lattice):
         "A. Output molecular positions in PNG/SVG format."
         logger = getLogger()
         if self.hydrogen > 0 or self.arrows:
@@ -262,52 +298,62 @@
         projected = np.dot(cellmat, self.proj)
         pos = lattice.reppositions
         prims = []
         RO = self.oxygen  # nm
         RHB = self.oxygen * self.HB  # nm
         xmin, xmax, ymin, ymax = draw_cell(prims, projected)
         if self.poly:
-            for ring in cycles_iter(nx.Graph(lattice.graph),
-                                    8,
-                                    pos=lattice.reppositions):
+            for ring in cycles_iter(
+                nx.Graph(lattice.graph), 8, pos=lattice.reppositions
+            ):
                 nedges = len(ring)
                 deltas = np.zeros((nedges, 3))
                 d2 = np.zeros(3)
                 for k, i in enumerate(ring):
                     d = lattice.reppositions[i] - lattice.reppositions[ring[0]]
                     d -= np.floor(d + 0.5)
                     deltas[k] = d
                 comofs = np.sum(deltas, axis=0) / len(ring)
                 deltas -= comofs
                 com = lattice.reppositions[ring[0]] + comofs
                 com -= np.floor(com)
                 # rel to abs
                 com = np.dot(com, projected)
                 deltas = np.dot(deltas, projected)
-                prims.append(
-                    [com, "P", deltas, {"fillhs": hue_sat[nedges]}])  # line
+                prims.append([com, "P", deltas, {"fillhs": hue_sat[nedges]}])  # line
         else:
             for i, j in lattice.graph.edges():
                 vi = pos[i]
                 d = pos[j] - pos[i]
                 d -= np.floor(d + 0.5)
-                clipped = clip_cyl(
-                    vi @ projected, RO, (vi + d) @ projected, RO, RHB)
+                clipped = clip_cyl(vi @ projected, RO, (vi + d) @ projected, RO, RHB)
                 if clipped is not None:
                     prims.append(clipped + [RHB, {"fill": "#fff"}])  # line
+                # If the bond intersects the cell boundary,
                 if np.linalg.norm(vi + d - pos[j]) > 0.01:
                     vj = pos[j]
                     d = pos[i] - pos[j]
                     d -= np.floor(d + 0.5)
                     clipped = clip_cyl(
-                        vj @ projected, RO, (vj + d) @ projected, RO, RHB)
+                        vj @ projected, RO, (vj + d) @ projected, RO, RHB
+                    )
                     if clipped is not None:
                         prims.append(clipped + [RHB, {"fill": "#fff"}])  # line
             for i, v in enumerate(pos):
-                prims.append([np.dot(v, projected), "C", RO, {}])  # circle
+                p = v @ projected
+                prims.append([p, "C", RO, {}])  # circle
+                # if the atom is on the boundary,
+                for j in range(3):
+                    if p[j] == 0:
+                        logger.info(f"On the boundary {j}")
+                        q = v.copy()
+                        q[j] = 1.0
+                        p = q @ projected
+                        prims.append([p, "C", RO, {}])  # circle
+        # size of the object
         xsize = xmax - xmin
         ysize = ymax - ymin
         zoom = 100
         if self.width > 0:
             zoom = self.width / xsize
             if self.height > 0:
                 z2 = self.height / ysize
@@ -318,105 +364,108 @@
                     xmin, xmax = xcenter - xsize / 2, xcenter + xsize / 2
                 else:
                     ysize = self.height / zoom
                     ycenter = (ymax + ymin) / 2
                     ymin, ymax = ycenter - ysize / 2, ycenter + ysize / 2
         elif self.height > 0:
             zoom = self.height / ysize
-        logger.debug(
-            "Zoom {0} {1}x{2}".format(
-                zoom,
-                zoom * xsize,
-                zoom * ysize))
-        self.output = self.renderer(prims, RO,
-                                    shadow=self.shadow,
-                                    topleft=np.array((xmin, ymin)),
-                                    size=(xsize, ysize),
-                                    zoom=zoom,
-                                    bgcolor=self.bgcolor,
-                                    encode=self.encode)
+        logger.debug("Zoom {0} {1}x{2}".format(zoom, zoom * xsize, zoom * ysize))
+        # margin in object scale
+        rmargin = self.margin / zoom
+        self.output = self.renderer(
+            prims,
+            RO,
+            shadow=self.shadow,
+            topleft=np.array((xmin - rmargin, ymin - rmargin)),
+            size=(xsize + rmargin * 2, ysize + rmargin * 2),
+            zoom=zoom,
+            bgcolor=self.bgcolor,
+            encode=self.encode,
+        )
         if self.hydrogen == 0 and not self.arrows:
             logger.info("Abort the following stages.")
             return True  # abort the following stages
 
     @timeit
     @banner
     def Hook6(self, lattice):
         "A. Output atomic positions in PNG/SVG format."
         logger = getLogger()
         if self.hydrogen == 0 and not self.arrows:
             # draw everything in hook2
             return
 
-        filloxygen = {"stroke_width": 1,
-                      "stroke": "#444",
-                      "fill": "#f00",
-                      # "stroke_linejoin": "round",
-                      # "stroke_linecap" : "round",
-                      # "fill_opacity": 1.0,
-                      }
-        fillhydrogen = {"stroke_width": 1,
-                        "stroke": "#444",
-                        "fill": "#0ff",
-                        # "stroke_linejoin": "round",
-                        # "stroke_linecap" : "round",
-                        # "fill_opacity": 1.0,
-                        }
-        lineOH = {"stroke_width": 1,
-                  "stroke": "#444",
-                  "fill": "#fff",
-                  }
-        lineHB = {"stroke_width": 1,
-                  "stroke": "#444",
-                  "fill": "#ff0",
-                  }
-        arrow = {"stroke_width": 3,
-                 "stroke": "#fff",
-                 }
+        filloxygen = {
+            "stroke_width": 1,
+            "stroke": "#444",
+            "fill": "#f00",
+            # "stroke_linejoin": "round",
+            # "stroke_linecap" : "round",
+            # "fill_opacity": 1.0,
+        }
+        fillhydrogen = {
+            "stroke_width": 1,
+            "stroke": "#444",
+            "fill": "#0ff",
+            # "stroke_linejoin": "round",
+            # "stroke_linecap" : "round",
+            # "fill_opacity": 1.0,
+        }
+        lineOH = {
+            "stroke_width": 1,
+            "stroke": "#444",
+            "fill": "#fff",
+        }
+        lineHB = {
+            "stroke_width": 1,
+            "stroke": "#444",
+            "fill": "#ff0",
+        }
+        arrow = {
+            "stroke_width": 3,
+            "stroke": "#fff",
+        }
         offset = np.zeros(3)
 
         # Projection to the viewport
         for i in range(3):
             self.proj[i] /= np.linalg.norm(self.proj[i])
         self.proj = np.linalg.inv(self.proj)
 
         cellmat = lattice.repcell.mat
         projected = np.dot(cellmat, self.proj)
 
         # pos = lattice.reppositions
         prims = []
         RO = self.oxygen  # nm
-        RHB = self.oxygen * self.HB       # nm
-        ROH = self.oxygen * self.OH       # nm
+        RHB = self.oxygen * self.HB  # nm
+        ROH = self.oxygen * self.OH  # nm
         RH = self.oxygen * self.hydrogen  # nm
         waters = defaultdict(dict)
         xmin, xmax, ymin, ymax = draw_cell(prims, projected)
         if self.arrows:
             pos = lattice.reppositions
             for i, j in lattice.spacegraph.edges():
                 vi = pos[i]
                 d = pos[j] - pos[i]
                 d -= np.floor(d + 0.5)
                 clipped = clip_cyl(
-                    vi @ projected,
-                    RO,
-                    (vi + d) @ projected,
-                    RO,
-                    0.0)  # line
+                    vi @ projected, RO, (vi + d) @ projected, RO, 0.0
+                )  # line
                 if clipped is not None:
                     prims.append(clipped + [0.0, {"stroke": "#fff"}])  # line
                 if np.linalg.norm(vi + d - pos[j]) > 0.01:
                     vj = pos[j]
                     d = pos[i] - pos[j]
                     d -= np.floor(d + 0.5)
                     clipped = clip_cyl(
-                        (vj + d) @ projected, RO, vj @ projected, RO, 0.0)
+                        (vj + d) @ projected, RO, vj @ projected, RO, 0.0
+                    )
                     if clipped is not None:
-                        prims.append(clipped +
-                                     [0.0, {"stroke": "#fff"}])  # line
+                        prims.append(clipped + [0.0, {"stroke": "#fff"}])  # line
             for i, v in enumerate(pos):
                 prims.append([np.dot(v, projected), "C", RO, {}])  # circle
         else:
             atoms = []
             for mols in lattice.universe:
                 atoms += serialize(mols)
 
@@ -431,49 +480,51 @@
                         waters[order]["H1"] = position
 
             # draw water molecules
             for order, water in waters.items():
                 O = water["O"]
                 H0 = water["H0"]
                 H1 = water["H1"]
-                prims.append([O  @ self.proj, "C", RO, filloxygen])  # circle
+                prims.append([O @ self.proj, "C", RO, filloxygen])  # circle
                 prims.append([H0 @ self.proj, "C", RH, fillhydrogen])  # circle
                 prims.append([H1 @ self.proj, "C", RH, fillhydrogen])  # circle
                 # clipped cylinder
                 clipped = clip_cyl(O @ self.proj, RO, H0 @ self.proj, RH, ROH)
                 if clipped is not None:
                     prims.append(clipped + [ROH, lineOH])
                 clipped = clip_cyl(O @ self.proj, RO, H1 @ self.proj, RH, ROH)
                 if clipped is not None:
                     prims.append(clipped + [ROH, lineOH])
             # draw HBs
-            for i, j, d in lattice.spacegraph.edges(data=True):
+            for i, j in lattice.digraph.edges():
                 if i in waters and j in waters:  # edge may connect to the dopant
                     O = waters[j]["O"]
                     H0 = waters[i]["H0"]
                     H1 = waters[i]["H1"]
                     d0 = H0 - O
                     d1 = H1 - O
                     rr0 = d0 @ d0
                     rr1 = d1 @ d1
                     if rr0 < rr1 and rr0 < 0.245**2:
-                        clipped = clip_cyl(
-                            O @ self.proj, RO, H0 @ self.proj, RH, RHB)
+                        clipped = clip_cyl(O @ self.proj, RO, H0 @ self.proj, RH, RHB)
                         if clipped is not None:
                             prims.append(clipped + [RHB, lineHB])
                     elif rr1 < rr0 and rr1 < 0.245**2:
-                        clipped = clip_cyl(
-                            O @ self.proj, RO, H1 @ self.proj, RH, RHB)
+                        clipped = clip_cyl(O @ self.proj, RO, H1 @ self.proj, RH, RHB)
                         if clipped is not None:
                             prims.append(clipped + [RHB, lineHB])
-                    else:
-                        logger.debug(
-                            (np.linalg.norm(
-                                d['vector']), rr0, rr1, 0.245**2))
+                    # else:
+                    #     logger.debug(
+                    #         (np.linalg.norm(d["vector"]), rr0, rr1, 0.245**2)
+                    #     )
         xsize = xmax - xmin
         ysize = ymax - ymin
-        self.output = self.renderer(prims, RO,
-                                    shadow=self.shadow,
-                                    topleft=np.array((xmin, ymin)),
-                                    size=(xsize, ysize),
-                                    bgcolor=self.bgcolor,
-                                    encode=self.encode)
+        rmargin = self.margin / zoom
+        self.output = self.renderer(
+            prims,
+            RO,
+            shadow=self.shadow,
+            topleft=np.array((xmin - rmargin, ymin - rmargin)),
+            size=(xsize + rmargin * 2, ysize + rmargin * 2),
+            bgcolor=self.bgcolor,
+            encode=self.encode,
+        )
```

### Comparing `genice2-svg-2.2/genice2_svg/render_png.py` & `genice2_svg-2.4.1/genice2_svg/render_png.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,20 +8,33 @@
 
 
 def cylinder(draw, v1_, v2_, r, **options):
     """
     draw a 3D cylinder
     """
     options = {"fill": "#fff", **options}
-    draw.line([int(x) for x in [v1_[0], v1_[1], v2_[0], v2_[1]]],
-              width=int(r * 2), fill=options["fill"])
-
-
-def Render(prims, Rsphere, shadow=None, topleft=np.array(
-        [-1., -1.]), size=(50, 50), zoom=200, vertices=None, vecs=None, bgcolor='#fff', encode=True):
+    draw.line(
+        [int(x) for x in [v1_[0], v1_[1], v2_[0], v2_[1]]],
+        width=int(r * 2),
+        fill=options["fill"],
+    )
+
+
+def Render(
+    prims,
+    Rsphere,
+    shadow=None,
+    topleft=np.array([-1.0, -1.0]),
+    size=(50, 50),
+    zoom=200,
+    vertices=None,
+    vecs=None,
+    bgcolor="#fff",
+    encode=True,
+):
     """
     Renter the image in PNG format and output to the stdout.
     Returns nothing.
 
     When vertex list is given, the coords in prims are not indicated in vectors but in indices
     Vecs are vectors not needed to be sorted (used in "L" command)
     """
@@ -31,94 +44,115 @@
     draw = ImageDraw.Draw(image, "RGBA")
     # special treatment for post-K project
     # draw.rectangle([0,0,size[0]/2,size[1]], fill="#EF5FA7")
     # draw.rectangle([size[0]/2,0,size[0],size[1]], fill="#00A2FF")
 
     TL0 = np.zeros(3)
     TL0[:2] = topleft
-    linedefaults = {"stroke_width": 2,
-                    "stroke": "#000",
-                    # "stroke_linejoin": "round",
-                    # "stroke_linecap" : "round",
-                    }
-    filldefaults = {"stroke_width": 1,
-                    "stroke": "#000",
-                    "fill": "#0ff",
-                    # "stroke_linejoin": "round",
-                    # "stroke_linecap" : "round",
-                    # "fill_opacity": 1.0,
-                    }
-    shadowdefaults = {"stroke_width": 0,
-                      # "fill": "#8881",
-                      "fill": shadow,
-                      # "fill_opacity": 0.08,
-                      }
+    linedefaults = {
+        "stroke_width": 2,
+        "stroke": "#000",
+        # "stroke_linejoin": "round",
+        # "stroke_linecap" : "round",
+    }
+    filldefaults = {
+        "stroke_width": 1,
+        "stroke": "#000",
+        "fill": "#0ff",
+        # "stroke_linejoin": "round",
+        # "stroke_linecap" : "round",
+        # "fill_opacity": 1.0,
+    }
+    shadowdefaults = {
+        "stroke_width": 0,
+        # "fill": "#8881",
+        "fill": shadow,
+        # "fill_opacity": 0.08,
+    }
     if shadow is not None:
         r = Rsphere
         Z = np.array([0, 0, 1.0])
-        prims += [[prim[0] - Z * r * 1.4**j, prim[1] + 'S', r * 1.4**j] + prim[3:]
-                  for j in range(1, 5) for prim in prims if prim[1] == 'C']
+        prims += [
+            [prim[0] - Z * r * 1.4**j, prim[1] + "S", r * 1.4**j] + prim[3:]
+            for j in range(1, 5)
+            for prim in prims
+            if prim[1] == "C"
+        ]
     prims.sort(key=lambda x: -x[0][2])
     while len(prims) > 0:
         prim = prims.pop()
-        if not ((-0.5 < prim[0][0] - topleft[0] < size[0] + 0.5) and
-                (-0.5 < prim[0][1] - topleft[1] < size[1] + 0.5)):
+        if not (
+            (-0.5 < prim[0][0] - topleft[0] < size[0] + 0.5)
+            and (-0.5 < prim[0][1] - topleft[1] < size[1] + 0.5)
+        ):
             continue
         if prim[1] == "L":
             if prim[4] == 0:
                 options = {**linedefaults, **prim[5]}
                 s = (prim[2][:2] - topleft) * zoom
                 e = (prim[3][:2] - topleft) * zoom
-                draw.line([int(s[0]), int(s[1]), int(e[0]), int(e[1])],
-                          fill=options["stroke"], width=options["stroke_width"])
+                draw.line(
+                    [int(s[0]), int(s[1]), int(e[0]), int(e[1])],
+                    fill=options["stroke"],
+                    width=options["stroke_width"],
+                )
             else:
                 options = {**filldefaults, **prim[5]}
                 cylinder(
                     draw,
                     (prim[2] - TL0) * zoom,
                     (prim[3] - TL0) * zoom,
                     prim[4] * zoom,
-                    **options)
+                    **options
+                )
         elif prim[1] == "L2":
             # new, simpler expression.
             # half relative vector is given
             if prim[3] == 0:
                 options = {**linedefaults, **prim[4]}
                 s = ((prim[0] + prim[2])[:2] - topleft) * zoom
                 e = ((prim[0] - prim[2])[:2] - topleft) * zoom
-                draw.line([int(s[0]), int(s[1]), int(e[0]), int(e[1])],
-                          fill=options["stroke"], width=options["stroke_width"])
+                draw.line(
+                    [int(s[0]), int(s[1]), int(e[0]), int(e[1])],
+                    fill=options["stroke"],
+                    width=options["stroke_width"],
+                )
             else:
                 options = {**filldefaults, **prim[4]}
                 cylinder(
                     draw,
                     (prim[0] + prim[2] - TL0) * zoom,
                     (prim[0] - prim[2] - TL0) * zoom,
                     prim[3] * zoom,
-                    **options)
+                    **options
+                )
         elif prim[1] == "C":
             options = {**filldefaults, **prim[3]}
             Rsphere = prim[2]
             center = (prim[0][:2] - topleft) * zoom
             r = Rsphere * zoom
             tl = center - r
             br = center + r
             draw.ellipse(
-                [int(x) for x in [tl[0], tl[1], br[0], br[1]]], fill=options["fill"])
+                [int(x) for x in [tl[0], tl[1], br[0], br[1]]], fill=options["fill"]
+            )
         elif prim[1] == "CS":
             Rsphere = prim[2]
-            options = {**shadowdefaults, }  # **prim[3] }
+            options = {
+                **shadowdefaults,
+            }  # **prim[3] }
             # logger.info("{0}".format(options))
             center = (prim[0][:2] - topleft) * zoom
             r = Rsphere * zoom
             tl = center - r
             br = center + r
 
             draw.ellipse(
-                [int(x) for x in [tl[0], tl[1], br[0], br[1]]], fill=options["fill"])
+                [int(x) for x in [tl[0], tl[1], br[0], br[1]]], fill=options["fill"]
+            )
     if encode:
         imgByteArr = io.BytesIO()
-        image.save(imgByteArr, format='PNG')
+        image.save(imgByteArr, format="PNG")
         imgByteArr = imgByteArr.getvalue()
         return imgByteArr
     else:
         return image
```

### Comparing `genice2-svg-2.2/genice2_svg/render_svg.py` & `genice2_svg-2.4.1/genice2_svg/render_svg.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,20 @@
     return sw.path.Path(d=p, **kwargs)
 
 
 def polygon(svg, com, d, **options):
     """
     draw a polygon
     """
-    group = svg.add(svg.g(id='Polygon'))
+    group = svg.add(svg.g(id="Polygon"))
     path = polygon_path(com + d, **options)
     group.add(path)
 
 
-sun = np.array([-1., -1., 2.])
+sun = np.array([-1.0, -1.0, 2.0])
 sun /= np.linalg.norm(sun)
 
 
 def Normal(vs):
     """
     Normal vector (not normalized)
     """
@@ -59,145 +59,164 @@
 
 
 def cylinder_new(svg, v1_, v2_, r, **options):
     """
     draw a 3D cylinder
     """
     logger = getLogger()
-    group = svg.add(svg.g(id='Cylinder'))
+    group = svg.add(svg.g(id="Cylinder"))
     if v1_[2] > v2_[2]:
         v1, v2 = v2_, v1_
     else:
         v1, v2 = v1_, v2_
     dir = v2[:2] - v1[:2]
     angle = atan2(dir[1], dir[0])
     d = v2 - v1
     ratio = d[2] / np.linalg.norm(d)
     L = np.linalg.norm(dir)
     path = cylinder_path(r, ratio, L, **options)
     path.translate(v1[0], v1[1])
     path.rotate(angle * 180 / pi, center=(0, 0))
     group.add(path)
-    u = sw.shapes.Ellipse(center=v2[:2], r=(ratio * r, r),
-                          **options)  # , fill=endfill)
+    u = sw.shapes.Ellipse(center=v2[:2], r=(ratio * r, r), **options)  # , fill=endfill)
     u.rotate(angle * 180 / pi, center=v2[:2])
     group.add(u)
 
 
-def Render(prims, Rsphere, shadow=None, zoom=100, topleft=np.array(
-        [-1., -1.]), size=(50., 50.), bgcolor=None, encode=False):
+def Render(
+    prims,
+    Rsphere,
+    shadow=None,
+    zoom=100,
+    topleft=np.array([-1.0, -1.0]),
+    size=(50.0, 50.0),
+    bgcolor=None,
+    encode=False,
+):
     # encode is dummy parameter.
     logger = getLogger()
     svg = sw.Drawing(
-        size=(
-            "{0}px".format(
-                size[0] *
-                zoom),
-            "{0}px".format(
-                size[1] *
-                zoom)))
+        size=("{0}px".format(size[0] * zoom), "{0}px".format(size[1] * zoom))
+    )
     if bgcolor is not None:
         svg.add(
             svg.rect(
-                insert=(
-                    0,
-                    0),
-                size=(
-                    "{0}px".format(
-                        size[0] *
-                        zoom),
-                    "{0}px".format(
-                        size[1] *
-                        zoom)),
-                fill=bgcolor))
+                insert=(0, 0),
+                size=("{0}px".format(size[0] * zoom), "{0}px".format(size[1] * zoom)),
+                fill=bgcolor,
+            )
+        )
     TL0 = np.zeros(3)
     TL0[:2] = topleft
     shadows = []
-    linedefaults = {"stroke_width": 2,
-                    "stroke": "#000",
-                    "stroke_linejoin": "round",
-                    "stroke_linecap": "round",
-                    }
-    filldefaults = {"stroke_width": 1,
-                    "stroke": "#000",
-                    "fill": "#0ff",
-                    "stroke_linejoin": "round",
-                    "stroke_linecap": "round",
-                    "fill_opacity": 1.0,
-                    }
-    shadowdefaults = {"stroke_width": 0,
-                      "fill": "#888",
-                      "fill_opacity": 0.08,
-                      }
+    linedefaults = {
+        "stroke_width": 2,
+        "stroke": "#000",
+        "stroke_linejoin": "round",
+        "stroke_linecap": "round",
+    }
+    filldefaults = {
+        "stroke_width": 1,
+        "stroke": "#000",
+        "fill": "#0ff",
+        "stroke_linejoin": "round",
+        "stroke_linecap": "round",
+        "fill_opacity": 1.0,
+    }
+    shadowdefaults = {
+        "stroke_width": 0,
+        "fill": "#888",
+        "fill_opacity": 0.08,
+    }
     if shadow is not None:
-        assert shadow[0] == '#' and len(shadow) in (5, 9)
+        assert shadow[0] == "#" and len(shadow) in (5, 9)
         if len(shadow) == 5:
             shadowdefaults["fill"] = shadow[:4]
             shadowdefaults["fill_opacity"] = int(shadow[4], 16) / 15
         else:
             shadowdefaults["fill"] = shadow[:7]
             shadowdefaults["fill_opacity"] = int(shadow[7:], 16) / 255
         r = Rsphere
         Z = np.array([0, 0, 1.0])
-        prims += [[prim[0] - Z * r * 1.4**j, prim[1] + 'S', r * 1.4**j, {}]
-                  for j in range(1, 5) for prim in prims if prim[1] == 'C']
+        prims += [
+            [prim[0] - Z * r * 1.4**j, prim[1] + "S", r * 1.4**j, {}]
+            for j in range(1, 5)
+            for prim in prims
+            if prim[1] == "C"
+        ]
     for prim in sorted(prims, key=lambda x: x[0][2]):
-        if not ((-0.5 < prim[0][0] - topleft[0] < size[0] + 0.5) and
-                (-0.5 < prim[0][1] - topleft[1] < size[1] + 0.5)):
+        if not (
+            (-0.5 < prim[0][0] - topleft[0] < size[0] + 0.5)
+            and (-0.5 < prim[0][1] - topleft[1] < size[1] + 0.5)
+        ):
             continue
         if prim[1] == "L":
             if prim[4] == 0:
                 options = {**linedefaults, **prim[5]}
-                svg.add(sw.shapes.Line(start=(
-                    prim[2][:2] - topleft) * zoom, end=(prim[3][:2] - topleft) * zoom, **options))
+                svg.add(
+                    sw.shapes.Line(
+                        start=(prim[2][:2] - topleft) * zoom,
+                        end=(prim[3][:2] - topleft) * zoom,
+                        **options
+                    )
+                )
             else:
                 options = {**filldefaults, **prim[5]}
                 cylinder_new(
                     svg,
                     (prim[2] - TL0) * zoom,
                     (prim[3] - TL0) * zoom,
                     prim[4] * zoom,
-                    **options)
+                    **options
+                )
         elif prim[1] == "L2":
             if prim[3] == 0:
                 options = {**linedefaults, **prim[4]}
                 s = ((prim[0] + prim[2])[:2] - topleft) * zoom
                 e = ((prim[0] - prim[2])[:2] - topleft) * zoom
                 svg.add(sw.shapes.Line(start=s, end=e, **options))
             else:
                 options = {**filldefaults, **prim[4]}
                 cylinder_new(
                     svg,
                     (prim[0] + prim[2] - TL0) * zoom,
                     (prim[0] - prim[2] - TL0) * zoom,
                     prim[3] * zoom,
-                    **options)
+                    **options
+                )
         elif prim[1] == "P":
             options = prim[3]
             if "fillhs" in options:
                 normal = Normal(prim[2])
                 normal /= np.linalg.norm(normal)
                 cosine = abs(np.dot(sun, normal))
                 hue, sat = options["fillhs"]
                 del options["fillhs"]
                 bri = cosine * 0.5 + 0.5
                 if sat < 0.2:
                     bri *= 0.9
                 if cosine > 0.8:
-                    sat *= (1 - (cosine - 0.8) * 3)
-                r, g, b = colorsys.hsv_to_rgb(hue / 360., sat, bri)
+                    sat *= 1 - (cosine - 0.8) * 3
+                r, g, b = colorsys.hsv_to_rgb(hue / 360.0, sat, bri)
                 rgb = "#{0:x}{1:x}{2:x}".format(
-                    int(r * 15.9), int(g * 15.9), int(b * 15.9))
+                    int(r * 15.9), int(g * 15.9), int(b * 15.9)
+                )
                 options["fill"] = rgb
             options = {**filldefaults, **options}
             polygon(svg, (prim[0] - TL0) * zoom, prim[2] * zoom, **options)
         elif prim[1] == "C":
             options = {**filldefaults, **prim[3]}
             Rsphere = prim[2]
-            svg.add(sw.shapes.Circle(
-                center=(prim[0][:2] - topleft) * zoom, r=Rsphere * zoom, **options))
+            svg.add(
+                sw.shapes.Circle(
+                    center=(prim[0][:2] - topleft) * zoom, r=Rsphere * zoom, **options
+                )
+            )
         elif prim[1] == "CS":
             Rsphere = prim[2]
             options = {**shadowdefaults, **prim[3]}
-            svg.add(sw.shapes.Circle(
-                center=(prim[0][:2] - topleft) * zoom, r=Rsphere * zoom, **options))
+            svg.add(
+                sw.shapes.Circle(
+                    center=(prim[0][:2] - topleft) * zoom, r=Rsphere * zoom, **options
+                )
+            )
     return svg.tostring()
```

