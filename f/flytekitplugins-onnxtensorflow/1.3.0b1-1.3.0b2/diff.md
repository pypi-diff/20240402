# Comparing `tmp/flytekitplugins-onnxtensorflow-1.3.0b1.tar.gz` & `tmp/flytekitplugins-onnxtensorflow-1.3.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-onnxtensorflow-1.3.0b1.tar", last modified: Mon Nov  7 16:40:36 2022, max compression
+gzip compressed data, was "flytekitplugins-onnxtensorflow-1.3.0b2.tar", last modified: Thu Dec  8 20:39:06 2022, max compression
```

## Comparing `flytekitplugins-onnxtensorflow-1.3.0b1.tar` & `flytekitplugins-onnxtensorflow-1.3.0b2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 16:40:36.312969 flytekitplugins-onnxtensorflow-1.3.0b1/
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-07 16:40:36.312969 flytekitplugins-onnxtensorflow-1.3.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-11-07 16:40:10.000000 flytekitplugins-onnxtensorflow-1.3.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 16:40:36.312969 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 16:40:36.312969 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins/onnxtensorflow/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-11-07 16:40:10.000000 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins/onnxtensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4846 2022-11-07 16:40:10.000000 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins/onnxtensorflow/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-07 16:40:36.312969 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins_onnxtensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-07 16:40:36.000000 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins_onnxtensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-07 16:40:36.000000 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins_onnxtensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-07 16:40:36.000000 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins_onnxtensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-07 16:40:36.000000 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins_onnxtensorflow.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-07 16:40:36.000000 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins_onnxtensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-07 16:40:36.000000 flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins_onnxtensorflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-07 16:40:36.312969 flytekitplugins-onnxtensorflow-1.3.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-11-07 16:40:28.000000 flytekitplugins-onnxtensorflow-1.3.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:06.329567 flytekitplugins-onnxtensorflow-1.3.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-08 20:39:06.325567 flytekitplugins-onnxtensorflow-1.3.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-08 20:38:40.000000 flytekitplugins-onnxtensorflow-1.3.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:06.325567 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:06.325567 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins/onnxtensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-08 20:38:40.000000 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins/onnxtensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2022-12-08 20:38:40.000000 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins/onnxtensorflow/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 20:39:06.325567 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins_onnxtensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2022-12-08 20:39:06.000000 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins_onnxtensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2022-12-08 20:39:06.000000 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins_onnxtensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 20:39:06.000000 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins_onnxtensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-08 20:39:06.000000 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins_onnxtensorflow.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-08 20:39:06.000000 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins_onnxtensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-08 20:39:06.000000 flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins_onnxtensorflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 20:39:06.329567 flytekitplugins-onnxtensorflow-1.3.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2022-12-08 20:38:58.000000 flytekitplugins-onnxtensorflow-1.3.0b2/setup.py
```

### Comparing `flytekitplugins-onnxtensorflow-1.3.0b1/PKG-INFO` & `flytekitplugins-onnxtensorflow-1.3.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxtensorflow
-Version: 1.3.0b1
+Version: 1.3.0b2
 Summary: ONNX TensorFlow Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins/onnxtensorflow/schema.py` & `flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins/onnxtensorflow/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-onnxtensorflow-1.3.0b1/flytekitplugins_onnxtensorflow.egg-info/PKG-INFO` & `flytekitplugins-onnxtensorflow-1.3.0b2/flytekitplugins_onnxtensorflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxtensorflow
-Version: 1.3.0b1
+Version: 1.3.0b2
 Summary: ONNX TensorFlow Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxtensorflow-1.3.0b1/setup.py` & `flytekitplugins-onnxtensorflow-1.3.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "onnxtensorflow"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.1.0b0,<2.0.0", "tf2onnx>=1.9.3", "tensorflow>=2.7.0"]
 
-__version__ = "1.3.0b1"
+__version__ = "1.3.0b2"
 
 setup(
     name=f"flytekitplugins-{PLUGIN_NAME}",
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="ONNX TensorFlow Plugin for Flytekit",
```

