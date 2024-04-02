# Comparing `tmp/flytekitplugins-onnxpytorch-1.9.0a0.tar.gz` & `tmp/flytekitplugins-onnxpytorch-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-onnxpytorch-1.9.0a0.tar", last modified: Thu Jul 20 18:58:23 2023, max compression
+gzip compressed data, was "flytekitplugins-onnxpytorch-1.9.1.tar", last modified: Mon Aug 28 16:43:10 2023, max compression
```

## Comparing `flytekitplugins-onnxpytorch-1.9.0a0.tar` & `flytekitplugins-onnxpytorch-1.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-20 18:57:54.000000 flytekitplugins-onnxpytorch-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.056715 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/onnxpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-20 18:57:54.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/onnxpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-07-20 18:57:54.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/onnxpytorch/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:23.000000 flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:23.060715 flytekitplugins-onnxpytorch-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-20 18:58:12.000000 flytekitplugins-onnxpytorch-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:10.566127 flytekitplugins-onnxpytorch-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-28 16:43:10.566127 flytekitplugins-onnxpytorch-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      205 2023-08-28 16:42:38.000000 flytekitplugins-onnxpytorch-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:10.562127 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:10.562127 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins/onnxpytorch/
+-rw-r--r--   0 runner    (1001) docker     (999)      215 2023-08-28 16:42:38.000000 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins/onnxpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5283 2023-08-28 16:42:38.000000 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins/onnxpytorch/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:10.566127 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins_onnxpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-28 16:43:10.000000 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins_onnxpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      410 2023-08-28 16:43:10.000000 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins_onnxpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:10.000000 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins_onnxpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:10.000000 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins_onnxpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       39 2023-08-28 16:43:10.000000 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins_onnxpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:10.000000 flytekitplugins-onnxpytorch-1.9.1/flytekitplugins_onnxpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:10.566127 flytekitplugins-onnxpytorch-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1175 2023-08-28 16:43:00.000000 flytekitplugins-onnxpytorch-1.9.1/setup.py
```

### Comparing `flytekitplugins-onnxpytorch-1.9.0a0/PKG-INFO` & `flytekitplugins-onnxpytorch-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxpytorch
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: ONNX PyTorch Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins/onnxpytorch/schema.py` & `flytekitplugins-onnxpytorch-1.9.1/flytekitplugins/onnxpytorch/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 import torch
-from dataclasses_json import dataclass_json
+from dataclasses_json import DataClassJsonMixin
 from torch.onnx import OperatorExportTypes, TrainingMode
 from typing_extensions import Annotated, get_args, get_origin
 
 from flytekit import FlyteContext
 from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError
 from flytekit.models.core.types import BlobType
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
 from flytekit.types.file import ONNXFile
 
 
-@dataclass_json
 @dataclass
-class PyTorch2ONNXConfig:
+class PyTorch2ONNXConfig(DataClassJsonMixin):
     """
     PyTorch2ONNXConfig is the config used during the pytorch to ONNX conversion.
 
     Args:
       args: The input to the model.
       export_params: Whether to export all the parameters.
       verbose: Whether to print description of the ONNX model.
@@ -49,17 +48,16 @@
     do_constant_folding: bool = False
     dynamic_axes: Union[Dict[str, Dict[int, str]], Dict[str, List[int]]] = field(default_factory=dict)
     keep_initializers_as_inputs: Optional[bool] = None
     custom_opsets: Dict[str, int] = field(default_factory=dict)
     export_modules_as_functions: Union[bool, set[Type]] = False
 
 
-@dataclass_json
 @dataclass
-class PyTorch2ONNX:
+class PyTorch2ONNX(DataClassJsonMixin):
     model: Union[torch.nn.Module, torch.jit.ScriptModule, torch.jit.ScriptFunction] = field(default=None)
 
 
 def extract_config(t: Type[PyTorch2ONNX]) -> Tuple[Type[PyTorch2ONNX], PyTorch2ONNXConfig]:
     config = None
     if get_origin(t) is Annotated:
         base_type, config = get_args(t)
```

### Comparing `flytekitplugins-onnxpytorch-1.9.0a0/flytekitplugins_onnxpytorch.egg-info/PKG-INFO` & `flytekitplugins-onnxpytorch-1.9.1/flytekitplugins_onnxpytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxpytorch
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: ONNX PyTorch Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxpytorch-1.9.0a0/setup.py` & `flytekitplugins-onnxpytorch-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "onnxpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "torch>=1.11.0"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=f"flytekitplugins-{PLUGIN_NAME}",
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="ONNX PyTorch Plugin for Flytekit",
```

