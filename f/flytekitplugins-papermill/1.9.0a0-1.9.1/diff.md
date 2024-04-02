# Comparing `tmp/flytekitplugins-papermill-1.9.0a0.tar.gz` & `tmp/flytekitplugins-papermill-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-papermill-1.9.0a0.tar", last modified: Thu Jul 20 18:58:24 2023, max compression
+gzip compressed data, was "flytekitplugins-papermill-1.9.1.tar", last modified: Mon Aug 28 16:43:11 2023, max compression
```

## Comparing `flytekitplugins-papermill-1.9.0a0.tar` & `flytekitplugins-papermill-1.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.484729 flytekitplugins-papermill-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-20 18:58:24.484729 flytekitplugins-papermill-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-20 18:57:54.000000 flytekitplugins-papermill-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.484729 flytekitplugins-papermill-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.484729 flytekitplugins-papermill-1.9.0a0/flytekitplugins/papermill/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 18:57:54.000000 flytekitplugins-papermill-1.9.0a0/flytekitplugins/papermill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15374 2023-07-20 18:57:54.000000 flytekitplugins-papermill-1.9.0a0/flytekitplugins/papermill/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:24.484729 flytekitplugins-papermill-1.9.0a0/flytekitplugins_papermill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-20 18:58:24.000000 flytekitplugins-papermill-1.9.0a0/flytekitplugins_papermill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-20 18:58:24.000000 flytekitplugins-papermill-1.9.0a0/flytekitplugins_papermill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:24.000000 flytekitplugins-papermill-1.9.0a0/flytekitplugins_papermill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:24.000000 flytekitplugins-papermill-1.9.0a0/flytekitplugins_papermill.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 18:58:24.000000 flytekitplugins-papermill-1.9.0a0/flytekitplugins_papermill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:24.000000 flytekitplugins-papermill-1.9.0a0/flytekitplugins_papermill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:24.484729 flytekitplugins-papermill-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-20 18:58:12.000000 flytekitplugins-papermill-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:11.986128 flytekitplugins-papermill-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      796 2023-08-28 16:43:11.986128 flytekitplugins-papermill-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      789 2023-08-28 16:42:38.000000 flytekitplugins-papermill-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:11.986128 flytekitplugins-papermill-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:11.986128 flytekitplugins-papermill-1.9.1/flytekitplugins/papermill/
+-rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-28 16:42:38.000000 flytekitplugins-papermill-1.9.1/flytekitplugins/papermill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15569 2023-08-28 16:42:38.000000 flytekitplugins-papermill-1.9.1/flytekitplugins/papermill/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:11.986128 flytekitplugins-papermill-1.9.1/flytekitplugins_papermill.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      796 2023-08-28 16:43:11.000000 flytekitplugins-papermill-1.9.1/flytekitplugins_papermill.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      392 2023-08-28 16:43:11.000000 flytekitplugins-papermill-1.9.1/flytekitplugins_papermill.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:11.000000 flytekitplugins-papermill-1.9.1/flytekitplugins_papermill.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:11.000000 flytekitplugins-papermill-1.9.1/flytekitplugins_papermill.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       60 2023-08-28 16:43:11.000000 flytekitplugins-papermill-1.9.1/flytekitplugins_papermill.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:11.000000 flytekitplugins-papermill-1.9.1/flytekitplugins_papermill.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:11.986128 flytekitplugins-papermill-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1205 2023-08-28 16:43:00.000000 flytekitplugins-papermill-1.9.1/setup.py
```

### Comparing `flytekitplugins-papermill-1.9.0a0/PKG-INFO` & `flytekitplugins-papermill-1.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.9.0a0/README.md` & `flytekitplugins-papermill-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.9.0a0/flytekitplugins/papermill/task.py` & `flytekitplugins-papermill-1.9.1/flytekitplugins/papermill/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         name: str,
         notebook_path: str,
         render_deck: bool = False,
         stream_logs: bool = False,
         task_config: T = None,
         inputs: typing.Optional[typing.Dict[str, typing.Type]] = None,
         outputs: typing.Optional[typing.Dict[str, typing.Type]] = None,
+        output_notebooks: typing.Optional[bool] = True,
         **kwargs,
     ):
         # Each instance of NotebookTask instantiates an underlying task with a dummy function that will only be used
         # to run pre- and post- execute functions using the corresponding task plugin.
         # We rename the function name here to ensure the generated task has a unique name and avoid duplicate task name
         # errors.
         # This seem like a hack. We should use a plugin_class that doesn't require a fake-function to make work.
@@ -161,21 +162,24 @@
             papermill_logger.addHandler(logging.StreamHandler(sys.stdout))
             # Papermill leaves the default level of DEBUG. We increase it here.
             papermill_logger.setLevel(logging.INFO)
 
         if not os.path.exists(self._notebook_path):
             raise ValueError(f"Illegal notebook path passed in {self._notebook_path}")
 
-        if outputs:
+        if output_notebooks:
+            if outputs is None:
+                outputs = {}
             outputs.update(
                 {
                     self._IMPLICIT_OP_NOTEBOOK: self._IMPLICIT_OP_NOTEBOOK_TYPE,
                     self._IMPLICIT_RENDERED_NOTEBOOK: self._IMPLICIT_RENDERED_NOTEBOOK_TYPE,
                 }
             )
+
         super().__init__(
             name,
             task_config,
             task_type=task_type,
             task_type_version=task_type_version,
             interface=Interface(inputs=inputs, outputs=outputs),
             **kwargs,
@@ -283,14 +287,16 @@
                 output_list.append(self.rendered_output_path)
             elif k in m:
                 v = TypeEngine.to_python_value(ctx=FlyteContext.current_context(), lv=m[k], expected_python_type=type_v)
                 output_list.append(v)
             else:
                 raise TypeError(f"Expected output {k} of type {type_v} not found in the notebook outputs")
 
+        if len(output_list) == 1:
+            return output_list[0]
         return tuple(output_list)
 
     def post_execute(self, user_params: ExecutionParameters, rval: Any) -> Any:
         if self._render_deck:
             nb_deck = Deck(self._IMPLICIT_RENDERED_NOTEBOOK)
             with open(self.rendered_output_path, "r") as f:
                 notebook_html = f.read()
```

### Comparing `flytekitplugins-papermill-1.9.0a0/flytekitplugins_papermill.egg-info/PKG-INFO` & `flytekitplugins-papermill-1.9.1/flytekitplugins_papermill.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.9.0a0/setup.py` & `flytekitplugins-papermill-1.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 PLUGIN_NAME = "papermill"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
-    "flytekit>=1.3.0b2,<2.0.0",
+    "flytekit",
     "papermill>=1.2.0",
     "nbconvert>=6.0.7",
     "ipykernel>=5.0.0",
 ]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is the flytekit papermill plugin",
```

