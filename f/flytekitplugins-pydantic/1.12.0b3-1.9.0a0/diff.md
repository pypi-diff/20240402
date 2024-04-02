# Comparing `tmp/flytekitplugins-pydantic-1.12.0b3.tar.gz` & `tmp/flytekitplugins-pydantic-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-pydantic-1.12.0b3.tar", last modified: Tue Apr  2 21:31:36 2024, max compression
+gzip compressed data, was "flytekitplugins-pydantic-1.9.0a0.tar", last modified: Thu Jul 20 18:58:25 2023, max compression
```

## Comparing `flytekitplugins-pydantic-1.12.0b3.tar` & `flytekitplugins-pydantic-1.9.0a0.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:36.565180 flytekitplugins-pydantic-1.12.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-02 21:31:36.565180 flytekitplugins-pydantic-1.12.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-02 21:31:04.000000 flytekitplugins-pydantic-1.12.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:36.565180 flytekitplugins-pydantic-1.12.0b3/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:36.565180 flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-02 21:31:04.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-02 21:31:04.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/basemodel_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-02 21:31:04.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-02 21:31:04.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-02 21:31:04.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:36.565180 flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-02 21:31:36.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-02 21:31:36.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:31:36.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 21:31:36.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 21:31:36.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-02 21:31:36.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 21:31:36.000000 flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:31:36.565180 flytekitplugins-pydantic-1.12.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-02 21:31:28.000000 flytekitplugins-pydantic-1.12.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:31:36.565180 flytekitplugins-pydantic-1.12.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-04-02 21:31:04.000000 flytekitplugins-pydantic-1.12.0b3/tests/test_type_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:25.436738 flytekitplugins-pydantic-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-20 18:58:25.436738 flytekitplugins-pydantic-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-20 18:57:54.000000 flytekitplugins-pydantic-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:25.432738 flytekitplugins-pydantic-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:25.432738 flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-20 18:57:54.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-20 18:57:54.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/basemodel_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-20 18:57:54.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-07-20 18:57:54.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-20 18:57:54.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:25.436738 flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-20 18:58:25.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-20 18:58:25.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:25.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-20 18:58:25.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:25.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 18:58:25.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:25.000000 flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:25.436738 flytekitplugins-pydantic-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-20 18:58:12.000000 flytekitplugins-pydantic-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-pydantic-1.12.0b3/PKG-INFO` & `flytekitplugins-pydantic-1.9.0a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pydantic
-Version: 1.12.0b3
+Version: 1.9.0a0
 Summary: Plugin adding type support for Pydantic models
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-pydantic
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,14 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: flytekit<2.0.0,>=1.7.0b0
-Requires-Dist: pydantic
 
 # Flytekit Pydantic Plugin
 
 Pydantic is a data validation and settings management library that uses Python type annotations to enforce type hints at runtime and provide user-friendly errors when data is invalid. Pydantic models are classes that inherit from `pydantic.BaseModel` and are used to define the structure and validation of data using Python type annotations.
 
 The plugin adds type support for pydantic models.
 
@@ -34,15 +32,15 @@
 ```bash
 pip install flytekitplugins-pydantic
 ```
 
 
 ## Type Example
 ```python
-from pydantic.v1 import BaseModel
+from pydantic import BaseModel
 
 
 class TrainConfig(BaseModel):
     lr: float = 1e-3
     batch_size: int = 32
     files: List[FlyteFile]
     directories: List[FlyteDirectory]
```

### Comparing `flytekitplugins-pydantic-1.12.0b3/README.md` & `flytekitplugins-pydantic-1.9.0a0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ```bash
 pip install flytekitplugins-pydantic
 ```
 
 
 ## Type Example
 ```python
-from pydantic.v1 import BaseModel
+from pydantic import BaseModel
 
 
 class TrainConfig(BaseModel):
     lr: float = 1e-3
     batch_size: int = 32
     files: List[FlyteFile]
     directories: List[FlyteDirectory]
```

### Comparing `flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/basemodel_transformer.py` & `flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/basemodel_transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 """Serializes & deserializes the pydantic basemodels """
 
-from typing import Dict, Type
+from typing import Type
 
+import pydantic
 from google.protobuf import json_format
 from typing_extensions import Annotated
 
 from flytekit import FlyteContext
 from flytekit.core import type_engine
 from flytekit.models import literals, types
 
 from . import deserialization, serialization
 
-try:
-    # TODO: Use pydantic v2 to serialize/deserialize data
-    # https://github.com/flyteorg/flyte/issues/5033
-    import pydantic.v1 as pydantic
-except ImportError:
-    import pydantic
-
-BaseModelLiterals = Annotated[
-    Dict[str, literals.Literal],
+BaseModelLiteralMap = Annotated[
+    literals.LiteralMap,
     """
-    BaseModel serialized to a LiteralMap consisting of:
-        1) the basemodel json with placeholders for flyte types
+    BaseModel serialized to a LiteralMap consisting of: 
+        1) the basemodel json with placeholders for flyte types 
         2) mapping from placeholders to serialized flyte type values in the object store
     """,
 ]
 
 
 class BaseModelTransformer(type_engine.TypeTransformer[pydantic.BaseModel]):
     _TYPE_INFO = types.LiteralType(simple=types.SimpleType.STRUCT)
@@ -42,38 +36,31 @@
         self,
         ctx: FlyteContext,
         python_val: pydantic.BaseModel,
         python_type: Type[pydantic.BaseModel],
         expected: types.LiteralType,
     ) -> literals.Literal:
         """Convert a given ``pydantic.BaseModel`` to the Literal representation."""
-        import warnings
-
-        warnings.warn(
-            "If you are using Pydantic version 2.0 or later, please import BaseModel using `from pydantic.v1 import BaseModel`.",
-            FutureWarning,
-        )
         return serialization.serialize_basemodel(python_val)
 
     def to_python_value(
         self,
         ctx: FlyteContext,
         lv: literals.Literal,
         expected_python_type: Type[pydantic.BaseModel],
     ) -> pydantic.BaseModel:
         """Re-hydrate the pydantic BaseModel object from Flyte Literal value."""
-        basemodel_literals: BaseModelLiterals = lv.map.literals
-        basemodel_json_w_placeholders = read_basemodel_json_from_literalmap(basemodel_literals)
-        with deserialization.PydanticDeserializationLiteralStore.attach(
-            basemodel_literals[serialization.OBJECTS_KEY].map
-        ):
+        literalmap: BaseModelLiteralMap = lv.map
+        basemodel_json_w_placeholders = read_basemodel_json_from_literalmap(literalmap)
+        flyte_obj_literalmap = literalmap.literals[serialization.FLYTETYPE_OBJSTORE_KEY]
+        with deserialization.PydanticDeserializationLiteralStore.attach(flyte_obj_literalmap):
             return expected_python_type.parse_raw(basemodel_json_w_placeholders)
 
 
-def read_basemodel_json_from_literalmap(lv: BaseModelLiterals) -> serialization.SerializedBaseModel:
-    basemodel_literal: literals.Literal = lv[serialization.BASEMODEL_JSON_KEY]
+def read_basemodel_json_from_literalmap(lv: BaseModelLiteralMap) -> serialization.SerializedBaseModel:
+    basemodel_literal: literals.Literal = lv.literals[serialization.BASEMODEL_JSON_KEY]
     basemodel_json_w_placeholders = json_format.MessageToJson(basemodel_literal.scalar.generic)
     assert isinstance(basemodel_json_w_placeholders, str)
     return basemodel_json_w_placeholders
 
 
 type_engine.TypeEngine.register(BaseModelTransformer())
```

### Comparing `flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/commons.py` & `flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/commons.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import builtins
 import datetime
-import types
 import typing
 from typing import Set
 
+import numpy
+import pyarrow
 from typing_extensions import Annotated
 
-from flytekit import lazy_module
 from flytekit.core import type_engine
 
-numpy = lazy_module("numpy")
-pyarrow = lazy_module("pyarrow")
-
-MODULES_TO_EXCLUDE_FROM_FLYTE_TYPES: Set[str] = {
-    m.__name__ for m in [builtins, types, typing, datetime, pyarrow, numpy]
-}
+MODULES_TO_EXCLUDE_FROM_FLYTE_TYPES: Set[str] = {m.__name__ for m in [builtins, typing, datetime, pyarrow, numpy]}
 
 
 def include_in_flyte_types(t: type) -> bool:
     if t is None:
         return False
     object_module = t.__module__
     if any(object_module.startswith(module) for module in MODULES_TO_EXCLUDE_FROM_FLYTE_TYPES):
```

### Comparing `flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/deserialization.py` & `flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/deserialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import contextlib
-from typing import Any, Callable, Dict, Generator, Iterator, List, Optional, Type, TypeVar, Union, cast
+from typing import Any, Callable, Dict, Generator, Iterator, List, Optional, Type, TypeVar, Union
 
+import pydantic
 from flytekitplugins.pydantic import commons, serialization
 
 from flytekit.core import context_manager, type_engine
 from flytekit.models import literals
 from flytekit.types import directory, file
 
-try:
-    # TODO: Use pydantic v2 to serialize/deserialize data
-    # https://github.com/flyteorg/flyte/issues/5033
-    import pydantic.v1 as pydantic
-except ImportError:
-    import pydantic
-
 # this field is used by pydantic to get the validator method
-PYDANTIC_VALIDATOR_METHOD_NAME = pydantic.BaseModel.__get_validators__.__name__
-
+PYDANTIC_VALIDATOR_METHOD_NAME = (
+    pydantic.BaseModel.__get_validators__.__name__
+    if pydantic.__version__ < "2.0.0"
+    else pydantic.BaseModel.__get_pydantic_core_schema__.__name___  # type: ignore
+)
 PythonType = TypeVar("PythonType")  # target type of the deserialization
 
 
 class PydanticDeserializationLiteralStore:
     """
     The purpose of this class is to provide a context manager that can be used to deserialize a basemodel from a
     literal map.
 
     Because pydantic validators are fixed when subclassing a BaseModel, this object is a singleton that
     serves as a namespace that can be set with the attach_to_literalmap context manager for the time that
     a basemodel is being deserialized. The validators are then accessing this namespace for the flyteobj
     placeholders that it is trying to deserialize.
     """
 
-    literal_store: Optional[serialization.LiteralStore] = None  # attachment point for the literal map
+    literal_store: Optional[serialization.LiteralStore] = None  # attachement point for the literal map
 
     def __init__(self) -> None:
         raise Exception("This class should not be instantiated")
 
     def __init_subclass__(cls) -> None:
         raise Exception("This class should not be subclassed")
 
@@ -88,18 +85,15 @@
 def add_flyte_validators_for_type(
     flyte_obj_type: Type[type_engine.T],
 ) -> Callable[[Any], Iterator[Callable[[Any], type_engine.T]]]:
     """
     Add flyte deserialisation validators to a type.
     """
 
-    previous_validators = cast(
-        Iterator[Callable[[Any], type_engine.T]],
-        getattr(flyte_obj_type, PYDANTIC_VALIDATOR_METHOD_NAME, lambda *_: [])(),
-    )
+    previous_validators = getattr(flyte_obj_type, PYDANTIC_VALIDATOR_METHOD_NAME, lambda *_: [])()
 
     def validator(object_uid_maybe: Union[commons.LiteralObjID, Any]) -> Union[type_engine.T, Any]:
         """Partial of deserialize_flyte_literal with the object_type fixed"""
         if not PydanticDeserializationLiteralStore.is_attached():
             return object_uid_maybe  # this validator should only trigger when we are deserializeing
         if not isinstance(object_uid_maybe, str):
             return object_uid_maybe  # object uids are strings and we dont want to trigger on other types
```

### Comparing `flytekitplugins-pydantic-1.12.0b3/flytekitplugins/pydantic/serialization.py` & `flytekitplugins-pydantic-1.9.0a0/flytekitplugins/pydantic/serialization.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,31 +7,26 @@
 2. Serialize the flyte types to separate literals and store them in the flyte object store (a singleton object)
 3. Return a literal map with the json and the flyte object store represented as a literalmap {placeholder: flyte type}
 
 """
 import uuid
 from typing import Any, Dict, Union, cast
 
+import pydantic
 from google.protobuf import json_format, struct_pb2
 from typing_extensions import Annotated
 
 from flytekit.core import context_manager, type_engine
 from flytekit.models import literals
 
 from . import commons
 
-try:
-    # TODO: Use pydantic v2 to serialize/deserialize data
-    # https://github.com/flyteorg/flyte/issues/5033
-    import pydantic.v1 as pydantic
-except ImportError:
-    import pydantic
-
 BASEMODEL_JSON_KEY = "BaseModel JSON"
-OBJECTS_KEY = "Serialized Flyte Objects"
+FLYTETYPE_OBJSTORE_KEY = "Flyte Object Store"
+
 
 SerializedBaseModel = Annotated[str, "A pydantic BaseModel that has been serialized with placeholders for Flyte types."]
 
 ObjectStoreID = Annotated[str, "Key for unique literalmap of a serialized basemodel."]
 LiteralObjID = Annotated[str, "Key for unique object in literal map."]
 LiteralStore = Annotated[Dict[LiteralObjID, literals.Literal], "uid to literals for a serialized BaseModel"]
 
@@ -50,31 +45,34 @@
         """Serialize to literal and return a unique identifier."""
         serialized_item = serialize_to_flyte_literal(python_object)
         identifier = make_identifier_for_serializeable(python_object)
         assert identifier not in self.literal_store
         self.literal_store[identifier] = serialized_item
         return identifier
 
-    def to_literal(self) -> literals.Literal:
-        """Convert the object store to a literal map."""
-        return literals.Literal(map=literals.LiteralMap(literals=self.literal_store))
+    def as_literalmap(self) -> literals.LiteralMap:
+        """
+        Converts the object store to a literal map
+        """
+        return literals.LiteralMap(literals=self.literal_store)
 
 
 def serialize_basemodel(basemodel: pydantic.BaseModel) -> literals.Literal:
     """
     Serializes a given pydantic BaseModel instance into a LiteralMap.
     The BaseModel is first serialized into a JSON format, where all Flyte types are replaced with unique placeholder strings.
     The Flyte Types are serialized into separate Flyte literals
     """
     store = BaseModelFlyteObjectStore()
     basemodel_literal = serialize_basemodel_to_literal(basemodel, store)
+    store_literal = store.as_literalmap()
     basemodel_literalmap = literals.LiteralMap(
         {
             BASEMODEL_JSON_KEY: basemodel_literal,  # json with flyte types replaced with placeholders
-            OBJECTS_KEY: store.to_literal(),  # flyte type-engine serialized types
+            FLYTETYPE_OBJSTORE_KEY: store_literal,  # placeholders mapped to flyte types
         }
     )
     literal = literals.Literal(map=basemodel_literalmap)  # type: ignore
     return literal
 
 
 def serialize_basemodel_to_literal(
```

### Comparing `flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/PKG-INFO` & `flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pydantic
-Version: 1.12.0b3
+Version: 1.9.0a0
 Summary: Plugin adding type support for Pydantic models
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-pydantic
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,14 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: flytekit<2.0.0,>=1.7.0b0
-Requires-Dist: pydantic
 
 # Flytekit Pydantic Plugin
 
 Pydantic is a data validation and settings management library that uses Python type annotations to enforce type hints at runtime and provide user-friendly errors when data is invalid. Pydantic models are classes that inherit from `pydantic.BaseModel` and are used to define the structure and validation of data using Python type annotations.
 
 The plugin adds type support for pydantic models.
 
@@ -34,15 +32,15 @@
 ```bash
 pip install flytekitplugins-pydantic
 ```
 
 
 ## Type Example
 ```python
-from pydantic.v1 import BaseModel
+from pydantic import BaseModel
 
 
 class TrainConfig(BaseModel):
     lr: float = 1e-3
     batch_size: int = 32
     files: List[FlyteFile]
     directories: List[FlyteDirectory]
```

### Comparing `flytekitplugins-pydantic-1.12.0b3/flytekitplugins_pydantic.egg-info/SOURCES.txt` & `flytekitplugins-pydantic-1.9.0a0/flytekitplugins_pydantic.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,9 +7,8 @@
 flytekitplugins/pydantic/serialization.py
 flytekitplugins_pydantic.egg-info/PKG-INFO
 flytekitplugins_pydantic.egg-info/SOURCES.txt
 flytekitplugins_pydantic.egg-info/dependency_links.txt
 flytekitplugins_pydantic.egg-info/entry_points.txt
 flytekitplugins_pydantic.egg-info/namespace_packages.txt
 flytekitplugins_pydantic.egg-info/requires.txt
-flytekitplugins_pydantic.egg-info/top_level.txt
-tests/test_type_transformer.py
+flytekitplugins_pydantic.egg-info/top_level.txt
```

### Comparing `flytekitplugins-pydantic-1.12.0b3/setup.py` & `flytekitplugins-pydantic-1.9.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "pydantic"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.7.0b0,<2.0.0", "pydantic"]
 
-__version__ = "1.12.0b3"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Plugin adding type support for Pydantic models",
```

