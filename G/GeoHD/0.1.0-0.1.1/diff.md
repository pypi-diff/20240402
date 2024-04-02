# Comparing `tmp/GeoHD-0.1.0.tar.gz` & `tmp/GeoHD-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoHD-0.1.0.tar", last modified: Tue Apr  2 13:53:48 2024, max compression
+gzip compressed data, was "GeoHD-0.1.1.tar", last modified: Tue Apr  2 13:59:44 2024, max compression
```

## Comparing `GeoHD-0.1.0.tar` & `GeoHD-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 13:53:48.673406 GeoHD-0.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-02 13:53:48.665406 GeoHD-0.1.0/GeoHD/
--rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.0/GeoHD/AKDE.py
--rw-rw-rw-   0        0        0      140 2024-04-01 18:26:55.000000 GeoHD-0.1.0/GeoHD/__init__.py
--rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.0/GeoHD/analyze.py
--rw-rw-rw-   0        0        0     4357 2024-04-01 18:15:13.000000 GeoHD-0.1.0/GeoHD/process.py
--rw-rw-rw-   0        0        0     2058 2024-04-02 08:36:24.000000 GeoHD-0.1.0/GeoHD/utils.py
--rw-rw-rw-   0        0        0     2912 2024-04-02 08:36:03.000000 GeoHD-0.1.0/GeoHD/visualize.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:53:48.671406 GeoHD-0.1.0/GeoHD.egg-info/
--rw-rw-rw-   0        0        0      390 2024-04-02 13:53:48.000000 GeoHD-0.1.0/GeoHD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-04-02 13:53:48.000000 GeoHD-0.1.0/GeoHD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 13:53:48.000000 GeoHD-0.1.0/GeoHD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-04-02 13:53:48.000000 GeoHD-0.1.0/GeoHD.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-02 13:53:48.000000 GeoHD-0.1.0/GeoHD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      390 2024-04-02 13:53:48.672408 GeoHD-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3509 2024-04-02 08:59:41.000000 GeoHD-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-02 13:53:48.673406 GeoHD-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      485 2024-04-02 09:23:25.000000 GeoHD-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:53:48.669407 GeoHD-0.1.0/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.0/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:59:44.103311 GeoHD-0.1.1/
+drwxrwxrwx   0        0        0        0 2024-04-02 13:59:44.096311 GeoHD-0.1.1/GeoHD/
+-rw-rw-rw-   0        0        0     8637 2024-04-01 18:15:13.000000 GeoHD-0.1.1/GeoHD/AKDE.py
+-rw-rw-rw-   0        0        0      140 2024-04-01 18:26:55.000000 GeoHD-0.1.1/GeoHD/__init__.py
+-rw-rw-rw-   0        0        0     4915 2024-04-01 16:22:54.000000 GeoHD-0.1.1/GeoHD/analyze.py
+-rw-rw-rw-   0        0        0     4357 2024-04-01 18:15:13.000000 GeoHD-0.1.1/GeoHD/process.py
+-rw-rw-rw-   0        0        0     2058 2024-04-02 08:36:24.000000 GeoHD-0.1.1/GeoHD/utils.py
+-rw-rw-rw-   0        0        0     2912 2024-04-02 08:36:03.000000 GeoHD-0.1.1/GeoHD/visualize.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:59:44.102311 GeoHD-0.1.1/GeoHD.egg-info/
+-rw-rw-rw-   0        0        0      407 2024-04-02 13:59:44.000000 GeoHD-0.1.1/GeoHD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-04-02 13:59:44.000000 GeoHD-0.1.1/GeoHD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 13:59:44.000000 GeoHD-0.1.1/GeoHD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-02 13:59:44.000000 GeoHD-0.1.1/GeoHD.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-02 13:59:44.000000 GeoHD-0.1.1/GeoHD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35182 2024-04-01 18:46:45.000000 GeoHD-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      407 2024-04-02 13:59:44.102311 GeoHD-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3509 2024-04-02 08:59:41.000000 GeoHD-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-02 13:59:44.103311 GeoHD-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      486 2024-04-02 13:58:54.000000 GeoHD-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 13:59:44.101311 GeoHD-0.1.1/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 18:50:35.000000 GeoHD-0.1.1/test/__init__.py
```

### Comparing `GeoHD-0.1.0/GeoHD/AKDE.py` & `GeoHD-0.1.1/GeoHD/AKDE.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.0/GeoHD/analyze.py` & `GeoHD-0.1.1/GeoHD/analyze.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.0/GeoHD/process.py` & `GeoHD-0.1.1/GeoHD/process.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.0/GeoHD/utils.py` & `GeoHD-0.1.1/GeoHD/utils.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.0/GeoHD/visualize.py` & `GeoHD-0.1.1/GeoHD/visualize.py`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.0/LICENSE` & `GeoHD-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoHD-0.1.0/README.md` & `GeoHD-0.1.1/README.md`

 * *Files identical despite different names*

