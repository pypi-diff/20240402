# Comparing `tmp/flytekitplugins-sqlalchemy-1.9.0a0.tar.gz` & `tmp/flytekitplugins-sqlalchemy-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-sqlalchemy-1.9.0a0.tar", last modified: Thu Jul 20 18:58:27 2023, max compression
+gzip compressed data, was "flytekitplugins-sqlalchemy-1.9.1.tar", last modified: Mon Aug 28 16:43:14 2023, max compression
```

## Comparing `flytekitplugins-sqlalchemy-1.9.0a0.tar` & `flytekitplugins-sqlalchemy-1.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:27.344756 flytekitplugins-sqlalchemy-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-20 18:58:27.344756 flytekitplugins-sqlalchemy-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 18:57:54.000000 flytekitplugins-sqlalchemy-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:27.340756 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:27.344756 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins/sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 18:57:54.000000 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins/sqlalchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-20 18:57:54.000000 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins/sqlalchemy/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:27.344756 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins_sqlalchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-20 18:58:27.000000 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins_sqlalchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 18:58:27.000000 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins_sqlalchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:27.000000 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins_sqlalchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:27.000000 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins_sqlalchemy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 18:58:27.000000 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins_sqlalchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:27.000000 flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins_sqlalchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:27.344756 flytekitplugins-sqlalchemy-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-20 18:58:13.000000 flytekitplugins-sqlalchemy-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:14.498133 flytekitplugins-sqlalchemy-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)      789 2023-08-28 16:43:14.498133 flytekitplugins-sqlalchemy-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-28 16:42:38.000000 flytekitplugins-sqlalchemy-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:14.498133 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:14.498133 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins/sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-28 16:42:38.000000 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins/sqlalchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5607 2023-08-28 16:42:38.000000 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins/sqlalchemy/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:43:14.498133 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins_sqlalchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)      789 2023-08-28 16:43:14.000000 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins_sqlalchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      400 2023-08-28 16:43:14.000000 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins_sqlalchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:43:14.000000 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins_sqlalchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:14.000000 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins_sqlalchemy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       43 2023-08-28 16:43:14.000000 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins_sqlalchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       16 2023-08-28 16:43:14.000000 flytekitplugins-sqlalchemy-1.9.1/flytekitplugins_sqlalchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 16:43:14.498133 flytekitplugins-sqlalchemy-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1156 2023-08-28 16:43:00.000000 flytekitplugins-sqlalchemy-1.9.1/setup.py
```

### Comparing `flytekitplugins-sqlalchemy-1.9.0a0/PKG-INFO` & `flytekitplugins-sqlalchemy-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-sqlalchemy
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: SQLAlchemy plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-sqlalchemy-1.9.0a0/README.md` & `flytekitplugins-sqlalchemy-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins/sqlalchemy/task.py` & `flytekitplugins-sqlalchemy-1.9.1/flytekitplugins/sqlalchemy/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from flytekit import current_context, kwtypes
 from flytekit.configuration import SerializationSettings
 from flytekit.configuration.default_images import DefaultImages, PythonVersion
 from flytekit.core.base_sql_task import SQLTask
 from flytekit.core.python_customized_container_task import PythonCustomizedContainerTask
 from flytekit.core.shim_task import ShimTaskExecutor
+from flytekit.loggers import logger
 from flytekit.models import task as task_models
 from flytekit.models.security import Secret
 from flytekit.types.schema import FlyteSchema
 
 
 class SQLAlchemyDefaultImages(DefaultImages):
     """Default images for the sqlalchemy flytekit plugin."""
@@ -122,18 +123,18 @@
     def execute_from_model(self, tt: task_models.TaskTemplate, **kwargs) -> typing.Any:
         if tt.custom["secret_connect_args"] is not None:
             for key, secret_dict in tt.custom["secret_connect_args"].items():
                 value = current_context().secrets.get(group=secret_dict["group"], key=secret_dict["key"])
                 tt.custom["connect_args"][key] = value
 
         engine = create_engine(tt.custom["uri"], connect_args=tt.custom["connect_args"], echo=False)
-        print(f"Connecting to db {tt.custom['uri']}")
+        logger.info(f"Connecting to db {tt.custom['uri']}")
 
         interpolated_query = SQLAlchemyTask.interpolate_query(tt.custom["query_template"], **kwargs)
-        print(f"Interpolated query {interpolated_query}")
+        logger.info(f"Interpolated query {interpolated_query}")
         with engine.begin() as connection:
             df = None
             if tt.interface.outputs:
                 df = pd.read_sql_query(text(interpolated_query), connection)
             else:
                 pandasSQL_builder(connection).execute(text(interpolated_query))
         return df
```

### Comparing `flytekitplugins-sqlalchemy-1.9.0a0/flytekitplugins_sqlalchemy.egg-info/PKG-INFO` & `flytekitplugins-sqlalchemy-1.9.1/flytekitplugins_sqlalchemy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-sqlalchemy
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: SQLAlchemy plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-sqlalchemy-1.9.0a0/setup.py` & `flytekitplugins-sqlalchemy-1.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "sqlalchemy"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "sqlalchemy>=1.4.7"]
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="dolthub",
     author_email="max@dolthub.com",
     description="SQLAlchemy plugin for flytekit",
```

