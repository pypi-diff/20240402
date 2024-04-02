# Comparing `tmp/sopa-1.0.7.tar.gz` & `tmp/sopa-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopa-1.0.7.tar", max compression
+gzip compressed data, was "sopa-1.0.8.tar", max compression
```

## Comparing `sopa-1.0.7.tar` & `sopa-1.0.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1523 2024-03-29 10:03:47.500038 sopa-1.0.7/LICENSE
--rw-r--r--   0        0        0     5407 2024-03-29 10:03:47.500038 sopa-1.0.7/README.md
--rw-r--r--   0        0        0     2749 2024-03-29 10:03:47.532039 sopa-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      185 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/__init__.py
--rw-r--r--   0        0        0     1258 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/_constants.py
--rw-r--r--   0        0        0     1075 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/_logging.py
--rw-r--r--   0        0        0     5866 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/_sdata.py
--rw-r--r--   0        0        0       58 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/annotation/__init__.py
--rw-r--r--   0        0        0     1683 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/annotation/fluorescence.py
--rw-r--r--   0        0        0       34 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/annotation/tangram/__init__.py
--rw-r--r--   0        0        0     9736 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/annotation/tangram/run.py
--rw-r--r--   0        0        0     2640 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/cli/annotate.py
--rw-r--r--   0        0        0     7640 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/cli/app.py
--rw-r--r--   0        0        0     4436 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/cli/check.py
--rw-r--r--   0        0        0     4833 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/cli/explorer.py
--rw-r--r--   0        0        0     3926 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/cli/patchify.py
--rw-r--r--   0        0        0     3572 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/cli/resolve.py
--rw-r--r--   0        0        0     6812 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/cli/segmentation.py
--rw-r--r--   0        0        0      562 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/cli/utils.py
--rw-r--r--   0        0        0       79 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/embedding/__init__.py
--rw-r--r--   0        0        0     1937 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/embedding/cluster.py
--rw-r--r--   0        0        0      182 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/embedding/models/__init__.py
--rw-r--r--   0        0        0      374 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/embedding/models/dinov2.py
--rw-r--r--   0        0        0      496 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/embedding/models/histo_ssl.py
--rw-r--r--   0        0        0      876 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/embedding/models/resnet.py
--rw-r--r--   0        0        0     8361 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/embedding/patches.py
--rw-r--r--   0        0        0      314 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/__init__.py
--rw-r--r--   0        0        0      278 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/explorer/__init__.py
--rw-r--r--   0        0        0     3919 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/explorer/_constants.py
--rw-r--r--   0        0        0     7882 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/explorer/converter.py
--rw-r--r--   0        0        0     8807 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/explorer/images.py
--rw-r--r--   0        0        0     7213 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/explorer/points.py
--rw-r--r--   0        0        0     3779 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/explorer/shapes.py
--rw-r--r--   0        0        0     5112 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/explorer/table.py
--rw-r--r--   0        0        0      906 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/explorer/utils.py
--rw-r--r--   0        0        0     3972 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/histopathology.py
--rw-r--r--   0        0        0    10199 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/imaging.py
--rw-r--r--   0        0        0       35 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/report/__init__.py
--rw-r--r--   0        0        0   207321 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/report/css.py
--rw-r--r--   0        0        0     8116 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/report/engine.py
--rw-r--r--   0        0        0     6735 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/report/generate.py
--rw-r--r--   0        0        0     2987 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/standardize.py
--rw-r--r--   0        0        0     9291 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/io/transcriptomics.py
--rw-r--r--   0        0        0       25 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/main.py
--rw-r--r--   0        0        0      187 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/__init__.py
--rw-r--r--   0        0        0    12558 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/aggregate.py
--rw-r--r--   0        0        0        0 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/baysor/__init__.py
--rw-r--r--   0        0        0      549 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/baysor/prepare.py
--rw-r--r--   0        0        0     6554 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/baysor/resolve.py
--rw-r--r--   0        0        0     2518 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/methods.py
--rw-r--r--   0        0        0    13339 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/patching.py
--rw-r--r--   0        0        0     6795 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/shapes.py
--rw-r--r--   0        0        0     7341 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/stainings.py
--rw-r--r--   0        0        0     4548 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/segmentation/tissue.py
--rw-r--r--   0        0        0      194 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/spatial/__init__.py
--rw-r--r--   0        0        0     4840 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/spatial/_build.py
--rw-r--r--   0        0        0     4154 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/spatial/_graph.py
--rw-r--r--   0        0        0     5628 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/spatial/distance.py
--rw-r--r--   0        0        0     6409 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/spatial/morpho.py
--rw-r--r--   0        0        0     1933 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/spatial/utils.py
--rw-r--r--   0        0        0        0 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/utils/__init__.py
--rw-r--r--   0        0        0     7128 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/utils/data.py
--rw-r--r--   0        0        0     2346 2024-03-29 10:03:47.532039 sopa-1.0.7/sopa/utils/image.py
--rw-r--r--   0        0        0     5067 2024-03-29 10:03:47.536039 sopa-1.0.7/sopa/utils/polygon_crop.py
--rw-r--r--   0        0        0     7737 1970-01-01 00:00:00.000000 sopa-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1523 2024-04-02 21:44:23.275434 sopa-1.0.8/LICENSE
+-rw-r--r--   0        0        0     5407 2024-04-02 21:44:23.275434 sopa-1.0.8/README.md
+-rw-r--r--   0        0        0     2749 2024-04-02 21:44:23.303434 sopa-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      185 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/__init__.py
+-rw-r--r--   0        0        0     1258 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/_constants.py
+-rw-r--r--   0        0        0     1075 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/_logging.py
+-rw-r--r--   0        0        0     7259 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/_sdata.py
+-rw-r--r--   0        0        0       58 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/annotation/__init__.py
+-rw-r--r--   0        0        0     1683 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/annotation/fluorescence.py
+-rw-r--r--   0        0        0       34 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/annotation/tangram/__init__.py
+-rw-r--r--   0        0        0     9736 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/annotation/tangram/run.py
+-rw-r--r--   0        0        0     2640 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/annotate.py
+-rw-r--r--   0        0        0     7640 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/app.py
+-rw-r--r--   0        0        0     4436 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/check.py
+-rw-r--r--   0        0        0     4833 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/explorer.py
+-rw-r--r--   0        0        0     3926 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/patchify.py
+-rw-r--r--   0        0        0     3572 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/resolve.py
+-rw-r--r--   0        0        0     6812 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/segmentation.py
+-rw-r--r--   0        0        0      562 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/cli/utils.py
+-rw-r--r--   0        0        0       79 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/cluster.py
+-rw-r--r--   0        0        0      182 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/models/__init__.py
+-rw-r--r--   0        0        0      374 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/models/dinov2.py
+-rw-r--r--   0        0        0      496 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/models/histo_ssl.py
+-rw-r--r--   0        0        0      876 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/models/resnet.py
+-rw-r--r--   0        0        0     8381 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/embedding/patches.py
+-rw-r--r--   0        0        0      314 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/__init__.py
+-rw-r--r--   0        0        0      278 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/__init__.py
+-rw-r--r--   0        0        0     3919 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/_constants.py
+-rw-r--r--   0        0        0     7882 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/converter.py
+-rw-r--r--   0        0        0     8851 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/images.py
+-rw-r--r--   0        0        0     7213 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/points.py
+-rw-r--r--   0        0        0     3779 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/shapes.py
+-rw-r--r--   0        0        0     5112 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/table.py
+-rw-r--r--   0        0        0      906 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/explorer/utils.py
+-rw-r--r--   0        0        0     3972 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/histopathology.py
+-rw-r--r--   0        0        0    10199 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/imaging.py
+-rw-r--r--   0        0        0       35 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/report/__init__.py
+-rw-r--r--   0        0        0   207321 2024-04-02 21:44:23.303434 sopa-1.0.8/sopa/io/report/css.py
+-rw-r--r--   0        0        0     8116 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/io/report/engine.py
+-rw-r--r--   0        0        0     6735 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/io/report/generate.py
+-rw-r--r--   0        0        0     2987 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/io/standardize.py
+-rw-r--r--   0        0        0     9291 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/io/transcriptomics.py
+-rw-r--r--   0        0        0       25 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/main.py
+-rw-r--r--   0        0        0      187 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/__init__.py
+-rw-r--r--   0        0        0    12678 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/aggregate.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/baysor/__init__.py
+-rw-r--r--   0        0        0      549 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/baysor/prepare.py
+-rw-r--r--   0        0        0     6615 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/baysor/resolve.py
+-rw-r--r--   0        0        0     2518 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/methods.py
+-rw-r--r--   0        0        0    13418 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/patching.py
+-rw-r--r--   0        0        0     6795 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/shapes.py
+-rw-r--r--   0        0        0     7390 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/stainings.py
+-rw-r--r--   0        0        0     4590 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/segmentation/tissue.py
+-rw-r--r--   0        0        0      194 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/__init__.py
+-rw-r--r--   0        0        0     4840 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/_build.py
+-rw-r--r--   0        0        0     4154 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/_graph.py
+-rw-r--r--   0        0        0     5628 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/distance.py
+-rw-r--r--   0        0        0     6409 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/morpho.py
+-rw-r--r--   0        0        0     1933 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/spatial/utils.py
+-rw-r--r--   0        0        0        0 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/utils/__init__.py
+-rw-r--r--   0        0        0     7128 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/utils/data.py
+-rw-r--r--   0        0        0     2346 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/utils/image.py
+-rw-r--r--   0        0        0     5109 2024-04-02 21:44:23.307434 sopa-1.0.8/sopa/utils/polygon_crop.py
+-rw-r--r--   0        0        0     7737 1970-01-01 00:00:00.000000 sopa-1.0.8/PKG-INFO
```

### Comparing `sopa-1.0.7/LICENSE` & `sopa-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/README.md` & `sopa-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/pyproject.toml` & `sopa-1.0.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sopa"
-version = "1.0.7"
+version = "1.0.8"
 description = "Spatial-omics pipeline and analysis"
 documentation = "https://gustaveroussy.github.io/sopa"
 homepage = "https://gustaveroussy.github.io/sopa"
 repository = "https://github.com/gustaveroussy/sopa"
 authors = ["Quentin Blampey <quentin.blampey@gmail.com>"]
 packages = [{ include = "sopa" }]
 license = "BSD-3-Clause"
@@ -19,16 +19,16 @@
 ]
 
 [tool.poetry.scripts]
 sopa = "sopa.main:app"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-spatialdata = ">=0.1.1"
-spatialdata-io = ">=0.1.1"
+spatialdata = ">=0.1.2"
+spatialdata-io = ">=0.1.2"
 scanpy = ">=1.9.5,!=1.9.7"
 botocore = "1.34.19"
 typer = ">=0.9.0"
 setuptools = ">=69.2.0"
 
 cellpose = { version = ">=3.0.5", optional = true }
 opencv-python = { version = ">=4.8.0.76", optional = true }
```

### Comparing `sopa-1.0.7/sopa/_constants.py` & `sopa-1.0.8/sopa/_constants.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/_logging.py` & `sopa-1.0.8/sopa/_logging.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/_sdata.py` & `sopa-1.0.8/sopa/_sdata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from __future__ import annotations
 
 import logging
+from pathlib import Path
 from typing import Iterator
 
 import geopandas as gpd
 import pandas as pd
 import xarray as xr
+import zarr
 from multiscale_spatial_image import MultiscaleSpatialImage
+from ome_zarr.io import parse_url
 from spatial_image import SpatialImage
 from spatialdata import SpatialData
+from spatialdata._io import write_image, write_shapes, write_table
 from spatialdata.models import SpatialElement
 from spatialdata.transformations import Identity, get_transformation, set_transformation
 
 from ._constants import SopaKeys
 
 log = logging.getLogger(__name__)
 
@@ -172,7 +176,48 @@
     image = sdata.images[key]
     if isinstance(image, MultiscaleSpatialImage):
         image = SpatialImage(next(iter(image["scale0"].values())))
 
     if return_key:
         return key, image
     return image
+
+
+def save_shapes(
+    sdata: SpatialData,
+    name: str,
+    overwrite: bool = False,
+) -> None:
+    elem_group = sdata._init_add_element(name=name, element_type="shapes", overwrite=overwrite)
+    write_shapes(
+        shapes=sdata.shapes[name],
+        group=elem_group,
+        name=name,
+    )
+
+
+def save_image(
+    sdata: SpatialData,
+    name: str,
+    overwrite: bool = False,
+) -> None:
+    elem_group = sdata._init_add_element(name=name, element_type="images", overwrite=overwrite)
+    write_image(
+        image=sdata.images[name],
+        group=elem_group,
+        name=name,
+    )
+    from spatialdata._io.io_raster import _read_multiscale
+
+    # reload the image from the Zarr storage so that now the element is lazy loaded, and most importantly,
+    # from the correct storage
+    assert elem_group.path == "images"
+    path = Path(elem_group.store.path) / "images" / name
+    image = _read_multiscale(path, raster_type="image")
+    sdata._add_image_in_memory(name=name, image=image, overwrite=True)
+
+
+def save_table(sdata: SpatialData):
+    store = parse_url(sdata.path, mode="r+").store
+    root = zarr.group(store=store)
+    elem_group = root.require_group(name="table")
+    write_table(table=sdata.table, group=elem_group, name="table")
```

### Comparing `sopa-1.0.7/sopa/annotation/fluorescence.py` & `sopa-1.0.8/sopa/annotation/fluorescence.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/annotation/tangram/run.py` & `sopa-1.0.8/sopa/annotation/tangram/run.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/cli/annotate.py` & `sopa-1.0.8/sopa/cli/annotate.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/cli/app.py` & `sopa-1.0.8/sopa/cli/app.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/cli/check.py` & `sopa-1.0.8/sopa/cli/check.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/cli/explorer.py` & `sopa-1.0.8/sopa/cli/explorer.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/cli/patchify.py` & `sopa-1.0.8/sopa/cli/patchify.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/cli/resolve.py` & `sopa-1.0.8/sopa/cli/resolve.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/cli/segmentation.py` & `sopa-1.0.8/sopa/cli/segmentation.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/cli/utils.py` & `sopa-1.0.8/sopa/cli/utils.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/embedding/cluster.py` & `sopa-1.0.8/sopa/embedding/cluster.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/embedding/models/resnet.py` & `sopa-1.0.8/sopa/embedding/models/resnet.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/embedding/patches.py` & `sopa-1.0.8/sopa/embedding/patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 import tqdm
 from multiscale_spatial_image import MultiscaleSpatialImage
 from spatial_image import SpatialImage
 from spatialdata import SpatialData, bounding_box_query
 from spatialdata.models import Image2DModel
 from spatialdata.transformations import Scale
 
-import sopa.embedding.models as models
-from sopa._constants import SopaKeys
-from sopa._sdata import get_intrinsic_cs, get_key
-from sopa.segmentation import Patches2D
+from .._constants import SopaKeys
+from .._sdata import get_intrinsic_cs, get_key, save_image
+from ..segmentation import Patches2D
+from . import models
 
 log = logging.getLogger(__name__)
 
 
 def _get_best_level_for_downsample(
     level_downsamples: list[float], downsample: float, epsilon: float = 0.01
 ) -> int:
@@ -213,14 +213,15 @@
             embedder.cs: Scale([embedder.patch_width, embedder.patch_width], axes=("x", "y"))
         },
     )
     embedding_image.coords["y"] = embedder.patch_width * embedding_image.coords["y"]
     embedding_image.coords["x"] = embedder.patch_width * embedding_image.coords["x"]
 
     embedding_key = f"sopa_{model_name}"
-    sdata.add_image(embedding_key, embedding_image)
+    sdata.images[embedding_key] = embedding_image
+    save_image(sdata, embedding_key)
 
     log.info(f"WSI embeddings saved as an image in sdata['{embedding_key}']")
 
     patches.write(shapes_key=SopaKeys.EMBEDDINGS_PATCHES_KEY)
 
     return sdata[embedding_key]
```

### Comparing `sopa-1.0.7/sopa/io/explorer/_constants.py` & `sopa-1.0.8/sopa/io/explorer/_constants.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/explorer/converter.py` & `sopa-1.0.8/sopa/io/explorer/converter.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/explorer/images.py` & `sopa-1.0.8/sopa/io/explorer/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import xarray as xr
 from multiscale_spatial_image import MultiscaleSpatialImage, to_multiscale
 from spatial_image import SpatialImage
 from spatialdata import SpatialData
 from spatialdata.transformations import Affine, set_transformation
 from tqdm import tqdm
 
-from ..._sdata import get_intrinsic_cs, get_spatial_image
+from ..._sdata import get_intrinsic_cs, get_spatial_image, save_image
 from ...utils.image import resize_numpy, scale_dtype
 from ._constants import ExplorerConstants, FileNames, image_metadata
 from .utils import explorer_file_path
 
 log = logging.getLogger(__name__)
 
 TILE_SIZE = ExplorerConstants.TILE_SIZE
@@ -220,8 +220,9 @@
 
     default_image = get_spatial_image(sdata, image_key)
     pixel_cs = get_intrinsic_cs(sdata, default_image)
 
     set_transformation(image, {pixel_cs: to_pixel}, set_all=True)
 
     log.info(f"Adding image {image_name}:\n{image}")
-    sdata.add_image(image_name, image, overwrite=overwrite)
+    sdata.images[image_name] = image
+    save_image(sdata, image_name, overwrite=overwrite)
```

### Comparing `sopa-1.0.7/sopa/io/explorer/points.py` & `sopa-1.0.8/sopa/io/explorer/points.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/explorer/shapes.py` & `sopa-1.0.8/sopa/io/explorer/shapes.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/explorer/table.py` & `sopa-1.0.8/sopa/io/explorer/table.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/explorer/utils.py` & `sopa-1.0.8/sopa/io/explorer/utils.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/histopathology.py` & `sopa-1.0.8/sopa/io/histopathology.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/imaging.py` & `sopa-1.0.8/sopa/io/imaging.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/report/css.py` & `sopa-1.0.8/sopa/io/report/css.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/report/engine.py` & `sopa-1.0.8/sopa/io/report/engine.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/report/generate.py` & `sopa-1.0.8/sopa/io/report/generate.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/standardize.py` & `sopa-1.0.8/sopa/io/standardize.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/io/transcriptomics.py` & `sopa-1.0.8/sopa/io/transcriptomics.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/segmentation/aggregate.py` & `sopa-1.0.8/sopa/segmentation/aggregate.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 from .._constants import SopaKeys
 from .._sdata import (
     get_boundaries,
     get_element,
     get_item,
     get_spatial_image,
+    save_shapes,
+    save_table,
     to_intrinsic,
 )
 from ..io.explorer.utils import str_cell_id
 from . import shapes
 
 log = logging.getLogger(__name__)
 
@@ -69,15 +71,16 @@
 
         self.table = sdata.table
 
     def standardize_table(self):
         self.table.obs_names = list(map(str_cell_id, range(self.table.n_obs)))
 
         self.geo_df.index = list(self.table.obs_names)
-        self.sdata.add_shapes(self.shapes_key, self.geo_df, overwrite=True)
+        self.sdata.shapes[self.shapes_key] = self.geo_df
+        save_shapes(self.sdata, self.shapes_key, overwrite=True)
 
         self.table.obsm["spatial"] = np.array(
             [[centroid.x, centroid.y] for centroid in self.geo_df.centroid]
         )
         self.table.obs[SopaKeys.REGION_KEY] = pd.Series(
             self.shapes_key, index=self.table.obs_names, dtype="category"
         )
@@ -96,15 +99,16 @@
             region_key=SopaKeys.REGION_KEY,
             region=self.shapes_key,
             instance_key=SopaKeys.INSTANCE_KEY,
         )
 
         if self.sdata.table is not None and self.overwrite:
             del self.sdata.table
-        self.sdata.table = self.table
+        self.sdata.tables["table"] = self.table
+        save_table(self.sdata)
 
     def filter_cells(self, where_filter: np.ndarray):
         log.info(f"Filtering {where_filter.sum()} cells")
 
         self.geo_df = self.geo_df[~where_filter]
 
         if self.table is not None:
```

### Comparing `sopa-1.0.7/sopa/segmentation/baysor/prepare.py` & `sopa-1.0.8/sopa/segmentation/baysor/prepare.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/segmentation/baysor/resolve.py` & `sopa-1.0.8/sopa/segmentation/baysor/resolve.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from shapely.geometry import Polygon, shape
 from spatialdata import SpatialData
 from spatialdata.models import ShapesModel, TableModel
 from spatialdata.transformations import get_transformation
 from tqdm import tqdm
 
 from ..._constants import SopaKeys
-from ..._sdata import get_element, get_key
+from ..._sdata import get_element, get_key, save_shapes
 from .. import aggregate, shapes
 
 log = logging.getLogger(__name__)
 
 
 def read_baysor(
     directory: str, min_area: float = 0, min_vertices: int = 4
@@ -167,15 +167,16 @@
     table = TableModel.parse(
         table,
         region_key=SopaKeys.REGION_KEY,
         region=SopaKeys.BAYSOR_BOUNDARIES,
         instance_key=SopaKeys.INSTANCE_KEY,
     )
 
-    sdata.add_shapes(SopaKeys.BAYSOR_BOUNDARIES, geo_df, overwrite=True)
+    sdata.shapes[SopaKeys.BAYSOR_BOUNDARIES] = geo_df
+    save_shapes(sdata, SopaKeys.BAYSOR_BOUNDARIES, overwrite=True)
 
     if sdata.table is not None:
         log.warn("Table already existing. It will be replaced by the new one.")
         del sdata.table
 
     sdata.table = table
```

### Comparing `sopa-1.0.7/sopa/segmentation/methods.py` & `sopa-1.0.8/sopa/segmentation/methods.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/segmentation/patching.py` & `sopa-1.0.8/sopa/segmentation/patching.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,21 @@
 from shapely.geometry import GeometryCollection, MultiPolygon, Polygon, box
 from spatial_image import SpatialImage
 from spatialdata import SpatialData
 from spatialdata.models import ShapesModel
 from spatialdata.transformations import get_transformation
 
 from .._constants import EPS, ROI, SopaFiles, SopaKeys
-from .._sdata import get_boundaries, get_item, get_spatial_image, to_intrinsic
+from .._sdata import (
+    get_boundaries,
+    get_item,
+    get_spatial_image,
+    save_shapes,
+    to_intrinsic,
+)
 
 log = logging.getLogger(__name__)
 
 
 class Patches1D:
     def __init__(self, xmin, xmax, patch_width, patch_overlap, tight, int_coords):
         self.xmin, self.xmax = xmin, xmax
@@ -200,15 +206,16 @@
                 SopaKeys.PATCHES_ILOCS: self.ilocs.tolist(),
             }
         )
         geo_df = ShapesModel.parse(
             geo_df, transformations=get_transformation(self.element, get_all=True)
         )
 
-        self.sdata.add_shapes(shapes_key, geo_df, overwrite=overwrite)
+        self.sdata.shapes[shapes_key] = geo_df
+        save_shapes(self.sdata, shapes_key, overwrite=overwrite)
 
         log.info(f"{len(geo_df)} patches were saved in sdata['{shapes_key}']")
 
         return geo_df
 
     def patchify_transcripts(
         self,
```

### Comparing `sopa-1.0.7/sopa/segmentation/shapes.py` & `sopa-1.0.8/sopa/segmentation/shapes.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/segmentation/stainings.py` & `sopa-1.0.8/sopa/segmentation/stainings.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from skimage import exposure
 from spatialdata import SpatialData
 from spatialdata.models import ShapesModel
 from spatialdata.transformations import get_transformation
 from tqdm import tqdm
 
 from .._constants import SopaKeys
-from .._sdata import get_spatial_image
+from .._sdata import get_spatial_image, save_shapes
 from . import shapes
 
 log = logging.getLogger(__name__)
 
 
 class StainingSegmentation:
     def __init__(
@@ -174,10 +174,11 @@
         """
         image = get_spatial_image(sdata, image_key)
 
         geo_df = gpd.GeoDataFrame({"geometry": cells})
         geo_df.index = image_key + geo_df.index.astype(str)
 
         geo_df = ShapesModel.parse(geo_df, transformations=get_transformation(image, get_all=True))
-        sdata.add_shapes(shapes_key, geo_df, overwrite=True)
+        sdata.shapes[shapes_key] = geo_df
+        save_shapes(sdata, shapes_key, overwrite=True)
 
         log.info(f"Added {len(geo_df)} cell boundaries in sdata['{shapes_key}']")
```

### Comparing `sopa-1.0.7/sopa/segmentation/tissue.py` & `sopa-1.0.8/sopa/segmentation/tissue.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import xarray as xr
 from multiscale_spatial_image import MultiscaleSpatialImage
 from shapely.geometry import Polygon
 from spatialdata import SpatialData
 from spatialdata.models import ShapesModel
 
 from .._constants import ROI
-from .._sdata import get_intrinsic_cs, get_item
+from .._sdata import get_intrinsic_cs, get_item, save_shapes
 
 log = logging.getLogger(__name__)
 
 
 def hsv_otsu(
     sdata: SpatialData,
     image_key: str | None = None,
@@ -109,10 +109,11 @@
     )
 
     image_cs = get_intrinsic_cs(sdata, sdata[image_key])
     geo_df = spatialdata.transform(
         geo_df, image_scale.attrs["transform"][image_cs], maintain_positioning=True
     )
 
-    sdata.add_shapes(ROI.KEY, geo_df)
+    sdata.shapes[ROI.KEY] = geo_df
+    save_shapes(sdata, ROI.KEY)
 
     log.info(f"Tissue segmentation saved in sdata['{ROI.KEY}']")
```

### Comparing `sopa-1.0.7/sopa/spatial/_build.py` & `sopa-1.0.8/sopa/spatial/_build.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/spatial/_graph.py` & `sopa-1.0.8/sopa/spatial/_graph.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/spatial/distance.py` & `sopa-1.0.8/sopa/spatial/distance.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/spatial/morpho.py` & `sopa-1.0.8/sopa/spatial/morpho.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/spatial/utils.py` & `sopa-1.0.8/sopa/spatial/utils.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/utils/data.py` & `sopa-1.0.8/sopa/utils/data.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/utils/image.py` & `sopa-1.0.8/sopa/utils/image.py`

 * *Files identical despite different names*

### Comparing `sopa-1.0.7/sopa/utils/polygon_crop.py` & `sopa-1.0.8/sopa/utils/polygon_crop.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from matplotlib.widgets import PolygonSelector
 from shapely.geometry import Polygon
 from spatialdata import SpatialData
 from spatialdata.models import ShapesModel
 from spatialdata.transformations import get_transformation
 
 from .._constants import ROI
-from .._sdata import get_spatial_image
+from .._sdata import get_spatial_image, save_shapes
 from .image import resize
 
 log = logging.getLogger(__name__)
 
 HELPER = """Enclose cells within a polygon. Helper:
     - Click on the plot to add a polygon vertex
     - Press the 'esc' key to start a new polygon
@@ -130,10 +130,11 @@
         image = get_spatial_image(sdata, image_key)
 
     geo_df = gpd.GeoDataFrame(geometry=[polygon])
 
     geo_df = ShapesModel.parse(
         geo_df, transformations=get_transformation(sdata[image_key], get_all=True)
     )
-    sdata.add_shapes(ROI.KEY, geo_df)
+    sdata.shapes[ROI.KEY] = geo_df
+    save_shapes(sdata, ROI.KEY)
 
     log.info(f"Polygon saved in sdata['{ROI.KEY}']")
```

### Comparing `sopa-1.0.7/PKG-INFO` & `sopa-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sopa
-Version: 1.0.7
+Version: 1.0.8
 Summary: Spatial-omics pipeline and analysis
 Home-page: https://gustaveroussy.github.io/sopa
 License: BSD-3-Clause
 Author: Quentin Blampey
 Author-email: quentin.blampey@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: BSD License
@@ -35,16 +35,16 @@
 Requires-Dist: mkdocstrings-python (>=1.7.3,<2.0.0) ; extra == "dev"
 Requires-Dist: opencv-python (>=4.8.0.76) ; extra == "cellpose" or extra == "wsi"
 Requires-Dist: pulp (>=2.3.1,<2.8) ; extra == "snakemake"
 Requires-Dist: pytest (>=7.1.3,<8.0.0) ; extra == "dev"
 Requires-Dist: scanpy (>=1.9.5,!=1.9.7)
 Requires-Dist: setuptools (>=69.2.0)
 Requires-Dist: snakemake (>=7.32.4,<8.0.0) ; extra == "snakemake"
-Requires-Dist: spatialdata (>=0.1.1)
-Requires-Dist: spatialdata-io (>=0.1.1)
+Requires-Dist: spatialdata (>=0.1.2)
+Requires-Dist: spatialdata-io (>=0.1.2)
 Requires-Dist: tangram-sc (>=1.0.4) ; extra == "tangram"
 Requires-Dist: tiffslide (>=2.3.1,<3.0.0) ; extra == "wsi"
 Requires-Dist: toml (>=0.10.2) ; extra == "baysor"
 Requires-Dist: torch (>=2.0.0,!=2.0.1,!=2.1.0) ; extra == "cellpose" or extra == "wsi"
 Requires-Dist: typer (>=0.9.0)
 Project-URL: Documentation, https://gustaveroussy.github.io/sopa
 Project-URL: Repository, https://github.com/gustaveroussy/sopa
```

