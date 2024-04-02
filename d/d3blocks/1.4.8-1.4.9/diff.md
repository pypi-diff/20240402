# Comparing `tmp/d3blocks-1.4.8.tar.gz` & `tmp/d3blocks-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d3blocks-1.4.8.tar", last modified: Sat Dec  9 22:01:47 2023, max compression
+gzip compressed data, was "d3blocks-1.4.9.tar", last modified: Mon Dec 11 22:34:10 2023, max compression
```

## Comparing `d3blocks-1.4.8.tar` & `d3blocks-1.4.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:47.030414 d3blocks-1.4.8/
--rw-rw-rw-   0        0        0    35837 2023-09-23 10:16:01.000000 d3blocks-1.4.8/LICENSE
--rw-rw-rw-   0        0        0      474 2023-09-23 10:16:01.000000 d3blocks-1.4.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8612 2023-12-09 22:01:47.014781 d3blocks-1.4.8/PKG-INFO
--rw-rw-rw-   0        0        0     8104 2023-09-23 10:16:01.000000 d3blocks-1.4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.762787 d3blocks-1.4.8/d3blocks/
--rw-rw-rw-   0        0        0     1621 2023-12-09 21:59:57.000000 d3blocks-1.4.8/d3blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.794754 d3blocks-1.4.8/d3blocks/chord/
--rw-rw-rw-   0        0        0    14235 2023-11-12 17:14:20.000000 d3blocks-1.4.8/d3blocks/chord/Chord.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/chord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.794754 d3blocks-1.4.8/d3blocks/chord/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/chord/d3js/__init__.py
--rw-rw-rw-   0        0        0     1253 2023-11-12 16:34:33.000000 d3blocks-1.4.8/d3blocks/chord/d3js/chord.html.j2
--rw-rw-rw-   0        0        0    59634 2023-10-17 21:01:24.000000 d3blocks-1.4.8/d3blocks/chord/d3js/chord.js
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.810391 d3blocks-1.4.8/d3blocks/circlepacking/
--rw-rw-rw-   0        0        0     7060 2023-11-12 17:13:51.000000 d3blocks-1.4.8/d3blocks/circlepacking/Circlepacking.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/circlepacking/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.810391 d3blocks-1.4.8/d3blocks/circlepacking/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/circlepacking/d3js/__init__.py
--rw-rw-rw-   0        0        0     6277 2023-11-12 17:03:42.000000 d3blocks-1.4.8/d3blocks/circlepacking/d3js/circlepacking.html.j2
--rw-rw-rw-   0        0        0   270687 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/circlepacking/d3js/d3.v6.min.js
--rw-rw-rw-   0        0        0    73154 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/circlepacking/d3js/lodash.min.js
--rw-rw-rw-   0        0        0   147544 2023-12-09 21:58:12.000000 d3blocks-1.4.8/d3blocks/d3blocks.py
--rw-rw-rw-   0        0        0    87594 2023-12-09 21:55:04.000000 d3blocks-1.4.8/d3blocks/examples.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.826003 d3blocks-1.4.8/d3blocks/heatmap/
--rw-rw-rw-   0        0        0    12112 2023-11-12 17:55:59.000000 d3blocks-1.4.8/d3blocks/heatmap/Heatmap.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/heatmap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.857260 d3blocks-1.4.8/d3blocks/heatmap/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/heatmap/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js
--rw-rw-rw-   0        0        0   978290 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/heatmap/d3js/d3.v4.js
--rw-rw-rw-   0        0        0   125978 2023-11-12 17:54:56.000000 d3blocks-1.4.8/d3blocks/heatmap/d3js/heatmap.html.j2
--rw-rw-rw-   0        0        0     4569 2023-11-12 16:50:51.000000 d3blocks-1.4.8/d3blocks/heatmap/d3js/matrix.html.j2
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.857260 d3blocks-1.4.8/d3blocks/imageslider/
--rw-rw-rw-   0        0        0     8638 2023-11-12 18:39:46.000000 d3blocks-1.4.8/d3blocks/imageslider/Imageslider.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/imageslider/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.904739 d3blocks-1.4.8/d3blocks/imageslider/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/imageslider/d3js/.keep
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/imageslider/d3js/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-11-12 18:44:04.000000 d3blocks-1.4.8/d3blocks/imageslider/d3js/imageslider.html.j2
--rw-rw-rw-   0        0        0   256541 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/imageslider/d3js/jquery-2.1.1.js
--rw-rw-rw-   0        0        0     5543 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/imageslider/d3js/main.js
--rw-rw-rw-   0        0        0    52757 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/imageslider/d3js/modernizr.js
--rw-rw-rw-   0        0        0      989 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/imageslider/d3js/reset.css
--rw-rw-rw-   0        0        0     4326 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/imageslider/d3js/style.css
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.904739 d3blocks-1.4.8/d3blocks/maps/
--rw-rw-rw-   0        0        0     8479 2023-11-12 18:50:39.000000 d3blocks-1.4.8/d3blocks/maps/Maps.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/maps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.920372 d3blocks-1.4.8/d3blocks/maps/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/maps/d3js/__init__.py
--rw-rw-rw-   0        0        0   270687 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/maps/d3js/d3.v6.min.js
--rw-rw-rw-   0        0        0     7620 2023-11-12 18:51:27.000000 d3blocks-1.4.8/d3blocks/maps/d3js/maps.html.j2
--rw-rw-rw-   0        0        0   252663 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/maps/d3js/world.geojson
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.920372 d3blocks-1.4.8/d3blocks/matrix/
--rw-rw-rw-   0        0        0     9568 2023-11-12 17:56:16.000000 d3blocks-1.4.8/d3blocks/matrix/Matrix.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/matrix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.935989 d3blocks-1.4.8/d3blocks/matrix/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/matrix/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js
--rw-rw-rw-   0        0        0   978290 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/matrix/d3js/d3.v4.js
--rw-rw-rw-   0        0        0     4483 2023-11-12 17:55:00.000000 d3blocks-1.4.8/d3blocks/matrix/d3js/matrix.html.j2
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.935989 d3blocks-1.4.8/d3blocks/movingbubbles/
--rw-rw-rw-   0        0        0    24802 2023-11-12 18:55:34.000000 d3blocks-1.4.8/d3blocks/movingbubbles/Movingbubbles.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/movingbubbles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.951620 d3blocks-1.4.8/d3blocks/movingbubbles/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/movingbubbles/d3js/__init__.py
--rw-rw-rw-   0        0        0   151129 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js
--rw-rw-rw-   0        0        0    10692 2023-11-12 19:04:58.000000 d3blocks-1.4.8/d3blocks/movingbubbles/d3js/movingbubbles.html.j2
--rw-rw-rw-   0        0        0     1901 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/movingbubbles/d3js/style.css
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.951620 d3blocks-1.4.8/d3blocks/particles/
--rw-rw-rw-   0        0        0     2322 2023-11-12 19:12:55.000000 d3blocks-1.4.8/d3blocks/particles/Particles.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/particles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.951620 d3blocks-1.4.8/d3blocks/particles/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/particles/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js
--rw-rw-rw-   0        0        0   221958 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/particles/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     6813 2023-11-12 19:14:22.000000 d3blocks-1.4.8/d3blocks/particles/d3js/particles.html.j2
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.951620 d3blocks-1.4.8/d3blocks/sankey/
--rw-rw-rw-   0        0        0    11003 2023-12-09 21:53:12.000000 d3blocks-1.4.8/d3blocks/sankey/Sankey.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/sankey/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.967193 d3blocks-1.4.8/d3blocks/sankey/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/sankey/d3js/__init__.py
--rw-rw-rw-   0        0        0     3910 2023-11-12 19:23:40.000000 d3blocks-1.4.8/d3blocks/sankey/d3js/sankey.html.j2
--rw-rw-rw-   0        0        0    73715 2023-12-09 21:54:42.000000 d3blocks-1.4.8/d3blocks/sankey/d3js/sankey.js
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.967193 d3blocks-1.4.8/d3blocks/scatter/
--rw-rw-rw-   0        0        0    16216 2023-11-12 19:29:39.000000 d3blocks-1.4.8/d3blocks/scatter/Scatter.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/scatter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.973807 d3blocks-1.4.8/d3blocks/scatter/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/scatter/d3js/__init__.py
--rw-rw-rw-   0        0        0   221958 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/scatter/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     7165 2023-11-12 19:39:58.000000 d3blocks-1.4.8/d3blocks/scatter/d3js/scatter.html.j2
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.973807 d3blocks-1.4.8/d3blocks/tests/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/tests/__init__.py
--rw-rw-rw-   0        0        0    23380 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/tests/test_d3blocks.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.983419 d3blocks-1.4.8/d3blocks/timeseries/
--rw-rw-rw-   0        0        0     9711 2023-11-12 19:41:59.000000 d3blocks-1.4.8/d3blocks/timeseries/Timeseries.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/timeseries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.983419 d3blocks-1.4.8/d3blocks/timeseries/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/timeseries/d3js/__init__.py
--rw-rw-rw-   0        0        0   347498 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/timeseries/d3js/d3.v3.js
--rw-rw-rw-   0        0        0    15492 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/timeseries/d3js/script.js
--rw-rw-rw-   0        0        0      735 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/timeseries/d3js/style.css
--rw-rw-rw-   0        0        0     1098 2023-11-12 19:42:53.000000 d3blocks-1.4.8/d3blocks/timeseries/d3js/timeseries.html.j2
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.983419 d3blocks-1.4.8/d3blocks/tree/
--rw-rw-rw-   0        0        0     6525 2023-11-12 19:50:55.000000 d3blocks-1.4.8/d3blocks/tree/Tree.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.999161 d3blocks-1.4.8/d3blocks/tree/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/tree/d3js/__init__.py
--rw-rw-rw-   0        0        0    28939 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/tree/d3js/d3.tree.js
--rw-rw-rw-   0        0        0   231140 2023-11-12 19:52:16.000000 d3blocks-1.4.8/d3blocks/tree/d3js/tree.html.j2
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.999161 d3blocks-1.4.8/d3blocks/treemap/
--rw-rw-rw-   0        0        0     6144 2023-11-12 20:00:01.000000 d3blocks-1.4.8/d3blocks/treemap/Treemap.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/treemap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.999161 d3blocks-1.4.8/d3blocks/treemap/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/treemap/d3js/__init__.py
--rw-rw-rw-   0        0        0   221958 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/treemap/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     3370 2023-11-12 20:02:36.000000 d3blocks-1.4.8/d3blocks/treemap/d3js/treemap.html.j2
--rw-rw-rw-   0        0        0    27740 2023-11-12 20:14:39.000000 d3blocks-1.4.8/d3blocks/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:47.014781 d3blocks-1.4.8/d3blocks/violin/
--rw-rw-rw-   0        0        0    11759 2023-11-12 20:06:03.000000 d3blocks-1.4.8/d3blocks/violin/Violin.py
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/violin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:47.014781 d3blocks-1.4.8/d3blocks/violin/d3js/
--rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/violin/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js
--rw-rw-rw-   0        0        0   221958 2023-09-23 10:16:01.000000 d3blocks-1.4.8/d3blocks/violin/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     6785 2023-11-12 20:12:54.000000 d3blocks-1.4.8/d3blocks/violin/d3js/violin.html.j2
-drwxrwxrwx   0        0        0        0 2023-12-09 22:01:46.794754 d3blocks-1.4.8/d3blocks.egg-info/
--rw-rw-rw-   0        0        0     8612 2023-12-09 22:01:46.000000 d3blocks-1.4.8/d3blocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3289 2023-12-09 22:01:46.000000 d3blocks-1.4.8/d3blocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-09 22:01:46.000000 d3blocks-1.4.8/d3blocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-12-09 22:01:46.000000 d3blocks-1.4.8/d3blocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-12-09 22:01:46.000000 d3blocks-1.4.8/d3blocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-09 22:01:47.030414 d3blocks-1.4.8/setup.cfg
--rw-rw-rw-   0        0        0     1757 2023-10-17 18:22:48.000000 d3blocks-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.717382 d3blocks-1.4.9/
+-rw-rw-rw-   0        0        0    35837 2023-09-23 10:16:01.000000 d3blocks-1.4.9/LICENSE
+-rw-rw-rw-   0        0        0      474 2023-09-23 10:16:01.000000 d3blocks-1.4.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8612 2023-12-11 22:34:10.717382 d3blocks-1.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0     8104 2023-09-23 10:16:01.000000 d3blocks-1.4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.356245 d3blocks-1.4.9/d3blocks/
+-rw-rw-rw-   0        0        0     1621 2023-12-11 22:30:37.000000 d3blocks-1.4.9/d3blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.403089 d3blocks-1.4.9/d3blocks/chord/
+-rw-rw-rw-   0        0        0    14235 2023-11-12 17:14:20.000000 d3blocks-1.4.9/d3blocks/chord/Chord.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/chord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.418712 d3blocks-1.4.9/d3blocks/chord/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/chord/d3js/__init__.py
+-rw-rw-rw-   0        0        0     1253 2023-11-12 16:34:33.000000 d3blocks-1.4.9/d3blocks/chord/d3js/chord.html.j2
+-rw-rw-rw-   0        0        0    59634 2023-10-17 21:01:24.000000 d3blocks-1.4.9/d3blocks/chord/d3js/chord.js
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.418712 d3blocks-1.4.9/d3blocks/circlepacking/
+-rw-rw-rw-   0        0        0     7060 2023-11-12 17:13:51.000000 d3blocks-1.4.9/d3blocks/circlepacking/Circlepacking.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/circlepacking/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.434805 d3blocks-1.4.9/d3blocks/circlepacking/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/circlepacking/d3js/__init__.py
+-rw-rw-rw-   0        0        0     6277 2023-11-12 17:03:42.000000 d3blocks-1.4.9/d3blocks/circlepacking/d3js/circlepacking.html.j2
+-rw-rw-rw-   0        0        0   270687 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/circlepacking/d3js/d3.v6.min.js
+-rw-rw-rw-   0        0        0    73154 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/circlepacking/d3js/lodash.min.js
+-rw-rw-rw-   0        0        0   147934 2023-12-11 22:29:12.000000 d3blocks-1.4.9/d3blocks/d3blocks.py
+-rw-rw-rw-   0        0        0    89819 2023-12-11 22:28:55.000000 d3blocks-1.4.9/d3blocks/examples.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.450494 d3blocks-1.4.9/d3blocks/heatmap/
+-rw-rw-rw-   0        0        0    12112 2023-11-12 17:55:59.000000 d3blocks-1.4.9/d3blocks/heatmap/Heatmap.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/heatmap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.466092 d3blocks-1.4.9/d3blocks/heatmap/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/heatmap/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   978290 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/heatmap/d3js/d3.v4.js
+-rw-rw-rw-   0        0        0   125978 2023-11-12 17:54:56.000000 d3blocks-1.4.9/d3blocks/heatmap/d3js/heatmap.html.j2
+-rw-rw-rw-   0        0        0     4569 2023-11-12 16:50:51.000000 d3blocks-1.4.9/d3blocks/heatmap/d3js/matrix.html.j2
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.466092 d3blocks-1.4.9/d3blocks/imageslider/
+-rw-rw-rw-   0        0        0     8638 2023-11-12 18:39:46.000000 d3blocks-1.4.9/d3blocks/imageslider/Imageslider.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/imageslider/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.512997 d3blocks-1.4.9/d3blocks/imageslider/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/imageslider/d3js/.keep
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/imageslider/d3js/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-11-12 18:44:04.000000 d3blocks-1.4.9/d3blocks/imageslider/d3js/imageslider.html.j2
+-rw-rw-rw-   0        0        0   256541 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/imageslider/d3js/jquery-2.1.1.js
+-rw-rw-rw-   0        0        0     5543 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/imageslider/d3js/main.js
+-rw-rw-rw-   0        0        0    52757 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/imageslider/d3js/modernizr.js
+-rw-rw-rw-   0        0        0      989 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/imageslider/d3js/reset.css
+-rw-rw-rw-   0        0        0     4326 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/imageslider/d3js/style.css
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.533657 d3blocks-1.4.9/d3blocks/maps/
+-rw-rw-rw-   0        0        0     8479 2023-11-12 18:50:39.000000 d3blocks-1.4.9/d3blocks/maps/Maps.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/maps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.576150 d3blocks-1.4.9/d3blocks/maps/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/maps/d3js/__init__.py
+-rw-rw-rw-   0        0        0   270687 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/maps/d3js/d3.v6.min.js
+-rw-rw-rw-   0        0        0     7620 2023-11-12 18:51:27.000000 d3blocks-1.4.9/d3blocks/maps/d3js/maps.html.j2
+-rw-rw-rw-   0        0        0   252663 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/maps/d3js/world.geojson
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.576150 d3blocks-1.4.9/d3blocks/matrix/
+-rw-rw-rw-   0        0        0     9568 2023-11-12 17:56:16.000000 d3blocks-1.4.9/d3blocks/matrix/Matrix.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/matrix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.622935 d3blocks-1.4.9/d3blocks/matrix/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/matrix/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   978290 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/matrix/d3js/d3.v4.js
+-rw-rw-rw-   0        0        0     4483 2023-11-12 17:55:00.000000 d3blocks-1.4.9/d3blocks/matrix/d3js/matrix.html.j2
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.639168 d3blocks-1.4.9/d3blocks/movingbubbles/
+-rw-rw-rw-   0        0        0    24802 2023-11-12 18:55:34.000000 d3blocks-1.4.9/d3blocks/movingbubbles/Movingbubbles.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/movingbubbles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.639168 d3blocks-1.4.9/d3blocks/movingbubbles/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/movingbubbles/d3js/__init__.py
+-rw-rw-rw-   0        0        0   151129 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js
+-rw-rw-rw-   0        0        0    10692 2023-11-12 19:04:58.000000 d3blocks-1.4.9/d3blocks/movingbubbles/d3js/movingbubbles.html.j2
+-rw-rw-rw-   0        0        0     1901 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/movingbubbles/d3js/style.css
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.639168 d3blocks-1.4.9/d3blocks/particles/
+-rw-rw-rw-   0        0        0     2322 2023-11-12 19:12:55.000000 d3blocks-1.4.9/d3blocks/particles/Particles.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/particles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.654919 d3blocks-1.4.9/d3blocks/particles/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/particles/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   221958 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/particles/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     6813 2023-11-12 19:14:22.000000 d3blocks-1.4.9/d3blocks/particles/d3js/particles.html.j2
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.654919 d3blocks-1.4.9/d3blocks/sankey/
+-rw-rw-rw-   0        0        0    11716 2023-12-11 22:21:52.000000 d3blocks-1.4.9/d3blocks/sankey/Sankey.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/sankey/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.654919 d3blocks-1.4.9/d3blocks/sankey/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/sankey/d3js/__init__.py
+-rw-rw-rw-   0        0        0     3910 2023-11-12 19:23:40.000000 d3blocks-1.4.9/d3blocks/sankey/d3js/sankey.html.j2
+-rw-rw-rw-   0        0        0    74285 2023-12-11 22:01:00.000000 d3blocks-1.4.9/d3blocks/sankey/d3js/sankey.js
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.670494 d3blocks-1.4.9/d3blocks/scatter/
+-rw-rw-rw-   0        0        0    16216 2023-11-12 19:29:39.000000 d3blocks-1.4.9/d3blocks/scatter/Scatter.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/scatter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.670494 d3blocks-1.4.9/d3blocks/scatter/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/scatter/d3js/__init__.py
+-rw-rw-rw-   0        0        0   221958 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/scatter/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     7165 2023-11-12 19:39:58.000000 d3blocks-1.4.9/d3blocks/scatter/d3js/scatter.html.j2
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.670494 d3blocks-1.4.9/d3blocks/tests/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/tests/__init__.py
+-rw-rw-rw-   0        0        0    23380 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/tests/test_d3blocks.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.670494 d3blocks-1.4.9/d3blocks/timeseries/
+-rw-rw-rw-   0        0        0     9711 2023-11-12 19:41:59.000000 d3blocks-1.4.9/d3blocks/timeseries/Timeseries.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/timeseries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.686071 d3blocks-1.4.9/d3blocks/timeseries/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/timeseries/d3js/__init__.py
+-rw-rw-rw-   0        0        0   347498 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/timeseries/d3js/d3.v3.js
+-rw-rw-rw-   0        0        0    15492 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/timeseries/d3js/script.js
+-rw-rw-rw-   0        0        0      735 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/timeseries/d3js/style.css
+-rw-rw-rw-   0        0        0     1098 2023-11-12 19:42:53.000000 d3blocks-1.4.9/d3blocks/timeseries/d3js/timeseries.html.j2
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.686071 d3blocks-1.4.9/d3blocks/tree/
+-rw-rw-rw-   0        0        0     6525 2023-11-12 19:50:55.000000 d3blocks-1.4.9/d3blocks/tree/Tree.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.686071 d3blocks-1.4.9/d3blocks/tree/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/tree/d3js/__init__.py
+-rw-rw-rw-   0        0        0    28939 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/tree/d3js/d3.tree.js
+-rw-rw-rw-   0        0        0   231140 2023-11-12 19:52:16.000000 d3blocks-1.4.9/d3blocks/tree/d3js/tree.html.j2
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.686071 d3blocks-1.4.9/d3blocks/treemap/
+-rw-rw-rw-   0        0        0     6144 2023-12-10 14:26:24.000000 d3blocks-1.4.9/d3blocks/treemap/Treemap.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/treemap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.701696 d3blocks-1.4.9/d3blocks/treemap/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/treemap/d3js/__init__.py
+-rw-rw-rw-   0        0        0   221958 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/treemap/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     3370 2023-11-12 20:02:36.000000 d3blocks-1.4.9/d3blocks/treemap/d3js/treemap.html.j2
+-rw-rw-rw-   0        0        0    27740 2023-11-12 20:14:39.000000 d3blocks-1.4.9/d3blocks/utils.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.701696 d3blocks-1.4.9/d3blocks/violin/
+-rw-rw-rw-   0        0        0    11759 2023-11-12 20:06:03.000000 d3blocks-1.4.9/d3blocks/violin/Violin.py
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/violin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.701696 d3blocks-1.4.9/d3blocks/violin/d3js/
+-rw-rw-rw-   0        0        0        0 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/violin/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   221958 2023-09-23 10:16:01.000000 d3blocks-1.4.9/d3blocks/violin/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     6785 2023-11-12 20:12:54.000000 d3blocks-1.4.9/d3blocks/violin/d3js/violin.html.j2
+drwxrwxrwx   0        0        0        0 2023-12-11 22:34:10.403089 d3blocks-1.4.9/d3blocks.egg-info/
+-rw-rw-rw-   0        0        0     8612 2023-12-11 22:34:10.000000 d3blocks-1.4.9/d3blocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3289 2023-12-11 22:34:10.000000 d3blocks-1.4.9/d3blocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-11 22:34:10.000000 d3blocks-1.4.9/d3blocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-12-11 22:34:10.000000 d3blocks-1.4.9/d3blocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-12-11 22:34:10.000000 d3blocks-1.4.9/d3blocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-11 22:34:10.717382 d3blocks-1.4.9/setup.cfg
+-rw-rw-rw-   0        0        0     1757 2023-10-17 18:22:48.000000 d3blocks-1.4.9/setup.py
```

### Comparing `d3blocks-1.4.8/LICENSE` & `d3blocks-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/PKG-INFO` & `d3blocks-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: d3blocks
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python package d3blocks
 Home-page: https://github.com/d3blocks/d3blocks
-Download-URL: https://github.com/d3blocks/d3blocks/archive/1.4.8.tar.gz
+Download-URL: https://github.com/d3blocks/d3blocks/archive/1.4.9.tar.gz
 Author: Erdogan Taskesen, Oliver Verver
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: d3blocks Version: 1.4.8 Summary: Python package
+Metadata-Version: 2.1 Name: d3blocks Version: 1.4.9 Summary: Python package
 d3blocks Home-page: https://github.com/d3blocks/d3blocks Download-URL: https://
-github.com/d3blocks/d3blocks/archive/1.4.8.tar.gz Author: Erdogan Taskesen,
+github.com/d3blocks/d3blocks/archive/1.4.9.tar.gz Author: Erdogan Taskesen,
 Oliver Verver Author-email: erdogant@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved Classifier: Operating System
 :: OS Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE
            _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_3_b_l_o_c_k_s_/_d_3_b_l_o_c_k_s_/_b_l_o_b_/_m_a_i_n_/_l_o_g_o_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/d3blocks)](https://
 img.shields.io/pypi/pyversions/d3blocks) [![Pypi](https://img.shields.io/pypi/
```

### Comparing `d3blocks-1.4.8/README.md` & `d3blocks-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/__init__.py` & `d3blocks-1.4.9/d3blocks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     adjmat2vec,
     vec2adjmat,
     convert_flare2source_target,
     )
 
 __author__ = 'Erdogan Taskesen, Oliver Verver'
 __email__ = 'erdogant@gmail.com, mail@oliver3.nl'
-__version__ = '1.4.8'
+__version__ = '1.4.9'
 
 # module level doc-string
 __doc__ = """
 d3blocks
 =====================================================================
 
 d3blocks is for the creation of stand-alone and interactive d3 graphs.
```

### Comparing `d3blocks-1.4.8/d3blocks/chord/Chord.py` & `d3blocks-1.4.9/d3blocks/chord/Chord.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/chord/d3js/chord.html.j2` & `d3blocks-1.4.9/d3blocks/chord/d3js/chord.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/chord/d3js/chord.js` & `d3blocks-1.4.9/d3blocks/chord/d3js/chord.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/circlepacking/Circlepacking.py` & `d3blocks-1.4.9/d3blocks/circlepacking/Circlepacking.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/circlepacking/d3js/circlepacking.html.j2` & `d3blocks-1.4.9/d3blocks/circlepacking/d3js/circlepacking.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/circlepacking/d3js/d3.v6.min.js` & `d3blocks-1.4.9/d3blocks/circlepacking/d3js/d3.v6.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/circlepacking/d3js/lodash.min.js` & `d3blocks-1.4.9/d3blocks/circlepacking/d3js/lodash.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/d3blocks.py` & `d3blocks-1.4.9/d3blocks/d3blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -978,21 +978,25 @@
         Parameters
         ----------
         df : pd.DataFrame()
             Input data containing the following columns:
                 * 'source'
                 * 'target'
                 * 'weight'
+        color : dict or None.
+            Dictionary containing node with color information.
+                color={'Nuclear': '#FF0000', 'Wind':'#FF0000'}
         link : dict.
             Dictionary containing edge or link information.
                 * "linkColor" : "source", "target", "source-target"
                 * "linkStrokeOpacity" : 0.5
                 * "color_static": '#0f0f0f' or "grey", "blue", "red" etc
-        fontsize: int.
-            Fontsize of the text: default: 10
+        fontsize: int or dict.
+                * 10 : All nodes get this fontsize
+                * {'Nuclear': 10, 'Wind': 20}
         margin : dict.
             margin, in pixels.
                 * "top" : 5
                 * "right" : 1
                 * "bottom" : 5
                 * "left" : 1
         node : dict.
@@ -2821,14 +2825,16 @@
         Returns
         -------
         labels : dict()
             Dictionary containing class information.
 
         """
         # Make dict with properties
+        if self.config['chart']=='Sankey' and hasattr(self, 'config') and kwargs.get('fontsize', None) is None:
+            kwargs['fontsize'] = self.config['fontsize']
         if self.chart is not None:
             labels = self.chart.set_node_properties(*args, **kwargs)
         else:
             raise Exception(logger.error('You need to specify the chart during initialization. Hint: d3 = D3Blocks(chart="movingbubbles")'))
 
         # Convert to frame
         self.node_properties = utils.convert_dataframe_dict(labels, frame=self.config['frame'], logger=logger)
```

### Comparing `d3blocks-1.4.8/d3blocks/examples.py` & `d3blocks-1.4.9/d3blocks/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,101 @@
 # %%
 # import d3blocks
 # print(dir(d3blocks))
 # print(d3blocks.__version__)
 import pandas as pd
 import numpy as np
 
+# %%
+from d3blocks import D3Blocks
+d3 = D3Blocks()
+
+# Sankey
+sankey_table = d3.import_example(data='energy')
+# Sort the Sankey table by 'source'
+sankey_table.sort_values(by='source', inplace=True)
+
+# Create a D3Blocks Sankey chart
+d3 = D3Blocks(chart='Sankey', frame=True)
+d3.config['figsize'] = [1200, 800]
+d3.config['fontsize'] = 10
+
+# Node properties
+sankey_table['source'] = sankey_table['source'].astype(str)
+sankey_table['target'] = sankey_table['target'].astype(str)
+sankey_table['weight'] = sankey_table['weight'].astype(str)
+d3.set_node_properties(sankey_table)
+
+# Edge properties
+d3.set_edge_properties(sankey_table, color='target', opacity='target')
+d3.show()
+
+# %%
+
+# Initialize
+from d3blocks import D3Blocks
+# Sankey chart
+d3 = D3Blocks(chart='Sankey', frame=True)
+# Get example data
+df = d3.import_example(data='energy')
+# Create chart
+html = d3.sankey(df,
+                 fontsize=20,
+                 color={'Nuclear': '#FF0000',
+                        'Wind':'#FF0000',
+                        'Electricity grid':'#7FFFD4',
+                        'Bio-conversion':'#000000',
+                        'Industry': '#000000'},
+                 filepath=r'c:/temp/sankey.html'
+                 )
+
+
+# %%
+from d3blocks import D3Blocks
+d3 = D3Blocks()
+
+# Sankey
+df = d3.import_example(data='energy')
+html = d3.sankey(df, fontsize=20)
+
+d3.node_properties
+
+# %%
+
+
+
+# %% issue 45
+# https://github.com/d3blocks/d3blocks/issues/45
+# from d3blocks import D3Blocks
+# d3 = D3Blocks()
+# Treemap
+# df = d3.import_example(data='energy')
+# html = d3.treemap(df, filepath=r'c:\temp\treemap1.html')
+
+
+from d3blocks import D3Blocks
+# Initialize
+d3 = D3Blocks(chart='treemap', frame=False)
+# Import example
+df = d3.import_example('energy')
+
+# Set node properties
+d3.set_node_properties(df)
+
+# Set specific properties
+d3.node_properties['Bio-conversion']['tooltip'] = 'Title: P Operations<br><img src="https://source.unsplash.com/collection/385548/150x100">'
+# Set properties for Losses
+d3.node_properties.get('Losses')['tooltip'] = ''
+
+# Set edge properties
+d3.set_edge_properties(df)
+
+# Show chart
+d3.show(filepath=r'c:\temp\treemap.html')
+
 # %% issue 45
 # https://github.com/d3blocks/d3blocks/issues/45
 from d3blocks import D3Blocks
 d3 = D3Blocks()
 
 # Sankey
 df = d3.import_example(data='energy')
```

### Comparing `d3blocks-1.4.8/d3blocks/heatmap/Heatmap.py` & `d3blocks-1.4.9/d3blocks/heatmap/Heatmap.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js` & `d3blocks-1.4.9/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/heatmap/d3js/d3.v4.js` & `d3blocks-1.4.9/d3blocks/heatmap/d3js/d3.v4.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/heatmap/d3js/heatmap.html.j2` & `d3blocks-1.4.9/d3blocks/heatmap/d3js/heatmap.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/heatmap/d3js/matrix.html.j2` & `d3blocks-1.4.9/d3blocks/heatmap/d3js/matrix.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/imageslider/Imageslider.py` & `d3blocks-1.4.9/d3blocks/imageslider/Imageslider.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/imageslider/d3js/imageslider.html.j2` & `d3blocks-1.4.9/d3blocks/imageslider/d3js/imageslider.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/imageslider/d3js/jquery-2.1.1.js` & `d3blocks-1.4.9/d3blocks/imageslider/d3js/jquery-2.1.1.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/imageslider/d3js/main.js` & `d3blocks-1.4.9/d3blocks/imageslider/d3js/main.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/imageslider/d3js/modernizr.js` & `d3blocks-1.4.9/d3blocks/imageslider/d3js/modernizr.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/imageslider/d3js/reset.css` & `d3blocks-1.4.9/d3blocks/imageslider/d3js/reset.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/imageslider/d3js/style.css` & `d3blocks-1.4.9/d3blocks/imageslider/d3js/style.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/maps/Maps.py` & `d3blocks-1.4.9/d3blocks/maps/Maps.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/maps/d3js/d3.v6.min.js` & `d3blocks-1.4.9/d3blocks/maps/d3js/d3.v6.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/maps/d3js/maps.html.j2` & `d3blocks-1.4.9/d3blocks/maps/d3js/maps.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/maps/d3js/world.geojson` & `d3blocks-1.4.9/d3blocks/maps/d3js/world.geojson`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/matrix/Matrix.py` & `d3blocks-1.4.9/d3blocks/matrix/Matrix.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js` & `d3blocks-1.4.9/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/matrix/d3js/d3.v4.js` & `d3blocks-1.4.9/d3blocks/matrix/d3js/d3.v4.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/matrix/d3js/matrix.html.j2` & `d3blocks-1.4.9/d3blocks/matrix/d3js/matrix.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/movingbubbles/Movingbubbles.py` & `d3blocks-1.4.9/d3blocks/movingbubbles/Movingbubbles.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js` & `d3blocks-1.4.9/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/movingbubbles/d3js/movingbubbles.html.j2` & `d3blocks-1.4.9/d3blocks/movingbubbles/d3js/movingbubbles.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/movingbubbles/d3js/style.css` & `d3blocks-1.4.9/d3blocks/movingbubbles/d3js/style.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/particles/Particles.py` & `d3blocks-1.4.9/d3blocks/particles/Particles.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js` & `d3blocks-1.4.9/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/particles/d3js/d3.v4.min.js` & `d3blocks-1.4.9/d3blocks/particles/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/particles/d3js/particles.html.j2` & `d3blocks-1.4.9/d3blocks/particles/d3js/particles.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/sankey/Sankey.py` & `d3blocks-1.4.9/d3blocks/sankey/Sankey.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,21 +24,21 @@
     config['chart'] ='sankey'
     config['title'] = kwargs.get('title', 'Sankey - D3blocks')
     config['filepath'] = set_path(kwargs.get('filepath', 'sankey.html'), logger)
     config['figsize'] = kwargs.get('figsize', [800, 600])
     config['showfig'] = kwargs.get('showfig', True)
     config['overwrite'] = kwargs.get('overwrite', True)
     config['cmap'] = kwargs.get('cmap', 'Set1')
-    config['fontsize'] = kwargs.get('fontsize', 10)
     config['reset_properties'] = kwargs.get('reset_properties', True)
     config['link'] = {**{"color": "source-target", "stroke_opacity": 0.5, "color_static": '#d3d3d3'}, **link}
-    config['node'] = {**{"align": "justify", "width": 15, "padding": 15, "color": "currentColor", 'fontsize': config['fontsize']}, **node}
+    config['node'] = {**{"align": "justify", "width": 15, "padding": 15, "color": "currentColor"}, **node}
     config['margin'] = {**{"top": 5, "right": 1, "bottom": 5, "left": 1}, **margin}
     config['notebook'] = kwargs.get('notebook', False)
     config['save_button'] = kwargs.get('save_button', True)
+    config['fontsize'] = kwargs.get('fontsize', 10)
     # return
     return config
 
 
 # %% Get unique labels
 # def set_labels(labels, logger=None):
 #     """Set unique labels."""
@@ -116,22 +116,34 @@
     if color is not None:
         # Make same changes in the labels for the input nodes
         labels = dict(zip(dfO['source'].values.tolist() + dfO['target'].values.tolist(), df['source'].values.tolist() + df['target'].values.tolist()))
         keys = list(color.keys())
         for key in keys:
             color[labels.get(key)] = color.pop(key)
 
+    # Get fontsize
+    # fontsize = df.get('fontsize', None)
+    # if fontsize is None: fontsize = kwargs.get('fontsize', None)
+    # if (fontsize is not None) and (not isinstance(fontsize, int)):
+    #     # Make same changes in the labels for the input nodes
+    #     labels = dict(zip(dfO['source'].values.tolist() + dfO['target'].values.tolist(), df['source'].values.tolist() + df['target'].values.tolist()))
+    #     keys = list(fontsize.keys())
+    #     for key in keys:
+    #         fontsize[labels.get(key)] = fontsize.pop(key)
+    fontsize = kwargs.get('fontsize', 10)
+
+    # Store in final dict
     dict_labels = {}
     for i, label in enumerate(uilabels):
         getcolor = '#d3d3d3'
         # Change color if user-defined.
-        if color is not None:
-            getcolor = color.get(label, getcolor)
+        if color is not None: getcolor = color.get(label, getcolor)
+        # getfontsize = fontsize.get(label, getfontsize)
         # create dict labels
-        dict_labels[label] = {'id': i, 'label': label, 'color': getcolor, 'fontsize': kwargs['node']['fontsize']}
+        dict_labels[label] = {'id': i, 'label': label, 'color': getcolor, 'fontsize': fontsize}
     # Return
     return dict_labels
 
 
 def show(df, **kwargs):
     """Build and show the graph.
 
@@ -169,14 +181,17 @@
     # Set link_color selection correct on the form
     config['link_color_select'] = {'source': '', 'target': '', 'source-target': ''}
     config['link_color_select'][config['link']['color']] = 'selected="selected"'
     # Set align selection correct on the form
     config['align_select'] = {'left': '', 'right': '', 'justify': '', 'center': ''}
     config['align_select'][config['node']['align']] = 'selected="selected"'
 
+    # Update the fontsize
+    config['fontsize'] = kwargs['node_properties']['fontsize'][0]
+
     # Create the data from the input of javascript
     X = get_data_ready_for_d3(df, node_properties)
     # Check whether dataframe is circular
     if is_circular(df, logger):
         logger.warning("The dataframe seems to be circular which can not be handled by this chart!")
 
     # node_properties = convert_dataframe_dict(node_properties.copy(), frame=True)
@@ -227,15 +242,15 @@
         'marginRight': config['margin']['right'],
         'marginBottom': config['margin']['bottom'],
         'marginLeft': config['margin']['left'],
         'node_align': config['node']['align'],
         'node_width': config['node']['width'],
         'node_padding': config['node']['padding'],
         'node_stroke_color': config['node']['color'],
-        'fontsize': config['fontsize'],
+        'font_size': config['fontsize'],
 
         'SAVE_TO_SVG_SCRIPT': save_script,
         'SAVE_BUTTON_START': show_save_button[0],
         'SAVE_BUTTON_STOP': show_save_button[1],
         'SUPPORT': config['support'],
     }
```

### Comparing `d3blocks-1.4.8/d3blocks/sankey/d3js/sankey.html.j2` & `d3blocks-1.4.9/d3blocks/sankey/d3js/sankey.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/sankey/d3js/sankey.js` & `d3blocks-1.4.9/d3blocks/sankey/d3js/sankey.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2392,14 +2392,23 @@
             .data(nodes)
             .join("rect")
             .attr("x", d => d.x0)
             .attr("y", d => d.y0)
             .attr("height", d => d.y1 - d.y0)
             .attr("width", d => d.x1 - d.x0);
 
+        // CREATE DICT WITH THE LABEL AND FONTSIZE
+        /*
+        let font_size = {};
+        data.nodes.forEach(item => {
+          font_size[item.name] = item.fontsize;
+        });
+        */
+        // console.log(font_size)
+
         // SET THE NODE COLORS
         let node_color = {};
         data.nodes.forEach(item => {
             node_color[item.name] = item.color;
         });
         // console.log(node_color)
 
@@ -2471,21 +2480,28 @@
             .attr("stroke-width", ({
                 width
             }) => Math.max(1, width))
             .call(Lt ? path => path.append("title").text(({
                 index: i
             }) => Lt[i]) : () => {});
 
+        // console.log(font_size)
         if (Tl) svg.append("g")
             .attr("font-family", "sans-serif")
             .attr("font-size", {
                 {
-                    fontsize
+                    font_size
                 }
             })
+            //.attr("font-size", (d, i) => data.nodes[i].fontsize)
+            //.attr("font-size", (d, i) => {
+            //    console.log(data.nodes[i].fontsize);
+            //    return data.nodes[i].fontsize;
+            //})
+            // .attr("font-size", (d, i) => font_size[G[i]])
             .selectAll("text")
             .data(nodes)
             .join("text")
             .attr("x", d => d.x0 < width / 2 ? d.x1 + nodeLabelPadding : d.x0 - nodeLabelPadding)
             .attr("y", d => (d.y1 + d.y0) / 2)
             .attr("dy", "0.35em")
             .attr("text-anchor", d => d.x0 < width / 2 ? "start" : "end")
```

### Comparing `d3blocks-1.4.8/d3blocks/scatter/Scatter.py` & `d3blocks-1.4.9/d3blocks/scatter/Scatter.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/scatter/d3js/d3.v4.min.js` & `d3blocks-1.4.9/d3blocks/scatter/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/scatter/d3js/scatter.html.j2` & `d3blocks-1.4.9/d3blocks/scatter/d3js/scatter.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/tests/test_d3blocks.py` & `d3blocks-1.4.9/d3blocks/tests/test_d3blocks.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/timeseries/Timeseries.py` & `d3blocks-1.4.9/d3blocks/timeseries/Timeseries.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/timeseries/d3js/d3.v3.js` & `d3blocks-1.4.9/d3blocks/timeseries/d3js/d3.v3.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/timeseries/d3js/script.js` & `d3blocks-1.4.9/d3blocks/timeseries/d3js/script.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/timeseries/d3js/style.css` & `d3blocks-1.4.9/d3blocks/timeseries/d3js/style.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/timeseries/d3js/timeseries.html.j2` & `d3blocks-1.4.9/d3blocks/timeseries/d3js/timeseries.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/tree/Tree.py` & `d3blocks-1.4.9/d3blocks/tree/Tree.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/tree/d3js/d3.tree.js` & `d3blocks-1.4.9/d3blocks/tree/d3js/d3.tree.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/tree/d3js/tree.html.j2` & `d3blocks-1.4.9/d3blocks/tree/d3js/tree.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/treemap/Treemap.py` & `d3blocks-1.4.9/d3blocks/treemap/Treemap.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/treemap/d3js/d3.v4.min.js` & `d3blocks-1.4.9/d3blocks/treemap/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/treemap/d3js/treemap.html.j2` & `d3blocks-1.4.9/d3blocks/treemap/d3js/treemap.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/utils.py` & `d3blocks-1.4.9/d3blocks/utils.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/violin/Violin.py` & `d3blocks-1.4.9/d3blocks/violin/Violin.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js` & `d3blocks-1.4.9/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/violin/d3js/d3.v4.min.js` & `d3blocks-1.4.9/d3blocks/violin/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks/violin/d3js/violin.html.j2` & `d3blocks-1.4.9/d3blocks/violin/d3js/violin.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/d3blocks.egg-info/PKG-INFO` & `d3blocks-1.4.9/d3blocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: d3blocks
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python package d3blocks
 Home-page: https://github.com/d3blocks/d3blocks
-Download-URL: https://github.com/d3blocks/d3blocks/archive/1.4.8.tar.gz
+Download-URL: https://github.com/d3blocks/d3blocks/archive/1.4.9.tar.gz
 Author: Erdogan Taskesen, Oliver Verver
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: d3blocks Version: 1.4.8 Summary: Python package
+Metadata-Version: 2.1 Name: d3blocks Version: 1.4.9 Summary: Python package
 d3blocks Home-page: https://github.com/d3blocks/d3blocks Download-URL: https://
-github.com/d3blocks/d3blocks/archive/1.4.8.tar.gz Author: Erdogan Taskesen,
+github.com/d3blocks/d3blocks/archive/1.4.9.tar.gz Author: Erdogan Taskesen,
 Oliver Verver Author-email: erdogant@gmail.com Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved Classifier: Operating System
 :: OS Independent Requires-Python: >=3 Description-Content-Type: text/markdown
 License-File: LICENSE
            _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_d_3_b_l_o_c_k_s_/_d_3_b_l_o_c_k_s_/_b_l_o_b_/_m_a_i_n_/_l_o_g_o_._p_n_g_]
 [![Python](https://img.shields.io/pypi/pyversions/d3blocks)](https://
 img.shields.io/pypi/pyversions/d3blocks) [![Pypi](https://img.shields.io/pypi/
```

### Comparing `d3blocks-1.4.8/d3blocks.egg-info/SOURCES.txt` & `d3blocks-1.4.9/d3blocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `d3blocks-1.4.8/setup.py` & `d3blocks-1.4.9/setup.py`

 * *Files identical despite different names*

