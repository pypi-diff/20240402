# Comparing `tmp/rio_cogeo-5.2.0.tar.gz` & `tmp/rio_cogeo-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio_cogeo-5.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "rio_cogeo-5.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rio_cogeo-5.2.0.tar` & `rio_cogeo-5.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      213 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1249 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/.gitignore
--rw-r--r--   0        0        0      799 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1517 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/LICENSE
--rw-r--r--   0        0        0     3373 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/README.md
--rw-r--r--   0        0        0     2329 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/pyproject.toml
--rw-r--r--   0        0        0      218 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/rio_cogeo/__init__.py
--rw-r--r--   0        0        0    31808 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/rio_cogeo/cogeo.py
--rw-r--r--   0        0        0      406 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/rio_cogeo/errors.py
--rw-r--r--   0        0        0     2017 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/rio_cogeo/models.py
--rw-r--r--   0        0        0     4521 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/rio_cogeo/profiles.py
--rw-r--r--   0        0        0       21 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/rio_cogeo/scripts/__init__.py
--rw-r--r--   0        0        0    14647 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/rio_cogeo/scripts/cli.py
--rw-r--r--   0        0        0     4607 2024-02-16 14:06:26.978831 rio_cogeo-5.2.0/rio_cogeo/utils.py
--rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 rio_cogeo-5.2.0/PKG-INFO
+-rw-r--r--   0        0        0      213 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1249 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/.gitignore
+-rw-r--r--   0        0        0      799 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1517 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/LICENSE
+-rw-r--r--   0        0        0     3373 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/README.md
+-rw-r--r--   0        0        0     2329 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0      218 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/rio_cogeo/__init__.py
+-rw-r--r--   0        0        0    32419 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/rio_cogeo/cogeo.py
+-rw-r--r--   0        0        0      406 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/rio_cogeo/errors.py
+-rw-r--r--   0        0        0     2017 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/rio_cogeo/models.py
+-rw-r--r--   0        0        0     4521 2024-04-02 11:36:15.351074 rio_cogeo-5.3.0/rio_cogeo/profiles.py
+-rw-r--r--   0        0        0       21 2024-04-02 11:36:15.355074 rio_cogeo-5.3.0/rio_cogeo/scripts/__init__.py
+-rw-r--r--   0        0        0    14940 2024-04-02 11:36:15.355074 rio_cogeo-5.3.0/rio_cogeo/scripts/cli.py
+-rw-r--r--   0        0        0     4607 2024-04-02 11:36:15.355074 rio_cogeo-5.3.0/rio_cogeo/utils.py
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 rio_cogeo-5.3.0/PKG-INFO
```

### Comparing `rio_cogeo-5.2.0/.gitignore` & `rio_cogeo-5.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rio_cogeo-5.2.0/.pre-commit-config.yaml` & `rio_cogeo-5.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rio_cogeo-5.2.0/LICENSE` & `rio_cogeo-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rio_cogeo-5.2.0/README.md` & `rio_cogeo-5.3.0/README.md`

 * *Files identical despite different names*

### Comparing `rio_cogeo-5.2.0/pyproject.toml` & `rio_cogeo-5.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rio_cogeo-5.2.0/rio_cogeo/cogeo.py` & `rio_cogeo-5.3.0/rio_cogeo/cogeo.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     forward_ns_tags: bool = False,
     quiet: bool = False,
     progress_out: Optional[TextIO] = None,
     temporary_compression: str = "DEFLATE",
     colormap: Optional[Dict] = None,
     additional_cog_metadata: Optional[Dict] = None,
     use_cog_driver: bool = False,
+    decimation_base: int = 2,
 ):
     """
     Create Cloud Optimized Geotiff.
 
     Parameters
     ----------
     source : str, PathLike object or rasterio.io.DatasetReader
@@ -167,14 +168,18 @@
         Compression used for the intermediate file, default is deflate.
     colormap: dict, optional
         Overwrite or add a colormap to the output COG.
     additional_cog_metadata: dict, optional
         Additional dataset metadata to add to the COG.
     use_cog_driver: bool, optional (default: False)
         Use GDAL COG driver if set to True. COG driver is available starting with GDAL 3.1.
+    decimation_base: int, default: 2
+        How overviews are divided at each zoom level (default is 2). Must be greater than 1.
+        Also requires that `overview_level` is provided for `decimation_base` values greater
+        than 2.
 
     .. deprecated:: 5.1.2
         `web_optimized` is deprecated in favor of `tms`.
         Previously, `tms` usage was conditioned by `web_optimized` state.
         The behaviour has changed to allow setting a tile matrix set without the need of `web_optimized` flag.
         `web_optimized` now only serve to activate a default `WebMercatorQuad` tile matrix set.
         Set to be removed 6.0.
@@ -183,14 +188,23 @@
     if web_optimized:
         warnings.warn(
             "'web_optomized' option is deprecated and will be removed in 6.0. Please use the `tms` option",
             DeprecationWarning,
         )
         tms = tms or morecantile.tms.get("WebMercatorQuad")
 
+    if decimation_base <= 1:
+        raise ValueError(
+            "Decimation base must be greater than 1 for building overviews."
+        )
+    elif decimation_base > 2 and overview_level is None:
+        raise ValueError(
+            "Decimation base values greater than 2 require that overview_level is defined."
+        )
+
     dst_kwargs = dst_kwargs.copy()
 
     if isinstance(indexes, int):
         indexes = (indexes,)
 
     config = config or {}
     with rasterio.Env(**config):
@@ -339,15 +353,15 @@
                     overview_level = get_maximum_overview_level(
                         vrt_dst.width, vrt_dst.height, minsize=tilesize
                     )
 
                 if not quiet and overview_level:
                     click.echo("Adding overviews...", err=True)
 
-                overviews = [2**j for j in range(1, overview_level + 1)]
+                overviews = [decimation_base**j for j in range(1, overview_level + 1)]
                 tmp_dst.build_overviews(overviews, ResamplingEnums[overview_resampling])
 
                 if not quiet:
                     click.echo("Updating dataset tags...", err=True)
 
                 for i, b in enumerate(indexes):
                     tmp_dst.set_band_description(i + 1, src_dst.descriptions[b - 1])
```

### Comparing `rio_cogeo-5.2.0/rio_cogeo/models.py` & `rio_cogeo-5.3.0/rio_cogeo/models.py`

 * *Files identical despite different names*

### Comparing `rio_cogeo-5.2.0/rio_cogeo/profiles.py` & `rio_cogeo-5.3.0/rio_cogeo/profiles.py`

 * *Files identical despite different names*

### Comparing `rio_cogeo-5.2.0/rio_cogeo/scripts/cli.py` & `rio_cogeo-5.3.0/rio_cogeo/scripts/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,22 @@
     "--overview-level",
     type=int,
     help="Overview level (if not provided, appropriate overview level will be "
     "selected until the smallest overview is smaller than the value of the "
     "internal blocksize)",
 )
 @click.option(
+    "--decimation-base",
+    type=int,
+    help="Decimation base, how to sub-divide a raster for each overview level. "
+    "Also requires that --overview-level is provided.",
+    default=2,
+    show_default=True,
+)
+@click.option(
     "--overview-resampling",
     help="Overview creation resampling algorithm.",
     type=click.Choice(list(typing.get_args(RIOResampling))),
     default="nearest",
     show_default=True,
 )
 @click.option(
@@ -226,14 +234,15 @@
     bidx,
     cogeo_profile,
     nodata,
     dtype,
     add_mask,
     blocksize,
     overview_level,
+    decimation_base,
     overview_resampling,
     overview_blocksize,
     web_optimized,
     zoom_level_strategy,
     zoom_level,
     aligned_levels,
     resampling,
@@ -314,14 +323,15 @@
         config=config,
         allow_intermediate_compression=allow_intermediate_compression,
         forward_band_tags=forward_band_tags,
         forward_ns_tags=forward_ns_tags,
         tms=tilematrixset,
         use_cog_driver=use_cog_driver,
         quiet=quiet,
+        decimation_base=decimation_base,
     )
 
 
 @cogeo.command(short_help="Validate COGEO")
 @options.file_in_arg
 @click.option(
     "--strict",
```

### Comparing `rio_cogeo-5.2.0/rio_cogeo/utils.py` & `rio_cogeo-5.3.0/rio_cogeo/utils.py`

 * *Files identical despite different names*

### Comparing `rio_cogeo-5.2.0/PKG-INFO` & `rio_cogeo-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-cogeo
-Version: 5.2.0
+Version: 5.3.0
 Summary: Cloud Optimized GeoTIFF (COGEO) creation plugin for rasterio
 Keywords: COGEO,CloudOptimized Geotiff,rasterio
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rio-cogeo Version: 5.2.0 Summary: Cloud Optimized
+Metadata-Version: 2.1 Name: rio-cogeo Version: 5.3.0 Summary: Cloud Optimized
 GeoTIFF (COGEO) creation plugin for rasterio Keywords: COGEO,CloudOptimized
 Geotiff,rasterio Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

