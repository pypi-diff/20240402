# Comparing `tmp/flytekitplugins-onnxscikitlearn-1.9.0a0.tar.gz` & `tmp/flytekitplugins-onnxscikitlearn-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-onnxscikitlearn-1.9.0a0.tar", last modified: Thu Jul 20 18:58:23 2023, max compression
+gzip compressed data, was "flytekitplugins-onnxscikitlearn-1.9.1.tar", last modified: Mon Aug 28 16:43:11 2023, max compression
```

## Comparing `flytekitplugins-onnxscikitlearn-1.9.0a0.tar` & `flytekitplugins-onnxscikitlearn-1.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.548720 flytekitplugins-onnxscikitlearn-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 18:58:23.548720 flytekitplugins-onnxscikitlearn-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-20 18:57:54.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.544720 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.544720 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins/onnxscikitlearn/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-20 18:57:54.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins/onnxscikitlearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-20 18:57:54.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins/onnxscikitlearn/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.544720 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins_onnxscikitlearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 18:58:23.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 18:58:23.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins_onnxscikitlearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:23.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins_onnxscikitlearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:23.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins_onnxscikitlearn.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 18:58:23.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins_onnxscikitlearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:23.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins_onnxscikitlearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:23.548720 flytekitplugins-onnxscikitlearn-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-20 18:58:12.000000 flytekitplugins-onnxscikitlearn-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:11.050127 flytekitplugins-onnxscikitlearn-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      801 2023-08-28 16:43:11.050127 flytekitplugins-onnxscikitlearn-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      217 2023-08-28 16:42:38.000000 flytekitplugins-onnxscikitlearn-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:11.046127 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:11.046127 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins/onnxscikitlearn/
+-rw-r--r--   0 runner    (1001) docker     (999)      235 2023-08-28 16:42:38.000000 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins/onnxscikitlearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6333 2023-08-28 16:42:38.000000 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins/onnxscikitlearn/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:11.046127 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins_onnxscikitlearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      801 2023-08-28 16:43:11.000000 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      442 2023-08-28 16:43:11.000000 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins_onnxscikitlearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:11.000000 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins_onnxscikitlearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:11.000000 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins_onnxscikitlearn.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       41 2023-08-28 16:43:11.000000 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins_onnxscikitlearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:11.000000 flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins_onnxscikitlearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:11.050127 flytekitplugins-onnxscikitlearn-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1185 2023-08-28 16:43:00.000000 flytekitplugins-onnxscikitlearn-1.9.1/setup.py
```

### Comparing `flytekitplugins-onnxscikitlearn-1.9.0a0/PKG-INFO` & `flytekitplugins-onnxscikitlearn-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxscikitlearn
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: ONNX ScikitLearn Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins/onnxscikitlearn/schema.py` & `flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins/onnxscikitlearn/schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
 import inspect
 from dataclasses import dataclass, field
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
 
 import skl2onnx.common.data_types
-from dataclasses_json import dataclass_json
+from dataclasses_json import DataClassJsonMixin
 from skl2onnx import convert_sklearn
 from sklearn.base import BaseEstimator
 from typing_extensions import Annotated, get_args, get_origin
 
 from flytekit import FlyteContext
 from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError
 from flytekit.models.core.types import BlobType
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
 from flytekit.types.file import ONNXFile
 
 
-@dataclass_json
 @dataclass
-class ScikitLearn2ONNXConfig:
+class ScikitLearn2ONNXConfig(DataClassJsonMixin):
     """
     ScikitLearn2ONNXConfig is the config used during the scikitlearn to ONNX conversion.
 
     Args:
       initial_types: The types of the inputs to the model.
       name: The name of the graph in the produced ONNX model.
       doc_string: A string attached onto the produced ONNX model.
@@ -67,17 +66,16 @@
             validate_final_types = [
                 True for item in self.final_types if item in inspect.getmembers(skl2onnx.common.data_types)
             ]
             if not all(validate_final_types):
                 raise ValueError("All types in final_types must be in skl2onnx.common.data_types")
 
 
-@dataclass_json
 @dataclass
-class ScikitLearn2ONNX:
+class ScikitLearn2ONNX(DataClassJsonMixin):
     model: BaseEstimator = field(default=None)
 
 
 def extract_config(t: Type[ScikitLearn2ONNX]) -> Tuple[Type[ScikitLearn2ONNX], ScikitLearn2ONNXConfig]:
     config = None
 
     if get_origin(t) is Annotated:
```

### Comparing `flytekitplugins-onnxscikitlearn-1.9.0a0/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO` & `flytekitplugins-onnxscikitlearn-1.9.1/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxscikitlearn
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: ONNX ScikitLearn Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxscikitlearn-1.9.0a0/setup.py` & `flytekitplugins-onnxscikitlearn-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "onnxscikitlearn"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit<1.3.0b2,<2.0.0", "skl2onnx>=1.10.3"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=f"flytekitplugins-{PLUGIN_NAME}",
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="ONNX ScikitLearn Plugin for Flytekit",
```

