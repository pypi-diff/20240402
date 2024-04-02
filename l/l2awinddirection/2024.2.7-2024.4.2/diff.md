# Comparing `tmp/l2awinddirection-2024.2.7.tar.gz` & `tmp/l2awinddirection-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2awinddirection-2024.2.7.tar", last modified: Wed Feb  7 09:58:52 2024, max compression
+gzip compressed data, was "l2awinddirection-2024.4.2.tar", last modified: Tue Apr  2 15:15:10 2024, max compression
```

## Comparing `l2awinddirection-2024.2.7.tar` & `l2awinddirection-2024.4.2.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:58:52.645774 l2awinddirection-2024.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:58:52.641774 l2awinddirection-2024.2.7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:58:52.641774 l2awinddirection-2024.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-07 09:58:52.645774 l2awinddirection-2024.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:58:52.641774 l2awinddirection-2024.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4907 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:58:52.645774 l2awinddirection-2024.2.7/l2awinddirection/
--rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/l2awinddirection/M64RN4.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/l2awinddirection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/l2awinddirection/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/l2awinddirection/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/l2awinddirection/generate_L2A_winddir_pdf_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/l2awinddirection/generate_L2A_winddir_regression_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     9810 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/l2awinddirection/l2awinddirection.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/l2awinddirection/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:58:52.645774 l2awinddirection-2024.2.7/l2awinddirection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-07 09:58:52.000000 l2awinddirection-2024.2.7/l2awinddirection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-07 09:58:52.000000 l2awinddirection-2024.2.7/l2awinddirection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 09:58:52.000000 l2awinddirection-2024.2.7/l2awinddirection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-07 09:58:52.000000 l2awinddirection-2024.2.7/l2awinddirection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-07 09:58:52.000000 l2awinddirection-2024.2.7/l2awinddirection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-07 09:58:52.000000 l2awinddirection-2024.2.7/l2awinddirection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-07 09:58:52.645774 l2awinddirection-2024.2.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 09:58:52.645774 l2awinddirection-2024.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-07 09:58:37.000000 l2awinddirection-2024.2.7/tests/test_l2awinddirection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:10.426736 l2awinddirection-2024.4.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:10.418736 l2awinddirection-2024.4.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:10.418736 l2awinddirection-2024.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-02 15:15:10.426736 l2awinddirection-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:10.422736 l2awinddirection-2024.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4907 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:10.422736 l2awinddirection-2024.4.2/l2awinddirection/
+-rw-r--r--   0 runner    (1001) docker     (127)     9760 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/l2awinddirection/M64RN4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/l2awinddirection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/l2awinddirection/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/l2awinddirection/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/l2awinddirection/generate_L2A_winddir_pdf_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/l2awinddirection/generate_L2A_winddir_regression_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/l2awinddirection/mainl2awinddirection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/l2awinddirection/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:10.422736 l2awinddirection-2024.4.2/l2awinddirection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-02 15:15:10.000000 l2awinddirection-2024.4.2/l2awinddirection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-02 15:15:10.000000 l2awinddirection-2024.4.2/l2awinddirection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:15:10.000000 l2awinddirection-2024.4.2/l2awinddirection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 15:15:10.000000 l2awinddirection-2024.4.2/l2awinddirection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 15:15:10.000000 l2awinddirection-2024.4.2/l2awinddirection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 15:15:10.000000 l2awinddirection-2024.4.2/l2awinddirection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:15:10.426736 l2awinddirection-2024.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:15:10.422736 l2awinddirection-2024.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/tests/test_l2awinddirection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-02 15:14:56.000000 l2awinddirection-2024.4.2/tests/test_output_name.py
```

### Comparing `l2awinddirection-2024.2.7/.github/workflows/publish.yml` & `l2awinddirection-2024.4.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `l2awinddirection-2024.2.7/.gitignore` & `l2awinddirection-2024.4.2/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -123,7 +123,9 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+localconfig.yaml
```

### Comparing `l2awinddirection-2024.2.7/CONTRIBUTING.rst` & `l2awinddirection-2024.4.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `l2awinddirection-2024.2.7/LICENSE` & `l2awinddirection-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `l2awinddirection-2024.2.7/Makefile` & `l2awinddirection-2024.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `l2awinddirection-2024.2.7/PKG-INFO` & `l2awinddirection-2024.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l2awinddirection
-Version: 2024.2.7
+Version: 2024.4.2
 Summary: Python library to generate Level-2A wind direction files
 Author: Robin Marquart, Antoine Grouazel
 License: MIT
 Keywords: SAR,wind,reseach,neural-network,texture,tensorflow
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `l2awinddirection-2024.2.7/README.rst` & `l2awinddirection-2024.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `l2awinddirection-2024.2.7/docs/Makefile` & `l2awinddirection-2024.4.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `l2awinddirection-2024.2.7/docs/conf.py` & `l2awinddirection-2024.4.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 release = l2awinddirection.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `l2awinddirection-2024.2.7/docs/installation.rst` & `l2awinddirection-2024.4.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `l2awinddirection-2024.2.7/docs/make.bat` & `l2awinddirection-2024.4.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `l2awinddirection-2024.2.7/l2awinddirection/M64RN4.py` & `l2awinddirection-2024.4.2/l2awinddirection/M64RN4.py`

 * *Files identical despite different names*

### Comparing `l2awinddirection-2024.2.7/l2awinddirection/generate_L2A_winddir_pdf_product.py` & `l2awinddirection-2024.4.2/l2awinddirection/generate_L2A_winddir_pdf_product.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,109 +34,118 @@
     Returns:
         xarray.Dataset: dataset containing the tiles with associated wind direction.
     """
     try:
         tiles_stacked = tiles.stack(all_tiles=["burst", "tile_line", "tile_sample"])
     except:
         tiles_stacked = tiles.stack(all_tiles=["tile_line", "tile_sample"])
-    tiles_stacked_no_nan = tiles_stacked.where(
-        ~np.any(np.isnan(tiles_stacked.sigma0), axis=(0, 1)), drop=True
-    )
-    X = tiles_stacked_no_nan.sigma0.transpose("all_tiles", "azimuth", "range").values
+    # mask0 = ~np.any(
+    #     np.isnan(tiles_stacked.sigma0), axis=(0, 1)
+    # )  # original mask from Robin, sigma0 never contains NaN contrarily to sigma0_filt
+    mask = tiles_stacked.land_flag == False  # test AG
+    mask_indices = np.where(mask)
+    tiles_stacked_no_nan = tiles_stacked.where(mask, drop=True)
+
+    if "sigma0_filt" in tiles_stacked:
+        X = tiles_stacked_no_nan.sigma0_filt.transpose(
+            "all_tiles", "azimuth", "range"
+        ).values
+    else:
+        X = tiles_stacked_no_nan.sigma0.transpose(
+            "all_tiles", "azimuth", "range"
+        ).values
+
     X_normalized = np.array(
         [((x - np.average(x)) / np.std(x)).reshape(shape) for x in X]
     )  # Normalize data
 
-    heading_angle = np.deg2rad(tiles_stacked_no_nan["ground_heading"].values)
-
+    heading_angle = np.deg2rad(tiles_stacked["ground_heading"].values)
     # Assign new coordinates 'bin_centers' to the dataset
     dx = 180 / nb_classes
     angles = np.arange(0 + dx / 2, 180 + dx / 2, dx)
-
+    predictions = np.ones((tiles_stacked.longitude.size, angles.size)) * np.nan
     tiles_stacked_no_nan = tiles_stacked_no_nan.assign_coords(
         bin_centers=("bin_centers", angles)
     )
 
     # Predict wind direction distributions and add them to the dataset
     # predictions = np.squeeze(m64rn4.model.predict(X_normalized)) # original Robin
-    predictions = m64rn4.model.predict(X_normalized)
-    tiles_stacked_no_nan = tiles_stacked_no_nan.assign(
+    if X_normalized.size > 0:
+        predictions_usable = m64rn4.model.predict(X_normalized)
+        predictions[mask_indices, :] = predictions_usable
+
+    tiles_stacked = tiles_stacked.assign(
         wind_direction_distribution=(["all_tiles", "bin_centers"], predictions)
     )
 
     # Compute mean wind direction, most likely wind direction and associated standard deviation
     mean_wdir = xr.apply_ufunc(
         compute_mean_direction,
-        tiles_stacked_no_nan.wind_direction_distribution,
-        tiles_stacked_no_nan.bin_centers,
+        tiles_stacked.wind_direction_distribution,
+        tiles_stacked.bin_centers,
         input_core_dims=[["bin_centers"], ["bin_centers"]],
         vectorize=True,
     )
-
+    mean_wdir = mean_wdir + heading_angle
     most_likely_wdir = xr.apply_ufunc(
         compute_most_likely_direction,
-        tiles_stacked_no_nan.wind_direction_distribution,
-        tiles_stacked_no_nan.bin_centers,
+        tiles_stacked.wind_direction_distribution,
+        tiles_stacked.bin_centers,
         input_core_dims=[["bin_centers"], ["bin_centers"]],
         vectorize=True,
     )
-
+    most_likely_wdir = xr.where(tiles_stacked['land_flag'],np.nan,most_likely_wdir) # apply the land_mask on the wdin direction prediction
+    most_likely_wdir = most_likely_wdir + heading_angle
     std_wdir = xr.apply_ufunc(
         compute_standard_deviation,
-        tiles_stacked_no_nan.wind_direction_distribution,
-        tiles_stacked_no_nan.bin_centers,
+        tiles_stacked.wind_direction_distribution,
+        tiles_stacked.bin_centers,
         input_core_dims=[["bin_centers"], ["bin_centers"]],
         vectorize=True,
     )
 
     # Format dataset
-    tiles_stacked_no_nan = tiles_stacked_no_nan.assign(
-        mean_wdir=(["all_tiles"], mean_wdir.data)
-    )
-    tiles_stacked_no_nan["mean_wdir"].attrs[
+    tiles_stacked = tiles_stacked.assign(mean_wdir=(["all_tiles"], mean_wdir.data))
+    tiles_stacked["mean_wdir"].attrs[
         "definition"
     ] = "180° ambiguous mean wind direction."
-    tiles_stacked_no_nan["mean_wdir"].attrs["long_name"] = "Mean wind direction"
-    tiles_stacked_no_nan["mean_wdir"].attrs[
+    tiles_stacked["mean_wdir"].attrs["long_name"] = "Mean wind direction"
+    tiles_stacked["mean_wdir"].attrs[
         "convention"
     ] = "Clockwise, relative to geographic North."
-    tiles_stacked_no_nan["mean_wdir"].attrs["units"] = "degree"
-    tiles_stacked_no_nan["mean_wdir"].attrs["vmin"] = 0
-    tiles_stacked_no_nan["mean_wdir"].attrs["vmax"] = 180
+    tiles_stacked["mean_wdir"].attrs["units"] = "degree"
+    tiles_stacked["mean_wdir"].attrs["vmin"] = 0
+    tiles_stacked["mean_wdir"].attrs["vmax"] = 180
 
-    tiles_stacked_no_nan = tiles_stacked_no_nan.assign(
+    tiles_stacked = tiles_stacked.assign(
         most_likely_wdir=(["all_tiles"], most_likely_wdir.data)
     )
-    tiles_stacked_no_nan["most_likely_wdir"].attrs[
+    tiles_stacked["most_likely_wdir"].attrs[
         "definition"
     ] = "180° ambiguous most likely wind direction, defined with a bin precision of 2.5°."
-    tiles_stacked_no_nan["most_likely_wdir"].attrs[
-        "long_name"
-    ] = "Most likely wind direction"
-    tiles_stacked_no_nan["most_likely_wdir"].attrs[
+    tiles_stacked["most_likely_wdir"].attrs["long_name"] = "Most likely wind direction"
+    tiles_stacked["most_likely_wdir"].attrs[
         "convention"
     ] = "Clockwise, relative to geographic North."
-    tiles_stacked_no_nan["most_likely_wdir"].attrs["units"] = "degree"
-    tiles_stacked_no_nan["most_likely_wdir"].attrs["vmin"] = 0
-    tiles_stacked_no_nan["most_likely_wdir"].attrs["vmax"] = 180
+    tiles_stacked["most_likely_wdir"].attrs["units"] = "degree"
+    tiles_stacked["most_likely_wdir"].attrs["vmin"] = 0
+    tiles_stacked["most_likely_wdir"].attrs["vmax"] = 180
 
-    tiles_stacked_no_nan = tiles_stacked_no_nan.assign(
-        std_wdir=(["all_tiles"], std_wdir.data)
-    )
-    tiles_stacked_no_nan["std_wdir"].attrs[
+    tiles_stacked = tiles_stacked.assign(std_wdir=(["all_tiles"], std_wdir.data))
+    tiles_stacked["std_wdir"].attrs[
         "definition"
     ] = "Standard deviation associated with wind direction."
-    tiles_stacked_no_nan["std_wdir"].attrs[
+    tiles_stacked["std_wdir"].attrs[
         "long_name"
     ] = "Standard deviation of the wind direction"
-    tiles_stacked_no_nan["std_wdir"].attrs["units"] = "degree"
-    tiles_stacked_no_nan["std_wdir"].attrs["vmin"] = 0
-    tiles_stacked_no_nan["std_wdir"].attrs["vmax"] = 180
+    tiles_stacked["std_wdir"].attrs["units"] = "degree"
+    tiles_stacked["std_wdir"].attrs["vmin"] = 0
+    tiles_stacked["std_wdir"].attrs["vmax"] = 180
 
-    return tiles_stacked_no_nan.unstack()
+    return tiles_stacked.unstack()
 
 
 def compute_mean_direction(weights, angles):
     """
     Compute mean direction given an array of weights and angles taking into account the circularity between 0 and 180° of the angles.
     Parameters:
         weights (numpy.ndarray): probability corresponding to each angle.
```

### Comparing `l2awinddirection-2024.2.7/l2awinddirection/generate_L2A_winddir_regression_product.py` & `l2awinddirection-2024.4.2/l2awinddirection/generate_L2A_winddir_regression_product.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,97 @@
 """
 inspired from predict_wind_direction.py (project_rmarquart)
 January 2024
 """
+import pdb
 import numpy as np
 import scipy as sp
-import xarray as xr
 from scipy import stats
-import glob
-import os, sys
-from tqdm import tqdm
-from l2awinddirection.M64RN4 import M64RN4_regression
+
 
 # --------------------- #
 # ----- Functions ----- #
 # --------------------- #
 
-def generate_wind_product(tiles, model_regs, shape = (44, 44, 1)):
+
+def generate_wind_product(tiles, model_regs, shape=(44, 44, 1)):
     """
     Generate wind direction from previously extracted tiles and store them in an xarray.Dataset.
     Parameters:
         tiles (xarray.Dataset): L1b path of the file to process.
         model_regs (list of M64RN4): list of the M64RN4 models used for prediction.
         shape (tuple of int): shape of the inputs of the M64RN4 models.
     Returns:
         (xarray.Dataset): dataset containing the tiles with associated wind direction.
     """
-    tiles_stacked = tiles.stack(all_tiles = ['burst', 'tile_line','tile_sample'])
-    tiles_stacked_no_nan = tiles_stacked.where(~np.any(np.isnan(tiles_stacked.sigma0), axis = (0, 1)), drop = True)
-    X = tiles_stacked_no_nan.sigma0.transpose('all_tiles', 'azimuth', 'range').values
-    X_normalized = np.array([((x - np.average(x))/np.std(x)).reshape(shape) for x in X]) # Normalize data
-    
-    heading_angle = np.deg2rad(tiles_stacked_no_nan['ground_heading'].values) 
-    
-    #Predict wind directions using all models and obtain mean and std values
-    predictions = launch_prediction(X_normalized, model_regs)
-    mean_prediction = sp.stats.circmean(predictions, np.pi, axis = 1)
-    std_prediction = sp.stats.circstd(predictions, np.pi, axis = 1)
-    
+    try:
+        tiles_stacked = tiles.stack(all_tiles=["burst", "tile_line", "tile_sample"])
+    except:
+        tiles_stacked = tiles.stack(all_tiles=["tile_line", "tile_sample"])
+
+    mask = tiles_stacked.land_flag == False
+    mask_indices = np.where(mask)
+    tiles_stacked_no_nan = tiles_stacked.where(mask, drop=True)
+
+    if "sigma0_filt" in tiles_stacked:
+        X = tiles_stacked_no_nan.sigma0_filt.transpose(
+            "all_tiles", "azimuth", "range"
+        ).values
+    else:
+        X = tiles_stacked_no_nan.sigma0.transpose(
+            "all_tiles", "azimuth", "range"
+        ).values
+
+    X_normalized = np.array(
+        [((x - np.average(x)) / np.std(x)).reshape(shape) for x in X]
+    )  # Normalize data
+
+    heading_angle = np.deg2rad(tiles_stacked["ground_heading"].values)
+    predictions = np.ones((tiles_stacked.longitude.size,len(model_regs))) * np.NaN
+    # Predict wind directions using all models and obtain mean and std values
+    if X_normalized.size > 0:
+        predictions_usable = launch_prediction(X_normalized, model_regs)
+        predictions[mask_indices,:] = predictions_usable
+
+    mean_prediction = sp.stats.circmean(predictions, np.pi, axis=1)
+    std_prediction = sp.stats.circstd(predictions, np.pi, axis=1)
+
     predicted_wdir = mean_prediction + heading_angle
-    
+
     # Format dataset
-    tiles_stacked_no_nan = tiles_stacked_no_nan.assign(wind_direction = (['all_tiles'],  np.rad2deg(predicted_wdir)%180))
-    tiles_stacked_no_nan['wind_direction'].attrs['definition'] = '180° ambiguous wind direction, clockwise, relative to geographic North.'
-    tiles_stacked_no_nan['wind_direction'].attrs['units'] = 'degree'
-    tiles_stacked_no_nan['wind_direction'].attrs['vmin'] = 0
-    tiles_stacked_no_nan['wind_direction'].attrs['vmax'] = 180
-    
-    tiles_stacked_no_nan = tiles_stacked_no_nan.assign(wind_std = (['all_tiles'],  np.rad2deg(std_prediction)%180))
-    tiles_stacked_no_nan['wind_std'].attrs['definition'] = 'Standard deviation associated with wind direction. Calculated by computing the spread accross the '
-    tiles_stacked_no_nan['wind_std'].attrs['units'] = 'degree'
-    tiles_stacked_no_nan['wind_std'].attrs['vmin'] = 0
-    tiles_stacked_no_nan['wind_std'].attrs['vmax'] = 180
+    tiles_stacked = tiles_stacked.assign(
+        wind_direction=(["all_tiles"], np.rad2deg(predicted_wdir) % 180)
+    )
+    tiles_stacked["wind_direction"].attrs[
+        "definition"
+    ] = "180° ambiguous wind direction, clockwise, relative to geographic North."
+    tiles_stacked["wind_direction"].attrs["units"] = "degree"
+    tiles_stacked["wind_direction"].attrs["vmin"] = 0
+    tiles_stacked["wind_direction"].attrs["vmax"] = 180
+
+    tiles_stacked = tiles_stacked.assign(
+        wind_std=(["all_tiles"], np.rad2deg(std_prediction) % 180)
+    )
+    tiles_stacked["wind_std"].attrs[
+        "definition"
+    ] = "Standard deviation associated with wind direction. Calculated by computing the spread accross the "
+    tiles_stacked["wind_std"].attrs["units"] = "degree"
+    tiles_stacked["wind_std"].attrs["vmin"] = 0
+    tiles_stacked["wind_std"].attrs["vmax"] = 180
+    return tiles_stacked.unstack()
 
-    return tiles_stacked_no_nan.unstack()
-    
 
 def launch_prediction(X_normalized, model_regs):
     """
     Predicts wind direction of the given vector.
     Parameters:
         X_normalized (numpy.array): normalized array used for prediction.
         model_regs (list of M64RN4): list of the M64RN4 models used for prediction.
     Returns:
         predictions (numpy.array): array of predictions.
     """
     predictions = np.zeros((X_normalized.shape[0], len(model_regs)))
 
     for i, m64rn4 in enumerate(model_regs):
         predictions[:, i] = np.squeeze(m64rn4.model.predict(X_normalized))
-        
-    return predictions
-
-
-if __name__ == "__main__":
-
-    #Parameters to instantiante the models
-    input_shape = (44, 44, 1)
-    data_augmentation = True
-    learning_rate = 1e-3
 
-    model_regs = []
-
-    #Modify path_best_models depending of the acquisition mode (iw, ew, wv)
-    path_best_models = glob.glob('.../analysis/s1_data_analysis/project_rmarquar/wsat/trained_models/iw/*.hdf5')
-    for path in path_best_models:
-
-        m64rn4_reg = M64RN4_regression(input_shape, data_augmentation)
-        m64rn4_reg.create_and_compile(learning_rate)
-
-        m64rn4_reg.model.load_weights(path)
-
-        model_regs.append(m64rn4_reg)
-
-
-    #Get listing of files from which to generate the wind direction
-    files = glob.glob('.../analysis/s1_data_analysis/project_rmarquar/slc_wind_product/1.4k/*/tiles*1.4k.nc')
-    print("Number of files to process: %d" % len(files))
-
-    for file in tqdm(files):
-        tiles = xr.open_dataset(file)
-        if len(tiles.variables.keys()) == 0:
-            continue
-        res = generate_wind_product(tiles, model_regs)
-        res.to_netcdf(file.replace('.nc', '_wind.nc'))
-        # if you want to remove the file containing the tiles used for inference (data kept in final product)
-        del tiles
-        os.remove(file)
+    return predictions
```

### Comparing `l2awinddirection-2024.2.7/l2awinddirection/l2awinddirection.py` & `l2awinddirection-2024.4.2/l2awinddirection/mainl2awinddirection.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,55 +2,39 @@
 Step 1: move tiles nc files in a local directory for GPU processing (currently prediction is not working from another volume)
 Step 2: do the prediction -> generate a .nc file containing the wind direction
 Step 3: move the generated file to the archive storage
 
 """
 import glob
 import os
+os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 import pdb
 import shutil
 import xarray as xr
 from tqdm import tqdm
 import logging
 import time
 import numpy as np
-import warnings
-
-warnings.filterwarnings("ignore")
-# logging.getLogger("tensorflow").setLevel(logging.FATAL)
-import tensorflow as tf
-
-tf.get_logger().setLevel("ERROR")
-logging.getLogger("tensorflow").setLevel(logging.ERROR)
-# tf.debugging.set_log_device_placement(True)
-# logging.getLogger("tensorflow").setLevel(logging.WARNING)
-# tf.logging.set_verbosity(tf.logging.ERROR)
-# tf.keras.utils.disable_interactive_logging()
-# import keras
-# from keras.backend.tensorflow_backend import tf
-
-# tf.keras.utils.disable_interactive_logging()
-# import absl.logging
-# logging.root.removeHandler(absl.logging._absl_handler)
-# absl.logging._warn_preinit_stderr = False
-
-# logger = tf.get_logger()
-# logger.setLevel(logging.FATAL)
 
 import l2awinddirection
+
+try:
+    print(l2awinddirection.__version__)
+    print(l2awinddirection.__file__)
+except:
+    pass
 from l2awinddirection.generate_L2A_winddir_pdf_product import (
     generate_wind_distribution_product,
 )
 from l2awinddirection.generate_L2A_winddir_regression_product import (
     generate_wind_product,
 )
-from l2awinddirection.utils import get_conf
+from l2awinddirection.utils import get_conf,get_l2_filepath
 from l2awinddirection.M64RN4 import M64RN4_distribution, M64RN4_regression
 
-os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"  # disable logging tensorflow
 conf = get_conf()
 
 
 def get_memory_usage():
     try:
         import resource
 
@@ -88,15 +72,15 @@
         help="must must choose a NN model or regression or pdf",
     )
     parser.add_argument(
         "--l2awindirtilessafe",
         required=True,
         help="Level-2A wind direction SAFE where are stored the extracted DN tiles",
     )
-    # for now the output files will be in the same directory than the input SAFE
+    # for now the output files will be in the same directory as the input SAFE
     parser.add_argument(
         "--outputdir",
         required=True,
         help="directory where to move and store output netCDF files",
     )
     parser.add_argument(
         "--workspace",
@@ -111,24 +95,29 @@
     parser.add_argument(
         "--modelregression",
         help="specify the path of the NN model to predict float (regression) result [default is localconfig.yml or config.yml]",
         required=False,
     )
     parser.add_argument(
         "--skipmoves",
-        help="skip copy of the tiles in a workspace and move of the L2A winddir files from workspace to outputdir [default=False]",
+        help="True-> skip copy of the tiles in a workspace and move of the L2A winddir files from workspace to outputdir [default=False -> a workspace is used]",
         action="store_true",
         default=False,
     )
     parser.add_argument(
+        "--version",
+        help="product ID of the level-2 wdr to be generated (eg: D03)",
+        required=True,
+    )
+    parser.add_argument(
         "--remove-tiles",
-        help="remove the tiles files in the workspace directory [default=True]",
+        help="remove the tiles files in the workspace directory [default=False -> tiles kept in workspace]",
         required=False,
-        default=True,
-        action="store_false",
+        default=False,
+        action="store_true",
     )
     args = parser.parse_args()
     fmt = "%(asctime)s %(levelname)s %(filename)s(%(lineno)d) %(message)s"
     if args.verbose:
         logging.basicConfig(
             level=logging.DEBUG, format=fmt, datefmt="%d/%m/%Y %H:%M:%S", force=True
         )
@@ -156,55 +145,56 @@
         n_classes = 36
         model_m64rn4 = M64RN4_distribution(input_shape, data_augmentation, n_classes)
         model_m64rn4.create_and_compile(learning_rate)
 
         model_m64rn4.model.load_weights(path_model_pdf)
     elif args.mode == "regression":
         model_m64rn4 = []
-        # path_best_models = glob.glob(
-        #     ".../analysis/s1_data_analysis/project_rmarquar/wsat/trained_models/iw/*.hdf5"
-        # )
         path_best_models = glob.glob(os.path.join(dirmodelsreg, "*.hdf5"))
         assert len(path_best_models) > 1
         for path in path_best_models:
 
             m64rn4_reg = M64RN4_regression(input_shape, data_augmentation)
             m64rn4_reg.create_and_compile(learning_rate)
 
             m64rn4_reg.model.load_weights(path)
 
             model_m64rn4.append(m64rn4_reg)
     else:
         raise Exception("not handled case")
-    # files = glob.glob("/raid/localscratch/agrouaze/tiles_iw_4_wdir/3.1/*SAFE/*.nc")
+
     if args.l2awindirtilessafe.endswith("/"):
 
         l2awindirtilessafe = args.l2awindirtilessafe.rstrip("/")
     else:
         l2awindirtilessafe = args.l2awindirtilessafe
     if args.skipmoves:
-        workspace = os.path.dirname(l2awindirtilessafe)
+        workspace_input = os.path.dirname(l2awindirtilessafe)
         logging.info(
             "workspace is the place where the tiles are already stored: %s (no copies)",
-            workspace,
+            workspace_input,
         )
+        workspace_output = args.outputdir
     else:
         if args.workspace is None:
-            workspace = conf["workspace_prediction"]
+            workspace_input = conf["workspace_prediction"]
         else:
-            workspace = args.workspace
+            workspace_input = args.workspace
         logging.info(
             "workspace where the tiles will be temporarily moved is: %s",
-            workspace,
+            workspace_input,
         )
-    safefile = os.path.join(workspace, os.path.basename(l2awindirtilessafe))
-    if not os.path.exists(safefile) and args.skipmoves is True:
-        logging.info(" step 1: move %s -> %s", l2awindirtilessafe, safefile)
-        shutil.copytree(l2awindirtilessafe, safefile)
-    files = glob.glob(os.path.join(safefile, "*.nc"))
+        workspace_output = workspace_input
+    input_safe_full_path = os.path.join(workspace_input, os.path.basename(l2awindirtilessafe))
+    if not os.path.exists(input_safe_full_path) and args.skipmoves is True:
+        logging.info(" step 1: move %s -> %s", l2awindirtilessafe, input_safe_full_path)
+        shutil.copytree(l2awindirtilessafe, input_safe_full_path)
+    files = sorted(
+        glob.glob(os.path.join(input_safe_full_path, "*.nc")) # all polarisation accepted for prediction
+    )
     logging.info("Number of files to process: %d" % len(files))
     if not os.path.exists(args.outputdir):
         logging.info("mkdir %s", args.outputdir)
         os.makedirs(args.outputdir)
 
     logging.info("step 2: predictions")
     for ii in tqdm(range(len(files))):
@@ -214,45 +204,50 @@
         if len(tiles.variables.keys()) == 0:
             logging.info("no data in %s", file)
             continue
         if args.mode == "pdf":
             res = generate_wind_distribution_product(
                 tiles, model_m64rn4, nb_classes=36, shape=(44, 44, 1)
             )
-            outputfile = file.replace(
-                "_wind.nc", "_winddirection_pdf.nc"
-            )  # TODO: change to _tiles.nc -> _winddirection.nc
+            outputfile = get_l2_filepath(vignette_fullpath=file, version=args.version, outputdir=workspace_output)
             if args.skipmoves:
-                outputfile = outputfile.replace(workspace, args.outputdir)
+                # outputfile = outputfile.replace(workspace_output, args.outputdir)
                 if not os.path.exists(os.path.dirname(outputfile)):
                     os.makedirs(os.path.dirname(outputfile))
-            res.attrs["winddirection_L2A_processor"] = "l2awinddirection"
-            res.attrs["winddirection_L2A_processor_version"] = l2awinddirection.__version__
-            res.to_netcdf(outputfile)
         elif args.mode == "regression":
-
-            outputfile = file.replace(
-                "_wind.nc", "_winddirection_regression.nc"
-            )  # TODO: change to _tiles.nc -> _winddirection.nc
+            outputfile = get_l2_filepath(vignette_fullpath=file, version=args.version, outputdir=workspace_output)
             if args.skipmoves:
-                outputfile = outputfile.replace(workspace, args.outputdir)
+                # outputfile = outputfile.replace(workspace_output, args.outputdir)
                 if not os.path.exists(os.path.dirname(outputfile)):
                     os.makedirs(os.path.dirname(outputfile))
 
             res = generate_wind_product(tiles, model_m64rn4)
-            res.attrs["winddirection_L2A_processor"] = "l2awinddirection"
-            res.attrs["winddirection_L2A_processor_version"] = l2awinddirection.__version__
-            res.to_netcdf(outputfile)
+        res.attrs["winddirection_L2A_processor"] = "l2awinddirection"
+        res.attrs["winddirection_L2A_processor_version"] = l2awinddirection.__version__
+        if 'pol' in res.coords:
+            res.attrs["used_channel"] = res.coords["pol"].values
+        else:
+            res.attrs['used_channel'] = res['selected_pol'].values
+            # res.attrs["used_channel"] =
+        res.attrs["winddirection_L2A_processor_mode"] = args.mode
+        if 'pol' in res.coords:
+            res = res.drop('pol')
+        res.to_netcdf(outputfile)
 
         # if you want to remove the file containing the tiles used for inference (data kept in final product)
         del tiles
         if args.remove_tiles and args.skipmoves is False:
             logging.info("remove temporary tiles file in the workspace: %s", file)
             os.remove(file)
-    final_safe_path = os.path.join(args.outputdir, os.path.basename(l2awindirtilessafe))
-    if args.skipmoves is False:
-        logging.info("step 3: move %s -> %s", safefile, final_safe_path)
-        shutil.move(safefile, final_safe_path)
+
+    # final_safe_path = os.path.dirname(outputfile)
+    if args.skipmoves is False: # case for which a workspace has been used
+        # final_safe_path = os.path.join(args.outputdir, os.path.basename(l2awindirtilessafe))
+        final_safe_path = os.path.dirname(outputfile).replace(workspace_output,args.outputdir)
+        logging.info("step 3: move %s -> %s", os.path.dirname(outputfile), final_safe_path)
+        shutil.move(os.path.dirname(outputfile), final_safe_path)
+    else:
+        final_safe_path = os.path.dirname(outputfile)
     logging.info("Ifremer Level-2A wind direction SAFE path: %s", final_safe_path)
     logging.info("successful SAFE processing")
     logging.info("peak memory usage: %s ", get_memory_usage())
     logging.info("done in %1.3f min", (time.time() - t0) / 60.0)
```

### Comparing `l2awinddirection-2024.2.7/l2awinddirection.egg-info/PKG-INFO` & `l2awinddirection-2024.4.2/l2awinddirection.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l2awinddirection
-Version: 2024.2.7
+Version: 2024.4.2
 Summary: Python library to generate Level-2A wind direction files
 Author: Robin Marquart, Antoine Grouazel
 License: MIT
 Keywords: SAR,wind,reseach,neural-network,texture,tensorflow
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `l2awinddirection-2024.2.7/l2awinddirection.egg-info/SOURCES.txt` & `l2awinddirection-2024.4.2/l2awinddirection.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
+docs/modules.rst
 docs/readme.rst
 docs/usage.rst
 l2awinddirection/M64RN4.py
 l2awinddirection/__init__.py
 l2awinddirection/cli.py
 l2awinddirection/config.yaml
 l2awinddirection/generate_L2A_winddir_pdf_product.py
 l2awinddirection/generate_L2A_winddir_regression_product.py
-l2awinddirection/l2awinddirection.py
+l2awinddirection/mainl2awinddirection.py
 l2awinddirection/utils.py
 l2awinddirection.egg-info/PKG-INFO
 l2awinddirection.egg-info/SOURCES.txt
 l2awinddirection.egg-info/dependency_links.txt
 l2awinddirection.egg-info/entry_points.txt
 l2awinddirection.egg-info/requires.txt
 l2awinddirection.egg-info/top_level.txt
 tests/__init__.py
-tests/test_l2awinddirection.py
+tests/test_l2awinddirection.py
+tests/test_output_name.py
```

### Comparing `l2awinddirection-2024.2.7/pyproject.toml` & `l2awinddirection-2024.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 profile = "black"
 skip_gitignore = true
 float_to_top = true
 default_section = "THIRDPARTY"
 known_first_party = "l2awinddirection"
 
 [project.scripts]
-L2a-wind-dir-processor = "l2awinddirection.l2awinddirection:main"
+L2a-wind-dir-processor = "l2awinddirection.mainl2awinddirection:main"
```

### Comparing `l2awinddirection-2024.2.7/tests/test_l2awinddirection.py` & `l2awinddirection-2024.4.2/tests/test_l2awinddirection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """Tests for `l2awinddirection` package."""
 
 import pytest
 
 
-from l2awinddirection import l2awinddirection
+from l2awinddirection import mainl2awinddirection
 
 
 @pytest.fixture
 def response():
     """Sample pytest fixture.
 
     See more at: http://doc.pytest.org/en/latest/fixture.html
```

