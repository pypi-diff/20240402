# Comparing `tmp/cellmap_schemas-0.4.0.tar.gz` & `tmp/cellmap_schemas-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellmap_schemas-0.4.0.tar", max compression
+gzip compressed data, was "cellmap_schemas-0.5.0.tar", max compression
```

## Comparing `cellmap_schemas-0.4.0.tar` & `cellmap_schemas-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1466 2024-01-02 16:41:13.694316 cellmap_schemas-0.4.0/LICENSE
--rw-r--r--   0        0        0      122 2024-01-02 16:41:13.694316 cellmap_schemas-0.4.0/README.md
--rw-r--r--   0        0        0      976 2024-01-12 21:08:45.172651 cellmap_schemas-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-02 16:41:13.694316 cellmap_schemas-0.4.0/src/cellmap_schemas/__init__.py
--rw-r--r--   0        0        0    15006 2024-01-03 14:53:17.430748 cellmap_schemas-0.4.0/src/cellmap_schemas/annotation.py
--rw-r--r--   0        0        0     1521 2024-01-12 21:08:32.904506 cellmap_schemas-0.4.0/src/cellmap_schemas/base.py
--rw-r--r--   0        0        0     4239 2024-01-03 14:53:17.430748 cellmap_schemas-0.4.0/src/cellmap_schemas/cli.py
--rw-r--r--   0        0        0        0 2024-01-02 16:41:13.694316 cellmap_schemas-0.4.0/src/cellmap_schemas/multiscale/__init__.py
--rw-r--r--   0        0        0    20923 2024-01-12 21:08:32.904506 cellmap_schemas-0.4.0/src/cellmap_schemas/multiscale/cosem.py
--rw-r--r--   0        0        0     8645 2024-01-12 21:08:32.904506 cellmap_schemas-0.4.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py
--rw-r--r--   0        0        0    10524 2024-01-12 21:08:32.904506 cellmap_schemas-0.4.0/src/cellmap_schemas/n5_wrap.py
--rw-r--r--   0        0        0        0 2024-01-02 16:41:13.694316 cellmap_schemas-0.4.0/src/cellmap_schemas/py.typed
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 cellmap_schemas-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1466 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/LICENSE
+-rw-r--r--   0        0        0      122 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/README.md
+-rw-r--r--   0        0        0      976 2024-04-02 11:53:31.716960 cellmap_schemas-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/src/cellmap_schemas/__init__.py
+-rw-r--r--   0        0        0    16120 2024-04-02 10:04:21.469891 cellmap_schemas-0.5.0/src/cellmap_schemas/annotation.py
+-rw-r--r--   0        0        0     1521 2024-01-12 21:08:32.904506 cellmap_schemas-0.5.0/src/cellmap_schemas/base.py
+-rw-r--r--   0        0        0     4239 2024-01-03 14:53:17.430748 cellmap_schemas-0.5.0/src/cellmap_schemas/cli.py
+-rw-r--r--   0        0        0        0 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/__init__.py
+-rw-r--r--   0        0        0    20923 2024-01-12 21:08:32.904506 cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/cosem.py
+-rw-r--r--   0        0        0     8645 2024-01-12 21:08:32.904506 cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py
+-rw-r--r--   0        0        0    10524 2024-01-12 21:08:32.904506 cellmap_schemas-0.5.0/src/cellmap_schemas/n5_wrap.py
+-rw-r--r--   0        0        0        0 2024-01-02 16:41:13.694316 cellmap_schemas-0.5.0/src/cellmap_schemas/py.typed
+-rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 cellmap_schemas-0.5.0/PKG-INFO
```

### Comparing `cellmap_schemas-0.4.0/LICENSE` & `cellmap_schemas-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.4.0/pyproject.toml` & `cellmap_schemas-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "cellmap-schemas"
-version = "0.4.0"
+version = "0.5.0"
 description = "Schemas for data used by the Cellmap project team at Janelia Research Campus."
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 readme = "README.md"
 packages = [{include = "cellmap_schemas", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic-zarr = "^0.5.2"
+pydantic-zarr = "^0.7.0"
 s3fs = "^2023.10.0"
 rich = "^13.7.0"
 
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.4.2"
```

### Comparing `cellmap_schemas-0.4.0/src/cellmap_schemas/annotation.py` & `cellmap_schemas-0.5.0/src/cellmap_schemas/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 This module defines a convention for representing a dense crop as a collection of multiscale images. Each multiscale image
 should comply with the version 0.4 of the OME-NGFF specification.
 """
 from __future__ import annotations
 from datetime import date
 from enum import Enum
 from typing import (
-    Dict,
+    Any,
     Generic,
     List,
     Literal,
     Mapping,
     Optional,
     TypeVar,
     Union,
 )
 from pydantic_zarr.v2 import GroupSpec, ArraySpec
 from pydantic import BaseModel, model_validator, field_serializer
+import zarr
 
 T = TypeVar("T")
 
 
 class CellmapWrapper(BaseModel, Generic[T]):
     """
     A generic pydantic model that wraps the type `T` under the namespace "cellmap"
@@ -110,15 +111,15 @@
 
 
 class LabelList(BaseModel, extra="forbid"):
     labels: List[Label]
     annotation_type: AnnotationType = "semantic"
 
 
-classNameDict = {
+classNamedict = {
     1: InstanceName(short="ECS", long="Extracellular Space"),
     2: InstanceName(short="Plasma membrane", long="Plasma membrane"),
     3: InstanceName(short="Mito membrane", long="Mitochondrial membrane"),
     4: InstanceName(short="Mito lumen", long="Mitochondrial lumen"),
     5: InstanceName(short="Mito DNA", long="Mitochondrial DNA"),
     6: InstanceName(short="Golgi Membrane", long="Golgi apparatus membrane"),
     7: InstanceName(short="Golgi lumen", long="Golgi apparatus lumen"),
@@ -174,54 +175,54 @@
     numerical values represent separate semantic classes.
 
     Attributes
     ----------
 
     type: Literal["semantic_segmentation"]
         Must be the string 'semantic_segmentation'.
-    encoding: Dict[Union[Possibility, Literal["present"]], int]
+    encoding: dict[Union[Possibility, Literal["present"]], int]
         This dict represents the mapping from possibilities to numeric values. The keys
         must be strings in the set `{'unknown', 'absent', 'present'}`, and the values
         must be numeric values contained in the array described by this metadata.
 
         For example, if an annotator produces an array where 0 represents `unknown` and
         1 represents the presence of class X then `encoding` would take the value
         `{'unknown': 0, 'present': 1}`
 
     """
 
     type: Literal["semantic_segmentation"] = "semantic_segmentation"
-    encoding: Dict[Union[Possibility, Literal["present"]], int]
+    encoding: dict[Union[Possibility, Literal["present"]], int]
 
 
 class InstanceSegmentation(BaseModel, extra="forbid"):
     """
     Metadata for instance segmentation, i.e. a segmentation where unique numerical
     values represent distinct occurrences of the same semantic class.
 
     Attributes
     ----------
 
     type: Literal["instance_segmentation"]
         Must be the string "instance_segmentation"
-    encoding: Dict[Possibility, int]
+    encoding: dict[Possibility, int]
         This dict represents the mapping from possibilities to numeric values. The keys
         must be strings from the set `{'unknown', 'absent'}`, and the values
         must be numeric values contained in the array described by this metadata.
 
         For example, if an annotator produces an array where 0 represents 'unknown' and
         the values 1...N represent instances of some class, then `encoding` would take
         the value {'unknown': 0}. The meaning of the non-zero values (i.e., that they
         represent distinct instances of a class) can be inferred from the fact that
         this is instance segmentation, and thus these values do not appear as keys in
         `encoding`.
     """
 
     type: Literal["instance_segmentation"] = "instance_segmentation"
-    encoding: Dict[Possibility, int]
+    encoding: dict[Possibility, int]
 
 
 AnnotationType = Union[SemanticSegmentation, InstanceSegmentation]
 
 TName = TypeVar("TName", bound=str)
 
 
@@ -230,27 +231,27 @@
     The metadata for an array of annotated values.
 
     Attributes
     ----------
 
     class_name: str
         The name of the semantic class annotated in this array.
-    complement_counts: Optional[Dict[Possibility, int]]
+    complement_counts: Optional[dict[Possibility, int]]
         The frequency of 'absent' and / or 'missing' values in the array data.
         The total number of elements in the array that represent "positive" examples can
         be calculated from these counts -- take the number of elements in the array
         minus the sum of the values in this partial histogram.
     annotation_type: SemanticSegmentation | InstanceSegmentation
         The type of the annotation. Must be either an instance of SemanticSegmentation
         or an instance of InstanceSegmentation.
     """
 
     class_name: TName
     # a mapping from values to frequencies
-    complement_counts: Optional[Dict[Possibility, int]]
+    complement_counts: Optional[dict[Possibility, int]]
     # a mapping from class names to values
     # this is array metadata because labels might disappear during downsampling
     annotation_type: AnnotationType
 
     @model_validator(mode="after")
     def check_encoding(self: "AnnotationArrayAttrs"):
         assert set(self.annotation_type.encoding.keys()).issuperset((self.complement_counts.keys()))
@@ -304,15 +305,15 @@
     end_date: Optional[datetime.date]
         The calendar date when the crop was completed. Optional.
     duration_days: Optional[int]
         The number of days spent annotating the crop. Optional.
     protocol_uri: Optional[str]
         A URI pointing to a description of the annotation protocol used to produce the
         annotations. Optional.
-    class_names: list[str]
+    class_names: list[TName]
         The names of the classes that are annotated in this crop. Each element from
         `class_names` should also be the name of a Zarr group stored under the Zarr
         group that contains this metadata.
     """
 
     version: Literal["0.1.1"] = "0.1.1"
     name: Optional[str]
@@ -364,15 +365,15 @@
         under two outer dicts that define the namespace of this metadata,
         i.e. `{'cellmap': {'annotation': {...}}}`.
         See [AnnotationGroupAttrs][cellmap_schemas.annotation.AnnotationGroupAttrs] for
         details of the wrapped metadata.
     """
 
     attributes: CellmapWrapper[AnnotationWrapper[AnnotationGroupAttrs]]
-    members: Dict[str, AnnotationArray]
+    members: dict[str, AnnotationArray]
 
 
 class CropGroup(GroupSpec):
     """
     The specification of a crop group. Conventionally, a crop is a subset of a
     larger imaging volume that has been annotated by a human annotator. A crop may
     contain multiple semantic classes, which might be annotated via semantic
@@ -390,7 +391,40 @@
         A dict with keys that are strings and values that are instances of
         [AnnotationGroup][cellmap_schemas.annotation.AnnotationGroup].
 
     """
 
     attributes: CellmapWrapper[AnnotationWrapper[CropGroupAttrs]]
     members: Mapping[str, AnnotationGroup]
+
+    @classmethod
+    def from_zarr(cls, group: zarr.Group):
+        """
+        Generate a `CropGroup` from a `zarr.Group`. Sub-groups that do not pass validation as
+        `AnnotationGroup` will be ignored, as will sub-arrays.
+
+        Parameters
+        ----------
+        group : zarr.Group
+            A Zarr group that implements the `CropGroup` layout.
+
+        Returns
+        -------
+        CropGroup
+
+        """
+
+        untyped_group = GroupSpec[CellmapWrapper[AnnotationWrapper[CropGroupAttrs]], Any].from_zarr(
+            group
+        )
+        class_names = untyped_group.attributes.cellmap.annotation.class_names
+        keep = {}
+        for name in class_names:
+            try:
+                keep[name] = untyped_group.members[name]
+            except KeyError as e:
+                msg = (
+                    f"Expected to find a group named {name} in {group.store}://{group.name}. "
+                    "No group was found with that name."
+                )
+                raise ValueError(msg) from e
+        return cls(attributes=untyped_group.attributes, members=keep)
```

### Comparing `cellmap_schemas-0.4.0/src/cellmap_schemas/base.py` & `cellmap_schemas-0.5.0/src/cellmap_schemas/base.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.4.0/src/cellmap_schemas/cli.py` & `cellmap_schemas-0.5.0/src/cellmap_schemas/cli.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.4.0/src/cellmap_schemas/multiscale/cosem.py` & `cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/cosem.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.4.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py` & `cellmap_schemas-0.5.0/src/cellmap_schemas/multiscale/neuroglancer_n5.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.4.0/src/cellmap_schemas/n5_wrap.py` & `cellmap_schemas-0.5.0/src/cellmap_schemas/n5_wrap.py`

 * *Files identical despite different names*

### Comparing `cellmap_schemas-0.4.0/PKG-INFO` & `cellmap_schemas-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cellmap-schemas
-Version: 0.4.0
+Version: 0.5.0
 Summary: Schemas for data used by the Cellmap project team at Janelia Research Campus.
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydantic-zarr (>=0.5.2,<0.6.0)
+Requires-Dist: pydantic-zarr (>=0.7.0,<0.8.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: s3fs (>=2023.10.0,<2024.0.0)
 Description-Content-Type: text/markdown
 
 # cellmap-schemas
 Schemas for our data
```

