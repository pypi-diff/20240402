# Comparing `tmp/dansplotcore-6.0.0.tar.gz` & `tmp/dansplotcore-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.0.0.tar", last modified: Thu Mar 21 21:41:10 2024, max compression
+gzip compressed data, was "dansplotcore-6.0.1.tar", last modified: Mon Apr  1 22:34:12 2024, max compression
```

## Comparing `dansplotcore-6.0.0.tar` & `dansplotcore-6.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-03-21 21:41:10.298836 dansplotcore-6.0.0/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-03-21 21:41:10.298836 dansplotcore-6.0.0/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-03-21 21:41:10.298836 dansplotcore-6.0.0/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.0.0/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.0.0/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     8067 2024-03-21 21:39:40.000000 dansplotcore-6.0.0/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.0.0/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.0.0/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7640 2024-03-13 18:12:37.000000 dansplotcore-6.0.0/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.0.0/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7153 2023-10-12 14:02:52.000000 dansplotcore-6.0.0/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-03-21 21:41:10.298836 dansplotcore-6.0.0/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-03-21 21:41:10.000000 dansplotcore-6.0.0/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-03-21 21:41:10.000000 dansplotcore-6.0.0/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-03-21 21:41:10.000000 dansplotcore-6.0.0/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-03-21 21:41:10.000000 dansplotcore-6.0.0/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-03-21 21:41:10.000000 dansplotcore-6.0.0/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-03-21 21:41:10.298836 dansplotcore-6.0.0/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-03-21 21:40:42.000000 dansplotcore-6.0.0/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 22:34:12.055562 dansplotcore-6.0.1/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 22:34:12.055562 dansplotcore-6.0.1/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 22:34:12.051562 dansplotcore-6.0.1/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.0.1/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.0.1/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7785 2024-04-01 22:26:57.000000 dansplotcore-6.0.1/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.0.1/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.0.1/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9135 2024-04-01 22:33:15.000000 dansplotcore-6.0.1/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.0.1/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7153 2023-10-12 14:02:52.000000 dansplotcore-6.0.1/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 22:34:12.051562 dansplotcore-6.0.1/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-01 22:34:12.055562 dansplotcore-6.0.1/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-01 22:34:03.000000 dansplotcore-6.0.1/setup.py
```

### Comparing `dansplotcore-6.0.0/dansplotcore/media.py` & `dansplotcore-6.0.1/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.0/dansplotcore/plot.py` & `dansplotcore-6.0.1/dansplotcore/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,34 +32,28 @@
         self.hide_axes = hide_axes
         self.set_primitive(primitive or primitives.Point())
         self.datetime_unit = datetime_unit
         self.legend_displacement = legend_displacement
         self.legend_offset = legend_offset
 
     def point(self, x, y, r=255, g=255, b=255, a=255):
-        x, y = self._to_screen(x, y)
         self.points.append([x, y, r, g, b, a])
         self._include(x, y)
 
     def line(self, xi, yi, xf, yf, r=255, g=255, b=255, a=255):
-        xi, yi = self._to_screen(xi, yi)
-        xf, yf = self._to_screen(xf, yf)
         self.lines.append([xi, yi, xf, yf, r, g, b, a])
         self._include(xi, yi)
         self._include(xf, yf)
 
     def rect(self, xi, yi, xf, yf, r=255, g=255, b=255, a=255):
-        xi, yi = self._to_screen(xi, yi)
-        xf, yf = self._to_screen(xf, yf)
         self.rects.append([xi, yi, xf, yf, r, g, b, a])
         self._include(xi, yi)
         self._include(xf, yf)
 
     def late_vertexor(self, vertexor, x, y, r=255, g=255, b=255, a=255):
-        x, y = self._to_screen(x, y)
         self.late_vertexors.append([vertexor, x, y, r, g, b, a])
         self._include(x, y)
 
     def text(self, s, x, y, r=255, g=255, b=255, a=255, max_w=math.inf, max_h=math.inf, scale=10):
         '`scale` is the number of pixels between the left side of each character.'
         self.texts.append([s, x, y, r, g, b, a, max_w, max_h, scale])
         self._include(x, y)
@@ -160,28 +154,25 @@
         self.series += 1
         self.primitive.reset()
 
     def set_primitive(self, primitive):
         self.primitive = primitive.set_plot(self)
 
     def _include(self, x, y):
+        if type(x) == datetime.datetime and type(self.x_min) != datetime.datetime:
+            self.x_min = x
+            self.x_max = x
+        if type(y) == datetime.datetime and type(self.y_min) != datetime.datetime:
+            self.y_min = y
+            self.y_max = y
         self.x_min = min(x, self.x_min)
         self.x_max = max(x, self.x_max)
         self.y_min = min(y, self.y_min)
         self.y_max = max(y, self.y_max)
 
-    def _to_screen(self, x, y):
-        c = [x, y]
-        for i, v in enumerate(c):
-            if type(v) == datetime.datetime:
-                if i not in self.epochs:
-                    self.epochs[i] = v
-                c[i] = (v - self.epochs[i]).total_seconds() / self.datetime_unit
-        return c[0], c[1]
-
     def _plot_common(
         self,
         next_series=True,
         legend=None,
         **kwargs,
     ):
         if legend:
```

### Comparing `dansplotcore-6.0.0/dansplotcore/primitives.py` & `dansplotcore-6.0.1/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.0/dansplotcore/transforms.py` & `dansplotcore-6.0.1/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.0/dansplotcore/vector_text.py` & `dansplotcore-6.0.1/dansplotcore/vector_text.py`

 * *Files identical despite different names*

