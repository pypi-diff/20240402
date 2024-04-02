# Comparing `tmp/valor-client-0.19.0.tar.gz` & `tmp/valor-client-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valor-client-0.19.0.tar", last modified: Wed Mar 27 20:54:42 2024, max compression
+gzip compressed data, was "valor-client-0.20.0.tar", last modified: Tue Apr  2 01:02:01 2024, max compression
```

## Comparing `valor-client-0.19.0.tar` & `valor-client-0.20.0.tar`

### file list

```diff
@@ -1,45 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:54:42.616757 valor-client-0.19.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-27 20:54:35.000000 valor-client-0.19.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-27 20:54:42.612756 valor-client-0.19.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-27 20:54:35.000000 valor-client-0.19.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 20:54:42.616757 valor-client-0.19.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-27 20:54:35.000000 valor-client-0.19.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:54:42.608756 valor-client-0.19.0/unit-tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:54:42.608756 valor-client-0.19.0/unit-tests/coretypes/
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/coretypes/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/coretypes/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/coretypes/test_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:54:42.608756 valor-client-0.19.0/unit-tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)    14092 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/schemas/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/schemas/test_evaluation_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/schemas/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/schemas/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/schemas/test_label.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/schemas/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-03-27 20:54:35.000000 valor-client-0.19.0/unit-tests/test_viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:54:42.612756 valor-client-0.19.0/valor/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    72104 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/metatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:54:42.612756 valor-client-0.19.0/valor/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16692 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/schemas/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/schemas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/schemas/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14221 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/schemas/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/schemas/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/schemas/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-03-27 20:54:35.000000 valor-client-0.19.0/valor/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 20:54:42.612756 valor-client-0.19.0/valor_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-03-27 20:54:42.000000 valor-client-0.19.0/valor_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-27 20:54:42.000000 valor-client-0.19.0/valor_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 20:54:42.000000 valor-client-0.19.0/valor_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-27 20:54:42.000000 valor-client-0.19.0/valor_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 20:54:42.000000 valor-client-0.19.0/valor_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 01:01:56.000000 valor-client-0.20.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-02 01:02:01.599599 valor-client-0.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-02 01:01:56.000000 valor-client-0.20.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:02:01.599599 valor-client-0.20.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 01:01:56.000000 valor-client-0.20.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/coretypes/
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/coretypes/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/coretypes/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/coretypes/test_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/schemas/test_evaluation_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/schemas/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/schemas/test_label.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/symbolic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/symbolic/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/collections/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/collections/test_static_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12326 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/collections/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.595599 valor-client-0.20.0/unit-tests/symbolic/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    14686 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/types/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28256 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/symbolic/types/test_symbolic_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-02 01:01:56.000000 valor-client-0.20.0/unit-tests/test_viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/valor/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53715 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/metatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/valor/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14596 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/valor/schemas/symbolic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/symbolic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25442 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/symbolic/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/symbolic/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46702 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/schemas/symbolic/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/type_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10632 2024-04-02 01:01:56.000000 valor-client-0.20.0/valor/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:02:01.599599 valor-client-0.20.0/valor_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 01:02:01.000000 valor-client-0.20.0/valor_client.egg-info/top_level.txt
```

### Comparing `valor-client-0.19.0/LICENSE` & `valor-client-0.20.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valor-client-0.19.0/PKG-INFO` & `valor-client-0.20.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.19.0
+Version: 0.20.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor-client-0.19.0/pyproject.toml` & `valor-client-0.20.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `valor-client-0.19.0/unit-tests/conftest.py` & `valor-client-0.20.0/unit-tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-from typing import List
+from typing import List, Tuple
 
 import numpy as np
 import pytest
 
-from valor import Label, schemas
+from valor import Label
+from valor.schemas import BoundingBox, BoundingPolygon, Raster
 
 
 @pytest.fixture
 def labels() -> List[Label]:
     return [
         Label(key="k1", value="v1"),
         Label(key="k2", value="v2"),
     ]
 
 
 @pytest.fixture
-def box_points() -> List[schemas.Point]:
+def box_points() -> List[Tuple[float, float]]:
     return [
-        schemas.Point(x=0, y=0),
-        schemas.Point(x=10, y=0),
-        schemas.Point(x=10, y=10),
-        schemas.Point(x=0, y=10),
+        (0, 0),
+        (10, 0),
+        (10, 10),
+        (0, 10),
+        (0, 0),
     ]
 
 
 @pytest.fixture
-def basic_polygon(box_points) -> schemas.BasicPolygon:
-    return schemas.BasicPolygon(points=box_points)
+def bbox() -> BoundingBox:
+    return BoundingBox.from_extrema(xmin=0, xmax=10, ymin=0, ymax=10)
 
 
 @pytest.fixture
-def bbox() -> schemas.BoundingBox:
-    return schemas.BoundingBox.from_extrema(xmin=0, xmax=10, ymin=0, ymax=10)
-
-
-@pytest.fixture
-def polygon(basic_polygon) -> schemas.Polygon:
-    return schemas.Polygon(boundary=basic_polygon)
+def polygon(box_points) -> BoundingPolygon:
+    return BoundingPolygon([box_points])
 
 
 @pytest.fixture
 def raster_raw_mask() -> np.ndarray:
     """
     Creates a 2d numpy of bools of shape:
     | T  F |
@@ -50,16 +47,16 @@
     zeros = np.zeros((10, 10))
     top = np.concatenate((ones, zeros), axis=1)
     bottom = np.concatenate((zeros, ones), axis=1)
     return np.concatenate((top, bottom), axis=0) == 1
 
 
 @pytest.fixture
-def raster(raster_raw_mask) -> schemas.Raster:
-    return schemas.Raster.from_numpy(raster_raw_mask)
+def raster(raster_raw_mask) -> Raster:
+    return Raster.from_numpy(raster_raw_mask)
 
 
 @pytest.fixture
 def metadata() -> dict:
     return {
         "a": 1234,
         "b": 1.234,
```

### Comparing `valor-client-0.19.0/unit-tests/coretypes/test_core.py` & `valor-client-0.20.0/unit-tests/coretypes/test_core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 
 import pytest
 
 from valor import Annotation, Datum, GroundTruth, Label, Prediction, enums
+from valor.schemas import Score
 
 
 def test_datum():
     Datum(uid="123")
     Datum(uid="123", metadata={})
     Datum(uid="123", metadata={"name": 1})
 
@@ -55,15 +56,15 @@
         labels=labels,
         metadata=metadata,
     )
 
     # test `__post_init__`
     with pytest.raises(ValueError) as e:
         Annotation(task_type="something", labels=labels)  # type: ignore
-    assert "is not a valid TaskType" in str(e)
+    assert "TaskType" in str(e)
     with pytest.raises(TypeError) as e:
         Annotation(
             task_type=enums.TaskType.OBJECT_DETECTION,
             labels=labels,
             bounding_box=polygon,
         )
     with pytest.raises(TypeError) as e:
@@ -86,15 +87,15 @@
         )
     with pytest.raises(TypeError) as e:
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION,
             labels=labels,
             metadata={1: 1},  # type: ignore
         )
-    with pytest.raises(TypeError) as e:
+    with pytest.raises(ValueError) as e:
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION,
             labels=labels,
             metadata={"test": None},  # type: ignore
         )
 
 
@@ -108,52 +109,52 @@
         task_type=enums.TaskType.CLASSIFICATION,
         labels=[l1, l2, l3],
     )
 
     # test `__post_init__`
     with pytest.raises(ValueError) as e:
         Annotation(task_type="soemthing", labels=[l1])  # type: ignore
-    assert "is not a valid TaskType" in str(e)
+    assert "TaskType" in str(e)
     with pytest.raises(TypeError) as e:
         Annotation(task_type=enums.TaskType.CLASSIFICATION, labels=l1)  # type: ignore
-    assert "List[valor.Label]" in str(e)
+    assert "List[Label]" in str(e)
     with pytest.raises(TypeError) as e:
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION, labels=[l1, l2, "label"]  # type: ignore
         )
-    assert "valor.Label" in str(e)
+    assert "Label" in str(e)
 
 
 def test_prediction_annotation():
     l1 = Label(key="test", value="value")
     l2 = Label(key="test", value="other")
     l3 = Label(key="other", value="value")
 
     s1 = copy.deepcopy(l1)
-    s1.score = 0.5
+    s1.score = Score(0.5)
     s2 = copy.deepcopy(l2)
-    s2.score = 0.5
+    s2.score = Score(0.5)
     s3 = copy.deepcopy(l3)
-    s3.score = 1.0
+    s3.score = Score(1.0)
 
     # valid
     Annotation(task_type=enums.TaskType.CLASSIFICATION, labels=[s1, s2, s3])
 
     # test `__post_init__`
     with pytest.raises(ValueError) as e:
         Annotation(task_type="something", labels=[s1, s2, s3])  # type: ignore
-    assert "is not a valid TaskType" in str(e)
+    assert "TaskType" in str(e)
     with pytest.raises(TypeError) as e:
         Annotation(task_type=enums.TaskType.CLASSIFICATION, labels=s1)  # type: ignore
-    assert "List[valor.Label]" in str(e)
+    assert "List[Label]" in str(e)
     with pytest.raises(TypeError) as e:
         Annotation(
             task_type=enums.TaskType.CLASSIFICATION, labels=[s1, s2, "label"]  # type: ignore
         )
-    assert "valor.Label" in str(e)
+    assert "Label" in str(e)
 
 
 def test_groundtruth():
     label = Label(key="test", value="value")
     datum = Datum(uid="somefile")
     gts = [
         Annotation(task_type=enums.TaskType.CLASSIFICATION, labels=[label]),
@@ -168,27 +169,27 @@
 
     # test `__post_init__`
     with pytest.raises(TypeError) as e:
         GroundTruth(
             datum="datum",  # type: ignore
             annotations=gts,
         )
-    assert "valor.Datum" in str(e)
+    assert "Datum" in str(e)
     with pytest.raises(TypeError) as e:
         GroundTruth(
             datum=datum,
             annotations=gts[0],  # type: ignore
         )
-    assert "List[valor.Annotation]" in str(e)
+    assert "List[Annotation]" in str(e)
     with pytest.raises(TypeError) as e:
         GroundTruth(
             datum=datum,
             annotations=[gts[0], gts[1], "annotation"],  # type: ignore
         )
-    assert "valor.Annotation" in str(e)
+    assert "Annotation" in str(e)
 
     # test equalities
     with pytest.raises(TypeError):
         _ = (
             GroundTruth(
                 datum=datum,
                 annotations=gts,
@@ -218,50 +219,51 @@
 
     # valid
     Prediction(datum=datum, annotations=pds)
 
     string = str(Prediction(datum=datum, annotations=pds))
     assert (
         string
-        == '{\n    "datum": {\n        "uid": "somefile",\n        "metadata": {}\n    },\n    "annotations": [\n        {\n            "task_type": "classification",\n            "labels": [\n                {\n                    "key": "test",\n                    "value": "value",\n                    "score": 1.0\n                }\n            ],\n            "metadata": {},\n            "bounding_box": null,\n            "polygon": null,\n            "raster": null,\n            "embedding": null\n        },\n        {\n            "task_type": "classification",\n            "labels": [\n                {\n                    "key": "test",\n                    "value": "value",\n                    "score": 1.0\n                }\n            ],\n            "metadata": {},\n            "bounding_box": null,\n            "polygon": null,\n            "raster": null,\n            "embedding": null\n        }\n    ]\n}'
+        == "{'datum': {'uid': 'somefile', 'metadata': {}}, 'annotations': [{'task_type': 'classification', 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'metadata': {}, 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}, {'task_type': 'classification', 'labels': [{'key': 'test', 'value': 'value', 'score': 1.0}], 'metadata': {}, 'bounding_box': None, 'polygon': None, 'raster': None, 'embedding': None}]}"
     )
     assert "dataset_name" not in string
 
     # test `__post_init__`
     with pytest.raises(TypeError) as e:
-        Prediction(datum="datum", annotations=pds)  # type: ignore
-    assert "valor.Datum" in str(e)
+        Prediction.create(datum="datum", annotations=pds)  # type: ignore
+    assert "Datum" in str(e)
     with pytest.raises(TypeError) as e:
-        Prediction(
+        Prediction.create(
             datum=datum,
             annotations=pds[0],  # type: ignore
         )
-    assert "List[valor.Annotation]" in str(e)
+    assert "List[Annotation]" in str(e)
+
     with pytest.raises(TypeError) as e:
-        Prediction(
+        Prediction.create(
             datum=datum,
             annotations=[pds[0], pds[1], "annotation"],  # type: ignore
         )
-    assert "valor.Annotation" in str(e)
+    assert "Annotation" in str(e)
 
     with pytest.raises(ValueError) as e:
-        Prediction(
+        Prediction.create(
             datum=datum,
             annotations=[
-                Annotation(
+                Annotation.create(
                     task_type=enums.TaskType.CLASSIFICATION,
                     labels=[
-                        Label(key="test", value="value", score=0.8),
-                        Label(key="test", value="other", score=0.1),
+                        Label.create(key="test", value="value", score=0.8),
+                        Label.create(key="test", value="other", score=0.1),
                     ],
                 )
             ],
         )
     assert "for label key test got scores summing to 0.9" in str(e)
 
     # test equalities
     with pytest.raises(TypeError):
-        _ = Prediction(datum=datum, annotations=pds) == 1
+        _ = Prediction.create(datum=datum, annotations=pds) == 1
 
-    assert Prediction(datum=datum, annotations=pds) == Prediction(
+    assert Prediction.create(
         datum=datum, annotations=pds
-    )
+    ) == Prediction.create(datum=datum, annotations=pds)
```

### Comparing `valor-client-0.19.0/unit-tests/coretypes/test_evaluation.py` & `valor-client-0.20.0/unit-tests/coretypes/test_evaluation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from typing import Optional
 from unittest.mock import Mock
 
 import pytest
 
 from valor import Evaluation, enums, schemas
 
@@ -47,14 +48,17 @@
                 "d",
                 parameters={"x": 0.123, "y": 0.987},
                 value=0.3,
                 label={"key": "k1", "value": "v1"},
             ),
         ],
         confusion_matrices=[],
+        created_at=datetime.datetime(
+            year=2024, month=1, day=1, microsecond=1
+        ).strftime("%Y-%m-%dT%H:%M:%S.%fZ"),
         connection=Mock(),
     ).to_dataframe()
 
     df_str = """                                        value
     evaluation                              1
     type parameters               label
     a    "n/a"                    n/a        0.99
```

### Comparing `valor-client-0.19.0/unit-tests/coretypes/test_filtering.py` & `valor-client-0.20.0/unit-tests/coretypes/test_filtering.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,111 @@
 import datetime
 
 import pytest
 
-from valor import Annotation, Constraint, Dataset, Filter, Label, Model
+from valor import Annotation, Dataset, Filter, Label, Model
 from valor.coretypes import _format_filter
+from valor.schemas import Polygon
+from valor.schemas.filters import Constraint
 
 
 @pytest.fixture
-def geojson() -> dict:
+def polygon() -> Polygon:
     coordinates = [
         [
-            [125.2750725, 38.760525],
-            [125.3902365, 38.775069],
-            [125.5054005, 38.789613],
-            [125.5051935, 38.71402425],
-            [125.5049865, 38.6384355],
-            [125.3902005, 38.6244225],
-            [125.2754145, 38.6104095],
-            [125.2752435, 38.68546725],
-            [125.2750725, 38.760525],
+            (125.2750725, 38.760525),
+            (125.3902365, 38.775069),
+            (125.5054005, 38.789613),
+            (125.5051935, 38.71402425),
+            (125.5049865, 38.6384355),
+            (125.3902005, 38.6244225),
+            (125.2754145, 38.6104095),
+            (125.2752435, 38.68546725),
+            (125.2750725, 38.760525),
         ]
     ]
-    return {"type": "Polygon", "coordinates": coordinates}
+    return Polygon(coordinates)
 
 
-def test__format_filter(geojson):
+@pytest.fixture
+def geojson(polygon: Polygon):
+    return {"type": "Polygon", "coordinates": polygon.get_value()}
+
+
+def test__format_filter(geojson, polygon):
 
     filter_object = Filter(
         dataset_names=["a", "b", "c"],
         model_names=["x", "y", "z"],
         label_scores=[Constraint(value=0.75, operator=">")],
         polygon_area=[
             Constraint(value=1000, operator=">"),
             Constraint(value=5000, operator="<"),
         ],
+        raster_area=[
+            Constraint(value=100, operator=">"),
+            Constraint(value=500, operator="<"),
+        ],
         dataset_metadata={
             "some_str": [Constraint(value="foobar", operator="==")],
             "some_float": [Constraint(value=0.123, operator=">=")],
             "some_datetime": [
                 Constraint(
                     value={
-                        "duration": str(
-                            datetime.timedelta(days=1).total_seconds()
-                        )
+                        "duration": datetime.timedelta(days=1).total_seconds()
                     },
                     operator=">",
                 )
             ],
             "some_geospatial": [
                 Constraint(
                     value=geojson,
                     operator="intersect",
                 )
             ],
         },
     )
 
-    filter_from_constraints = _format_filter(
+    filter_from_constraints = Filter.create(
         [
-            Dataset.name.in_(["a", "b", "c"]),  # type: ignore - filter type error
-            Model.name.in_(["x", "y", "z"]),  # type: ignore - filter type error
-            Label.score > 0.75,  # type: ignore - filter type error
-            Annotation.polygon.area > 1000,  # type: ignore - filter type error
-            Annotation.polygon.area < 5000,  # type: ignore - filter type error
-            Dataset.metadata["some_str"] == "foobar",  # type: ignore - filter type error
-            Dataset.metadata["some_float"] >= 0.123,  # type: ignore - filter type error
-            Dataset.metadata["some_datetime"] > datetime.timedelta(days=1),  # type: ignore - filter type error
-            Dataset.metadata["some_geospatial"].intersect(geojson),  # type: ignore - filter type error
+            Dataset.name.in_(["a", "b", "c"]),
+            (Model.name == "x") | Model.name.in_(["y", "z"]),
+            Label.score > 0.75,
+            Annotation.polygon.area > 1000,
+            Annotation.polygon.area < 5000,
+            (Annotation.raster.area > 100) & (Annotation.raster.area < 500),
+            Dataset.metadata["some_str"] == "foobar",
+            Dataset.metadata["some_float"] >= 0.123,
+            Dataset.metadata["some_datetime"] > datetime.timedelta(days=1),
+            Dataset.metadata["some_geospatial"].intersects(polygon),
         ]
     )
 
     filter_from_dictionary = _format_filter(
         {
             "dataset_names": ["a", "b", "c"],
             "model_names": ["x", "y", "z"],
             "label_scores": [{"value": 0.75, "operator": ">"}],
             "polygon_area": [
                 {"value": 1000, "operator": ">"},
                 {"value": 5000, "operator": "<"},
             ],
+            "raster_area": [
+                {"value": 100, "operator": ">"},
+                {"value": 500, "operator": "<"},
+            ],
             "dataset_metadata": {
                 "some_str": [{"value": "foobar", "operator": "=="}],
                 "some_float": [{"value": 0.123, "operator": ">="}],
                 "some_datetime": [
                     {
                         "value": {
-                            "duration": str(
-                                datetime.timedelta(days=1).total_seconds()
-                            )
+                            "duration": datetime.timedelta(
+                                days=1
+                            ).total_seconds()
                         },
                         "operator": ">",
                     }
                 ],
                 "some_geospatial": [
                     {
                         "value": geojson,
```

### Comparing `valor-client-0.19.0/unit-tests/test_client.py` & `valor-client-0.20.0/unit-tests/test_client.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.19.0/unit-tests/test_viz.py` & `valor-client-0.20.0/unit-tests/test_viz.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,176 +1,186 @@
 import numpy as np
 import PIL.Image
 import pytest
 
 from valor import Annotation, GroundTruth, Label
 from valor.enums import TaskType
 from valor.metatypes import ImageMetadata
-from valor.schemas import BasicPolygon, MultiPolygon, Point, Polygon, Raster
+from valor.schemas import BoundingPolygon, MultiPolygon, Polygon, Raster
 from valor.viz import (
     _polygons_to_binary_mask,
     create_combined_segmentation_mask,
     draw_detections_on_image,
 )
 
 
 @pytest.fixture
-def bounding_poly() -> BasicPolygon:
-    return BasicPolygon(
-        points=[
-            Point(100, 100),
-            Point(200, 100),
-            Point(200, 200),
-            Point(100, 200),
+def bounding_poly() -> Polygon:
+    return Polygon(
+        [
+            [
+                (100, 100),
+                (200, 100),
+                (200, 200),
+                (100, 200),
+                (100, 100),
+            ]
         ]
     )
 
 
 @pytest.fixture
-def poly1(bounding_poly: BasicPolygon) -> Polygon:
+def poly1(bounding_poly: Polygon) -> Polygon:
     return Polygon(
-        boundary=bounding_poly,
-        holes=[
-            BasicPolygon(
-                points=[
-                    Point(150, 120),
-                    Point(180, 120),
-                    Point(180, 140),
-                    Point(150, 140),
-                ]
-            )
-        ],
+        [
+            bounding_poly.get_value()[0],
+            [
+                (150, 120),
+                (180, 120),
+                (180, 140),
+                (150, 140),
+                (150, 120),
+            ],
+        ]
     )
 
 
 def test__polygons_to_binary_mask(poly1):
     poly2 = Polygon(
-        boundary=BasicPolygon(
-            points=[
-                Point(10, 15),
-                Point(20, 15),
-                Point(20, 20),
-                Point(10, 20),
+        [
+            [
+                (10, 15),
+                (20, 15),
+                (20, 20),
+                (10, 20),
+                (10, 15),
             ]
-        )
+        ]
     )
 
     mask = _polygons_to_binary_mask([poly1, poly2], 500, 600)
 
     area_poly1 = (200 - 100 + 1) * (200 - 100 + 1) - (180 - 150 + 1) * (
         140 - 120 + 1
     )
 
     area_poly2 = (20 - 10 + 1) * (20 - 15 + 1)
 
     assert mask.sum() == area_poly1 + area_poly2
 
 
 def test_create_combined_segmentation_mask(poly1: Polygon):
-    with pytest.raises(ValueError) as exc_info:
-        create_combined_segmentation_mask(
-            [],
-            label_key="",
-            task_type=TaskType.OBJECT_DETECTION,
-        )
-    assert "cannot be empty" in str(exc_info)
-
-    image = ImageMetadata(uid="uid", height=200, width=200).to_datum()
+    image = ImageMetadata.create(uid="uid", height=200, width=200).datum
 
     gt1 = GroundTruth(
         datum=image,
         annotations=[
             Annotation(
                 task_type=TaskType.OBJECT_DETECTION,
                 labels=[
                     Label(key="k1", value="v1"),
                     Label(key="k2", value="v2"),
                     Label(key="k3", value="v3"),
                 ],
                 raster=Raster.from_geometry(
-                    MultiPolygon(polygons=[poly1]),
-                    height=200,
-                    width=200,
+                    MultiPolygon([poly1.get_value()]),
+                    height=2,
+                    width=2,
+                ),
+            ),
+            Annotation(
+                task_type=TaskType.SEMANTIC_SEGMENTATION,
+                labels=[
+                    Label(key="k1", value="v1"),
+                    Label(key="k2", value="v3"),
+                ],
+                raster=Raster.from_numpy(
+                    np.array([[True, False], [False, True]]),
                 ),
             ),
         ],
     )
 
-    gt2 = GroundTruth(
+    gt_with_size_mismatch = GroundTruth(
         datum=image,
         annotations=[
             Annotation(
+                task_type=TaskType.OBJECT_DETECTION,
+                labels=[
+                    Label(key="k1", value="v1"),
+                    Label(key="k2", value="v2"),
+                    Label(key="k3", value="v3"),
+                ],
+                raster=Raster.from_geometry(
+                    MultiPolygon([poly1.get_value()]),
+                    height=20,
+                    width=20,
+                ),
+            ),
+            Annotation(
                 task_type=TaskType.SEMANTIC_SEGMENTATION,
                 labels=[
                     Label(key="k1", value="v1"),
                     Label(key="k2", value="v3"),
                 ],
                 raster=Raster.from_numpy(
                     np.array([[True, False], [False, True]]),
                 ),
-            )
+            ),
         ],
     )
 
-    gts = [gt1, gt2]
+    # test that a size mistmatch between rasters is caught
+    with pytest.raises(ValueError) as exc_info:
+        create_combined_segmentation_mask(
+            gt_with_size_mismatch,
+            label_key="k2",
+            task_type=TaskType.SEMANTIC_SEGMENTATION,
+        )
+    assert "(20, 20) != (2, 2)" in str(exc_info)
 
     # check get an error since "k3" isn't a label key in seg2
     with pytest.raises(RuntimeError) as exc_info:
         create_combined_segmentation_mask(
-            [gts[1]],
+            gt1,
             label_key="k3",
             task_type=TaskType.SEMANTIC_SEGMENTATION,
         )
     assert "doesn't have a label" in str(exc_info)
 
     # should have one distinct (non-black) color
-    combined_mask, _ = create_combined_segmentation_mask(
-        gts,
+    combined_mask, legend = create_combined_segmentation_mask(
+        gt1,
         label_key="k1",
         task_type=TaskType.SEMANTIC_SEGMENTATION,
     )
     combined_mask = np.array(combined_mask)
     # check that we get two unique RGB values (black and one color for label value "v1")
-    unique_rgb = np.unique(combined_mask.reshape(-1, 3), axis=0)
-    assert unique_rgb.shape == (2, 3)
+    assert combined_mask.shape == (2, 2, 3)
+    assert len(legend) == 1  # background color 'black' is not counted
 
     # should have two distinct (non-black) color
-    combined_mask, _ = create_combined_segmentation_mask(gts, label_key="k2")
+    combined_mask, legend = create_combined_segmentation_mask(
+        gt1, label_key="k2"
+    )
     combined_mask = np.array(combined_mask)
-    # check that we get two unique RGB values (black and one color for label value "v1")
-    unique_rgb = np.unique(combined_mask.reshape(-1, 3), axis=0)
-    assert unique_rgb.shape == (3, 3)
-
-    with pytest.raises(RuntimeError) as exc_info:
-        create_combined_segmentation_mask(
-            gts
-            + [
-                GroundTruth(
-                    datum=ImageMetadata(
-                        "different uid", height=10, width=100
-                    ).to_datum(),
-                    annotations=gts[0].annotations,
-                )
-            ],
-            "",
-        )
-    assert "belong to the same image" in str(exc_info)
+    # check that we get three unique RGB values (black and two colors for label values "v2" and "v3")
+    assert combined_mask.shape == (2, 2, 3)
+    assert len(legend) == 2  # background color 'black' is not counted
 
 
-def test_draw_detections_on_image(bounding_poly: BasicPolygon):
+def test_draw_detections_on_image(bounding_poly: Polygon):
     detections = [
         GroundTruth(
-            datum=ImageMetadata("test", 300, 300).to_datum(),
+            datum=ImageMetadata.create("test", 300, 300).datum,
             annotations=[
                 Annotation(
                     task_type=TaskType.OBJECT_DETECTION,
-                    labels=[Label("k", "v")],
-                    polygon=Polygon(
-                        boundary=bounding_poly,
-                    ),
+                    labels=[Label(key="k", value="v")],
+                    polygon=BoundingPolygon(bounding_poly.get_value()),
                 )
             ],
         ),
     ]
     img = PIL.Image.new("RGB", (300, 300))
 
     img = draw_detections_on_image(detections, img)
```

### Comparing `valor-client-0.19.0/valor/__init__.py` & `valor-client-0.20.0/valor/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,34 +8,30 @@
 try:
     __version__ = importlib_metadata.version("valor")
 except importlib_metadata.PackageNotFoundError:
     __version__ = ""
 
 from .client import ClientConnection, connect
 from .coretypes import (
-    Annotation,
     Client,
     Dataset,
-    Datum,
     Evaluation,
     GroundTruth,
-    Label,
     Model,
     Prediction,
 )
-from .schemas import Constraint, Filter
+from .schemas import Annotation, Datum, Filter, Label
 
 __all__ = [
     "connect",
     "Client",
     "ClientConnection",
-    "Label",
     "Evaluation",
     "Dataset",
     "Model",
     "Datum",
     "Annotation",
     "GroundTruth",
     "Prediction",
     "Filter",
-    "Constraint",
+    "Label",
 ]
```

### Comparing `valor-client-0.19.0/valor/client.py` & `valor-client-0.20.0/valor/client.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.19.0/valor/coretypes.py` & `valor-client-0.20.0/valor/coretypes.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,41 +3,31 @@
 import datetime
 import json
 import time
 import warnings
 from dataclasses import asdict, dataclass
 from typing import Dict, List, Optional, Tuple, Union
 
-import numpy as np
-
 from valor.client import ClientConnection, connect, get_connection
 from valor.enums import AnnotationType, EvaluationStatus, TableStatus, TaskType
 from valor.exceptions import ClientException
-from valor.schemas.constraints import BinaryExpression
-from valor.schemas.evaluation import EvaluationParameters, EvaluationRequest
-from valor.schemas.filters import Filter
-from valor.schemas.geometry import BoundingBox, Polygon, Raster
-from valor.schemas.metadata import (
-    MetadataType,
-    dump_metadata,
-    load_metadata,
-    validate_metadata,
-)
-from valor.schemas.properties import (
-    DictionaryProperty,
-    GeometryProperty,
-    LabelProperty,
-    NumericProperty,
-    StringProperty,
+from valor.schemas import (
+    Annotation,
+    Datum,
+    Dictionary,
+    EvaluationParameters,
+    EvaluationRequest,
+    Filter,
+    Label,
 )
-from valor.typing import is_float
+from valor.schemas import List as SymbolicList
+from valor.schemas import StaticCollection, String
+from valor.schemas.compatibility import decode_api_format, encode_api_format
 
-FilterType = Union[
-    Filter, List[Union[BinaryExpression, List[BinaryExpression]]], dict
-]
+FilterType = Union[list, dict, Filter]  # TODO - Remove this
 
 
 def _format_filter(filter_by: Optional[FilterType]) -> Filter:
     """
     Formats the various filter or constraint representations into a 'schemas.Filter' object.
 
     Parameters
@@ -57,746 +47,161 @@
         return Filter.create(filter_by)
     elif isinstance(filter_by, dict):
         return Filter(**filter_by)
     else:
         raise TypeError
 
 
-class Label:
+class GroundTruth(StaticCollection):
     """
-    An object for labeling datasets, models, and annotations.
-
-    Parameters
-    ----------
-    key : str
-        The class key of the label.
-    value : str
-        The class value of the label.
-    score : float, optional
-        The score associated with the label (if applicable).
-
-    Attributes
-    ----------
-    filter_by : filter_factory
-        Declarative mappers used to create filters.
-    """
-
-    value = StringProperty("label_values")
-    key = StringProperty("label_keys")
-    score = NumericProperty("label_scores")
-
-    def __init__(
-        self,
-        key: str,
-        value: str,
-        score: Union[float, np.floating, None] = None,
-    ):
-        if not isinstance(key, str):
-            raise TypeError("Attribute `key` should have type `str`.")
-        if not isinstance(value, str):
-            raise TypeError("Attribute `value` should have type `str`.")
-        if score is not None:
-            if not is_float(score):
-                raise TypeError(
-                    "Attribute `score` should be a floating-point number or `None`."
-                )
-
-        self.key = key
-        self.value = value
-        self.score = score
-
-    def __str__(self) -> str:
-        """Dumps the object into a JSON formatted string."""
-        return json.dumps(self.to_dict(), indent=4)
-
-    def __repr__(self) -> str:
-        return str(self.tuple())
-
-    def to_dict(self) -> Dict[str, Union[str, float, np.floating, None]]:
-        """
-        Defines how a `valor.Label` object is serialized into a dictionary.
-
-        Returns
-        ----------
-        dict
-            A dictionary describing a label.
-        """
-        return {
-            "key": self.key,
-            "value": self.value,
-            "score": self.score,
-        }
-
-    @classmethod
-    def from_dict(cls, resp) -> Label:
-        """
-        Construct a label from a dictionary.
-
-        Parameters
-        ----------
-        resp : dict
-            The dictionary containing a label.
-
-        Returns
-        -------
-        valor.Label
-        """
-        return cls(**resp)
-
-    def __eq__(self, other) -> bool:
-        """
-        Defines how `Labels` are compared to one another.
-
-        Parameters
-        ----------
-        other : Label
-            The object to compare with the `Label`.
-
-        Returns
-        ----------
-        boolean
-            A boolean describing whether the two objects are equal.
-        """
-        # type mismatch
-        if type(other) is not type(self):
-            return False
-
-        # k,v mismatch
-        if self.key != other.key or self.value != other.value:
-            return False
-
-        # score is None
-        if self.score is None or other.score is None:
-            return (other.score is None) == (self.score is None)
-
-        # scores not equal
-        if is_float(self.score) and is_float(other.score):
-            return bool(np.isclose(self.score, other.score))
-
-        return False
-
-    def __hash__(self) -> int:
-        """
-        Defines how a `Label` is hashed.
-
-        Returns
-        ----------
-        int
-            The hashed 'Label`.
-        """
-        return hash(f"key:{self.key},value:{self.value},score:{self.score}")
-
-    def tuple(self) -> Tuple[str, str, Union[float, np.floating, None]]:
-        """
-        Defines how the `Label` is turned into a tuple.
-
-        Returns
-        ----------
-        tuple
-            A tuple of the `Label's` arguments.
-        """
-        return (self.key, self.value, self.score)
-
-
-class Annotation:
-    """
-    A class used to annotate `GroundTruths` and `Predictions`.
-
-    Parameters
-    ----------
-    task_type: TaskType
-        The task type associated with the `Annotation`.
-    labels: List[Label], optional
-        A list of labels to use for the `Annotation`.
-    metadata: Dict[str, Union[int, float, str, bool, datetime.datetime, datetime.date, datetime.time]]
-        A dictionary of metadata that describes the `Annotation`.
-    bounding_box: BoundingBox, optional
-        A bounding box to assign to the `Annotation`.
-    polygon: Polygon, optional
-        A polygon to assign to the `Annotation`.
-    raster: Raster, optional
-        A raster to assign to the `Annotation`.
-    embedding: List[float], optional
-        An embedding, described by a list of values with type float and a maximum length of 16,000.
+    An object describing a ground truth (e.g., a human-drawn bounding box on an image).
 
     Attributes
     ----------
-    geometric_area : float
-        The area of the annotation.
+    datum : Datum
+        The datum associated with the groundtruth.
+    annotations : List[Annotation]
+        The list of annotations associated with the groundtruth.
 
     Examples
     --------
-
-    Classification
-    >>> Annotation(
-    ...     task_type=TaskType.CLASSIFICATION,
-    ...     labels=[
-    ...         Label(key="class", value="dog"),
-    ...         Label(key="category", value="animal"),
+    >>> GroundTruth(
+    ...     datum=Datum(uid="uid1"),
+    ...     annotations=[
+    ...         Annotation(
+    ...             task_type=TaskType.CLASSIFICATION,
+    ...             labels=[Label(key="k1", value="v1")],
+    ...         )
     ...     ]
     ... )
-
-    Object-Detection BoundingBox
-    >>> annotation = Annotation(
-    ...     task_type=TaskType.OBJECT_DETECTION,
-    ...     labels=[Label(key="k1", value="v1")],
-    ...     bounding_box=box2,
-    ... )
-
-    Object-Detection Polygon
-    >>> annotation = Annotation(
-    ...     task_type=TaskType.OBJECT_DETECTION,
-    ...     labels=[Label(key="k1", value="v1")],
-    ...     polygon=polygon1,
-    ... )
-
-    Object-Detection Raster
-    >>> annotation = Annotation(
-    ...     task_type=TaskType.OBJECT_DETECTION,
-    ...     labels=[Label(key="k1", value="v1")],
-    ...     raster=raster1,
-    ... )
-
-    Semantic-Segmentation Raster
-    >>> annotation = Annotation(
-    ...     task_type=TaskType.SEMANTIC_SEGMENTATION,
-    ...     labels=[Label(key="k1", value="v1")],
-    ...     raster=raster1,
-    ... )
-
-    Defining all supported annotation types for a given `task_type` is allowed!
-    >>> Annotation(
-    ...     task_type=TaskType.OBJECT_DETECTION,
-    ...     labels=[Label(key="k1", value="v1")],
-    ...     bounding_box=box1,
-    ...     polygon=polygon1,
-    ...     raster=raster1,
-    ... )
     """
 
-    task_type = StringProperty("task_types")
-    labels = LabelProperty("labels")
-    metadata = DictionaryProperty("annotation_metadata")
-    bounding_box = GeometryProperty("bounding_box")
-    polygon = GeometryProperty("polygon")
-    raster = GeometryProperty("raster")
-
-    def __init__(
-        self,
-        task_type: TaskType,
-        labels: Optional[List[Label]] = None,
-        metadata: Optional[MetadataType] = None,
-        bounding_box: Optional[BoundingBox] = None,
-        polygon: Optional[Polygon] = None,
-        raster: Optional[Raster] = None,
-        embedding: Optional[List[float]] = None,
-    ):
-        self.task_type = TaskType(task_type)
-        self.labels = labels if labels else []
-        self.metadata = metadata if metadata else {}
-        self.bounding_box = bounding_box
-        self.polygon = polygon
-        self.raster = raster
-        self.embedding = embedding
-        self._validate()
-
-    def _validate(self):
-        """
-        Validates the parameters used to create an `Annotation` object.
-        """
-        # labels
-        if not isinstance(self.labels, list):
-            raise TypeError(
-                "Attribute `labels` should have type `List[valor.Label]`."
-            )
-        for idx, label in enumerate(self.labels):
-            if not isinstance(label, Label):
-                raise TypeError(
-                    f"Attribute `labels[{idx}]` should have type `valor.Label`."
-                )
-
-        # bounding box
-        if self.bounding_box is not None:
-            if not isinstance(self.bounding_box, BoundingBox):
-                raise TypeError(
-                    "Attribute `bounding_box` should have type `valor.schemas.BoundingBox`."
-                )
-
-        # polygon
-        if self.polygon is not None:
-            if not isinstance(self.polygon, Polygon):
-                raise TypeError(
-                    "Attribute `polygon` should have type `valor.schemas.Polygon`."
-                )
-
-        # raster
-        if self.raster is not None:
-            if not isinstance(self.raster, Raster):
-                raise TypeError(
-                    "Attribute `raster` should have type `valor.schemas.Raster`."
-                )
-
-        # embedding
-        if self.embedding is not None:
-            if not isinstance(self.embedding, list):
-                raise TypeError(
-                    "Attribute `embedding` should have type `List[float]`."
-                )
-            for idx, embedding in enumerate(self.embedding):
-                if not isinstance(embedding, (int, float, np.floating)):
-                    raise TypeError(
-                        f"Attribute `embedding[{idx}]` should have type `float`, received element with type `{type(embedding)}`."
-                    )
-
-        # metadata
-        if not isinstance(self.metadata, dict):
-            raise TypeError("Attribute `metadata` should have type `dict`.")
-        validate_metadata(self.metadata)
+    datum: Datum = Datum.symbolic(owner="groundtruth", name="datum")
+    annotations: SymbolicList[Annotation] = SymbolicList[Annotation].symbolic(
+        owner="groundtruth", name="annotations"
+    )
 
     @classmethod
-    def from_dict(cls, resp: dict) -> Annotation:
-        """
-        Construct an annotation from a dictionary.
-
-        Parameters
-        ----------
-        resp : dict
-            The dictionary containing an annotation.
-
-        Returns
-        -------
-        valor.Annotation
-        """
-
-        task_type = TaskType(resp["task_type"])
-        labels = [Label.from_dict(label) for label in resp["labels"]]
-        metadata = load_metadata(resp["metadata"])
-
-        bounding_box = None
-        polygon = None
-        raster = None
-        embedding = None
-
-        if "bounding_box" in resp:
-            bounding_box = (
-                BoundingBox(**resp["bounding_box"])
-                if resp["bounding_box"]
-                else None
-            )
-        if "polygon" in resp:
-            polygon = Polygon(**resp["polygon"]) if resp["polygon"] else None
-        if "raster" in resp:
-            raster = Raster(**resp["raster"]) if resp["raster"] else None
-        if "embedding" in resp:
-            embedding = resp["embedding"]
-
-        return cls(
-            task_type=task_type,
-            labels=labels,
-            metadata=metadata,
-            bounding_box=bounding_box,
-            polygon=polygon,
-            raster=raster,
-            embedding=embedding,
-        )
-
-    def to_dict(self) -> dict:
-        """
-        Defines how a `valor.Annotation` object is serialized into a dictionary.
-
-        Returns
-        -------
-        dict
-            A dictionary describing an annotation.
-        """
-        return {
-            "task_type": self.task_type.value,
-            "labels": [label.to_dict() for label in self.labels],
-            "metadata": dump_metadata(self.metadata),
-            "bounding_box": (
-                asdict(self.bounding_box) if self.bounding_box else None
-            ),
-            "polygon": asdict(self.polygon) if self.polygon else None,
-            "raster": asdict(self.raster) if self.raster else None,
-            "embedding": self.embedding if self.embedding else None,
-        }
-
-    def __str__(self) -> str:
-        """Dumps the object into a JSON formatted string."""
-        return json.dumps(self.to_dict(), indent=4)
-
-    def __eq__(self, other) -> bool:
-        """
-        Defines how `Annotations` are compared to one another.
-
-        Parameters
-        ----------
-        other : Annotation
-            The object to compare with the `Annotation`.
-
-        Returns
-        ----------
-        boolean
-            A boolean describing whether the two objects are equal.
-        """
-        if not isinstance(other, Annotation):
-            raise TypeError(
-                f"Expected type `{type(Annotation)}`, got `{other}`"
-            )
-        return self.to_dict() == other.to_dict()
-
-
-class Datum:
-    """
-    A class used to store datum about `GroundTruths` and `Predictions`.
-
-    Parameters
-    ----------
-    uid : str
-        The UID of the `Datum`.
-    metadata : dict
-        A dictionary of metadata that describes the `Datum`.
-    """
-
-    uid = StringProperty("datum_uids")
-    metadata = DictionaryProperty("datum_metadata")
-
-    def __init__(
-        self,
-        uid: str,
-        metadata: Optional[MetadataType] = None,
+    def create(
+        cls,
+        datum: Datum,
+        annotations: List[Annotation],
+        **_,
     ):
-        self.uid = uid
-        self.metadata = metadata if metadata else {}
-
-        if not isinstance(self.uid, str):
-            raise TypeError("Attribute `uid` should have type `str`.")
-        validate_metadata(self.metadata)
-
-    def to_dict(self, dataset_name: Optional[str] = None) -> dict:
-        """
-        Defines how a `valor.Datum` object is serialized into a dictionary.
-
-        Returns
-        ----------
-        dict
-            A dictionary describing a datum.
         """
-        return {
-            "dataset_name": dataset_name,
-            "uid": self.uid,
-            "metadata": dump_metadata(self.metadata),
-        }
-
-    @classmethod
-    def from_dict(cls, resp: dict) -> Datum:
-        """
-        Construct a datum from a dictionary.
+        Creates a ground truth.
 
         Parameters
         ----------
-        resp : dict
-            The dictionary containing a datum.
-
-        Returns
-        -------
-        valor.Datum
-        """
-        resp.pop("dataset_name", None)
-        resp["metadata"] = load_metadata(resp["metadata"])
-        return cls(**resp)
-
-    def __str__(self) -> str:
-        """Dumps the object into a JSON formatted string."""
-        objdict = self.to_dict(dataset_name=None)
-        objdict.pop("dataset_name")
-        return json.dumps(objdict, indent=4)
-
-    def __eq__(self, other) -> bool:
+        datum : Datum
+            The `Datum` associated with the `GroundTruth`.
+        annotations : List[Annotation]
+            The list of `Annotations` associated with the `GroundTruth`.
         """
-        Defines how `Datums` are compared to one another.
-
-        Parameters
-        ----------
-        other : Datum
-            The object to compare with the `Datum`.
+        return cls.definite(
+            datum=datum,
+            annotations=annotations,
+        )
 
-        Returns
-        ----------
-        bool
-            A boolean describing whether the two objects are equal.
-        """
-        if not isinstance(other, Datum):
-            raise TypeError(f"Expected type `{type(Datum)}`, got `{other}`")
-        return self.to_dict() == other.to_dict()
+    def __post_init__(self):
+        for annotation in self.annotations:
+            for label in annotation.labels:
+                if label.score.get_value() is not None:
+                    raise ValueError(
+                        "GroundTruth labels should not have scores."
+                    )
 
 
-class GroundTruth:
+class Prediction(StaticCollection):
     """
-    An object describing a ground truth (e.g., a human-drawn bounding box on an image).
+    An object describing a prediction (e.g., a machine-drawn bounding box on an image).
 
-    Parameters
+    Attributes
     ----------
     datum : Datum
-        The `Datum` associated with the `GroundTruth`.
+        The datum associated with the prediction.
     annotations : List[Annotation]
-        The list of `Annotations` associated with the `GroundTruth`.
-    """
+        The list of annotations associated with the prediction.
 
-    def __init__(self, datum: Datum, annotations: List[Annotation]):
-        self.datum = datum
-        self.annotations = annotations
-        self._validate()
-
-    def _validate(self):
-        """
-        Validate the inputs of the `GroundTruth`.
-        """
-        # validate datum
-        if not isinstance(self.datum, Datum):
-            raise TypeError(
-                "Attribute `datum` should have type `valor.Datum`."
-            )
-
-        # validate annotations
-        if not isinstance(self.annotations, list):
-            raise TypeError(
-                "Attribute `datum` should have type `List[valor.Annotation]`."
-            )
-        for idx, annotation in enumerate(self.annotations):
-            if not isinstance(annotation, Annotation):
-                raise TypeError(
-                    f"Attribute `annotations[{idx}]` should have type `valor.Annotation`."
-                )
+    Examples
+    --------
+    >>> Prediction(
+    ...     datum=Datum(uid="uid1"),
+    ...     annotations=[
+    ...         Annotation(
+    ...             task_type=TaskType.CLASSIFICATION,
+    ...             labels=[
+    ...                 Label(key="k1", value="v1", score=0.9),
+    ...                 Label(key="k1", value="v1", score=0.1)
+    ...             ],
+    ...         )
+    ...     ]
+    ... )
+    """
 
-    def to_dict(
-        self,
-        dataset_name: Optional[str] = None,
-    ) -> dict:
-        """
-        Defines how a `valor.GroundTruth` object is serialized into a dictionary.
-
-        Returns
-        ----------
-        dict
-            A dictionary describing a ground truth.
-        """
-        return {
-            "datum": self.datum.to_dict(dataset_name),
-            "annotations": [
-                annotation.to_dict() for annotation in self.annotations
-            ],
-        }
+    datum: Datum = Datum.symbolic(owner="prediction", name="datum")
+    annotations: SymbolicList[Annotation] = SymbolicList[Annotation].symbolic(
+        owner="prediction", name="annotations"
+    )
 
     @classmethod
-    def from_dict(cls, resp: dict) -> GroundTruth:
+    def create(
+        cls,
+        datum: Datum,
+        annotations: List[Annotation],
+        **_,
+    ):
         """
-        Construct a ground truth from a dictionary.
+        Creates a prediction.
 
         Parameters
         ----------
-        resp : dict
-            The dictionary containing a ground truth.
-
-        Returns
-        -------
-        valor.GroundTruth
+        datum : Datum
+            The `Datum` associated with the `Prediction`.
+        annotations : List[Annotation]
+            The list of `Annotations` associated with the `Prediction`.
         """
-        expected_keys = {"datum", "annotations"}
-        if set(resp.keys()) != expected_keys:
-            raise ValueError(
-                f"Expected keys `{expected_keys}`, received `{set(resp.keys())}`."
-            )
-        if not isinstance(resp["annotations"], list):
-            raise TypeError("Expected `annotations` member to be a `list`.")
-        return cls(
-            datum=Datum.from_dict(resp["datum"]),
-            annotations=[
-                Annotation.from_dict(annotation)
-                for annotation in resp["annotations"]
-            ],
+        return cls.definite(
+            datum=datum,
+            annotations=annotations,
         )
 
-    def __str__(self) -> str:
-        """Dumps the object into a JSON formatted string."""
-        objdict = self.to_dict(dataset_name=None)
-        objdict["datum"].pop("dataset_name")
-        return json.dumps(objdict, indent=4)
-
-    def __eq__(self, other):
-        """
-        Defines how `GroundTruths` are compared to one another.
-
-        Parameters
-        ----------
-        other : GroundTruth
-            The object to compare with the `GroundTruth`.
-
-        Returns
-        ----------
-        boolean
-            A boolean describing whether the two objects are equal.
-        """
-        if not isinstance(other, GroundTruth):
-            raise TypeError(
-                f"Expected type `{type(GroundTruth)}`, got `{other}`"
-            )
-        return self.to_dict() == other.to_dict()
-
-
-class Prediction:
-    """
-    An object describing a prediction (e.g., a machine-drawn bounding box on an image).
-
-    Parameters
-    ----------
-    datum : Datum
-        The `Datum` associated with the `Prediction`.
-    annotations : List[Annotation]
-        The list of `Annotations` associated with the `Prediction`.
-
-    Attributes
-    ----------
-    score : Union[float, int]
-        The score assigned to the `Prediction`.
-    """
-
-    def __init__(
-        self,
-        datum: Datum,
-        annotations: List[Annotation],
-    ):
-        self.datum = datum
-        self.annotations = annotations
-        self._validate()
-
-    def _validate(self):
+    def __post_init__(self):
         """
-        Validate the inputs of the `Prediction`.
+        Validate the inputs of the `Prediction` based on task type.
         """
-        # validate datum
-        if not isinstance(self.datum, Datum):
-            raise TypeError(
-                "Attribute `datum` should have type `valor.Datum`."
-            )
-
-        # validate annotations
-        if not isinstance(self.annotations, list):
-            raise TypeError(
-                "Attribute `datum` should have type `List[valor.Annotation]`."
-            )
-        for idx, annotation in enumerate(self.annotations):
-            if not isinstance(annotation, Annotation):
-                raise TypeError(
-                    f"Attribute `annotations[{idx}]` should have type `valor.Annotation`."
-                )
-
-        # TaskType-specific validations
         for annotation in self.annotations:
-            if annotation.task_type in [
+            task_type = annotation.task_type.get_value()
+            if task_type in [
                 TaskType.CLASSIFICATION,
                 TaskType.OBJECT_DETECTION,
             ]:
                 for label in annotation.labels:
-                    if label.score is None:
+                    label_score = label.score._value
+                    if label_score is None:
                         raise ValueError(
-                            f"For task type `{annotation.task_type}` prediction labels must have scores, but got `None`"
+                            f"For task type `{task_type}` prediction labels must have scores, but got `None`"
                         )
-            if annotation.task_type == TaskType.CLASSIFICATION:
+            if task_type == TaskType.CLASSIFICATION:
+
                 label_keys_to_sum = {}
                 for scored_label in annotation.labels:
-                    label_key = scored_label.key
+                    label_key = scored_label.key.get_value()
+                    label_score = scored_label.score.get_value()
                     if label_key not in label_keys_to_sum:
                         label_keys_to_sum[label_key] = 0.0
-                    label_keys_to_sum[label_key] += scored_label.score
+                    label_keys_to_sum[label_key] += label_score
 
                 for k, total_score in label_keys_to_sum.items():
                     if abs(total_score - 1) > 1e-5:
                         raise ValueError(
                             "For each label key, prediction scores must sum to 1, but"
                             f" for label key {k} got scores summing to {total_score}."
                         )
 
-    def to_dict(
-        self,
-        dataset_name: Optional[str] = None,
-        model_name: Optional[str] = None,
-    ) -> dict:
-        """
-        Defines how a `valor.Prediction` object is serialized into a dictionary.
-
-        Returns
-        ----------
-        dict
-            A dictionary describing a prediction.
-        """
-        return {
-            "datum": self.datum.to_dict(dataset_name=dataset_name),
-            "model_name": model_name,
-            "annotations": [
-                annotation.to_dict() for annotation in self.annotations
-            ],
-        }
-
-    @classmethod
-    def from_dict(cls, resp: dict) -> Prediction:
-        """
-        Construct a Prediction from a dictionary.
-
-        Parameters
-        ----------
-        resp : dict
-            The dictionary containing a prediction.
-
-        Returns
-        -------
-        valor.Prediction
-        """
-        expected_keys = {"datum", "annotations", "model_name"}
-        if set(resp.keys()) != expected_keys:
-            raise ValueError(
-                f"Expected keys `{expected_keys}`, received `{set(resp.keys())}`."
-            )
-        if not isinstance(resp["annotations"], list):
-            raise TypeError("Expected `annotations` member to be a `list`.")
-        return cls(
-            datum=Datum.from_dict(resp["datum"]),
-            annotations=[
-                Annotation.from_dict(annotation)
-                for annotation in resp["annotations"]
-            ],
-        )
-
-    def __str__(self) -> str:
-        """Dumps the object into a JSON formatted string."""
-        objdict = self.to_dict(dataset_name=None)
-        objdict["datum"].pop("dataset_name")
-        objdict.pop("model_name")
-        return json.dumps(objdict, indent=4)
-
-    def __eq__(self, other):
-        """
-        Defines how `Predictions` are compared to one another.
-
-        Parameters
-        ----------
-        other : Prediction
-            The object to compare with the `Prediction`.
-
-        Returns
-        ----------
-        boolean
-            A boolean describing whether the two objects are equal.
-        """
-        if not isinstance(other, Prediction):
-            raise TypeError(
-                f"Expected type `{type(Prediction)}`, got `{other}`"
-            )
-        return self.to_dict(None, None) == other.to_dict(None, None)
-
 
 class Evaluation:
     """
     Wraps `valor.client.Job` to provide evaluation-specifc members.
     """
 
     def __init__(
@@ -821,38 +226,14 @@
             A list of confusion matrix dictionaries returned by the job.
         """
         if not connection:
             connection = get_connection()
         self.conn = connection
         self.update(**kwargs)
 
-    def __str__(self) -> str:
-        """Dumps the object into a JSON formatted string."""
-        return json.dumps(self.to_dict(), indent=4)
-
-    def to_dict(self) -> dict:
-        """
-        Defines how a `valor.Evaluation` object is serialized into a dictionary.
-
-        Returns
-        ----------
-        dict
-            A dictionary describing an evaluation.
-        """
-        return {
-            "id": self.id,
-            "model_name": self.model_name,
-            "datum_filter": asdict(self.datum_filter),
-            "parameters": asdict(self.parameters),
-            "status": self.status.value,
-            "metrics": self.metrics,
-            "confusion_matrices": self.confusion_matrices,
-            **self.kwargs,
-        }
-
     def update(
         self,
         *_,
         id: int,
         model_name: str,
         datum_filter: Filter,
         parameters: EvaluationParameters,
@@ -931,14 +312,38 @@
             EvaluationStatus.FAILED,
         ]:
             time.sleep(interval)
             if timeout and time.time() - t_start > timeout:
                 raise TimeoutError
         return self.status
 
+    def __str__(self) -> str:
+        """Dumps the object into a JSON formatted string."""
+        return json.dumps(self.to_dict(), indent=4)
+
+    def to_dict(self) -> dict:
+        """
+        Defines how a `valor.Evaluation` object is serialized into a dictionary.
+
+        Returns
+        ----------
+        dict
+            A dictionary describing an evaluation.
+        """
+        return {
+            "id": self.id,
+            "model_name": self.model_name,
+            "datum_filter": asdict(self.datum_filter),
+            "parameters": asdict(self.parameters),
+            "status": self.status.value,
+            "metrics": self.metrics,
+            "confusion_matrices": self.confusion_matrices,
+            **self.kwargs,
+        }
+
     def to_dataframe(
         self,
         stratify_by: Optional[Tuple[str, str]] = None,
     ):
         """
         Get all metrics associated with a Model and return them in a `pd.DataFrame`.
 
@@ -991,73 +396,56 @@
     num_datums: int
     num_annotations: int
     num_bounding_boxes: int
     num_polygons: int
     num_rasters: int
     task_types: List[TaskType]
     labels: List[Label]
-    datum_metadata: List[MetadataType]
-    annotation_metadata: List[MetadataType]
+    datum_metadata: List[dict]
+    annotation_metadata: List[dict]
 
     def __post_init__(self):
         for i, tt in enumerate(self.task_types):
             if isinstance(tt, str):
                 self.task_types[i] = TaskType(tt)
         for i, label in enumerate(self.labels):
             if isinstance(label, dict):
                 self.labels[i] = Label(**label)
 
 
-class Dataset:
+class Dataset(StaticCollection):
     """
     A class describing a given dataset.
 
-    Parameters
+    Attributes
     ----------
-    name : str
+    name : String
         The name of the dataset.
-    metadata : dict
+    metadata : Dictionary
         A dictionary of metadata that describes the dataset.
-    """
-
-    name = StringProperty("dataset_names")
-    metadata = DictionaryProperty("dataset_metadata")
-
-    def __init__(
-        self,
-        name: str,
-        metadata: Optional[MetadataType] = None,
-        connection: Optional[ClientConnection] = None,
-    ):
-        """
-        Create or get a `Dataset` object.
 
-        Parameters
-        ----------
-        name : str
-            The name of the dataset.
-        metadata : dict
-            An optional dictionary of metadata that describes the dataset.
-        connection : ClientConnnetion
-            An optional Valor client object for interacting with the API.
-        """
-        self.conn = connection
-        self.name = name
-        self.metadata = metadata if metadata else {}
+    Examples
+    --------
+    >>> Dataset.create(name="dataset1")
+    >>> Dataset.create(name="dataset1", metadata={})
+    >>> Dataset.create(name="dataset1", metadata={"foo": "bar", "pi": 3.14})
+    """
 
-        # validation
-        if not isinstance(self.name, str):
-            raise TypeError("`name` should be of type `str`")
-        validate_metadata(self.metadata)
+    name: String = String.symbolic(owner="dataset", name="name")
+    metadata: Dictionary = Dictionary.symbolic(
+        owner="dataset", name="metadata"
+    )
 
     @classmethod
     def create(
         cls,
         name: str,
-        metadata: Optional[MetadataType] = None,
+        metadata: Optional[dict] = None,
+        connection: Optional[ClientConnection] = None,
+        **_,
     ) -> Dataset:
         """
         Creates a dataset that persists in the back end.
 
         Parameters
         ----------
         name : str
@@ -1066,78 +454,56 @@
             A dictionary of metadata that describes the dataset.
 
         Returns
         -------
         valor.Dataset
             The created dataset.
         """
-        dataset = cls(
+        dataset = cls.definite(
             name=name,
             metadata=metadata,
         )
+        dataset.add_connection(connection)
         Client(dataset.conn).create_dataset(dataset)
         return dataset
 
     @classmethod
     def get(
         cls,
         name: str,
+        connection: Optional[ClientConnection] = None,
     ) -> Union[Dataset, None]:
         """
         Retrieves a dataset from the back end database.
 
         Parameters
         ----------
         name : str
             The name of the dataset.
 
         Returns
         -------
         Union[valor.Dataset, None]
             The dataset or 'None' if it doesn't exist.
         """
-        return Client().get_dataset(name)
+        return Client(connection).get_dataset(name)
 
-    @classmethod
-    def from_dict(
-        cls, resp: dict, connection: Optional[ClientConnection] = None
-    ) -> Dataset:
+    def add_connection(
+        self,
+        connection: Optional[ClientConnection],
+    ):
         """
-        Construct a dataset from a dictionary.
+        Stores a pre-existing connection.
 
         Parameters
         ----------
-        resp : dict
-            The dictionary containing a dataset.
-        connection : ClientConnection, optional
-            Option to share a ClientConnection rather than request a new one.
-
-        Returns
-        -------
-        valor.Dataset
-        """
-        resp["metadata"] = load_metadata(resp["metadata"])
-        return cls(**resp, connection=connection)
-
-    def to_dict(self) -> dict:
-        """
-        Defines how a `valor.Dataset` object is serialized into a dictionary.
-
-        Returns
-        ----------
-        dict
-            A dictionary describing a model.
+        connection : ClientConnnetion, optional
+            An optional Valor client object for interacting with the API.
         """
-        return {"name": self.name, "metadata": dump_metadata(self.metadata)}
-
-    def __str__(self) -> str:
-        """Dumps the object into a JSON formatted string."""
-        objdict = self.to_dict()
-        objdict.pop("id")
-        return json.dumps(objdict, indent=4)
+        self.conn = connection
 
     def add_groundtruth(
         self,
         groundtruth: GroundTruth,
     ) -> None:
         """
         Add a ground truth to the dataset.
@@ -1184,14 +550,17 @@
         Returns
         ----------
         Union[GroundTruth, None]
             The matching ground truth or 'None' if it doesn't exist.
         """
         return Client(self.conn).get_groundtruth(dataset=self, datum=datum)
 
+    def get_name(self) -> str:
+        return self.name.get_value()
+
     def get_labels(
         self,
     ) -> List[Label]:
         """
         Get all labels associated with a given dataset.
 
         Returns
@@ -1221,15 +590,15 @@
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
 
         if filter_.get("dataset_names"):
             raise ValueError(
                 "Cannot filter by dataset_names when calling `Dataset.get_datums`."
             )
-        filter_["dataset_names"] = [self.name]
+        filter_["dataset_names"] = [self.get_name()]
         return Client(self.conn).get_datums(filter_by=filter_)
 
     def get_evaluations(
         self,
     ) -> List[Evaluation]:
         """
         Get all evaluations associated with a given dataset.
@@ -1269,15 +638,15 @@
 
             datum_metadata: list of the unique metadata dictionaries in the dataset that are associated
             to datums
 
             groundtruth_annotation_metadata: list of the unique metadata dictionaries in the dataset that are
             associated to annotations
         """
-        return Client(self.conn).get_dataset_summary(self.name)
+        return Client(self.conn).get_dataset_summary(self.get_name())
 
     def finalize(
         self,
     ):
         """
         Finalizes the dataset such that new ground truths cannot be added to it.
         """
@@ -1291,144 +660,104 @@
         Delete the dataset from the back end.
 
         Parameters
         ----------
         timeout : int, default=0
             Sets a timeout in seconds.
         """
-        Client(self.conn).delete_dataset(self.name, timeout)
+        Client(self.conn).delete_dataset(self.get_name(), timeout)
 
 
-class Model:
+class Model(StaticCollection):
     """
     A class describing a model that was trained on a particular dataset.
 
-    Parameters
+    Attributes
     ----------
-    name : str
+    name : String
         The name of the model.
-    metadata : dict
+    metadata : Dictionary
         A dictionary of metadata that describes the model.
-    """
-
-    name = StringProperty("model_names")
-    metadata = DictionaryProperty("model_metadata")
-
-    def __init__(
-        self,
-        name: str,
-        metadata: Optional[MetadataType] = None,
-        connection: Optional[ClientConnection] = None,
-    ):
-        """
-        Create or get a `Model` object.
 
-        Parameters
-        ----------
-        name : str
-            The name of the model.
-        metadata : dict
-            An optional dictionary of metadata that describes the dataset.
-        connection : ClientConnnetion
-            An optional Valor client object for interacting with the API.
-        """
-        self.conn = connection
-        self.name = name
-        self.metadata = metadata if metadata else {}
+    Examples
+    --------
+    >>> Model.create(name="model1")
+    >>> Model.create(name="model1", metadata={})
+    >>> Model.create(name="model1", metadata={"foo": "bar", "pi": 3.14})
+    """
 
-        # validation
-        if not isinstance(self.name, str):
-            raise TypeError("`name` should be of type `str`")
-        validate_metadata(self.metadata)
+    name: String = String.symbolic(owner="model", name="name")
+    metadata: Dictionary = Dictionary.symbolic(owner="model", name="metadata")
 
     @classmethod
     def create(
         cls,
         name: str,
-        metadata: Optional[MetadataType] = None,
+        metadata: Optional[dict] = None,
+        connection: Optional[ClientConnection] = None,
+        **_,
     ) -> Model:
         """
         Creates a model that persists in the back end.
 
         Parameters
         ----------
         name : str
             The name of the model.
         metadata : dict
             A dictionary of metadata that describes the model.
+        connection : ClientConnnetion, optional
+            An optional Valor client object for interacting with the API.
 
         Returns
         -------
         valor.Model
             The created model.
         """
-        model = cls(
+        model = cls.definite(
             name=name,
             metadata=metadata,
         )
-        Client(model.conn).create_model(model)
+        model.add_connection(connection)
+        Client(connection).create_model(model)
         return model
 
     @classmethod
     def get(
         cls,
         name: str,
+        connection: Optional[ClientConnection] = None,
     ) -> Union[Model, None]:
         """
         Retrieves a model from the back end database.
 
         Parameters
         ----------
         name : str
             The name of the model.
+        connection : ClientConnnetion, optional
+            An optional Valor client object for interacting with the API.
 
         Returns
         -------
         Union[valor.Model, None]
             The model or 'None' if it doesn't exist.
         """
-        return Client().get_model(name)
+        return Client(connection).get_model(name)
 
-    @classmethod
-    def from_dict(
-        cls, resp: dict, connection: Optional[ClientConnection] = None
-    ) -> Model:
+    def add_connection(self, connection: Optional[ClientConnection]):
         """
-        Construct a model from a dictionary.
+        Stores a pre-existing connection.
 
         Parameters
         ----------
-        resp : dict
-            The dictionary containing a model.
-        connection : ClientConnection, optional
-            Option to share a ClientConnection rather than request a new one.
-
-        Returns
-        -------
-        valor.Model
-        """
-        resp["metadata"] = load_metadata(resp["metadata"])
-        return cls(**resp, connection=connection)
-
-    def to_dict(self) -> dict:
-        """
-        Defines how a `valor.Model` object is serialized into a dictionary.
-
-        Returns
-        ----------
-        dict
-            A dictionary describing a model.
+        connection : ClientConnnetion, optional
+            An optional Valor client object for interacting with the API.
         """
-        return {"name": self.name, "metadata": dump_metadata(self.metadata)}
-
-    def __str__(self) -> str:
-        """Dumps the object into a JSON formatted string."""
-        objdict = self.to_dict()
-        objdict.pop("id")
-        return json.dumps(objdict, indent=4)
+        self.conn = connection
 
     def add_prediction(
         self,
         dataset: Dataset,
         prediction: Prediction,
     ) -> None:
         """
@@ -1464,14 +793,17 @@
         """
         Client(self.conn).create_predictions(
             dataset=dataset,
             model=self,
             predictions=predictions,
         )
 
+    def get_name(self) -> str:
+        return self.name.get_value()
+
     def get_prediction(
         self, dataset: Union[Dataset, str], datum: Union[Datum, str]
     ) -> Union[Prediction, None]:
         """
         Get a particular prediction.
 
         Parameters
@@ -1490,33 +822,33 @@
             dataset=dataset, model=self, datum=datum
         )
 
     def finalize_inferences(self, dataset: Union[Dataset, str]) -> None:
         """
         Finalizes the model over a dataset such that new predictions cannot be added to it.
         """
-        if isinstance(dataset, Dataset):
-            dataset = dataset.name
         return Client(self.conn).finalize_inferences(
             dataset=dataset, model=self
         )
 
     def _format_constraints(
         self,
         datasets: Optional[Union[Dataset, List[Dataset]]] = None,
         filter_by: Optional[FilterType] = None,
     ) -> Filter:
         """Formats the 'datum_filter' for any evaluation requests."""
 
         # get list of dataset names
         dataset_names_from_obj = []
         if isinstance(datasets, list):
-            dataset_names_from_obj = [dataset.name for dataset in datasets]
+            dataset_names_from_obj = [
+                dataset.get_name() for dataset in datasets
+            ]
         elif isinstance(datasets, Dataset):
-            dataset_names_from_obj = [datasets.name]
+            dataset_names_from_obj = [datasets.get_name()]
 
         # create a 'schemas.Filter' object from the constraints.
         filter_ = _format_filter(filter_by)
 
         # reset model name
         filter_.model_names = None
         filter_.model_metadata = None
@@ -1541,19 +873,32 @@
                 for key, value in label_map.items()
             ]
         ):
             raise TypeError(
                 "label_map should be a dictionary with valid Labels for both the key and value."
             )
 
-        return_value = [
-            [[key.key, key.value], [value.key, value.value]]
-            for key, value in label_map.items()
-        ]
-
+        return_value = []
+        for key, value in label_map.items():
+            if not all(
+                [
+                    (
+                        isinstance(v.key._value, str)
+                        and isinstance(v.value._value, str)
+                    )
+                    for v in [key, value]
+                ]
+            ):
+                raise TypeError
+            return_value.append(
+                [
+                    [key.key._value, key.value._value],
+                    [value.key._value, value.value._value],
+                ]
+            )
         return return_value
 
     def evaluate_classification(
         self,
         datasets: Optional[Union[Dataset, List[Dataset]]] = None,
         filter_by: Optional[FilterType] = None,
         label_map: Optional[Dict[Label, Label]] = None,
@@ -1582,15 +927,15 @@
             raise ValueError(
                 "Evaluation requires the definition of either datasets, dataset filters or both."
             )
 
         # format request
         datum_filter = self._format_constraints(datasets, filter_by)
         request = EvaluationRequest(
-            model_names=[self.name],
+            model_names=[self.get_name()],
             datum_filter=datum_filter,
             parameters=EvaluationParameters(
                 task_type=TaskType.CLASSIFICATION,
                 label_map=self._create_label_map(label_map=label_map),
                 compute_pr_curves=compute_pr_curves,
             ),
         )
@@ -1659,15 +1004,15 @@
             label_map=self._create_label_map(label_map=label_map),
             recall_score_threshold=recall_score_threshold,
             compute_pr_curves=compute_pr_curves,
             pr_curve_iou_threshold=pr_curve_iou_threshold,
         )
         datum_filter = self._format_constraints(datasets, filter_by)
         request = EvaluationRequest(
-            model_names=[self.name],
+            model_names=[self.get_name()],
             datum_filter=datum_filter,
             parameters=parameters,
         )
 
         # create evaluation
         evaluation = Client(self.conn).evaluate(request)
         if len(evaluation) != 1:
@@ -1696,15 +1041,15 @@
         -------
         Evaluation
             A job object that can be used to track the status of the job and get the metrics of it upon completion
         """
         # format request
         datum_filter = self._format_constraints(datasets, filter_by)
         request = EvaluationRequest(
-            model_names=[self.name],
+            model_names=[self.get_name()],
             datum_filter=datum_filter,
             parameters=EvaluationParameters(
                 task_type=TaskType.SEMANTIC_SEGMENTATION,
                 label_map=self._create_label_map(label_map=label_map),
             ),
         )
 
@@ -1719,15 +1064,15 @@
         Delete the `Model` object from the back end.
 
         Parameters
         ----------
         timeout : int, default=0
             Sets a timeout in seconds.
         """
-        Client(self.conn).delete_model(self.name, timeout)
+        Client(self.conn).delete_model(self.get_name(), timeout)
 
     def get_labels(
         self,
     ) -> List[Label]:
         """
         Get all labels associated with a given model.
 
@@ -1802,17 +1147,15 @@
         Returns
         ------
         List[valor.Label]
             A list of labels.
         """
         filter_ = _format_filter(filter_by)
         filter_ = asdict(filter_)
-        return [
-            Label.from_dict(label) for label in self.conn.get_labels(filter_)
-        ]
+        return [Label(**label) for label in self.conn.get_labels(filter_)]
 
     def get_labels_from_dataset(
         self, dataset: Union[Dataset, str]
     ) -> List[Label]:
         """
         Get all labels associated with a dataset's ground truths.
 
@@ -1823,18 +1166,18 @@
 
         Returns
         ------
         List[valor.Label]
             A list of labels.
         """
         dataset_name = (
-            dataset.name if isinstance(dataset, Dataset) else dataset
+            dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
         return [
-            Label.from_dict(label)
+            Label(**label)
             for label in self.conn.get_labels_from_dataset(dataset_name)
         ]
 
     def get_labels_from_model(self, model: Union[Model, str]) -> List[Label]:
         """
         Get all labels associated with a model's ground truths.
 
@@ -1844,17 +1187,17 @@
             The model to search by.
 
         Returns
         ------
         List[valor.Label]
             A list of labels.
         """
-        model_name = model.name if isinstance(model, Model) else model
+        model_name = model.get_name() if isinstance(model, Model) else model
         return [
-            Label.from_dict(label)
+            Label(**label)
             for label in self.conn.get_labels_from_model(model_name)
         ]
 
     def create_dataset(
         self,
         dataset: Union[Dataset, dict],
     ) -> None:
@@ -1863,15 +1206,15 @@
 
         Parameters
         ----------
         dataset : valor.Dataset
             The dataset to create.
         """
         if isinstance(dataset, Dataset):
-            dataset = dataset.to_dict()
+            dataset = encode_api_format(dataset)
         self.conn.create_dataset(dataset)
 
     def create_groundtruths(
         self,
         dataset: Dataset,
         groundtruths: List[GroundTruth],
     ):
@@ -1888,21 +1231,23 @@
         """
         groundtruths_json = []
         for groundtruth in groundtruths:
             if not isinstance(groundtruth, GroundTruth):
                 raise TypeError(
                     f"Expected ground truth to be of type 'valor.GroundTruth' not '{type(groundtruth)}'."
                 )
-            if len(groundtruth.annotations) == 0:
+            if not isinstance(groundtruth.annotations._value, list):
+                raise TypeError
+            if len(groundtruth.annotations._value) == 0:
                 warnings.warn(
                     f"GroundTruth for datum with uid `{groundtruth.datum.uid}` contains no annotations."
                 )
-            groundtruths_json.append(
-                groundtruth.to_dict(dataset_name=dataset.name)
-            )
+            groundtruth_dict = encode_api_format(groundtruth)
+            groundtruth_dict["datum"]["dataset_name"] = dataset.get_name()
+            groundtruths_json.append(groundtruth_dict)
         self.conn.create_groundtruths(groundtruths_json)
 
     def get_groundtruth(
         self,
         dataset: Union[Dataset, str],
         datum: Union[Datum, str],
     ) -> Union[GroundTruth, None]:
@@ -1918,23 +1263,23 @@
 
         Returns
         ----------
         Union[GroundTruth, None]
             The matching ground truth or 'None' if it doesn't exist.
         """
         dataset_name = (
-            dataset.name if isinstance(dataset, Dataset) else dataset
+            dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
-        datum_uid = datum.uid if isinstance(datum, Datum) else datum
-
+        datum_uid = datum.get_uid() if isinstance(datum, Datum) else datum
         try:
             resp = self.conn.get_groundtruth(
                 dataset_name=dataset_name, datum_uid=datum_uid
             )
-            return GroundTruth.from_dict(resp)
+            resp = decode_api_format(resp)
+            return GroundTruth(**resp)
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def finalize_dataset(self, dataset: Union[Dataset, str]) -> None:
         """
@@ -1942,15 +1287,15 @@
 
         Parameters
         ----------
         dataset : str
             The dataset to be finalized.
         """
         dataset_name = (
-            dataset.name if isinstance(dataset, Dataset) else dataset
+            dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
         return self.conn.finalize_dataset(name=dataset_name)
 
     def get_dataset(
         self,
         name: str,
     ) -> Union[Dataset, None]:
@@ -1964,17 +1309,20 @@
 
         Returns
         -------
         Union[Dataset, None]
             A Dataset with a matching name, or 'None' if one doesn't exist.
         """
         try:
-            return Dataset.from_dict(
-                self.conn.get_dataset(name), connection=self.conn
+            resp = decode_api_format(self.conn.get_dataset(name))
+            dataset = Dataset(
+                **resp,
             )
+            dataset.add_connection(self.conn)
+            return dataset
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def get_datasets(
         self,
@@ -1992,18 +1340,21 @@
         ------
         List[valor.Dataset]
             A list of datasets.
         """
         filter_ = _format_filter(filter_by)
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
-        return [
-            Dataset.from_dict(dataset, connection=self.conn)
-            for dataset in self.conn.get_datasets(filter_)
-        ]
+        dataset_list = []
+        for kwargs in self.conn.get_datasets(filter_):
+            kwargs = decode_api_format(kwargs)
+            dataset = Dataset(**kwargs)
+            dataset.add_connection(self.conn)
+            dataset_list.append(dataset)
+        return dataset_list
 
     def get_datums(
         self,
         filter_by: Optional[FilterType] = None,
     ) -> List[Datum]:
         """
         Get all datums using an optional filter.
@@ -2018,15 +1369,16 @@
         List[valor.Datum]
             A list datums.
         """
         filter_ = _format_filter(filter_by)
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
         return [
-            Datum.from_dict(datum) for datum in self.conn.get_datums(filter_)
+            Datum.create(**decode_api_format(datum))
+            for datum in self.conn.get_datums(filter_)
         ]
 
     def get_datum(
         self,
         dataset: Union[Dataset, str],
         uid: str,
     ) -> Union[Datum, None]:
@@ -2041,19 +1393,20 @@
             The UID of the datum.
         Returns
         -------
         valor.Datum
             The requested datum or 'None' if it doesn't exist.
         """
         dataset_name = (
-            dataset.name if isinstance(dataset, Dataset) else dataset
+            dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
         try:
             resp = self.conn.get_datum(dataset_name=dataset_name, uid=uid)
-            return Datum.from_dict(resp)
+            resp = decode_api_format(resp)
+            return Datum.create(**resp)
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def get_dataset_status(
         self,
@@ -2127,15 +1480,15 @@
 
         Parameters
         ----------
         model : valor.Model
             The model to create.
         """
         if isinstance(model, Model):
-            model = model.to_dict()
+            model = encode_api_format(model)
         self.conn.create_model(model)
 
     def create_predictions(
         self,
         dataset: Dataset,
         model: Model,
         predictions: List[Prediction],
@@ -2154,24 +1507,24 @@
         """
         predictions_json = []
         for prediction in predictions:
             if not isinstance(prediction, Prediction):
                 raise TypeError(
                     f"Expected prediction to be of type 'valor.Prediction' not '{type(prediction)}'."
                 )
-            if len(prediction.annotations) == 0:
+            if not isinstance(prediction.annotations._value, list):
+                raise TypeError
+            if len(prediction.annotations._value) == 0:
                 warnings.warn(
                     f"Prediction for datum with uid `{prediction.datum.uid}` contains no annotations."
                 )
-            predictions_json.append(
-                prediction.to_dict(
-                    dataset_name=dataset.name,
-                    model_name=model.name,
-                )
-            )
+            prediction_dict = encode_api_format(prediction)
+            prediction_dict["datum"]["dataset_name"] = dataset.get_name()
+            prediction_dict["model_name"] = model.get_name()
+            predictions_json.append(prediction_dict)
         self.conn.create_predictions(predictions_json)
 
     def get_prediction(
         self,
         dataset: Union[Dataset, str],
         model: Union[Model, str],
         datum: Union[Datum, str],
@@ -2190,41 +1543,41 @@
 
         Returns
         ----------
         Union[Prediction, None]
             The matching prediction or 'None' if it doesn't exist.
         """
         dataset_name = (
-            dataset.name if isinstance(dataset, Dataset) else dataset
+            dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
-        model_name = model.name if isinstance(model, Model) else model
-        datum_uid = datum.uid if isinstance(datum, Datum) else datum
-
+        model_name = model.get_name() if isinstance(model, Model) else model
+        datum_uid = datum.get_uid() if isinstance(datum, Datum) else datum
         try:
             resp = self.conn.get_prediction(
                 dataset_name=dataset_name,
                 model_name=model_name,
                 datum_uid=datum_uid,
             )
-            return Prediction.from_dict(resp)
+            resp = decode_api_format(resp)
+            return Prediction.create(**resp)
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def finalize_inferences(
         self, dataset: Union[Dataset, str], model: Union[Model, str]
     ) -> None:
         """
         Finalizes a model-dataset pairing such that new predictions cannot be added to it.
         """
         dataset_name = (
-            dataset.name if isinstance(dataset, Dataset) else dataset
+            dataset.get_name() if isinstance(dataset, Dataset) else dataset
         )
-        model_name = model.name if isinstance(model, Model) else model
+        model_name = model.get_name() if isinstance(model, Model) else model
         return self.conn.finalize_inferences(
             dataset_name=dataset_name,
             model_name=model_name,
         )
 
     def get_model(
         self,
@@ -2240,17 +1593,18 @@
 
         Returns
         -------
         Union[valor.Model, None]
             A Model with matching name or 'None' if one doesn't exist.
         """
         try:
-            return Model.from_dict(
-                self.conn.get_model(name), connection=self.conn
-            )
+            resp = decode_api_format(self.conn.get_model(name))
+            model = Model(**resp)
+            model.add_connection(self.conn)
+            return model
         except ClientException as e:
             if e.status_code == 404:
                 return None
             raise e
 
     def get_models(
         self,
@@ -2268,18 +1622,21 @@
         ------
         List[valor.Model]
             A list of models.
         """
         filter_ = _format_filter(filter_by)
         if isinstance(filter_, Filter):
             filter_ = asdict(filter_)
-        return [
-            Model.from_dict(model, connection=self.conn)
-            for model in self.conn.get_models(filter_)
-        ]
+        model_list = []
+        for kwargs in self.conn.get_models(filter_):
+            kwargs = decode_api_format(kwargs)
+            model = Model(**kwargs)
+            model.add_connection(self.conn)
+            model_list.append(model)
+        return model_list
 
     def get_model_status(
         self,
         dataset_name: str,
         model_name: str,
     ) -> Optional[TableStatus]:
         """
@@ -2320,15 +1677,15 @@
             The model to search by.
 
         Returns
         -------
         List[Evaluation]
             A list of evaluations.
         """
-        model_name = model.name if isinstance(model, Model) else model
+        model_name = model.get_name() if isinstance(model, Model) else model
         return [
             Evaluation(**evaluation, connection=self.conn)
             for evaluation in self.conn.get_model_eval_requests(model_name)
         ]
 
     def delete_model(self, name: str, timeout: int = 0) -> None:
         """
@@ -2375,20 +1732,20 @@
         Returns
         -------
         List[valor.Evaluation]
             A list of evaluations.
         """
         if isinstance(datasets, list):
             datasets = [
-                element.name if isinstance(element, Dataset) else element
+                element.get_name() if isinstance(element, Dataset) else element
                 for element in datasets
             ]
         if isinstance(models, list):
             models = [
-                element.name if isinstance(element, Model) else element
+                element.get_name() if isinstance(element, Model) else element
                 for element in models
             ]
         return [
             Evaluation(connection=self.conn, **evaluation)
             for evaluation in self.conn.get_evaluations(
                 evaluation_ids=evaluation_ids,
                 models=models,
```

### Comparing `valor-client-0.19.0/valor/enums.py` & `valor-client-0.20.0/valor/enums.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.19.0/valor/exceptions.py` & `valor-client-0.20.0/valor/exceptions.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.19.0/valor/schemas/evaluation.py` & `valor-client-0.20.0/valor/schemas/evaluation.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.19.0/valor/schemas/metadata.py` & `valor-client-0.20.0/valor/metatypes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,174 @@
-import datetime
-from typing import Dict, List, Union
+from typing import Optional
 
-from valor.typing import is_geojson
+from PIL.Image import Image
 
-GeoJSONPointType = Dict[str, Union[str, List[Union[float, int]]]]
-GeoJSONPolygonType = Dict[str, Union[str, List[List[List[Union[float, int]]]]]]
-GeoJSONMultiPolygonType = Dict[
-    str, Union[str, List[List[List[List[Union[float, int]]]]]]
-]
-GeoJSONType = Union[
-    GeoJSONPointType, GeoJSONPolygonType, GeoJSONMultiPolygonType
-]
-
-ValueType = Union[
-    bool,
-    int,
-    float,
-    str,
-    datetime.datetime,
-    datetime.date,
-    datetime.time,
-    datetime.timedelta,
-    GeoJSONType,
-]
-
-MetadataType = Dict[str, ValueType]
-ConvertibleMetadataType = Dict[
-    str,
-    Union[
-        bool,
-        int,
-        float,
-        str,
-        Dict[str, str],
-        Dict[str, GeoJSONType],
-    ],
-]
-
-
-def _convert_object_to_metadatum(
-    value: ValueType,
-) -> Union[bool, int, float, str, Dict[str, str], Dict[str, GeoJSONType]]:
-    """Converts an object into a valor metadatum."""
-
-    # atomic types
-    if (
-        isinstance(value, bool)
-        or isinstance(value, int)
-        or isinstance(value, float)
-        or isinstance(value, str)
-    ):
-        return value
+from valor import Datum
+from valor.schemas import Integer
 
-    # datetime
-    elif isinstance(value, datetime.datetime):
-        return {"datetime": value.isoformat()}
-    elif isinstance(value, datetime.date):
-        return {"date": value.isoformat()}
-    elif isinstance(value, datetime.time):
-        return {"time": value.isoformat()}
-    elif isinstance(value, datetime.timedelta):
-        return {"duration": str(value.total_seconds())}
-
-    # geojson
-    elif is_geojson(value):
-        return {"geojson": value}
-
-    # not implemented
-    else:
-        raise NotImplementedError(
-            f"Object with type '{type(value)}' is not currently supported."
-        )
 
+class ImageMetadata:
+    """
+    A class describing the metadata for a particular image.
+
+    Parameters
+    ----------
+    uid : str
+        The UID of the image.
+    height : int
+        The height of the image.
+    width : int
+        The width of the image.
+    metadata : dict
+        A dictionary of metadata that describes the image.
+    """
+
+    def __init__(self, datum: Datum):
+        """
+        Creates an `ImageMetadata` object from a `Datum`.
+
+        Parameters
+        ----------
+        datum : Datum
+            The `Datum` to extract metadata from.
+        """
+        if not isinstance(datum, Datum):
+            raise TypeError
+        elif datum.is_symbolic:
+            raise ValueError
 
-def _convert_metadatum_to_object(
-    value: Union[bool, int, float, str, Dict[str, str], Dict[str, GeoJSONType]]
-) -> ValueType:
-    """Converts a valor metadatum into an object."""
-
-    # atomic types
-    if (
-        isinstance(value, bool)
-        or isinstance(value, int)
-        or isinstance(value, float)
-        or isinstance(value, str)
+        height = int(datum.metadata.get_value()["height"].get_value())
+        width = int(datum.metadata.get_value()["width"].get_value())
+        datum.metadata["height"] = Integer(height)
+        datum.metadata["width"] = Integer(width)
+        self.datum = datum
+
+    @classmethod
+    def create(
+        cls,
+        uid: str,
+        height: int,
+        width: int,
+        metadata: Optional[dict] = None,
     ):
-        return value
-
-    # validate serialized type
-    elif not isinstance(value, dict):
-        raise TypeError(
-            f"Object with type '{type(value)}' is not atomic and not serialized."
+        if not isinstance(height, int) or not isinstance(width, int):
+            raise TypeError("Height and width must be integers.")
+        metadata = metadata if metadata else dict()
+        metadata["height"] = height
+        metadata["width"] = width
+        return cls(
+            datum=Datum.definite(
+                uid=uid,
+                metadata=metadata,
+            )
         )
 
-    # datetime
-    elif "datetime" in value:
-        if not isinstance(value["datetime"], str):
-            raise TypeError
-        return datetime.datetime.fromisoformat(value["datetime"])
-    elif "date" in value:
-        if not isinstance(value["date"], str):
-            raise TypeError
-        return datetime.date.fromisoformat(value["date"])
-    elif "time" in value:
-        if not isinstance(value["time"], str):
-            raise TypeError
-        return datetime.time.fromisoformat(value["time"])
-    elif "duration" in value:
-        if not isinstance(value["duration"], str):
-            raise TypeError
-        return datetime.timedelta(seconds=float(value["duration"]))
-
-    # geojson
-    elif "geojson" in value:
-        return value["geojson"]
-
-    # not implemented
-    else:
-        raise TypeError(
-            f"Object with type '{value.keys()}' is not currently supported."
-        )
+    @classmethod
+    def from_pil(cls, image: Image, uid: str):
+        """
+        Creates an `ImageMetadata` object from an image.
+
+        Parameters
+        ----------
+        image : PIL.Image.Image
+            The image to create metadata for.
+        uid : str
+            The UID of the image.
+        """
+        width, height = image.size
+        return cls.create(uid=uid, height=height, width=width)
+
+    @property
+    def height(self) -> int:
+        value = self.datum.metadata["height"].get_value()
+        if not isinstance(value, int):
+            raise TypeError
+        return int(value)
+
+    @property
+    def width(self) -> int:
+        value = self.datum.metadata["width"].get_value()
+        if not isinstance(value, int):
+            raise TypeError
+        return int(value)
 
 
-def validate_metadata(metadata: MetadataType):
-    """Validates metadata dictionary."""
-    if not isinstance(metadata, dict):
-        raise TypeError("`metadata` should be an object of type `dict`.")
-    for key, value in metadata.items():
-        if not isinstance(key, str):
-            raise TypeError("`metadata` key should have type `str`.")
-        if not (
-            isinstance(value, int)
-            or isinstance(value, float)
-            or isinstance(value, str)
-            or isinstance(value, datetime.datetime)
-            or isinstance(value, datetime.date)
-            or isinstance(value, datetime.time)
-            or is_geojson(value)
+class VideoFrameMetadata:
+    """
+    A class describing the metadata for the frame of a video.
+
+    Parameters
+    ----------
+    image : ImageMetadata
+        Metadata describing the frame of the video.
+    frame: int
+        The number of seconds into the video that the frame was taken.
+    """
+
+    def __init__(self, datum: Datum):
+        """
+        Creates a `VideoFrameMetadata` object from a `Datum`.
+
+        Parameters
+        ----------
+        datum : Datum
+            The `Datum` to extract metadata from.
+        """
+        if not isinstance(datum, Datum):
+            raise TypeError
+        elif datum.is_symbolic:
+            raise ValueError
+
+        height = int(datum.metadata.get_value()["height"].get_value())
+        width = int(datum.metadata.get_value()["width"].get_value())
+        frame = int(datum.metadata.get_value()["frame"].get_value())
+        datum.metadata["height"] = Integer(height)
+        datum.metadata["width"] = Integer(width)
+        datum.metadata["frame"] = Integer(frame)
+        self.datum = datum
+
+    @classmethod
+    def create(
+        cls,
+        uid: str,
+        height: int,
+        width: int,
+        frame: int,
+        metadata: Optional[dict] = None,
+    ):
+        if (
+            not isinstance(height, int)
+            or not isinstance(width, int)
+            or not isinstance(frame, int)
         ):
-            raise TypeError(
-                "`metadata` value should have type `str`, `int`, `float`, `datetime` or `geojson`."
+            raise TypeError("Height, width and frame must be integers.")
+        metadata = metadata if metadata else dict()
+        metadata["height"] = height
+        metadata["width"] = width
+        metadata["frame"] = frame
+        return cls(
+            Datum.definite(
+                uid=uid,
+                metadata=metadata,
             )
+        )
 
+    @property
+    def height(self) -> int:
+        value = self.datum.metadata["height"].get_value()
+        if not isinstance(value, int):
+            raise TypeError
+        return int(value)
 
-def dump_metadata(metadata: MetadataType) -> ConvertibleMetadataType:
-    """Converts metadata to API-compatible dictionary."""
-    return {
-        key: _convert_object_to_metadatum(value)
-        for key, value in metadata.items()
-    }
-
+    @property
+    def width(self) -> int:
+        value = self.datum.metadata["width"].get_value()
+        if not isinstance(value, int):
+            raise TypeError
+        return int(value)
 
-def load_metadata(metadata: ConvertibleMetadataType) -> MetadataType:
-    """Converts API metadata to Client-compatible dictionary."""
-    return {
-        key: _convert_metadatum_to_object(value)
-        for key, value in metadata.items()
-    }
+    @property
+    def frame(self) -> int:
+        value = self.datum.metadata["frame"].get_value()
+        if not isinstance(value, int):
+            raise TypeError
+        return int(value)
```

### Comparing `valor-client-0.19.0/valor/typing.py` & `valor-client-0.20.0/valor/type_checks.py`

 * *Files identical despite different names*

### Comparing `valor-client-0.19.0/valor/viz.py` & `valor-client-0.20.0/valor/viz.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import math
 from typing import Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 from PIL import Image, ImageDraw, ImageFont
 
 from valor import Annotation, GroundTruth, Prediction, enums, schemas
-from valor.metatypes import ImageMetadata
 
 # https://sashat.me/2017/01/11/list-of-20-simple-distinct-colors/
 COLOR_MAP = [
     (230, 25, 75),
     (60, 180, 75),
     (255, 225, 25),
     (0, 130, 200),
@@ -37,24 +36,24 @@
 ) -> np.ndarray:
     """note there's some aliasing/areas differences between this
     and e.g. postgis, so this method should only be used for visualization
     """
     mask = Image.new("1", (img_w, img_h), (False,))
     draw = ImageDraw.Draw(mask)
     for poly in polys:
-        draw.polygon(poly.boundary.tuple_list(), fill=(True,))  # type: ignore
+        draw.polygon(poly.boundary, fill=(True,))  # type: ignore
         if poly.holes is not None:
             for hole in poly.holes:
-                draw.polygon(hole.tuple_list(), fill=(False,))  # type: ignore
+                draw.polygon(hole, fill=(False,))  # type: ignore
 
     return np.array(mask)
 
 
 def create_combined_segmentation_mask(
-    annotated_datums: Sequence[Union[GroundTruth, Prediction]],
+    annotated_datum: Union[GroundTruth, Prediction],
     label_key: str,
     task_type: Union[enums.TaskType, None] = None,
 ) -> Tuple[Image.Image, Dict[str, Image.Image]]:
     """
     Creates a combined segmentation mask from a list of segmentations.
 
     Parameters
@@ -79,110 +78,107 @@
     RuntimeError
         If all segmentations don't belong to the same image or there is a
         segmentation that doesn't have `label_key` as the key of one of its labels.
     ValueError
         If there aren't any segmentations.
     """
 
-    if len(annotated_datums) == 0:
-        raise ValueError("`segs` cannot be empty.")
-
-    if (
-        len(
-            set(
-                [
-                    annotated_datum.datum.uid
-                    for annotated_datum in annotated_datums
-                ]
+    # validate input type
+    if not isinstance(annotated_datum, (GroundTruth, Prediction)):
+        raise ValueError("Expected either a 'GroundTruth' or 'Prediction'")
+
+    # verify there are a nonzero number of annotations
+    if len(annotated_datum.annotations) == 0:
+        raise ValueError("annotations cannot be empty.")
+
+    # validate raster size
+    img_h = None
+    img_w = None
+    for annotation in annotated_datum.annotations:
+        if img_h is None:
+            img_h = annotation.raster.height
+        if img_w is None:
+            img_w = annotation.raster.width
+        if (img_h != annotation.raster.height) or (
+            img_w != annotation.raster.width
+        ):
+            raise ValueError(
+                f"Size mismatch between rasters. {(img_h, img_w)} != {(annotation.raster.height, annotation.raster.width)}"
             )
-        )
-        > 1
-    ):
-        raise RuntimeError(
-            "Expected all segmentation to belong to the same image"
+    if img_h is None or img_w is None:
+        raise ValueError(
+            f"Segmentation bounds not properly defined. {(img_h, img_w)}"
         )
 
-    # Validate task type
+    # validate task type
     if task_type is not None and task_type not in [
         enums.TaskType.OBJECT_DETECTION,
         enums.TaskType.SEMANTIC_SEGMENTATION,
     ]:
         raise RuntimeError(
             "Expected either Instance or Semantic segmentation task_type."
         )
 
-    # Create valid task type list
+    # create valid task type list
     if task_type is None:
         task_types = [
             enums.TaskType.OBJECT_DETECTION,
             enums.TaskType.SEMANTIC_SEGMENTATION,
         ]
     else:
         task_types = [task_type]
 
     # unpack raster annotations
     annotations: List[Annotation] = []
-    for annotated_datum in annotated_datums:
-        for annotation in annotated_datum.annotations:
-            if annotation.task_type in task_types:
-                annotations.append(annotation)
+    for annotation in annotated_datum.annotations:
+        if annotation.task_type.get_value() in task_types:
+            annotations.append(annotation)
 
+    # unpack label values
     label_values = []
     for annotation in annotations:
         for label in annotation.labels:
-            if label.key == label_key:
-                label_values.append(label.value)
+            if label.key.get_value() == label_key:
+                label_values.append(label.value.get_value())
     if not label_values:
         raise RuntimeError(
             f"Annotation doesn't have a label with key `{label_key}`"
         )
 
+    # assign label coloring
     unique_label_values = list(set(label_values))
     label_value_to_color = {
         v: COLOR_MAP[i] for i, v in enumerate(unique_label_values)
     }
     seg_colors = [label_value_to_color[v] for v in label_values]
 
-    image = ImageMetadata.from_datum(annotated_datums[0].datum)
-    img_w, img_h = image.width, image.height
-
+    # create mask
     combined_mask = np.zeros((img_h, img_w, 3), dtype=np.uint8)
     for annotation, color in zip(annotations, seg_colors):
-        if annotation.raster is not None:
+        if annotation.raster.array is not None:
             if annotation.raster.geometry is None:
-                mask = annotation.raster.to_numpy()
+                mask = annotation.raster.array
             elif isinstance(annotation.raster.geometry, schemas.MultiPolygon):
                 mask = _polygons_to_binary_mask(
                     annotation.raster.geometry.polygons,
                     img_w=img_w,
                     img_h=img_h,
                 )
             elif isinstance(annotation.raster.geometry, schemas.Polygon):
                 mask = _polygons_to_binary_mask(
                     [annotation.raster.geometry],
                     img_w=img_w,
                     img_h=img_h,
                 )
-            elif isinstance(annotation.raster.geometry, schemas.BoundingBox):
-                mask = _polygons_to_binary_mask(
-                    [
-                        schemas.Polygon(
-                            boundary=annotation.raster.geometry.polygon
-                        )
-                    ],
-                    img_w=img_w,
-                    img_h=img_h,
-                )
             else:
                 continue
+            combined_mask[np.where(mask)] = color
         else:
             continue
 
-        combined_mask[np.where(mask)] = color
-
     legend = {
         v: Image.new("RGB", (20, 20), color)
         for v, color in label_value_to_color.items()
     }
 
     return Image.fromarray(combined_mask), legend
 
@@ -235,58 +231,61 @@
         RGB tuple of the color to use.
 
     Returns
     -------
     img
         Pillow image with bounding box drawn on it.
     """
+    coords = bounding_box.get_value()
+    if not coords:
+        raise ValueError("Bounding box contains 'None'")
     return _draw_bounding_polygon_on_image(
-        bounding_box.polygon, img, color=color, inplace=False
+        schemas.Polygon(coords), img, color=color, inplace=False
     )
 
 
 def _draw_detection_on_image(
     detection: Annotation, img: Image.Image, inplace: bool
 ) -> Image.Image:
     """Draw a detection on an image."""
     text = ", ".join(
         [f"{label.key}:{label.value}" for label in detection.labels]
     )
     if detection.polygon is not None:
         img = _draw_bounding_polygon_on_image(
-            detection.polygon.boundary,
+            detection.polygon,
             img,
             inplace=inplace,
             text=text,
         )
     elif detection.bounding_box is not None:
         img = _draw_bounding_polygon_on_image(
-            detection.bounding_box.polygon,
+            detection.bounding_box,
             img,
             inplace=inplace,
             text=text,
         )
 
     return img
 
 
 def _draw_bounding_polygon_on_image(
-    polygon: schemas.BasicPolygon,
+    polygon: schemas.Polygon,
     img: Image.Image,
     color: Tuple[int, int, int] = (255, 0, 0),
     inplace: bool = False,
     text: Optional[str] = None,
     font_size: int = 24,
 ) -> Image.Image:
     """Draw a bounding polygon on an image."""
     img = img if inplace else img.copy()
     img_draw = ImageDraw.Draw(img)
 
     img_draw.polygon(
-        [(p.x, p.y) for p in polygon.points],
+        [p for p in polygon.boundary],
         outline=color,
     )
 
     if text is not None:
         _write_text(
             font_size=font_size,
             text=text,
@@ -296,15 +295,15 @@
         )
     return img
 
 
 def _write_text(
     font_size: int,
     text: str,
-    boundary: schemas.BasicPolygon,
+    boundary: schemas.Polygon,
     draw: ImageDraw.ImageDraw,
     color: Union[Tuple[int, int, int], str],
 ):
     """Write text on an image."""
     try:
         font = ImageFont.truetype("arial.ttf", font_size)
     except IOError:
@@ -349,15 +348,17 @@
         pillow image to draw on.
     color
         RGB tuple of the color to use
     alpha
         alpha (transparency) value of the mask. 0 is fully transparent, 1 is fully opaque
     """
     img = img.copy()
-    binary_mask = raster.to_numpy()
+    binary_mask = raster.array
+    if not binary_mask:
+        raise ValueError
     mask_arr = np.zeros(
         (binary_mask.shape[0], binary_mask.shape[1], 3), dtype=np.uint8
     )
     mask_arr[binary_mask] = color
     mask_img = Image.fromarray(mask_arr)
     blend = Image.blend(img, mask_img, alpha=alpha)
     img.paste(blend, (0, 0), mask=Image.fromarray(binary_mask))
```

### Comparing `valor-client-0.19.0/valor_client.egg-info/PKG-INFO` & `valor-client-0.20.0/valor_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valor-client
-Version: 0.19.0
+Version: 0.20.0
 Summary: Python client for the Valor evaluation store
 License: MIT License
         
         Copyright (c) 2023 Striveworks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `valor-client-0.19.0/valor_client.egg-info/SOURCES.txt` & `valor-client-0.20.0/valor_client.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,33 +4,38 @@
 unit-tests/conftest.py
 unit-tests/test_client.py
 unit-tests/test_types.py
 unit-tests/test_viz.py
 unit-tests/coretypes/test_core.py
 unit-tests/coretypes/test_evaluation.py
 unit-tests/coretypes/test_filtering.py
-unit-tests/schemas/test_constraints.py
 unit-tests/schemas/test_evaluation_schemas.py
 unit-tests/schemas/test_filters.py
-unit-tests/schemas/test_geometry.py
+unit-tests/schemas/test_geojson.py
 unit-tests/schemas/test_label.py
-unit-tests/schemas/test_metadata.py
+unit-tests/symbolic/test_operators.py
+unit-tests/symbolic/collections/test_dictionary.py
+unit-tests/symbolic/collections/test_static_collection.py
+unit-tests/symbolic/collections/test_structures.py
+unit-tests/symbolic/types/test_schemas.py
+unit-tests/symbolic/types/test_symbolic_types.py
 valor/__init__.py
 valor/client.py
 valor/coretypes.py
 valor/enums.py
 valor/exceptions.py
 valor/metatypes.py
-valor/typing.py
+valor/type_checks.py
 valor/viz.py
 valor/schemas/__init__.py
-valor/schemas/constraints.py
+valor/schemas/compatibility.py
 valor/schemas/evaluation.py
 valor/schemas/filters.py
-valor/schemas/geometry.py
-valor/schemas/metadata.py
-valor/schemas/properties.py
+valor/schemas/symbolic/__init__.py
+valor/schemas/symbolic/collections.py
+valor/schemas/symbolic/operators.py
+valor/schemas/symbolic/types.py
 valor_client.egg-info/PKG-INFO
 valor_client.egg-info/SOURCES.txt
 valor_client.egg-info/dependency_links.txt
 valor_client.egg-info/requires.txt
 valor_client.egg-info/top_level.txt
```

