# Comparing `tmp/libhreels-2.1.1.tar.gz` & `tmp/libhreels-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libhreels-2.1.1.tar", max compression
+gzip compressed data, was "libhreels-2.2.0.tar", max compression
```

## Comparing `libhreels-2.1.1.tar` & `libhreels-2.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     3653 2024-02-27 17:13:53.136568 libhreels-2.1.1/README.md
--rw-r--r--   0        0        0     6877 2024-02-04 16:42:22.538727 libhreels-2.1.1/libhreels/Auger.py
--rw-r--r--   0        0        0    21814 2024-02-04 16:42:22.538727 libhreels-2.1.1/libhreels/HREELS.py
--rw-r--r--   0        0        0     2721 2024-02-04 16:42:22.538727 libhreels-2.1.1/libhreels/LEED.py
--rw-r--r--   0        0        0       21 2024-02-04 16:42:22.538727 libhreels-2.1.1/libhreels/NoExpLogbook.py
--rwxr-xr-x   0        0        0     2927 2024-02-01 17:06:29.565198 libhreels-2.1.1/libhreels/README.md
--rw-r--r--   0        0        0    17300 2024-02-07 10:00:06.512762 libhreels-2.1.1/libhreels/ViewAuger.py
--rw-r--r--   0        0        0    22984 2024-02-07 09:58:29.316442 libhreels-2.1.1/libhreels/ViewHREELS.py
--rw-r--r--   0        0        0      172 2024-02-04 16:42:22.538727 libhreels-2.1.1/libhreels/__init__.py
--rw-r--r--   0        0        0    29603 2024-03-09 11:57:29.484600 libhreels-2.1.1/libhreels/calcHREELS20.png
--rwxr-xr-x   0        0        0    11889 2024-03-09 11:57:27.212605 libhreels-2.1.1/libhreels/calcHREELS20.py
--rwxr-xr-x   0        0        0     9311 2024-03-05 14:20:28.337206 libhreels-2.1.1/libhreels/dielectrics20.py
--rw-r--r--   0        0        0     1493 2024-02-04 16:42:22.538727 libhreels-2.1.1/libhreels/expLogbook.py
--rwxr-xr-x   0        0        0     7845 2024-03-05 13:23:52.958974 libhreels-2.1.1/libhreels/materials20.json
--rw-r--r--   0        0        0     1848 2024-03-08 18:07:59.243138 libhreels-2.1.1/libhreels/mod_doeels.mod
--rw-r--r--   0        0        0   210696 2024-02-04 16:42:22.538727 libhreels-2.1.1/libhreels/myBoson.cpython-36m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0   257256 2024-02-04 16:42:22.550727 libhreels-2.1.1/libhreels/myBoson.cpython-38-x86_64-linux-gnu.so
--rw-r--r--   0        0        0    26782 2024-02-04 16:42:22.550727 libhreels-2.1.1/libhreels/myBoson.f90
--rw-r--r--   0        0        0    20031 2024-02-04 16:42:22.550727 libhreels-2.1.1/libhreels/myBoson.o
--rwxr-xr-x   0        0        0   399688 2024-03-09 11:58:53.976411 libhreels-2.1.1/libhreels/myEels20.cpython-38-x86_64-linux-gnu.so
--rwxr-xr-x   0        0        0    32043 2024-03-09 11:47:04.045683 libhreels-2.1.1/libhreels/myEels20.f90
--rw-r--r--   0        0        0     8583 2024-02-04 16:42:22.566727 libhreels-2.1.1/libhreels/viewauger.ui
--rw-r--r--   0        0        0    10420 2024-02-04 16:42:22.566727 libhreels-2.1.1/libhreels/viewhreels.ui
--rw-r--r--   0        0        0      963 2024-02-04 16:42:22.566727 libhreels-2.1.1/libhreels/viewhreels_dialog.ui
--rw-r--r--   0        0        0     1129 2024-03-09 11:12:00.560523 libhreels-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 libhreels-2.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     3653 2024-04-02 10:52:57.484341 libhreels-2.2.0/README.md
+-rwxr-xr-x   0        0        0     6877 2024-04-02 10:52:57.862904 libhreels-2.2.0/libhreels/Auger.py
+-rwxr-xr-x   0        0        0    21814 2024-04-02 10:52:57.868992 libhreels-2.2.0/libhreels/HREELS.py
+-rwxr-xr-x   0        0        0     2721 2024-04-02 10:52:57.871902 libhreels-2.2.0/libhreels/LEED.py
+-rwxr-xr-x   0        0        0       21 2024-04-02 10:52:57.874575 libhreels-2.2.0/libhreels/NoExpLogbook.py
+-rwxr-xr-x   0        0        0     2927 2024-04-02 10:52:57.877199 libhreels-2.2.0/libhreels/README.md
+-rwxr-xr-x   0        0        0    17300 2024-04-02 10:52:57.880920 libhreels-2.2.0/libhreels/ViewAuger.py
+-rwxr-xr-x   0        0        0    22984 2024-04-02 10:52:57.886045 libhreels-2.2.0/libhreels/ViewHREELS.py
+-rwxr-xr-x   0        0        0      172 2024-04-02 10:52:57.888541 libhreels-2.2.0/libhreels/__init__.py
+-rwxr-xr-x   0        0        0    29603 2024-04-02 10:52:57.893706 libhreels-2.2.0/libhreels/calcHREELS20.png
+-rwxr-xr-x   0        0        0    11829 2024-04-02 10:59:12.652766 libhreels-2.2.0/libhreels/calcHREELS20.py
+-rwxr-xr-x   0        0        0     9311 2024-04-02 10:52:57.901232 libhreels-2.2.0/libhreels/dielectrics20.py
+-rwxr-xr-x   0        0        0     1493 2024-04-02 10:52:57.906935 libhreels-2.2.0/libhreels/expLogbook.py
+-rwxr-xr-x   0        0        0     7845 2024-04-02 10:52:57.909814 libhreels-2.2.0/libhreels/materials20.json
+-rwxr-xr-x   0        0        0     1848 2024-04-02 10:52:57.913091 libhreels-2.2.0/libhreels/mod_doeels.mod
+-rwxr-xr-x   0        0        0   202528 2024-04-02 10:56:56.321840 libhreels-2.2.0/libhreels/myBoson.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0   210696 2024-04-02 10:52:57.931834 libhreels-2.2.0/libhreels/myBoson.cpython-36m-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0   257256 2024-04-02 10:52:57.954938 libhreels-2.2.0/libhreels/myBoson.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    26782 2024-04-02 10:52:57.960799 libhreels-2.2.0/libhreels/myBoson.f90
+-rwxr-xr-x   0        0        0    20031 2024-04-02 10:52:57.964565 libhreels-2.2.0/libhreels/myBoson.o
+-rwxr-xr-x   0        0        0   320112 2024-04-02 10:57:10.572316 libhreels-2.2.0/libhreels/myEels20.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0   399688 2024-04-02 10:52:58.004341 libhreels-2.2.0/libhreels/myEels20.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    32043 2024-04-02 10:52:58.009221 libhreels-2.2.0/libhreels/myEels20.f90
+-rwxr-xr-x   0        0        0     8583 2024-04-02 10:52:58.012215 libhreels-2.2.0/libhreels/viewauger.ui
+-rwxr-xr-x   0        0        0    10420 2024-04-02 10:52:58.016257 libhreels-2.2.0/libhreels/viewhreels.ui
+-rwxr-xr-x   0        0        0      963 2024-04-02 10:52:58.019187 libhreels-2.2.0/libhreels/viewhreels_dialog.ui
+-rwxr-xr-x   0        0        0     1032 2024-04-02 12:20:57.110389 libhreels-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4564 1970-01-01 00:00:00.000000 libhreels-2.2.0/PKG-INFO
```

### Comparing `libhreels-2.1.1/README.md` & `libhreels-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/Auger.py` & `libhreels-2.2.0/libhreels/Auger.py`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/HREELS.py` & `libhreels-2.2.0/libhreels/HREELS.py`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/LEED.py` & `libhreels-2.2.0/libhreels/LEED.py`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/README.md` & `libhreels-2.2.0/libhreels/README.md`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/ViewAuger.py` & `libhreels-2.2.0/libhreels/ViewAuger.py`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/ViewHREELS.py` & `libhreels-2.2.0/libhreels/ViewHREELS.py`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/calcHREELS20.png` & `libhreels-2.2.0/libhreels/calcHREELS20.png`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/calcHREELS20.py` & `libhreels-2.2.0/libhreels/calcHREELS20.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 from libhreels.HREELS import myPath
 from copy import deepcopy
 
 import scipy.integrate as integrate
 
 libDir = os.path.dirname(os.path.realpath(__file__)) 
 
-if not (sys.version.startswith('3.6') or sys.version.startswith('3.8')):
-    print('''Make sure the Fortran routines 'myEels20' and 'myBoson' 
-    have been complied with the proper f2py3 for the right 
-    python version!!''') 
 try:
     from libhreels import myEels20 as LambinEELS   # wrapper for myEels20.f90
     from libhreels import myBoson as LambinBoson  # wrapper for myBoson.f90
 except:
     print('myEels20 and MyBoson are not available here (Check your version)')			
+    print('''Make sure the Fortran routines 'myEels20' and 'myBoson' 
+    have been complied with the proper f2py for the right python version!!''')
+    print('\n\n\n')
 
 # Experimental setup as dictionary:
 setup = {
     "e0": 4.0,
     "theta": 60.,
     "phia": 0.33,
     "phib": 2.0,
```

### Comparing `libhreels-2.1.1/libhreels/dielectrics20.py` & `libhreels-2.2.0/libhreels/dielectrics20.py`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/expLogbook.py` & `libhreels-2.2.0/libhreels/expLogbook.py`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/materials20.json` & `libhreels-2.2.0/libhreels/materials20.json`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/mod_doeels.mod` & `libhreels-2.2.0/libhreels/mod_doeels.mod`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/myBoson.cpython-36m-x86_64-linux-gnu.so` & `libhreels-2.2.0/libhreels/myBoson.cpython-36m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/myBoson.cpython-38-x86_64-linux-gnu.so` & `libhreels-2.2.0/libhreels/myBoson.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/myBoson.f90` & `libhreels-2.2.0/libhreels/myBoson.f90`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/myBoson.o` & `libhreels-2.2.0/libhreels/myBoson.o`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/myEels20.cpython-38-x86_64-linux-gnu.so` & `libhreels-2.2.0/libhreels/myEels20.cpython-38-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/myEels20.f90` & `libhreels-2.2.0/libhreels/myEels20.f90`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/viewauger.ui` & `libhreels-2.2.0/libhreels/viewauger.ui`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/viewhreels.ui` & `libhreels-2.2.0/libhreels/viewhreels.ui`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/libhreels/viewhreels_dialog.ui` & `libhreels-2.2.0/libhreels/viewhreels_dialog.ui`

 * *Files identical despite different names*

### Comparing `libhreels-2.1.1/pyproject.toml` & `libhreels-2.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [tool.poetry]
 name = "libhreels"
-version = "2.1.1"
+version = "2.2.0"
 description = "Handling, simulating, and plotting HREELS and Auger spectroscopy data"
 authors = ["Wolf Widdra <wolf.widdra@physik.uni-halle.de>"]
 include = ["*./libhreels/*"]
 exclude = ["./libhreels/eLog*"]
 readme = "README.md"
 homepage = "https://gitlab.informatik.uni-halle.de/e3fm8/libhreels"
 
 
 [tool.poetry.dependencies]
-importlib-metadata = {version = "^1.0", python = "<3.8"} 
+importlib-metadata = {version = "^1.0", python = "<4.0"} 
 python = "^3.8"
-matplotlib = "^3.2"
-scipy = "^1.4"
-#elog = {url = "https://github.com/paulscherrerinstitute/py_elog/archive/master.zip"}
+matplotlib = "^3.8"
+scipy = "^1.10"
 requests = "^2.23.0"
 argparse = "^1.4.0"
-numpy = "^1.18.2"
+numpy = "^1.22"
+PyQt5-Qt5 = "^5.15.2"
+PyQt5 = "^5.15"
+
 #elog = {url = "https://github.com/paulscherrerinstitute/py_elog/archive/master.zip"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 
 [tool.poetry.scripts]
 dielectrics = "libhreels.dielectrics:myMain"
 calchreels = "libhreels.calcHREELS20:myMain"
-viewhreelstest = "libhreels.ViewHREELS:myMain"
 
 [tool.poetry.plugins."gui_scripts"]
 viewauger = "libhreels.ViewAuger:myMain"
-viewhreels = "libhreels.ViewHREELS20:myMain"
+viewhreels = "libhreels.ViewHREELS:myMain"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `libhreels-2.1.1/PKG-INFO` & `libhreels-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: libhreels
-Version: 2.1.1
+Version: 2.2.0
 Summary: Handling, simulating, and plotting HREELS and Auger spectroscopy data
 Home-page: https://gitlab.informatik.uni-halle.de/e3fm8/libhreels
 Author: Wolf Widdra
 Author-email: wolf.widdra@physik.uni-halle.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyQt5 (>=5.15,<6.0)
+Requires-Dist: PyQt5-Qt5 (>=5.15.2,<6.0.0)
 Requires-Dist: argparse (>=1.4.0,<2.0.0)
-Requires-Dist: importlib-metadata (>=1.0,<2.0) ; python_version < "3.8"
-Requires-Dist: matplotlib (>=3.2,<4.0)
-Requires-Dist: numpy (>=1.18.2,<2.0.0)
+Requires-Dist: importlib-metadata (>=1.0,<2.0) ; python_version < "4.0"
+Requires-Dist: matplotlib (>=3.8,<4.0)
+Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
-Requires-Dist: scipy (>=1.4,<2.0)
+Requires-Dist: scipy (>=1.10,<2.0)
 Description-Content-Type: text/markdown
 
 # HREELS data handling and simulation
 
 Set of data analysis routines for surface vibrational spectroscopy based on a Delta05 spectrometer with software from VSI or SPECS. 
 
 Simple data reading and plotting routines are provided, but also advanced routines for in depth analysis.
```

