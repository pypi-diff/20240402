# Comparing `tmp/flytekitplugins-bigquery-1.9.0a0.tar.gz` & `tmp/flytekitplugins-bigquery-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-bigquery-1.9.0a0.tar", last modified: Thu Jul 20 18:58:14 2023, max compression
+gzip compressed data, was "flytekitplugins-bigquery-1.9.1.tar", last modified: Mon Aug 28 16:43:02 2023, max compression
```

## Comparing `flytekitplugins-bigquery-1.9.0a0.tar` & `flytekitplugins-bigquery-1.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-20 18:57:54.000000 flytekitplugins-bigquery-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.868624 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 18:57:54.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-20 18:57:54.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/backend_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-20 18:57:54.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:14.000000 flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:14.872624 flytekitplugins-bigquery-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-20 18:58:12.000000 flytekitplugins-bigquery-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.498116 flytekitplugins-bigquery-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      810 2023-08-28 16:43:02.498116 flytekitplugins-bigquery-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      535 2023-08-28 16:42:38.000000 flytekitplugins-bigquery-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.494116 flytekitplugins-bigquery-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.498116 flytekitplugins-bigquery-1.9.1/flytekitplugins/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (999)      323 2023-08-28 16:42:38.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4459 2023-08-28 16:42:38.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins/bigquery/agent.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3246 2023-08-28 16:42:38.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins/bigquery/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.498116 flytekitplugins-bigquery-1.9.1/flytekitplugins_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      810 2023-08-28 16:43:02.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      469 2023-08-28 16:43:02.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:02.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       55 2023-08-28 16:43:02.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins_bigquery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:02.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins_bigquery.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       47 2023-08-28 16:43:02.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:02.000000 flytekitplugins-bigquery-1.9.1/flytekitplugins_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:02.498116 flytekitplugins-bigquery-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1270 2023-08-28 16:43:00.000000 flytekitplugins-bigquery-1.9.1/setup.py
```

### Comparing `flytekitplugins-bigquery-1.9.0a0/PKG-INFO` & `flytekitplugins-bigquery-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.9.0a0/README.md` & `flytekitplugins-bigquery-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-bigquery-1.9.0a0/flytekitplugins/bigquery/backend_plugin.py` & `flytekitplugins-bigquery-1.9.1/flytekitplugins/bigquery/task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,83 @@
-import datetime
-from typing import Dict, Optional
+from dataclasses import dataclass
+from typing import Any, Dict, Optional, Type
 
-import grpc
-from flyteidl.service.external_plugin_service_pb2 import (
-    SUCCEEDED,
-    TaskCreateResponse,
-    TaskDeleteResponse,
-    TaskGetResponse,
-)
 from google.cloud import bigquery
+from google.protobuf import json_format
+from google.protobuf.struct_pb2 import Struct
 
-from flytekit import FlyteContextManager, StructuredDataset, logger
-from flytekit.core.type_engine import TypeEngine
-from flytekit.extend.backend.base_plugin import BackendPluginBase, BackendPluginRegistry, convert_to_flyte_state
-from flytekit.models import literals
-from flytekit.models.literals import LiteralMap
-from flytekit.models.task import TaskTemplate
-from flytekit.models.types import LiteralType, StructuredDatasetType
-
-pythonTypeToBigQueryType: Dict[type, str] = {
-    # https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types#data_type_sizes
-    list: "ARRAY",
-    bool: "BOOL",
-    bytes: "BYTES",
-    datetime.datetime: "DATETIME",
-    float: "FLOAT64",
-    int: "INT64",
-    str: "STRING",
-}
-
-
-class BigQueryPlugin(BackendPluginBase):
-    def __init__(self):
-        super().__init__(task_type="bigquery_query_job_task")
+from flytekit.configuration import SerializationSettings
+from flytekit.extend import SQLTask
+from flytekit.extend.backend.base_agent import AsyncAgentExecutorMixin
+from flytekit.models import task as _task_model
+from flytekit.types.structured import StructuredDataset
 
-    def create(
-        self,
-        context: grpc.ServicerContext,
-        output_prefix: str,
-        task_template: TaskTemplate,
-        inputs: Optional[LiteralMap] = None,
-    ) -> TaskCreateResponse:
-        job_config = None
-        if inputs:
-            ctx = FlyteContextManager.current_context()
-            python_interface_inputs = {
-                name: TypeEngine.guess_python_type(lt.type) for name, lt in task_template.interface.inputs.items()
-            }
-            native_inputs = TypeEngine.literal_map_to_kwargs(ctx, inputs, python_interface_inputs)
 
-            logger.info(f"Create BigQuery job config with inputs: {native_inputs}")
-            job_config = bigquery.QueryJobConfig(
-                query_parameters=[
-                    bigquery.ScalarQueryParameter(name, pythonTypeToBigQueryType[python_interface_inputs[name]], val)
-                    for name, val in native_inputs.items()
-                ]
-            )
-
-        custom = task_template.custom
-        client = bigquery.Client(project=custom["ProjectID"], location=custom["Location"])
-        query_job = client.query(task_template.sql.statement, job_config=job_config)
-
-        return TaskCreateResponse(job_id=str(query_job.job_id))
-
-    def get(self, context: grpc.ServicerContext, job_id: str) -> TaskGetResponse:
-        client = bigquery.Client()
-        job = client.get_job(job_id)
-        cur_state = convert_to_flyte_state(str(job.state))
-        res = None
-
-        if cur_state == SUCCEEDED:
-            ctx = FlyteContextManager.current_context()
-            output_location = f"bq://{job.destination.project}:{job.destination.dataset_id}.{job.destination.table_id}"
-            res = literals.LiteralMap(
-                {
-                    "results": TypeEngine.to_literal(
-                        ctx,
-                        StructuredDataset(uri=output_location),
-                        StructuredDataset,
-                        LiteralType(structured_dataset_type=StructuredDatasetType(format="")),
-                    )
-                }
-            )
-
-        return TaskGetResponse(state=cur_state, outputs=res.to_flyte_idl())
-
-    def delete(self, context: grpc.ServicerContext, job_id: str) -> TaskDeleteResponse:
-        client = bigquery.Client()
-        client.cancel_job(job_id)
-        return TaskDeleteResponse()
+@dataclass
+class BigQueryConfig(object):
+    """
+    BigQueryConfig should be used to configure a BigQuery Task.
+    """
+
+    ProjectID: str
+    Location: Optional[str] = None
+    QueryJobConfig: Optional[bigquery.QueryJobConfig] = None
+
 
+class BigQueryTask(AsyncAgentExecutorMixin, SQLTask[BigQueryConfig]):
+    """
+    This is the simplest form of a BigQuery Task, that can be used even for tasks that do not produce any output.
+    """
 
-BackendPluginRegistry.register(BigQueryPlugin())
+    # This task is executed using the BigQuery handler in the backend.
+    # https://github.com/flyteorg/flyteplugins/blob/43623826fb189fa64dc4cb53e7025b517d911f22/go/tasks/plugins/webapi/bigquery/plugin.go#L34
+    _TASK_TYPE = "bigquery_query_job_task"
+
+    def __init__(
+        self,
+        name: str,
+        query_template: str,
+        task_config: Optional[BigQueryConfig],
+        inputs: Optional[Dict[str, Type]] = None,
+        output_structured_dataset_type: Optional[Type[StructuredDataset]] = None,
+        **kwargs,
+    ):
+        """
+        To be used to query BigQuery Tables.
+
+        :param name: Name of this task, should be unique in the project
+        :param query_template: The actual query to run. We use Flyte's Golang templating format for Query templating. Refer to the templating documentation
+        :param task_config: BigQueryConfig object
+        :param inputs: Name and type of inputs specified as an ordered dictionary
+        :param output_structured_dataset_type: If some data is produced by this query, then you can specify the output StructuredDataset type
+        :param kwargs: All other args required by Parent type - SQLTask
+        """
+        outputs = None
+        if output_structured_dataset_type is not None:
+            outputs = {
+                "results": output_structured_dataset_type,
+            }
+        super().__init__(
+            name=name,
+            task_config=task_config,
+            query_template=query_template,
+            inputs=inputs,
+            outputs=outputs,
+            task_type=self._TASK_TYPE,
+            **kwargs,
+        )
+        self._output_structured_dataset_type = output_structured_dataset_type
+
+    def get_custom(self, settings: SerializationSettings) -> Dict[str, Any]:
+        config = {
+            "Location": self.task_config.Location,
+            "ProjectID": self.task_config.ProjectID,
+        }
+        if self.task_config.QueryJobConfig is not None:
+            config.update(self.task_config.QueryJobConfig.to_api_repr()["query"])
+        s = Struct()
+        s.update(config)
+        return json_format.MessageToDict(s)
+
+    def get_sql(self, settings: SerializationSettings) -> Optional[_task_model.Sql]:
+        sql = _task_model.Sql(statement=self.query_template, dialect=_task_model.Sql.Dialect.ANSI)
+        return sql
```

### Comparing `flytekitplugins-bigquery-1.9.0a0/flytekitplugins_bigquery.egg-info/PKG-INFO` & `flytekitplugins-bigquery-1.9.1/flytekitplugins_bigquery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-bigquery
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This package holds the Bigquery plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-bigquery-1.9.0a0/setup.py` & `flytekitplugins-bigquery-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "bigquery"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "google-cloud-bigquery"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package holds the Bigquery plugins for flytekit",
```

