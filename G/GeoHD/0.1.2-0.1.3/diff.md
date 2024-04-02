# Comparing `tmp/GeoHD-0.1.2.tar.gz` & `tmp/GeoHD-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoHD-0.1.2.tar", last modified: Tue Apr  2 14:02:58 2024, max compression
+gzip compressed data, was "GeoHD-0.1.3.tar", last modified: Tue Apr  2 14:40:32 2024, max compression
```

## Comparing `GeoHD-0.1.2.tar` & `GeoHD-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:02:58.577468 GeoHD-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-04-02 14:02:58.570469 GeoHD-0.1.2/GeoHD/
--rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.2/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      140 2024-04-01 18:26:55.000000 GeoHD-0.1.2/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.2/GeoHD/analyze.py
--rw-rw-rw-   0        0        0     4357 2024-04-01 18:15:13.000000 GeoHD-0.1.2/GeoHD/process.py
--rw-rw-rw-   0        0        0     2058 2024-04-02 08:36:24.000000 GeoHD-0.1.2/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-02 08:36:03.000000 GeoHD-0.1.2/GeoHD/visualize.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:02:58.575467 GeoHD-0.1.2/GeoHD.egg-info/
--rw-rw-rw-   0        0        0      386 2024-04-02 14:02:58.000000 GeoHD-0.1.2/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-04-02 14:02:58.000000 GeoHD-0.1.2/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:02:58.000000 GeoHD-0.1.2/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-02 14:02:58.000000 GeoHD-0.1.2/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 14:02:58.000000 GeoHD-0.1.2/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      386 2024-04-02 14:02:58.577468 GeoHD-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3509 2024-04-02 08:59:41.000000 GeoHD-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 14:02:58.578469 GeoHD-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      469 2024-04-02 14:02:41.000000 GeoHD-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:02:58.574468 GeoHD-0.1.2/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:40:32.671933 GeoHD-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-04-02 14:40:32.662931 GeoHD-0.1.3/GeoHD/
+-rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.3/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      140 2024-04-01 18:26:55.000000 GeoHD-0.1.3/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.3/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     4355 2024-04-02 14:23:48.000000 GeoHD-0.1.3/GeoHD/process.py
+-rw-rw-rw-   0        0        0     2058 2024-04-02 08:36:24.000000 GeoHD-0.1.3/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-02 08:36:03.000000 GeoHD-0.1.3/GeoHD/visualize.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:40:32.669930 GeoHD-0.1.3/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0      386 2024-04-02 14:40:32.000000 GeoHD-0.1.3/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-04-02 14:40:32.000000 GeoHD-0.1.3/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 14:40:32.000000 GeoHD-0.1.3/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-02 14:40:32.000000 GeoHD-0.1.3/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 14:40:32.000000 GeoHD-0.1.3/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      386 2024-04-02 14:40:32.670955 GeoHD-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3509 2024-04-02 08:59:41.000000 GeoHD-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:40:32.671933 GeoHD-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      469 2024-04-02 14:37:30.000000 GeoHD-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:40:32.668930 GeoHD-0.1.3/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.3/test/__init__.py
```

### Comparing `GeoHD-0.1.2/GeoHD/AKDE.py` & `GeoHD-0.1.3/GeoHD/AKDE.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.2/GeoHD/analyze.py` & `GeoHD-0.1.3/GeoHD/analyze.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.2/GeoHD/process.py` & `GeoHD-0.1.3/GeoHD/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     Parameters:
         smoothed_density (numpy.ndarray): Smoothed density raster array.
         xmin (float): Minimum x-coordinate of the bounding box.
         ymin (float): Minimum y-coordinate of the bounding box.
         xmax (float): Maximum x-coordinate of the bounding box.
         ymax (float): Maximum y-coordinate of the bounding box.
     """
-    plt.figure(figsize=(10, 10))
+    plt.figure(figsize=(8, 8))
     plt.imshow(smoothed_density, extent=[xmin, xmax, ymin, ymax], origin='lower', cmap='Purples')
     plt.colorbar(label='Density')
     plt.xlabel('Longitude')
     plt.ylabel('Latitude')
     plt.title('Kernel Density Estimation')
     plt.show()
```

### Comparing `GeoHD-0.1.2/GeoHD/utils.py` & `GeoHD-0.1.3/GeoHD/utils.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.2/GeoHD/visualize.py` & `GeoHD-0.1.3/GeoHD/visualize.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.2/LICENSE` & `GeoHD-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.2/README.md` & `GeoHD-0.1.3/README.md`

 * *Files identical despite different names*

