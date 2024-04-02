# Comparing `tmp/pymonke-0.0.5.tar.gz` & `tmp/pymonke-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonke-0.0.5.tar", last modified: Fri Mar 15 15:06:13 2024, max compression
+gzip compressed data, was "pymonke-0.1.0.tar", last modified: Tue Apr  2 20:39:27 2024, max compression
```

## Comparing `pymonke-0.0.5.tar` & `pymonke-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,74 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.514830 pymonke-0.0.5/
--rw-rw-rw-   0        0        0     1095 2024-01-31 16:24:15.000000 pymonke-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      597 2024-03-15 15:06:13.514830 pymonke-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5033 2024-03-03 13:48:10.000000 pymonke-0.0.5/README.md
--rw-rw-rw-   0        0        0      160 2024-03-03 13:48:10.000000 pymonke-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      724 2024-03-15 15:06:13.515835 pymonke-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.480765 pymonke-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.489257 pymonke-0.0.5/src/pymonke/
--rw-rw-rw-   0        0        0      146 2024-03-15 14:31:02.000000 pymonke-0.0.5/src/pymonke/__init__.py
--rw-rw-rw-   0        0        0     1548 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/constants.py
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.496783 pymonke-0.0.5/src/pymonke/fit/
--rw-rw-rw-   0        0        0       57 2024-03-15 14:30:24.000000 pymonke-0.0.5/src/pymonke/fit/__init__.py
--rw-rw-rw-   0        0        0     7589 2024-03-15 14:33:02.000000 pymonke-0.0.5/src/pymonke/fit/fit.py
--rw-rw-rw-   0        0        0     1625 2024-03-15 09:08:19.000000 pymonke-0.0.5/src/pymonke/fit/fit_result.py
--rw-rw-rw-   0        0        0     4161 2024-03-15 08:02:06.000000 pymonke-0.0.5/src/pymonke/fit/parse.py
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.497283 pymonke-0.0.5/src/pymonke/gui/
--rw-rw-rw-   0        0        0        0 2024-03-15 14:48:59.000000 pymonke-0.0.5/src/pymonke/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.502282 pymonke-0.0.5/src/pymonke/latex/
--rw-rw-rw-   0        0        0      157 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/latex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.503787 pymonke-0.0.5/src/pymonke/latex/tests/
--rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/latex/tests/__init__.py
--rw-rw-rw-   0        0        0     1225 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/latex/tests/table_test.py
--rw-rw-rw-   0        0        0     3121 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/latex/tex_table.py
--rw-rw-rw-   0        0        0     3098 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/latex/tex_tabular.py
--rw-rw-rw-   0        0        0     4323 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/latex/tex_tabular.pyi
--rw-rw-rw-   0        0        0     3298 2024-03-13 17:50:44.000000 pymonke-0.0.5/src/pymonke/latex/utils.py
--rw-rw-rw-   0        0        0     1549 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/latex/utils.pyi
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.506385 pymonke-0.0.5/src/pymonke/misc/
--rw-rw-rw-   0        0        0        0 2024-03-13 17:06:30.000000 pymonke-0.0.5/src/pymonke/misc/__init__.py
--rw-rw-rw-   0        0        0     1267 2024-03-14 08:45:57.000000 pymonke-0.0.5/src/pymonke/misc/dataframe.py
--rw-rw-rw-   0        0        0      976 2024-03-13 17:40:45.000000 pymonke-0.0.5/src/pymonke/misc/file_management.py
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.509809 pymonke-0.0.5/src/pymonke/mmath/
--rw-rw-rw-   0        0        0      107 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/mmath/__init__.py
--rw-rw-rw-   0        0        0     2671 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/mmath/num_with_error.py
--rw-rw-rw-   0        0        0     1177 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/mmath/rounding.py
--rw-rw-rw-   0        0        0      890 2024-03-14 10:22:20.000000 pymonke-0.0.5/src/pymonke/mmath/statistics.py
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.512309 pymonke-0.0.5/src/pymonke/mmath/tests/
--rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/mmath/tests/__init__.py
--rw-rw-rw-   0        0        0     5073 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/mmath/tests/num_with_error_test.py
--rw-rw-rw-   0        0        0      678 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/mmath/tests/rounding_test.py
--rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.0.5/src/pymonke/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.513813 pymonke-0.0.5/src/pymonke.egg-info/
--rw-rw-rw-   0        0        0      597 2024-03-15 15:06:13.000000 pymonke-0.0.5/src/pymonke.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1038 2024-03-15 15:06:13.000000 pymonke-0.0.5/src/pymonke.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 15:06:13.000000 pymonke-0.0.5/src/pymonke.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-03-15 15:06:13.000000 pymonke-0.0.5/src/pymonke.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-15 15:06:13.000000 pymonke-0.0.5/src/pymonke.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-15 15:06:13.512808 pymonke-0.0.5/tests/
--rw-rw-rw-   0        0        0      110 2024-03-13 18:05:18.000000 pymonke-0.0.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.131871 pymonke-0.1.0/
+-rw-rw-rw-   0        0        0     1095 2024-01-31 16:24:15.000000 pymonke-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      660 2024-04-02 20:39:27.131871 pymonke-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5033 2024-03-03 13:48:10.000000 pymonke-0.1.0/README.md
+-rw-rw-rw-   0        0        0      160 2024-03-03 13:48:10.000000 pymonke-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      899 2024-04-02 20:39:27.132876 pymonke-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.068730 pymonke-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.079242 pymonke-0.1.0/src/pymonke/
+-rw-rw-rw-   0        0        0      333 2024-04-02 12:37:38.000000 pymonke-0.1.0/src/pymonke/__init__.py
+-rw-rw-rw-   0        0        0      269 2024-03-15 15:51:29.000000 pymonke-0.1.0/src/pymonke/__main__.py
+-rw-rw-rw-   0        0        0     1548 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.088260 pymonke-0.1.0/src/pymonke/fit/
+-rw-rw-rw-   0        0        0      133 2024-03-29 19:58:06.000000 pymonke-0.1.0/src/pymonke/fit/__init__.py
+-rw-rw-rw-   0        0        0     1106 2024-03-29 19:57:55.000000 pymonke-0.1.0/src/pymonke/fit/__misc.py
+-rw-rw-rw-   0        0        0    10447 2024-04-02 14:16:53.000000 pymonke-0.1.0/src/pymonke/fit/fit.py
+-rw-rw-rw-   0        0        0     1601 2024-04-02 12:34:08.000000 pymonke-0.1.0/src/pymonke/fit/fit_result.py
+-rw-rw-rw-   0        0        0     6700 2024-04-02 12:41:49.000000 pymonke-0.1.0/src/pymonke/fit/parse.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.098786 pymonke-0.1.0/src/pymonke/gui/
+-rw-rw-rw-   0        0        0      289 2024-03-22 17:45:13.000000 pymonke-0.1.0/src/pymonke/gui/__init__.py
+-rw-rw-rw-   0        0        0     3840 2024-03-25 21:06:09.000000 pymonke-0.1.0/src/pymonke/gui/app.py
+-rw-rw-rw-   0        0        0     1185 2024-03-23 22:03:51.000000 pymonke-0.1.0/src/pymonke/gui/browse_frame.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.102792 pymonke-0.1.0/src/pymonke/gui/data_init/
+-rw-rw-rw-   0        0        0        0 2024-03-17 12:55:10.000000 pymonke-0.1.0/src/pymonke/gui/data_init/__init__.py
+-rw-rw-rw-   0        0        0      751 2024-03-23 20:42:12.000000 pymonke-0.1.0/src/pymonke/gui/data_init/browse_save_frame.py
+-rw-rw-rw-   0        0        0     5217 2024-03-24 15:12:49.000000 pymonke-0.1.0/src/pymonke/gui/data_init/data_init_frame.py
+-rw-rw-rw-   0        0        0     1398 2024-03-24 08:58:03.000000 pymonke-0.1.0/src/pymonke/gui/data_init/status_frame.py
+-rw-rw-rw-   0        0        0     5729 2024-03-25 15:55:43.000000 pymonke-0.1.0/src/pymonke/gui/dict_frame.py
+-rw-rw-rw-   0        0        0     1123 2024-03-23 22:07:47.000000 pymonke-0.1.0/src/pymonke/gui/entry_label_frame.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.107312 pymonke-0.1.0/src/pymonke/gui/fitting/
+-rw-rw-rw-   0        0        0     3505 2024-03-25 22:43:11.000000 pymonke-0.1.0/src/pymonke/gui/fitting/add_args_frame.py
+-rw-rw-rw-   0        0        0    10157 2024-03-25 22:19:06.000000 pymonke-0.1.0/src/pymonke/gui/fitting/fit_frame.py
+-rw-rw-rw-   0        0        0     2462 2024-03-24 15:12:59.000000 pymonke-0.1.0/src/pymonke/gui/fitting/fit_option_menu.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.110311 pymonke-0.1.0/src/pymonke/gui/formula/
+-rw-rw-rw-   0        0        0     2889 2024-03-23 21:13:25.000000 pymonke-0.1.0/src/pymonke/gui/formula/formula_frame.py
+-rw-rw-rw-   0        0        0     1424 2024-03-23 21:18:19.000000 pymonke-0.1.0/src/pymonke/gui/formula/parameter_frame.py
+-rw-rw-rw-   0        0        0     2421 2024-03-23 21:25:28.000000 pymonke-0.1.0/src/pymonke/gui/formula/parameters_scrollable_frame.py
+-rw-rw-rw-   0        0        0      388 2024-03-23 21:44:32.000000 pymonke-0.1.0/src/pymonke/gui/info_label.py
+-rw-rw-rw-   0        0        0      561 2024-03-25 22:19:40.000000 pymonke-0.1.0/src/pymonke/gui/labeled_entry.py
+-rw-rw-rw-   0        0        0     2628 2024-03-25 15:19:40.000000 pymonke-0.1.0/src/pymonke/gui/list_frame.py
+-rw-rw-rw-   0        0        0       85 2024-03-23 22:16:21.000000 pymonke-0.1.0/src/pymonke/gui/main.py
+-rw-rw-rw-   0        0        0     3038 2024-03-23 22:27:18.000000 pymonke-0.1.0/src/pymonke/gui/misc.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.114337 pymonke-0.1.0/src/pymonke/gui/plot/
+-rw-rw-rw-   0        0        0     3560 2024-03-25 13:24:18.000000 pymonke-0.1.0/src/pymonke/gui/plot/limits_frame.py
+-rw-rw-rw-   0        0        0     4806 2024-03-26 15:12:55.000000 pymonke-0.1.0/src/pymonke/gui/plot/misc_data_frame.py
+-rw-rw-rw-   0        0        0     2114 2024-03-24 10:01:38.000000 pymonke-0.1.0/src/pymonke/gui/plot/plot_canvas.py
+-rw-rw-rw-   0        0        0     4544 2024-04-02 20:38:13.000000 pymonke-0.1.0/src/pymonke/gui/plot/plot_frame.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.118842 pymonke-0.1.0/src/pymonke/latex/
+-rw-rw-rw-   0        0        0      175 2024-04-02 12:24:16.000000 pymonke-0.1.0/src/pymonke/latex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.120842 pymonke-0.1.0/src/pymonke/latex/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/latex/tests/__init__.py
+-rw-rw-rw-   0        0        0     1225 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/latex/tests/table_test.py
+-rw-rw-rw-   0        0        0     3096 2024-04-02 08:30:50.000000 pymonke-0.1.0/src/pymonke/latex/tex_table.py
+-rw-rw-rw-   0        0        0     4420 2024-04-02 11:45:56.000000 pymonke-0.1.0/src/pymonke/latex/utils.py
+-rw-rw-rw-   0        0        0     1549 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/latex/utils.pyi
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.126372 pymonke-0.1.0/src/pymonke/misc/
+-rw-rw-rw-   0        0        0        0 2024-03-13 17:06:30.000000 pymonke-0.1.0/src/pymonke/misc/__init__.py
+-rw-rw-rw-   0        0        0     1853 2024-04-02 12:26:57.000000 pymonke-0.1.0/src/pymonke/misc/benchmark.py
+-rw-rw-rw-   0        0        0     3198 2024-04-02 14:02:30.000000 pymonke-0.1.0/src/pymonke/misc/dataframe.py
+-rw-rw-rw-   0        0        0     1010 2024-04-02 12:27:25.000000 pymonke-0.1.0/src/pymonke/misc/file_management.py
+-rw-rw-rw-   0        0        0      757 2024-04-02 20:39:13.000000 pymonke-0.1.0/src/pymonke/misc/pymonke_json_decoder.py
+-rw-rw-rw-   0        0        0      297 2024-04-02 14:33:51.000000 pymonke-0.1.0/src/pymonke/misc/pymonke_json_encoder.py
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.128872 pymonke-0.1.0/src/pymonke/mmath/
+-rw-rw-rw-   0        0        0       65 2024-04-02 12:36:10.000000 pymonke-0.1.0/src/pymonke/mmath/__init__.py
+-rw-rw-rw-   0        0        0      759 2024-04-02 12:35:53.000000 pymonke-0.1.0/src/pymonke/mmath/rounding.py
+-rw-rw-rw-   0        0        0      890 2024-03-14 10:22:20.000000 pymonke-0.1.0/src/pymonke/mmath/statistics.py
+-rw-rw-rw-   0        0        0        0 2024-03-03 13:48:10.000000 pymonke-0.1.0/src/pymonke/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.130872 pymonke-0.1.0/src/pymonke.egg-info/
+-rw-rw-rw-   0        0        0      660 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1817 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-02 20:39:27.000000 pymonke-0.1.0/src/pymonke.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 20:39:27.129871 pymonke-0.1.0/tests/
+-rw-rw-rw-   0        0        0     2243 2024-04-02 14:13:14.000000 pymonke-0.1.0/tests/test.py
```

### Comparing `pymonke-0.0.5/LICENSE` & `pymonke-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymonke-0.0.5/PKG-INFO` & `pymonke-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pymonke
-Version: 0.0.5
+Version: 0.1.0
 Summary: Tools for creating lab reports and data analysis
 Home-page: https://github.com/GabrielRemi/pymonke
 Author: Gabriel Remiszewski
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: numpy>=1.26
 Requires-Dist: pandas>=2.2
 Requires-Dist: nltk>=3.8
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: mypy_extensions>=1.0
 Requires-Dist: scienceplots>=2.1
+Requires-Dist: customtkinter>=5.2
+Requires-Dist: scipy>=1.12
 
 longer description
```

### Comparing `pymonke-0.0.5/README.md` & `pymonke-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pymonke-0.0.5/setup.cfg` & `pymonke-0.1.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 6f6e 6b65 0d0a 7665 7273   = pymonke..vers
-00000020: 696f 6e20 3d20 302e 302e 350d 0a61 7574  ion = 0.0.5..aut
+00000020: 696f 6e20 3d20 302e 312e 300d 0a61 7574  ion = 0.1.0..aut
 00000030: 686f 7220 3d20 4761 6272 6965 6c20 5265  hor = Gabriel Re
 00000040: 6d69 737a 6577 736b 690d 0a64 6573 6372  miszewski..descr
 00000050: 6970 7469 6f6e 203d 2054 6f6f 6c73 2066  iption = Tools f
 00000060: 6f72 2063 7265 6174 696e 6720 6c61 6220  or creating lab 
 00000070: 7265 706f 7274 7320 616e 6420 6461 7461  reports and data
 00000080: 2061 6e61 6c79 7369 730d 0a6c 6f6e 675f   analysis..long_
 00000090: 6465 7363 7269 7074 696f 6e20 3d20 6c6f  description = lo
@@ -26,21 +26,32 @@
 00000190: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
 000001a0: 096e 756d 7079 3e3d 312e 3236 0d0a 0970  .numpy>=1.26...p
 000001b0: 616e 6461 733e 3d32 2e32 0d0a 096e 6c74  andas>=2.2...nlt
 000001c0: 6b3e 3d33 2e38 0d0a 096d 6174 706c 6f74  k>=3.8...matplot
 000001d0: 6c69 623e 3d33 2e38 0d0a 096d 7970 795f  lib>=3.8...mypy_
 000001e0: 6578 7465 6e73 696f 6e73 3e3d 312e 300d  extensions>=1.0.
 000001f0: 0a09 7363 6965 6e63 6570 6c6f 7473 3e3d  ..scienceplots>=
-00000200: 322e 310d 0a0d 0a5b 6d79 7079 5d0d 0a0d  2.1....[mypy]...
-00000210: 0a5b 6d79 7079 2d73 6369 7079 2e2a 5d0d  .[mypy-scipy.*].
-00000220: 0a69 676e 6f72 655f 6d69 7373 696e 675f  .ignore_missing_
-00000230: 696d 706f 7274 7320 3d20 7472 7565 0d0a  imports = true..
-00000240: 0d0a 5b6d 7970 792d 6e6c 746b 2e2a 5d0d  ..[mypy-nltk.*].
-00000250: 0a69 676e 6f72 655f 6d69 7373 696e 675f  .ignore_missing_
-00000260: 696d 706f 7274 7320 3d20 7472 7565 0d0a  imports = true..
-00000270: 0d0a 5b6d 7970 792d 7363 6965 6e63 6570  ..[mypy-sciencep
-00000280: 6c6f 7473 2e2a 5d0d 0a69 676e 6f72 655f  lots.*]..ignore_
-00000290: 6d69 7373 696e 675f 696d 706f 7274 7320  missing_imports 
-000002a0: 3d20 7472 7565 0d0a 0d0a 5b65 6767 5f69  = true....[egg_i
-000002b0: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
-000002c0: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
-000002d0: 0d0a 0d0a                                ....
+00000200: 322e 310d 0a09 6375 7374 6f6d 746b 696e  2.1...customtkin
+00000210: 7465 723e 3d35 2e32 0d0a 0973 6369 7079  ter>=5.2...scipy
+00000220: 3e3d 312e 3132 0d0a 0d0a 5b6d 7970 795d  >=1.12....[mypy]
+00000230: 0d0a 6469 7361 6c6c 6f77 5f75 6e74 7970  ..disallow_untyp
+00000240: 6564 5f64 6566 7320 3d20 5472 7565 0d0a  ed_defs = True..
+00000250: 6469 7361 6c6c 6f77 5f73 7562 636c 6173  disallow_subclas
+00000260: 7369 6e67 5f61 6e79 203d 2046 616c 7365  sing_any = False
+00000270: 0d0a 0d0a 5b6d 7970 792d 7363 6970 792e  ....[mypy-scipy.
+00000280: 2a2c 6e6c 746b 2e2a 2c73 6369 656e 6365  *,nltk.*,science
+00000290: 706c 6f74 732e 2a2c 6375 7374 6f6d 746b  plots.*,customtk
+000002a0: 696e 7465 722e 2a2c 6963 6563 7265 616d  inter.*,icecream
+000002b0: 2c75 6e63 6572 7461 696e 7469 6573 2e2a  ,uncertainties.*
+000002c0: 5d0d 0a69 676e 6f72 655f 6d69 7373 696e  ]..ignore_missin
+000002d0: 675f 696d 706f 7274 7320 3d20 7472 7565  g_imports = true
+000002e0: 0d0a 0d0a 5b6d 7970 792d 6d61 7470 6c6f  ....[mypy-matplo
+000002f0: 746c 6962 2e62 6163 6b65 6e64 732e 2a5d  tlib.backends.*]
+00000300: 0d0a 696d 706c 6963 6974 5f72 6565 7870  ..implicit_reexp
+00000310: 6f72 7420 3d20 5472 7565 0d0a 6469 7361  ort = True..disa
+00000320: 6c6c 6f77 5f75 6e74 7970 6564 5f64 6566  llow_untyped_def
+00000330: 7320 3d20 4661 6c73 650d 0a63 6865 636b  s = False..check
+00000340: 5f75 6e74 7970 6564 5f64 6566 7320 3d20  _untyped_defs = 
+00000350: 4661 6c73 650d 0a0d 0a5b 6567 675f 696e  False....[egg_in
+00000360: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000370: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000380: 0a0d 0a                                  ...
```

### Comparing `pymonke-0.0.5/src/pymonke/constants.py` & `pymonke-0.1.0/src/pymonke/constants.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.0.5/src/pymonke/fit/fit_result.py` & `pymonke-0.1.0/src/pymonke/fit/fit_result.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import pandas as pd
 from mypy_extensions import VarArg
 import numpy as np
-from pandas import DataFrame
+from uncertainties import ufloat
 
 from dataclasses import dataclass, field
-from typing import List, Dict, Callable, TypeAlias, Iterable
+from typing import List, Dict, Callable, TypeAlias, Iterable, Any
 
-from ..mmath import NumWithError
 
 scalar: TypeAlias = int | float
 array: TypeAlias = np.ndarray | pd.Series
 numerical: TypeAlias = scalar | array
 
 
 @dataclass(repr=True)
@@ -25,18 +24,18 @@
         """Calculated values of the fitted function"""
         result = self.function(x, *self.parameter_values)
         if isinstance(result, Iterable):
             return np.array(result)
         else:
             return float(result)
 
-    def as_dict(self, chi_square=False) -> dict[str, NumWithError]:
+    def as_dict(self, chi_square: bool = False) -> dict[str, Any | float]:
         result: dict = dict()
         for name, x, sigma in zip(self.parameter_names, self.parameter_values, self.parameter_sigmas):
-            result[name] = NumWithError(x, sigma)
+            result[name] = ufloat(x, sigma)
 
         if chi_square:
             result["reduced_chi_squared"] = self.reduced_chi_squared
 
         return result
 
     def set_reduced_chi_squared(self, x: array, y: array, sigma: array) -> float:
```

### Comparing `pymonke-0.0.5/src/pymonke/fit/parse.py` & `pymonke-0.1.0/src/pymonke/fit/parse.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from mypy_extensions import VarArg
 import nltk
 import numpy as np
 from pandas import Series
 
 from typing import Callable, List, Tuple, TypeAlias, Iterable, Dict
+from .fit_result import FitResult
 
 scalar: TypeAlias = float | int
 array: TypeAlias = Series | np.ndarray
 numerical: TypeAlias = scalar | array
 func_type: TypeAlias = Callable[[VarArg(str)], str]
 
 
+class RepetitionError(Exception):
+    def __init__(self):
+        super().__init__("Trying to change name of a parameter, but name already exists.")
+
+
 def __gauss(*args: str) -> str:
     return f"({args[0]} * exp((-(x - {args[1]}) ** 2) / (2 * {args[2]} ** 2)))"
 
 
 def __linear(*args: str) -> str:
     return f"({args[0]} * x + {args[1]})"
 
@@ -68,24 +74,38 @@
               not token.isnumeric() and token != "x")
     if answer and token[0].isnumeric():
         raise ValueError("param names cannot start with a number")
     return answer
 
 
 def rename_parameters(_formula: str, rename: Dict[str, str]) -> str:
+    # check for duplicates in rename dict
+    if len(rename.values()) != len(set(rename.values())):
+        raise RepetitionError
+
     tokens = nltk.tokenize.wordpunct_tokenize(_formula)
+    params = get_params(tokens)
     for index, token in enumerate(tokens):
         for key in rename.keys():
+            if (new := rename[key]) == key:
+                continue
+            else:
+                if new in params:
+                    raise RepetitionError
+            if not __is_param(new):
+                raise ValueError("invalid parameter name")
             if key == token:
-                tokens[index] = rename[key]
+                tokens[index] = new
 
     return "".join(tokens)
 
 
 def replace_funcs(_formula: str) -> str:
+    if _formula == "":
+        return _formula
     tokens = nltk.tokenize.wordpunct_tokenize(_formula)
     params: List[str] = []
     for token in tokens:
         if __is_param(token) and token not in params:
             params.append(token)
 
     for index, token in enumerate(tokens):
@@ -93,14 +113,22 @@
             b = [__get_unique_name(i, params) for i in __FUNCS[token][1]]
             tokens[index] = __FUNCS[token][0](*b)
             params.extend(b)
 
     return "".join(tokens)
 
 
+def get_params(tokens: List[str]) -> List[str]:
+    params: List[str] = []
+    for index, token in enumerate(tokens):
+        if __is_param(token):
+            params.append(token)
+    return params
+
+
 def parse_function(_formula: str) -> Tuple[Callable[[numerical, VarArg(float | int)], numerical], List[str]]:
     """Creates a python function out of a string that represents a mathematical formula.
     x is the variable and all the other arguments are passed as positional arguments to the
     generated callable with the form f(x: float, *params) -> float.
     Returns the callable and a list of all the arguments mentioned in _formula"""
     tokens = nltk.tokenize.wordpunct_tokenize(_formula)
     params: List[str] = []
@@ -127,8 +155,54 @@
             if tok == "x":
                 _tokens[i] = str(x)
         string = " ".join(_tokens)
         for op in __SYMBOL_OPERATORS.keys():
             string = string.replace(op, __SYMBOL_OPERATORS[op])
         return eval(string)
 
+    try:
+        function(0, *([0] * len(params)))
+    except SyntaxError as e:
+        raise SyntaxError(e)
+    except ArithmeticError:
+        pass
+
     return function, params
+
+
+def parse_variable_str(label_str: str, result: FitResult) -> str:
+    """Reads a string that has variable names marked with '#' and replaces them with their values
+    from the FitResult object."""
+    res_dict = result.as_dict(chi_square=True)
+    tokens = label_str.split()
+    for index, tok in enumerate(tokens):
+        if tok[0] != "#":
+            continue
+        tok = tok[1:]
+        key_error = f"Parameter {tok} not found. Please check if your parameters are correct."
+        value_error = f"Cannot access attribute of parameter {tok}. Only #paramter.val or #paramter.err are "
+        f"allowed as inputs"
+        if "." not in tok:
+            if tok == "chi":
+                tokens[index] = str(round(res_dict["reduced_chi_squared"], 2))
+            else:
+                try:
+                    tokens[index] = str(res_dict[tok])
+                except KeyError:
+                    raise KeyError(key_error)
+        else:
+            try:
+                param, attr = tok.split(".")
+            except:
+                raise ValueError(value_error)
+            try:
+                if attr == "val":
+                    tokens[index] = str(res_dict[param].nominal_value)
+                elif attr == "err":
+                    tokens[index] = str(res_dict[param].std_dev)
+                else:
+                    raise ValueError(value_error)
+            except KeyError:
+                raise KeyError(key_error)
+
+
+    return " ".join(tokens)
```

### Comparing `pymonke-0.0.5/src/pymonke/latex/tests/table_test.py` & `pymonke-0.1.0/src/pymonke/latex/tests/table_test.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.0.5/src/pymonke/latex/tex_table.py` & `pymonke-0.1.0/src/pymonke/latex/tex_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from dataclasses import dataclass, field
 from typing import List
 
-from .tex_tabular import TexTabular
-
 
 @dataclass(repr=True)
 class TexTable:
     r"""Class for generating a LaTeX table. The idea behind this class is to have the ability to
      create a table with multiple tabular environments, in the case where the user wants to have
      multiple tabular environments side by side.
      In the case where one tabular environment is enough, this class is not necessary to generate a LaTeX table.
 
      Parameters
      ----------
      positioning: str
      Is "htbp" by default and defines the position behavior of the table.
-     tabular: List[TexTabular]
-     Defines a list with tabular objects inside, which contain the data for the tabular environments.
+     tabular: List[str]
+     Defines a list with strings that represent latex tabulars inside, which contain the data for the tabular
+     environments.
      widths: List[float]
      Defines the space relative to the line width of the page that is given for the tabular environments.
      It is a list that should have the same length as the `tabular list.
      spacing: List[float | str]
      Defines the spacing between two tabular environments. It is a list which should be shorter by one
      than the `tabular` list. An element could be a string, which will be inserted verbosely, but in the case
      of a floating point number, it will be inserted as an argument to the `hspace` macro.
      """
-    tabular: List[TexTabular]
+    tabular: List[str]
     positioning: str = "htbp"
     widths: List[float] = field(default_factory=list)
     spacing: List[float | str] = field(default_factory=list)
 
     def save(self, file_path: str, method: str = "w") -> None:
         r"""Saves the LaTeX table to a file specified by `file_path`. The `method` argument is the same as
         for the builtin `open()` function."""
```

### Comparing `pymonke-0.0.5/src/pymonke/latex/utils.py` & `pymonke-0.1.0/src/pymonke/latex/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 
-from typing import List
+from uncertainties import ufloat
+from typing import Any
 
-from ..mmath.num_with_error import NumWithError
 from ..misc.dataframe import get_error_column_name
 
 
-def transform_dataframe_to_latex_ready(data, **kwargs):
+def transform_dataframe_to_latex_ready(data: pd.DataFrame, **kwargs: Any) -> pd.DataFrame:
     # initialize all keyword arguments
     if kwargs.get("error_marker") is None:
         kwargs["error_marker"] = ["err", "error", "fehler", "Err", "Error", "Fehler"]
     else:
         list(kwargs["error_marker"])
     if kwargs.get("columns") is None:
         kwargs["columns"] = {}
@@ -26,32 +26,36 @@
         raise TypeError("is_table must be a boolean")
     if kwargs.get("siunitx_column_option") is None:
         kwargs["siunitx_column_option"] = {}
     else:
         dict(kwargs["siunitx_column_option"])
 
     new_dataframe = data.copy()  # new dataframe for end result
+    new_dataframe = new_dataframe.apply(lambda x: replace_ufloat_with_latex_macro(x, **kwargs), axis=0)
 
     # look for columns with errors
     for column in data.columns:
         error = get_error_column_name(data, column, kwargs["error_marker"])
         if error is None:
             continue
         num_data = data[column]
         error_data = data[error]
         new_data = []
         option: str | None = kwargs["siunitx_column_option"].get(column)
         for x, err in zip(num_data, error_data):
-            if kwargs["is_table_num"]:
-                new_data.append(NumWithError(x, err).display_table_separate(option))
-            else:
-                new_data.append(NumWithError(x, err).display_separate(option))
+            num = "{:S}".format(ufloat(x, err))
+            # if kwargs["is_table_num"]:
+            #     new_data.append(NumWithError(x, err).display_table_separate(option))
+            # else:
+            #     new_data.append(NumWithError(x, err).display_separate(option))
+            new_data.append(num_in_siunitx(num, kwargs["is_table_num"], option))
         new_dataframe[column] = new_data
         new_dataframe.drop(error, axis=1, inplace=True)
 
+
     if kwargs["ignore_rest"]:
         columns = list(new_dataframe.columns)
         columns_to_ignore = [c for c in columns if c not in kwargs["columns"]]
         new_dataframe.drop(columns=columns_to_ignore, inplace=True)
 
     for col in list(new_dataframe.columns):
         option = kwargs["siunitx_column_option"].get(col)
@@ -60,14 +64,41 @@
                               for i in new_dataframe[col]]
 
     new_dataframe.rename(columns=kwargs["columns"], inplace=True)
 
     return new_dataframe
 
 
+def num_in_siunitx(num: str, is_table_num: bool = False, option: str | None = None) -> str:
+    """Wraps number string insided \num or \tablenum macro depending on is_table_num boolean.
+    option is another string put in []  as a macro option. """
+    if is_table_num:
+        text = "tablenum"
+    else:
+        text = "num"
+    if option is None:
+        option = ""
+    else:
+        option = f"[{option}]"
+
+    return f"\\{text}{option}{{{num}}}"
+
+
+def replace_ufloat_with_latex_macro(x: pd.Series, **kwargs: Any) -> pd.Series:
+    def func(i: Any) -> Any:
+        try:
+            val = "{:S}".format(i)
+            return num_in_siunitx(val, kwargs.get("is_table_num") or False,
+                                  kwargs["siunitx_column_option"].get(x.name))
+        except:
+            return i
+
+    return x.apply(func)
+
+
 def __display_num_value(x: int | float, option: str | None = None, is_table_num: bool = True) -> str | None:
     """takes a number and formats it to use with the siunitx package. Returns None if the value is not a number
     Example
     -------
     __display_num_value(2.3, sinuitx_option="round-mode=figures") -> \tablenum[round-mode=figures]{2.3}"""
     if str(x) == "nan":
         return None
```

### Comparing `pymonke-0.0.5/src/pymonke/latex/utils.pyi` & `pymonke-0.1.0/src/pymonke/latex/utils.pyi`

 * *Files identical despite different names*

### Comparing `pymonke-0.0.5/src/pymonke/misc/file_management.py` & `pymonke-0.1.0/src/pymonke/misc/file_management.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import numpy as np
 import pandas as pd
 from pandas import DataFrame
 
-from typing import List
+from typing import List, Any
 
 
 def get_file_type(filename: str) -> str:
     return filename.split('.')[-1]
 
 
-def read_txt_into_dataframe(file: str, skiprows: int = 1, **args) -> DataFrame:
+def read_txt_into_dataframe(file: str, skiprows: int = 1, **args: Any) -> DataFrame:
     columns: List[str]
     with open(file, 'r') as f:
         if (delim := args.get("delimiter")) is None:
             delim = " "
-        columns = f.readline().replace(delim, " ").replace("\n", "").split(" ")
+        columns = f.readline().replace(delim, " ").replace("\t", " ").replace("\n", "").split(" ")
     data = np.loadtxt(file, skiprows=skiprows, **args)
     return DataFrame(data=data, columns=columns)
 
 
-def read_data_into_dataframe(file: str, **args) -> DataFrame:
+def read_data_into_dataframe(file: str, **args: Any) -> DataFrame:
     """tries to Convert the file into a DataFrame"""
     file_type = get_file_type(file)
     if file_type == "csv":
         return pd.read_csv(file, **args)
     elif file_type == "txt":
         return read_txt_into_dataframe(file, **args)
     else:
```

### Comparing `pymonke-0.0.5/src/pymonke/mmath/statistics.py` & `pymonke-0.1.0/src/pymonke/mmath/statistics.py`

 * *Files identical despite different names*

### Comparing `pymonke-0.0.5/src/pymonke.egg-info/PKG-INFO` & `pymonke-0.1.0/src/pymonke.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pymonke
-Version: 0.0.5
+Version: 0.1.0
 Summary: Tools for creating lab reports and data analysis
 Home-page: https://github.com/GabrielRemi/pymonke
 Author: Gabriel Remiszewski
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: numpy>=1.26
 Requires-Dist: pandas>=2.2
 Requires-Dist: nltk>=3.8
 Requires-Dist: matplotlib>=3.8
 Requires-Dist: mypy_extensions>=1.0
 Requires-Dist: scienceplots>=2.1
+Requires-Dist: customtkinter>=5.2
+Requires-Dist: scipy>=1.12
 
 longer description
```

### Comparing `pymonke-0.0.5/src/pymonke.egg-info/SOURCES.txt` & `pymonke-0.1.0/src/pymonke.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,58 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/pymonke/__init__.py
+src/pymonke/__main__.py
 src/pymonke/constants.py
 src/pymonke/py.typed
 src/pymonke.egg-info/PKG-INFO
 src/pymonke.egg-info/SOURCES.txt
 src/pymonke.egg-info/dependency_links.txt
 src/pymonke.egg-info/requires.txt
 src/pymonke.egg-info/top_level.txt
 src/pymonke/fit/__init__.py
+src/pymonke/fit/__misc.py
 src/pymonke/fit/fit.py
 src/pymonke/fit/fit_result.py
 src/pymonke/fit/parse.py
 src/pymonke/gui/__init__.py
+src/pymonke/gui/app.py
+src/pymonke/gui/browse_frame.py
+src/pymonke/gui/dict_frame.py
+src/pymonke/gui/entry_label_frame.py
+src/pymonke/gui/info_label.py
+src/pymonke/gui/labeled_entry.py
+src/pymonke/gui/list_frame.py
+src/pymonke/gui/main.py
+src/pymonke/gui/misc.py
+src/pymonke/gui/data_init/__init__.py
+src/pymonke/gui/data_init/browse_save_frame.py
+src/pymonke/gui/data_init/data_init_frame.py
+src/pymonke/gui/data_init/status_frame.py
+src/pymonke/gui/fitting/add_args_frame.py
+src/pymonke/gui/fitting/fit_frame.py
+src/pymonke/gui/fitting/fit_option_menu.py
+src/pymonke/gui/formula/formula_frame.py
+src/pymonke/gui/formula/parameter_frame.py
+src/pymonke/gui/formula/parameters_scrollable_frame.py
+src/pymonke/gui/plot/limits_frame.py
+src/pymonke/gui/plot/misc_data_frame.py
+src/pymonke/gui/plot/plot_canvas.py
+src/pymonke/gui/plot/plot_frame.py
 src/pymonke/latex/__init__.py
 src/pymonke/latex/tex_table.py
-src/pymonke/latex/tex_tabular.py
-src/pymonke/latex/tex_tabular.pyi
 src/pymonke/latex/utils.py
 src/pymonke/latex/utils.pyi
 src/pymonke/latex/tests/__init__.py
 src/pymonke/latex/tests/table_test.py
 src/pymonke/misc/__init__.py
+src/pymonke/misc/benchmark.py
 src/pymonke/misc/dataframe.py
 src/pymonke/misc/file_management.py
+src/pymonke/misc/pymonke_json_decoder.py
+src/pymonke/misc/pymonke_json_encoder.py
 src/pymonke/mmath/__init__.py
-src/pymonke/mmath/num_with_error.py
 src/pymonke/mmath/rounding.py
 src/pymonke/mmath/statistics.py
-src/pymonke/mmath/tests/__init__.py
-src/pymonke/mmath/tests/num_with_error_test.py
-src/pymonke/mmath/tests/rounding_test.py
 tests/test.py
```

