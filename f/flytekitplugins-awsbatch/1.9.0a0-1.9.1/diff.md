# Comparing `tmp/flytekitplugins-awsbatch-1.9.0a0.tar.gz` & `tmp/flytekitplugins-awsbatch-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-awsbatch-1.9.0a0.tar", last modified: Thu Jul 20 18:58:13 2023, max compression
+gzip compressed data, was "flytekitplugins-awsbatch-1.9.1.tar", last modified: Mon Aug 28 16:43:01 2023, max compression
```

## Comparing `flytekitplugins-awsbatch-1.9.0a0.tar` & `flytekitplugins-awsbatch-1.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:13.860611 flytekitplugins-awsbatch-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-20 18:58:13.860611 flytekitplugins-awsbatch-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 18:57:54.000000 flytekitplugins-awsbatch-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:13.856611 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:13.856611 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins/awsbatch/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-20 18:57:54.000000 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins/awsbatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-20 18:57:54.000000 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins/awsbatch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:13.860611 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins_awsbatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-20 18:58:13.000000 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins_awsbatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-20 18:58:13.000000 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins_awsbatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:13.000000 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins_awsbatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:13.000000 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins_awsbatch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 18:58:13.000000 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins_awsbatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:13.000000 flytekitplugins-awsbatch-1.9.0a0/flytekitplugins_awsbatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:13.860611 flytekitplugins-awsbatch-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-20 18:58:12.000000 flytekitplugins-awsbatch-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:01.518114 flytekitplugins-awsbatch-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      811 2023-08-28 16:43:01.514114 flytekitplugins-awsbatch-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      244 2023-08-28 16:42:38.000000 flytekitplugins-awsbatch-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:01.514114 flytekitplugins-awsbatch-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:01.514114 flytekitplugins-awsbatch-1.9.1/flytekitplugins/awsbatch/
+-rw-r--r--   0 runner    (1001) docker     (999)      243 2023-08-28 16:42:38.000000 flytekitplugins-awsbatch-1.9.1/flytekitplugins/awsbatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3371 2023-08-28 16:42:38.000000 flytekitplugins-awsbatch-1.9.1/flytekitplugins/awsbatch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:01.514114 flytekitplugins-awsbatch-1.9.1/flytekitplugins_awsbatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      811 2023-08-28 16:43:01.000000 flytekitplugins-awsbatch-1.9.1/flytekitplugins_awsbatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      384 2023-08-28 16:43:01.000000 flytekitplugins-awsbatch-1.9.1/flytekitplugins_awsbatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:01.000000 flytekitplugins-awsbatch-1.9.1/flytekitplugins_awsbatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:01.000000 flytekitplugins-awsbatch-1.9.1/flytekitplugins_awsbatch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       25 2023-08-28 16:43:01.000000 flytekitplugins-awsbatch-1.9.1/flytekitplugins_awsbatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:01.000000 flytekitplugins-awsbatch-1.9.1/flytekitplugins_awsbatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:01.518114 flytekitplugins-awsbatch-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1157 2023-08-28 16:43:00.000000 flytekitplugins-awsbatch-1.9.1/setup.py
```

### Comparing `flytekitplugins-awsbatch-1.9.0a0/PKG-INFO` & `flytekitplugins-awsbatch-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-awsbatch
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This package holds the AWS Batch plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-awsbatch-1.9.0a0/flytekitplugins/awsbatch/task.py` & `flytekitplugins-awsbatch-1.9.1/flytekitplugins/awsbatch/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, List, Optional
 
-from dataclasses_json import dataclass_json
+from dataclasses_json import DataClassJsonMixin
 from google.protobuf import json_format
 from google.protobuf.struct_pb2 import Struct
 
 from flytekit import PythonFunctionTask
 from flytekit.configuration import SerializationSettings
 from flytekit.extend import TaskPlugins
 
 
-@dataclass_json
 @dataclass
-class AWSBatchConfig(object):
+class AWSBatchConfig(DataClassJsonMixin):
     """
     Use this to configure SubmitJobInput for a AWS batch job. Task's marked with this will automatically execute
     natively onto AWS batch service.
     Refer to AWS SubmitJobInput for more detail: https://docs.aws.amazon.com/sdk-for-go/api/service/batch/#SubmitJobInput
     """
 
     parameters: Optional[Dict[str, str]] = None
     schedulingPriority: Optional[int] = None
     platformCapabilities: str = "EC2"
     propagateTags: Optional[bool] = None
     tags: Optional[Dict[str, str]] = None
 
     def to_dict(self):
         s = Struct()
-        s.update(self.to_dict())
+        s.update(super().to_dict())
         return json_format.MessageToDict(s)
 
 
 class AWSBatchFunctionTask(PythonFunctionTask):
     """
     Actual Plugin that transforms the local python code for execution within AWS batch job
     """
```

### Comparing `flytekitplugins-awsbatch-1.9.0a0/flytekitplugins_awsbatch.egg-info/PKG-INFO` & `flytekitplugins-awsbatch-1.9.1/flytekitplugins_awsbatch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-awsbatch
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This package holds the AWS Batch plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-awsbatch-1.9.0a0/setup.py` & `flytekitplugins-awsbatch-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "awsbatch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the AWS Batch plugins for flytekit",
```

