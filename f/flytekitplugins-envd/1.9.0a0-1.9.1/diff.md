# Comparing `tmp/flytekitplugins-envd-1.9.0a0.tar.gz` & `tmp/flytekitplugins-envd-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-envd-1.9.0a0.tar", last modified: Thu Jul 20 18:58:18 2023, max compression
+gzip compressed data, was "flytekitplugins-envd-1.9.1.tar", last modified: Mon Aug 28 16:43:05 2023, max compression
```

## Comparing `flytekitplugins-envd-1.9.0a0.tar` & `flytekitplugins-envd-1.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.196665 flytekitplugins-envd-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-20 18:58:18.196665 flytekitplugins-envd-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-20 18:57:54.000000 flytekitplugins-envd-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.192665 flytekitplugins-envd-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.196665 flytekitplugins-envd-1.9.0a0/flytekitplugins/envd/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-20 18:57:54.000000 flytekitplugins-envd-1.9.0a0/flytekitplugins/envd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-20 18:57:54.000000 flytekitplugins-envd-1.9.0a0/flytekitplugins/envd/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:18.196665 flytekitplugins-envd-1.9.0a0/flytekitplugins_envd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-20 18:58:18.000000 flytekitplugins-envd-1.9.0a0/flytekitplugins_envd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-20 18:58:18.000000 flytekitplugins-envd-1.9.0a0/flytekitplugins_envd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:18.000000 flytekitplugins-envd-1.9.0a0/flytekitplugins_envd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 18:58:18.000000 flytekitplugins-envd-1.9.0a0/flytekitplugins_envd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:18.000000 flytekitplugins-envd-1.9.0a0/flytekitplugins_envd.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 18:58:18.000000 flytekitplugins-envd-1.9.0a0/flytekitplugins_envd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:18.000000 flytekitplugins-envd-1.9.0a0/flytekitplugins_envd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:18.196665 flytekitplugins-envd-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-20 18:58:12.000000 flytekitplugins-envd-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:05.762122 flytekitplugins-envd-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      886 2023-08-28 16:43:05.762122 flytekitplugins-envd-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      797 2023-08-28 16:42:38.000000 flytekitplugins-envd-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:05.762122 flytekitplugins-envd-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:05.762122 flytekitplugins-envd-1.9.1/flytekitplugins/envd/
+-rw-r--r--   0 runner    (1001) docker     (999)      255 2023-08-28 16:42:38.000000 flytekitplugins-envd-1.9.1/flytekitplugins/envd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3905 2023-08-28 16:42:38.000000 flytekitplugins-envd-1.9.1/flytekitplugins/envd/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:05.762122 flytekitplugins-envd-1.9.1/flytekitplugins_envd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      886 2023-08-28 16:43:05.000000 flytekitplugins-envd-1.9.1/flytekitplugins_envd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      408 2023-08-28 16:43:05.000000 flytekitplugins-envd-1.9.1/flytekitplugins_envd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:05.000000 flytekitplugins-envd-1.9.1/flytekitplugins_envd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       47 2023-08-28 16:43:05.000000 flytekitplugins-envd-1.9.1/flytekitplugins_envd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:05.000000 flytekitplugins-envd-1.9.1/flytekitplugins_envd.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       22 2023-08-28 16:43:05.000000 flytekitplugins-envd-1.9.1/flytekitplugins_envd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:05.000000 flytekitplugins-envd-1.9.1/flytekitplugins_envd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:05.762122 flytekitplugins-envd-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1320 2023-08-28 16:43:00.000000 flytekitplugins-envd-1.9.1/setup.py
```

### Comparing `flytekitplugins-envd-1.9.0a0/PKG-INFO` & `flytekitplugins-envd-1.9.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.9.0a0/README.md` & `flytekitplugins-envd-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-envd-1.9.0a0/flytekitplugins/envd/image_builder.py` & `flytekitplugins-envd-1.9.1/flytekitplugins/envd/image_builder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,90 @@
+import os
 import pathlib
 import shutil
 import subprocess
 
 import click
 
 from flytekit.configuration import DefaultImages
 from flytekit.core import context_manager
+from flytekit.core.constants import REQUIREMENTS_FILE_NAME
 from flytekit.image_spec.image_spec import _F_IMG_ID, ImageBuildEngine, ImageSpec, ImageSpecBuilder
 
 
 class EnvdImageSpecBuilder(ImageSpecBuilder):
     """
     This class is used to build a docker image using envd.
     """
 
-    def build_image(self, image_spec: ImageSpec):
-        cfg_path = create_envd_config(image_spec)
-        command = f"envd build --path {pathlib.Path(cfg_path).parent}  --platform {image_spec.platform}"
-        if image_spec.registry:
-            command += f" --output type=image,name={image_spec.image_name()},push=true"
+    def execute_command(self, command):
         click.secho(f"Run command: {command} ", fg="blue")
         p = subprocess.Popen(command.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         for line in iter(p.stdout.readline, ""):
             if p.poll() is not None:
                 break
             if line.decode().strip() != "":
                 click.secho(line.decode().strip(), fg="blue")
 
         if p.returncode != 0:
             _, stderr = p.communicate()
-            raise Exception(
-                f"failed to build the imageSpec at {cfg_path} with error {stderr}",
-            )
+            raise Exception(f"failed to run command {command} with error {stderr}")
+
+    def build_image(self, image_spec: ImageSpec):
+        cfg_path = create_envd_config(image_spec)
+
+        if image_spec.registry_config:
+            bootstrap_command = f"envd bootstrap --registry-config {image_spec.registry_config}"
+            self.execute_command(bootstrap_command)
+
+        build_command = f"envd build --path {pathlib.Path(cfg_path).parent}  --platform {image_spec.platform}"
+        if image_spec.registry:
+            build_command += f" --output type=image,name={image_spec.image_name()},push=true"
+        self.execute_command(build_command)
 
 
 def create_envd_config(image_spec: ImageSpec) -> str:
     base_image = DefaultImages.default_image() if image_spec.base_image is None else image_spec.base_image
+    if image_spec.cuda:
+        if image_spec.python_version is None:
+            raise Exception("python_version is required when cuda and cudnn are specified")
+        base_image = "ubuntu20.04"
+
     packages = [] if image_spec.packages is None else image_spec.packages
     apt_packages = [] if image_spec.apt_packages is None else image_spec.apt_packages
     env = {"PYTHONPATH": "/root", _F_IMG_ID: image_spec.image_name()}
     if image_spec.env:
         env.update(image_spec.env)
+    pip_index = "https://pypi.org/simple" if image_spec.pip_index is None else image_spec.pip_index
 
     envd_config = f"""# syntax=v1
 
 def build():
     base(image="{base_image}", dev=False)
-    install.python_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', packages)))}])
-    install.apt_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', apt_packages)))}])
+    install.python_packages(name=[{', '.join(map(str, map(lambda x: f'"{x}"', packages)))}])
+    install.apt_packages(name=[{', '.join(map(str, map(lambda x: f'"{x}"', apt_packages)))}])
     runtime.environ(env={env})
+    config.pip_index(url="{pip_index}")
 """
+    ctx = context_manager.FlyteContextManager.current_context()
+    cfg_path = ctx.file_access.get_random_local_path("build.envd")
+    pathlib.Path(cfg_path).parent.mkdir(parents=True, exist_ok=True)
+
+    if image_spec.requirements:
+        requirement_path = f"{pathlib.Path(cfg_path).parent}{os.sep}{REQUIREMENTS_FILE_NAME}"
+        shutil.copyfile(image_spec.requirements, requirement_path)
+        envd_config += f'    install.python_packages(requirements="{REQUIREMENTS_FILE_NAME}")\n'
 
     if image_spec.python_version:
         # Indentation is required by envd
         envd_config += f'    install.python(version="{image_spec.python_version}")\n'
 
-    ctx = context_manager.FlyteContextManager.current_context()
-    cfg_path = ctx.file_access.get_random_local_path("build.envd")
-    pathlib.Path(cfg_path).parent.mkdir(parents=True, exist_ok=True)
+    if image_spec.cuda:
+        cudnn = image_spec.cudnn if image_spec.cudnn else ""
+        envd_config += f'    install.cuda(version="{image_spec.cuda}", cudnn="{cudnn}")\n'
 
     if image_spec.source_root:
         shutil.copytree(image_spec.source_root, pathlib.Path(cfg_path).parent, dirs_exist_ok=True)
         # Indentation is required by envd
         envd_config += '    io.copy(host_path="./", envd_path="/root")'
 
     with open(cfg_path, "w+") as f:
```

### Comparing `flytekitplugins-envd-1.9.0a0/flytekitplugins_envd.egg-info/PKG-INFO` & `flytekitplugins-envd-1.9.1/flytekitplugins_envd.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.9.0a0/setup.py` & `flytekitplugins-envd-1.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 PLUGIN_NAME = "envd"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = ["flytekit", "envd>=0.3.22"]
+plugin_requires = ["flytekit", "envd>=0.3.33"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables users to easily build a Docker image for tasks or workflows.",
```

