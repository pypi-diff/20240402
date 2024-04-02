# Comparing `tmp/genice2-cif-2.1.1.tar.gz` & `tmp/genice2_cif-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genice2-cif-2.1.1.tar", last modified: Thu Sep 21 07:36:33 2023, max compression
+gzip compressed data, was "genice2_cif-2.2.tar", max compression
```

## Comparing `genice2-cif-2.1.1.tar` & `genice2_cif-2.2.tar`

### file list

```diff
@@ -1,18 +1,7 @@
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-09-21 07:36:33.470363 genice2-cif-2.1.1/
--rw-r--r--   0 matto      (505) staff       (20)     1733 2023-09-21 07:36:33.470216 genice2-cif-2.1.1/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)     1275 2023-09-21 07:36:33.000000 genice2-cif-2.1.1/README.md
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-09-21 07:36:33.468712 genice2-cif-2.1.1/genice2_cif/
--rw-r--r--   0 matto      (505) staff       (20)       67 2023-09-21 07:34:52.000000 genice2-cif-2.1.1/genice2_cif/__init__.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-09-21 07:36:33.470009 genice2-cif-2.1.1/genice2_cif/lattices/
--rw-r--r--   0 matto      (505) staff       (20)        0 2021-01-26 07:53:55.000000 genice2-cif-2.1.1/genice2_cif/lattices/__init__.py
--rw-r--r--   0 matto      (505) staff       (20)     4193 2022-02-26 10:58:28.000000 genice2-cif-2.1.1/genice2_cif/lattices/cif.py
--rw-r--r--   0 matto      (505) staff       (20)     4193 2022-02-26 10:58:28.000000 genice2-cif-2.1.1/genice2_cif/lattices/zeolite.py
-drwxr-xr-x   0 matto      (505) staff       (20)        0 2023-09-21 07:36:33.469529 genice2-cif-2.1.1/genice2_cif.egg-info/
--rw-r--r--   0 matto      (505) staff       (20)     1733 2023-09-21 07:36:33.000000 genice2-cif-2.1.1/genice2_cif.egg-info/PKG-INFO
--rw-r--r--   0 matto      (505) staff       (20)      347 2023-09-21 07:36:33.000000 genice2-cif-2.1.1/genice2_cif.egg-info/SOURCES.txt
--rw-r--r--   0 matto      (505) staff       (20)        1 2023-09-21 07:36:33.000000 genice2-cif-2.1.1/genice2_cif.egg-info/dependency_links.txt
--rw-r--r--   0 matto      (505) staff       (20)       88 2023-09-21 07:36:33.000000 genice2-cif-2.1.1/genice2_cif.egg-info/entry_points.txt
--rw-r--r--   0 matto      (505) staff       (20)       34 2023-09-21 07:36:33.000000 genice2-cif-2.1.1/genice2_cif.egg-info/requires.txt
--rw-r--r--   0 matto      (505) staff       (20)       12 2023-09-21 07:36:33.000000 genice2-cif-2.1.1/genice2_cif.egg-info/top_level.txt
--rw-r--r--   0 matto      (505) staff       (20)       38 2023-09-21 07:36:33.470408 genice2-cif-2.1.1/setup.cfg
--rw-r--r--   0 matto      (505) staff       (20)     1386 2023-09-21 07:31:58.000000 genice2-cif-2.1.1/setup.py
+-rw-r--r--   0        0        0     1333 2024-04-02 06:17:24.163266 genice2_cif-2.2/README.md
+-rw-r--r--   0        0        0       44 2024-04-02 04:25:31.822193 genice2_cif-2.2/genice2_cif/__init__.py
+-rw-r--r--   0        0        0        0 2021-01-26 07:53:55.000000 genice2_cif-2.2/genice2_cif/lattices/__init__.py
+-rw-r--r--   0        0        0     4200 2024-04-02 06:16:39.403452 genice2_cif-2.2/genice2_cif/lattices/cif.py
+-rw-r--r--   0        0        0     4200 2024-04-02 04:38:56.420736 genice2_cif-2.2/genice2_cif/lattices/zeolite.py
+-rw-r--r--   0        0        0     1040 2024-04-02 05:48:29.818234 genice2_cif-2.2/pyproject.toml
+-rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 genice2_cif-2.2/PKG-INFO
```

### Comparing `genice2-cif-2.1.1/README.md` & `genice2_cif-2.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,33 @@
-# [genice2-cif](https://github.com/vitroid/genice-cif/)
+![Logo](https://raw.githubusercontent.com/vitroid/GenIce/develop/logo/genice-v0.png)
 
-A loader plugin for [GenIce2](https://github.com/vitroid/GenIce) to read CIF file or to obtain structures in Zeolite DB.
+# [genice2-cif](https://github.com/vitroid/genice-cif)
 
-version 2.1.1
+A loader plugin for [GenIce2](https://github.com/vitroid/GenIce) to read CIF file or to obtain structures in [Zeolite DB](https://www.iza-structure.org/databases/).
 
-## Requirements
+version 2.2
 
+## Requirements
 
+* python^3.9
 * cif2ice>=0.3.0
-* GenIce2
-* validators
+* GenIce2^2.2.5.2
+* validators*
+
 
 ## Installation from PyPI
 
 ```shell
 % pip install genice2-cif
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
-Copy the files in genice2_cif/formats/ into your local formats/ folder.
-
 ## Usage
         
+    A loader plugin for GenIce2 to read CIF file or to obtain structures in Zeolite DB.
+
     * To convert a local cif file to Gromacs format,
 
         % genice2 cif[RHO.cif] > RHO.gro
         % genice2 cif[ice.cif:O=O] > RHO.gro   # Specify the tetrahedral atom type ()
 
       * Options:
 
@@ -42,12 +35,14 @@
         * O=M:      Regards the atom type M as the position of a water molecule.
                     (Default is "TS" (Tetrahedral hypothetical element "T" or "S"ilica, and "O" is ignored.))
 
     * Some zeolites share the network topology with low-density ices. If you want to retrieve a zeolite ITT structure from [IZA structure database](http://www.iza-structure.org/databases) to prepare a low-density ice, try the following command:
 
         % genice2 zeolite[ITT] > ITT.gro
 
+
+
 ## Test in place
 
 ```shell
 % make test
 ```
```

### Comparing `genice2-cif-2.1.1/genice2_cif/lattices/cif.py` & `genice2_cif-2.2/genice2_cif/lattices/cif.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,52 +14,54 @@
                 (Default is "TS" (Tetrahedral hypothetical element "T" or "S"ilica, and "O" is ignored.))
 
 * Some zeolites share the network topology with low-density ices. If you want to retrieve a zeolite ITT structure from [IZA structure database](http://www.iza-structure.org/databases) to prepare a low-density ice, try the following command:
 
     % genice2 zeolite[ITT] > ITT.gro
 """
 
-desc = { "ref": {"IZA structure database": "IZA database"},
-         "brief": "Read a CIF file.",
-         "usage": __doc__
-        }
+desc = {
+    "ref": {"IZA structure database": "IZA database"},
+    "brief": "Read a CIF file.",
+    "usage": __doc__,
+}
 
 if __name__[-16:] == "lattices.zeolite":
     desc["brief"] = "Retrieve a structure from the IZA Zeolite DB."
 
 
-#system modules
+# system modules
 import os
 import sys
 import itertools as it
 from logging import getLogger
 
-#external modules
+# external modules
 import numpy as np
-from requests import get #requests package
-import validators        #validators package
+from requests import get  # requests package
+import validators  # validators package
 from cif2ice import read_cif
 from genice2.cell import cellvectors
 import genice2.lattices
 
-def shortest_distance(atoms,cell):
+
+def shortest_distance(atoms, cell):
     Lmin = 1e99
-    for a1,a2 in it.combinations(atoms@cell,2):
-        d = a1-a2
-        L = d@d
+    for a1, a2 in it.combinations(atoms @ cell, 2):
+        d = a1 - a2
+        L = d @ d
         if L < Lmin:
             Lmin = L
     return Lmin**0.5
 
 
 def is_unique(L, pos):
     for x in L:
-        d = x-pos
+        d = x - pos
         d -= np.floor(d + 0.5)
-        if np.dot(d,d) < 0.0000001:
+        if np.dot(d, d) < 0.0000001:
             return False
     return True
 
 
 def download(url, file_name):
     # open in binary mode
     with open(file_name, "wb") as file:
@@ -69,23 +71,23 @@
         file.write(response.content)
 
 
 class Lattice(genice2.lattices.Lattice):
     def __init__(self, **kwargs):
         logger = getLogger()
         path = ""
-        atomtype = "TS"   # typical atom name in zeolite framework. (T or Si)
+        atomtype = "TS"  # typical atom name in zeolite framework. (T or Si)
         for k, v in kwargs.items():
-            if k == 'name':
+            if k == "name":
                 path = v
-            elif k == 'O':
+            elif k == "O":
                 atomtype = v
             elif v is True:
                 path = k
-        #input must be a file......too bad.
+        # input must be a file......too bad.
         if os.path.exists(path):
             fNameIn = path
         else:
             if validators.url(path):
                 URL = path
                 path = os.path.basename(path)
                 if path[-4:] in (".cif", ".CIF"):
@@ -114,16 +116,15 @@
         logger.debug("Atoms: {0}".format(atoms))
         self.cell = cellvectors(*cellshape) / 10  # in nm
         dmin = shortest_distance(atoms, self.cell)
         scale = 2.76 / dmin
         logger.debug("Shape: {0}".format(cellshape))
         logger.debug("Scale: {0}".format(scale))
         volume = np.linalg.det(self.cell)
-        icell  = np.linalg.inv(self.cell)
+        icell = np.linalg.inv(self.cell)
         self.waters = atoms
         self.coord = "relative"
         # bondlen = 3
-        self.density = len(atoms)*18.0/(volume*scale**3*1e-24*6.022e23)
-
+        self.density = len(atoms) * 18.0 / (volume * scale**3 * 1e-24 * 6.022e23)
 
 
 # Do nothing by default; it causes an error when arguments are missing.
```

### Comparing `genice2-cif-2.1.1/genice2_cif/lattices/zeolite.py` & `genice2_cif-2.2/genice2_cif/lattices/zeolite.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,52 +14,54 @@
                 (Default is "TS" (Tetrahedral hypothetical element "T" or "S"ilica, and "O" is ignored.))
 
 * Some zeolites share the network topology with low-density ices. If you want to retrieve a zeolite ITT structure from [IZA structure database](http://www.iza-structure.org/databases) to prepare a low-density ice, try the following command:
 
     % genice2 zeolite[ITT] > ITT.gro
 """
 
-desc = { "ref": {"IZA structure database": "IZA database"},
-         "brief": "Read a CIF file.",
-         "usage": __doc__
-        }
+desc = {
+    "ref": {"IZA structure database": "IZA database"},
+    "brief": "Read a CIF file.",
+    "usage": __doc__,
+}
 
 if __name__[-16:] == "lattices.zeolite":
     desc["brief"] = "Retrieve a structure from the IZA Zeolite DB."
 
 
-#system modules
+# system modules
 import os
 import sys
 import itertools as it
 from logging import getLogger
 
-#external modules
+# external modules
 import numpy as np
-from requests import get #requests package
-import validators        #validators package
+from requests import get  # requests package
+import validators  # validators package
 from cif2ice import read_cif
 from genice2.cell import cellvectors
 import genice2.lattices
 
-def shortest_distance(atoms,cell):
+
+def shortest_distance(atoms, cell):
     Lmin = 1e99
-    for a1,a2 in it.combinations(atoms@cell,2):
-        d = a1-a2
-        L = d@d
+    for a1, a2 in it.combinations(atoms @ cell, 2):
+        d = a1 - a2
+        L = d @ d
         if L < Lmin:
             Lmin = L
     return Lmin**0.5
 
 
 def is_unique(L, pos):
     for x in L:
-        d = x-pos
+        d = x - pos
         d -= np.floor(d + 0.5)
-        if np.dot(d,d) < 0.0000001:
+        if np.dot(d, d) < 0.0000001:
             return False
     return True
 
 
 def download(url, file_name):
     # open in binary mode
     with open(file_name, "wb") as file:
@@ -69,23 +71,23 @@
         file.write(response.content)
 
 
 class Lattice(genice2.lattices.Lattice):
     def __init__(self, **kwargs):
         logger = getLogger()
         path = ""
-        atomtype = "TS"   # typical atom name in zeolite framework. (T or Si)
+        atomtype = "TS"  # typical atom name in zeolite framework. (T or Si)
         for k, v in kwargs.items():
-            if k == 'name':
+            if k == "name":
                 path = v
-            elif k == 'O':
+            elif k == "O":
                 atomtype = v
             elif v is True:
                 path = k
-        #input must be a file......too bad.
+        # input must be a file......too bad.
         if os.path.exists(path):
             fNameIn = path
         else:
             if validators.url(path):
                 URL = path
                 path = os.path.basename(path)
                 if path[-4:] in (".cif", ".CIF"):
@@ -114,16 +116,15 @@
         logger.debug("Atoms: {0}".format(atoms))
         self.cell = cellvectors(*cellshape) / 10  # in nm
         dmin = shortest_distance(atoms, self.cell)
         scale = 2.76 / dmin
         logger.debug("Shape: {0}".format(cellshape))
         logger.debug("Scale: {0}".format(scale))
         volume = np.linalg.det(self.cell)
-        icell  = np.linalg.inv(self.cell)
+        icell = np.linalg.inv(self.cell)
         self.waters = atoms
         self.coord = "relative"
         # bondlen = 3
-        self.density = len(atoms)*18.0/(volume*scale**3*1e-24*6.022e23)
-
+        self.density = len(atoms) * 18.0 / (volume * scale**3 * 1e-24 * 6.022e23)
 
 
 # Do nothing by default; it causes an error when arguments are missing.
```

