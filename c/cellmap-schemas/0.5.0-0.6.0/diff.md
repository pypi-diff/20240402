# Comparing `tmp/cellmap_schemas-0.5.0.tar.gz` & `tmp/cellmap_schemas-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmap_schemas-0.5.0.tar", max compression
+gzip compressed data, was "cellmap_schemas-0.6.0.tar", max compression
```

## Comparing `cellmap_schemas-0.5.0.tar` & `cellmap_schemas-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1466 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/LICENSE
--rw-r--r--   0        0        0      122 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/README.md
--rw-r--r--   0        0        0      976 2024-04-02 11:53:31.716960 cellmap_schemas-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/src/cellmap_schemas/__init__.py
--rw-r--r--   0        0        0    16120 2024-04-02 10:04:21.469891 cellmap_schemas-0.5.0/src/cellmap_schemas/annotation.py
--rw-r--r--   0        0        0     1521 2024-01-12 21:08:32.904506 cellmap_schemas-0.5.0/src/cellmap_schemas/base.py
--rw-r--r--   0        0        0     4239 2024-01-03 14:53:17.430748 cellmap_schemas-0.5.0/src/cellmap_schemas/cli.py
--rw-r--r--   0        0        0        0 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/__init__.py
--rw-r--r--   0        0        0    20923 2024-01-12 21:08:32.904506 cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/cosem.py
--rw-r--r--   0        0        0     8645 2024-01-12 21:08:32.904506 cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py
--rw-r--r--   0        0        0    10524 2024-01-12 21:08:32.904506 cellmap_schemas-0.5.0/src/cellmap_schemas/n5_wrap.py
--rw-r--r--   0        0        0        0 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/src/cellmap_schemas/py.typed
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 cellmap_schemas-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1466 2024-04-02 13:34:59.790001 cellmap_schemas-0.6.0/LICENSE
+-rw-r--r--   0        0        0      122 2024-04-02 13:34:59.790001 cellmap_schemas-0.6.0/README.md
+-rw-r--r--   0        0        0      976 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/__init__.py
+-rw-r--r--   0        0        0    16120 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/annotation.py
+-rw-r--r--   0        0        0     1393 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/base.py
+-rw-r--r--   0        0        0     4274 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/cli.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/__init__.py
+-rw-r--r--   0        0        0    20877 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/cosem.py
+-rw-r--r--   0        0        0     8679 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py
+-rw-r--r--   0        0        0    10559 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/n5_wrap.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:34:59.794001 cellmap_schemas-0.6.0/src/cellmap_schemas/py.typed
+-rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 cellmap_schemas-0.6.0/PKG-INFO
```

### Comparing `cellmap_schemas-0.5.0/LICENSE` & `cellmap_schemas-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.5.0/pyproject.toml` & `cellmap_schemas-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cellmap-schemas"
-version = "0.5.0"
+version = "0.6.0"
 description = "Schemas for data used by the Cellmap project team at Janelia Research Campus."
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cellmap_schemas", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `cellmap_schemas-0.5.0/src/cellmap_schemas/annotation.py` & `cellmap_schemas-0.6.0/src/cellmap_schemas/annotation.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.5.0/src/cellmap_schemas/base.py` & `cellmap_schemas-0.6.0/src/cellmap_schemas/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,17 @@
+from __future__ import annotations
 from pydantic_zarr.v2 import ArraySpec, GroupSpec
 
 
-def structure_array_equal(spec_a: ArraySpec, spec_b: ArraySpec) -> bool:
-    return spec_a.model_dump(exclude=["attributes"]) == spec_b.model_dump(exclude=["attributes"])
-
-
 def structure_group_equal(spec_a: GroupSpec, spec_b: GroupSpec) -> bool:
     keys_equal = spec_a.members.keys() == spec_b.members.keys()
     if keys_equal:
         for member_a, member_b in zip(spec_a.members.values(), spec_b.members.values()):
             if isinstance(member_a, ArraySpec):
-                member_eq = structure_array_equal(member_a, member_b)
+                member_eq = member_a.like(member_b, exclude={"attributes"})
             else:
                 member_eq = structure_group_equal(member_a, member_b)
             if member_eq is False:
                 return False
         return True
     else:
         return False
@@ -27,12 +24,12 @@
     if not (
         isinstance(spec_a, (ArraySpec, GroupSpec)) and isinstance(spec_b, (ArraySpec, GroupSpec))
     ):
         raise TypeError(
             f"Cannot apply this function to objects with types ({type(spec_a)}, {type(spec_b)})"
         )
     if isinstance(spec_a, ArraySpec) and isinstance(spec_b, ArraySpec):
-        return structure_array_equal(spec_a, spec_b)
+        return spec_a.like(spec_b, exclude="attributes")
     elif isinstance(spec_a, GroupSpec) and isinstance(spec_b, GroupSpec):
         return structure_group_equal(spec_a, spec_b)
     else:
         return False
```

### Comparing `cellmap_schemas-0.5.0/src/cellmap_schemas/cli.py` & `cellmap_schemas-0.6.0/src/cellmap_schemas/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from typing import Any, Literal, Tuple, Union, cast
 import click
 from pydantic_zarr.v2 import ArraySpec, GroupSpec, from_zarr
 from pydantic import ValidationError
 import zarr
 from rich.console import Console
 from rich.traceback import install
```

### Comparing `cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/cosem.py` & `cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/cosem.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 This module contains Pydantic models for "COSEM-flavored" multiscale images. These images
 are  stored in the [N5](https://github.com/saalfeldlab/n5) format, and use a layout / metadata
 that's compatible with the [Neuroglancer](https://github.com/google/neuroglancer) visualization tool.
 
 Note that the hierarchy convention modeled here will likely be superceded by conventions defined
 in the [OME-NGFF](https://ngff.openmicroscopy.org/) specification.
 """
-
+from __future__ import annotations
 from typing import Annotated, Dict, List, Literal, Optional, Sequence, Tuple
 import numpy as np
 from pydantic_zarr.v2 import GroupSpec, ArraySpec
 from pydantic import BaseModel, Field, model_validator
 from cellmap_schemas.multiscale import neuroglancer_n5
 from cellmap_schemas.multiscale.neuroglancer_n5 import PixelResolution
 
@@ -488,27 +488,23 @@
     }
     base_member = tuple(members_sorted.values())[0]
     base_transform = base_member.attributes.transform
     new_base_transform = new_sttransform(
         base_transform, scale=scale, axes=axes, order=order, translate=translate, units=units
     )
     # if we started at 4 and end up at 8, then the scale_diff should be 2
-    scale_diff = [
-        a / b for a, b in zip(new_base_transform.scale, base_transform.scale, strict=True)
-    ]
+    scale_diff = [a / b for a, b in zip(new_base_transform.scale, base_transform.scale)]
     # if we started at 0 and we are moved to 10, then the translation_diff should be +10
-    translate_diff = [
-        a - b for a, b in zip(new_base_transform.translate, base_transform.translate, strict=True)
-    ]
+    translate_diff = [a - b for a, b in zip(new_base_transform.translate, base_transform.translate)]
     new_transforms = {}
 
     for key, member in members_sorted.items():
         old_tx = member.attributes.transform
-        new_scale = [a * b for a, b in zip(old_tx.scale, scale_diff, strict=True)]
-        new_trans = [a + b for a, b in zip(old_tx.translate, translate_diff, strict=True)]
+        new_scale = [a * b for a, b in zip(old_tx.scale, scale_diff)]
+        new_trans = [a + b for a, b in zip(old_tx.translate, translate_diff)]
         new_transforms[key] = new_sttransform(
             old_tx, scale=new_scale, translate=new_trans, order=order, units=units, axes=axes
         )
 
     new_groupmeta = GroupMetadata.from_transforms(
         new_transforms, name=group.attributes.multiscales[0].name
     )
```

### Comparing `cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py` & `cellmap_schemas-0.6.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This module contains Pydantic models for Neuroglancer-compatible multiscale images stored 
 in N5 groups. See Neuroglancer's [N5-specific documentation](https://github.com/google/neuroglancer/tree/master/src/neuroglancer/datasource/n5) 
 for details on what Neuroglancer expects when it reads N5 data.
 """
-
+from __future__ import annotations
 from typing import Annotated, Sequence
 from pydantic import BaseModel, PositiveInt, model_validator, AfterValidator
 from pydantic_zarr.v2 import ArraySpec
 
 from cellmap_schemas.n5_wrap import N5GroupSpec
```

### Comparing `cellmap_schemas-0.5.0/src/cellmap_schemas/n5_wrap.py` & `cellmap_schemas-0.6.0/src/cellmap_schemas/n5_wrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 from pydantic_zarr.v2 import ArraySpec, GroupSpec
 from typing import overload, Union
 
 from zarr.core import Array
 from zarr.storage import BaseStore
 import zarr
```

### Comparing `cellmap_schemas-0.5.0/PKG-INFO` & `cellmap_schemas-0.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap-schemas
-Version: 0.5.0
+Version: 0.6.0
 Summary: Schemas for data used by the Cellmap project team at Janelia Research Campus.
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

