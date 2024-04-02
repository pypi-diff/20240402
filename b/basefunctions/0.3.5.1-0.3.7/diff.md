# Comparing `tmp/basefunctions-0.3.5.1.tar.gz` & `tmp/basefunctions-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basefunctions-0.3.5.1.tar", last modified: Sun Mar 24 19:47:45 2024, max compression
+gzip compressed data, was "basefunctions-0.3.7.tar", last modified: Tue Apr  2 18:09:34 2024, max compression
```

## Comparing `basefunctions-0.3.5.1.tar` & `basefunctions-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-03-24 19:47:45.483404 basefunctions-0.3.5.1/
--rw-r--r--   0 neutro2    (501) staff       (20)     7053 2024-03-24 19:47:45.482903 basefunctions-0.3.5.1/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-03-22 21:23:12.000000 basefunctions-0.3.5.1/license
--rw-r--r--   0 neutro2    (501) staff       (20)     1070 2024-03-24 19:46:14.000000 basefunctions-0.3.5.1/pyproject.toml
--rw-r--r--   0 neutro2    (501) staff       (20)     5040 2024-03-24 19:45:37.000000 basefunctions-0.3.5.1/readme.md
--rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-03-24 19:47:45.483510 basefunctions-0.3.5.1/setup.cfg
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-03-24 19:47:45.472487 basefunctions-0.3.5.1/src/
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-03-24 19:47:45.477794 basefunctions-0.3.5.1/src/basefunctions/
--rw-r--r--   0 neutro2    (501) staff       (20)     2456 2024-03-24 19:36:31.000000 basefunctions-0.3.5.1/src/basefunctions/__init__.py
--rw-r--r--   0 neutro2    (501) staff       (20)     4218 2024-03-23 18:23:48.000000 basefunctions-0.3.5.1/src/basefunctions/database.py
--rw-r--r--   0 neutro2    (501) staff       (20)    14876 2024-03-22 21:23:12.000000 basefunctions-0.3.5.1/src/basefunctions/filefunctions.py
--rw-r--r--   0 neutro2    (501) staff       (20)    15673 2024-03-24 15:36:32.000000 basefunctions-0.3.5.1/src/basefunctions/threadpool.py
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-03-24 19:47:45.481959 basefunctions-0.3.5.1/src/basefunctions.egg-info/
--rw-r--r--   0 neutro2    (501) staff       (20)     7053 2024-03-24 19:47:45.000000 basefunctions-0.3.5.1/src/basefunctions.egg-info/PKG-INFO
--rw-r--r--   0 neutro2    (501) staff       (20)      409 2024-03-24 19:47:45.000000 basefunctions-0.3.5.1/src/basefunctions.egg-info/SOURCES.txt
--rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-03-24 19:47:45.000000 basefunctions-0.3.5.1/src/basefunctions.egg-info/dependency_links.txt
--rw-r--r--   0 neutro2    (501) staff       (20)       97 2024-03-24 19:47:45.000000 basefunctions-0.3.5.1/src/basefunctions.egg-info/requires.txt
--rw-r--r--   0 neutro2    (501) staff       (20)       14 2024-03-24 19:47:45.000000 basefunctions-0.3.5.1/src/basefunctions.egg-info/top_level.txt
-drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-03-24 19:47:45.480576 basefunctions-0.3.5.1/tests/
--rw-r--r--   0 neutro2    (501) staff       (20)    23668 2024-03-22 21:23:12.000000 basefunctions-0.3.5.1/tests/test_filefunctions.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.223413 basefunctions-0.3.7/
+-rw-r--r--   0 neutro2    (501) staff       (20)     7051 2024-04-02 18:09:34.222602 basefunctions-0.3.7/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)     1074 2024-03-22 21:23:12.000000 basefunctions-0.3.7/license
+-rw-r--r--   0 neutro2    (501) staff       (20)     1068 2024-03-29 12:54:00.000000 basefunctions-0.3.7/pyproject.toml
+-rw-r--r--   0 neutro2    (501) staff       (20)     5040 2024-03-24 19:45:37.000000 basefunctions-0.3.7/readme.md
+-rw-r--r--   0 neutro2    (501) staff       (20)       38 2024-04-02 18:09:34.223556 basefunctions-0.3.7/setup.cfg
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.210922 basefunctions-0.3.7/src/
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.216618 basefunctions-0.3.7/src/basefunctions/
+-rw-r--r--   0 neutro2    (501) staff       (20)     2502 2024-03-28 15:03:07.000000 basefunctions-0.3.7/src/basefunctions/__init__.py
+-rw-r--r--   0 neutro2    (501) staff       (20)     5349 2024-04-02 17:30:05.000000 basefunctions-0.3.7/src/basefunctions/database.py
+-rw-r--r--   0 neutro2    (501) staff       (20)    14876 2024-03-22 21:23:12.000000 basefunctions-0.3.7/src/basefunctions/filefunctions.py
+-rw-r--r--   0 neutro2    (501) staff       (20)    17600 2024-03-29 20:35:19.000000 basefunctions-0.3.7/src/basefunctions/threadpool.py
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.221340 basefunctions-0.3.7/src/basefunctions.egg-info/
+-rw-r--r--   0 neutro2    (501) staff       (20)     7051 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/PKG-INFO
+-rw-r--r--   0 neutro2    (501) staff       (20)      409 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)        1 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       97 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/requires.txt
+-rw-r--r--   0 neutro2    (501) staff       (20)       14 2024-04-02 18:09:34.000000 basefunctions-0.3.7/src/basefunctions.egg-info/top_level.txt
+drwxr-xr-x   0 neutro2    (501) staff       (20)        0 2024-04-02 18:09:34.219979 basefunctions-0.3.7/tests/
+-rw-r--r--   0 neutro2    (501) staff       (20)    23668 2024-03-22 21:23:12.000000 basefunctions-0.3.7/tests/test_filefunctions.py
```

### Comparing `basefunctions-0.3.5.1/PKG-INFO` & `basefunctions-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basefunctions
-Version: 0.3.5.1
+Version: 0.3.7
 Summary: simple library to have some commonly used functions for everyday purpose
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `basefunctions-0.3.5.1/license` & `basefunctions-0.3.7/license`

 * *Files identical despite different names*

### Comparing `basefunctions-0.3.5.1/pyproject.toml` & `basefunctions-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "basefunctions"
-version = "0.3.5.1"
+version = "0.3.7"
 
 authors = [{ name = "NeuralDevelopment", email = "neutro2@outlook.de" }]
 description = "simple library to have some commonly used functions for everyday purpose"
 
 readme = "readme.md"
 license = { file = "license" }
 requires-python = ">=3.9"
```

### Comparing `basefunctions-0.3.5.1/readme.md` & `basefunctions-0.3.7/readme.md`

 * *Files identical despite different names*

### Comparing `basefunctions-0.3.5.1/src/basefunctions/__init__.py` & `basefunctions-0.3.7/src/basefunctions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 # -------------------------------------------------------------
 # IMPORTS
 # -------------------------------------------------------------
 from basefunctions.database import (
     check_if_table_exists,
     connect_to_database,
+    create_database,
     execute_sql_command,
     get_number_of_elements_in_table,
 )
 from basefunctions.filefunctions import (
     check_if_dir_exists,
     check_if_exists,
     check_if_file_exists,
@@ -60,14 +61,15 @@
     "ThreadPoolMessage",
     "ThreadPoolUserObject",
     "check_if_dir_exists",
     "check_if_exists",
     "check_if_file_exists",
     "check_if_table_exists",
     "connect_to_database",
+    "create_database",
     "create_directory",
     "create_file_list",
     "create_threadpool_message",
     "execute_sql_command",
     "get_base_name",
     "get_base_name_prefix",
     "get_current_directory",
```

### Comparing `basefunctions-0.3.5.1/src/basefunctions/database.py` & `basefunctions-0.3.7/src/basefunctions/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,55 +16,89 @@
 # =============================================================================
 """
 
 # -------------------------------------------------------------
 # IMPORTS
 # -------------------------------------------------------------
 import decouple
+import psycopg2
 import sqlalchemy
 
 # -------------------------------------------------------------
+#  FUNCTION DEFINITIONS
+# -------------------------------------------------------------
+
+# -------------------------------------------------------------
 # DEFINITIONS REGISTRY
 # -------------------------------------------------------------
 
 # -------------------------------------------------------------
 # DEFINITIONS
 # -------------------------------------------------------------
 
 # -------------------------------------------------------------
 # VARIABLE DEFINTIONS
 # -------------------------------------------------------------
 
 
-# -------------------------------------------------------------
-#  FUNCTION DEFINITIONS
-# -------------------------------------------------------------
+def create_database(prefix: str = "BASEFUNCTIONS") -> None:
+    """
+    create a postgresql database if it does not exist.
+
+    Returns
+    -------
+    None
+
+    """
+    # read the variables from the .env file
+
+    host_name = decouple.config(f"{prefix}_HOST", default="localhost", cast=str)
+    database_name = decouple.config(f"{prefix}_DB", default=None, cast=str)
+    user_name = decouple.config(f"{prefix}_USER", default="postgres", cast=str)
+    password = decouple.config(f"{prefix}_PASSWORD", default=None, cast=str)
+    port = decouple.config(f"{prefix}_PORT", default=5432, cast=int)
+
+    connection = psycopg2.connect(
+        host=host_name, database="postgres", user=user_name, password=password, port=port
+    )
+    connection.autocommit = True
+    cursor = connection.cursor()
+    cursor.execute(f"SELECT 1 FROM pg_catalog.pg_database WHERE datname = '{database_name}'")
+    if not cursor.fetchone():
+        cursor.execute(f"CREATE DATABASE {database_name}")
+    cursor.close()
+    connection.close()
 
 
 # -------------------------------------------------------------
 #  create an engine object for connecting to the database
 # -------------------------------------------------------------
-def connect_to_database(prefix: str) -> sqlalchemy.engine.base.Engine:
+def connect_to_database(prefix: str = "BASEFUNCTIONS") -> sqlalchemy.engine.base.Engine:
     """
     connect to the database and return the connection object
 
+    Parameters
+    ----------
+    prefix : str
+        prefix for the environment variables
+
     Returns
     -------
     sqlalchemy.engine.Engine
         connection object
     """
 
     sqlalchemy_protocol = decouple.config(
         f"{prefix}_PROTOCOL",
         default="postgresql+psycopg2",
         cast=str,
     )
-    host_name = decouple.config(f"{prefix}_HOSTNAME", default="localhost", cast=str)
-    database_name = decouple.config(f"{prefix}_DATABASE", default=None, cast=str)
-    user_name = decouple.config(f"{prefix}_USERNAME", default="postgres", cast=str)
+    host_name = decouple.config(f"{prefix}_HOST", default="localhost", cast=str)
+    database_name = decouple.config(f"{prefix}_DB", default=None, cast=str)
+    user_name = decouple.config(f"{prefix}_USER", default="postgres", cast=str)
     password = decouple.config(f"{prefix}_PASSWORD", default=None, cast=str)
     port = decouple.config(f"{prefix}_PORT", default=5432, cast=int)
 
     engine = sqlalchemy.create_engine(
         f"{sqlalchemy_protocol}://{user_name}:{password}" f"@{host_name}:{port}/{database_name}"
     )
     return engine
```

### Comparing `basefunctions-0.3.5.1/src/basefunctions/filefunctions.py` & `basefunctions-0.3.7/src/basefunctions/filefunctions.py`

 * *Files identical despite different names*

### Comparing `basefunctions-0.3.5.1/src/basefunctions/threadpool.py` & `basefunctions-0.3.7/src/basefunctions/threadpool.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 import queue
 import threading
 import types
 from dataclasses import dataclass
 from typing import Any, Callable, List
 
 import decouple
+import numpy as np
+import pandas as pd
 
 # -------------------------------------------------------------
 # DEFINITIONS REGISTRY
 # -------------------------------------------------------------
 
 # -------------------------------------------------------------
 # DEFINITIONS
@@ -363,27 +365,78 @@
             The output queue of the thread pool.
         """
         return self.output_queue
 
     # -------------------------------------------------------------
     # GET DATAFRAMES FROM OUTPUT QUEUE AND JOIN THEM INTO DICTIONARY
     # -------------------------------------------------------------
-    def get_dataframes_from_output_queue(self) -> dict:
+    def get_dataframes_from_output_queue(
+        self, dict_result: bool = True, inner_dates: bool = False
+    ) -> pd.DataFrame | dict:
         """
         Receive a list of DataFrames from the EOD2PD message handler.
 
+        Parameters
+        ----------
+        dict_result : bool
+            If True, the result will be a dictionary with the message type as key.
+            If False, the result will be a list of DataFrames.
+        inner_dates : bool
+            If False, the DataFrames will be filled with None for missing dates.
+            If True, the DataFrames will be aligned to the newest date.
+
         Returns
         -------
-        list
-            A list of DataFrames from the EOD2PD message handler.
+        dict or DataFrame
+            A dictionary of DataFrames if dict_result is True or if there are multiple DataFrames.
+            Otherwise, returns a single DataFrame.
         """
-        # get the list of dataframes
+        # TODO: inner_dates in jedem Fall berücksichtigen
+
         result = {}
         while not self.get_output_queue().empty():
-            result = result | self.get_output_queue().get()
+            result.update(self.get_output_queue().get())
+        if dict_result:
+            return result
+        else:
+            if len(result) > 1:
+                return self.create_multiindex_dataframe(result=result, inner_dates=inner_dates)
+            else:
+                return result[list(result.keys())[0]]
+
+    def create_multiindex_dataframe(self, result: dict, inner_dates=False) -> pd.DataFrame:
+        """
+        Create a multi-index DataFrame from a dictionary of DataFrames.
+
+        Parameters:
+        -----------
+        result : dict
+            A dictionary of DataFrames.
+        inner_dates : bool
+            If False, the DataFrames will be filled with None for missing dates.
+            If True, the DataFrames will be aligned to the newest date.
+
+        Returns:
+        --------
+        pd.DataFrame
+            A multi-index DataFrame containing the DataFrames from the dictionary.
+        """
+        # align all DataFrames to start and end with the date range
+        keys = sorted(result.keys())
+        values = [result[key] for key in keys]
+
+        # Concatenate aligned DataFrames with MultiIndex columns
+        result = pd.concat(
+            values,
+            axis=1,
+            join="inner" if inner_dates else "outer",
+            sort=True,
+            keys=[key.upper() for key in keys],
+        )
+
         return result
 
 
 class TimerThread:
     """
     A class representing a timer thread that raises a RuntimeError in the
     thread with the specified thread_id to terminate it after a specified
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `basefunctions-0.3.5.1/src/basefunctions.egg-info/PKG-INFO` & `basefunctions-0.3.7/src/basefunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basefunctions
-Version: 0.3.5.1
+Version: 0.3.7
 Summary: simple library to have some commonly used functions for everyday purpose
 Author-email: NeuralDevelopment <neutro2@outlook.de>
 License: MIT License
         
         Copyright (c) 2023 NeuralDevelopment
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `basefunctions-0.3.5.1/tests/test_filefunctions.py` & `basefunctions-0.3.7/tests/test_filefunctions.py`

 * *Files identical despite different names*

