# Comparing `tmp/genice2-mdanalysis-0.6.5.tar.gz` & `tmp/genice2_mdanalysis-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genice2-mdanalysis-0.6.5.tar", last modified: Wed May 12 03:43:12 2021, max compression
+gzip compressed data, was "genice2_mdanalysis-0.7.tar", max compression
```

## Comparing `genice2-mdanalysis-0.6.5.tar` & `genice2_mdanalysis-0.7.tar`

### file list

```diff
@@ -1,17 +1,6 @@
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-12 03:43:12.096844 genice2-mdanalysis-0.6.5/
--rw-r--r--   0 matto      (505) staff       (20)     2453 2021-05-12 03:43:12.096927 genice2-mdanalysis-0.6.5/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)     1436 2021-05-12 03:43:11.000000 genice2-mdanalysis-0.6.5/README.md
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-12 03:43:12.095539 genice2-mdanalysis-0.6.5/genice2_mdanalysis/
--rw-r--r--   0 matto      (505) staff       (20)       93 2021-05-12 03:41:45.000000 genice2-mdanalysis-0.6.5/genice2_mdanalysis/__init__.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-12 03:43:12.096708 genice2-mdanalysis-0.6.5/genice2_mdanalysis/formats/
--rw-r--r--   0 matto      (505) staff       (20)        1 2021-03-20 16:18:45.000000 genice2-mdanalysis-0.6.5/genice2_mdanalysis/formats/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)     3253 2021-05-12 03:43:05.000000 genice2-mdanalysis-0.6.5/genice2_mdanalysis/formats/mdanalysis.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2021-05-12 03:43:12.096327 genice2-mdanalysis-0.6.5/genice2_mdanalysis.egg-info/
--rw-r--r--   0 matto      (505) staff       (20)     2453 2021-05-12 03:43:11.000000 genice2-mdanalysis-0.6.5/genice2_mdanalysis.egg-info/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)      393 2021-05-12 03:43:11.000000 genice2-mdanalysis-0.6.5/genice2_mdanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 matto      (505) staff       (20)        1 2021-05-12 03:43:11.000000 genice2-mdanalysis-0.6.5/genice2_mdanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 matto      (505) staff       (20)       69 2021-05-12 03:43:11.000000 genice2-mdanalysis-0.6.5/genice2_mdanalysis.egg-info/entry_points.txt
--rw-r--r--   0 matto      (505) staff       (20)       26 2021-05-12 03:43:11.000000 genice2-mdanalysis-0.6.5/genice2_mdanalysis.egg-info/requires.txt
--rw-r--r--   0 matto      (505) staff       (20)       19 2021-05-12 03:43:11.000000 genice2-mdanalysis-0.6.5/genice2_mdanalysis.egg-info/top_level.txt
--rw-r--r--   0 matto      (505) staff       (20)      108 2021-05-12 03:43:12.097185 genice2-mdanalysis-0.6.5/setup.cfg
--rw-r--r--   0 matto      (505) staff       (20)     1479 2021-03-24 07:38:09.000000 genice2-mdanalysis-0.6.5/setup.py
+-rw-r--r--   0        0        0     1190 2024-04-02 05:54:14.656006 genice2_mdanalysis-0.7/README.md
+-rw-r--r--   0        0        0       73 2024-04-02 04:55:46.312405 genice2_mdanalysis-0.7/genice2_mdanalysis/__init__.py
+-rw-r--r--   0        0        0        1 2021-03-20 16:18:45.928872 genice2_mdanalysis-0.7/genice2_mdanalysis/formats/__init__.py
+-rw-r--r--   0        0        0     3253 2021-05-12 03:43:05.376265 genice2_mdanalysis-0.7/genice2_mdanalysis/formats/mdanalysis.py
+-rw-r--r--   0        0        0     1074 2024-04-02 05:50:01.137612 genice2_mdanalysis-0.7/pyproject.toml
+-rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 genice2_mdanalysis-0.7/PKG-INFO
```

### Comparing `genice2-mdanalysis-0.6.5/README.md` & `genice2_mdanalysis-0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,46 @@
-# [genice2-mdanalysis](https://github.com/vitroid/genice-mdanalysis/)
+![Logo](https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png)
 
-A [GenIce2](https://github.com/vitroid/GenIce) format plugin to make a Universe of MDAnalysis.
+# [genice2-mdanalysis](https://github.com/vitroid/genice-mdanalysis)
 
-version 0.6.5
-
-## Requirements
+A format plugin for [GenIce2](https://github.com/vitroid/GenIce) to make a Universe of MDAnalysis.
 
+version 0.7
 
-* GenIce2>=2.1b2
-* MDAnalysis
-
-### For Apple M1
+## Requirements
 
-The newest MDAnalysis is required but is not available at PyPI. Follow the instructions below to install it.
+* python^3.9
+* GenIce2^2.2.5.2
+* MDAnalysis*
 
-```shell
-% git clone https://github.com/MDAnalysis/MDAnalysis.git
-% cd MDAnalysis/package; ./setup.py install
-```
 
 ## Installation from PyPI
 
 ```shell
 % pip install genice2-mdanalysis
 ```
 
-## Manual Installation
-
-### System-wide installation
-
-```shell
-% make install
-```
-
-### Private installation
-
-Copy the files in genice2_mdanalysis/formats/ into your local formats/ folder.
-
 ## Usage
         
+    Write the ice structure in various file formats with the help of MDAnalysis.
+
     Usage:
         % genice 1c -f mdanalysis > 1c.pickle
         % genice 1c -f mdanalysis[1c.gro]
         % genice 1c -f mdanalysis[1c.xtc]
 
     Options:
         filename  The file name to be written. The file type is specified by the
                   suffix. All the supported file types are listed in the
                   [MDAnalysis web page](https://docs.mdanalysis.org/stable/documentation_pages/coordinates/init.html#supported-coordinate-formats).
                   If the file name is not specified, the Universe instance of
                   MDAnalysis is written to the stdout in the python pickle
                   format.
 
 
+
+
 ## Test in place
 
 ```shell
 % make test
 ```
```

### Comparing `genice2-mdanalysis-0.6.5/genice2_mdanalysis/formats/mdanalysis.py` & `genice2_mdanalysis-0.7/genice2_mdanalysis/formats/mdanalysis.py`

 * *Files identical despite different names*

