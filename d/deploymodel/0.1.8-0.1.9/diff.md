# Comparing `tmp/deploymodel-0.1.8.tar.gz` & `tmp/deploymodel-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deploymodel-0.1.8.tar", max compression
+gzip compressed data, was "deploymodel-0.1.9.tar", max compression
```

## Comparing `deploymodel-0.1.8.tar` & `deploymodel-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      330 2024-03-29 10:48:57.451898 deploymodel-0.1.8/README.md
--rw-r--r--   0        0        0       84 2024-03-15 20:50:46.703155 deploymodel-0.1.8/deploymodel/__init__.py
--rw-r--r--   0        0        0     1383 2024-03-26 19:39:22.244956 deploymodel-0.1.8/deploymodel/docker_utils.py
--rw-r--r--   0        0        0      275 2024-03-29 10:52:08.397886 deploymodel-0.1.8/deploymodel/io/__init__.py
--rw-r--r--   0        0        0     6007 2024-03-29 11:19:50.262290 deploymodel-0.1.8/deploymodel/main.py
--rw-r--r--   0        0        0     2773 2024-03-26 19:39:22.244956 deploymodel-0.1.8/deploymodel/serverless/__init__.py
--rw-r--r--   0        0        0      243 2024-03-25 21:01:50.720395 deploymodel-0.1.8/deploymodel/set_env.py
--rw-r--r--   0        0        0       41 2024-03-27 17:33:50.532123 deploymodel-0.1.8/deploymodel/settings.py
--rw-r--r--   0        0        0      654 2024-03-29 11:20:16.414555 deploymodel-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 deploymodel-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      330 2024-03-29 10:48:57.451898 deploymodel-0.1.9/README.md
+-rw-r--r--   0        0        0       84 2024-03-15 20:50:46.703155 deploymodel-0.1.9/deploymodel/__init__.py
+-rw-r--r--   0        0        0     1476 2024-03-29 15:57:28.867863 deploymodel-0.1.9/deploymodel/docker_utils.py
+-rw-r--r--   0        0        0      275 2024-03-29 10:52:08.397886 deploymodel-0.1.9/deploymodel/io/__init__.py
+-rw-r--r--   0        0        0     6043 2024-03-29 14:35:10.889500 deploymodel-0.1.9/deploymodel/main.py
+-rw-r--r--   0        0        0     2773 2024-03-26 19:39:22.244956 deploymodel-0.1.9/deploymodel/serverless/__init__.py
+-rw-r--r--   0        0        0      243 2024-03-25 21:01:50.720395 deploymodel-0.1.9/deploymodel/set_env.py
+-rw-r--r--   0        0        0       41 2024-03-27 17:33:50.532123 deploymodel-0.1.9/deploymodel/settings.py
+-rw-r--r--   0        0        0      654 2024-03-29 15:56:58.327557 deploymodel-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 deploymodel-0.1.9/PKG-INFO
```

### Comparing `deploymodel-0.1.8/deploymodel/docker_utils.py` & `deploymodel-0.1.9/deploymodel/docker_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,34 +22,38 @@
     try:
         output = client.images.push(name, tag, stream=True, decode=True)
     except docker.errors.APIError as e:
         logger.error(e)
         raise
     for line in output:
         if "errorDetail" in line:
-            raise RuntimeError(f"Failed to push {name}:{tag} - {line['errorDetail']['message']}")
+            raise RuntimeError(
+                f"Failed to push {name}:{tag} - {line['errorDetail']['message']}"
+            )
 
 
 def build_image(
     context: Path,
     tag: str,
     buildargs: dict = None,
     rm: bool = True,
     quiet: bool = False,
     nocache: bool = False,
+    dockerfile: str = None,
 ):
     buildargs = buildargs or {}
     client = docker.from_env()
     try:
         image, build_logs = client.images.build(
             path=str(context),
             tag=tag,
             rm=rm,
             quiet=quiet,
             buildargs=buildargs,
             nocache=nocache,
+            dockerfile=dockerfile,
         )
     except docker.errors.BuildError as e:
         log_docker_error(e.build_log)
         raise
     log_docker_output(build_logs)
     return image
```

### Comparing `deploymodel-0.1.8/deploymodel/main.py` & `deploymodel-0.1.9/deploymodel/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,18 +97,19 @@
 def build_docker_image(
     dockerfile: Path, token: str, nocache: bool = False
 ) -> docker.models.images.Image:
     client = docker.from_env()
     context = Path(dockerfile).parent
 
     logger.info(
-        f"Building Docker image from context={str(context)} (dockerfile={str(dockerfile)})"
+        f"Building Docker image from context={str(context)} (dockerfile={dockerfile.name})"
     )
     image = docker_utils.build_image(
         context=context,
+        dockerfile=dockerfile.name,
         tag=f"dm-build-{token}".lower(),
         rm=True,
         quiet=False,
         nocache=nocache,
     )
     logger.debug("Docker image built successfully")
     module, handler, init = get_module_and_handler_and_init(client, image)
```

### Comparing `deploymodel-0.1.8/deploymodel/serverless/__init__.py` & `deploymodel-0.1.9/deploymodel/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `deploymodel-0.1.8/pyproject.toml` & `deploymodel-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deploymodel"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Hello <accounts@deploymodel.com>"]
 readme = "README.md"
 homepage = "https://deploymodel.com"
 repository = "https://github.com/DeployModel/deploymodel-templates"
```

### Comparing `deploymodel-0.1.8/PKG-INFO` & `deploymodel-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deploymodel
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://deploymodel.com
 Author: Hello
 Author-email: accounts@deploymodel.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

