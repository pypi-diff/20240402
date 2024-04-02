# Comparing `tmp/flytekitplugins-awssagemaker-1.9.0a0.tar.gz` & `tmp/flytekitplugins-awssagemaker-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-awssagemaker-1.9.0a0.tar", last modified: Thu Jul 20 18:58:14 2023, max compression
+gzip compressed data, was "flytekitplugins-awssagemaker-1.9.1.tar", last modified: Mon Aug 28 16:43:02 2023, max compression
```

## Comparing `flytekitplugins-awssagemaker-1.9.0a0.tar` & `flytekitplugins-awssagemaker-1.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.372617 flytekitplugins-awssagemaker-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-20 18:58:14.372617 flytekitplugins-awssagemaker-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.368617 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.372617 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/distributed_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     7141 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.372617 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/models/hpo_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/models/parameter_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/models/training_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.372617 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins_awssagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-20 18:58:14.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins_awssagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-20 18:58:14.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins_awssagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:14.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins_awssagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:14.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins_awssagemaker.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 18:58:14.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins_awssagemaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:14.000000 flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins_awssagemaker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:14.372617 flytekitplugins-awssagemaker-1.9.0a0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-20 18:57:54.000000 flytekitplugins-awssagemaker-1.9.0a0/scripts/flytekit_sagemaker_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:14.372617 flytekitplugins-awssagemaker-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-20 18:58:12.000000 flytekitplugins-awssagemaker-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.014115 flytekitplugins-awssagemaker-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      786 2023-08-28 16:43:02.014115 flytekitplugins-awssagemaker-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1182 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.010115 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.010115 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/
+-rw-r--r--   0 runner    (1001) docker     (999)     2446 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3034 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/distributed_training.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7141 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.010115 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/models/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6916 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/models/hpo_job.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10533 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/models/parameter_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11779 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/models/training_job.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8464 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/training.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.010115 flytekitplugins-awssagemaker-1.9.1/flytekitplugins_awssagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      786 2023-08-28 16:43:01.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins_awssagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      749 2023-08-28 16:43:01.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins_awssagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:01.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins_awssagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:01.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins_awssagemaker.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       72 2023-08-28 16:43:01.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins_awssagemaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:01.000000 flytekitplugins-awssagemaker-1.9.1/flytekitplugins_awssagemaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:02.014115 flytekitplugins-awssagemaker-1.9.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (999)     3790 2023-08-28 16:42:38.000000 flytekitplugins-awssagemaker-1.9.1/scripts/flytekit_sagemaker_runner.py
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:02.014115 flytekitplugins-awssagemaker-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-28 16:43:00.000000 flytekitplugins-awssagemaker-1.9.1/setup.py
```

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/PKG-INFO` & `flytekitplugins-awssagemaker-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-awssagemaker
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: AWS Plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/README.md` & `flytekitplugins-awssagemaker-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/__init__.py` & `flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/distributed_training.py` & `flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/distributed_training.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/hpo.py` & `flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/hpo.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/models/hpo_job.py` & `flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/models/hpo_job.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/models/parameter_ranges.py` & `flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/models/parameter_ranges.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/models/training_job.py` & `flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/models/training_job.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins/awssagemaker/training.py` & `flytekitplugins-awssagemaker-1.9.1/flytekitplugins/awssagemaker/training.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins_awssagemaker.egg-info/PKG-INFO` & `flytekitplugins-awssagemaker-1.9.1/flytekitplugins_awssagemaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-awssagemaker
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: AWS Plugins for flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/flytekitplugins_awssagemaker.egg-info/SOURCES.txt` & `flytekitplugins-awssagemaker-1.9.1/flytekitplugins_awssagemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/scripts/flytekit_sagemaker_runner.py` & `flytekitplugins-awssagemaker-1.9.1/scripts/flytekit_sagemaker_runner.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-awssagemaker-1.9.0a0/setup.py` & `flytekitplugins-awssagemaker-1.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "awssagemaker"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "sagemaker-training>=3.6.2,<4.0.0", "retry2==0.9.5"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 # TODO: move sagemaker install script here.
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
```

