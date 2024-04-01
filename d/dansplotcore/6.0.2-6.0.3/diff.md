# Comparing `tmp/dansplotcore-6.0.2.tar.gz` & `tmp/dansplotcore-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dansplotcore-6.0.2.tar", last modified: Mon Apr  1 23:00:24 2024, max compression
+gzip compressed data, was "dansplotcore-6.0.3.tar", last modified: Mon Apr  1 23:14:04 2024, max compression
```

## Comparing `dansplotcore-6.0.2.tar` & `dansplotcore-6.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/PKG-INFO
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/dansplotcore/
--rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.0.2/dansplotcore/__init__.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.0.2/dansplotcore/media.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     8151 2024-04-01 22:58:56.000000 dansplotcore-6.0.2/dansplotcore/plot.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.0.2/dansplotcore/primitives.py
--rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.0.2/dansplotcore/process.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     9129 2024-04-01 22:57:41.000000 dansplotcore-6.0.2/dansplotcore/show.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.0.2/dansplotcore/transforms.py
--rw-rw-r--   0 dan       (1001) dan       (1001)     7153 2023-10-12 14:02:52.000000 dansplotcore-6.0.2/dansplotcore/vector_text.py
-drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/dansplotcore.egg-info/
--rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/PKG-INFO
--rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/SOURCES.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/dependency_links.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/requires.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-01 23:00:24.000000 dansplotcore-6.0.2/dansplotcore.egg-info/top_level.txt
--rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-01 23:00:24.987144 dansplotcore-6.0.2/setup.cfg
--rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-01 23:00:09.000000 dansplotcore-6.0.2/setup.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/PKG-INFO
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/dansplotcore/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      158 2024-03-11 15:41:59.000000 dansplotcore-6.0.3/dansplotcore/__init__.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     4953 2023-04-05 20:25:28.000000 dansplotcore-6.0.3/dansplotcore/media.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     8151 2024-04-01 22:58:56.000000 dansplotcore-6.0.3/dansplotcore/plot.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2645 2024-03-11 16:06:00.000000 dansplotcore-6.0.3/dansplotcore/primitives.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)      479 2024-03-11 16:06:00.000000 dansplotcore-6.0.3/dansplotcore/process.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     9155 2024-04-01 23:12:44.000000 dansplotcore-6.0.3/dansplotcore/show.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     2907 2024-03-21 21:31:30.000000 dansplotcore-6.0.3/dansplotcore/transforms.py
+-rw-rw-r--   0 dan       (1001) dan       (1001)     7153 2023-10-12 14:02:52.000000 dansplotcore-6.0.3/dansplotcore/vector_text.py
+drwxrwxr-x   0 dan       (1001) dan       (1001)        0 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/dansplotcore.egg-info/
+-rw-rw-r--   0 dan       (1001) dan       (1001)      325 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/PKG-INFO
+-rw-rw-r--   0 dan       (1001) dan       (1001)      382 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/SOURCES.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)        1 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/dependency_links.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       15 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/requires.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       13 2024-04-01 23:14:04.000000 dansplotcore-6.0.3/dansplotcore.egg-info/top_level.txt
+-rw-rw-r--   0 dan       (1001) dan       (1001)       38 2024-04-01 23:14:04.691553 dansplotcore-6.0.3/setup.cfg
+-rw-rw-r--   0 dan       (1001) dan       (1001)      492 2024-04-01 23:13:57.000000 dansplotcore-6.0.3/setup.py
```

### Comparing `dansplotcore-6.0.2/dansplotcore/media.py` & `dansplotcore-6.0.3/dansplotcore/media.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.2/dansplotcore/plot.py` & `dansplotcore-6.0.3/dansplotcore/plot.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.2/dansplotcore/primitives.py` & `dansplotcore-6.0.3/dansplotcore/primitives.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.2/dansplotcore/show.py` & `dansplotcore-6.0.3/dansplotcore/show.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,17 +208,17 @@
             while i < view.x + view.w:
                 s = '{:.5}'.format(i)
                 if view.x + view.w - i > increment:
                     if i == 0 and plot.epochs.get('x') != None:
                         texter.text(
                             plot.epochs['x']['min'].isoformat('\n'),
                             x=i + margin_x,
-                            y=view.y + margin_y + text_h,
-                            w=text_w / 2,
-                            h=text_h / 2,
+                            y=view.y + margin_y + 1.33 * text_h,
+                            w=text_w * 0.66,
+                            h=text_h * 0.66,
                         )
                     else:
                         texter.text(s, x=i+margin_x, y=view.y+margin_y, w=text_w, h=text_h)
                     texter.text('L', i, view.y, text_w * 2, text_h)
                 i += increment
             # draw y axis
             increment = 10 ** math.floor(math.log10(view.h))
@@ -229,17 +229,17 @@
             i = (view.y + text_h + 2*margin_y) // increment * increment + increment
             while i < view.y + view.h - (text_h + 2*margin_y):
                 s = '{:.5}'.format(i)
                 if i == 0 and plot.epochs.get('y') != None:
                     texter.text(
                         plot.epochs['y']['min'].isoformat('\n'),
                         x=view.x + margin_x,
-                        y=i + margin_y + text_h,
-                        w=text_w / 2,
-                        h=text_h / 2,
+                        y=i + margin_y + 1.33 * text_h,
+                        w=text_w * 0.66,
+                        h=text_h * 0.66,
                     )
                 else:
                     texter.text(s, x=view.x+margin_x, y=i+margin_y, w=text_w, h=text_h)
                 texter.text('L', view.x, i, text_w * 2, text_h)
                 i += increment
         plot.buffer_text.data = texter.data
         plot.buffer_text.prep('dynamic')
```

### Comparing `dansplotcore-6.0.2/dansplotcore/transforms.py` & `dansplotcore-6.0.3/dansplotcore/transforms.py`

 * *Files identical despite different names*

### Comparing `dansplotcore-6.0.2/dansplotcore/vector_text.py` & `dansplotcore-6.0.3/dansplotcore/vector_text.py`

 * *Files identical despite different names*

