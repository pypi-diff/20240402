# Comparing `tmp/dansplotcore-6.0.1.tar.gz` & `tmp/dansplotcore-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.0.1.tar", last modified: Mon Apr  1 22:34:12 2024, max compression
+gzip compressed data, was "dansplotcore-6.0.2.tar", last modified: Mon Apr  1 23:00:24 2024, max compression
```

## Comparing `dansplotcore-6.0.1.tar` & `dansplotcore-6.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 22:34:12.055562 dansplotcore-6.0.1/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 22:34:12.055562 dansplotcore-6.0.1/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 22:34:12.051562 dansplotcore-6.0.1/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.0.1/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.0.1/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7785 2024-04-01 22:26:57.000000 dansplotcore-6.0.1/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.0.1/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.0.1/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9135 2024-04-01 22:33:15.000000 dansplotcore-6.0.1/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.0.1/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7153 2023-10-12 14:02:52.000000 dansplotcore-6.0.1/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 22:34:12.051562 dansplotcore-6.0.1/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-01 22:34:12.000000 dansplotcore-6.0.1/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-01 22:34:12.055562 dansplotcore-6.0.1/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-01 22:34:03.000000 dansplotcore-6.0.1/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.0.2/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.0.2/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     8151 2024-04-01 22:58:56.000000 dansplotcore-6.0.2/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.0.2/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.0.2/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9129 2024-04-01 22:57:41.000000 dansplotcore-6.0.2/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.0.2/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7153 2023-10-12 14:02:52.000000 dansplotcore-6.0.2/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-01 23:00:09.000000 dansplotcore-6.0.2/setup.py
```

### Comparing `dansplotcore-6.0.1/dansplotcore/media.py` & `dansplotcore-6.0.2/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.1/dansplotcore/plot.py` & `dansplotcore-6.0.2/dansplotcore/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,24 +154,32 @@
         self.series += 1
         self.primitive.reset()
 
     def set_primitive(self, primitive):
         self.primitive = primitive.set_plot(self)
 
     def _include(self, x, y):
-        if type(x) == datetime.datetime and type(self.x_min) != datetime.datetime:
-            self.x_min = x
-            self.x_max = x
-        if type(y) == datetime.datetime and type(self.y_min) != datetime.datetime:
-            self.y_min = y
-            self.y_max = y
-        self.x_min = min(x, self.x_min)
-        self.x_max = max(x, self.x_max)
-        self.y_min = min(y, self.y_min)
-        self.y_max = max(y, self.y_max)
+        if type(x) == datetime.datetime:
+            if 'x' in self.epochs:
+                self.epochs['x']['min'] = min(x, self.epochs['x']['min'])
+                self.epochs['x']['max'] = max(x, self.epochs['x']['max'])
+            else:
+                self.epochs['x'] = {'min': x, 'max': x}
+        else:
+            self.x_min = min(x, self.x_min)
+            self.x_max = max(x, self.x_max)
+        if type(y) == datetime.datetime:
+            if 'y' in self.epochs:
+                self.epochs['y']['min'] = min(y, self.epochs['y']['min'])
+                self.epochs['y']['max'] = max(y, self.epochs['y']['max'])
+            else:
+                self.epochs['y'] = {'min': y, 'max': y}
+        else:
+            self.y_min = min(y, self.y_min)
+            self.y_max = max(y, self.y_max)
 
     def _plot_common(
         self,
         next_series=True,
         legend=None,
         **kwargs,
     ):
```

### Comparing `dansplotcore-6.0.1/dansplotcore/primitives.py` & `dansplotcore-6.0.2/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.1/dansplotcore/show.py` & `dansplotcore-6.0.2/dansplotcore/show.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,45 +18,43 @@
         i if type(i) == float else i/255
         for i in [r, g, b, a]
     ]
 
 def translate_x_date(plot, list_, component):
     for i in list_:
         x = i[component]
-        x = (x - plot.x_min).total_seconds() / plot.datetime_unit
+        x = (x - plot.epochs['x']['min']).total_seconds() / plot.datetime_unit
         i[component] = x
 
 def translate_y_date(plot, list_, component):
     for i in list_:
         y = i[component]
-        y = (y - plot.y_min).total_seconds() / plot.datetime_unit
+        y = (y - plot.epochs['y']['min']).total_seconds() / plot.datetime_unit
         i[component] = y
 
 def translate_dates(plot):
-    if type(plot.x_min) != datetime.datetime and type(plot.y_min) != datetime.datetime: return
-    if type(plot.x_min) == datetime.datetime:
+    if not plot.epochs: return
+    if 'x' in plot.epochs:
         translate_x_date(plot, plot.late_vertexors, 1)
         translate_x_date(plot, plot.points, 0)
         translate_x_date(plot, plot.lines, 0)
         translate_x_date(plot, plot.lines, 2)
         translate_x_date(plot, plot.rects, 0)
         translate_x_date(plot, plot.rects, 2)
-        plot.epochs[0] = plot.x_min
-        plot.x_max = (plot.x_max - plot.x_min).total_seconds() / plot.datetime_unit
-        plot.x_min = 0
-    if type(plot.y_min) == datetime.datetime:
+        plot.x_max = max(plot.x_max, (plot.epochs['x']['max'] - plot.epochs['x']['min']).total_seconds() / plot.datetime_unit)
+        plot.x_min = min(plot.x_min, 0)
+    if 'y' in plot.epochs:
         translate_y_date(plot, plot.late_vertexors, 2)
         translate_y_date(plot, plot.points, 1)
         translate_y_date(plot, plot.lines, 1)
         translate_y_date(plot, plot.lines, 3)
         translate_y_date(plot, plot.rects, 1)
         translate_y_date(plot, plot.rects, 3)
-        plot.epochs[1] = plot.y_min
-        plot.y_max = (plot.y_max - plot.y_min).total_seconds() / plot.datetime_unit
-        plot.y_min = 0
+        plot.y_max = max(plot.y_max, (plot.epochs['y']['max'] - plot.epochs['y']['min']).total_seconds() / plot.datetime_unit)
+        plot.y_min = min(plot.y_min, 0)
 
 def construct(plot, view, w, h):
     plot.buffer = media.Buffer()
     plot.buffer_text = media.Buffer()
     # late vertexors
     if plot.late_vertexors:
         if hasattr(plot, 'original_points'):
@@ -206,17 +204,17 @@
                 increment /= 5
             elif view.w / increment < 5:
                 increment /= 2
             i = view.x // increment * increment + increment
             while i < view.x + view.w:
                 s = '{:.5}'.format(i)
                 if view.x + view.w - i > increment:
-                    if i == 0 and plot.epochs.get(0) != None:
+                    if i == 0 and plot.epochs.get('x') != None:
                         texter.text(
-                            plot.epochs[0].isoformat('\n'),
+                            plot.epochs['x']['min'].isoformat('\n'),
                             x=i + margin_x,
                             y=view.y + margin_y + text_h,
                             w=text_w / 2,
                             h=text_h / 2,
                         )
                     else:
                         texter.text(s, x=i+margin_x, y=view.y+margin_y, w=text_w, h=text_h)
@@ -227,17 +225,17 @@
             if view.h / increment < 2:
                 increment /= 5
             elif view.h / increment < 5:
                 increment /= 2
             i = (view.y + text_h + 2*margin_y) // increment * increment + increment
             while i < view.y + view.h - (text_h + 2*margin_y):
                 s = '{:.5}'.format(i)
-                if i == 0 and plot.epochs.get(1) != None:
+                if i == 0 and plot.epochs.get('y') != None:
                     texter.text(
-                        plot.epochs[1].isoformat('\n'),
+                        plot.epochs['y']['min'].isoformat('\n'),
                         x=view.x + margin_x,
                         y=i + margin_y + text_h,
                         w=text_w / 2,
                         h=text_h / 2,
                     )
                 else:
                     texter.text(s, x=view.x+margin_x, y=i+margin_y, w=text_w, h=text_h)
```

### Comparing `dansplotcore-6.0.1/dansplotcore/transforms.py` & `dansplotcore-6.0.2/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.1/dansplotcore/vector_text.py` & `dansplotcore-6.0.2/dansplotcore/vector_text.py`

 * *Files identical despite different names*

