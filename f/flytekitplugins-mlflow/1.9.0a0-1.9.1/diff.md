# Comparing `tmp/flytekitplugins-mlflow-1.9.0a0.tar.gz` & `tmp/flytekitplugins-mlflow-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-mlflow-1.9.0a0.tar", last modified: Thu Jul 20 18:58:22 2023, max compression
+gzip compressed data, was "flytekitplugins-mlflow-1.9.1.tar", last modified: Mon Aug 28 16:43:09 2023, max compression
```

## Comparing `flytekitplugins-mlflow-1.9.0a0.tar` & `flytekitplugins-mlflow-1.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:22.112706 flytekitplugins-mlflow-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-20 18:58:22.112706 flytekitplugins-mlflow-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-20 18:57:54.000000 flytekitplugins-mlflow-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:22.108706 flytekitplugins-mlflow-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:22.108706 flytekitplugins-mlflow-1.9.0a0/flytekitplugins/mlflow/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-20 18:57:54.000000 flytekitplugins-mlflow-1.9.0a0/flytekitplugins/mlflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-07-20 18:57:54.000000 flytekitplugins-mlflow-1.9.0a0/flytekitplugins/mlflow/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:22.112706 flytekitplugins-mlflow-1.9.0a0/flytekitplugins_mlflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-20 18:58:22.000000 flytekitplugins-mlflow-1.9.0a0/flytekitplugins_mlflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-20 18:58:22.000000 flytekitplugins-mlflow-1.9.0a0/flytekitplugins_mlflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:22.000000 flytekitplugins-mlflow-1.9.0a0/flytekitplugins_mlflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:22.000000 flytekitplugins-mlflow-1.9.0a0/flytekitplugins_mlflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 18:58:22.000000 flytekitplugins-mlflow-1.9.0a0/flytekitplugins_mlflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:22.000000 flytekitplugins-mlflow-1.9.0a0/flytekitplugins_mlflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:22.112706 flytekitplugins-mlflow-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-20 18:58:12.000000 flytekitplugins-mlflow-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:09.606126 flytekitplugins-mlflow-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      818 2023-08-28 16:43:09.606126 flytekitplugins-mlflow-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      588 2023-08-28 16:42:38.000000 flytekitplugins-mlflow-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:09.602126 flytekitplugins-mlflow-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:09.602126 flytekitplugins-mlflow-1.9.1/flytekitplugins/mlflow/
+-rw-r--r--   0 runner    (1001) docker     (999)      242 2023-08-28 16:42:38.000000 flytekitplugins-mlflow-1.9.1/flytekitplugins/mlflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4973 2023-08-28 16:42:38.000000 flytekitplugins-mlflow-1.9.1/flytekitplugins/mlflow/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:09.606126 flytekitplugins-mlflow-1.9.1/flytekitplugins_mlflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      818 2023-08-28 16:43:09.000000 flytekitplugins-mlflow-1.9.1/flytekitplugins_mlflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      372 2023-08-28 16:43:09.000000 flytekitplugins-mlflow-1.9.1/flytekitplugins_mlflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:09.000000 flytekitplugins-mlflow-1.9.1/flytekitplugins_mlflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:09.000000 flytekitplugins-mlflow-1.9.1/flytekitplugins_mlflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       37 2023-08-28 16:43:09.000000 flytekitplugins-mlflow-1.9.1/flytekitplugins_mlflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:09.000000 flytekitplugins-mlflow-1.9.1/flytekitplugins_mlflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:09.606126 flytekitplugins-mlflow-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1182 2023-08-28 16:43:00.000000 flytekitplugins-mlflow-1.9.1/setup.py
```

### Comparing `flytekitplugins-mlflow-1.9.0a0/PKG-INFO` & `flytekitplugins-mlflow-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mlflow
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This package enables seamless use of MLFlow within Flyte
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-mlflow-1.9.0a0/README.md` & `flytekitplugins-mlflow-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-mlflow-1.9.0a0/flytekitplugins/mlflow/tracking.py` & `flytekitplugins-mlflow-1.9.1/flytekitplugins/mlflow/tracking.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from mlflow import MlflowClient
 from mlflow.entities.metric import Metric
 from plotly.subplots import make_subplots
 
 import flytekit
 from flytekit import FlyteContextManager
 from flytekit.bin.entrypoint import get_one_of
-from flytekit.core.context_manager import ExecutionState
 from flytekit.deck.renderer import TopFrameRenderer
 
 
 def metric_to_df(metrics: typing.List[Metric]) -> pd.DataFrame:
     """
     Converts mlflow Metric object to a dataframe of 2 columns ['timestamp', 'value']
     """
@@ -110,16 +109,16 @@
         framework.autolog()
         params = FlyteContextManager.current_context().user_space_params
         ctx = FlyteContextManager.current_context()
 
         experiment = experiment_name or "local workflow"
         run_name = None  # MLflow will generate random name if value is None
 
-        if ctx.execution_state.mode != ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
-            experiment = experiment_name and f"{get_one_of('FLYTE_INTERNAL_EXECUTION_WORKFLOW', '_F_WF')}"
+        if not ctx.execution_state.is_local_execution():
+            experiment = f"{get_one_of('FLYTE_INTERNAL_EXECUTION_WORKFLOW', '_F_WF')}" or experiment_name
             run_name = f"{params.execution_id.name}.{params.task_id.name.split('.')[-1]}"
 
         mlflow.set_experiment(experiment)
         with mlflow.start_run(run_name=run_name):
             out = fn(*args, **kwargs)
             run = mlflow.active_run()
             if run is not None:
```

### Comparing `flytekitplugins-mlflow-1.9.0a0/flytekitplugins_mlflow.egg-info/PKG-INFO` & `flytekitplugins-mlflow-1.9.1/flytekitplugins_mlflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mlflow
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This package enables seamless use of MLFlow within Flyte
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-mlflow-1.9.0a0/setup.py` & `flytekitplugins-mlflow-1.9.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "mlflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.1.0,<2.0.0", "plotly", "mlflow"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables seamless use of MLFlow within Flyte",
```

