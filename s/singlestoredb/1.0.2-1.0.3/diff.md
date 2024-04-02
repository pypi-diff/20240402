# Comparing `tmp/singlestoredb-1.0.2.tar.gz` & `tmp/singlestoredb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singlestoredb-1.0.2.tar", last modified: Fri Mar  8 17:45:09 2024, max compression
+gzip compressed data, was "singlestoredb-1.0.3.tar", last modified: Tue Apr  2 21:29:31 2024, max compression
```

## Comparing `singlestoredb-1.0.2.tar` & `singlestoredb-1.0.3.tar`

### file list

```diff
@@ -1,135 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.310416 singlestoredb-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-08 17:45:09.310416 singlestoredb-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   151339 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/accel.c
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-08 17:45:09.310416 singlestoredb-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.298416 singlestoredb-1.0.2/singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.302416 singlestoredb-1.0.2/singlestoredb/alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    44227 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.302416 singlestoredb-1.0.2/singlestoredb/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/functions/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    36712 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/functions/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.302416 singlestoredb-1.0.2/singlestoredb/functions/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/functions/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/functions/ext/arrow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18911 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/functions/ext/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/functions/ext/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/functions/ext/rowdat_1.py
--rw-r--r--   0 runner    (1001) docker     (127)    19343 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/functions/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.302416 singlestoredb-1.0.2/singlestoredb/fusion/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/fusion/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)    18338 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/fusion/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.302416 singlestoredb-1.0.2/singlestoredb/fusion/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/fusion/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/fusion/handlers/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/fusion/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/fusion/handlers/workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/fusion/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/fusion/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.302416 singlestoredb-1.0.2/singlestoredb/http/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/http/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.302416 singlestoredb-1.0.2/singlestoredb/management/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/management/billing_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/management/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/management/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/management/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/management/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/management/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51907 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/management/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.306416 singlestoredb-1.0.2/singlestoredb/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/charset.py
--rw-r--r--   0 runner    (1001) docker     (127)    64746 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.306416 singlestoredb-1.0.2/singlestoredb/mysql/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/constants/CLIENT.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/constants/COMMAND.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/constants/CR.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/constants/ER.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/constants/FIELD_TYPE.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/constants/FLAG.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/constants/SERVER_STATUS.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21246 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/cursors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/err.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/optionfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.306416 singlestoredb-1.0.2/singlestoredb/mysql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_DictCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_SSCursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_err.py
--rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_load_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_nextset.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/test_optionfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.306416 singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.306416 singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/mysql/times.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/pytest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.310416 singlestoredb-1.0.2/singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/empty.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.310416 singlestoredb-1.0.2/singlestoredb/tests/ext_funcs/
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/ext_funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/local_infile.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test2.sql
--rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_basics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    50741 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_dbapi.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37330 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_ext_func.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    47693 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_ext_func_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_fusion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_http.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_results.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28490 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_udf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/test_xdict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.310416 singlestoredb-1.0.2/singlestoredb/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/utils/convert_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/utils/mogrify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/utils/results.py
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-03-08 17:44:43.000000 singlestoredb-1.0.2/singlestoredb/utils/xdict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:45:09.298416 singlestoredb-1.0.2/singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-03-08 17:45:09.000000 singlestoredb-1.0.2/singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-08 17:45:09.000000 singlestoredb-1.0.2/singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:45:09.000000 singlestoredb-1.0.2/singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-08 17:45:09.000000 singlestoredb-1.0.2/singlestoredb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-08 17:45:09.000000 singlestoredb-1.0.2/singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-08 17:45:09.000000 singlestoredb-1.0.2/singlestoredb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   151339 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/accel.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb/alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44227 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12515 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36712 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb/functions/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/arrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21938 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/mmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22274 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/ext/rowdat_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18866 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/functions/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/fusion/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18338 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/fusion/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handlers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/handlers/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11772 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/fusion/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/http/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/management/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/billing_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14362 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8810 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51907 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/management/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.185015 singlestoredb-1.0.3/singlestoredb/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/charset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64746 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.189015 singlestoredb-1.0.3/singlestoredb/mysql/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/CLIENT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/COMMAND.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/CR.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/ER.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/FIELD_TYPE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/FLAG.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/SERVER_STATUS.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21246 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/cursors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/err.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/optionfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.189015 singlestoredb-1.0.3/singlestoredb/mysql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4878 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_DictCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_SSCursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15465 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32297 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_err.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_load_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_nextset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/test_optionfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.189015 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.189015 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31414 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/mysql/times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/empty.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/singlestoredb/tests/ext_funcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/ext_funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/local_infile.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9954 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test2.sql
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44180 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_basics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11184 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    50741 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_dbapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37347 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_ext_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47693 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_ext_func_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_fusion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8580 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_http.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28223 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6582 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_results.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4500 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28075 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_udf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10408 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/test_xdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9969 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.193015 singlestoredb-1.0.3/singlestoredb/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24503 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/convert_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/mogrify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2024-04-02 21:29:08.000000 singlestoredb-1.0.3/singlestoredb/utils/xdict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:29:31.181015 singlestoredb-1.0.3/singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 21:29:31.000000 singlestoredb-1.0.3/singlestoredb.egg-info/top_level.txt
```

### Comparing `singlestoredb-1.0.2/LICENSE` & `singlestoredb-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/PKG-INFO` & `singlestoredb-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.0.2
+Version: 1.0.3
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.0.2/README.md` & `singlestoredb-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/accel.c` & `singlestoredb-1.0.3/accel.c`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/setup.cfg` & `singlestoredb-1.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = singlestoredb
-version = 1.0.2
+version = 1.0.3
 description = Interface to the SingleStoreDB database and workspace management APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/singlestoredb-python
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
```

### Comparing `singlestoredb-1.0.2/setup.py` & `singlestoredb-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/__init__.py` & `singlestoredb-1.0.3/singlestoredb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 >>> cur = conn.cursor()
 >>> cur.execute('select * from customers')
 >>> for row in cur:
 ...     print(row)
 
 """
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 from typing import Any
 
 from .config import options, get_option, set_option, describe_option
 from .connection import connect, apilevel, threadsafety, paramstyle
 from .exceptions import (
     Warning, Error, InterfaceError, DatabaseError, OperationalError,
```

### Comparing `singlestoredb-1.0.2/singlestoredb/alchemy/__init__.py` & `singlestoredb-1.0.3/singlestoredb/alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/auth.py` & `singlestoredb-1.0.3/singlestoredb/auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/config.py` & `singlestoredb-1.0.3/singlestoredb/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -249,14 +249,26 @@
 #
 register_option(
     'management.token', 'string', check_str, None,
     'Specifies the authentication token for the management API.',
     environ=['SINGLESTOREDB_MANAGEMENT_TOKEN'],
 )
 
+register_option(
+    'management.base_url', 'string', check_str, 'https://api.singlestore.com',
+    'Specifies the base URL for the management API.',
+    environ=['SINGLESTOREDB_MANAGEMENT_BASE_URL'],
+)
+
+register_option(
+    'management.version', 'string', check_str, 'v1',
+    'Specifies the version for the management API.',
+    environ=['SINGLESTOREDB_MANAGEMENT_VERSION'],
+)
+
 
 #
 # Debugging options
 #
 register_option(
     'debug.queries', 'bool', check_bool, False,
     'Print queries and parameters to stderr.',
```

### Comparing `singlestoredb-1.0.2/singlestoredb/connection.py` & `singlestoredb-1.0.3/singlestoredb/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/converters.py` & `singlestoredb-1.0.3/singlestoredb/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/exceptions.py` & `singlestoredb-1.0.3/singlestoredb/exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/functions/decorator.py` & `singlestoredb-1.0.3/singlestoredb/functions/decorator.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,59 +18,28 @@
     return [x]
 
 
 def udf(
     func: Optional[Callable[..., Any]] = None,
     *,
     name: Optional[str] = None,
-    database: Optional[str] = None,
-    environment: Optional[str] = None,
-    packages: Optional[Union[str, List[str]]] = None,
-    resources: Optional[Union[str, List[str]]] = None,
-    max_batch_size: int = 500,
-    n_processes: int = 1,
-    n_instances: int = 1,
     args: Optional[Union[DataType, List[DataType], Dict[str, DataType]]] = None,
     returns: Optional[str] = None,
-    replace: bool = False,
-    remote_service: Optional[str] = None,
-    link: Optional[str] = None,
     data_format: Optional[str] = None,
     include_masks: bool = False,
 ) -> Callable[..., Any]:
     """
     Apply attributes to a UDF.
 
     Parameters
     ----------
     func : callable, optional
         The UDF to apply parameters to
     name : str, optional
         The name to use for the UDF in the database
-    database : str, optional
-        The database to create the functions in
-    environment : str, optional
-        The environment to create for the functions
-    packages : str or list-of-strs, optional
-        The package dependency specifications. Strings must be in the
-        format used in requirements.txt files.
-    max_match_size : int, optional
-        The number of rows to batch in the server before sending
-        them to the UDF application
-    n_processes : int, optional
-        The number of sub-processes to spin up to process sub-batches
-        of rows of data. This may be used if the UDF is CPU-intensive
-        and there are free CPUs in the server the web application
-        is running in. If the UDF is very short-running, setting this
-        parameter to greater than one will likey cause the UDF to
-        run slower since the overhead of the extra processes and moving
-        data would be the limiting factor.
-    n_instances : int, optional
-        The number of runtime environments to use to handle data
-        processing requests
     args : str | Callable | List[str | Callable] | Dict[str, str | Callable], optional
         Specifies the data types of the function arguments. Typically,
         the function data types are derived from the function parameter
         annotations. These annotations can be overridden. If the function
         takes a single type for all parameters, `args` can be set to a
         SQL string describing all parameters. If the function takes more
         than one parameter and all of the parameters are being manually
@@ -79,38 +48,26 @@
         for a subset of parameters; the keys are the names of the
         function parameters. Callables may also be used for datatypes. This
         is primarily for using the functions in the ``dtypes`` module that
         are associated with SQL types with all default options (e.g., ``dt.FLOAT``).
     returns : str, optional
         Specifies the return data type of the function. If not specified,
         the type annotation from the function is used.
-    replace : bool, optional
-        Should an existing function of the same name be replaced when
-        creating the function in the database?
-    remote_service : str, optional
-        URL of the remote service that handles this function. If using an
-        environment, this URL is generated automatically.
-    link : str, optional
-        Name of link to use to connect to remote service
     data_format : str, optional
         The data format of each parameter: python, pandas, arrow, polars
     include_masks : bool, optional
         Should boolean masks be included with each input parameter to indicate
         which elements are NULL? This is only used when a input parameters are
         configured to a vector type (numpy, pandas, polars, arrow).
 
     Returns
     -------
     Callable
 
     """
-    assert max_batch_size >= 1
-    assert n_processes >= 1
-    assert n_instances >= 1
-
     if args is None:
         pass
     elif isinstance(args, (list, tuple)):
         args = list(args)
         for i, item in enumerate(args):
             if callable(item):
                 args[i] = item()
@@ -149,26 +106,16 @@
             'include_masks is only valid when using '
             'vectors for input parameters',
         )
 
     _singlestoredb_attrs = {  # type: ignore
         k: v for k, v in dict(
             name=name,
-            database=database,
-            environment=environment,
-            packages=listify(packages),
-            resources=listify(resources),
-            max_batch_size=max(1, int(max_batch_size)),
-            n_processes=max(1, int(n_processes)),
-            n_instances=max(1, int(n_instances)),
             args=args,
             returns=returns,
-            replace=bool(replace),
-            remote_service=remote_service,
-            link=link,
             data_format=data_format,
             include_masks=include_masks,
         ).items() if v is not None
     }
 
     # No func was specified, this is an uncalled decorator that will get
     # called later, so the wrapper much be created with the func passed
```

### Comparing `singlestoredb-1.0.2/singlestoredb/functions/dtypes.py` & `singlestoredb-1.0.3/singlestoredb/functions/dtypes.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/functions/ext/arrow.py` & `singlestoredb-1.0.3/singlestoredb/functions/ext/arrow.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/functions/ext/asgi.py` & `singlestoredb-1.0.3/singlestoredb/functions/ext/asgi.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,32 +14,35 @@
 created in Python code rather than from the command-line, exported
 functions can be specified in the parameters.
 
 An example of starting a server is shown below.
 
 Example
 -------
-$ SINGLESTOREDB_EXT_FUNCTIONS='myfuncs.[percentile_90,percentile_95]' \
+$ SINGLESTOREDB_EXT_FUNCTIONS='myfuncs.[percentage_90,percentage_95]' \
     uvicorn --factory singlestoredb.functions.ext:create_app
 
 '''
 import importlib.util
 import io
 import itertools
+import json
 import os
-import urllib
+import re
+import secrets
 from types import ModuleType
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
+from typing import Set
 from typing import Tuple
 from typing import Union
 
 from . import arrow
 from . import json as jdata
 from . import rowdat_1
 from ... import connection
@@ -192,16 +195,20 @@
             Iterable[str],
             Callable[..., Any],
             Iterable[Callable[..., Any]],
             ModuleType,
             Iterable[ModuleType],
         ]
     ] = None,
-
-
+    app_mode: str = 'remote',
+    url: str = 'http://localhost:8000/invoke',
+    data_format: str = 'rowdat_1',
+    data_version: str = '1.0',
+    link_config: Optional[Dict[str, Any]] = None,
+    link_credentials: Optional[Dict[str, Any]] = None,
 ) -> Callable[..., Any]:
     '''
     Create an external function application.
 
     If `functions` is None, the environment is searched for function
     specifications in variables starting with `SINGLESTOREDB_EXT_FUNCTIONS`.
     Any number of environment variables can be specified as long as they
@@ -212,14 +219,28 @@
     ----------
     functions : str or Iterable[str], optional
         Python functions are specified using a string format as follows:
             * Single function : <pkg1>.<func1>
             * Multiple functions : <pkg1>.[<func1-name,func2-name,...]
             * Function aliases : <pkg1>.[<func1@alias1,func2@alias2,...]
             * Multiple packages : <pkg1>.<func1>:<pkg2>.<func2>
+    app_mode : str, optional
+        The mode of operation for the application: remote or collocated
+    url : str, optional
+        The URL of the function API
+    data_format : str, optional
+        The format of the data rows: 'rowdat_1' or 'json'
+    data_version : str, optional
+        The version of the call format to expect: '1.0'
+    link_config : Dict[str, Any], optional
+        The CONFIG section of a LINK definition. This dictionary gets
+        converted to JSON for the CREATE LINK call.
+    link_credentials : Dict[str, Any], optional
+        The CREDENTIALS section of a LINK definition. This dictionary gets
+        converted to JSON for the CREATE LINK call.
 
     Returns
     -------
     Callable : the application request handler
 
     '''
 
@@ -465,24 +486,24 @@
             body = output_handler['dump'](func._ext_func_returns, *out)  # type: ignore
 
             await send(output_handler['response'])
 
         # Handle api reflection
         elif method == 'GET' and path == show_create_function_path:
             host = headers.get(b'host', b'localhost:80')
-            url = f'{scope["scheme"]}://{host.decode("utf-8")}/invoke'
+            reflected_url = f'{scope["scheme"]}://{host.decode("utf-8")}/invoke'
             data_format = 'json' if b'json' in content_type else 'rowdat_1'
 
             syntax = []
             for key, endpoint in endpoints.items():
                 if not func_name or key == func_name:
                     syntax.append(
                         signature_to_sql(
                             endpoint._ext_func_signature,  # type: ignore
-                            base_url=url,
+                            url=url or reflected_url,
                             data_format=data_format,
                         ),
                     )
             body = '\n'.join(syntax).encode('utf-8')
 
             await send(text_response_dict)
 
@@ -492,64 +513,121 @@
             await send(path_not_found_response_dict)
 
         # Send body
         out = body_response_dict.copy()
         out['body'] = body
         await send(out)
 
+    def _create_link(
+        config: Optional[Dict[str, Any]],
+        credentials: Optional[Dict[str, Any]],
+    ) -> Tuple[str, str]:
+        """Generate CREATE LINK command."""
+        if not config and not credentials:
+            return '', ''
+
+        link_name = f'link_{secrets.token_hex(16)}'
+        out = [f'CREATE LINK {link_name} AS HTTP']
+
+        if config:
+            out.append(f"CONFIG '{json.dumps(config)}'")
+
+        if credentials:
+            out.append(f"CREDENTIALS '{json.dumps(credentials)}'")
+
+        return link_name, ' '.join(out) + ';'
+
+    def _locate_app_functions(cur: Any) -> Tuple[Set[str], Set[str]]:
+        """Locate all current functions and links belonging to this app."""
+        funcs, links = set(), set()
+        cur.execute('SHOW FUNCTIONS')
+        for name, ftype, _, _, _, link in list(cur):
+            # Only look at external functions
+            if 'external' not in ftype.lower():
+                continue
+            # See if function URL matches url
+            cur.execute(f'SHOW CREATE FUNCTION `{name}`')
+            for fname, _, code, *_ in list(cur):
+                m = re.search(r" (?:\w+) SERVICE '([^']+)'", code)
+                if m and m.group(1) == url:
+                    funcs.add(fname)
+                    if link:
+                        links.add(link)
+        return funcs, links
+
     def show_create_functions(
-        base_url: str = 'http://localhost:8000',
-        data_format: str = 'rowdat_1',
+        replace: bool = False,
     ) -> List[str]:
+        """Generate CREATE FUNCTION calls."""
+        if not endpoints:
+            return []
+
         out = []
+        link = ''
+        if app_mode.lower() == 'remote':
+            link, link_str = _create_link(link_config, link_credentials)
+            if link and link_str:
+                out.append(link_str)
+
         for key, endpoint in endpoints.items():
             out.append(
                 signature_to_sql(
                     endpoint._ext_func_signature,  # type: ignore
-                    base_url=urllib.parse.urljoin(base_url, '/invoke'),
+                    url=url,
                     data_format=data_format,
+                    app_mode=app_mode,
+                    replace=replace,
+                    link=link or None,
                 ),
             )
+
         return out
 
     app.show_create_functions = show_create_functions  # type: ignore
 
     def register_functions(
         *connection_args: Any,
-        base_url: str = 'http://localhost:8000',
-        data_format: str = 'rowdat_1',
+        replace: bool = False,
         **connection_kwargs: Any,
     ) -> None:
+        """Register functions with the database."""
         with connection.connect(*connection_args, **connection_kwargs) as conn:
             with conn.cursor() as cur:
-                for func in app.show_create_functions(  # type: ignore
-                                base_url=base_url,
-                                data_format=data_format,
-                ):  # type: ignore
+                if replace:
+                    funcs, links = _locate_app_functions(cur)
+                    for fname in funcs:
+                        cur.execute(f'DROP FUNCTION IF EXISTS `{fname}`')
+                    for link in links:
+                        cur.execute(f'DROP LINK {link}')
+                for func in app.show_create_functions(replace=replace):  # type: ignore
                     cur.execute(func)
 
     app.register_functions = register_functions  # type: ignore
 
     def drop_functions(
         *connection_args: Any,
         **connection_kwargs: Any,
     ) -> None:
+        """Drop registered functions from database."""
         with connection.connect(*connection_args, **connection_kwargs) as conn:
             with conn.cursor() as cur:
-                for key in endpoints.keys():
-                    cur.execute(f'DROP FUNCTION IF EXISTS `{key.decode("utf8")}`')
+                funcs, links = _locate_app_functions(cur)
+                for fname in funcs:
+                    cur.execute(f'DROP FUNCTION IF EXISTS `{fname}`')
+                for link in links:
+                    cur.execute(f'DROP LINK {link}')
 
     app.drop_functions = drop_functions  # type: ignore
 
     async def call(
         name: str,
         data_in: io.BytesIO,
         data_out: io.BytesIO,
-        data_format: str = 'rowdat_1',
-        data_version: str = '1.0',
+        data_format: str = data_format,
+        data_version: str = data_version,
     ) -> None:
 
         async def receive() -> Dict[str, Any]:
             return dict(body=data_in.read())
 
         async def send(content: Dict[str, Any]) -> None:
             status = content.get('status', 200)
```

### Comparing `singlestoredb-1.0.2/singlestoredb/functions/ext/json.py` & `singlestoredb-1.0.3/singlestoredb/functions/ext/json.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/functions/ext/rowdat_1.py` & `singlestoredb-1.0.3/singlestoredb/functions/ext/rowdat_1.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/functions/signature.py` & `singlestoredb-1.0.3/singlestoredb/functions/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/usr/bin/env python3
 import datetime
 import inspect
 import numbers
 import os
 import re
 import string
-import textwrap
 import typing
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import TypeVar
 from typing import Union
-from urllib.parse import urljoin
 
 try:
     import numpy as np
     has_numpy = True
 except ImportError:
     has_numpy = False
 
@@ -607,16 +605,19 @@
         return f'RECORD({", ".join(item_dtypes)}){nullable}{default_clause}'
 
     return f'{sql_type_map[dtype]}{nullable}{default_clause}'
 
 
 def signature_to_sql(
     signature: Dict[str, Any],
-    base_url: Optional[str] = None,
+    url: Optional[str] = None,
     data_format: str = 'rowdat_1',
+    app_mode: str = 'remote',
+    link: Optional[str] = None,
+    replace: bool = False,
 ) -> str:
     '''
     Convert a dictionary function signature into SQL.
 
     Parameters
     ----------
     signature : Dict[str, Any]
@@ -642,41 +643,31 @@
     if signature.get('returns'):
         res = signature['returns']['sql']
         returns = f' RETURNS {res}'
 
     host = os.environ.get('SINGLESTOREDB_EXT_HOST', '127.0.0.1')
     port = os.environ.get('SINGLESTOREDB_EXT_PORT', '8000')
 
-    url = urljoin(base_url or f'https://{host}:{port}', signature['endpoint'])
+    if app_mode.lower() == 'remote':
+        url = url or f'https://{host}:{port}/invoke'
+    elif url is None:
+        raise ValueError('url can not be `None`')
 
     database = ''
     if signature.get('database'):
         database = escape_name(signature['database']) + '.'
 
-    replace = 'OR REPLACE ' if signature.get('replace') else ''
+    or_replace = 'OR REPLACE ' if (bool(signature.get('replace')) or replace) else ''
 
-    return (
-        f'CREATE {replace}EXTERNAL FUNCTION {database}{escape_name(signature["name"])}' +
-        '(' + ', '.join(args) + ')' + returns +
-        f' AS REMOTE SERVICE "{url}" FORMAT {data_format.upper()};'
-    )
-
-
-def func_to_env(func: Callable[..., Any]) -> str:
-    # TODO: multiple functions
-    signature = get_signature(func)
-    env_name = signature['environment']
-    replace = 'OR REPLACE ' if signature.get('replace') else ''
-    packages = ', '.join(escape_item(x, 'utf8') for x in signature.get('packages', []))
-    resources = ', '.join(escape_item(x, 'utf8') for x in signature.get('resources', []))
-    code = inspect.getsource(func)
+    link_str = ''
+    if link:
+        if not re.match(r'^[\w_]+$', link):
+            raise ValueError(f'invalid LINK name: {link}')
+        link_str = f' LINK {link}'
 
     return (
-        f'CREATE {replace}ENVIRONMENT {env_name} LANGUAGE PYTHON ' +
-        'USING EXPORTS ' + escape_name(func.__name__) + ' ' +
-        (f'\n    PACKAGES ({packages}) ' if packages else '') +
-        (f'\n    RESOURCES ({resources}) ' if resources else '') +
-        '\n    AS CLOUD SERVICE' +
-        '\n    BEGIN\n' +
-        textwrap.indent(code, '    ') +
-        '    END;'
+        f'CREATE {or_replace}EXTERNAL FUNCTION ' +
+        f'{database}{escape_name(signature["name"])}' +
+        '(' + ', '.join(args) + ')' + returns +
+        f' AS {app_mode.upper()} SERVICE "{url}" FORMAT {data_format.upper()}'
+        f'{link_str};'
     )
```

### Comparing `singlestoredb-1.0.2/singlestoredb/fusion/graphql.py` & `singlestoredb-1.0.3/singlestoredb/fusion/graphql.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/fusion/handler.py` & `singlestoredb-1.0.3/singlestoredb/fusion/handler.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/fusion/handlers/stage.py` & `singlestoredb-1.0.3/singlestoredb/fusion/handlers/stage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/fusion/handlers/utils.py` & `singlestoredb-1.0.3/singlestoredb/fusion/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/fusion/handlers/workspace.py` & `singlestoredb-1.0.3/singlestoredb/fusion/handlers/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/fusion/registry.py` & `singlestoredb-1.0.3/singlestoredb/fusion/registry.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/fusion/result.py` & `singlestoredb-1.0.3/singlestoredb/fusion/result.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/http/__init__.py` & `singlestoredb-1.0.3/singlestoredb/http/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/http/connection.py` & `singlestoredb-1.0.3/singlestoredb/http/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/management/billing_usage.py` & `singlestoredb-1.0.3/singlestoredb/management/billing_usage.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/management/cluster.py` & `singlestoredb-1.0.3/singlestoredb/management/cluster.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/management/manager.py` & `singlestoredb-1.0.3/singlestoredb/management/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,18 @@
         return False
 
 
 class Manager(object):
     """SingleStoreDB manager base class."""
 
     #: Management API version if none is specified.
-    default_version = 'v1'
+    default_version = config.get_option('management.version')
 
     #: Base URL if none is specified.
-    default_base_url = 'https://api.singlestore.com'
+    default_base_url = config.get_option('management.base_url')
 
     #: Object type
     obj_type = ''
 
     def __init__(
         self, access_token: Optional[str] = None, version: Optional[str] = None,
         base_url: Optional[str] = None, *, organization_id: Optional[str] = None,
```

### Comparing `singlestoredb-1.0.2/singlestoredb/management/organization.py` & `singlestoredb-1.0.3/singlestoredb/management/organization.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/management/region.py` & `singlestoredb-1.0.3/singlestoredb/management/region.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/management/utils.py` & `singlestoredb-1.0.3/singlestoredb/management/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/management/workspace.py` & `singlestoredb-1.0.3/singlestoredb/management/workspace.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/__init__.py` & `singlestoredb-1.0.3/singlestoredb/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/_auth.py` & `singlestoredb-1.0.3/singlestoredb/mysql/_auth.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/charset.py` & `singlestoredb-1.0.3/singlestoredb/mysql/charset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/connection.py` & `singlestoredb-1.0.3/singlestoredb/mysql/connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/constants/CLIENT.py` & `singlestoredb-1.0.3/singlestoredb/mysql/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/constants/COMMAND.py` & `singlestoredb-1.0.3/singlestoredb/mysql/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/constants/CR.py` & `singlestoredb-1.0.3/singlestoredb/mysql/constants/CR.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/constants/ER.py` & `singlestoredb-1.0.3/singlestoredb/mysql/constants/ER.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/converters.py` & `singlestoredb-1.0.3/singlestoredb/mysql/converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/cursors.py` & `singlestoredb-1.0.3/singlestoredb/mysql/cursors.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/err.py` & `singlestoredb-1.0.3/singlestoredb/mysql/err.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/optionfile.py` & `singlestoredb-1.0.3/singlestoredb/mysql/optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/protocol.py` & `singlestoredb-1.0.3/singlestoredb/mysql/protocol.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/__init__.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/base.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/base.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/conftest.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_DictCursor.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_DictCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_SSCursor.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_SSCursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_basic.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_connection.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_converters.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_cursor.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_cursor.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_issues.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_issues.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_load_local.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_load_local.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_nextset.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_nextset.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/test_optionfile.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/test_optionfile.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_capabilities.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_dbapi20.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py` & `singlestoredb-1.0.3/singlestoredb/mysql/tests/thirdparty/test_MySQLdb/test_MySQLdb_nonstandard.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/pytest.py` & `singlestoredb-1.0.3/singlestoredb/pytest.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/ext_funcs/__init__.py` & `singlestoredb-1.0.3/singlestoredb/tests/ext_funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test.sql` & `singlestoredb-1.0.3/singlestoredb/tests/test.sql`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_basics.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_config.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_connection.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_dbapi.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_exceptions.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_ext_func.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_ext_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,19 +61,21 @@
             if out.status_code == 200:
                 break
         except Exception:
             pass
         time.sleep(3)
         retries -= 1
 
-    app = create_app(ext_funcs)
+    app = create_app(
+        ext_funcs,
+        url=f'http://{HTTP_HOST}:{port}/invoke',
+        data_format=data_format,
+    )
     app.register_functions(
-        base_url=f'http://{HTTP_HOST}:{port}',
         database=database,
-        data_format=data_format,
     )
 
     with s2.connect(database=database) as conn:
         with conn.cursor() as cur:
             cur.execute('set global enable_external_functions=on')
             cur.execute('show functions')
             for item in list(cur):
```

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_ext_func_data.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_ext_func_data.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_fusion.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_fusion.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_http.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_management.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_plugin.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_results.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_types.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_udf.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,25 +408,14 @@
                               'RETURNS BIGINT NOT NULL'
 
         @udf(name='hello`_`world')
         def foo(x: int) -> int: ...
         assert to_sql(foo) == '`hello``_``world`(`x` BIGINT NOT NULL) ' \
                               'RETURNS BIGINT NOT NULL'
 
-        # Add database name
-        @udf(database='mydb')
-        def foo(x: int) -> int: ...
-        assert to_sql(foo) == '`mydb`.`foo`(`x` BIGINT NOT NULL) ' \
-                              'RETURNS BIGINT NOT NULL'
-
-        @udf(database='my`db')
-        def foo(x: int) -> int: ...
-        assert to_sql(foo) == '`my``db`.`foo`(`x` BIGINT NOT NULL) ' \
-                              'RETURNS BIGINT NOT NULL'
-
     def test_dtypes(self):
         assert dt.BOOL() == 'BOOL NULL'
         assert dt.BOOL(nullable=False) == 'BOOL NOT NULL'
         assert dt.BOOL(default=False) == 'BOOL NULL DEFAULT 0'
         assert dt.BOOL(default=True) == 'BOOL NULL DEFAULT 1'
         assert dt.BOOL(default='a') == 'BOOL NULL DEFAULT 1'
```

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/test_xdict.py` & `singlestoredb-1.0.3/singlestoredb/tests/test_xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/tests/utils.py` & `singlestoredb-1.0.3/singlestoredb/tests/utils.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/types.py` & `singlestoredb-1.0.3/singlestoredb/types.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/utils/config.py` & `singlestoredb-1.0.3/singlestoredb/utils/config.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/utils/convert_rows.py` & `singlestoredb-1.0.3/singlestoredb/utils/convert_rows.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/utils/mogrify.py` & `singlestoredb-1.0.3/singlestoredb/utils/mogrify.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/utils/results.py` & `singlestoredb-1.0.3/singlestoredb/utils/results.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb/utils/xdict.py` & `singlestoredb-1.0.3/singlestoredb/utils/xdict.py`

 * *Files identical despite different names*

### Comparing `singlestoredb-1.0.2/singlestoredb.egg-info/PKG-INFO` & `singlestoredb-1.0.3/singlestoredb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singlestoredb
-Version: 1.0.2
+Version: 1.0.3
 Summary: Interface to the SingleStoreDB database and workspace management APIs
 Home-page: https://github.com/singlestore-labs/singlestoredb-python
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `singlestoredb-1.0.2/singlestoredb.egg-info/SOURCES.txt` & `singlestoredb-1.0.3/singlestoredb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 singlestoredb/functions/decorator.py
 singlestoredb/functions/dtypes.py
 singlestoredb/functions/signature.py
 singlestoredb/functions/ext/__init__.py
 singlestoredb/functions/ext/arrow.py
 singlestoredb/functions/ext/asgi.py
 singlestoredb/functions/ext/json.py
+singlestoredb/functions/ext/mmap.py
 singlestoredb/functions/ext/rowdat_1.py
 singlestoredb/fusion/__init__.py
 singlestoredb/fusion/graphql.py
 singlestoredb/fusion/handler.py
 singlestoredb/fusion/registry.py
 singlestoredb/fusion/result.py
 singlestoredb/fusion/handlers/__init__.py
```

