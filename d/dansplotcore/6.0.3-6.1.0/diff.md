# Comparing `tmp/dansplotcore-6.0.3.tar.gz` & `tmp/dansplotcore-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.0.3.tar", last modified: Mon Apr  1 23:14:04 2024, max compression
+gzip compressed data, was "dansplotcore-6.1.0.tar", last modified: Tue Apr  2 20:20:49 2024, max compression
```

## Comparing `dansplotcore-6.0.3.tar` & `dansplotcore-6.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.0.3/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.0.3/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     8151 2024-04-01 22:58:56.000000 dansplotcore-6.0.3/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.0.3/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.0.3/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9155 2024-04-01 23:12:44.000000 dansplotcore-6.0.3/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.0.3/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7153 2023-10-12 14:02:52.000000 dansplotcore-6.0.3/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-01 23:13:57.000000 dansplotcore-6.0.3/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.1.0/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.1.0/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     8546 2024-04-02 20:04:39.000000 dansplotcore-6.1.0/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.1.0/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.1.0/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9334 2024-04-02 20:13:35.000000 dansplotcore-6.1.0/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.1.0/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7455 2024-04-02 20:00:09.000000 dansplotcore-6.1.0/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-02 20:20:49.000000 dansplotcore-6.1.0/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-02 20:20:49.215951 dansplotcore-6.1.0/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-02 20:06:28.000000 dansplotcore-6.1.0/setup.py
```

### Comparing `dansplotcore-6.0.3/dansplotcore/media.py` & `dansplotcore-6.1.0/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.3/dansplotcore/plot.py` & `dansplotcore-6.1.0/dansplotcore/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from . import primitives
 from . import transforms
+from . import vector_text
 
 import datetime
 import math
 
 class Plot:
     def __init__(
         self,
@@ -18,14 +19,15 @@
     ):
         self.title = title
         self.points = []
         self.lines = []
         self.rects = []
         self.late_vertexors = []
         self.texts = []
+        self.static_texter = vector_text.Texter()
         self.x_min =  math.inf
         self.x_max = -math.inf
         self.y_min =  math.inf
         self.y_max = -math.inf
         self.epochs = {}
         self.series = 0
         self.transform = transform or transforms.Default()
@@ -54,14 +56,21 @@
         self._include(x, y)
 
     def text(self, s, x, y, r=255, g=255, b=255, a=255, max_w=math.inf, max_h=math.inf, scale=10):
         '`scale` is the number of pixels between the left side of each character.'
         self.texts.append([s, x, y, r, g, b, a, max_w, max_h, scale])
         self._include(x, y)
 
+    def text_static(self, s, x, y, w=1, h=1, r=255, g=255, b=255, a=255):
+        '`w` and `h` are for a single character.'
+        if not s: return
+        self.static_texter.text(s, x, y, w, h, r, g, b, a)
+        self._include(*self.static_texter.bounds[0:2])
+        self._include(*self.static_texter.bounds[2:4])
+
     def show(self, w=640, h=480):
         from .show import show
         show(self, w, h)
 
     def plot_list(self, l, **kwargs):
         for i, v in enumerate(l):
             self.primitive(**self.transform(i, v, i, self.series))
```

### Comparing `dansplotcore-6.0.3/dansplotcore/primitives.py` & `dansplotcore-6.1.0/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.3/dansplotcore/show.py` & `dansplotcore-6.1.0/dansplotcore/show.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,18 +65,21 @@
             plot.original_lines = copy.copy(plot.lines)
         for vertexor, x, y, r, g, b, a in plot.late_vertexors:
             vertexor(plot, view, w, h, x, y, r, g, b, a)
     # points
     for x, y, r, g, b, a in plot.points:
         plot.buffer.add(x, y, *fcolor(r, g, b, a))
     points_f = len(plot.buffer)
-    # lines
+    # lines & static text
     for xi, yi, xf, yf, r, g, b, a in plot.lines:
         plot.buffer.add(xi, yi, *fcolor(r, g, b, a))
         plot.buffer.add(xf, yf, *fcolor(r, g, b, a))
+    for i in range(0, len(plot.static_texter.data), 6):
+        x, y, r, g, b, a = plot.static_texter.data[i:i+6]
+        plot.buffer.add(x, y, *fcolor(r, g, b, a))
     lines_f = len(plot.buffer)
     # rects
     for xi, yi, xf, yf, r, g, b, a in plot.rects:
         plot.buffer.add(xi, yi, *fcolor(r, g, b, a))
         plot.buffer.add(xf, yf, *fcolor(r, g, b, a))
         plot.buffer.add(xi, yf, *fcolor(r, g, b, a))
         plot.buffer.add(xi, yi, *fcolor(r, g, b, a))
```

### Comparing `dansplotcore-6.0.3/dansplotcore/transforms.py` & `dansplotcore-6.1.0/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.3/dansplotcore/vector_text.py` & `dansplotcore-6.1.0/dansplotcore/vector_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -213,23 +213,30 @@
     # glyph for unhandled character
     None: ['O', 'N7I', 'N3I', 'N1I', 'N9I'],
 }
 
 class Texter:
     def __init__(self):
         self.data = [];
+        self.bounds = None
 
     def text(self, s, x, y, w, h, r=1.0, g=1.0, b=1.0, a=1.0):
+        if not self.bounds:
+            self.bounds = [x, y, x, y]
         x_i = x
         for c in s:
             self.glyph(c, x, y, w, h, r, g, b, a)
             x += w
+            self.bounds[0] = min(self.bounds[0], x)
+            self.bounds[2] = max(self.bounds[2], x)
             if c == '\n':
                 x = x_i
                 y -= h * 2
+            self.bounds[1] = min(self.bounds[1], y)
+            self.bounds[3] = max(self.bounds[3], y)
 
     def glyph(self, c, x, y, w, h, r, g, b, a):
         glyph = glyphs.get(c, glyphs[None])
         i = 0
         while i < len(glyph):
             if type(glyph[i]) == str:
                 self.glyph(glyph[i], x, y, w, h, r, g, b, a)
```

