# Comparing `tmp/optscale_arcee-0.1.37.tar.gz` & `tmp/optscale_arcee-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optscale_arcee-0.1.37.tar", last modified: Tue Dec 26 17:30:42 2023, max compression
+gzip compressed data, was "optscale_arcee-0.1.38.tar", last modified: Tue Apr  2 10:01:11 2024, max compression
```

## Comparing `optscale_arcee-0.1.37.tar` & `optscale_arcee-0.1.38.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:42.765102 optscale_arcee-0.1.37/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-12-26 17:30:42.765102 optscale_arcee-0.1.37/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:42.761103 optscale_arcee-0.1.37/optscale_arcee/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/arcee.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:42.765102 optscale_arcee-0.1.37/optscale_arcee/collectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/collectors/command_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/collectors/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/collectors/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/collectors/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/collectors/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:42.765102 optscale_arcee-0.1.37/optscale_arcee/platforms_meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/platforms_meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2023-12-26 17:30:36.000000 optscale_arcee-0.1.37/optscale_arcee/platforms_meta/azure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:42.765102 optscale_arcee-0.1.37/optscale_arcee/sender/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:37.000000 optscale_arcee-0.1.37/optscale_arcee/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2023-12-26 17:30:37.000000 optscale_arcee-0.1.37/optscale_arcee/sender/sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2023-12-26 17:30:37.000000 optscale_arcee-0.1.37/optscale_arcee/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:42.765102 optscale_arcee-0.1.37/optscale_arcee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2023-12-26 17:30:42.000000 optscale_arcee-0.1.37/optscale_arcee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-26 17:30:42.000000 optscale_arcee-0.1.37/optscale_arcee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 17:30:42.000000 optscale_arcee-0.1.37/optscale_arcee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-26 17:30:42.000000 optscale_arcee-0.1.37/optscale_arcee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-26 17:30:42.000000 optscale_arcee-0.1.37/optscale_arcee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-26 17:30:42.765102 optscale_arcee-0.1.37/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-26 17:30:37.000000 optscale_arcee-0.1.37/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 17:30:42.765102 optscale_arcee-0.1.37/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2023-12-26 17:30:37.000000 optscale_arcee-0.1.37/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2023-12-26 17:30:37.000000 optscale_arcee-0.1.37/tests/test_platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.198480 optscale_arcee-0.1.38/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-02 10:01:11.198480 optscale_arcee-0.1.38/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/arcee.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee/collectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/collectors/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee/platforms_meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/platforms_meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/platforms_meta/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee/sender/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/sender/sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/optscale_arcee/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/optscale_arcee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 10:01:11.000000 optscale_arcee-0.1.38/optscale_arcee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 10:01:11.198480 optscale_arcee-0.1.38/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:01:11.194480 optscale_arcee-0.1.38/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-02 10:01:08.000000 optscale_arcee-0.1.38/tests/test_platform.py
```

### Comparing `optscale_arcee-0.1.37/LICENSE` & `optscale_arcee-0.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/PKG-INFO` & `optscale_arcee-0.1.38/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optscale_arcee
-Version: 0.1.37
+Version: 0.1.38
 Summary: ML profiling tool for OptScale
 Home-page: https://my.optscale.com/
 Author: Hystax
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/hystax/optscale_arcee
 Keywords: arcee,ml,optscale,finops,mlops
 Requires-Python: <4,>=3.7
@@ -31,34 +31,34 @@
 First of all you need to import and init arcee in your code:
 ```sh
 import optscale_arcee as arcee
 ```
 
 ```sh
 # init arcee using context manager syntax
-with arcee.init('token', 'model_key'):
+with arcee.init('token', 'task_key'):
     # some code
 ```
 
 To use custom endpoint and enable\disable ssl checks (supports using self-signed ssl certificates):
 ```sh
-with arcee.init('token', 'model_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
+with arcee.init('token', 'task_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
     # some code
 ```
 
 Alternatively arcee can be initialized via function call. However manual finish is required:
 ```sh
-arcee.init('token', 'model_key')
+arcee.init('token', 'task_key')
 # some code
 arcee.finish()
 ```
 
 Or in error case:
 ```sh
-arcee.init('token', 'model_key')
+arcee.init('token', 'task_key')
 # some code
 arcee.error()
 ```
 
 To send stats:
 ```sh
 arcee.send({"loss": 2.0012, "iter": 2, "epoch": 1})
@@ -87,7 +87,21 @@
 
 ## Logging datasets
 To log a dataset, use the dataset method with the following parameter:
 - path (str): the path of the dataset.
 ```
 arcee.dataset("dataset_path")
 ```
+
+## Models
+To create a model, use the model method with the following parameters:
+- key (str): the unique key of the model
+- path (str): the path of the run artifacts
+```
+arcee.model("my_model", "/home/user/my_model")
+```
+
+To set custom model version, use the set_model_version method with the following parameter:
+- version (str): version name
+```
+arcee.set_model_version("1.2.3-release")
+```
```

### Comparing `optscale_arcee-0.1.37/optscale_arcee/arcee.py` & `optscale_arcee-0.1.38/optscale_arcee/arcee.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import warnings
 import time
 import threading
 
 from optscale_arcee.sender.sender import Sender
 from optscale_arcee.collectors.console import (
     acquire_console, release_console)
 from optscale_arcee.name_generator import NameGenerator
@@ -32,26 +33,27 @@
             self.job()
             time.sleep(sleep)
 
 
 @single
 class Arcee:
     def __init__(
-        self, token=None, model_key=None, endpoint_url=None, ssl=True
+        self, token=None, task_key=None, endpoint_url=None, ssl=True
     ):
         self.shutdown_flag = threading.Event()
         self.token = token
-        self.model_key = model_key
+        self.task_key = task_key
         self.sender = Sender(endpoint_url, ssl, self.shutdown_flag)
         self.hb = None
         self._run = None
         self._tags = dict()
         self._name = None
         self._hyperparams = dict()
         self._dataset = None
+        self._model = None
 
     @property
     def run(self):
         return self._run
 
     @run.setter
     def run(self, value):
@@ -97,36 +99,54 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type is None:
             finish()
         else:
             error()
         return exc_type is None
 
+    @property
+    def model(self):
+        return self._model
+
+    @model.setter
+    def model(self, value):
+        self._model = value
+
 
 def init(
-    token, model_key, run_name=None, endpoint_url=None, ssl=True, period=1
+    token, task_key=None, run_name=None, endpoint_url=None, ssl=True, period=1,
+        model_key=None
 ):
+    if model_key:
+        warnings.warn(
+            "`model_key` parameter is deprecated and will be removed in the "
+            "future releases, consider using `task_key` instead",
+            UserWarning
+        )
+    if not task_key or model_key:
+        raise TypeError('`task_key` is not provided')
     acquire_console()
-    arcee = Arcee(token, model_key, endpoint_url, ssl)
+    arcee = Arcee(token, task_key or model_key, endpoint_url, ssl)
     name = (
         run_name if run_name is not None else NameGenerator.get_random_name()
     )
-    run_id = asyncio.run(arcee.sender.get_run_id(model_key, token, name))["id"]
+    run_id = asyncio.run(arcee.sender.get_run_id(
+        task_key or model_key, token, name))["id"]
     arcee.run = run_id
     arcee.name = name
     arcee.hb = Job(
         meth_args=(arcee.sender, run_id, token),
         sleep=period,
         shutdown_flag=arcee.shutdown_flag,
     )
     arcee.hb.start()
     asyncio.run(
         arcee.sender.send_stats(
             arcee.token,
-            {"project": arcee.model_key, "run": arcee.run, "data": {}},
+            {"project": arcee.task_key, "run": arcee.run, "data": {}},
         )
     )
     return arcee
 
 
 def hyperparam(key, value):
     """
@@ -159,15 +179,15 @@
 
 
 def dataset(path):
     arcee = Arcee()
     if arcee.dataset is None:
         arcee.dataset = path
         asyncio.run(arcee.sender.register_dataset(
-            arcee.run, arcee.name, arcee.model_key, path, arcee.token))
+            arcee.run, arcee.name, arcee.task_key, path, arcee.token))
 
 
 def finish():
     release_console()
     arcee = Arcee()
     try:
         asyncio.run(
@@ -218,10 +238,33 @@
 
 
 def send(data):
     arcee = Arcee()
     asyncio.run(
         arcee.sender.send_stats(
             arcee.token,
-            {"project": arcee.model_key, "run": arcee.run, "data": data},
+            {"project": arcee.task_key, "run": arcee.run, "data": data},
+        )
+    )
+
+
+def model(key, path=None):
+    arcee = Arcee()
+    arcee.model = asyncio.run(
+        arcee.sender.add_model(
+            arcee.token, key
+        )
+    )
+    asyncio.run(
+        arcee.sender.assign_model_run(
+            arcee.model, arcee.run, arcee.token, path=path
+        )
+    )
+
+
+def set_model_version(version):
+    arcee = Arcee()
+    asyncio.run(
+        arcee.sender.add_version(
+            arcee.model, arcee.run, arcee.token, version
         )
     )
```

### Comparing `optscale_arcee-0.1.37/optscale_arcee/collectors/console.py` & `optscale_arcee-0.1.38/optscale_arcee/collectors/console.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/optscale_arcee/collectors/git.py` & `optscale_arcee-0.1.38/optscale_arcee/collectors/git.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/optscale_arcee/collectors/hardware.py` & `optscale_arcee-0.1.38/optscale_arcee/collectors/hardware.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/optscale_arcee/collectors/module.py` & `optscale_arcee-0.1.38/optscale_arcee/collectors/module.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/optscale_arcee/name_generator.py` & `optscale_arcee-0.1.38/optscale_arcee/name_generator.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/optscale_arcee/platform.py` & `optscale_arcee-0.1.38/optscale_arcee/platform.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/optscale_arcee/platforms_meta/azure.py` & `optscale_arcee-0.1.38/optscale_arcee/platforms_meta/azure.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/optscale_arcee/sender/sender.py` & `optscale_arcee-0.1.38/optscale_arcee/sender/sender.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,16 +74,16 @@
         async with aiohttp.ClientSession(headers=headers) as session:
             async with session.patch(
                 url, json=data, raise_for_status=True, ssl=self.ssl
             ) as response:
                 return await response.json()
 
     @check_shutdown_flag_set
-    async def get_run_id(self, model_key, token, run_name):
-        uri = "%s/applications/%s/run" % (self.endpoint_url, model_key)
+    async def get_run_id(self, task_key, token, run_name):
+        uri = "%s/tasks/%s/run" % (self.endpoint_url, task_key)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
         data = {
             "imports": await self._imports_data(),
             "git": await self._git_data(),
             "command": await self._self_command(),
             "name": run_name
         }
@@ -132,23 +132,23 @@
         meta = await self.m()
         proc = await self._proc_data()
         data.update({"platform": meta.to_dict()})
         data.update({"proc_stats": proc})
         return await self.send_post_request(uri, headers, data)
 
     @check_shutdown_flag_set
-    async def register_dataset(self, run_id, run_name, model_key, path, token):
+    async def register_dataset(self, run_id, run_name, task_key, path, token):
         uri = f"{self.endpoint_url}/run/{run_id}/dataset_register"
         headers = {"x-api-key": token, "Content-Type": "application/json"}
 
         data = {
             "path": path,
             "name": f"Dataset {int(datetime.utcnow().timestamp())}",
             "description": f"Discovered in training "
-                           f"{model_key} - {run_name}({run_id})"
+                           f"{task_key} - {run_name}({run_id})"
         }
         await self.send_post_request(uri, headers, data)
 
     @check_shutdown_flag_set
     async def add_hyperparams(self, run_id, token, hyperparams):
         uri = "%s/run/%s" % (self.endpoint_url, run_id)
         headers = {"x-api-key": token, "Content-Type": "application/json"}
@@ -158,7 +158,29 @@
 
     async def send_console(self, run_id, token):
         uri = f"{self.endpoint_url}/run/{run_id}/consoles"
         headers = {"x-api-key": token, "Content-Type": "application/json"}
 
         data = await self._output()
         await self.send_post_request(uri, headers, data)
+
+    @check_shutdown_flag_set
+    async def add_model(self, token, key):
+        headers = {"x-api-key": token, "Content-Type": "application/json"}
+        model = await self.send_post_request(
+            self.endpoint_url + '/models', headers, {"key": key}
+        )
+        return model.get('_id')
+
+    @check_shutdown_flag_set
+    async def assign_model_run(self, model_id, run_id, token, path=None):
+        headers = {"x-api-key": token, "Content-Type": "application/json"}
+        uri = f'{self.endpoint_url}/models/{model_id}/runs/{run_id}'
+        body = {'path': path} if path else {}
+        await self.send_post_request(uri, headers, body)
+
+    @check_shutdown_flag_set
+    async def add_version(self, model_id, run_id, token, version):
+        headers = {"x-api-key": token, "Content-Type": "application/json"}
+        uri = f'{self.endpoint_url}/models/{model_id}/runs/{run_id}'
+        body = {'version': str(version)}
+        await self.send_patch_request(uri, headers, body)
```

### Comparing `optscale_arcee-0.1.37/optscale_arcee/utils.py` & `optscale_arcee-0.1.38/optscale_arcee/utils.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/optscale_arcee.egg-info/PKG-INFO` & `optscale_arcee-0.1.38/optscale_arcee.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optscale_arcee
-Version: 0.1.37
+Version: 0.1.38
 Summary: ML profiling tool for OptScale
 Home-page: https://my.optscale.com/
 Author: Hystax
 License: "Apache License 2.0"
 Project-URL: Source, https://github.com/hystax/optscale_arcee
 Keywords: arcee,ml,optscale,finops,mlops
 Requires-Python: <4,>=3.7
@@ -31,34 +31,34 @@
 First of all you need to import and init arcee in your code:
 ```sh
 import optscale_arcee as arcee
 ```
 
 ```sh
 # init arcee using context manager syntax
-with arcee.init('token', 'model_key'):
+with arcee.init('token', 'task_key'):
     # some code
 ```
 
 To use custom endpoint and enable\disable ssl checks (supports using self-signed ssl certificates):
 ```sh
-with arcee.init('token', 'model_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
+with arcee.init('token', 'task_key', endpoint_url='https://my.custom.endpoint:443/arcee/v2', ssl=False):
     # some code
 ```
 
 Alternatively arcee can be initialized via function call. However manual finish is required:
 ```sh
-arcee.init('token', 'model_key')
+arcee.init('token', 'task_key')
 # some code
 arcee.finish()
 ```
 
 Or in error case:
 ```sh
-arcee.init('token', 'model_key')
+arcee.init('token', 'task_key')
 # some code
 arcee.error()
 ```
 
 To send stats:
 ```sh
 arcee.send({"loss": 2.0012, "iter": 2, "epoch": 1})
@@ -87,7 +87,21 @@
 
 ## Logging datasets
 To log a dataset, use the dataset method with the following parameter:
 - path (str): the path of the dataset.
 ```
 arcee.dataset("dataset_path")
 ```
+
+## Models
+To create a model, use the model method with the following parameters:
+- key (str): the unique key of the model
+- path (str): the path of the run artifacts
+```
+arcee.model("my_model", "/home/user/my_model")
+```
+
+To set custom model version, use the set_model_version method with the following parameter:
+- version (str): version name
+```
+arcee.set_model_version("1.2.3-release")
+```
```

### Comparing `optscale_arcee-0.1.37/optscale_arcee.egg-info/SOURCES.txt` & `optscale_arcee-0.1.38/optscale_arcee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/setup.cfg` & `optscale_arcee-0.1.38/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = optscale_arcee
-version = 0.1.37
+version = 0.1.38
 author = Hystax
 description = ML profiling tool for OptScale
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = "Apache License 2.0"
 url = https://my.optscale.com/
 project_urls =
```

### Comparing `optscale_arcee-0.1.37/tests/test_data.py` & `optscale_arcee-0.1.38/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `optscale_arcee-0.1.37/tests/test_platform.py` & `optscale_arcee-0.1.38/tests/test_platform.py`

 * *Files identical despite different names*

