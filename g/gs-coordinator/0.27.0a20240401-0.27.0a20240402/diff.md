# Comparing `tmp/gs_coordinator-0.27.0a20240401-py2.py3-none-macosx_12_0_x86_64.whl.zip` & `tmp/gs_coordinator-0.27.0a20240402-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,50 +1,40 @@
-Zip file size: 102179 bytes, number of entries: 48
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 graphscope_runtime/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 gs_coordinator-0.27.0a20240401.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 gscoordinator/
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-01 20:24 graphscope_runtime/__init__.py
--rw-rw-r--  2.0 unx     3451 b- defN 24-Apr-01 21:32 gs_coordinator-0.27.0a20240401.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 24-Apr-01 21:25 gs_coordinator-0.27.0a20240401.dist-info/WHEEL
--rw-r--r--  2.0 unx       33 b- defN 24-Apr-01 21:25 gs_coordinator-0.27.0a20240401.dist-info/top_level.txt
--rw-r--r--  2.0 unx    23840 b- defN 24-Apr-01 21:25 gs_coordinator-0.27.0a20240401.dist-info/METADATA
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 gscoordinator/template/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 gscoordinator/servicer/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 gscoordinator/builtin/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 gscoordinator/hook/
--rw-r--r--  2.0 unx    54960 b- defN 24-Apr-01 20:24 gscoordinator/kubernetes_launcher.py
--rw-r--r--  2.0 unx     5450 b- defN 24-Apr-01 20:24 gscoordinator/coordinator.py
--rw-r--r--  2.0 unx     5702 b- defN 24-Apr-01 20:24 gscoordinator/dag_manager.py
--rw-r--r--  2.0 unx     1045 b- defN 24-Apr-01 20:24 gscoordinator/version.py
--rw-r--r--  2.0 unx     6950 b- defN 24-Apr-01 20:24 gscoordinator/monitor.py
--rw-r--r--  2.0 unx    43296 b- defN 24-Apr-01 20:24 gscoordinator/op_executor.py
--rw-r--r--  2.0 unx     2653 b- defN 24-Apr-01 20:24 gscoordinator/object_manager.py
--rw-r--r--  2.0 unx     4351 b- defN 24-Apr-01 20:24 gscoordinator/operator_launcher.py
--rw-r--r--  2.0 unx      343 b- defN 24-Apr-01 20:24 gscoordinator/constants.py
--rw-r--r--  2.0 unx      990 b- defN 24-Apr-01 20:24 gscoordinator/__init__.py
--rw-r--r--  2.0 unx    21916 b- defN 24-Apr-01 20:24 gscoordinator/cluster_builder.py
--rw-r--r--  2.0 unx    22198 b- defN 24-Apr-01 20:24 gscoordinator/local_launcher.py
--rw-r--r--  2.0 unx     2975 b- defN 24-Apr-01 20:24 gscoordinator/launch_graphlearn_torch.py
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-01 20:30 gscoordinator/VERSION
--rw-r--r--  2.0 unx    80235 b- defN 24-Apr-01 20:24 gscoordinator/utils.py
--rw-r--r--  2.0 unx     4091 b- defN 24-Apr-01 20:24 gscoordinator/io_utils.py
--rw-r--r--  2.0 unx     5372 b- defN 24-Apr-01 20:24 gscoordinator/launcher.py
--rw-r--r--  2.0 unx     2494 b- defN 24-Apr-01 20:24 gscoordinator/launch_graphlearn.py
--rw-r--r--  2.0 unx       77 b- defN 24-Apr-01 20:24 gscoordinator/__main__.py
--rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 20:24 gscoordinator/template/__init__.py
--rw-r--r--  2.0 unx     4340 b- defN 24-Apr-01 20:24 gscoordinator/template/pregel.pxd.template
--rw-r--r--  2.0 unx     4957 b- defN 24-Apr-01 20:24 gscoordinator/template/pie.pxd.template
--rw-r--r--  2.0 unx    22656 b- defN 24-Apr-01 20:24 gscoordinator/template/CMakeLists.template
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 gscoordinator/servicer/graphscope_one/
--rw-r--r--  2.0 unx      707 b- defN 24-Apr-01 20:24 gscoordinator/servicer/__init__.py
--rw-r--r--  2.0 unx    24792 b- defN 24-Apr-01 20:24 gscoordinator/servicer/graphscope_one/service.py
--rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 20:24 gscoordinator/servicer/graphscope_one/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 gscoordinator/builtin/app/
--rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 20:24 gscoordinator/builtin/__init__.py
--rw-r--r--  2.0 unx    25282 b- defN 24-Apr-01 20:24 gscoordinator/builtin/app/.gs_conf.yaml
--rw-r--r--  2.0 unx     5715 b- defN 24-Apr-01 21:25 gscoordinator/builtin/app/builtin_app.gar
--rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 20:24 gscoordinator/builtin/app/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 21:32 gscoordinator/hook/prestop/
--rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 20:24 gscoordinator/hook/__init__.py
--rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 20:24 gscoordinator/hook/prestop/__init__.py
--rw-r--r--  2.0 unx     1560 b- defN 24-Apr-01 20:24 gscoordinator/hook/prestop/__main__.py
-48 files, 387157 bytes uncompressed, 95387 bytes compressed:  75.4%
+Zip file size: 102969 bytes, number of entries: 38
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-02 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-02 19:06 gscoordinator/VERSION
+-rw-r--r--  2.0 unx      990 b- defN 24-Apr-02 19:01 gscoordinator/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 24-Apr-02 19:01 gscoordinator/__main__.py
+-rw-r--r--  2.0 unx    24165 b- defN 24-Apr-02 19:01 gscoordinator/cluster_builder.py
+-rw-r--r--  2.0 unx      400 b- defN 24-Apr-02 19:01 gscoordinator/constants.py
+-rw-r--r--  2.0 unx     5450 b- defN 24-Apr-02 19:01 gscoordinator/coordinator.py
+-rw-r--r--  2.0 unx     5702 b- defN 24-Apr-02 19:01 gscoordinator/dag_manager.py
+-rw-r--r--  2.0 unx     4091 b- defN 24-Apr-02 19:01 gscoordinator/io_utils.py
+-rw-r--r--  2.0 unx    66027 b- defN 24-Apr-02 19:01 gscoordinator/kubernetes_launcher.py
+-rw-r--r--  2.0 unx     2494 b- defN 24-Apr-02 19:01 gscoordinator/launch_graphlearn.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-Apr-02 19:01 gscoordinator/launch_graphlearn_torch.py
+-rw-r--r--  2.0 unx     5395 b- defN 24-Apr-02 19:01 gscoordinator/launcher.py
+-rw-r--r--  2.0 unx    22431 b- defN 24-Apr-02 19:01 gscoordinator/local_launcher.py
+-rw-r--r--  2.0 unx     6950 b- defN 24-Apr-02 19:01 gscoordinator/monitor.py
+-rw-r--r--  2.0 unx     2761 b- defN 24-Apr-02 19:01 gscoordinator/object_manager.py
+-rw-r--r--  2.0 unx    43296 b- defN 24-Apr-02 19:01 gscoordinator/op_executor.py
+-rw-r--r--  2.0 unx     4369 b- defN 24-Apr-02 19:01 gscoordinator/operator_launcher.py
+-rw-r--r--  2.0 unx    80684 b- defN 24-Apr-02 19:01 gscoordinator/utils.py
+-rw-r--r--  2.0 unx     1045 b- defN 24-Apr-02 19:01 gscoordinator/version.py
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-02 19:01 gscoordinator/builtin/__init__.py
+-rw-r--r--  2.0 unx    25282 b- defN 24-Apr-02 19:01 gscoordinator/builtin/app/.gs_conf.yaml
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-02 19:01 gscoordinator/builtin/app/__init__.py
+-rw-r--r--  2.0 unx     5264 b- defN 24-Apr-02 20:04 gscoordinator/builtin/app/builtin_app.gar
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-02 19:01 gscoordinator/hook/__init__.py
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-02 19:01 gscoordinator/hook/prestop/__init__.py
+-rw-r--r--  2.0 unx     1560 b- defN 24-Apr-02 19:01 gscoordinator/hook/prestop/__main__.py
+-rw-r--r--  2.0 unx      707 b- defN 24-Apr-02 19:01 gscoordinator/servicer/__init__.py
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-02 19:01 gscoordinator/servicer/graphscope_one/__init__.py
+-rw-r--r--  2.0 unx    24964 b- defN 24-Apr-02 19:01 gscoordinator/servicer/graphscope_one/service.py
+-rw-r--r--  2.0 unx    22656 b- defN 24-Apr-02 19:01 gscoordinator/template/CMakeLists.template
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-02 19:01 gscoordinator/template/__init__.py
+-rw-r--r--  2.0 unx     4957 b- defN 24-Apr-02 19:01 gscoordinator/template/pie.pxd.template
+-rw-r--r--  2.0 unx     4340 b- defN 24-Apr-02 19:01 gscoordinator/template/pregel.pxd.template
+-rw-r--r--  2.0 unx    23840 b- defN 24-Apr-02 20:04 gs_coordinator-0.27.0a20240402.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-02 20:04 gs_coordinator-0.27.0a20240402.dist-info/WHEEL
+-rw-r--r--  2.0 unx       33 b- defN 24-Apr-02 20:04 gs_coordinator-0.27.0a20240402.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     3413 b- defN 24-Apr-02 20:04 gs_coordinator-0.27.0a20240402.dist-info/RECORD
+38 files, 401916 bytes uncompressed, 97441 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -1,145 +1,115 @@
-Filename: graphscope_runtime/
-Comment: 
-
-Filename: gs_coordinator-0.27.0a20240401.dist-info/
-Comment: 
-
-Filename: gscoordinator/
-Comment: 
-
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_coordinator-0.27.0a20240401.dist-info/RECORD
-Comment: 
-
-Filename: gs_coordinator-0.27.0a20240401.dist-info/WHEEL
-Comment: 
-
-Filename: gs_coordinator-0.27.0a20240401.dist-info/top_level.txt
-Comment: 
-
-Filename: gs_coordinator-0.27.0a20240401.dist-info/METADATA
-Comment: 
-
-Filename: gscoordinator/template/
+Filename: gscoordinator/VERSION
 Comment: 
 
-Filename: gscoordinator/servicer/
+Filename: gscoordinator/__init__.py
 Comment: 
 
-Filename: gscoordinator/builtin/
+Filename: gscoordinator/__main__.py
 Comment: 
 
-Filename: gscoordinator/hook/
+Filename: gscoordinator/cluster_builder.py
 Comment: 
 
-Filename: gscoordinator/kubernetes_launcher.py
+Filename: gscoordinator/constants.py
 Comment: 
 
 Filename: gscoordinator/coordinator.py
 Comment: 
 
 Filename: gscoordinator/dag_manager.py
 Comment: 
 
-Filename: gscoordinator/version.py
-Comment: 
-
-Filename: gscoordinator/monitor.py
+Filename: gscoordinator/io_utils.py
 Comment: 
 
-Filename: gscoordinator/op_executor.py
+Filename: gscoordinator/kubernetes_launcher.py
 Comment: 
 
-Filename: gscoordinator/object_manager.py
+Filename: gscoordinator/launch_graphlearn.py
 Comment: 
 
-Filename: gscoordinator/operator_launcher.py
+Filename: gscoordinator/launch_graphlearn_torch.py
 Comment: 
 
-Filename: gscoordinator/constants.py
+Filename: gscoordinator/launcher.py
 Comment: 
 
-Filename: gscoordinator/__init__.py
+Filename: gscoordinator/local_launcher.py
 Comment: 
 
-Filename: gscoordinator/cluster_builder.py
+Filename: gscoordinator/monitor.py
 Comment: 
 
-Filename: gscoordinator/local_launcher.py
+Filename: gscoordinator/object_manager.py
 Comment: 
 
-Filename: gscoordinator/launch_graphlearn_torch.py
+Filename: gscoordinator/op_executor.py
 Comment: 
 
-Filename: gscoordinator/VERSION
+Filename: gscoordinator/operator_launcher.py
 Comment: 
 
 Filename: gscoordinator/utils.py
 Comment: 
 
-Filename: gscoordinator/io_utils.py
-Comment: 
-
-Filename: gscoordinator/launcher.py
+Filename: gscoordinator/version.py
 Comment: 
 
-Filename: gscoordinator/launch_graphlearn.py
+Filename: gscoordinator/builtin/__init__.py
 Comment: 
 
-Filename: gscoordinator/__main__.py
+Filename: gscoordinator/builtin/app/.gs_conf.yaml
 Comment: 
 
-Filename: gscoordinator/template/__init__.py
+Filename: gscoordinator/builtin/app/__init__.py
 Comment: 
 
-Filename: gscoordinator/template/pregel.pxd.template
+Filename: gscoordinator/builtin/app/builtin_app.gar
 Comment: 
 
-Filename: gscoordinator/template/pie.pxd.template
+Filename: gscoordinator/hook/__init__.py
 Comment: 
 
-Filename: gscoordinator/template/CMakeLists.template
+Filename: gscoordinator/hook/prestop/__init__.py
 Comment: 
 
-Filename: gscoordinator/servicer/graphscope_one/
+Filename: gscoordinator/hook/prestop/__main__.py
 Comment: 
 
 Filename: gscoordinator/servicer/__init__.py
 Comment: 
 
-Filename: gscoordinator/servicer/graphscope_one/service.py
-Comment: 
-
 Filename: gscoordinator/servicer/graphscope_one/__init__.py
 Comment: 
 
-Filename: gscoordinator/builtin/app/
+Filename: gscoordinator/servicer/graphscope_one/service.py
 Comment: 
 
-Filename: gscoordinator/builtin/__init__.py
+Filename: gscoordinator/template/CMakeLists.template
 Comment: 
 
-Filename: gscoordinator/builtin/app/.gs_conf.yaml
+Filename: gscoordinator/template/__init__.py
 Comment: 
 
-Filename: gscoordinator/builtin/app/builtin_app.gar
+Filename: gscoordinator/template/pie.pxd.template
 Comment: 
 
-Filename: gscoordinator/builtin/app/__init__.py
+Filename: gscoordinator/template/pregel.pxd.template
 Comment: 
 
-Filename: gscoordinator/hook/prestop/
+Filename: gs_coordinator-0.27.0a20240402.dist-info/METADATA
 Comment: 
 
-Filename: gscoordinator/hook/__init__.py
+Filename: gs_coordinator-0.27.0a20240402.dist-info/WHEEL
 Comment: 
 
-Filename: gscoordinator/hook/prestop/__init__.py
+Filename: gs_coordinator-0.27.0a20240402.dist-info/top_level.txt
 Comment: 
 
-Filename: gscoordinator/hook/prestop/__main__.py
+Filename: gs_coordinator-0.27.0a20240402.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## gscoordinator/kubernetes_launcher.py

```diff
@@ -23,14 +23,16 @@
 import os
 import random
 import shlex
 import subprocess
 import sys
 import time
 
+from graphscope.proto import message_pb2
+
 from gscoordinator.cluster_builder import EngineCluster
 from gscoordinator.cluster_builder import MarsCluster
 
 try:
     from kubernetes import client as kube_client
     from kubernetes import config as kube_config
     from kubernetes import watch as kube_watch
@@ -52,24 +54,26 @@
 from graphscope.deploy.kubernetes.utils import get_kubernetes_object_info
 from graphscope.deploy.kubernetes.utils import resolve_api_client
 from graphscope.framework.utils import PipeWatcher
 from graphscope.framework.utils import get_tempdir
 from graphscope.proto import types_pb2
 
 from gscoordinator.constants import ANALYTICAL_CONTAINER_NAME
+from gscoordinator.constants import GRAPHLEARN_CONTAINER_NAME
+from gscoordinator.constants import GRAPHLEARN_TORCH_CONTAINER_NAME
 from gscoordinator.constants import INTERACTIVE_EXECUTOR_CONTAINER_NAME
-from gscoordinator.constants import LEARNING_CONTAINER_NAME
 from gscoordinator.launcher import AbstractLauncher
 from gscoordinator.utils import ANALYTICAL_ENGINE_PATH
 from gscoordinator.utils import GRAPHSCOPE_HOME
 from gscoordinator.utils import INTERACTIVE_ENGINE_SCRIPT
 from gscoordinator.utils import WORKSPACE
 from gscoordinator.utils import ResolveMPICmdPrefix
 from gscoordinator.utils import delegate_command_to_pod
 from gscoordinator.utils import parse_as_glog_level
+from gscoordinator.utils import replace_string_in_dict
 from gscoordinator.utils import run_kube_cp_command
 
 logger = logging.getLogger("graphscope")
 
 
 class FakeKubeResponse:
     def __init__(self, obj):
@@ -80,14 +84,15 @@
     def __init__(self, config: Config):
         super().__init__()
         self._serving = False
 
         self._api_client = resolve_api_client()
         self._core_api = kube_client.CoreV1Api(self._api_client)
         self._apps_api = kube_client.AppsV1Api(self._api_client)
+        self._pytorchjobs_api = kube_client.CustomObjectsApi(self._api_client)
         self._resource_object = ResourceManager(self._api_client)
 
         self._config: Config = config
         self._config.kubernetes_launcher.engine.post_setup()
         launcher_config = config.kubernetes_launcher
 
         # glog level
@@ -188,35 +193,45 @@
         self._analytical_java_pod_ip = []
         self._analytical_java_pod_host_ip = []
         # interactive engine
         self._interactive_resource_object = {}
         self._interactive_pod_name = {}
         self._interactive_pod_ip = {}
         self._interactive_pod_host_ip = {}
-        # learning engine
-        self._learning_resource_object = {}
-        self._learning_pod_name = {}
-        self._learning_pod_ip = {}
-        self._learning_pod_host_ip = {}
+        # graphlearn engine
+        self._graphlearn_resource_object = {}
+        self._graphlearn_pod_name = {}
+        self._graphlearn_pod_ip = {}
+        self._graphlearn_pod_host_ip = {}
+        # graphlearn_torch engine
+        self._graphlearn_torch_resource_object = {}
+        self._graphlearn_torch_pod_name = {}
+        self._graphlearn_torch_pod_ip = {}
+        self._graphlearn_torch_pod_host_ip = {}
 
         self._analytical_engine_endpoint = None
         self._mars_service_endpoint = None
 
         self._analytical_engine_process = None
         self._random_analytical_engine_rpc_port = random.randint(56001, 57000)
         # interactive engine
         # executor inter-processing port
         # executor rpc port
         # frontend port
         self._interactive_port = 8233
         # 8000 ~ 9000 is exposed
-        self._learning_start_port = 8000
+        self._graphlearn_start_port = 8000
+        # 9001 ~ 10001 is exposed
+        self._graphlearn_torch_start_port = 9001
 
         self._graphlearn_services = {}
-        self._learning_instance_processes = {}
+        self._graphlearn_instance_processes = {}
+
+        self._graphlearn_torch_services = {}
+        self._graphlearn_torch_instance_processes = {}
 
         # workspace
         self._instance_workspace = os.path.join(WORKSPACE, self._instance_id)
         os.makedirs(self._instance_workspace, exist_ok=True)
         self._session_workspace = None
 
         self._engine_cluster = self._build_engine_cluster()
@@ -238,15 +253,16 @@
 
     # the argument `with_analytical_` means whether to add the analytical engine
     # container to the engine statefulsets, and the other three arguments are similar.
     def _build_engine_cluster(self):
         return EngineCluster(
             config=self._config,
             engine_pod_prefix=self._engine_pod_prefix,
-            learning_start_port=self._learning_start_port,
+            graphlearn_start_port=self._graphlearn_start_port,
+            graphlearn_torch_start_port=self._graphlearn_torch_start_port,
         )
 
     def get_coordinator_owner_references(self):
         owner_references = []
         if self._coordinator_name:
             try:
                 deployment = self._apps_api.read_namespaced_deployment(
@@ -386,15 +402,18 @@
             self._config.kubernetes_launcher.engine.enable_gae_java = (
                 engine_type == "analytical-java"
             )
             self._config.kubernetes_launcher.engine.enable_gie = (
                 engine_type == "interactive"
             )
             self._config.kubernetes_launcher.engine.enable_gle = (
-                engine_type == "learning"
+                engine_type == "graphlearn"
+            )
+            self._config.kubernetes_launcher.engine.enable_glt = (
+                engine_type == "graphlearn-torch"
             )
 
             self._engine_cluster = self._build_engine_cluster()
             response = self._create_engine_stateful_set()
             self._waiting_for_services_ready()
 
             if object_id:
@@ -483,22 +502,28 @@
             )
         ]
         name = f"gs-interactive-frontend-{object_id}-{self._instance_id}"
         self._create_frontend_deployment(name, owner_references)
 
         return pod_name_list, pod_ip_list, pod_host_ip_list
 
-    def deploy_learning_engine(self, object_id):
-        return self.deploy_engine("learning", object_id)
+    def deploy_graphlearn_engine(self, object_id):
+        return self.deploy_engine("graphlearn", object_id)
+
+    def deploy_graphlearn_torch_engine(self, object_id):
+        return self.deploy_engine("graphlearn-torch", object_id)
 
     def delete_interactive_engine(self, object_id):
         self.delete_engine_stateful_set_with_object_id("interactive", object_id)
 
-    def delete_learning_engine(self, object_id):
-        self.delete_engine_stateful_set_with_object_id("learning", object_id)
+    def delete_graphlearn_engine(self, object_id):
+        self.delete_engine_stateful_set_with_object_id("graphlearn", object_id)
+
+    def delete_graphlearn_torch_engine(self, object_id):
+        self.delete_engine_stateful_set_with_object_id("graphlearn-torch", object_id)
 
     def _allocate_interactive_engine(self, object_id):
         # check the interactive engine flag
         if not self._config.kubernetes_launcher.engine.enable_gie:
             raise NotImplementedError("Interactive engine not enabled")
 
         # allocate analytical engine based on the mode
@@ -844,24 +869,34 @@
     def _create_frontend_service(self):
         logger.info("Creating frontend service...")
         service = self._engine_cluster.get_interactive_frontend_service(8233, 7687)
         service.metadata.owner_references = self._owner_references
         response = self._core_api.create_namespaced_service(self._namespace, service)
         self._resource_object.append(response)
 
-    def _create_learning_service(self, object_id):
-        logger.info("Creating learning service...")
-        service = self._engine_cluster.get_learning_service(
-            object_id, self._learning_start_port
+    def _create_graphlearn_service(self, object_id):
+        logger.info("Creating graphlearn service...")
+        service = self._engine_cluster.get_graphlearn_service(
+            object_id, self._graphlearn_start_port
         )
         service.metadata.owner_references = self._owner_references
         response = self._core_api.create_namespaced_service(self._namespace, service)
         self._graphlearn_services[object_id] = response
         self._resource_object.append(response)
 
+    def _create_graphlearn_torch_service(self, object_id):
+        logger.info("Creating graphlearn torch service...")
+        service = self._engine_cluster.get_graphlearn_torch_service(
+            object_id, self._graphlearn_torch_start_port
+        )
+        service.metadata.owner_references = self._owner_references
+        response = self._core_api.create_namespaced_service(self._namespace, service)
+        self._graphlearn_torch_services[object_id] = response
+        self._resource_object.append(response)
+
     def get_engine_config(self):
         config = {
             "vineyard_service_name": self._engine_cluster.vineyard_service_name,
             "vineyard_rpc_endpoint": self._vineyard_service_endpoint,
         }
         if self._config.kubernetes_launcher.mars.enable:
             config["mars_endpoint"] = self._mars_service_endpoint
@@ -1257,55 +1292,67 @@
 
                 else:
                     # delete coordinator deployment and service
                     self._delete_dangling_coordinator()
             self._serving = False
             logger.info("Kubernetes launcher stopped")
 
-    def _allocate_learning_engine(self, object_id):
-        # check the learning engine flag
+    def _allocate_graphlearn_engine(self, object_id):
+        # check the graphlearn engine flag
         if not self._config.kubernetes_launcher.engine.enable_gle:
-            raise NotImplementedError("Learning engine not enabled")
+            raise NotImplementedError("GraphLearn engine not enabled")
+
+        # allocate graphlearn engine based on the mode
+        if self._deploy_mode == "eager":
+            return self._pod_name_list, self._pod_ip_list, self._pod_host_ip_list
+        return self.deploy_graphlearn_engine(object_id)
 
-        # allocate learning engine based on the mode
+    def _allocate_graphlearn_torch_engine(self, object_id):
+        # check the graphlearn torch engine flag
+        if not self._config.kubernetes_launcher.engine.enable_glt:
+            raise NotImplementedError("GraphLearn torch engine not enabled")
+
+        # allocate graphlearn engine based on the mode
         if self._deploy_mode == "eager":
             return self._pod_name_list, self._pod_ip_list, self._pod_host_ip_list
-        return self.deploy_learning_engine(object_id)
+        return self.deploy_graphlearn_torch_engine(object_id)
 
-    def _distribute_learning_process(
+    def _distribute_graphlearn_process(
         self, pod_name_list, pod_host_ip_list, object_id, handle, config
     ):
         # allocate service for ports
         # prepare arguments
         handle = json.loads(
             base64.b64decode(handle.encode("utf-8", errors="ignore")).decode(
                 "utf-8", errors="ignore"
             )
         )
         hosts = ",".join(
             [
                 f"{pod_name}:{port}"
                 for pod_name, port in zip(
                     pod_name_list,
-                    self._engine_cluster.get_learning_ports(self._learning_start_port),
+                    self._engine_cluster.get_graphlearn_ports(
+                        self._graphlearn_start_port
+                    ),
                 )
             ]
         )
         handle["server"] = hosts
         handle = base64.b64encode(
             json.dumps(handle).encode("utf-8", errors="ignore")
         ).decode("utf-8", errors="ignore")
 
         # launch the server
-        self._learning_instance_processes[object_id] = []
+        self._graphlearn_instance_processes[object_id] = []
         for pod_index, pod in enumerate(self._pod_name_list):
-            container = LEARNING_CONTAINER_NAME
+            container = GRAPHLEARN_CONTAINER_NAME
             sub_cmd = f"python3 -m gscoordinator.launch_graphlearn {handle} {config} {pod_index}"
             cmd = f"kubectl -n {self._namespace} exec -it -c {container} {pod} -- {sub_cmd}"
-            logger.debug("launching learning server: %s", " ".join(cmd))
+            # logger.debug("launching learning server: %s", " ".join(cmd))
             proc = subprocess.Popen(
                 shlex.split(cmd),
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
                 encoding="utf-8",
                 errors="replace",
                 universal_newlines=True,
@@ -1314,59 +1361,275 @@
             stdout_watcher = PipeWatcher(
                 proc.stdout,
                 sys.stdout,
                 drop=True,
                 suppressed=(not logger.isEnabledFor(logging.DEBUG)),
             )
             setattr(proc, "stdout_watcher", stdout_watcher)
-            self._learning_instance_processes[object_id].append(proc)
+            self._graphlearn_instance_processes[object_id].append(proc)
 
         # Create Service
-        self._create_learning_service(object_id)
+        self._create_graphlearn_service(object_id)
         # update the port usage record
-        self._learning_start_port += len(pod_name_list)
+        self._graphlearn_start_port += len(pod_name_list)
         # parse the service hosts and ports
         return self._engine_cluster.get_graphlearn_service_endpoint(
             self._api_client, object_id, pod_host_ip_list
         )
 
-    def create_learning_instance(self, object_id, handle, config, learning_backend):
-        pod_name_list, _, pod_host_ip_list = self._allocate_learning_engine(object_id)
-        if not pod_name_list or not pod_host_ip_list:
-            raise RuntimeError("Failed to allocate learning engine")
-        return self._distribute_learning_process(
-            pod_name_list, pod_host_ip_list, object_id, handle, config
+    def _distribute_graphlearn_torch_process(
+        self, pod_name_list, pod_ip_list, object_id, handle, config
+    ):
+        # allocate service for ports
+        # prepare arguments
+        handle = json.loads(
+            base64.b64decode(handle.encode("utf-8", errors="ignore")).decode(
+                "utf-8", errors="ignore"
+            )
+        )
+
+        ports = self._engine_cluster.get_graphlearn_torch_ports(
+            self._graphlearn_torch_start_port
         )
+        handle["master_addr"] = pod_ip_list[0]
+        handle["server_client_master_port"] = ports[0]
+        server_list = [f"{pod_ip_list[0]}:{ports[i]}" for i in range(4)]
+
+        server_handle = base64.b64encode(
+            json.dumps(handle).encode("utf-8", errors="ignore")
+        ).decode("utf-8", errors="ignore")
+
+        # launch the server
+        self._graphlearn_torch_instance_processes[object_id] = []
+        for pod_index, pod in enumerate(self._pod_name_list):
+            container = GRAPHLEARN_TORCH_CONTAINER_NAME
+            sub_cmd = f"env PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python \
+                python3 -m gscoordinator.launch_graphlearn_torch \
+                {server_handle} {config} {pod_index}"
+            cmd = f"kubectl -n {self._namespace} exec -it -c {container} {pod} -- {sub_cmd}"
+            # logger.debug("launching learning server: %s", " ".join(cmd))
+            proc = subprocess.Popen(
+                shlex.split(cmd),
+                stdout=subprocess.PIPE,
+                stderr=subprocess.STDOUT,
+                encoding="utf-8",
+                errors="replace",
+                universal_newlines=True,
+                bufsize=1,
+            )
+            stdout_watcher = PipeWatcher(
+                proc.stdout,
+                sys.stdout,
+                suppressed=(not logger.isEnabledFor(logging.DEBUG)),
+            )
+
+            time.sleep(5)
+            logger.debug("process status: %s", proc.poll())
 
-    def close_learning_instance(self, object_id):
+            setattr(proc, "stdout_watcher", stdout_watcher)
+            self._graphlearn_torch_instance_processes[object_id].append(proc)
+
+        # Create Service
+        self._create_graphlearn_torch_service(object_id)
+        # update the port usage record
+        self._graphlearn_torch_start_port += len(pod_name_list)
+
+        # prepare config map for client scripts
+        config_map = kube_client.V1ConfigMap(
+            api_version="v1",
+            kind="ConfigMap",
+            metadata=kube_client.V1ObjectMeta(
+                name="graphlearn-torch-client-config",
+                namespace=self._namespace,
+            ),
+            data=handle["client_content"],
+        )
+        self._core_api.create_namespaced_config_map(self._namespace, config_map)
+
+        # prepare the manifest
+        pytorch_job_manifest = replace_string_in_dict(
+            handle["manifest"], "${MASTER_ADDR}", handle["master_addr"]
+        )
+        # parse the pytorchjob yaml
+        group = pytorch_job_manifest["apiVersion"].split("/")[0]
+        version = pytorch_job_manifest["apiVersion"].split("/")[1]
+        name = pytorch_job_manifest["metadata"]["name"]
+        namespace = pytorch_job_manifest["metadata"]["namespace"]
+        plural = "pytorchjobs"  # This is PyTorchJob CRD's plural name
+
+        try:
+            # create PyTorchJob
+            api_response = self._pytorchjobs_api.create_namespaced_custom_object(
+                group=group,
+                version=version,
+                namespace=namespace,
+                plural=plural,
+                body=pytorch_job_manifest,
+            )
+            logger.info(api_response)
+        except K8SApiException as e:
+            logger.info(
+                f"Exception when calling CustomObjectsApi->create_namespaced_custom_object: {e}"
+            )
+            raise
+
+        # set Watcher to monitor the state of the PyTorchJob
+        w = kube_watch.Watch()
+
+        # loop checking the state of PyTorchJob
+        for event in w.stream(
+            self._pytorchjobs_api.list_namespaced_custom_object,
+            group,
+            version,
+            namespace,
+            plural,
+        ):
+            pytorch_job = event["object"]
+            if pytorch_job.get("metadata", {}).get("name") == name:
+                status = pytorch_job.get("status", {})
+                if status:  # check status existence
+                    conditions = status.get("conditions", [])
+                    for condition in conditions:
+                        if (
+                            condition.get("type") == "Succeeded"
+                            and condition.get("status") == "True"
+                        ):
+                            logger.info(f"PyTorchJob {name} has succeeded!")
+                            w.stop()
+                            break
+                        elif (
+                            condition.get("type") == "Failed"
+                            and condition.get("status") == "True"
+                        ):
+                            logger.info(f"PyTorchJob {name} has failed!")
+                            w.stop()
+                            break
+
+        self.close_graphlearn_torch_client(group, name, version, plural, namespace)
+
+        return server_list
+
+    def create_learning_instance(self, object_id, handle, config, learning_backend):
+        if learning_backend == message_pb2.LearningBackend.GRAPHLEARN:
+            pod_name_list, _, pod_host_ip_list = self._allocate_graphlearn_engine(
+                object_id
+            )
+            if not pod_name_list or not pod_host_ip_list:
+                raise RuntimeError("Failed to allocate learning engine")
+            return self._distribute_graphlearn_process(
+                pod_name_list, pod_host_ip_list, object_id, handle, config
+            )
+        elif learning_backend == message_pb2.LearningBackend.GRAPHLEARN_TORCH:
+            pod_name_list, pod_ip_list, pod_host_ip_list = (
+                self._allocate_graphlearn_torch_engine(object_id)
+            )
+            if not pod_name_list or not pod_host_ip_list:
+                raise RuntimeError("Failed to allocate learning engine")
+            return self._distribute_graphlearn_torch_process(
+                pod_name_list, pod_ip_list, object_id, handle, config
+            )
+        else:
+            raise ValueError("invalid learning backend")
+
+    def close_learning_instance(self, object_id, learning_backend):
+        if learning_backend == message_pb2.LearningBackend.GRAPHLEARN:
+            self.close_graphlearn_instance(object_id)
+        elif learning_backend == message_pb2.LearningBackend.GRAPHLEARN_TORCH:
+            self.close_graphlearn_torch_instance(object_id)
+        else:
+            raise ValueError("invalid learning backend")
+
+    def close_graphlearn_instance(self, object_id):
         if self._deploy_mode == "lazy":
-            self.delete_learning_engine(object_id)
+            self.delete_graphlearn_engine(object_id)
             return
-        if object_id not in self._learning_instance_processes:
+        if object_id not in self._graphlearn_instance_processes:
             return
         # delete the services
         target = self._graphlearn_services[object_id]
         try:
             delete_kubernetes_object(
                 api_client=self._api_client,
                 target=target,
                 wait=self._waiting_for_delete,
                 timeout_seconds=self._timeout_seconds,
             )
         except Exception:  # pylint: disable=broad-except
             logger.exception("Failed to delete graphlearn service for %s", object_id)
 
         # terminate the process
-        for proc in self._learning_instance_processes[object_id]:
+        for proc in self._graphlearn_instance_processes[object_id]:
             try:
                 proc.terminate()
                 proc.wait(1)
             except Exception:  # pylint: disable=broad-except
                 logger.exception("Failed to terminate graphlearn server")
-        self._learning_instance_processes[object_id].clear()
+        self._graphlearn_instance_processes[object_id].clear()
+
+    def close_graphlearn_torch_instance(self, object_id):
+        if self._deploy_mode == "lazy":
+            self.delete_graphlearn_torch_engine(object_id)
+            return
+        if object_id not in self._graphlearn_torch_instance_processes:
+            return
+        # delete the services
+        target = self._graphlearn_torch_services[object_id]
+        try:
+            delete_kubernetes_object(
+                api_client=self._api_client,
+                target=target,
+                wait=self._waiting_for_delete,
+                timeout_seconds=self._timeout_seconds,
+            )
+        except Exception:  # pylint: disable=broad-except
+            logger.exception(
+                "Failed to delete graphlearn torch service for %s", object_id
+            )
+
+        # terminate the process
+        for proc in self._graphlearn_torch_instance_processes[object_id]:
+            try:
+                proc.terminate()
+                proc.wait(1)
+            except Exception:  # pylint: disable=broad-except
+                logger.exception("Failed to terminate graphlearn torch server")
+        self._graphlearn_torch_instance_processes[object_id].clear()
+
+    def close_graphlearn_torch_client(self, group, name, version, plural, namespace):
+        # clear PyTorchJob
+        logger.info(f"Deleting PyTorchJob {name}...")
+        try:
+            response = self._pytorchjobs_api.delete_namespaced_custom_object(
+                group=group,
+                name=name,
+                version=version,
+                plural=plural,
+                namespace=namespace,
+                body=kube_client.V1DeleteOptions(
+                    propagation_policy="Foreground",
+                ),
+            )
+            logger.info(f"PyTorchJob {name} deleted. Response: {response}")
+        except K8SApiException as e:
+            logger.info(
+                f"Exception when calling CustomObjectsApi->delete_namespaced_custom_object: {e}"
+            )
+
+        try:
+            response = self._core_api.delete_namespaced_config_map(
+                name="graphlearn-torch-client-config",
+                namespace=self._namespace,
+            )
+            logger.info(
+                f"ConfigMap graphlearn-torch-client-config deleted. Response: {response}"
+            )
+        except K8SApiException as e:
+            logger.info(
+                f"Exception when calling CoreV1Api->delete_namespaced_config_map: {e}"
+            )
 
 
 class ResourceManager(object):
     """A class to manager kubernetes object.
 
     Object managed by this class will dump meta info to disk file
     for pod preStop lifecycle management.
```

## gscoordinator/object_manager.py

```diff
@@ -57,16 +57,19 @@
             if self.endpoint is None:
                 raise RuntimeError("InteractiveQueryManager's endpoint cannot be None")
             self.client = Client(f"ws://{self.endpoint}/gremlin", "g")
         return self.client.submit(message, bindings, request_options)
 
 
 class LearningInstanceManager(object):
-    def __init__(self, object_id):
-        self.type = "gle_manager"
+    def __init__(self, object_id, learning_backend):
+        if learning_backend == 0:
+            self.type = "gle_manager"
+        else:
+            self.type = "glt_manager"
         self.object_id = object_id
 
 
 class ObjectManager(object):
     """Manage the objects hold by the coordinator."""
 
     def __init__(self):
```

## gscoordinator/operator_launcher.py

```diff
@@ -91,15 +91,15 @@
 
     def close_analytical_instance(self):
         pass
 
     def close_interactive_instance(self, object_id):
         pass
 
-    def close_learning_instance(self, object_id):
+    def close_learning_instance(self, object_id, learning_backend):
         pass
 
     def launch_etcd(self):
         pass
 
     def launch_vineyard(self):
         pass
```

## gscoordinator/constants.py

```diff
@@ -1,8 +1,9 @@
 # This must be same with v6d:modules/io/python/drivers/io/kube_ssh.sh
 ANALYTICAL_CONTAINER_NAME = "engine"
 INTERACTIVE_FRONTEND_CONTAINER_NAME = "frontend"
 INTERACTIVE_EXECUTOR_CONTAINER_NAME = "executor"
-LEARNING_CONTAINER_NAME = "learning"
+GRAPHLEARN_CONTAINER_NAME = "graphlearn"
+GRAPHLEARN_TORCH_CONTAINER_NAME = "graphlearn-torch"
 DATASET_CONTAINER_NAME = "dataset"
 MARS_CONTAINER_NAME = "mars"
 VINEYARD_CONTAINER_NAME = "vineyard"
```

## gscoordinator/cluster_builder.py

```diff
@@ -29,17 +29,18 @@
 from graphscope.config import Config
 from graphscope.config import KubernetesLauncherConfig
 from graphscope.deploy.kubernetes.resource_builder import ResourceBuilder
 from graphscope.deploy.kubernetes.utils import get_service_endpoints
 
 from gscoordinator.constants import ANALYTICAL_CONTAINER_NAME
 from gscoordinator.constants import DATASET_CONTAINER_NAME
+from gscoordinator.constants import GRAPHLEARN_CONTAINER_NAME
+from gscoordinator.constants import GRAPHLEARN_TORCH_CONTAINER_NAME
 from gscoordinator.constants import INTERACTIVE_EXECUTOR_CONTAINER_NAME
 from gscoordinator.constants import INTERACTIVE_FRONTEND_CONTAINER_NAME
-from gscoordinator.constants import LEARNING_CONTAINER_NAME
 from gscoordinator.utils import parse_as_glog_level
 from gscoordinator.version import __version__
 
 logger = logging.getLogger("graphscope")
 
 BASE_MACHINE_ENVS = {
     "MY_NODE_NAME": "spec.nodeName",
@@ -59,15 +60,16 @@
 
 
 class EngineCluster:
     def __init__(
         self,
         config: Config,
         engine_pod_prefix,
-        learning_start_port,
+        graphlearn_start_port,
+        graphlearn_torch_start_port,
     ):
         self._instance_id = config.session.instance_id
         self._glog_level = parse_as_glog_level(config.log_level)
         self._num_workers = config.session.num_workers
 
         launcher_config: KubernetesLauncherConfig = config.kubernetes_launcher
 
@@ -77,15 +79,16 @@
         self._engine_resources = launcher_config.engine
 
         self._with_dataset = launcher_config.dataset.enable
 
         self._with_analytical = launcher_config.engine.enable_gae
         self._with_analytical_java = launcher_config.engine.enable_gae_java
         self._with_interactive = launcher_config.engine.enable_gie
-        self._with_learning = launcher_config.engine.enable_gle
+        self._with_graphlearn = launcher_config.engine.enable_gle
+        self._with_graphlearn_torch = launcher_config.engine.enable_glt
         self._with_mars = launcher_config.mars.enable
 
         def load_base64_json(string):
             if string is None:
                 return None
             json_str = base64.b64decode(string).decode("utf-8", errors="ignore")
             return json.loads(json_str)
@@ -104,33 +107,36 @@
         tag = launcher_config.image.tag
 
         image_prefix = f"{registry}/{repository}" if registry else repository
         self._analytical_image = f"{image_prefix}/analytical:{tag}"
         self._analytical_java_image = f"{image_prefix}/analytical-java:{tag}"
         self._interactive_frontend_image = f"{image_prefix}/interactive-frontend:{tag}"
         self._interactive_executor_image = f"{image_prefix}/interactive-executor:{tag}"
-        self._learning_image = f"{image_prefix}/learning:{tag}"
+        self._graphlearn_image = f"{image_prefix}/graphlearn:{tag}"
+        self._graphlearn_torch_image = f"{image_prefix}/graphlearn-torch:{tag}"
         self._dataset_image = f"{image_prefix}/dataset:{tag}"
 
         self._vineyard_deployment = config.vineyard.deployment_name
         self._vineyard_image = config.vineyard.image
         self._vineyard_service_port = config.vineyard.rpc_port
         self._sock = "/tmp/vineyard_workspace/vineyard.sock"
 
         self._dataset_requests = {"cpu": "200m", "memory": "64Mi"}
 
         self._engine_pod_prefix = engine_pod_prefix
         self._analytical_prefix = "gs-analytical-"
         self._interactive_frontend_prefix = "gs-interactive-frontend-"
-        self._learning_prefix = "gs-learning-"
+        self._graphlearn_prefix = "gs-graphlearn-"
+        self._graphlearn_torch_prefix = "gs-graphlearn-torch-"
         self._vineyard_prefix = "vineyard-"
         self._mars_scheduler_name_prefix = "mars-scheduler-"
         self._mars_service_name_prefix = "mars-"
 
-        self._learning_start_port = learning_start_port
+        self._graphlearn_start_port = graphlearn_start_port
+        self._graphlearn_torch_start_port = graphlearn_torch_start_port
 
         self._engine_labels = {
             "app.kubernetes.io/name": "graphscope",
             "app.kubernetes.io/instance": self._instance_id,
             "app.kubernetes.io/version": __version__,
             "app.kubernetes.io/component": "engine",
             "app.kubernetes.io/engine_selector": self.engine_stateful_set_name,
@@ -251,25 +257,44 @@
         ]
         resource = self._engine_resources.gie_executor_resource
         container = self.get_engine_container_helper(
             name, image, args, volume_mounts, resource
         )
         return container
 
-    def get_learning_container(self, volume_mounts):
-        name = LEARNING_CONTAINER_NAME
-        image = self._learning_image
+    def get_graphlearn_container(self, volume_mounts):
+        name = GRAPHLEARN_CONTAINER_NAME
+        image = self._graphlearn_image
         args = ["tail", "-f", "/dev/null"]
         resource = self._engine_resources.gle_resource
         container = self.get_engine_container_helper(
             name, image, args, volume_mounts, resource
         )
         container.ports = [
             kube_client.V1ContainerPort(container_port=p)
-            for p in range(self._learning_start_port, self._learning_start_port + 1000)
+            for p in range(
+                self._graphlearn_start_port, self._graphlearn_start_port + 1000
+            )
+        ]
+        return container
+
+    def get_graphlearn_torch_container(self, volume_mounts):
+        name = GRAPHLEARN_TORCH_CONTAINER_NAME
+        image = self._graphlearn_torch_image
+        args = ["tail", "-f", "/dev/null"]
+        resource = self._engine_resources.glt_resource
+        container = self.get_engine_container_helper(
+            name, image, args, volume_mounts, resource
+        )
+        container.ports = [
+            kube_client.V1ContainerPort(container_port=p)
+            for p in range(
+                self._graphlearn_torch_start_port,
+                self._graphlearn_torch_start_port + 1000,
+            )
         ]
         return container
 
     def get_mars_container(self):
         pass
 
     def get_dataset_container(self, volume_mounts):
@@ -334,17 +359,21 @@
             )
         if self._with_interactive:
             containers.append(
                 self.get_interactive_executor_container(
                     volume_mounts=engine_volume_mounts
                 )
             )
-        if self._with_learning:
+        if self._with_graphlearn:
             containers.append(
-                self.get_learning_container(volume_mounts=engine_volume_mounts)
+                self.get_graphlearn_container(volume_mounts=engine_volume_mounts)
+            )
+        if self._with_graphlearn_torch:
+            containers.append(
+                self.get_graphlearn_torch_container(volume_mounts=engine_volume_mounts)
             )
 
         if self._with_dataset:
             volume, src_volume_mount, dst_volume_mount = self.get_dataset_volume()
             volumes.append(volume)
             containers.append(
                 self.get_dataset_container(volume_mounts=[src_volume_mount])
@@ -393,34 +422,54 @@
         # Necessary, create a headless service for statefulsets
         service_spec.cluster_ip = "None"
         service = ResourceBuilder.get_service(
             self._namespace, name, service_spec, self._engine_labels
         )
         return service
 
-    def get_learning_service(self, object_id, start_port):
+    def get_graphlearn_service(self, object_id, start_port):
         service_type = self._service_type
         num_workers = self._num_workers
-        name = self.get_learning_service_name(object_id)
+        name = self.get_graphlearn_service_name(object_id)
         ports = []
         for i in range(start_port, start_port + num_workers):
             port = kube_client.V1ServicePort(name=f"{name}-{i}", port=i, protocol="TCP")
             ports.append(port)
         service_spec = ResourceBuilder.get_service_spec(
             service_type, ports, self._engine_labels, "Local"
         )
         service = ResourceBuilder.get_service(
             self._namespace, name, service_spec, self._engine_labels
         )
         return service
 
-    def get_learning_ports(self, start_port):
+    def get_graphlearn_torch_service(self, object_id, start_port):
+        service_type = self._service_type
+        num_workers = self._num_workers
+        name = self.get_graphlearn_torch_service_name(object_id)
+        ports = []
+        for i in range(start_port, start_port + num_workers):
+            port = kube_client.V1ServicePort(name=f"{name}-{i}", port=i, protocol="TCP")
+            ports.append(port)
+        service_spec = ResourceBuilder.get_service_spec(
+            service_type, ports, self._engine_labels, "Local"
+        )
+        service = ResourceBuilder.get_service(
+            self._namespace, name, service_spec, self._engine_labels
+        )
+        return service
+
+    def get_graphlearn_ports(self, start_port):
         num_workers = self._num_workers
         return [i for i in range(start_port, start_port + num_workers)]
 
+    def get_graphlearn_torch_ports(self, start_port):
+        num_loaders = 4
+        return [i for i in range(start_port, start_port + num_loaders)]
+
     @property
     def engine_stateful_set_name(self):
         return f"{self._engine_pod_prefix}{self._instance_id}"
 
     @property
     def frontend_deployment_name(self):
         return f"{self._interactive_frontend_prefix}{self._instance_id}"
@@ -440,19 +489,22 @@
             namespace=self._namespace,
             name=service_name,
             service_type=self._service_type,
         )
         assert len(endpoints) > 0
         return endpoints[0]
 
-    def get_learning_service_name(self, object_id):
-        return f"{self._learning_prefix}{object_id}"
+    def get_graphlearn_service_name(self, object_id):
+        return f"{self._graphlearn_prefix}{object_id}"
+
+    def get_graphlearn_torch_service_name(self, object_id):
+        return f"{self._graphlearn_torch_prefix}{object_id}"
 
     def get_graphlearn_service_endpoint(self, api_client, object_id, pod_host_ip_list):
-        service_name = self.get_learning_service_name(object_id)
+        service_name = self.get_graphlearn_service_name(object_id)
         service_type = self._service_type
         core_api = kube_client.CoreV1Api(api_client)
         if service_type == "NodePort":
             # TODO: add label_selector to filter the service
             services = core_api.list_namespaced_service(self._namespace)
             for svc in services.items:
                 if svc.metadata.name == service_name:
```

## gscoordinator/local_launcher.py

```diff
@@ -313,15 +313,15 @@
             base64.b64decode(handle.encode("utf-8", errors="ignore")).decode(
                 "utf-8", errors="ignore"
             )
         )
 
         server_client_master_port = get_free_port("localhost")
         handle["server_client_master_port"] = server_client_master_port
-
+        handle["master_addr"] = "localhost"
         server_list = [f"localhost:{server_client_master_port}"]
         # for train, val and test
         for _ in range(3):
             server_list.append("localhost:" + str(get_free_port("localhost")))
 
         handle = base64.b64encode(
             json.dumps(handle).encode("utf-8", errors="ignore")
@@ -343,31 +343,36 @@
                 sys.executable,
                 "-m",
                 "gscoordinator.launch_graphlearn_torch",
                 handle,
                 config,
                 str(index),
             ]
-            logger.debug("launching graphlearn_torch server: %s", " ".join(str(cmd)))
+            # logger.debug("launching graphlearn_torch server: %s", " ".join(cmd))
 
             proc = subprocess.Popen(
                 cmd,
                 env=env,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.STDOUT,
                 encoding="utf-8",
                 errors="replace",
                 universal_newlines=True,
                 bufsize=1,
             )
+            logger.debug("suppressed: %s", (not logger.isEnabledFor(logging.DEBUG)))
             stdout_watcher = PipeWatcher(
                 proc.stdout,
                 sys.stdout,
                 suppressed=(not logger.isEnabledFor(logging.DEBUG)),
             )
+
+            time.sleep(5)
+            logger.debug("process status: %s", proc.poll())
+
             setattr(proc, "stdout_watcher", stdout_watcher)
             self._learning_instance_processes[object_id].append(proc)
         return server_list
 
     def close_analytical_instance(self):
         self._stop_subprocess(self._analytical_engine_process, kill=True)
         self._analytical_engine_endpoint = None
@@ -383,15 +388,15 @@
         ]
         logger.info("Close GIE instance with command: %s", " ".join(cmd))
         process = self._popen_helper(cmd, cwd=os.getcwd(), env=env)
         # 60 seconds is enough
         process.wait(timeout=self._timeout_seconds)
         return process
 
-    def close_learning_instance(self, object_id):
+    def close_learning_instance(self, object_id, learning_backend=0):
         if object_id not in self._learning_instance_processes:
             return
 
         # terminate the process
         for proc in self._learning_instance_processes[object_id]:
             self._stop_subprocess(proc, kill=True)
         self._learning_instance_processes.clear()
```

## gscoordinator/launch_graphlearn_torch.py

```diff
@@ -15,79 +15,112 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import base64
 import json
 import logging
-import os.path as osp
 import sys
 
+import graphscope
 import graphscope.learning.graphlearn_torch as glt
 import torch
 from graphscope.learning.gl_torch_graph import GLTorchGraph
 
+graphscope.set_option(show_log=True)
+graphscope.set_option(log_level="DEBUG")
+
 logger = logging.getLogger("graphscope")
 
 
 def decode_arg(arg):
     if isinstance(arg, dict):
         return arg
     return json.loads(
         base64.b64decode(arg.encode("utf-8", errors="ignore")).decode(
             "utf-8", errors="ignore"
         )
     )
 
 
+def extract_node_type_names(edges):
+    node_type_names = set()
+    for edge in edges:
+        node_type_names.update([edge[0], edge[-1]])
+    return node_type_names
+
+
+def init_node_pb(handle, server_rank, node_type_names):
+    node_pb = (
+        glt.data.VineyardPartitionBook(
+            str(handle["vineyard_socket"]),
+            str(handle["fragments"][server_rank]),
+            list(node_type_names)[0],
+        )
+        if len(node_type_names) == 1
+        else {
+            node_type_name: glt.data.VineyardPartitionBook(
+                str(handle["vineyard_socket"]),
+                str(handle["fragments"][server_rank]),
+                node_type_name,
+            )
+            for node_type_name in node_type_names
+        }
+    )
+    return node_pb
+
+
 def run_server_proc(proc_rank, handle, config, server_rank, dataset):
     glt.distributed.init_server(
         num_servers=handle["num_servers"],
         server_rank=server_rank,
         dataset=dataset,
         master_addr=handle["master_addr"],
         master_port=handle["server_client_master_port"],
         num_rpc_threads=16,
         is_dynamic=True,
     )
-    logger.info(f"-- [Server {server_rank}] Waiting for exit ...")
     glt.distributed.wait_and_shutdown_server()
-    logger.info(f"-- [Server {server_rank}] Exited ...")
 
 
 def launch_graphlearn_torch_server(handle, config, server_rank):
     logger.info(f"-- [Server {server_rank}] Initializing server ...")
-
     edge_dir = config.pop("edge_dir")
     random_node_split = config.pop("random_node_split")
-    dataset = glt.distributed.DistDataset(edge_dir=edge_dir)
+    edges = config.pop("edges")
+    node_type_names = extract_node_type_names(edges)
+
+    dataset = glt.distributed.DistDataset(
+        edge_dir=edge_dir,
+        num_partitions=handle["num_servers"],
+        partition_idx=server_rank,
+        node_pb=init_node_pb(handle, server_rank, node_type_names),
+    )
     dataset.load_vineyard(
-        vineyard_id=str(handle["vineyard_id"]),
+        vineyard_id=str(handle["fragments"][server_rank]),
         vineyard_socket=handle["vineyard_socket"],
+        edges=edges,
         **config,
     )
     if random_node_split is not None:
         dataset.random_node_split(**random_node_split)
-    logger.info(f"-- [Server {server_rank}] Initializing server ...")
+    logger.info(f"-- [Server {server_rank}] Running server ...")
 
     torch.multiprocessing.spawn(
         fn=run_server_proc, args=(handle, config, server_rank, dataset), nprocs=1
     )
+    logger.info(f"-- [Server {server_rank}] Server exited.")
 
 
 if __name__ == "__main__":
     if len(sys.argv) < 3:
         logger.info(
             "Usage: ./launch_graphlearn_torch.py <handle> <config> <server_index>",
-            file=sys.stderr,
         )
         sys.exit(-1)
 
     handle = decode_arg(sys.argv[1])
     config = decode_arg(sys.argv[2])
     server_index = int(sys.argv[3])
     config = GLTorchGraph.reverse_transform_config(config)
 
-    logger.info(
-        f"launch_graphlearn_torch_server handle: {handle} config: {config} server_index: {server_index}"
-    )
     launch_graphlearn_torch_server(handle, config, server_index)
```

## gscoordinator/VERSION

```diff
@@ -1 +1 @@
-0.27.0a20240401
+0.27.0a20240402
```

## gscoordinator/utils.py

```diff
@@ -2109,7 +2109,19 @@
             return True
         time.sleep(3)
         if time.time() - begin_time > INTERACTIVE_INSTANCE_TIMEOUT_SECONDS:
             executor.shutdown(wait=False)
             raise TimeoutError(
                 f"{server.capitalize()} check query failed: {error_message}"
             )
+
+
+def replace_string_in_dict(dict_obj, old, new):
+    if isinstance(dict_obj, dict):
+        for key, value in dict_obj.items():
+            dict_obj[key] = replace_string_in_dict(value, old, new)
+    elif isinstance(dict_obj, list):
+        for index, item in enumerate(dict_obj):
+            dict_obj[index] = replace_string_in_dict(item, old, new)
+    elif isinstance(dict_obj, str):
+        return dict_obj.replace(old, new)
+    return dict_obj
```

## gscoordinator/launcher.py

```diff
@@ -105,15 +105,15 @@
         pass
 
     @abstractmethod
     def close_interactive_instance(self, object_id: int):
         pass
 
     @abstractmethod
-    def close_learning_instance(self, object_id: int):
+    def close_learning_instance(self, object_id: int, learning_backend: int):
         pass
 
     @abstractmethod
     def launch_etcd(self):
         pass
 
     @abstractmethod
```

## gscoordinator/servicer/graphscope_one/service.py

```diff
@@ -453,31 +453,32 @@
             gremlin_endpoint=gremlin_endpoint,
             cypher_endpoint=cypher_endpoint,
             object_id=object_id,
         )
 
     def CreateLearningInstance(self, request, context):
         object_id = request.object_id
-        logger.info("Create learning instance with object id %ld", object_id)
         handle, config, learning_backend = (
             request.handle,
             request.config,
             request.learning_backend,
         )
         try:
             endpoints = self._launcher.create_learning_instance(
                 object_id, handle, config, learning_backend
             )
-            self._object_manager.put(object_id, LearningInstanceManager(object_id))
+            self._object_manager.put(
+                object_id, LearningInstanceManager(object_id, learning_backend)
+            )
         except Exception as e:
             context.set_code(grpc.StatusCode.ABORTED)
             context.set_details(
                 f"Create learning instance failed: ${e}. The traceback is: {traceback.format_exc()}"
             )
-            self._launcher.close_learning_instance(object_id)
+            self._launcher.close_learning_instance(object_id, learning_backend)
             self._object_manager.pop(object_id)
             return message_pb2.CreateLearningInstanceResponse()
         return message_pb2.CreateLearningInstanceResponse(
             object_id=object_id, handle=handle, config=config, endpoints=endpoints
         )
 
     def CloseAnalyticalInstance(self, request, context):
@@ -500,15 +501,17 @@
 
     def CloseLearningInstance(self, request, context):
         object_id = request.object_id
         if object_id in self._object_manager:
             self._object_manager.pop(object_id)
             logger.info("Close learning instance with object id %ld", object_id)
             try:
-                self._launcher.close_learning_instance(object_id)
+                self._launcher.close_learning_instance(
+                    object_id, request.learning_backend
+                )
             except Exception as e:
                 context.set_code(grpc.StatusCode.ABORTED)
                 context.set_details(
                     f"Close learning instance failed: ${e}. The traceback is: {traceback.format_exc()}"
                 )
         return message_pb2.CloseLearningInstanceResponse()
 
@@ -530,15 +533,17 @@
                 config[types_pb2.GRAPH_NAME] = s_to_attr(obj.key)
                 # dynamic graph doesn't have a object id
                 if obj.object_id != -1:
                     config[types_pb2.VINEYARD_ID] = i_to_attr(obj.object_id)
             elif obj.type == "gie_manager":
                 self._launcher.close_interactive_instance(obj.object_id)
             elif obj.type == "gle_manager":
-                self._launcher.close_learning_instance(obj.object_id)
+                self._launcher.close_learning_instance(obj.object_id, 0)
+            elif obj.type == "glt_manager":
+                self._launcher.close_learning_instance(obj.object_id, 1)
 
             if op_type is not None:
                 dag_def = create_single_op_dag(op_type, config)
                 try:
                     self._operation_executor.run_step(dag_def, [])
                 except grpc.RpcError as e:
                     logger.error(
```

## gscoordinator/builtin/app/builtin_app.gar

### zipinfo {}

```diff
@@ -1,5 +1,5 @@
-Zip file size: 5715 bytes, number of entries: 3
--rw-r--r--  2.0 unx    25282 b- defN 24-Apr-01 20:24 .gs_conf.yaml
--rw-r--r--  2.0 unx      646 b- defN 24-Apr-01 20:24 __init__.py
--rw-r--r--  2.0 unx     2733 b- defN 24-Apr-01 21:25 builtin_app.zip
-3 files, 28661 bytes uncompressed, 5387 bytes compressed:  81.2%
+Zip file size: 5264 bytes, number of entries: 3
+-rw-r--r--  2.0 unx    25282 b- defN 24-Apr-03 03:01 .gs_conf.yaml
+-rw-r--r--  2.0 unx     2282 b- defN 24-Apr-03 04:04 builtin_app.zip
+-rw-r--r--  2.0 unx      646 b- defN 24-Apr-03 03:01 __init__.py
+3 files, 28210 bytes uncompressed, 4936 bytes compressed:  82.5%
```

### zipnote «TEMP»/diffoscope_ykk43ihd_/tmpy898v_i1_.zip

```diff
@@ -1,10 +1,10 @@
 Filename: .gs_conf.yaml
 Comment: 
 
-Filename: __init__.py
+Filename: builtin_app.zip
 Comment: 
 
-Filename: builtin_app.zip
+Filename: __init__.py
 Comment: 
 
 Zip file comment:
```

### builtin_app.zip

 * *Command `'zipinfo {}'` failed with exit code 9. Standard output:*

 * *    Archive:  /tmp/diffoscope_ykk43ihd_/tmp0p7q1mxx_ZipContainer/builtin_app.zip*

 * *    […]*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

```diff
@@ -1,8 +1,8 @@
-00000000: 504b 0304 1400 0000 0800 08a3 8158 f458  PK...........X.X
+00000000: 504b 0304 1400 0000 0800 3818 8358 f458  PK........8..X.X
 00000010: 240e bf08 0000 c262 0000 0d00 0000 2e67  $......b.......g
 00000020: 735f 636f 6e66 2e79 616d 6ccd 9c5b 739b  s_conf.yaml..[s.
 00000030: 3814 80df f757 e40f b0cc a46f 7973 48b3  8....W.....oysH.
 00000040: cd34 693d 71ba bbb3 2f8c 0c8a ad8d 0c2c  .4i=q.../......,
 00000050: 126e dd5f bf47 0299 8b01 1fd9 a9c5 431c  .n._.G........C.
 00000060: 8fd1 b97c 3aba 1c09 01c9 b29b dfae aebc  ...|:...........
 00000070: 2bc2 57e9 cd55 4656 3427 c91b fc74 7525  +.W..UFV4'...tu%
@@ -136,36 +136,8 @@
 00000870: 2125 402b ac1e 5f08 826f c71e 6068 a369  !%@+.._..o..`h.i
 00000880: f56e b6d0 6df6 d0b1 63fb d2cd e00e 662d  .n..m...c.....f-
 00000890: eeea 00ce e813 4f6d 1e37 3774 8445 7816  ......Om.77t.Ex.
 000008a0: e8f0 0837 e111 56e1 59e0 c323 5c85 6799  ...7..V.Y..#\.g.
 000008b0: 3350 826f 71ba 38b6 cde9 c2ee a86c 7a92  3P.oq.8......lz.
 000008c0: 1640 7726 5dda 4dc0 403c cc52 9658 6414  .@w&].M.@<.R.Xd.
 000008d0: 859c 2b01 ec58 5e48 4f1b 704a 67f3 e067  ..+..X^HO.pJg..g
-000008e0: c587 8dde 1ef0 2201 fc1f 504b 0304 1400  ......"...PK....
-000008f0: 0000 0800 08a3 8158 7cbd 2df0 9a01 0000  .......X|.-.....
-00000900: 8602 0000 0b00 0000 5f5f 696e 6974 5f5f  ........__init__
-00000910: 2e70 7965 9241 6fdb 300c 85ef fd15 6fc9  .pye.Ao.0.....o.
-00000920: 651b 9238 c82e 4377 f2d2 6c35 1638 409c  e..8..Cw..l5.8@.
-00000930: aee8 51b6 699b 8023 6992 5c37 ff7e 949b  ..Q.i..#i.\7.~..
-00000940: 012d a68b 20f1 f1e9 23a9 f907 2483 7749  .-.. ...#...$.wI
-00000950: c93a 21fd 0c7b 099d d15f 6ee6 587e 5ea2  .:!..{..._n.X~^.
-00000960: 3235 ebf6 1643 6896 5fe3 cdcd 5c22 5b63  25...Ch._...\"[c
-00000970: 2f8e db2e 60b3 deac 91f6 5caa 52e1 a733  /...`.....\.R..3
-00000980: 83c5 bde9 630e f67c e640 f56a cad8 7345  ....c..|.@.j..sE
-00000990: da53 8d41 d7e4 103a 426a 5525 db35 b2c0  .S.A...:BjU%.5..
-000009a0: 6f72 9e8d c666 b5c6 c728 985d 43b3 4fdf  or...f...(.]C.O.
-000009b0: c4e1 6206 9cd5 05da 040c 9ec4 823d 1aee  ..b..........=..
-000009c0: 09f4 5291 0d60 2db4 67db b3d2 1561 e4d0  ..R..`-.g....a..
-000009d0: 4dcf 5c4d 0403 4f57 0b53 0625 6a25 7a2b  M.\M..OW.S.%j%z+
-000009e0: a7e6 ad0e 2a4c c071 7521 d8db 2419 c771  ....*L.qu!..$..q
-000009f0: a526 d895 716d d2bf 0a7d b2cf b6bb bcd8  .&..qm...}......
-00000a00: 2d05 784a 79d0 3d79 0f47 7f06 7652 6a79  -.xJy.=y.G..vRjy
-00000a10: 81b2 c253 a952 287b 35c2 38a8 d691 c482  ...S.R({5.8.....
-00000a20: 89bc a3e3 20ad 5ac0 9b26 8cca 91b8 d4ec  .... .Z..&......
-00000a30: 83e3 7208 ef9a f58f 4e6a 7e2b 9076 298d  ..r.....Nj~+.v).
-00000a40: 595a 202b 66f8 9e16 59b1 108f c7ec 747f  YZ +f...Y.....t.
-00000a50: 7838 e131 3d1e d3fc 94ed 0a1c 8ed8 1ef2  x8.1=...........
-00000a60: bbec 941d 7239 fd40 9a3f e157 96df 2d40  ....r9.@.?.W..-@
-00000a70: d22a 7986 5eac 8bfc 02c9 b18d d3e8 5010  .*y.^.........P.
-00000a80: bd03 68cc 2b90 b754 71c3 95d4 a5db 41b5  ..h.+..Tq.....A.
-00000a90: 84d6 3c93 d371 f296 dc99 7d1c a617 bc5a  ..<..q....}....Z
-00000aa0: 5cfa f817 5498 6efe 2b2a fe90 bf         \...T.n.+*...
+000008e0: c587 8dde 1ef0 2201 fc1f                 ......"...
```

#### builtin_app.zip

```diff
@@ -1,8 +1,8 @@
-00000000: 504b 0304 1400 0000 0800 08a3 8158 f458  PK...........X.X
+00000000: 504b 0304 1400 0000 0800 3818 8358 f458  PK........8..X.X
 00000010: 240e bf08 0000 c262 0000 0d00 0000 2e67  $......b.......g
 00000020: 735f 636f 6e66 2e79 616d 6ccd 9c5b 739b  s_conf.yaml..[s.
 00000030: 3814 80df f757 e40f b0cc a46f 7973 48b3  8....W.....oysH.
 00000040: cd34 693d 71ba bbb3 2f8c 0c8a ad8d 0c2c  .4i=q.../......,
 00000050: 126e dd5f bf47 0299 8b01 1fd9 a9c5 431c  .n._.G........C.
 00000060: 8fd1 b97c 3aba 1c09 01c9 b29b dfae aebc  ...|:...........
 00000070: 2bc2 57e9 cd55 4656 3427 c91b fc74 7525  +.W..UFV4'...tu%
@@ -136,36 +136,8 @@
 00000870: 2125 402b ac1e 5f08 826f c71e 6068 a369  !%@+.._..o..`h.i
 00000880: f56e b6d0 6df6 d0b1 63fb d2cd e00e 662d  .n..m...c.....f-
 00000890: eeea 00ce e813 4f6d 1e37 3774 8445 7816  ......Om.77t.Ex.
 000008a0: e8f0 0837 e111 56e1 59e0 c323 5c85 6799  ...7..V.Y..#\.g.
 000008b0: 3350 826f 71ba 38b6 cde9 c2ee a86c 7a92  3P.oq.8......lz.
 000008c0: 1640 7726 5dda 4dc0 403c cc52 9658 6414  .@w&].M.@<.R.Xd.
 000008d0: 859c 2b01 ec58 5e48 4f1b 704a 67f3 e067  ..+..X^HO.pJg..g
-000008e0: c587 8dde 1ef0 2201 fc1f 504b 0304 1400  ......"...PK....
-000008f0: 0000 0800 08a3 8158 7cbd 2df0 9a01 0000  .......X|.-.....
-00000900: 8602 0000 0b00 0000 5f5f 696e 6974 5f5f  ........__init__
-00000910: 2e70 7965 9241 6fdb 300c 85ef fd15 6fc9  .pye.Ao.0.....o.
-00000920: 651b 9238 c82e 4377 f2d2 6c35 1638 409c  e..8..Cw..l5.8@.
-00000930: aee8 51b6 699b 8023 6992 5c37 ff7e 949b  ..Q.i..#i.\7.~..
-00000940: 012d a68b 20f1 f1e9 23a9 f907 2483 7749  .-.. ...#...$.wI
-00000950: c93a 21fd 0c7b 099d d15f 6ee6 587e 5ea2  .:!..{..._n.X~^.
-00000960: 3235 ebf6 1643 6896 5fe3 cdcd 5c22 5b63  25...Ch._...\"[c
-00000970: 2f8e db2e 60b3 deac 91f6 5caa 52e1 a733  /...`.....\.R..3
-00000980: 83c5 bde9 630e f67c e640 f56a cad8 7345  ....c..|.@.j..sE
-00000990: da53 8d41 d7e4 103a 426a 5525 db35 b2c0  .S.A...:BjU%.5..
-000009a0: 6f72 9e8d c666 b5c6 c728 985d 43b3 4fdf  or...f...(.]C.O.
-000009b0: c4e1 6206 9cd5 05da 040c 9ec4 823d 1aee  ..b..........=..
-000009c0: 09f4 5291 0d60 2db4 67db b3d2 1561 e4d0  ..R..`-.g....a..
-000009d0: 4dcf 5c4d 0403 4f57 0b53 0625 6a25 7a2b  M.\M..OW.S.%j%z+
-000009e0: a7e6 ad0e 2a4c c071 7521 d8db 2419 c771  ....*L.qu!..$..q
-000009f0: a526 d895 716d d2bf 0a7d b2cf b6bb bcd8  .&..qm...}......
-00000a00: 2d05 784a 79d0 3d79 0f47 7f06 7652 6a79  -.xJy.=y.G..vRjy
-00000a10: 81b2 c253 a952 287b 35c2 38a8 d691 c482  ...S.R({5.8.....
-00000a20: 89bc a3e3 20ad 5ac0 9b26 8cca 91b8 d4ec  .... .Z..&......
-00000a30: 83e3 7208 ef9a f58f 4e6a 7e2b 9076 298d  ..r.....Nj~+.v).
-00000a40: 595a 202b 66f8 9e16 59b1 108f c7ec 747f  YZ +f...Y.....t.
-00000a50: 7838 e131 3d1e d3fc 94ed 0a1c 8ed8 1ef2  x8.1=...........
-00000a60: bbec 941d 7239 fd40 9a3f e157 96df 2d40  ....r9.@.?.W..-@
-00000a70: d22a 7986 5eac 8bfc 02c9 b18d d3e8 5010  .*y.^.........P.
-00000a80: bd03 68cc 2b90 b754 71c3 95d4 a5db 41b5  ..h.+..Tq.....A.
-00000a90: 84d6 3c93 d371 f296 dc99 7d1c a617 bc5a  ..<..q....}....Z
-00000aa0: 5cfa f817 5498 6efe 2b2a fe90 bf         \...T.n.+*...
+000008e0: c587 8dde 1ef0 2201 fc1f                 ......"...
```

## Comparing `gs_coordinator-0.27.0a20240401.dist-info/RECORD` & `gs_coordinator-0.27.0a20240402.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-gs_coordinator-0.27.0a20240401.dist-info/RECORD,,
-gs_coordinator-0.27.0a20240401.dist-info/WHEEL,sha256=EACXjPwsYzxTpWW_PsZniqQc4RzZfXb_Ir_SpN_ifuM,140
-gs_coordinator-0.27.0a20240401.dist-info/top_level.txt,sha256=GiJfpWt7WpC-H1BxUy5V39G7WAtPut6eqH3yAciJhqQ,33
-gs_coordinator-0.27.0a20240401.dist-info/METADATA,sha256=gztRSyjwVc3e3aHGZGiDDaoA7_7W3TOhf7RpAs-Unpk,23840
-gscoordinator/kubernetes_launcher.py,sha256=8cvqbR2M_l5ppj25B9OvaBw4dyaK-Ez7XSN7Sd-ZBMI,54960
-gscoordinator/coordinator.py,sha256=JxvRRQVngJD5jT014qgMdrlIS4XBBLSG5NjXcCJvQ2E,5450
-gscoordinator/dag_manager.py,sha256=qA88ACSe97ANR02viegLksZ3vkVJdASK_hsNVZj9ieg,5702
-gscoordinator/version.py,sha256=bS71qRjwM-xk4LAFTExdiWJOaJEXaeNdlJYCAqtD98U,1045
-gscoordinator/monitor.py,sha256=8nfT_UfQ8UeYGqpNDxoK0Dw9vWTbVSI-W6pFZy4Lq0A,6950
-gscoordinator/op_executor.py,sha256=x59Mrg9wOfyFT7nRuizc21DESo_KTOllnQpGEninxrk,43296
-gscoordinator/object_manager.py,sha256=e-5KcWigw8VM9o1WSMZ9BIQHIATvWD4gCXfiZVjPR6U,2653
-gscoordinator/operator_launcher.py,sha256=e9LuVPw3gfUFHxjO0vYuthpAMgCI0TYWOWbTE8yxD6s,4351
-gscoordinator/constants.py,sha256=FxXDGCJ6vQ9LyKBGUW45jvdlRPRgtQkwxTuqh1S3tBQ,343
-gscoordinator/__init__.py,sha256=nUqENyB6dtqMgYfbJjblAdV2nemmlsaTMp_yTteBnOw,990
-gscoordinator/cluster_builder.py,sha256=RE29hMZIGiyQpA0xagzs9hggQ6en61uMdR7KbnCDoqI,21916
-gscoordinator/local_launcher.py,sha256=8zx3bxaB9pQUv4X07-hq-IpoSllOUxNCMJNvvDWuSOo,22198
-gscoordinator/launch_graphlearn_torch.py,sha256=euyryABQwNKAm0OpguRpn6EZNA20j6f0xVFa-KukRwE,2975
-gscoordinator/VERSION,sha256=5H8IfbvFQA3D2DxKwtgeI7teV2KusNJ7E4pjycDcyQE,16
-gscoordinator/utils.py,sha256=orWfdjfQ3NL5ex6XB1VvfBhxyOqlRFR6OSMOE3jgmcE,80235
-gscoordinator/io_utils.py,sha256=8lxUPh-DfBj4yPIAPY9ovv2Iweg7MG8V77LscRlPM8o,4091
-gscoordinator/launcher.py,sha256=Nn6zrfo1ycuB-Msj5_Slx9MDQO8C2Zqd6_-MpJXiQA0,5372
-gscoordinator/launch_graphlearn.py,sha256=91UC3ECqfVLbF4nsxYxORWLiHGRTjbVMjwiRNM9ZjLI,2494
-gscoordinator/__main__.py,sha256=pfC-UJ0gz8i-p1lGAs2jBB8zALAz6PaBokLa9v6AYQ4,77
-gscoordinator/template/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
-gscoordinator/template/pregel.pxd.template,sha256=Eh4tESR8KlmM30Mcw-eIUfiQNeadDj3WWGCUzkIsT2M,4340
-gscoordinator/template/pie.pxd.template,sha256=-hYphyhUzTnyQELecGEsCK_S-fEXLWGiTV91-gDqAU8,4957
-gscoordinator/template/CMakeLists.template,sha256=EqTx-5CWuZ6bf6lUhGZ8Hwu6s3AANu-cScKpjxm4ndw,22656
-gscoordinator/servicer/__init__.py,sha256=i0VzRn8z0PsDlQj3oZzOsii2qVSk-vcZQzFtbse9fVo,707
-gscoordinator/servicer/graphscope_one/service.py,sha256=IS1zquyYhLBn4dSGyYCNJz1GKuz5EHO4ityrvG5JHD4,24792
-gscoordinator/servicer/graphscope_one/__init__.py,sha256=hSEiV3pYv8wKgo6KzUx0p4563wJ1on2osrFZxZ4pT2o,646
-gscoordinator/builtin/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
-gscoordinator/builtin/app/.gs_conf.yaml,sha256=gWoCXtVzGb1xks9ioQ5WfYMnFPRJGiq9Cb-w3oF8SVA,25282
-gscoordinator/builtin/app/builtin_app.gar,sha256=kRsAjE21drRK7JIm5vB_Dku5damE9v5c7Huyb0kKV1E,5715
-gscoordinator/builtin/app/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
-gscoordinator/hook/__init__.py,sha256=jzzLJxC1gBgRLMb4xzX6vucYuNdosuWOtZKRj7Cal_o,646
-gscoordinator/hook/prestop/__init__.py,sha256=jzzLJxC1gBgRLMb4xzX6vucYuNdosuWOtZKRj7Cal_o,646
-gscoordinator/hook/prestop/__main__.py,sha256=1FmS0g2hwl85NPMOtbAvW_IGn4GFnldmjbSSwaj9GrE,1560
+graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
+gscoordinator/VERSION,sha256=RGzr4DXZBaDiqo8StEeXDMkIj5VgGbqK7YRgqx259yo,16
+gscoordinator/__init__.py,sha256=nUqENyB6dtqMgYfbJjblAdV2nemmlsaTMp_yTteBnOw,990
+gscoordinator/__main__.py,sha256=pfC-UJ0gz8i-p1lGAs2jBB8zALAz6PaBokLa9v6AYQ4,77
+gscoordinator/cluster_builder.py,sha256=gBn3gpLflgjIMvcfKYojFD9O9b3oh4d8Ox8sIApeyOo,24165
+gscoordinator/constants.py,sha256=wHKzhJg-LM2qU6P-AuBjAd5t8kII6RCLKXxgDfrXLoE,400
+gscoordinator/coordinator.py,sha256=JxvRRQVngJD5jT014qgMdrlIS4XBBLSG5NjXcCJvQ2E,5450
+gscoordinator/dag_manager.py,sha256=qA88ACSe97ANR02viegLksZ3vkVJdASK_hsNVZj9ieg,5702
+gscoordinator/io_utils.py,sha256=8lxUPh-DfBj4yPIAPY9ovv2Iweg7MG8V77LscRlPM8o,4091
+gscoordinator/kubernetes_launcher.py,sha256=qdP8-zqA3AlJNDexAB9B4-TMzzu9H5TTzOtNIV9M6MQ,66027
+gscoordinator/launch_graphlearn.py,sha256=91UC3ECqfVLbF4nsxYxORWLiHGRTjbVMjwiRNM9ZjLI,2494
+gscoordinator/launch_graphlearn_torch.py,sha256=M6yP-FLLzZxCxinenS1AgutZqP7i9LKBJae4DATr1uQ,3877
+gscoordinator/launcher.py,sha256=3_B2bX7A-NikKr_7snXbku6p4mibOj157YCdhihhTRI,5395
+gscoordinator/local_launcher.py,sha256=kBvZ2i3lTHgrkpXCiex9-GNoysTShcjA6FpBlemW3-s,22431
+gscoordinator/monitor.py,sha256=8nfT_UfQ8UeYGqpNDxoK0Dw9vWTbVSI-W6pFZy4Lq0A,6950
+gscoordinator/object_manager.py,sha256=dsMQYqsjSjjD63QZ3qnR6rVpnKyW0d4TZgdneHMIBcw,2761
+gscoordinator/op_executor.py,sha256=x59Mrg9wOfyFT7nRuizc21DESo_KTOllnQpGEninxrk,43296
+gscoordinator/operator_launcher.py,sha256=mCwTFN-nHsPU-lK14VfdrEwEkLq1eyQuqyZUWOSbNMY,4369
+gscoordinator/utils.py,sha256=zVk2usMHqsNObzOGcYxqVW8Qg7X89T-gwk5R-yilOIc,80684
+gscoordinator/version.py,sha256=bS71qRjwM-xk4LAFTExdiWJOaJEXaeNdlJYCAqtD98U,1045
+gscoordinator/builtin/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
+gscoordinator/builtin/app/.gs_conf.yaml,sha256=gWoCXtVzGb1xks9ioQ5WfYMnFPRJGiq9Cb-w3oF8SVA,25282
+gscoordinator/builtin/app/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
+gscoordinator/builtin/app/builtin_app.gar,sha256=YYuRQB72TQcEWhpUroZP7QZmnq3wbDYTJJr-EN2--U4,5264
+gscoordinator/hook/__init__.py,sha256=jzzLJxC1gBgRLMb4xzX6vucYuNdosuWOtZKRj7Cal_o,646
+gscoordinator/hook/prestop/__init__.py,sha256=jzzLJxC1gBgRLMb4xzX6vucYuNdosuWOtZKRj7Cal_o,646
+gscoordinator/hook/prestop/__main__.py,sha256=1FmS0g2hwl85NPMOtbAvW_IGn4GFnldmjbSSwaj9GrE,1560
+gscoordinator/servicer/__init__.py,sha256=i0VzRn8z0PsDlQj3oZzOsii2qVSk-vcZQzFtbse9fVo,707
+gscoordinator/servicer/graphscope_one/__init__.py,sha256=hSEiV3pYv8wKgo6KzUx0p4563wJ1on2osrFZxZ4pT2o,646
+gscoordinator/servicer/graphscope_one/service.py,sha256=0jOELYYbA7_8rRYM9mHXAeA6r4LY7o2Iyvk11GFqkIQ,24964
+gscoordinator/template/CMakeLists.template,sha256=EqTx-5CWuZ6bf6lUhGZ8Hwu6s3AANu-cScKpjxm4ndw,22656
+gscoordinator/template/__init__.py,sha256=TsAsMQRDcEJ9nRXDAeF-pJPapJrZPwVeb-TxxVp42aY,646
+gscoordinator/template/pie.pxd.template,sha256=-hYphyhUzTnyQELecGEsCK_S-fEXLWGiTV91-gDqAU8,4957
+gscoordinator/template/pregel.pxd.template,sha256=Eh4tESR8KlmM30Mcw-eIUfiQNeadDj3WWGCUzkIsT2M,4340
+gs_coordinator-0.27.0a20240402.dist-info/METADATA,sha256=gZelUp_0NJcg7jvXS0J0eJpAcGvu0CLQnjblBsZ64xE,23840
+gs_coordinator-0.27.0a20240402.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+gs_coordinator-0.27.0a20240402.dist-info/top_level.txt,sha256=GiJfpWt7WpC-H1BxUy5V39G7WAtPut6eqH3yAciJhqQ,33
+gs_coordinator-0.27.0a20240402.dist-info/RECORD,,
```

## Comparing `gs_coordinator-0.27.0a20240401.dist-info/METADATA` & `gs_coordinator-0.27.0a20240402.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-coordinator
-Version: 0.27.0a20240401
+Version: 0.27.0a20240402
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 Requires-Dist: grpcio-tools >=1.49
 Requires-Dist: kubernetes >=24.2.0
 Requires-Dist: protobuf >=4
 Requires-Dist: PyYAML
 Requires-Dist: prometheus-client >=0.14.1
 Requires-Dist: packaging
 Requires-Dist: tqdm
-Requires-Dist: graphscope-client ==0.27.0a20240401
+Requires-Dist: graphscope-client ==0.27.0a20240402
 Requires-Dist: vineyard >=0.16.3 ; sys_platform != "win32"
 Requires-Dist: vineyard-io >=0.16.3 ; sys_platform != "win32"
 Provides-Extra: dev
 Requires-Dist: black >=23.3.0 ; extra == 'dev'
 Requires-Dist: flake8 ==4.0.1 ; extra == 'dev'
 Requires-Dist: isort ==5.10.1 ; extra == 'dev'
 Requires-Dist: setuptools ==65.7.0 ; extra == 'dev'
```

