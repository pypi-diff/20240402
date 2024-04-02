# Comparing `tmp/flytekitplugins-dbt-1.9.0a0.tar.gz` & `tmp/flytekitplugins-dbt-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-dbt-1.9.0a0.tar", last modified: Thu Jul 20 18:58:16 2023, max compression
+gzip compressed data, was "flytekitplugins-dbt-1.9.1.tar", last modified: Mon Aug 28 16:43:03 2023, max compression
```

## Comparing `flytekitplugins-dbt-1.9.0a0.tar` & `flytekitplugins-dbt-1.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:16.312642 flytekitplugins-dbt-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-20 18:58:16.312642 flytekitplugins-dbt-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 18:57:54.000000 flytekitplugins-dbt-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:16.308642 flytekitplugins-dbt-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:16.312642 flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-20 18:57:54.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-20 18:57:54.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-07-20 18:57:54.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-07-20 18:57:54.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-20 18:57:54.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:16.312642 flytekitplugins-dbt-1.9.0a0/flytekitplugins_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-20 18:58:16.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 18:58:16.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:16.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:16.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins_dbt.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 18:58:16.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:16.000000 flytekitplugins-dbt-1.9.0a0/flytekitplugins_dbt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:16.312642 flytekitplugins-dbt-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-20 18:58:12.000000 flytekitplugins-dbt-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:03.890118 flytekitplugins-dbt-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)     1211 2023-08-28 16:43:03.890118 flytekitplugins-dbt-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      313 2023-08-28 16:42:38.000000 flytekitplugins-dbt-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:03.890118 flytekitplugins-dbt-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:03.890118 flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/
+-rw-r--r--   0 runner    (1001) docker     (999)      443 2023-08-28 16:42:38.000000 flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1132 2023-08-28 16:42:38.000000 flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/error.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5840 2023-08-28 16:42:38.000000 flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/schema.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11181 2023-08-28 16:42:38.000000 flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/task.py
+-rw-r--r--   0 runner    (1001) docker     (999)      996 2023-08-28 16:42:38.000000 flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/util.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:03.890118 flytekitplugins-dbt-1.9.1/flytekitplugins_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     1211 2023-08-28 16:43:03.000000 flytekitplugins-dbt-1.9.1/flytekitplugins_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      431 2023-08-28 16:43:03.000000 flytekitplugins-dbt-1.9.1/flytekitplugins_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:03.000000 flytekitplugins-dbt-1.9.1/flytekitplugins_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:03.000000 flytekitplugins-dbt-1.9.1/flytekitplugins_dbt.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       41 2023-08-28 16:43:03.000000 flytekitplugins-dbt-1.9.1/flytekitplugins_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:03.000000 flytekitplugins-dbt-1.9.1/flytekitplugins_dbt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:03.890118 flytekitplugins-dbt-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1331 2023-08-28 16:43:00.000000 flytekitplugins-dbt-1.9.1/setup.py
```

### Comparing `flytekitplugins-dbt-1.9.0a0/PKG-INFO` & `flytekitplugins-dbt-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-dbt
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: DBT Plugin for Flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-dbt
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/error.py` & `flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/error.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/schema.py` & `flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 from dataclasses import dataclass
 from typing import List, Optional
 
-from dataclasses_json import dataclass_json
+from dataclasses_json import DataClassJsonMixin
 
 
-@dataclass_json
 @dataclass
-class BaseDBTInput:
+class BaseDBTInput(DataClassJsonMixin):
     """
     Base class for DBT Task Input.
 
     Attributes
     ----------
     project_dir : str
         Path to directory containing the DBT ``dbt_project.yml``.
@@ -72,17 +71,16 @@
                     continue
 
                 args.append(str(value))
 
         return args
 
 
-@dataclass_json
 @dataclass
-class BaseDBTOutput:
+class BaseDBTOutput(DataClassJsonMixin):
     """
     Base class for output of DBT task.
 
     Attributes
     ----------
     command : str
         Complete CLI command and flags that was executed by DBT Task.
@@ -90,15 +88,14 @@
         Exit code returned by DBT CLI.
     """
 
     command: str
     exit_code: int
 
 
-@dataclass_json
 @dataclass
 class DBTRunInput(BaseDBTInput):
     """
     Input to DBT Run task.
 
     Attributes
     ----------
@@ -127,15 +124,14 @@
 
         if self.exclude is not None:
             args += ["--exclude"] + self.exclude
 
         return args
 
 
-@dataclass_json
 @dataclass
 class DBTRunOutput(BaseDBTOutput):
     """
     Output of DBT run task.
 
     Attributes
     ----------
@@ -145,15 +141,14 @@
         Raw value of DBT's ``manifest.json``.
     """
 
     raw_run_result: str
     raw_manifest: str
 
 
-@dataclass_json
 @dataclass
 class DBTTestInput(BaseDBTInput):
     """
     Input to DBT Test task.
 
     Attributes
     ----------
@@ -183,15 +178,14 @@
 
         if self.exclude is not None:
             args += ["--exclude"] + self.exclude
 
         return args
 
 
-@dataclass_json
 @dataclass
 class DBTTestOutput(BaseDBTOutput):
     """
     Output of DBT test task.
 
     Attributes
     ----------
@@ -201,15 +195,14 @@
         Raw value of DBT's ``manifest.json``.
     """
 
     raw_run_result: str
     raw_manifest: str
 
 
-@dataclass_json
 @dataclass
 class DBTFreshnessInput(BaseDBTInput):
     """
     Input to DBT Freshness task.
 
     Attributes
     ----------
@@ -239,15 +232,14 @@
 
         if self.exclude is not None:
             args += ["--exclude"] + self.exclude
 
         return args
 
 
-@dataclass_json
 @dataclass
 class DBTFreshnessOutput(BaseDBTOutput):
     """
     Output of DBT Freshness task.
 
     Attributes
     ----------
```

### Comparing `flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/task.py` & `flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dbt-1.9.0a0/flytekitplugins/dbt/util.py` & `flytekitplugins-dbt-1.9.1/flytekitplugins/dbt/util.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dbt-1.9.0a0/flytekitplugins_dbt.egg-info/PKG-INFO` & `flytekitplugins-dbt-1.9.1/flytekitplugins_dbt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-dbt
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: DBT Plugin for Flytekit
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-dbt
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-dbt-1.9.0a0/setup.py` & `flytekitplugins-dbt-1.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "dbt-core>=1.0.0",
 ]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="DBT Plugin for Flytekit",
```

