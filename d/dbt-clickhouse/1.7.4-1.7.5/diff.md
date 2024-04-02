# Comparing `tmp/dbt-clickhouse-1.7.4.tar.gz` & `tmp/dbt-clickhouse-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickhouse-1.7.4.tar", last modified: Sat Mar 23 10:44:04 2024, max compression
+gzip compressed data, was "dbt-clickhouse-1.7.5.tar", last modified: Tue Apr  2 06:29:19 2024, max compression
```

## Comparing `dbt-clickhouse-1.7.4.tar` & `dbt-clickhouse-1.7.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.948298 dbt-clickhouse-1.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23358 2024-03-23 10:44:04.948298 dbt-clickhouse-1.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22383 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.936298 dbt-clickhouse-1.7.4/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.936298 dbt-clickhouse-1.7.4/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.944298 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/dbclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/nativeclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.936298 dbt-clickhouse-1.7.4/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.944298 dbt-clickhouse-1.7.4/dbt/include/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.944298 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.944298 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/column_spec_ddl.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.944298 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/dictionary.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/distributed_table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.944298 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/materialized_view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/s3.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/view.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/persist_docs.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.944298 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/schema_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/schema_tests/relationships.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.948298 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/utils/datatypes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/utils/utils.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 10:44:04.948298 dbt-clickhouse-1.7.4/dbt_clickhouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23358 2024-03-23 10:44:04.000000 dbt-clickhouse-1.7.4/dbt_clickhouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-23 10:44:04.000000 dbt-clickhouse-1.7.4/dbt_clickhouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 10:44:04.000000 dbt-clickhouse-1.7.4/dbt_clickhouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-23 10:44:04.000000 dbt-clickhouse-1.7.4/dbt_clickhouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-23 10:44:04.000000 dbt-clickhouse-1.7.4/dbt_clickhouse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-23 10:44:04.948298 dbt-clickhouse-1.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-03-23 10:44:02.000000 dbt-clickhouse-1.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23390 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22383 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.823651 dbt-clickhouse-1.7.5/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.823651 dbt-clickhouse-1.7.5/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16052 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/dbclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/nativeclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.823651 dbt-clickhouse-1.7.5/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/column_spec_ddl.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/dictionary.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/distributed_table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     7566 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    11323 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/s3.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/persist_docs.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.831651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/schema_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/schema_tests/relationships.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/datatypes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/utils.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23390 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 06:29:19.000000 dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 06:29:19.835651 dbt-clickhouse-1.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-02 06:29:14.000000 dbt-clickhouse-1.7.5/setup.py
```

### Comparing `dbt-clickhouse-1.7.4/LICENSE` & `dbt-clickhouse-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/PKG-INFO` & `dbt-clickhouse-1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.7.4
+Version: 1.7.5
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: clickhouse-connect>=0.6.22
 Requires-Dist: clickhouse-driver>=0.2.6
+Requires-Dist: setuptools>=0.69
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ClickHouse/dbt-clickhouse/master/etc/chdbt.png" alt="clickhouse dbt logo" width="300"/>
 </p>
 
 # dbt-clickhouse
```

### Comparing `dbt-clickhouse-1.7.4/README.md` & `dbt-clickhouse-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/__init__.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/cache.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/column.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/connections.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/credentials.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/dbclient.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/dbclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,28 @@
     if driver == 'native':
         try:
             import clickhouse_driver  # noqa
 
             from dbt.adapters.clickhouse.nativeclient import ChNativeClient
 
             return ChNativeClient(credentials)
-        except ImportError:
+        except ImportError as ex:
             raise FailedToConnectError(
                 'Native adapter required but package clickhouse-driver is not installed'
-            )
+            ) from ex
     try:
         import clickhouse_connect  # noqa
 
         from dbt.adapters.clickhouse.httpclient import ChHttpClient
 
         return ChHttpClient(credentials)
-    except ImportError:
+    except ImportError as ex:
         raise FailedToConnectError(
             'HTTP adapter required but package clickhouse-connect is not installed'
-        )
+        ) from ex
 
 
 class ChRetryableException(Exception):
     pass
 
 
 class ChClientWrapper(ABC):
@@ -146,15 +146,16 @@
         pass
 
     @abstractmethod
     def _server_version(self):
         pass
 
     def update_model_settings(self, model_settings: Dict[str, str], materialization_type: str):
-        model_settings_to_add = copy.deepcopy(self._model_settings[materialization_type])
+        settings = self._model_settings.get(materialization_type, {})
+        model_settings_to_add = copy.deepcopy(settings)
         model_settings_to_add.update(self._model_settings['general'])
         for key, value in model_settings_to_add.items():
             if key not in model_settings:
                 model_settings[key] = value
 
     def _check_lightweight_deletes(self, requested: bool):
         lw_deletes, lw_read_only = self.get_ch_setting(LW_DELETE_SETTING)
```

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/errors.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/errors.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/httpclient.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/httpclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/impl.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/nativeclient.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/nativeclient.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/relation.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/adapters/clickhouse/util.py` & `dbt-clickhouse-1.7.5/dbt/adapters/clickhouse/util.py`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/adapters/apply_grants.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/adapters/relation.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/adapters.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/catalog.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/column_spec_ddl.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/column_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/dictionary.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/dictionary.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/distributed_table.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/distributed_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/distributed_incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/incremental/is_incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/materialized_view.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/s3.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/s3.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/seed.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/snapshot.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/table.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/materializations/view.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/persist_docs.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt/include/clickhouse/macros/utils/utils.sql` & `dbt-clickhouse-1.7.5/dbt/include/clickhouse/macros/utils/utils.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/dbt_clickhouse.egg-info/PKG-INFO` & `dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-clickhouse
-Version: 1.7.4
+Version: 1.7.5
 Summary: The Clickhouse plugin for dbt (data build tool)
 Home-page: https://github.com/ClickHouse/dbt-clickhouse
 Author: ClickHouse Inc.
 Author-email: guy@clickhouse.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: clickhouse-connect>=0.6.22
 Requires-Dist: clickhouse-driver>=0.2.6
+Requires-Dist: setuptools>=0.69
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/ClickHouse/dbt-clickhouse/master/etc/chdbt.png" alt="clickhouse dbt logo" width="300"/>
 </p>
 
 # dbt-clickhouse
```

### Comparing `dbt-clickhouse-1.7.4/dbt_clickhouse.egg-info/SOURCES.txt` & `dbt-clickhouse-1.7.5/dbt_clickhouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-clickhouse-1.7.4/setup.py` & `dbt-clickhouse-1.7.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
             'include/clickhouse/macros/**/*.sql',
         ]
     },
     install_requires=[
         f'dbt-core~={dbt_version}',
         'clickhouse-connect>=0.6.22',
         'clickhouse-driver>=0.2.6',
+        'setuptools>=0.69',
     ],
     python_requires=">=3.8",
     platforms='any',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: Microsoft :: Windows',
```

