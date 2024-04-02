# Comparing `tmp/genice2-cage-2.2.tar.gz` & `tmp/genice2_cage-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genice2-cage-2.2.tar", last modified: Fri Sep 22 03:40:24 2023, max compression
+gzip compressed data, was "genice2_cage-2.3.tar", max compression
```

## Comparing `genice2-cage-2.2.tar` & `genice2_cage-2.3.tar`

### file list

```diff
@@ -1,17 +1,6 @@
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-09-22 03:40:24.654880 genice2-cage-2.2/
--rw-r--r--   0 matto      (505) staff       (20)     3091 2023-09-22 03:40:24.654946 genice2-cage-2.2/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)     2628 2023-09-22 03:40:24.000000 genice2-cage-2.2/README.md
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-09-22 03:40:24.653808 genice2-cage-2.2/genice2_cage/
--rw-r--r--   0 matto      (505) staff       (20)       59 2023-09-22 03:40:17.000000 genice2-cage-2.2/genice2_cage/__init__.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-09-22 03:40:24.654755 genice2-cage-2.2/genice2_cage/formats/
--rw-r--r--   0 matto      (505) staff       (20)        0 2021-01-26 07:57:38.000000 genice2-cage-2.2/genice2_cage/formats/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)    15255 2023-09-22 03:31:07.000000 genice2-cage-2.2/genice2_cage/formats/cage.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-09-22 03:40:24.654541 genice2-cage-2.2/genice2_cage.egg-info/
--rw-r--r--   0 matto      (505) staff       (20)     3091 2023-09-22 03:40:24.000000 genice2-cage-2.2/genice2_cage.egg-info/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)      333 2023-09-22 03:40:24.000000 genice2-cage-2.2/genice2_cage.egg-info/SOURCES.txt
--rw-r--r--   0 matto      (505) staff       (20)        1 2023-09-22 03:40:24.000000 genice2-cage-2.2/genice2_cage.egg-info/dependency_links.txt
--rw-r--r--   0 matto      (505) staff       (20)       50 2023-09-22 03:40:24.000000 genice2-cage-2.2/genice2_cage.egg-info/entry_points.txt
--rw-r--r--   0 matto      (505) staff       (20)       64 2023-09-22 03:40:24.000000 genice2-cage-2.2/genice2_cage.egg-info/requires.txt
--rw-r--r--   0 matto      (505) staff       (20)       13 2023-09-22 03:40:24.000000 genice2-cage-2.2/genice2_cage.egg-info/top_level.txt
--rw-r--r--   0 matto      (505) staff       (20)      108 2023-09-22 03:40:24.655153 genice2-cage-2.2/setup.cfg
--rwxr--r--   0 matto      (505) staff       (20)     1510 2021-03-19 15:16:15.000000 genice2-cage-2.2/setup.py
+-rw-r--r--   0        0        0     2621 2024-04-02 05:49:04.579322 genice2_cage-2.3/README.md
+-rw-r--r--   0        0        0       59 2024-04-02 06:01:42.155600 genice2_cage-2.3/genice2_cage/__init__.py
+-rw-r--r--   0        0        0        0 2021-01-26 07:57:38.000000 genice2_cage-2.3/genice2_cage/formats/__init__.py
+-rw-r--r--   0        0        0    15255 2023-09-22 03:31:07.599550 genice2_cage-2.3/genice2_cage/formats/cage.py
+-rw-r--r--   0        0        0     1077 2024-04-02 05:48:43.371344 genice2_cage-2.3/pyproject.toml
+-rw-r--r--   0        0        0     3410 1970-01-01 00:00:00.000000 genice2_cage-2.3/PKG-INFO
```

### Comparing `genice2-cage-2.2/PKG-INFO` & `genice2_cage-2.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 Metadata-Version: 2.1
 Name: genice2-cage
-Version: 2.2
-Summary: Cage detection plugin for GenIce.
-Home-page: https://github.com/vitroid/genice-cage/
-Author: Masakazu Matsumoto
-Author-email: vitroid@gmail.com
+Version: 2.3
+Summary: A format plugin for GenIce2 to detect cages.
 License: MIT
-Keywords: genice,cage
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
+Author: vitroid
+Author-email: vitroid@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: GenIce2 (>=2.2.5.2,<3.0.0.0)
+Requires-Dist: cycless (>=0.4.2,<0.5.0)
+Requires-Dist: graphstat (>=0.2.1,<0.3.0)
+Requires-Dist: networkx (>=3.2.1,<4.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: yaplotlib (>=0.1.2,<0.2.0)
 Description-Content-Type: text/markdown
 
-# [genice2-cage](https://github.com/vitroid/genice-cage/)
+![Logo](https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png)
 
-A [GenIce2](https://github.com/vitroid/GenIce) format plugin to detect cage-like topologies.
+# [genice2-cage](https://github.com/vitroid/genice-cage)
+
+A format plugin for [GenIce2](https://github.com/vitroid/GenIce) to detect cages.
 
 version 2.2
 
 ## Requirements
 
+* python^3.9
+* GenIce2^2.2.5.2
+* graphstat^0.2.1
+* cycless^0.4.2
+* yaplotlib^0.1.2
+* numpy^1.26.4
+* networkx^3.2.1
 
-* cycless
-* attrdict
-* networkx
-* numpy
-* yaplotlib>=0.1.2
-* genice2>=2.1b0
 
 ## Installation from PyPI
 
 ```shell
 % pip install genice2-cage
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
-Copy the files in genice2_cage/formats/ into your local formats/ folder.
-
 ## Usage
         
+    A GenIce2 format plugin to detect cage-like topologies.
+
     Usage:
         % genice2 CS1 -r 2 2 2 -f cage[12,14-16:ring=-6]
         % genice2 CRN1 -f cage[sizes=3-10:json]
         % genice2 CRN1 -f cage[sizes=3-10:yaplot]
         % genice2 CS2 -w tip4p -f cage[gromacs:sizes=-16:ring=5,6]
         % analice2 traj.gro -O OW -H HW[12] -w tip4p -f cage[quad]
         % analice2 traj.gro -O OW -H HW[12] -w tip4p -f cage[quad:json]
@@ -67,16 +67,19 @@
         json2      Output values in [JSON](https://www.json.org/) format (Assess cage locations based on HB network topology by labeling them).
         yaplot     Visualize cages with [Yaplot](https://github.com/vitroid/Yaplot/). Cages are drawn in different layers according to the number of faces, and faces are colored according to the number of vertices.
         gromacs    Output individual cages in Gromacs format. (EXPERIMENTAL)
         quad       Quadcage order parameter to identify the Frank-Kasper-type crystal structures.[JMM2011] Cages sizes and maximum ring size are set appropriately automatically.
         python     Output cage types in python format convenient for GenIce lattice modules.
     * [JMM2011] Jacobson, L. C., Matsumoto, M. & Molinero, V. Order parameters for the multistep crystallization of clathrate hydrates. J. Chem. Phys. 135, 074501 (2011).[doi:10.1063/1.3613667](https://doi.org/10.1063/1.3613667)
 
+
+
 ## Test in place
 
 ```shell
 % make test
 ```
 
 ## Algorithms
 
 * M. Matsumoto, A. Baba, and I. Ohmine, Topological building blocks of hydrogen bond network in water, J. Chem. Phys. 127, 134504 (2007); [doi:10.1063/1.2772627](http://dx.doi.org/doi:10.1063/1.2772627)
+
```

### Comparing `genice2-cage-2.2/README.md` & `genice2_cage-2.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,36 @@
-# [genice2-cage](https://github.com/vitroid/genice-cage/)
+![Logo](https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png)
 
-A [GenIce2](https://github.com/vitroid/GenIce) format plugin to detect cage-like topologies.
+# [genice2-cage](https://github.com/vitroid/genice-cage)
+
+A format plugin for [GenIce2](https://github.com/vitroid/GenIce) to detect cages.
 
 version 2.2
 
 ## Requirements
 
+* python^3.9
+* GenIce2^2.2.5.2
+* graphstat^0.2.1
+* cycless^0.4.2
+* yaplotlib^0.1.2
+* numpy^1.26.4
+* networkx^3.2.1
 
-* cycless
-* attrdict
-* networkx
-* numpy
-* yaplotlib>=0.1.2
-* genice2>=2.1b0
 
 ## Installation from PyPI
 
 ```shell
 % pip install genice2-cage
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
-Copy the files in genice2_cage/formats/ into your local formats/ folder.
-
 ## Usage
         
+    A GenIce2 format plugin to detect cage-like topologies.
+
     Usage:
         % genice2 CS1 -r 2 2 2 -f cage[12,14-16:ring=-6]
         % genice2 CRN1 -f cage[sizes=3-10:json]
         % genice2 CRN1 -f cage[sizes=3-10:yaplot]
         % genice2 CS2 -w tip4p -f cage[gromacs:sizes=-16:ring=5,6]
         % analice2 traj.gro -O OW -H HW[12] -w tip4p -f cage[quad]
         % analice2 traj.gro -O OW -H HW[12] -w tip4p -f cage[quad:json]
@@ -52,14 +45,16 @@
         json2      Output values in [JSON](https://www.json.org/) format (Assess cage locations based on HB network topology by labeling them).
         yaplot     Visualize cages with [Yaplot](https://github.com/vitroid/Yaplot/). Cages are drawn in different layers according to the number of faces, and faces are colored according to the number of vertices.
         gromacs    Output individual cages in Gromacs format. (EXPERIMENTAL)
         quad       Quadcage order parameter to identify the Frank-Kasper-type crystal structures.[JMM2011] Cages sizes and maximum ring size are set appropriately automatically.
         python     Output cage types in python format convenient for GenIce lattice modules.
     * [JMM2011] Jacobson, L. C., Matsumoto, M. & Molinero, V. Order parameters for the multistep crystallization of clathrate hydrates. J. Chem. Phys. 135, 074501 (2011).[doi:10.1063/1.3613667](https://doi.org/10.1063/1.3613667)
 
+
+
 ## Test in place
 
 ```shell
 % make test
 ```
 
 ## Algorithms
```

### Comparing `genice2-cage-2.2/genice2_cage/formats/cage.py` & `genice2_cage-2.3/genice2_cage/formats/cage.py`

 * *Files identical despite different names*

