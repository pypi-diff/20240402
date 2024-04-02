# Comparing `tmp/flytekitplugins-great_expectations-1.9.0a0.tar.gz` & `tmp/flytekitplugins-great_expectations-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-great_expectations-1.9.0a0.tar", last modified: Thu Jul 20 18:58:18 2023, max compression
+gzip compressed data, was "flytekitplugins-great_expectations-1.9.1.tar", last modified: Mon Aug 28 16:43:06 2023, max compression
```

## Comparing `flytekitplugins-great_expectations-1.9.0a0.tar` & `flytekitplugins-great_expectations-1.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.680671 flytekitplugins-great_expectations-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 18:58:18.680671 flytekitplugins-great_expectations-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-20 18:57:54.000000 flytekitplugins-great_expectations-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.676671 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.676671 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-20 18:57:54.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12853 2023-07-20 18:57:54.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-20 18:57:54.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.680671 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:18.000000 flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:18.680671 flytekitplugins-great_expectations-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-20 18:58:12.000000 flytekitplugins-great_expectations-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:06.222122 flytekitplugins-great_expectations-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      806 2023-08-28 16:43:06.222122 flytekitplugins-great_expectations-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     2266 2023-08-28 16:42:38.000000 flytekitplugins-great_expectations-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:06.218122 flytekitplugins-great_expectations-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:06.222122 flytekitplugins-great_expectations-1.9.1/flytekitplugins/great_expectations/
+-rw-r--r--   0 runner    (1001) docker     (999)      466 2023-08-28 16:42:38.000000 flytekitplugins-great_expectations-1.9.1/flytekitplugins/great_expectations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12853 2023-08-28 16:42:38.000000 flytekitplugins-great_expectations-1.9.1/flytekitplugins/great_expectations/schema.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10377 2023-08-28 16:42:38.000000 flytekitplugins-great_expectations-1.9.1/flytekitplugins/great_expectations/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:06.222122 flytekitplugins-great_expectations-1.9.1/flytekitplugins_great_expectations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      806 2023-08-28 16:43:06.000000 flytekitplugins-great_expectations-1.9.1/flytekitplugins_great_expectations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-28 16:43:06.000000 flytekitplugins-great_expectations-1.9.1/flytekitplugins_great_expectations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:06.000000 flytekitplugins-great_expectations-1.9.1/flytekitplugins_great_expectations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:06.000000 flytekitplugins-great_expectations-1.9.1/flytekitplugins_great_expectations.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      142 2023-08-28 16:43:06.000000 flytekitplugins-great_expectations-1.9.1/flytekitplugins_great_expectations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:06.000000 flytekitplugins-great_expectations-1.9.1/flytekitplugins_great_expectations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:06.222122 flytekitplugins-great_expectations-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1311 2023-08-28 16:43:00.000000 flytekitplugins-great_expectations-1.9.1/setup.py
```

### Comparing `flytekitplugins-great_expectations-1.9.0a0/PKG-INFO` & `flytekitplugins-great_expectations-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-great_expectations
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Great Expectations Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-great_expectations-1.9.0a0/README.md` & `flytekitplugins-great_expectations-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/schema.py` & `flytekitplugins-great_expectations-1.9.1/flytekitplugins/great_expectations/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 import os
 import typing
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import great_expectations as ge
-from dataclasses_json import dataclass_json
+from dataclasses_json import DataClassJsonMixin
 from great_expectations.checkpoint import SimpleCheckpoint
 from great_expectations.core.run_identifier import RunIdentifier
 from great_expectations.core.util import convert_to_json_serializable
 from great_expectations.exceptions import ValidationError
 
 from flytekit import FlyteContext
 from flytekit.extend import TypeEngine, TypeTransformer
@@ -19,17 +19,16 @@
 from flytekit.models.types import LiteralType
 from flytekit.types.file.file import FlyteFile, FlyteFilePathTransformer
 from flytekit.types.schema.types import FlyteSchema, FlyteSchemaTransformer
 
 from .task import BatchRequestConfig
 
 
-@dataclass_json
 @dataclass
-class GreatExpectationsFlyteConfig(object):
+class GreatExpectationsFlyteConfig(DataClassJsonMixin):
     """
     Use this configuration to configure GreatExpectations Plugin.
 
     Args:
         datasource_name: tell where your data lives and how to get it
         expectation_suite_name: suite which consists of the data expectations
         data_connector_name: connector to identify data batches
```

### Comparing `flytekitplugins-great_expectations-1.9.0a0/flytekitplugins/great_expectations/task.py` & `flytekitplugins-great_expectations-1.9.1/flytekitplugins/great_expectations/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import datetime
 import os
 import shutil
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Type, Union
 
 import great_expectations as ge
-from dataclasses_json import dataclass_json
+from dataclasses_json import DataClassJsonMixin
 from great_expectations.checkpoint import SimpleCheckpoint
 from great_expectations.core.run_identifier import RunIdentifier
 from great_expectations.core.util import convert_to_json_serializable
 from great_expectations.exceptions import ValidationError
 
 from flytekit import PythonInstanceTask
 from flytekit.core.context_manager import FlyteContext
 from flytekit.extend import Interface
 from flytekit.loggers import logger
 from flytekit.types.file.file import FlyteFile
 from flytekit.types.schema import FlyteSchema
 
 
-@dataclass_json
 @dataclass
-class BatchRequestConfig(object):
+class BatchRequestConfig(DataClassJsonMixin):
     """
     Use this configuration to configure Batch Request. A BatchRequest can either be
     a simple BatchRequest or a RuntimeBatchRequest.
 
     Args:
         data_connector_query: query to request data batch
         runtime_parameters: parameters to be passed at runtime
@@ -179,18 +178,26 @@
                     "batch_spec_passthrough": self._batch_request_config.batch_spec_passthrough,
                 }
             )
 
             if is_runtime and issubclass(datatype, str):
                 final_batch_request["runtime_parameters"]["query"] = dataset
             elif is_runtime and issubclass(datatype, FlyteSchema):
-                final_batch_request["runtime_parameters"]["batch_data"] = dataset.open().all()
+                # if execution engine is SparkDF, transform the data to pyspark.sql.dataframe.DataFrame, else transform the data
+                # to the default pandas.dataframe
+                if selected_datasource[0]["execution_engine"]["class_name"] == "SparkDFExecutionEngine":
+                    import pyspark
+
+                    final_batch_request["runtime_parameters"]["batch_data"] = dataset.open(
+                        pyspark.sql.dataframe.DataFrame
+                    ).all()
+                else:
+                    final_batch_request["runtime_parameters"]["batch_data"] = dataset.open().all()
             else:
                 raise AssertionError("Can only use runtime_parameters for query(str)/schema data")
-
         # Great Expectations' BatchRequest
         elif self._batch_request_config:
             final_batch_request.update(
                 {
                     "data_connector_query": self._batch_request_config.data_connector_query,
                     "batch_spec_passthrough": self._batch_request_config.batch_spec_passthrough,
                 }
```

### Comparing `flytekitplugins-great_expectations-1.9.0a0/flytekitplugins_great_expectations.egg-info/PKG-INFO` & `flytekitplugins-great_expectations-1.9.1/flytekitplugins_great_expectations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-great-expectations
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Great Expectations Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-great_expectations-1.9.0a0/setup.py` & `flytekitplugins-great_expectations-1.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 from setuptools import setup
 
 PLUGIN_NAME = "great_expectations"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "great-expectations>=0.13.30", "sqlalchemy>=1.4.23,<2.0.0"]
+plugin_requires = [
+    "flytekit>=1.5.0,<2.0.0",
+    "great-expectations>=0.13.30",
+    "sqlalchemy>=1.4.23,<2.0.0",
+    "pyspark==3.3.1",
+    "flytekitplugins-spark>=1.5.0,<2.0.0",
+    "s3fs<2023.6.0",
+]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Great Expectations Plugin for Flytekit",
```

