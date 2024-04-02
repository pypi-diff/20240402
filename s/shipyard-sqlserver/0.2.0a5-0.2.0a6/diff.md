# Comparing `tmp/shipyard_sqlserver-0.2.0a5.tar.gz` & `tmp/shipyard_sqlserver-0.2.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_sqlserver-0.2.0a5.tar", max compression
+gzip compressed data, was "shipyard_sqlserver-0.2.0a6.tar", max compression
```

## Comparing `shipyard_sqlserver-0.2.0a5.tar` & `shipyard_sqlserver-0.2.0a6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-08-14 16:50:02.446349 shipyard_sqlserver-0.2.0a5/README.md
--rw-r--r--   0        0        0      681 2024-03-21 21:42:34.948180 shipyard_sqlserver-0.2.0a5/pyproject.toml
--rw-r--r--   0        0        0       39 2023-08-14 16:50:02.447093 shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:26:39.005282 shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/cli/__init__.py
--rw-r--r--   0        0        0      985 2024-03-08 21:36:38.948885 shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/cli/authtest.py
--rw-r--r--   0        0        0     2018 2024-03-21 19:58:58.540433 shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/cli/execute_sql.py
--rw-r--r--   0        0        0     2950 2024-03-21 19:58:58.540877 shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/cli/store_query_results.py
--rw-r--r--   0        0        0     4131 2024-03-21 21:38:51.875504 shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/cli/upload_file.py
--rw-r--r--   0        0        0      342 2024-03-21 21:29:51.046227 shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/exceptions.py
--rw-r--r--   0        0        0     4652 2024-03-21 21:40:55.865334 shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/sqlserver.py
--rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 shipyard_sqlserver-0.2.0a5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-14 16:50:02.446349 shipyard_sqlserver-0.2.0a6/README.md
+-rw-r--r--   0        0        0      681 2024-03-25 20:44:34.238427 shipyard_sqlserver-0.2.0a6/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-08-14 16:50:02.447093 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:26:39.005282 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/__init__.py
+-rw-r--r--   0        0        0      770 2024-03-25 20:45:07.917157 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/authtest.py
+-rw-r--r--   0        0        0     2059 2024-03-25 20:27:00.253292 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/execute_sql.py
+-rw-r--r--   0        0        0     2991 2024-03-25 20:27:16.630788 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/store_query_results.py
+-rw-r--r--   0        0        0     4149 2024-03-25 20:26:29.621579 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/upload_file.py
+-rw-r--r--   0        0        0      342 2024-03-25 20:25:45.260252 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/exceptions.py
+-rw-r--r--   0        0        0     4652 2024-03-25 20:26:13.511943 shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/sqlserver.py
+-rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 shipyard_sqlserver-0.2.0a6/PKG-INFO
```

### Comparing `shipyard_sqlserver-0.2.0a5/pyproject.toml` & `shipyard_sqlserver-0.2.0a6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-sqlserver"
-version = "0.2.0a5"
+version = "0.2.0a6"
 description = "A local client for connecting and working with Sql Server Databases"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_sqlserver"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/cli/execute_sql.py` & `shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/execute_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         parser.error("--database requires --host and --username")
     if args.username and not (args.host or args.username):
         parser.error("--username requires --host and --username")
     return args
 
 
 def main():
+    client = None
     try:
         args = get_args()
         query = text(args.query)
         client = SqlServerClient(
             user=args.username,
             pwd=args.password,
             host=args.host,
@@ -49,12 +50,13 @@
     except Exception as e:
         logger.error(
             f"An unexpected error occurred when attempting to fetch data from SQL Server. Message from the server reads: {e}"
         )
         sys.exit(Database.EXIT_CODE_UNKNOWN)
 
     finally:
-        client.close()
+        if client:
+            client.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/cli/store_query_results.py` & `shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/store_query_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         parser.error("--database requires --host and --username")
     if args.username and not (args.host or args.username):
         parser.error("--username requires --host and --username")
     return args
 
 
 def main():
+    client = None
     try:
         args = get_args()
         dest_file = args.destination_file_name
         dest_dir = args.destination_folder_name
         if dest_dir:
             shipyard.files.create_folder_if_dne(dest_dir)
         dest_path = shipyard.files.combine_folder_and_file_name(
@@ -77,12 +78,13 @@
     except Exception as e:
         logger.error(
             f"An unexpected error occurred when attempting to fetch data from SQL Server. Message from the server reads: {e}"
         )
         sys.exit(Database.EXIT_CODE_UNKNOWN)
 
     finally:
-        client.close()
+        if client:
+            client.close()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/cli/upload_file.py` & `shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/cli/upload_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         parser.error("--database requires --host and --username")
     if args.username and not (args.host or args.username):
         parser.error("--username requires --host and --username")
     return args
 
 
 def main():
+    client = None
     try:
         args = get_args()
         match_type = args.source_file_name_match_type
         file_name = args.source_file_name
         dir_name = args.source_folder_name
         file_path = shipyard.files.combine_folder_and_file_name(
             folder_name=dir_name, file_name=file_name
```

### Comparing `shipyard_sqlserver-0.2.0a5/shipyard_sqlserver/sqlserver.py` & `shipyard_sqlserver-0.2.0a6/shipyard_sqlserver/sqlserver.py`

 * *Files identical despite different names*

### Comparing `shipyard_sqlserver-0.2.0a5/PKG-INFO` & `shipyard_sqlserver-0.2.0a6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-sqlserver
-Version: 0.2.0a5
+Version: 0.2.0a6
 Summary: A local client for connecting and working with Sql Server Databases
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

