# Comparing `tmp/shipyard_postgresql-0.2.0a3.tar.gz` & `tmp/shipyard_postgresql-0.2.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_postgresql-0.2.0a3.tar", max compression
+gzip compressed data, was "shipyard_postgresql-0.2.0a4.tar", max compression
```

## Comparing `shipyard_postgresql-0.2.0a3.tar` & `shipyard_postgresql-0.2.0a4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-07-20 19:30:44.104122 shipyard_postgresql-0.2.0a3/README.md
--rw-r--r--   0        0        0      687 2024-03-25 19:17:48.174776 shipyard_postgresql-0.2.0a3/pyproject.toml
--rw-r--r--   0        0        0       37 2024-03-25 18:11:40.032340 shipyard_postgresql-0.2.0a3/shipyard_postgresql/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:26:38.968910 shipyard_postgresql-0.2.0a3/shipyard_postgresql/cli/__init__.py
--rw-r--r--   0        0        0      621 2024-03-25 18:11:40.033375 shipyard_postgresql-0.2.0a3/shipyard_postgresql/cli/authtest.py
--rw-r--r--   0        0        0     2074 2024-03-25 18:15:25.490264 shipyard_postgresql-0.2.0a3/shipyard_postgresql/cli/execute_sql.py
--rw-r--r--   0        0        0     2976 2024-03-25 18:14:59.400343 shipyard_postgresql-0.2.0a3/shipyard_postgresql/cli/store_query_results.py
--rw-r--r--   0        0        0     4584 2024-03-25 18:15:31.511996 shipyard_postgresql-0.2.0a3/shipyard_postgresql/cli/upload_file.py
--rw-r--r--   0        0        0     7527 2024-03-25 18:11:40.036808 shipyard_postgresql-0.2.0a3/shipyard_postgresql/postgres.py
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 shipyard_postgresql-0.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-20 19:30:44.104122 shipyard_postgresql-0.2.0a4/README.md
+-rw-r--r--   0        0        0      687 2024-03-25 20:01:32.767012 shipyard_postgresql-0.2.0a4/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-03-25 19:26:33.119590 shipyard_postgresql-0.2.0a4/shipyard_postgresql/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:26:38.968910 shipyard_postgresql-0.2.0a4/shipyard_postgresql/cli/__init__.py
+-rw-r--r--   0        0        0      621 2024-03-25 19:26:33.120317 shipyard_postgresql-0.2.0a4/shipyard_postgresql/cli/authtest.py
+-rw-r--r--   0        0        0     2175 2024-03-25 19:58:35.441046 shipyard_postgresql-0.2.0a4/shipyard_postgresql/cli/execute_sql.py
+-rw-r--r--   0        0        0     3100 2024-03-25 20:01:53.049327 shipyard_postgresql-0.2.0a4/shipyard_postgresql/cli/store_query_results.py
+-rw-r--r--   0        0        0     4717 2024-03-25 20:01:12.661093 shipyard_postgresql-0.2.0a4/shipyard_postgresql/cli/upload_file.py
+-rw-r--r--   0        0        0     7527 2024-03-25 19:26:33.122426 shipyard_postgresql-0.2.0a4/shipyard_postgresql/postgres.py
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 shipyard_postgresql-0.2.0a4/PKG-INFO
```

### Comparing `shipyard_postgresql-0.2.0a3/pyproject.toml` & `shipyard_postgresql-0.2.0a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-postgresql"
-version = "0.2.0a3"
+version = "0.2.0a4"
 description = "A local client for connecting and working with Postgresql Databases"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_postgresql"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_postgresql-0.2.0a3/shipyard_postgresql/cli/authtest.py` & `shipyard_postgresql-0.2.0a4/shipyard_postgresql/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_postgresql-0.2.0a3/shipyard_postgresql/cli/execute_sql.py` & `shipyard_postgresql-0.2.0a4/shipyard_postgresql/cli/store_query_results.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,91 @@
-from sqlalchemy import text
 import argparse
+import os
 import sys
+import shipyard_bp_utils as shipyard
 from shipyard_postgresql import PostgresClient
-from shipyard_templates import ShipyardLogger, ExitCodeException, Database
+from shipyard_templates import ExitCodeException, ShipyardLogger, Database
+from sqlalchemy import text
 
 logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--username", dest="username", required=False)
     parser.add_argument("--password", dest="password", required=False)
     parser.add_argument("--host", dest="host", required=False)
     parser.add_argument("--database", dest="database", required=False)
     parser.add_argument("--port", dest="port", default="5432", required=False)
     parser.add_argument("--url-parameters", dest="url_parameters", required=False)
     parser.add_argument("--query", dest="query", required=True)
+    parser.add_argument(
+        "--destination-file-name",
+        dest="destination_file_name",
+        default="output.csv",
+        required=True,
+    )
+    parser.add_argument(
+        "--destination-folder-name",
+        dest="destination_folder_name",
+        default="",
+        required=False,
+    )
+    parser.add_argument(
+        "--file-header", dest="file_header", default="True", required=False
+    )
     args = parser.parse_args()
 
     if args.host and not (args.database or args.username):
         parser.error("--host requires --database and --username")
     if args.database and not (args.host or args.username):
         parser.error("--database requires --host and --username")
     if args.username and not (args.host or args.username):
         parser.error("--username requires --host and --username")
-
     return args
 
 
 def main():
-    args = get_args()
-    query = text(args.query)
-    client_args = {
-        "user": args.username,
-        "pwd": args.password,
-        "host": args.host,
-        "database": args.database,
-        "port": args.port,
-        "url_params": args.url_parameters if args.url_parameters != "" else None,
-    }
-    postgres = PostgresClient(**client_args)
+    postgres = None
     try:
-        postgres.execute_query(query)
-        logger.info("Successfully executed query")
+        args = get_args()
+        target_file = args.destination_file_name
+        target_dir = args.destination_folder_name
+        target_path = shipyard.files.combine_folder_and_file_name(
+            folder_name=target_dir, file_name=target_file
+        )
+        file_header = shipyard.args.convert_to_boolean(args.file_header)
+        query = text(args.query)
+
+        client_args = {
+            "user": args.username,
+            "pwd": args.password,
+            "host": args.host,
+            "database": args.database,
+            "port": args.port,
+            "url_params": args.url_parameters if args.url_parameters != "" else None,
+        }
+        postgres = PostgresClient(**client_args)
+        if target_dir:
+            shipyard.files.create_folder_if_dne(target_dir)
+
+        postgres.read_chunks(query=query, dest_path=target_path, header=file_header)
+
+        logger.info(f"Successfully downloaded query results to {target_path}")
 
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
 
     except Exception as e:
         logger.error(
-            f"An unexpected error occurred when attempting to execute query in Postgres. Message from the server reads: {e}"
+            f"An unexpected error occurred when trying to fetch data from Postgres. Message from the server reads: {e}"
         )
         sys.exit(Database.EXIT_CODE_UNKNOWN)
 
     finally:
-        postgres.close()
+        if postgres is not None:
+            postgres.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_postgresql-0.2.0a3/shipyard_postgresql/cli/store_query_results.py` & `shipyard_postgresql-0.2.0a4/shipyard_postgresql/cli/execute_sql.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,64 @@
+from sqlalchemy import text
 import argparse
-import os
 import sys
-import shipyard_bp_utils as shipyard
 from shipyard_postgresql import PostgresClient
-from shipyard_templates import ExitCodeException, ShipyardLogger, Database
-from sqlalchemy import text
+from shipyard_templates import ShipyardLogger, ExitCodeException, Database
 
 logger = ShipyardLogger.get_logger()
 
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("--username", dest="username", required=False)
     parser.add_argument("--password", dest="password", required=False)
     parser.add_argument("--host", dest="host", required=False)
     parser.add_argument("--database", dest="database", required=False)
     parser.add_argument("--port", dest="port", default="5432", required=False)
     parser.add_argument("--url-parameters", dest="url_parameters", required=False)
     parser.add_argument("--query", dest="query", required=True)
-    parser.add_argument(
-        "--destination-file-name",
-        dest="destination_file_name",
-        default="output.csv",
-        required=True,
-    )
-    parser.add_argument(
-        "--destination-folder-name",
-        dest="destination_folder_name",
-        default="",
-        required=False,
-    )
-    parser.add_argument(
-        "--file-header", dest="file_header", default="True", required=False
-    )
     args = parser.parse_args()
 
     if args.host and not (args.database or args.username):
         parser.error("--host requires --database and --username")
     if args.database and not (args.host or args.username):
         parser.error("--database requires --host and --username")
     if args.username and not (args.host or args.username):
         parser.error("--username requires --host and --username")
+
     return args
 
 
 def main():
-    args = get_args()
-    target_file = args.destination_file_name
-    target_dir = args.destination_folder_name
-    target_path = shipyard.files.combine_folder_and_file_name(
-        folder_name=target_dir, file_name=target_file
-    )
-    file_header = shipyard.args.convert_to_boolean(args.file_header)
-    query = text(args.query)
-
-    client_args = {
-        "user": args.username,
-        "pwd": args.password,
-        "host": args.host,
-        "database": args.database,
-        "port": args.port,
-        "url_params": args.url_parameters if args.url_parameters != "" else None,
-    }
-    postgres = PostgresClient(**client_args)
-
+    postgres = None
     try:
-        if target_dir:
-            shipyard.files.create_folder_if_dne(target_dir)
-
-        postgres.read_chunks(query=query, dest_path=target_path, header=file_header)
-
-        logger.info(f"Successfully downloaded query results to {target_path}")
+        args = get_args()
+        query = text(args.query)
+        client_args = {
+            "user": args.username,
+            "pwd": args.password,
+            "host": args.host,
+            "database": args.database,
+            "port": args.port,
+            "url_params": args.url_parameters if args.url_parameters != "" else None,
+        }
+        postgres = PostgresClient(**client_args)
+        postgres.execute_query(query)
+        logger.info("Successfully executed query")
 
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
 
     except Exception as e:
         logger.error(
-            f"An unexpected error occurred when trying to fetch data from Postgres. Message from the server reads: {e}"
+            f"An unexpected error occurred when attempting to execute query in Postgres. Message from the server reads: {e}"
         )
         sys.exit(Database.EXIT_CODE_UNKNOWN)
 
     finally:
-        postgres.close()
+        if postgres is not None:
+            postgres.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_postgresql-0.2.0a3/shipyard_postgresql/cli/upload_file.py` & `shipyard_postgresql-0.2.0a4/shipyard_postgresql/cli/upload_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,35 +54,36 @@
         parser.error("--database requires --host and --username")
     if args.username and not (args.host or args.username):
         parser.error("--username requires --host and --username")
     return args
 
 
 def main():
-    args = get_args()
-    match_type = args.source_file_name_match_type
-    src_file = args.source_file_name
-    src_dir = args.source_folder_name
-    src_path = shipyard.files.combine_folder_and_file_name(
-        folder_name=src_dir, file_name=src_file
-    )
-    table_name = args.table_name
-    insert_method = args.insert_method
-
-    client_args = {
-        "user": args.username,
-        "pwd": args.password,
-        "host": args.host,
-        "database": args.database,
-        "port": args.port,
-        "schema": args.schema if args.schema != "" else None,
-        "url_params": args.url_parameters if args.url_parameters != "" else None,
-    }
-    postgres = PostgresClient(**client_args)
+    postgres = None
     try:
+        args = get_args()
+        match_type = args.source_file_name_match_type
+        src_file = args.source_file_name
+        src_dir = args.source_folder_name
+        src_path = shipyard.files.combine_folder_and_file_name(
+            folder_name=src_dir, file_name=src_file
+        )
+        table_name = args.table_name
+        insert_method = args.insert_method
+
+        client_args = {
+            "user": args.username,
+            "pwd": args.password,
+            "host": args.host,
+            "database": args.database,
+            "port": args.port,
+            "schema": args.schema if args.schema != "" else None,
+            "url_params": args.url_parameters if args.url_parameters != "" else None,
+        }
+        postgres = PostgresClient(**client_args)
         if match_type == "regex_match":
             file_names = shipyard.files.find_all_local_file_names(src_dir)
             matching_file_names = shipyard.files.find_all_file_matches(
                 file_names, re.compile(src_file)
             )
             if (n_matches := len(matching_file_names)) == 0:
                 logger.error("No files matching files found for the supplied regex")
@@ -121,12 +122,13 @@
     except Exception as e:
         logger.error(
             f"An unexpected error occurred when trying to load data to Postgres. Message from the server reads: {e}"
         )
         sys.exit(Database.EXIT_CODE_UNKNOWN)
 
     finally:
-        postgres.close()
+        if postgres is not None:
+            postgres.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_postgresql-0.2.0a3/shipyard_postgresql/postgres.py` & `shipyard_postgresql-0.2.0a4/shipyard_postgresql/postgres.py`

 * *Files identical despite different names*

### Comparing `shipyard_postgresql-0.2.0a3/PKG-INFO` & `shipyard_postgresql-0.2.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-postgresql
-Version: 0.2.0a3
+Version: 0.2.0a4
 Summary: A local client for connecting and working with Postgresql Databases
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

