# Comparing `tmp/sqldbclient-0.1.0.tar.gz` & `tmp/sqldbclient-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldbclient-0.1.0.tar", last modified: Thu Aug 17 23:30:53 2023, max compression
+gzip compressed data, was "sqldbclient-0.1.1.tar", last modified: Tue Apr  2 11:43:18 2024, max compression
```

## Comparing `sqldbclient-0.1.0.tar` & `sqldbclient-0.1.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.787087 sqldbclient-0.1.0/
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1055 2022-07-27 13:52:49.000000 sqldbclient-0.1.0/LICENSE
--rw-r--r--   0 yuakozhev   (501) staff       (20)    13496 2023-08-17 23:30:53.786342 sqldbclient-0.1.0/PKG-INFO
--rw-r--r--   0 yuakozhev   (501) staff       (20)    11418 2023-08-17 22:29:07.000000 sqldbclient-0.1.0/README.rst
--rw-r--r--   0 yuakozhev   (501) staff       (20)      917 2023-08-17 23:30:41.000000 sqldbclient-0.1.0/pyproject.toml
--rw-r--r--   0 yuakozhev   (501) staff       (20)       38 2023-08-17 23:30:53.787167 sqldbclient-0.1.0/setup.cfg
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1482 2023-08-17 23:30:41.000000 sqldbclient-0.1.0/setup.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.762373 sqldbclient-0.1.0/src/
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.766308 sqldbclient-0.1.0/src/sqldbclient/
--rw-r--r--   0 yuakozhev   (501) staff       (20)     2072 2023-08-17 22:17:02.000000 sqldbclient-0.1.0/src/sqldbclient/__init__.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.768008 sqldbclient-0.1.0/src/sqldbclient/db_inspector/
--rw-r--r--   0 yuakozhev   (501) staff       (20)      507 2023-08-17 12:23:15.000000 sqldbclient-0.1.0/src/sqldbclient/db_inspector/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     2106 2023-08-07 13:34:04.000000 sqldbclient-0.1.0/src/sqldbclient/db_inspector/db_inspector.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.768480 sqldbclient-0.1.0/src/sqldbclient/dialects/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-30 18:37:52.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/__init__.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.768978 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1347 2023-08-17 12:25:44.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/__init__.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.770295 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_factory/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-29 20:36:29.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_factory/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     2452 2022-12-30 11:13:44.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_factory/pg_info_queries.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     5820 2023-08-06 23:20:40.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_factory/sql_view_factory.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      806 2022-12-30 11:15:04.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_factory/view.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.771135 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_materializer/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-29 21:55:08.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_materializer/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     3523 2023-08-06 23:24:59.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_materializer/sql_view_materializer.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     4437 2023-08-06 23:31:55.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_materializer/sql_view_materializer_utils.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      852 2023-08-06 23:35:32.000000 sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/utils.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.771464 sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/
--rw-r--r--   0 yuakozhev   (501) staff       (20)      880 2023-08-17 12:49:35.000000 sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/__init__.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.771946 sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/sql_async_executor/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-28 20:40:13.000000 sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/sql_async_executor/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1804 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/sql_async_executor/sql_async_executor.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.772427 sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/sql_async_planner/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-28 20:30:52.000000 sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/sql_async_planner/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1161 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/sql_async_planner/sql_async_planner.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.773048 sqldbclient-0.1.0/src/sqldbclient/sql_engine_factory/
--rw-r--r--   0 yuakozhev   (501) staff       (20)      515 2023-08-17 13:54:42.000000 sqldbclient-0.1.0/src/sqldbclient/sql_engine_factory/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      686 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_engine_factory/sql_engine_factory.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.773607 sqldbclient-0.1.0/src/sqldbclient/sql_executor/
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1191 2023-08-17 13:57:07.000000 sqldbclient-0.1.0/src/sqldbclient/sql_executor/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     7075 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.774355 sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor_builder/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-28 18:55:00.000000 sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor_builder/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      231 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor_builder/parameter_not_specified_exception.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1606 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor_builder/sql_executor_builder.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.774740 sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor_config/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-28 18:23:41.000000 sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor_config/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1242 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor_config/sql_executor_config.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.775489 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/
--rw-r--r--   0 yuakozhev   (501) staff       (20)      382 2023-08-17 15:11:37.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      819 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/orm_config.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     6207 2023-08-07 12:02:36.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/sql_history_manager.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.775820 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-03 19:24:15.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/__init__.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.776139 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-03 19:25:17.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     2467 2023-08-06 23:39:13.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query/executed_sql_query.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.777202 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-03 19:26:33.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/__init__.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.781050 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-03 19:28:26.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      979 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/data_frame.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      907 2023-08-06 23:37:07.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/data_types.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1210 2022-12-03 21:53:45.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/executed_sql_query_result.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      525 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/parse_executed_sql_query_result.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.782585 sqldbclient-0.1.0/src/sqldbclient/sql_query_preparator/
--rw-r--r--   0 yuakozhev   (501) staff       (20)      294 2023-08-17 15:20:57.000000 sqldbclient-0.1.0/src/sqldbclient/sql_query_preparator/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      246 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_query_preparator/incorrect_sql_query_exception.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      386 2023-08-06 12:12:34.000000 sqldbclient-0.1.0/src/sqldbclient/sql_query_preparator/prepared_sql_query.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     3443 2023-08-17 15:26:31.000000 sqldbclient-0.1.0/src/sqldbclient/sql_query_preparator/sql_query_preparator.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.783568 sqldbclient-0.1.0/src/sqldbclient/sql_transaction_manager/
--rw-r--r--   0 yuakozhev   (501) staff       (20)      188 2023-08-17 15:22:22.000000 sqldbclient-0.1.0/src/sqldbclient/sql_transaction_manager/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      219 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/sql_transaction_manager/not_in_transaction_exception.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     3041 2023-08-06 23:09:55.000000 sqldbclient-0.1.0/src/sqldbclient/sql_transaction_manager/sql_transaction_manager.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.784350 sqldbclient-0.1.0/src/sqldbclient/utils/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-08-04 12:07:18.000000 sqldbclient-0.1.0/src/sqldbclient/utils/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      739 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/utils/deprecated.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1625 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/utils/log_decorators.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.785792 sqldbclient-0.1.0/src/sqldbclient/utils/pandas/
--rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-08-04 12:08:24.000000 sqldbclient-0.1.0/src/sqldbclient/utils/pandas/__init__.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     1140 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/utils/pandas/cursor_result_to_df.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      174 2023-08-16 17:50:02.000000 sqldbclient-0.1.0/src/sqldbclient/utils/pandas/full_display.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)      512 2023-08-06 22:53:32.000000 sqldbclient-0.1.0/src/sqldbclient/utils/pandas/parse_dates.py
--rw-r--r--   0 yuakozhev   (501) staff       (20)     3165 2023-08-16 17:47:01.000000 sqldbclient-0.1.0/src/sqldbclient/utils/pandas/set_full_display.py
-drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2023-08-17 23:30:53.767484 sqldbclient-0.1.0/src/sqldbclient.egg-info/
--rw-r--r--   0 yuakozhev   (501) staff       (20)    13496 2023-08-17 23:30:53.000000 sqldbclient-0.1.0/src/sqldbclient.egg-info/PKG-INFO
--rw-r--r--   0 yuakozhev   (501) staff       (20)     3575 2023-08-17 23:30:53.000000 sqldbclient-0.1.0/src/sqldbclient.egg-info/SOURCES.txt
--rw-r--r--   0 yuakozhev   (501) staff       (20)        1 2023-08-17 23:30:53.000000 sqldbclient-0.1.0/src/sqldbclient.egg-info/dependency_links.txt
--rw-r--r--   0 yuakozhev   (501) staff       (20)       65 2023-08-17 23:30:53.000000 sqldbclient-0.1.0/src/sqldbclient.egg-info/requires.txt
--rw-r--r--   0 yuakozhev   (501) staff       (20)       12 2023-08-17 23:30:53.000000 sqldbclient-0.1.0/src/sqldbclient.egg-info/top_level.txt
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.980594 sqldbclient-0.1.1/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1055 2022-07-27 13:52:49.000000 sqldbclient-0.1.1/LICENSE
+-rw-r--r--   0 yuakozhev   (501) staff       (20)    13351 2024-04-02 11:43:18.980240 sqldbclient-0.1.1/PKG-INFO
+-rw-r--r--   0 yuakozhev   (501) staff       (20)    11421 2024-04-02 11:01:51.000000 sqldbclient-0.1.1/README.rst
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      942 2024-04-02 11:40:03.000000 sqldbclient-0.1.1/pyproject.toml
+-rw-r--r--   0 yuakozhev   (501) staff       (20)       38 2024-04-02 11:43:18.980670 sqldbclient-0.1.1/setup.cfg
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1511 2024-04-02 11:41:08.000000 sqldbclient-0.1.1/setup.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.930675 sqldbclient-0.1.1/src/
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.934997 sqldbclient-0.1.1/src/sqldbclient/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     2072 2024-04-02 11:12:09.000000 sqldbclient-0.1.1/src/sqldbclient/__init__.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.936991 sqldbclient-0.1.1/src/sqldbclient/db_inspector/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      507 2023-08-17 12:23:15.000000 sqldbclient-0.1.1/src/sqldbclient/db_inspector/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     2106 2023-08-07 13:34:04.000000 sqldbclient-0.1.1/src/sqldbclient/db_inspector/db_inspector.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.937422 sqldbclient-0.1.1/src/sqldbclient/dialects/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-30 18:37:52.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/__init__.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.937951 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1347 2023-08-17 12:25:44.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/__init__.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.939122 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_factory/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-29 20:36:29.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_factory/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     2993 2024-04-02 08:25:01.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_factory/pg_info_queries.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     7156 2024-04-02 10:47:56.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_factory/sql_view_factory.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      910 2024-04-02 08:25:01.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_factory/view.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.940110 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_materializer/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-29 21:55:08.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_materializer/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     3649 2024-04-02 10:47:21.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_materializer/sql_view_materializer.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     5402 2024-04-02 10:47:13.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_materializer/sql_view_materializer_utils.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      852 2023-08-06 23:35:32.000000 sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/utils.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.940434 sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      880 2023-08-17 12:49:35.000000 sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/__init__.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.942306 sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/sql_async_executor/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-28 20:40:13.000000 sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/sql_async_executor/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1804 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/sql_async_executor/sql_async_executor.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.944168 sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/sql_async_planner/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-28 20:30:52.000000 sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/sql_async_planner/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1161 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/sql_async_planner/sql_async_planner.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.946642 sqldbclient-0.1.1/src/sqldbclient/sql_engine_factory/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      515 2023-08-17 13:54:42.000000 sqldbclient-0.1.1/src/sqldbclient/sql_engine_factory/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      686 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_engine_factory/sql_engine_factory.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.948313 sqldbclient-0.1.1/src/sqldbclient/sql_executor/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1191 2023-08-17 13:57:07.000000 sqldbclient-0.1.1/src/sqldbclient/sql_executor/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     7075 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.949099 sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor_builder/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-28 18:55:00.000000 sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor_builder/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      231 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor_builder/parameter_not_specified_exception.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1606 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor_builder/sql_executor_builder.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.950677 sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor_config/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-28 18:23:41.000000 sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor_config/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1242 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor_config/sql_executor_config.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.953905 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      382 2023-08-17 15:11:37.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      819 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/orm_config.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     6207 2023-08-07 12:02:36.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/sql_history_manager.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.957955 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-03 19:24:15.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/__init__.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.958329 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-03 19:25:17.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     2467 2023-12-12 15:40:43.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query/executed_sql_query.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.964899 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-03 19:26:33.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/__init__.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.971281 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-12-03 19:28:26.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      979 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/data_frame.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      907 2023-08-06 23:37:07.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/data_types.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1210 2022-12-03 21:53:45.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/executed_sql_query_result.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      525 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/parse_executed_sql_query_result.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.975671 sqldbclient-0.1.1/src/sqldbclient/sql_query_preparator/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      294 2023-08-17 15:20:57.000000 sqldbclient-0.1.1/src/sqldbclient/sql_query_preparator/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      246 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_query_preparator/incorrect_sql_query_exception.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      386 2023-08-06 12:12:34.000000 sqldbclient-0.1.1/src/sqldbclient/sql_query_preparator/prepared_sql_query.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     3443 2023-08-17 15:26:31.000000 sqldbclient-0.1.1/src/sqldbclient/sql_query_preparator/sql_query_preparator.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.976846 sqldbclient-0.1.1/src/sqldbclient/sql_transaction_manager/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      188 2023-08-17 15:22:22.000000 sqldbclient-0.1.1/src/sqldbclient/sql_transaction_manager/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      219 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/sql_transaction_manager/not_in_transaction_exception.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     3041 2023-08-06 23:09:55.000000 sqldbclient-0.1.1/src/sqldbclient/sql_transaction_manager/sql_transaction_manager.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.977735 sqldbclient-0.1.1/src/sqldbclient/utils/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-08-04 12:07:18.000000 sqldbclient-0.1.1/src/sqldbclient/utils/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      739 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/utils/deprecated.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1625 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/utils/log_decorators.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.979050 sqldbclient-0.1.1/src/sqldbclient/utils/pandas/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        0 2022-08-04 12:08:24.000000 sqldbclient-0.1.1/src/sqldbclient/utils/pandas/__init__.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     1140 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/utils/pandas/cursor_result_to_df.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      174 2023-08-16 17:50:02.000000 sqldbclient-0.1.1/src/sqldbclient/utils/pandas/full_display.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)      512 2023-08-06 22:53:32.000000 sqldbclient-0.1.1/src/sqldbclient/utils/pandas/parse_dates.py
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     3165 2023-08-16 17:47:01.000000 sqldbclient-0.1.1/src/sqldbclient/utils/pandas/set_full_display.py
+drwxr-xr-x   0 yuakozhev   (501) staff       (20)        0 2024-04-02 11:43:18.979471 sqldbclient-0.1.1/src/sqldbclient.egg-info/
+-rw-r--r--   0 yuakozhev   (501) staff       (20)    13351 2024-04-02 11:43:18.000000 sqldbclient-0.1.1/src/sqldbclient.egg-info/PKG-INFO
+-rw-r--r--   0 yuakozhev   (501) staff       (20)     3575 2024-04-02 11:43:18.000000 sqldbclient-0.1.1/src/sqldbclient.egg-info/SOURCES.txt
+-rw-r--r--   0 yuakozhev   (501) staff       (20)        1 2024-04-02 11:43:18.000000 sqldbclient-0.1.1/src/sqldbclient.egg-info/dependency_links.txt
+-rw-r--r--   0 yuakozhev   (501) staff       (20)       65 2024-04-02 11:43:18.000000 sqldbclient-0.1.1/src/sqldbclient.egg-info/requires.txt
+-rw-r--r--   0 yuakozhev   (501) staff       (20)       12 2024-04-02 11:43:18.000000 sqldbclient-0.1.1/src/sqldbclient.egg-info/top_level.txt
```

### Comparing `sqldbclient-0.1.0/LICENSE` & `sqldbclient-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/PKG-INFO` & `sqldbclient-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqldbclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: A SQL client software package, mainly for use in Jupyter Notebook environment
 Home-page: https://github.com/YuriyKozhev/SqlDBClient
 Author: Yuriy Kozhev
 Author-email: Yuriy Kozhev <yuriy.kozhev@gmail.com>
 License: Copyright (c) 2022 Yuriy Kozhev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,27 +20,28 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/YuriyKozhev/SqlDBClient
-Project-URL: Documentation, https://sqldbclient.readthedocs.io/
-Project-URL: Release Notes, https://sqldbclient.readthedocs.io/en/latest/changes.html
-Project-URL: Source, https://github.com/YuriyKozhev/sqldbclient
-Project-URL: Tracker, https://github.com/YuriyKozhev/sqldbclient/issues
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: jupyter
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: sqlalchemy
+Requires-Dist: sqlparse
+Provides-Extra: jupyter
+Requires-Dist: jupyter; extra == "jupyter"
+Requires-Dist: notebook; extra == "jupyter"
+Requires-Dist: ipykernel; extra == "jupyter"
 
 Sql DB Client
 =============
 
 |packageversion|_
 |docs|_
 |totaldownloads|_
@@ -83,15 +84,15 @@
 further information about this project.
 
 
 Quick Start
 -----------
 
 The latest released version of **Sql DB Client** can be obtained from the `Python Package
-Index (PyPI) <https://pypi.org/project/sqlparse/>`_.
+Index (PyPI) <https://pypi.org/project/sqldbclient/>`_.
 You can install `sqldbclient` using `pip`:
 
 .. code-block:: sh
 
    $ pip install sqldbclient
 
 ``SqlExecutor``, main tool to execute SQL queries,
```

### Comparing `sqldbclient-0.1.0/README.rst` & `sqldbclient-0.1.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 further information about this project.
 
 
 Quick Start
 -----------
 
 The latest released version of **Sql DB Client** can be obtained from the `Python Package
-Index (PyPI) <https://pypi.org/project/sqlparse/>`_.
+Index (PyPI) <https://pypi.org/project/sqldbclient/>`_.
 You can install :mod:`sqldbclient` using :command:`pip`:
 
 .. code-block:: sh
 
    $ pip install sqldbclient
 
 ``SqlExecutor``, main tool to execute SQL queries,
```

### Comparing `sqldbclient-0.1.0/pyproject.toml` & `sqldbclient-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
     "setuptools>=42.0.0",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'sqldbclient'
-version = "0.1.0"
 authors = [
     { name="Yuriy Kozhev", email="yuriy.kozhev@gmail.com" },
 ]
 description = "A SQL client software package, mainly for use in Jupyter Notebook environment"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
 classifiers = [
@@ -20,14 +19,18 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pandas",
     "sqlalchemy",
     "sqlparse"
 ]
+dynamic = [
+    "readme",
+    "version",
+]
 
 [project-urls]
 Homepage = "https://github.com/YuriyKozhev/SqlDBClient"
 Documentation = "https://sqldbclient.readthedocs.io/"
 "Release Notes" = "https://sqldbclient.readthedocs.io/en/latest/changes.html"
 Source = "https://github.com/YuriyKozhev/sqldbclient"
 Tracker = "https://github.com/YuriyKozhev/sqldbclient/issues"
```

### Comparing `sqldbclient-0.1.0/setup.py` & `sqldbclient-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'pandas',
     'sqlalchemy',
     'sqlparse',
 )
 
 setuptools.setup(
     name="sqldbclient",
-    version="0.1.0",
+    version="0.1.1",
     author="Yuriy Kozhev",
     author_email="yuriy.kozhev@gmail.com",
     description="A SQL client software package, mainly for use in Jupyter Notebook environment",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/YuriyKozhev/SqlDBClient",
     project_urls={
@@ -37,8 +37,9 @@
     install_requires=dependencies,
     extras_require={
         'jupyter': ('jupyter', 'notebook', 'ipykernel'),
     },
     license='MIT',
     license_files=('LICENSE',),
     platforms=['any'],
+    readme=long_description,
 )
```

### Comparing `sqldbclient-0.1.0/src/sqldbclient/__init__.py` & `sqldbclient-0.1.1/src/sqldbclient/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 `MIT License <https://opensource.org/license/mit/>`_.
 
 Visit the project page at https://github.com/YuriyKozhev/SqlDbClient for
 further information about this project.
 
 """
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import logging
 
 from sqldbclient.sql_history_manager import SqlHistoryManager
 from sqldbclient.sql_query_preparator import SqlQueryPreparator
 from sqldbclient.sql_transaction_manager import SqlTransactionManager
```

### Comparing `sqldbclient-0.1.0/src/sqldbclient/db_inspector/db_inspector.py` & `sqldbclient-0.1.1/src/sqldbclient/db_inspector/db_inspector.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/__init__.py` & `sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_factory/pg_info_queries.py` & `sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_factory/pg_info_queries.py`

 * *Files 26% similar despite different names*

```diff
@@ -64,7 +64,23 @@
     SELECT 
         schemaname AS schema, 
         indexname AS name, 
         indexdef AS definition
     FROM pg_indexes
     WHERE tablename = '{name}' AND schemaname = '{schema}'
 '''
+
+PG_OBJECT_DESCRIPTIONS_TEMPLATE = '''
+    SELECT
+        s.nspname AS table_schema,
+        t.relname AS table_name,
+        pg_catalog.obj_description(t.oid) AS table_description,
+        json_object_agg(a.attname, pg_catalog.col_description(t.oid,a.attnum)) AS col_descriptions
+    FROM pg_attribute a
+      JOIN pg_class t ON a.attrelid = t.oid
+      JOIN pg_namespace s ON t.relnamespace = s.oid
+    WHERE a.attnum > 0 
+      AND NOT a.attisdropped
+      AND t.relname = '{name}'
+      AND s.nspname = '{schema}'
+    GROUP BY 1,2,3
+'''
```

### Comparing `sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_factory/sql_view_factory.py` & `sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_factory/sql_view_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
-from typing import List
+from typing import List, Dict, Tuple, Optional
 
 import pandas as pd
 
 from sqldbclient.dialects.postgresql.sql_view_factory.view import View, ViewType
 from sqldbclient.dialects.postgresql.sql_view_factory.pg_info_queries import PG_VIEWS_INFO_TEMPLATE, \
     PG_OBJECT_DEPENDENCIES_TEMPLATE, PG_OBJECT_INDEXES_TEMPLATE, PG_MATVIEWS_INFO_TEMPLATE, \
-    PG_OBJECT_PRIVILEGES_TEMPLATE
+    PG_OBJECT_PRIVILEGES_TEMPLATE, PG_OBJECT_DESCRIPTIONS_TEMPLATE
 from sqldbclient.sql_executor import SqlExecutor
 
 logger = logging.getLogger(__name__)
 
 
 def pre_traverse(name: str, schema: str, sql_executor: SqlExecutor) -> pd.DataFrame:
     """Collects object dependencies, dependencies of its dependencies, and etc.
@@ -83,31 +83,39 @@
     to be able to fully restore them in database, if necessary.
     """
     def __init__(self, view_name: str, view_schema: str, sql_executor: SqlExecutor):
         self.name = view_name
         self.schema = view_schema
         self.sql_executor = sql_executor
         self.parameters = dict(name=view_name, schema=view_schema)
+        self._cached_views: Optional[Dict[Tuple[str, str], View]] = None
 
     def _get_indexes(self) -> None:
         df = self.sql_executor.execute(PG_OBJECT_INDEXES_TEMPLATE.format(name=self.name, schema=self.schema))
         self.parameters['indexes'] = list(df.to_dict(orient='index').values())
 
     def _get_dependant_objects(self) -> None:
         dependencies = extract_dependant_objects(self.name, self.schema, self.sql_executor)
-        dependant_objects = dependencies.apply(
-            lambda row: SqlViewFactory(row['dependent_view'], row['dependent_schema'], self.sql_executor).create(),
-            axis=1
-        ).values.tolist()
+        dependant_objects = []
+        for _, row in dependencies.iterrows():
+            obj_factory = SqlViewFactory(row['dependent_view'], row['dependent_schema'], self.sql_executor)
+            obj_factory._cached_views = self._cached_views
+            obj = obj_factory.create()
+            dependant_objects.append(obj)
         self.parameters['dependant_objects'] = dependant_objects
 
     def _get_privileges(self) -> None:
         df = self.sql_executor.execute(PG_OBJECT_PRIVILEGES_TEMPLATE.substitute(name=self.name, schema=self.schema))
         self.parameters.update(df.set_index('grantee').to_dict())
 
+    def _get_descriptions(self) -> None:
+        df = self.sql_executor.execute(PG_OBJECT_DESCRIPTIONS_TEMPLATE.format(name=self.name, schema=self.schema))
+        self.parameters['table_description'] = df.iloc[0]['table_description']
+        self.parameters['col_descriptions'] = df.iloc[0]['col_descriptions']
+
     @staticmethod
     def _extract_main_parameters(result: pd.DataFrame) -> dict:
         if len(result) > 1:
             raise Exception('Unexpected error while extracting main view parameters')
         renamed = result.rename(columns={
             'viewowner': 'owner',
             'matviewowner': 'owner',
@@ -131,13 +139,29 @@
             raise Exception(f'View object "{self.schema}"."{self.name}" not found')
 
     def create(self) -> View:
         """Creates View object with all necessary information.
 
         :return: View object
         """
+        # None when called from user code, Dict when called within this class
+        if self._cached_views is None:
+            self._cached_views = {}
+
+        if (self.schema, self.name) in self._cached_views:
+            logger.info(f'Used cached version of View with schema = "{self.schema}" and name = "{self.name}"')
+            return self._cached_views[(self.schema, self.name)]
+
         self._get_main_parameters()
         self._get_privileges()
         self._get_dependant_objects()
         self._get_indexes()
+        self._get_descriptions()
         view_object = View(**self.parameters)
+
+        # cache will be used by non-direct and secondary parents of the View
+        self._cached_views[(self.schema, self.name)] = view_object
+        # when View is created there is no need to store reference to cache
+        # moreover, cache should be invalidated when user use the same SqlViewFactory another time
+        self._cached_views = None
+
         return view_object
```

### Comparing `sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_factory/view.py` & `sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_factory/view.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,12 +17,14 @@
     owner: str
     definition: str = field(repr=False)
     privileges: Dict[str, List[str]] = field(repr=False)
     dependant_objects: List['View'] = field(repr=False)
     dependant_objects_number: int = field(init=False)
     indexes: List[Dict[str, str]] = field(repr=False)
     indexes_number: int = field(init=False)
+    table_description: str = field(repr=False)
+    col_descriptions: Dict[str, str] = field(repr=False)
 
     def __post_init__(self):
         self.full_name = f'"{self.schema}"."{self.name}"'
         self.dependant_objects_number = len(self.dependant_objects)
         self.indexes_number = len(self.indexes)
```

### Comparing `sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_materializer/sql_view_materializer.py` & `sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_materializer/sql_view_materializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,17 +48,19 @@
         new_value = getattr(self.view, field.name)
         if existing_value == new_value:
             return
         logger.info(f'Found different value for field: {field.name}')
 
         if field.name in ['schema', 'name', 'full_name']:
             raise Exception('Unexpected error')
-        if field.name in ['dependant_objects', 'dependant_objects_number', 'indexes']:
+        if field.name in ['dependant_objects', 'dependant_objects_number', 'indexes', 'indexes_number']:
             logger.warning(f'{field.name} cannot be changed')
             return
+        if field.name in ('table_description', 'col_descriptions'):
+            raise NotImplementedError()
 
         if field.name == 'privileges':
             SqlViewMaterializerUtils(self.view, self.sql_executor).set_privileges()
         elif field.name == 'owner':
             SqlViewMaterializerUtils(self.view, self.sql_executor).set_owner()
         elif field.name in ['definition', 'view_type']:
             logger.warning(f'To change {field.name} view {self.view.full_name} will be fully recreated')
```

### Comparing `sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/sql_view_materializer/sql_view_materializer_utils.py` & `sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/sql_view_materializer/sql_view_materializer_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,19 +34,39 @@
         for grantee, privileges in self.view.privileges.items():
             for privilege in privileges:
                 self.sql_executor.execute(f"""
                     GRANT {privilege} ON {self.view.full_name} TO {grantee};
                 """)
         logger.info(f'View {self.view.full_name} privileges set')
 
+    def set_descriptions(self) -> None:
+        """Sets privileges"""
+        if self.view.table_description is not None:
+            if self.view.view_type == ViewType.REGULAR_VIEW:
+                self.sql_executor.execute(f"""
+                    COMMENT ON VIEW {self.view.full_name} IS '{self.view.table_description}';
+                """)
+            elif self.view.view_type == ViewType.MATERIALIZED_VIEW:
+                self.sql_executor.execute(f"""
+                    COMMENT ON MATERIALIZED VIEW {self.view.full_name} IS '{self.view.table_description}';
+                """)
+            else:
+                raise Exception('Unexpected error')
+        for col, col_description in self.view.col_descriptions.items():
+            if col_description is not None:
+                self.sql_executor.execute(f"""
+                    COMMENT ON COLUMN {self.view.full_name}.{col} IS '{col_description}';
+                """)
+
     def restore(self) -> None:
         """Fully restores object in database"""
         self.create()
         self.set_owner()
         self.set_privileges()
+        self.set_descriptions()
 
     def drop(self) -> None:
         """Drops database object"""
         if self.view.view_type == ViewType.REGULAR_VIEW:
             self.sql_executor.execute(f'DROP VIEW {self.view.full_name}')
         elif self.view.view_type == ViewType.MATERIALIZED_VIEW:
             self.sql_executor.execute(f'DROP MATERIALIZED VIEW {self.view.full_name}')
```

### Comparing `sqldbclient-0.1.0/src/sqldbclient/dialects/postgresql/utils.py` & `sqldbclient-0.1.1/src/sqldbclient/dialects/postgresql/utils.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/__init__.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/sql_async_executor/sql_async_executor.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/sql_async_executor/sql_async_executor.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_asyncio/sql_async_planner/sql_async_planner.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_asyncio/sql_async_planner/sql_async_planner.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_engine_factory/__init__.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_engine_factory/__init__.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_engine_factory/sql_engine_factory.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_engine_factory/sql_engine_factory.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_executor/__init__.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor_builder/sql_executor_builder.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor_builder/sql_executor_builder.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_executor/sql_executor_config/sql_executor_config.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_executor/sql_executor_config/sql_executor_config.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/orm_config.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/orm_config.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/sql_history_manager.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/sql_history_manager.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query/executed_sql_query.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query/executed_sql_query.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/data_frame.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/data_frame.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/data_types.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/custom_sqlalchemy_types/data_types.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/executed_sql_query_result.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/executed_sql_query_result.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/parse_executed_sql_query_result.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_history_manager/tables/executed_sql_query_result/parse_executed_sql_query_result.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_query_preparator/sql_query_preparator.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_query_preparator/sql_query_preparator.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/sql_transaction_manager/sql_transaction_manager.py` & `sqldbclient-0.1.1/src/sqldbclient/sql_transaction_manager/sql_transaction_manager.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/utils/deprecated.py` & `sqldbclient-0.1.1/src/sqldbclient/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/utils/log_decorators.py` & `sqldbclient-0.1.1/src/sqldbclient/utils/log_decorators.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/utils/pandas/cursor_result_to_df.py` & `sqldbclient-0.1.1/src/sqldbclient/utils/pandas/cursor_result_to_df.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/utils/pandas/parse_dates.py` & `sqldbclient-0.1.1/src/sqldbclient/utils/pandas/parse_dates.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient/utils/pandas/set_full_display.py` & `sqldbclient-0.1.1/src/sqldbclient/utils/pandas/set_full_display.py`

 * *Files identical despite different names*

### Comparing `sqldbclient-0.1.0/src/sqldbclient.egg-info/PKG-INFO` & `sqldbclient-0.1.1/src/sqldbclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqldbclient
-Version: 0.1.0
+Version: 0.1.1
 Summary: A SQL client software package, mainly for use in Jupyter Notebook environment
 Home-page: https://github.com/YuriyKozhev/SqlDBClient
 Author: Yuriy Kozhev
 Author-email: Yuriy Kozhev <yuriy.kozhev@gmail.com>
 License: Copyright (c) 2022 Yuriy Kozhev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,27 +20,28 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/YuriyKozhev/SqlDBClient
-Project-URL: Documentation, https://sqldbclient.readthedocs.io/
-Project-URL: Release Notes, https://sqldbclient.readthedocs.io/en/latest/changes.html
-Project-URL: Source, https://github.com/YuriyKozhev/sqldbclient
-Project-URL: Tracker, https://github.com/YuriyKozhev/sqldbclient/issues
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: jupyter
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: sqlalchemy
+Requires-Dist: sqlparse
+Provides-Extra: jupyter
+Requires-Dist: jupyter; extra == "jupyter"
+Requires-Dist: notebook; extra == "jupyter"
+Requires-Dist: ipykernel; extra == "jupyter"
 
 Sql DB Client
 =============
 
 |packageversion|_
 |docs|_
 |totaldownloads|_
@@ -83,15 +84,15 @@
 further information about this project.
 
 
 Quick Start
 -----------
 
 The latest released version of **Sql DB Client** can be obtained from the `Python Package
-Index (PyPI) <https://pypi.org/project/sqlparse/>`_.
+Index (PyPI) <https://pypi.org/project/sqldbclient/>`_.
 You can install `sqldbclient` using `pip`:
 
 .. code-block:: sh
 
    $ pip install sqldbclient
 
 ``SqlExecutor``, main tool to execute SQL queries,
```

### Comparing `sqldbclient-0.1.0/src/sqldbclient.egg-info/SOURCES.txt` & `sqldbclient-0.1.1/src/sqldbclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

