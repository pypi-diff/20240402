# Comparing `tmp/tableconv-1.9947.20231219.tar.gz` & `tmp/tableconv-1.9957.20240331.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableconv-1.9947.20231219.tar", last modified: Tue Dec 19 20:09:14 2023, max compression
+gzip compressed data, was "tableconv-1.9957.20240331.tar", last modified: Tue Apr  2 20:43:56 2024, max compression
```

## Comparing `tableconv-1.9947.20231219.tar` & `tableconv-1.9957.20240331.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-19 20:09:14.748314 tableconv-1.9947.20231219/
--rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9947.20231219/LICENSE
--rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9947.20231219/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-12-19 20:09:14.748314 tableconv-1.9947.20231219/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)     9258 2023-03-26 03:16:21.000000 tableconv-1.9947.20231219/README.md
--rw-rw-r--   0 john      (1000) john      (1000)       38 2023-12-19 20:09:14.748314 tableconv-1.9947.20231219/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9947.20231219/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-19 20:09:14.748314 tableconv-1.9947.20231219/tableconv/
--rw-rw-r--   0 john      (1000) john      (1000)      400 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)       73 2023-12-19 20:05:00.000000 tableconv-1.9947.20231219/tableconv/__version__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-19 20:09:14.748314 tableconv-1.9947.20231219/tableconv/adapters/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9947.20231219/tableconv/adapters/__init__.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-19 20:09:14.748314 tableconv-1.9947.20231219/tableconv/adapters/df/
--rw-rw-r--   0 john      (1000) john      (1000)      968 2023-12-19 19:55:07.000000 tableconv-1.9947.20231219/tableconv/adapters/df/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     4264 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/ascii.py
--rw-rw-r--   0 john      (1000) john      (1000)    14948 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/aws_athena.py
--rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/aws_dynamodb.py
--rw-r--r--   0 john      (1000) john      (1000)     2394 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/aws_logs.py
--rw-rw-r--   0 john      (1000) john      (1000)     1696 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/base.py
--rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9947.20231219/tableconv/adapters/df/example.py
--rw-rw-r--   0 john      (1000) john      (1000)     2526 2023-05-30 16:53:38.000000 tableconv-1.9947.20231219/tableconv/adapters/df/file_adapter_mixin.py
--rw-rw-r--   0 john      (1000) john      (1000)    13316 2023-08-07 22:28:07.000000 tableconv-1.9947.20231219/tableconv/adapters/df/gsheets.py
--rw-rw-r--   0 john      (1000) john      (1000)      339 2023-06-26 23:24:34.000000 tableconv-1.9947.20231219/tableconv/adapters/df/jira.py
--rw-rw-r--   0 john      (1000) john      (1000)     6463 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/json.py
--rw-r--r--   0 john      (1000) john      (1000)      500 2023-12-19 20:03:03.000000 tableconv-1.9947.20231219/tableconv/adapters/df/leveldb.py
--rw-rw-r--   0 john      (1000) john      (1000)     1876 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/nested_list.py
--rw-r--r--   0 john      (1000) john      (1000)     1509 2023-03-26 03:15:45.000000 tableconv-1.9947.20231219/tableconv/adapters/df/numbers.py
--rw-rw-r--   0 john      (1000) john      (1000)     8885 2023-06-30 22:42:07.000000 tableconv-1.9947.20231219/tableconv/adapters/df/pandas_io.py
--rw-rw-r--   0 john      (1000) john      (1000)     1642 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/python.py
--rw-rw-r--   0 john      (1000) john      (1000)     5805 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/rdbms.py
--rw-rw-r--   0 john      (1000) john      (1000)     2494 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/smart_sheet.py
--rw-r--r--   0 john      (1000) john      (1000)      866 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/sql_literal.py
--rw-rw-r--   0 john      (1000) john      (1000)     7714 2023-12-08 08:19:48.000000 tableconv-1.9947.20231219/tableconv/adapters/df/sumo_logic.py
--rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/text_array.py
--rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/adapters/df/yaml.py
--rw-rw-r--   0 john      (1000) john      (1000)    15651 2023-08-08 00:15:59.000000 tableconv-1.9947.20231219/tableconv/core.py
--rw-r--r--   0 john      (1000) john      (1000)     2301 2023-07-29 01:57:22.000000 tableconv-1.9947.20231219/tableconv/exceptions.py
--rw-rw-r--   0 john      (1000) john      (1000)     3469 2023-08-12 01:36:35.000000 tableconv-1.9947.20231219/tableconv/in_memory_query.py
--rw-rw-r--   0 john      (1000) john      (1000)     5836 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/interactive.py
--rw-rw-r--   0 john      (1000) john      (1000)    11215 2023-06-30 23:07:40.000000 tableconv-1.9947.20231219/tableconv/main.py
--rw-rw-r--   0 john      (1000) john      (1000)      726 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/parse_time.py
--rw-rw-r--   0 john      (1000) john      (1000)     1469 2023-01-22 04:03:54.000000 tableconv-1.9947.20231219/tableconv/uri.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-19 20:09:14.748314 tableconv-1.9947.20231219/tableconv.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     9724 2023-12-19 20:09:14.000000 tableconv-1.9947.20231219/tableconv.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     1275 2023-12-19 20:09:14.000000 tableconv-1.9947.20231219/tableconv.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-12-19 20:09:14.000000 tableconv-1.9947.20231219/tableconv.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       66 2023-12-19 20:09:14.000000 tableconv-1.9947.20231219/tableconv.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      243 2023-12-19 20:09:14.000000 tableconv-1.9947.20231219/tableconv.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       27 2023-12-19 20:09:14.000000 tableconv-1.9947.20231219/tableconv.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-12-19 20:09:14.748314 tableconv-1.9947.20231219/tableconv_daemon/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9947.20231219/tableconv_daemon/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9947.20231219/tableconv_daemon/main.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/
+-rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-09-03 04:22:14.000000 tableconv-1.9957.20240331/LICENSE
+-rw-rw-r--   0 john      (1000) john      (1000)       26 2021-09-03 04:22:14.000000 tableconv-1.9957.20240331/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     9922 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)     9456 2024-03-31 06:03:00.000000 tableconv-1.9957.20240331/README.md
+-rw-rw-r--   0 john      (1000) john      (1000)       38 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     2232 2023-01-22 04:21:13.000000 tableconv-1.9957.20240331/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.568556 tableconv-1.9957.20240331/tableconv/
+-rw-rw-r--   0 john      (1000) john      (1000)      400 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)       73 2024-03-31 06:34:11.000000 tableconv-1.9957.20240331/tableconv/__version__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.568556 tableconv-1.9957.20240331/tableconv/adapters/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2021-09-03 04:22:14.000000 tableconv-1.9957.20240331/tableconv/adapters/__init__.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/tableconv/adapters/df/
+-rw-rw-r--   0 john      (1000) john      (1000)     1047 2024-03-31 04:52:25.000000 tableconv-1.9957.20240331/tableconv/adapters/df/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4264 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/ascii.py
+-rw-rw-r--   0 john      (1000) john      (1000)    14948 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/aws_athena.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1081 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/aws_dynamodb.py
+-rw-r--r--   0 john      (1000) john      (1000)     2394 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/aws_logs.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1756 2024-01-19 23:13:24.000000 tableconv-1.9957.20240331/tableconv/adapters/df/base.py
+-rw-rw-r--   0 john      (1000) john      (1000)      403 2022-01-02 03:01:01.000000 tableconv-1.9957.20240331/tableconv/adapters/df/example.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2526 2023-05-30 16:53:38.000000 tableconv-1.9957.20240331/tableconv/adapters/df/file_adapter_mixin.py
+-rw-rw-r--   0 john      (1000) john      (1000)    13407 2024-03-31 06:02:50.000000 tableconv-1.9957.20240331/tableconv/adapters/df/gsheets.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1925 2024-03-31 06:02:50.000000 tableconv-1.9957.20240331/tableconv/adapters/df/jc.py
+-rw-rw-r--   0 john      (1000) john      (1000)      339 2023-06-26 23:24:34.000000 tableconv-1.9957.20240331/tableconv/adapters/df/jira.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6463 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/json.py
+-rw-rw-r--   0 john      (1000) john      (1000)      589 2024-03-31 06:31:52.000000 tableconv-1.9957.20240331/tableconv/adapters/df/leveldb.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1876 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/nested_list.py
+-rw-r--r--   0 john      (1000) john      (1000)     1509 2023-03-26 03:15:45.000000 tableconv-1.9957.20240331/tableconv/adapters/df/numbers.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1289 2024-03-31 06:31:52.000000 tableconv-1.9957.20240331/tableconv/adapters/df/osquery.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9186 2024-03-31 05:55:31.000000 tableconv-1.9957.20240331/tableconv/adapters/df/pandas_io.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1642 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/python.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5805 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/rdbms.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2494 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/smart_sheet.py
+-rw-r--r--   0 john      (1000) john      (1000)      881 2024-03-31 05:43:04.000000 tableconv-1.9957.20240331/tableconv/adapters/df/sql_literal.py
+-rw-rw-r--   0 john      (1000) john      (1000)     7714 2024-03-31 06:02:50.000000 tableconv-1.9957.20240331/tableconv/adapters/df/sumo_logic.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2999 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/text_array.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1644 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/adapters/df/yaml.py
+-rw-rw-r--   0 john      (1000) john      (1000)    17462 2024-03-31 06:07:39.000000 tableconv-1.9957.20240331/tableconv/core.py
+-rw-r--r--   0 john      (1000) john      (1000)     2301 2023-07-29 01:57:22.000000 tableconv-1.9957.20240331/tableconv/exceptions.py
+-rw-rw-r--   0 john      (1000) john      (1000)     3542 2024-03-31 06:33:22.000000 tableconv-1.9957.20240331/tableconv/in_memory_query.py
+-rw-rw-r--   0 john      (1000) john      (1000)     5884 2024-01-19 23:11:36.000000 tableconv-1.9957.20240331/tableconv/interactive.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11527 2024-03-31 05:59:27.000000 tableconv-1.9957.20240331/tableconv/main.py
+-rw-rw-r--   0 john      (1000) john      (1000)      726 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/parse_time.py
+-rw-rw-r--   0 john      (1000) john      (1000)     1469 2023-01-22 04:03:54.000000 tableconv-1.9957.20240331/tableconv/uri.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.568556 tableconv-1.9957.20240331/tableconv.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     9922 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     1336 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       66 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      243 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       27 2024-04-02 20:43:56.000000 tableconv-1.9957.20240331/tableconv.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2024-04-02 20:43:56.572557 tableconv-1.9957.20240331/tableconv_daemon/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-01-15 04:13:45.000000 tableconv-1.9957.20240331/tableconv_daemon/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     9537 2023-03-26 02:56:00.000000 tableconv-1.9957.20240331/tableconv_daemon/main.py
```

### Comparing `tableconv-1.9947.20231219/LICENSE` & `tableconv-1.9957.20240331/LICENSE`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/PKG-INFO` & `tableconv-1.9957.20240331/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9947.20231219
+Version: 1.9957.20240331
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -121,25 +121,26 @@
   -h, --help            show this help message and exit
   -q SOURCE_QUERY, -Q SOURCE_QUERY, --query SOURCE_QUERY
                         Query to run on the source. Even for non-SQL datasources (e.g. csv or
                         json), SQL querying is still supported, try `SELECT * FROM data`.
   -F INTERMEDIATE_FILTER_SQL, --filter INTERMEDIATE_FILTER_SQL
                         Filter (i.e. transform) the input data using a SQL query operating on the
                         dataset in memory using DuckDB SQL.
-  -o DEST_URL, --dest DEST_URL, --out DEST_URL
+  -o DEST_URL, --dest DEST_URL, --out DEST_URL, --output DEST_URL
                         Specify the data destination URL. If this destination already exists, be
                         aware that the default behavior is to overwrite.
   -i, --interactive     Enter interactive REPL query mode.
   --open                Open resulting file/url in the operating system desktop environment. (not
                         supported for all destination types)
   --schema SCHEMA_COERCION, --coerce-schema SCHEMA_COERCION
                         Coerce source schema according to a schema definition. (WARNING:
                         experimental feature)
   --restrict-schema     Exclude all columns not included in the SCHEMA_COERCION definition.
                         (WARNING: experimental feature)
+  --autocache, --cache  Cache network data, and reuse cached data.
   -v, --verbose, --debug
                         Show debug details, including API calls and error sources.
   --version             Show version number and exit
   --quiet               Only display errors.
   --print, --print-dest
                         Print resulting URL/path to stdout, for chaining with other commands.
   --daemon              Tableconv startup time (python startup time) is slow. To mitigate that,
@@ -175,51 +176,55 @@
   example.jsonl 
   example.jsonlines 
   example.ldjson 
   example.ndjson 
   example.numbers (source only)
   example.orc (source only)
   example.parquet 
+  example.pickledf 
   example.py 
   example.python 
   example.tsv 
   example.xls 
   example.xlsx 
   example.yaml 
   example.yml 
   gsheets://:new: 
-  jiracloud://mycorpname (source only)
+  jc://ls -l (source only)
   jiraformat:- (dest only)
   jsonarray:- 
   latex:- (dest only)
+  leveldblog:output-0 (source only)
   list:- 
   markdown:- (dest only)
   md:- (dest only)
   mediawikiformat:- (dest only)
   moinmoinformat:- (dest only)
   mssql://127.0.0.1:5432/example_db 
   mysql://127.0.0.1:5432/example_db 
   nestedlist:- (source only)
   oracle://127.0.0.1:5432/example_db 
+  osquery://processes (source only)
   postgis://127.0.0.1:5432/example_db 
   postgres://127.0.0.1:5432/example_db 
   postgresql://127.0.0.1:5432/example_db 
   pylist:- 
   pythonlist:- 
   rst:- (dest only)
   smartsheet://SHEET_ID (source only)
+  sql_literal:- (dest only)
   sql_values:- (dest only)
   sqlite3:///tmp/example.db 
   sqlite:///tmp/example.db 
   sumologic://?from=2021-03-01T00:00:00Z&to=2021-05-03T00:00:00Z (source only)
   tex:- (dest only)
   yamlsequence:- 
 
 help & support:
-  https://github.com/personalcomputer/tableconv/issues
+  https://github.com/personalcomputer/tableconv/issues/new
 ```
 
 ## Python API
 
 ### Quickstart Example: Basic API usage: Replicating a typical CLI command using the API
 
 ```python
```

### Comparing `tableconv-1.9947.20231219/README.md` & `tableconv-1.9957.20240331/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -104,25 +104,26 @@
   -h, --help            show this help message and exit
   -q SOURCE_QUERY, -Q SOURCE_QUERY, --query SOURCE_QUERY
                         Query to run on the source. Even for non-SQL datasources (e.g. csv or
                         json), SQL querying is still supported, try `SELECT * FROM data`.
   -F INTERMEDIATE_FILTER_SQL, --filter INTERMEDIATE_FILTER_SQL
                         Filter (i.e. transform) the input data using a SQL query operating on the
                         dataset in memory using DuckDB SQL.
-  -o DEST_URL, --dest DEST_URL, --out DEST_URL
+  -o DEST_URL, --dest DEST_URL, --out DEST_URL, --output DEST_URL
                         Specify the data destination URL. If this destination already exists, be
                         aware that the default behavior is to overwrite.
   -i, --interactive     Enter interactive REPL query mode.
   --open                Open resulting file/url in the operating system desktop environment. (not
                         supported for all destination types)
   --schema SCHEMA_COERCION, --coerce-schema SCHEMA_COERCION
                         Coerce source schema according to a schema definition. (WARNING:
                         experimental feature)
   --restrict-schema     Exclude all columns not included in the SCHEMA_COERCION definition.
                         (WARNING: experimental feature)
+  --autocache, --cache  Cache network data, and reuse cached data.
   -v, --verbose, --debug
                         Show debug details, including API calls and error sources.
   --version             Show version number and exit
   --quiet               Only display errors.
   --print, --print-dest
                         Print resulting URL/path to stdout, for chaining with other commands.
   --daemon              Tableconv startup time (python startup time) is slow. To mitigate that,
@@ -158,51 +159,55 @@
   example.jsonl 
   example.jsonlines 
   example.ldjson 
   example.ndjson 
   example.numbers (source only)
   example.orc (source only)
   example.parquet 
+  example.pickledf 
   example.py 
   example.python 
   example.tsv 
   example.xls 
   example.xlsx 
   example.yaml 
   example.yml 
   gsheets://:new: 
-  jiracloud://mycorpname (source only)
+  jc://ls -l (source only)
   jiraformat:- (dest only)
   jsonarray:- 
   latex:- (dest only)
+  leveldblog:output-0 (source only)
   list:- 
   markdown:- (dest only)
   md:- (dest only)
   mediawikiformat:- (dest only)
   moinmoinformat:- (dest only)
   mssql://127.0.0.1:5432/example_db 
   mysql://127.0.0.1:5432/example_db 
   nestedlist:- (source only)
   oracle://127.0.0.1:5432/example_db 
+  osquery://processes (source only)
   postgis://127.0.0.1:5432/example_db 
   postgres://127.0.0.1:5432/example_db 
   postgresql://127.0.0.1:5432/example_db 
   pylist:- 
   pythonlist:- 
   rst:- (dest only)
   smartsheet://SHEET_ID (source only)
+  sql_literal:- (dest only)
   sql_values:- (dest only)
   sqlite3:///tmp/example.db 
   sqlite:///tmp/example.db 
   sumologic://?from=2021-03-01T00:00:00Z&to=2021-05-03T00:00:00Z (source only)
   tex:- (dest only)
   yamlsequence:- 
 
 help & support:
-  https://github.com/personalcomputer/tableconv/issues
+  https://github.com/personalcomputer/tableconv/issues/new
 ```
 
 ## Python API
 
 ### Quickstart Example: Basic API usage: Replicating a typical CLI command using the API
 
 ```python
```

### Comparing `tableconv-1.9947.20231219/setup.py` & `tableconv-1.9957.20240331/setup.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/__init__.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from tableconv.adapters.df.base import write_adapters, read_adapters, adapters  # noqa: F401
 from .ascii import *  # noqa: F401 F403
 from .aws_athena import *  # noqa: F401 F403
 from .aws_dynamodb import *  # noqa: F401 F403
 from .aws_logs import *  # noqa: F401 F403
 from .gsheets import *  # noqa: F401 F403
+from .jc import *  # noqa: F401 F403
 from .jira import *  # noqa: F401 F403
 from .json import *  # noqa: F401 F403
 from .leveldb import *  # noqa: F401 F403
 from .nested_list import *  # noqa: F401 F403
 from .numbers import *  # noqa: F401 F403
+from .osquery import *  # noqa: F401 F403
 from .pandas_io import *  # noqa: F401 F403
 from .python import *  # noqa: F401 F403
 from .rdbms import *  # noqa: F401 F403
 from .smart_sheet import *  # noqa: F401 F403
 from .sql_literal import *  # noqa: F401 F403
 from .sumo_logic import *  # noqa: F401 F403
 from .text_array import *  # noqa: F401 F403
```

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/ascii.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/ascii.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/aws_athena.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/aws_athena.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/aws_dynamodb.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/aws_dynamodb.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/aws_logs.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/aws_logs.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/base.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,17 +35,17 @@
         raise NotImplementedError
 
     @classmethod
     def dump(cls, df: pd.DataFrame, uri: str) -> Optional[str]:
         raise NotImplementedError
 
 
-adapters = {}
-read_adapters = {}
-write_adapters = {}
+adapters: dict[str, Adapter] = {}
+read_adapters: dict[str, Adapter] = {}
+write_adapters: dict[str, Adapter] = {}
 
 
 def register_adapter(schemes: List[str], write_only: bool = False, read_only: bool = False):
     """
     TODO: better decorator api proposal:
     @register_write_adapter(
         protocol='sql_values', aliases=[], parameters={}, example_url='', text_based=True, file_based=True)
```

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/file_adapter_mixin.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/file_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/gsheets.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/gsheets.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     def _get_oauth_credentials():
         from oauth2client import client, tools
         from oauth2client.file import Storage
 
         creds_path = os.path.expanduser("~/.tableconv-gsheets-credentials")
         if not os.path.exists(creds_path):
             raise URLInaccessibleError(
-                'gsheets integration requires configuring Google Sheets API authentication credentials. '
-                'Please run `tableconv configure gsheets --help` for help.'
+                "gsheets integration requires configuring Google Sheets API authentication credentials. "
+                "Please run `tableconv configure gsheets --help` for help."
             )
         store = Storage(creds_path)
         credentials = store.get()
         sys.argv = [""]
         if not credentials or credentials.invalid:
             SCOPES = [
                 "https://www.googleapis.com/auth/spreadsheets",
@@ -112,15 +112,15 @@
             .get(
                 spreadsheetId=spreadsheet_id,
                 range=f"'{sheet_name}'",
             )
             .execute()
         )
 
-        num_columns = max(*[len(r) for r in  raw_data["values"]])
+        num_columns = max(*[len(r) for r in raw_data["values"]])
         header = list_ljust(raw_data["values"][0], num_columns)
         values = [list_ljust(row, num_columns) for row in raw_data["values"][1:]]
         df = pd.DataFrame(values, columns=header)
         return cls._query_in_memory(df, query)
 
     @staticmethod
     def _create_spreadsheet(googlesheets, spreadsheet_name, first_sheet_name, columns, rows):
@@ -265,25 +265,29 @@
                     raise TableAlreadyExistsError(exc.reason) from exc
                 new_sheet = False
             if not new_sheet:
                 spreadsheet_data = googlesheets.spreadsheets().get(spreadsheetId=spreadsheet_id).execute()
                 sheet = get_sheet_properties(spreadsheet_data, sheet_name=sheet_name)
                 sheet_id = sheet["sheetId"]
                 if if_exists == "replace":
-                    GoogleSheetsAdapter._reshape_sheet(googlesheets, spreadsheet_id, sheet_id, columns=columns, rows=rows)
+                    GoogleSheetsAdapter._reshape_sheet(
+                        googlesheets, spreadsheet_id, sheet_id, columns=columns, rows=rows
+                    )
                     # delete it..
                     # raise NotImplementedError("Sheet if_exists=replace not implemented yet")
                 elif if_exists == "append":
                     reformat = False
                     existing_rows = sheet["gridProperties"]["rowCount"]
                     existing_columns = sheet["gridProperties"]["columnCount"]
                     if existing_columns != columns:
                         raise AppendSchemeConflictError(f"Cannot append to {sheet_name} - columns don't match")
                     total_rows = existing_rows + rows
-                    GoogleSheetsAdapter._reshape_sheet(googlesheets, spreadsheet_id, sheet_id, columns=columns, rows=total_rows)
+                    GoogleSheetsAdapter._reshape_sheet(
+                        googlesheets, spreadsheet_id, sheet_id, columns=columns, rows=total_rows
+                    )
                     start_row = existing_rows + 1
                 else:
                     raise AssertionError
 
         # Insert data
         serialized_cells = serialized_records
         if reformat:
```

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/json.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/json.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/nested_list.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/nested_list.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/numbers.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/numbers.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/pandas_io.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/pandas_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,7 +221,18 @@
     def load_file(scheme, path, params):
         return pd.read_stata(path, **params)
 
     @staticmethod
     def dump_file(df, scheme, path, params):
         params["write_index"] = params.get("write_index", False)
         df.to_stata(path, **params)
+
+
+@register_adapter(["pickledf"])
+class PicklePandasAdapter(FileAdapterMixin, Adapter):
+    @staticmethod
+    def load_file(scheme, path, params):
+        return pd.read_pickle(path, **params)
+
+    @staticmethod
+    def dump_file(df, scheme, path, params):
+        return df.to_pickle(path, **params)
```

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/python.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/python.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/rdbms.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/rdbms.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/smart_sheet.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/smart_sheet.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/sql_literal.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/sql_literal.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from tableconv.adapters.df.base import Adapter, register_adapter
 from tableconv.adapters.df.file_adapter_mixin import FileAdapterMixin
 
 
-@register_adapter(["sql_values"], write_only=True)
+@register_adapter(["sql_values", "sql_literal"], write_only=True)
 class SQLLiteralAdapter(FileAdapterMixin, Adapter):
     """Currently only supports the PostgreSQL-flavored VALUES syntax"""
 
     text_based = True
 
     @staticmethod
     def get_example_url(scheme):
```

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/sumo_logic.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/sumo_logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,17 +103,17 @@
     search_job_id = search_job["id"]
 
     logger.info(f"Waiting for query to complete (job id: {search_job_id})")
     time.sleep((SUMO_API_RESULTS_POLLING_INTERVAL / 2).total_seconds())
     while True:
         status = sumo.search_job_status(search_job_id)
         STATES_THAT_MEAN_QUERY_STILL_IN_PROGRESS = [
-            'GATHERING RESULTS',
-            'DONE GATHERING HISTOGRAM',
-            'GATHERING RESULTS FROM SUBQUERIES',
+            "GATHERING RESULTS",
+            "DONE GATHERING HISTOGRAM",
+            "GATHERING RESULTS FROM SUBQUERIES",
         ]
 
         if status["state"] in STATES_THAT_MEAN_QUERY_STILL_IN_PROGRESS:
             time.sleep(SUMO_API_RESULTS_POLLING_INTERVAL.total_seconds())
             continue
 
         assert status["state"] == "DONE GATHERING RESULTS", status["state"]
```

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/text_array.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/text_array.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/adapters/df/yaml.py` & `tableconv-1.9957.20240331/tableconv/adapters/df/yaml.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/core.py` & `tableconv-1.9957.20240331/tableconv/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+import hashlib
+import json
 import logging
 import os
+import pathlib
 import re
 import tempfile
 import urllib.parse
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import ciso8601
 import pandas as pd
 from pandas.errors import EmptyDataError as pd_EmptyDataError
+from platformdirs import user_cache_dir
 
 from tableconv.adapters.df import read_adapters, write_adapters
 from tableconv.adapters.df.base import Adapter
 from tableconv.exceptions import (
     EmptyDataError,
     InvalidLocationReferenceError,
     InvalidURLSyntaxError,
-    UnrecognizedFormatError,
     SchemaCoercionError,
+    UnrecognizedFormatError,
 )
 from tableconv.in_memory_query import query_in_memory
 from tableconv.uri import parse_uri
 
 logger = logging.getLogger(__name__)
 
 
@@ -71,15 +75,15 @@
         if from_df is not None:
             self.df = from_df
         if from_dict_records is not None:
             self.df = pd.DataFrame.from_records(from_dict_records)
         if self.df.empty:
             raise EmptyDataError
 
-    def dump_to_url(self, url: str, params: Optional[Dict[str, Any]] = None) -> str:
+    def dump_to_url(self, url: str, params: Optional[Dict[str, Any]] = None) -> Optional[str]:
         """
         Export the table in the format and location identified by url.
 
         :return:
             A "permalink" url that can be used to access the exported data. This URL is normally identical to the URL
             that was passed in, but not always in cases where e.g. a new ID needed to be dynamically generated during
             the export, or in cases when the passed in URL was relative or otherwise vague.
@@ -102,15 +106,15 @@
         if params:
             # TODO: This is a total hack! Implementing real structured table references, including structured passing of
             # params to adapters, is still pending. Right now everything is stringly-typed internally.
             assert "?" not in url
             url += f"?{urllib.parse.urlencode(params)}"
         write_adapter_name = write_adapter.__qualname__  # type: ignore[attr-defined]
         logger.debug(f"Exporting data out via {write_adapter_name} to {url}")
-        with pd.option_context('display.float_format', str):
+        with pd.option_context("display.float_format", str):
             return write_adapter.dump(self.df, url)
 
     def get_json_schema(self):
         """
         Warning: This is just experimental / exploratory. The current implementation is also buggy.
         """
         # Consider instead using https://github.com/pandas-dev/pandas/blob/v1.3.2/pandas/io/json/_table_schema.py
@@ -269,21 +273,63 @@
     if os.path.exists(path):
         TWO_GIBIBYTES = 2 * (1024**3)
         if os.stat(path).st_size > TWO_GIBIBYTES:
             # TODO: make this adapter specific
             logger.warning("This looks like a huge table, expect heavy RAM and CPU usage.")
 
 
+def get_cache_key(read_adapter_name, url, query):
+    key_bits = json.dumps([read_adapter_name, url, query])
+    key = hashlib.md5(key_bits.encode()).hexdigest()
+    logger.debug(f"Cache key: {key} ({key_bits})")
+    return key
+
+
+CACHE_DIR = user_cache_dir("tableconv", "tableconv")
+
+
+def get_cache_file_path(read_adapter_name, url, query):
+    key = get_cache_key(read_adapter_name, url, query)
+    return os.path.join(CACHE_DIR, f"autocachev1/{key}.pickledf")
+
+
+def infer_if_url_is_local(url):
+    if os.path.exists(parse_uri(url).path):
+        return True
+    if "localhost" in url or "127.0.0.1" in url:
+        return True
+    if "http" not in url and not re.search(r":\d\d+", url):
+        return True
+    return False
+
+
+def load_from_cache(read_adapter_name, url, query) -> pd.DataFrame:
+    path = get_cache_file_path(read_adapter_name, url, query)
+    if not os.path.exists(path):
+        return None
+    return pd.read_pickle(path)
+
+
+def save_to_cache(read_adapter_name, url, query, df):
+    if infer_if_url_is_local(url):
+        # Don't cache local data
+        return
+    path = get_cache_file_path(read_adapter_name, url, query)
+    pathlib.Path(os.path.dirname(path)).mkdir(parents=True, exist_ok=True)  # ensure cache directory exists
+    df.to_pickle(path)
+
+
 def load_url(
     url: Union[str, Path],
     params: Optional[Dict[str, Any]] = None,
     query: Optional[str] = None,
     filter_sql: Optional[str] = None,
     schema_coercion: Optional[Dict[str, str]] = None,
     restrict_schema: bool = False,
+    autocache: bool = False,
 ) -> IntermediateExchangeTable:
     """
     Load the data referenced by ``url`` into tableconv's abstract intermediate tabular data type
     (:ref:`IntermediateExchangeTable`).
 
     :param url:
         This can be any URL referencing tabular or psuedo-tabular data. Refer to :ref:Adapters for the supported
@@ -333,24 +379,34 @@
         # table references, including structured passing of params to adapters, is still pending. Right now params are
         # totally stringly-typed internally, and are not even consistently represented within strings (nor even URL-spec
         # compliant!).
         assert "?" not in url
         url += f"?{urllib.parse.urlencode(params)}"
 
     read_adapter_name = read_adapter.__qualname__  # type: ignore[attr-defined]
-    logger.debug(f"Loading data in via {read_adapter_name} from {url}")
+    using_cache_statement = ""
     warn_if_location_too_large(url)
-    try:
-        df = read_adapter.load(url, query)
-    except pd_EmptyDataError as exc:
-        raise EmptyDataError(f"Empty data source {url}: {str(exc)}") from exc
-    except FileNotFoundError as exc:
-        raise InvalidLocationReferenceError(f"{url} not found: {str(exc)}") from exc
-    if df.empty:
-        raise EmptyDataError(f"Empty data source {url}")
+    df = None
+    if autocache:
+        df = load_from_cache(read_adapter_name, url, query)
+        if df is not None:
+            using_cache_statement = " (LOCALLY CACHED COPY)"
+            logger.info("Using cached data")
+    logger.debug(f"Loading data in via {read_adapter_name} from {url}{using_cache_statement}")
+    if df is None:
+        try:
+            df = read_adapter.load(url, query)
+        except pd_EmptyDataError as exc:
+            raise EmptyDataError(f"Empty data source {url}: {str(exc)}") from exc
+        except FileNotFoundError as exc:
+            raise InvalidLocationReferenceError(f"{url} not found: {str(exc)}") from exc
+        if df.empty:
+            raise EmptyDataError(f"Empty data source {url}")
+        if autocache:
+            save_to_cache(read_adapter_name, url, query, df)
 
     # Schema coercion
     if schema_coercion:
         df = coerce_schema(df, schema_coercion, restrict_schema)
 
     # Run in-memory filters
     if filter_sql:
```

### Comparing `tableconv-1.9947.20231219/tableconv/exceptions.py` & `tableconv-1.9957.20240331/tableconv/exceptions.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/in_memory_query.py` & `tableconv-1.9957.20240331/tableconv/in_memory_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,17 +50,17 @@
             if table_name == "data":
                 data_df = df
                 break
         transposed_data_df = data_df.transpose(copy=True).reset_index()
         dfs.append((transposed_data_table_name, transposed_data_df))
 
     query = re.sub(
-        r"\b(?:from_)?unix\((.+?)\)", r"(TIMESTAMP '1970-01-01 00:00:00' + to_seconds(\1))", query, flags=re.IGNORECASE)
-    query = re.sub(
-        r"\b(?:from_)?iso8601\((.+?)\)", r"CAST(\1 AS TIMESTAMP)", query, flags=re.IGNORECASE)
+        r"\b(?:from_)?unix\((.+?)\)", r"(TIMESTAMP '1970-01-01 00:00:00' + to_seconds(\1))", query, flags=re.IGNORECASE
+    )
+    query = re.sub(r"\b(?:from_)?iso8601\((.+?)\)", r"CAST(\1 AS TIMESTAMP)", query, flags=re.IGNORECASE)
 
     return dfs, query
 
 
 def query_in_memory(dfs: List[Tuple[str, pd.DataFrame]], query: str) -> pd.DataFrame:
     """Warning: Has a side effect of mutating the dfs"""
     import duckdb
@@ -70,17 +70,17 @@
     for table_name, df in dfs:
         flatten_arrays_for_duckdb(df)
         duck_conn.register(table_name, df)
     try:
         duck_conn.execute(query)
     except (RuntimeError, duckdb.ParserException, duckdb.CatalogException) as exc:
         raise InvalidQueryError(*exc.args) from exc
-    except duckdb.StandardException as exc:
-        if 'Parser Error' in exc.args[0]:
+    except duckdb.StandardException as exc:  # type: ignore[attr-defined]  # needed for backwards-compat with old duckdb
+        if "Parser Error" in exc.args[0]:
             raise InvalidQueryError(*exc.args) from exc
         raise
     except duckdb.BinderException as exc:
-        if 'No function matches the given name' in exc.args[0]:
+        if "No function matches the given name" in exc.args[0]:
             raise InvalidQueryError(*exc.args) from exc
         raise
     result_df = duck_conn.fetchdf()
     return result_df
```

### Comparing `tableconv-1.9947.20231219/tableconv/interactive.py` & `tableconv-1.9957.20240331/tableconv/interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 
 def create_empty_file(path):
     open(path, "wb").close()  # noqa: SIM115
 
 
 def run_interactive_shell(
-    source: str, dest: str, intermediate_filter_sql: str, open_dest: bool, schema_coercion, restrict_schema
+    source: str, dest: str, intermediate_filter_sql: str, open_dest: bool, schema_coercion, restrict_schema, autocache
 ) -> None:
     # shell_width, shell_height = shutil.get_terminal_size()
     try:
         readline.read_history_file(INTERACTIVE_HIST_PATH)
     except FileNotFoundError:
         create_empty_file(INTERACTIVE_HIST_PATH)
 
@@ -151,14 +151,15 @@
             last_result = None
             table = load_url(
                 url=source,
                 query=query,
                 filter_sql=intermediate_filter_sql,
                 schema_coercion=schema_coercion,
                 restrict_schema=restrict_schema,
+                autocache=autocache,
             )
             last_result = table
             # Dump to destination
             output = table.dump_to_url(url=dest)
             if output:
                 print(f"(Wrote out {output})", file=sys.stderr)
             if output and open_dest:
```

### Comparing `tableconv-1.9947.20231219/tableconv/main.py` & `tableconv-1.9957.20240331/tableconv/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,17 @@
             "loggers": {
                 "googleapiclient.discovery_cache": {
                     "level": "ERROR",
                 },
                 "botocore": {
                     "level": "WARNING",
                 },
+                "thrift.transport.TSocket": {
+                    "level": "CRITICAL",
+                },
             },
             "root": {
                 "level": "INFO",
                 "handlers": ["default"],
             },
         }
     )
@@ -175,14 +178,15 @@
     parser.add_argument("-q", "-Q", "--query", dest="source_query", default=None, help="Query to run on the source. Even for non-SQL datasources (e.g. csv or json), SQL querying is still supported, try `SELECT * FROM data`.")  # noqa: E501
     parser.add_argument("-F", "--filter", dest="intermediate_filter_sql", default=None, help="Filter (i.e. transform) the input data using a SQL query operating on the dataset in memory using DuckDB SQL.")  # noqa: E501
     parser.add_argument("-o", "--dest", "--out", "--output", dest="DEST_URL", type=str, help="Specify the data destination URL. If this destination already exists, be aware that the default behavior is to overwrite.")  # noqa: E501
     parser.add_argument("-i", "--interactive", action="store_true", help="Enter interactive REPL query mode.")  # noqa: E501
     parser.add_argument("--open", dest="open_dest", action="store_true", help="Open resulting file/url in the operating system desktop environment. (not supported for all destination types)")  # noqa: E501
     parser.add_argument("--schema", "--coerce-schema", dest="schema_coercion", default=None, help="Coerce source schema according to a schema definition. (WARNING: experimental feature)")  # noqa: E501
     parser.add_argument("--restrict-schema", dest="restrict_schema", action="store_true", help="Exclude all columns not included in the SCHEMA_COERCION definition. (WARNING: experimental feature)")  # noqa: E501
+    parser.add_argument("--autocache", "--cache", action="store_true", help="Cache network data, and reuse cached data.")  # noqa: E501
     parser.add_argument("-v", "--verbose", "--debug", dest="verbose", action="store_true", help="Show debug details, including API calls and error sources.")  # noqa: E501
     parser.add_argument("--version", action="version", help="Show version number and exit", version=f"%(prog)s {__version__}")  # noqa: E501
     parser.add_argument("--quiet", action="store_true", help="Only display errors.")
     parser.add_argument("--print", "--print-dest", action="store_true", help="Print resulting URL/path to stdout, for chaining with other commands.")  # noqa: E501
     parser.add_argument("--debug-shell", "--pandas-debug-shell", "--debug-pandas-shell", action="store_true", help=argparse.SUPPRESS)  # noqa: E501
     parser.add_argument("--daemon", action="store_true", help="Tableconv startup time (python startup time) is slow. To mitigate that, you can first run tableconv as a daemon, and then all future invocations (while daemon is still alive) will be fast.  (WARNING: experimental feature)")  # noqa: E501
 
@@ -231,24 +235,26 @@
             run_interactive_shell(
                 args.SOURCE_URL,
                 dest,
                 args.intermediate_filter_sql,
                 args.open_dest,
                 schema_coercion,
                 args.restrict_schema,
+                args.autocache,
             )
             return
 
         # Load source
         table = load_url(
             url=args.SOURCE_URL,
             query=args.source_query,
             filter_sql=args.intermediate_filter_sql,
             schema_coercion=schema_coercion,
             restrict_schema=args.restrict_schema,
+            autocache=args.autocache,
         )
         if args.debug_shell:
             df = table.as_pandas_df()  # noqa: F841
             breakpoint()
 
         # Dump to destination
         output = table.dump_to_url(url=dest)
```

### Comparing `tableconv-1.9947.20231219/tableconv/parse_time.py` & `tableconv-1.9957.20240331/tableconv/parse_time.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv/uri.py` & `tableconv-1.9957.20240331/tableconv/uri.py`

 * *Files identical despite different names*

### Comparing `tableconv-1.9947.20231219/tableconv.egg-info/PKG-INFO` & `tableconv-1.9957.20240331/tableconv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableconv
-Version: 1.9947.20231219
+Version: 1.9957.20240331
 Summary: CLI data plumbing tool
 Home-page: https://github.com/personalcomputer/tableconv
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
@@ -121,25 +121,26 @@
   -h, --help            show this help message and exit
   -q SOURCE_QUERY, -Q SOURCE_QUERY, --query SOURCE_QUERY
                         Query to run on the source. Even for non-SQL datasources (e.g. csv or
                         json), SQL querying is still supported, try `SELECT * FROM data`.
   -F INTERMEDIATE_FILTER_SQL, --filter INTERMEDIATE_FILTER_SQL
                         Filter (i.e. transform) the input data using a SQL query operating on the
                         dataset in memory using DuckDB SQL.
-  -o DEST_URL, --dest DEST_URL, --out DEST_URL
+  -o DEST_URL, --dest DEST_URL, --out DEST_URL, --output DEST_URL
                         Specify the data destination URL. If this destination already exists, be
                         aware that the default behavior is to overwrite.
   -i, --interactive     Enter interactive REPL query mode.
   --open                Open resulting file/url in the operating system desktop environment. (not
                         supported for all destination types)
   --schema SCHEMA_COERCION, --coerce-schema SCHEMA_COERCION
                         Coerce source schema according to a schema definition. (WARNING:
                         experimental feature)
   --restrict-schema     Exclude all columns not included in the SCHEMA_COERCION definition.
                         (WARNING: experimental feature)
+  --autocache, --cache  Cache network data, and reuse cached data.
   -v, --verbose, --debug
                         Show debug details, including API calls and error sources.
   --version             Show version number and exit
   --quiet               Only display errors.
   --print, --print-dest
                         Print resulting URL/path to stdout, for chaining with other commands.
   --daemon              Tableconv startup time (python startup time) is slow. To mitigate that,
@@ -175,51 +176,55 @@
   example.jsonl 
   example.jsonlines 
   example.ldjson 
   example.ndjson 
   example.numbers (source only)
   example.orc (source only)
   example.parquet 
+  example.pickledf 
   example.py 
   example.python 
   example.tsv 
   example.xls 
   example.xlsx 
   example.yaml 
   example.yml 
   gsheets://:new: 
-  jiracloud://mycorpname (source only)
+  jc://ls -l (source only)
   jiraformat:- (dest only)
   jsonarray:- 
   latex:- (dest only)
+  leveldblog:output-0 (source only)
   list:- 
   markdown:- (dest only)
   md:- (dest only)
   mediawikiformat:- (dest only)
   moinmoinformat:- (dest only)
   mssql://127.0.0.1:5432/example_db 
   mysql://127.0.0.1:5432/example_db 
   nestedlist:- (source only)
   oracle://127.0.0.1:5432/example_db 
+  osquery://processes (source only)
   postgis://127.0.0.1:5432/example_db 
   postgres://127.0.0.1:5432/example_db 
   postgresql://127.0.0.1:5432/example_db 
   pylist:- 
   pythonlist:- 
   rst:- (dest only)
   smartsheet://SHEET_ID (source only)
+  sql_literal:- (dest only)
   sql_values:- (dest only)
   sqlite3:///tmp/example.db 
   sqlite:///tmp/example.db 
   sumologic://?from=2021-03-01T00:00:00Z&to=2021-05-03T00:00:00Z (source only)
   tex:- (dest only)
   yamlsequence:- 
 
 help & support:
-  https://github.com/personalcomputer/tableconv/issues
+  https://github.com/personalcomputer/tableconv/issues/new
 ```
 
 ## Python API
 
 ### Quickstart Example: Basic API usage: Replicating a typical CLI command using the API
 
 ```python
```

### Comparing `tableconv-1.9947.20231219/tableconv.egg-info/SOURCES.txt` & `tableconv-1.9957.20240331/tableconv.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,21 @@
 tableconv/adapters/df/aws_athena.py
 tableconv/adapters/df/aws_dynamodb.py
 tableconv/adapters/df/aws_logs.py
 tableconv/adapters/df/base.py
 tableconv/adapters/df/example.py
 tableconv/adapters/df/file_adapter_mixin.py
 tableconv/adapters/df/gsheets.py
+tableconv/adapters/df/jc.py
 tableconv/adapters/df/jira.py
 tableconv/adapters/df/json.py
 tableconv/adapters/df/leveldb.py
 tableconv/adapters/df/nested_list.py
 tableconv/adapters/df/numbers.py
+tableconv/adapters/df/osquery.py
 tableconv/adapters/df/pandas_io.py
 tableconv/adapters/df/python.py
 tableconv/adapters/df/rdbms.py
 tableconv/adapters/df/smart_sheet.py
 tableconv/adapters/df/sql_literal.py
 tableconv/adapters/df/sumo_logic.py
 tableconv/adapters/df/text_array.py
```

### Comparing `tableconv-1.9947.20231219/tableconv_daemon/main.py` & `tableconv-1.9957.20240331/tableconv_daemon/main.py`

 * *Files identical despite different names*

