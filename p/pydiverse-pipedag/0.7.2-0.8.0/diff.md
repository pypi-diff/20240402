# Comparing `tmp/pydiverse_pipedag-0.7.2.tar.gz` & `tmp/pydiverse_pipedag-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse_pipedag-0.7.2.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.8.0.tar", max compression
```

## Comparing `pydiverse_pipedag-0.7.2.tar` & `pydiverse_pipedag-0.8.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1517 2024-03-25 09:52:33.455887 pydiverse_pipedag-0.7.2/LICENSE
--rw-r--r--   0        0        0     5512 2024-03-25 09:52:33.455887 pydiverse_pipedag-0.7.2/docs/package/README.md
--rw-r--r--   0        0        0     3912 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/pyproject.toml
--rw-r--r--   0        0        0       13 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      515 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      857 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       97 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     6613 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0      393 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/__init__.py
--rw-r--r--   0        0        0     6097 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/base.py
--rw-r--r--   0        0        0    13599 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/database.py
--rw-r--r--   0        0        0     2756 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/filelock.py
--rw-r--r--   0        0        0      769 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/nolock.py
--rw-r--r--   0        0        0     3983 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/zookeeper.py
--rw-r--r--   0        0        0      233 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    28594 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0      108 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/cache/__init__.py
--rw-r--r--   0        0        0     3455 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/cache/base.py
--rw-r--r--   0        0        0     6892 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/cache/parquet.py
--rw-r--r--   0        0        0     6757 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0      157 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/__init__.py
--rw-r--r--   0        0        0    40062 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/ddl.py
--rw-r--r--   0        0        0      187 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
--rw-r--r--   0        0        0     3926 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
--rw-r--r--   0        0        0     9233 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
--rw-r--r--   0        0        0    10439 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
--rw-r--r--   0        0        0     5345 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
--rw-r--r--   0        0        0    27007 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/hooks.py
--rw-r--r--   0        0        0     4617 2024-03-25 09:52:33.459887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/reflection.py
--rw-r--r--   0        0        0    54570 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/sql.py
--rw-r--r--   0        0        0       81 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     8887 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/util/dtype.py
--rw-r--r--   0        0        0      433 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0    10203 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    27793 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      311 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0    22345 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/config.py
--rw-r--r--   0        0        0    20648 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     4294 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     8035 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     8392 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      135 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/debug/__init__.py
--rw-r--r--   0        0        0      368 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      654 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     3133 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/engine/dask.py
--rw-r--r--   0        0        0     7269 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1388 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/management/__init__.py
--rw-r--r--   0        0        0      620 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/management/cli.py
--rw-r--r--   0        0        0        0 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/management/commands/__init__.py
--rw-r--r--   0        0        0     1741 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/management/commands/clear_metadata.py
--rw-r--r--   0        0        0     2744 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/management/commands/delete_schemas.py
--rw-r--r--   0        0        0      182 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     1642 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0    12330 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0    30769 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2921 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/debug.py
--rw-r--r--   0        0        0     3837 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/details.py
--rw-r--r--   0        0        0     2074 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    20861 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0      213 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0     9273 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/computation_tracing.py
--rw-r--r--   0        0        0     2061 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1681 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      944 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1129 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/hashing.py
--rw-r--r--   0        0        0     3816 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     7992 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     4812 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/json.py
--rw-r--r--   0        0        0     1377 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     2847 2024-03-25 09:52:33.463887 pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/structlog.py
--rw-r--r--   0        0        0     7394 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-04-02 08:29:11.021852 pydiverse_pipedag-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5483 2024-04-02 08:29:11.021852 pydiverse_pipedag-0.8.0/docs/package/README.md
+-rw-r--r--   0        0        0     3912 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      515 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      857 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       97 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     6613 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0      393 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/__init__.py
+-rw-r--r--   0        0        0     6097 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/base.py
+-rw-r--r--   0        0        0    13599 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/database.py
+-rw-r--r--   0        0        0     2756 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/filelock.py
+-rw-r--r--   0        0        0      769 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/nolock.py
+-rw-r--r--   0        0        0     3983 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/zookeeper.py
+-rw-r--r--   0        0        0      233 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    30207 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0      108 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/__init__.py
+-rw-r--r--   0        0        0     3455 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/base.py
+-rw-r--r--   0        0        0     6892 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/parquet.py
+-rw-r--r--   0        0        0     6757 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0      157 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/__init__.py
+-rw-r--r--   0        0        0    41260 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/ddl.py
+-rw-r--r--   0        0        0      187 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/__init__.py
+-rw-r--r--   0        0        0     4411 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py
+-rw-r--r--   0        0        0    10670 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py
+-rw-r--r--   0        0        0    12669 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py
+-rw-r--r--   0        0        0     5443 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py
+-rw-r--r--   0        0        0    29307 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/hooks.py
+-rw-r--r--   0        0        0     4617 2024-04-02 08:29:11.025852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/reflection.py
+-rw-r--r--   0        0        0    64631 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/sql.py
+-rw-r--r--   0        0        0       81 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     8887 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/util/dtype.py
+-rw-r--r--   0        0        0      433 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0    11531 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    27793 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      311 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    23202 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0    22133 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     4294 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     8035 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     8392 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      135 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/debug/__init__.py
+-rw-r--r--   0        0        0      368 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      654 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     3133 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/dask.py
+-rw-r--r--   0        0        0     7269 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1388 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/__init__.py
+-rw-r--r--   0        0        0      620 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/cli.py
+-rw-r--r--   0        0        0        0 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/__init__.py
+-rw-r--r--   0        0        0     1741 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/clear_metadata.py
+-rw-r--r--   0        0        0     2744 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/delete_schemas.py
+-rw-r--r--   0        0        0      182 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     1709 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0    13261 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0    32965 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2921 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/debug.py
+-rw-r--r--   0        0        0     3837 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/details.py
+-rw-r--r--   0        0        0     2074 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    20861 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0      213 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     9273 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/computation_tracing.py
+-rw-r--r--   0        0        0     2061 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1848 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      944 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     1129 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/hashing.py
+-rw-r--r--   0        0        0     3816 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     7992 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     4812 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/json.py
+-rw-r--r--   0        0        0     1377 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2847 2024-04-02 08:29:11.029852 pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     7365 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.8.0/PKG-INFO
```

### Comparing `pydiverse_pipedag-0.7.2/LICENSE` & `pydiverse_pipedag-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/docs/package/README.md` & `pydiverse_pipedag-0.8.0/docs/package/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -139,13 +139,13 @@
 (i.e. containerized Postgres), please look [here](https://pydiversepipedag.readthedocs.io/en/latest/database_testing.html).
 
 ## Troubleshooting
 
 ### Installing mssql odbc driver for linux
 
 Installing with
-instructions [here](https://docs.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16#suse18)
+instructions [here](https://docs.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server)
 worked.
 But `odbcinst -j` revealed that it installed the configuration in `/etc/unixODBC/*`. But conda installed pyodbc brings
 its own `odbcinst` executable and that shows odbc config files are expected in `/etc/*`. Symlinks were enough to fix the
 problem. Try `python -c 'import pyodbc;print(pyodbc.drivers())'` and see whether you get more than an empty list.
 Furthermore, make sure you use 127.0.0.1 instead of localhost. It seems that /etc/hosts is ignored.
```

### Comparing `pydiverse_pipedag-0.7.2/pyproject.toml` & `pydiverse_pipedag-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-pipedag"
-version = "0.7.2"
+version = "0.8.0"
 description = "A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files."
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/__init__.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/blob.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/base.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/database.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/database.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/filelock.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/filelock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/nolock.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/nolock.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/lock/zookeeper.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/lock/zookeeper.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections.abc import Iterable
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Generic
 
 import structlog
 from typing_extensions import Self
 
+from pydiverse.pipedag import ConfigContext
 from pydiverse.pipedag._typing import T, TableHookResolverT
 from pydiverse.pipedag.context import RunContext, TaskContext
 from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.materialize.cache import TaskCacheInfo, lazy_table_cache_key
 from pydiverse.pipedag.materialize.container import RawSql, Table
 from pydiverse.pipedag.materialize.metadata import (
     LazyTableMetadata,
@@ -330,15 +331,15 @@
         table object represents a lazy table / query, the store first checks
         if the same query with the same input (based on `table.cache_key`)
         has already been executed before. If yes, instead of evaluating
         the query, it just copies the previous result to the commit stage.
 
         Used when `lazy = True` is set for a materializing task.
         """
-
+        config_context = ConfigContext.get()
         try:
             hook = self.get_m_table_hook(type(table.obj))
             query_str = hook.lazy_query_str(self, table.obj)
         except TypeError:
             self.logger.warning(
                 f"The output table {table.name} given by a"
                 f" {repr(type(table.obj))} of the lazy task {task.name} does"
@@ -348,29 +349,42 @@
             # Assign random query string to ensure that task is not cache valid
             query_str = uuid.uuid4().hex
 
         query_hash = stable_hash("LAZY-TABLE", query_str)
 
         # Store the table
         try:
+            if task_cache_info.force_task_execution:
+                self.logger.info(
+                    "Forced task execution due to config",
+                    cache_validation=config_context.cache_validation,
+                )
+                raise CacheError("Forced task execution")
             # Try retrieving the table from the cache and then copying it
             # to the transaction stage
             metadata = self.retrieve_lazy_table_metadata(
                 query_hash, task_cache_info.cache_key, table.stage
             )
             self.copy_lazy_table_to_transaction(metadata, table)
             self.logger.info(f"Lazy cache of table '{table.name}' found")
         except CacheError as e:
             # Either not found in cache, or copying failed
             # -> Store using default method
             self.logger.warning(
                 "Cache miss", table=table.name, stage=table.stage.name, cause=str(e)
             )
-
             TaskContext.get().is_cache_valid = False
+            if task_cache_info.assert_no_materialization:
+                raise AssertionError(
+                    "cache_validation.mode=ASSERT_NO_FRESH_INPUT is a "
+                    "protection mechanism to prevent execution of "
+                    "source tasks to keep pipeline input stable. However,"
+                    "this table was still about to be materialized: "
+                    f"{table.stage.name}.{table.name}"
+                ) from None
             self.store_table(table, task)
 
         # Store table metadata
         self.store_lazy_table_metadata(
             LazyTableMetadata(
                 name=table.name,
                 stage=table.stage.name,
@@ -404,14 +418,21 @@
             r'(__tmp|__even|__odd)(?=[ \t\n.;"]|$)', "", query_str.lower()
         )
 
         query_hash = stable_hash("RAW-SQL", query_str)
 
         # Store raw sql
         try:
+            if task_cache_info.force_task_execution:
+                config_context = ConfigContext.get()
+                self.logger.info(
+                    "Forced task execution due to config",
+                    cache_validation=config_context.cache_validation,
+                )
+                raise CacheError("Forced task execution")
             # Try retrieving the table from the cache and then copying it
             # to the transaction stage
             metadata = self.retrieve_raw_sql_metadata(
                 query_hash, task_cache_info.cache_key, raw_sql.stage
             )
             self.copy_raw_sql_tables_to_transaction(metadata, raw_sql.stage)
             self.logger.info(f"Lazy cache of stage '{raw_sql.stage}' found")
@@ -422,14 +443,22 @@
             # Either not found in cache, or copying failed
             # -> Store using default method
             self.logger.warning("Cache miss for raw-SQL", cause=str(e))
 
             TaskContext.get().is_cache_valid = False
             RunContext.get().set_stage_has_changed(task.stage)
 
+            if task_cache_info.assert_no_materialization:
+                raise AssertionError(
+                    "cache_validation.mode=ASSERT_NO_FRESH_INPUT is a "
+                    "protection mechanism to prevent execution of "
+                    "source tasks to keep pipeline input stable. However,"
+                    f"this raw SQL script was still about to be executed: {raw_sql}"
+                ) from None
+
             prev_objects = self.get_objects_in_stage(raw_sql.stage)
             self.execute_raw_sql(raw_sql)
             post_objects = self.get_objects_in_stage(raw_sql.stage)
 
             # Object names must be sorted to ensure that we can identify the task
             # again in the future even if the objects get returned in a different order.
             prev_objects = sorted(prev_objects)
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/cache/base.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/cache/parquet.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/cache/parquet.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/ddl.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/ddl.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 __all__ = [
     "Schema",
     "CreateSchema",
     "DropSchema",
     "RenameSchema",
     "DropSchemaContent",
     "CreateTableAsSelect",
+    "InsertIntoSelect",
     "CreateTableWithSuffix",
     "CreateViewAsSelect",
     "CreateAlias",
     "CopyTable",
     "RenameTable",
     "DropTable",
     "CreateDatabase",
@@ -30,14 +31,16 @@
     "DropProcedure",
     "DropView",
     "AddPrimaryKey",
     "AddIndex",
     "ChangeColumnNullable",
     "ChangeColumnTypes",
     "ChangeTableLogged",
+    "LockTable",
+    "LockSourceTable",
     "split_ddl_statement",
 ]
 
 from sqlalchemy.sql.type_api import TypeEngine
 
 
 @frozen
@@ -93,52 +96,65 @@
 class DropDatabase(DDLElement):
     def __init__(self, database: str, if_exists=False, cascade=False):
         self.database = database
         self.if_exists = if_exists
         self.cascade = cascade
 
 
+class InsertIntoSelect(DDLElement):
+    def __init__(
+        self,
+        name: str,
+        schema: Schema,
+        query: Select | TextClause | sa.Text,
+    ):
+        self.name = name
+        self.schema = schema
+        self.query = query
+
+
 class CreateTableAsSelect(DDLElement):
     def __init__(
         self,
         name: str,
         schema: Schema,
         query: Select | TextClause | sa.Text,
         *,
-        early_not_null: None | str | list[str] = None,
-        source_tables: None | list[dict[str, str]] = None,
         unlogged: bool = False,
         suffix: str = "",
     ):
         self.name = name
         self.schema = schema
         self.query = query
-        # some dialects may choose to set NOT-NULL constraint in the middle of
-        # create table as select
-        self.early_not_null = early_not_null
-        # some dialects may lock source and destination tables
-        self.source_tables = source_tables
         # Postgres supports creating unlogged tables. Flag should get ignored by
         # other dialects
         self.unlogged = unlogged
         # Suffix to be appended to the statement, e.g. from materialization details
         self.suffix = suffix
 
 
 class CreateTableWithSuffix(DDLElement):
     def __init__(
-        self, name: str, schema: Schema, sql_dtypes: dict[str, TypeEngine], suffix: str
+        self,
+        name: str,
+        schema: Schema,
+        sql_dtypes: dict[str, TypeEngine],
+        nullable: list[str] | None,
+        non_nullable: list[str] | None,
+        suffix: str,
     ):
         """
         This is used for dialect=ibm_sa_db to create a table in a
         table space and with compression before we let Pandas fill it with data.
         """
         self.name = name
         self.schema = schema
         self.sql_dtypes = sql_dtypes
+        self.nullable = nullable
+        self.non_nullable = non_nullable
         self.suffix = suffix
 
 
 class CreateViewAsSelect(DDLElement):
     def __init__(self, name: str, schema: Schema, query: Select | TextClause | sa.Text):
         self.name = name
         self.schema = schema
@@ -164,24 +180,23 @@
 class CopyTable(DDLElement):
     def __init__(
         self,
         from_name,
         from_schema: Schema,
         to_name,
         to_schema: Schema,
-        if_not_exists=False,
-        early_not_null: None | str | list[str] = None,
+        *,
+        unlogged: bool = False,
         suffix: str = "",
     ):
         self.from_name = from_name
         self.from_schema = from_schema
         self.to_name = to_name
         self.to_schema = to_schema
-        self.if_not_exists = if_not_exists
-        self.early_not_null = early_not_null
+        self.unlogged = unlogged
         self.suffix = suffix
 
 
 class RenameTable(DDLElement):
     def __init__(
         self,
         from_name,
@@ -357,14 +372,32 @@
         logged: bool,
     ):
         self.table_name = table_name
         self.schema = schema
         self.logged = logged
 
 
+class LockTable(DDLElement):
+    def __init__(self, name: str, schema: Schema | str):
+        """
+        Lock Table in exclusive mode for writing
+        """
+        self.name = name
+        self.schema = schema.get() if isinstance(schema, Schema) else schema
+
+
+class LockSourceTable(DDLElement):
+    def __init__(self, name: str, schema: Schema):
+        """
+        Lock Table in shared mode for reading.
+        """
+        self.name = name
+        self.schema = schema.get() if isinstance(schema, Schema) else schema
+
+
 @compiles(CreateSchema)
 def visit_create_schema(create: CreateSchema, compiler, **kw):
     _ = kw
     schema = compiler.preparer.format_schema(create.schema.get())
     text = ["CREATE SCHEMA"]
     if create.if_not_exists:
         text.append("IF NOT EXISTS")
@@ -641,35 +674,51 @@
         text.append("CASCADE")
     ret = " ".join(text)
     raise NotImplementedError(
         f"Disable for now for safety reasons (not yet needed): {ret}"
     )
 
 
-def _visit_create_obj_as_select(create, compiler, _type, kw, *, prefix="", suffix=""):
+def _visit_fill_obj_as_select(
+    create, compiler, _type, kw, *, cmd="CREATE ", sep=" AS", prefix="", suffix=""
+):
     name = compiler.preparer.quote(create.name)
     schema = compiler.preparer.format_schema(create.schema.get())
     kw["literal_binds"] = True
     select = compiler.sql_compiler.process(create.query, **kw)
-    return f"CREATE {_type} {schema}.{name} AS\n{prefix}{select}{suffix}"
+    return f"{cmd}{_type} {schema}.{name}{sep}\n{prefix}{select}{suffix}"
+
+
+@compiles(InsertIntoSelect)
+def visit_insert_into_select(insert: InsertIntoSelect, compiler, **kw):
+    return _visit_fill_obj_as_select(
+        insert, compiler, "", kw, cmd="INSERT INTO", sep=""
+    )
+
+
+@compiles(InsertIntoSelect, "mssql")
+def visit_insert_into_select_mssql(insert: InsertIntoSelect, compiler, **kw):
+    return _visit_fill_obj_as_select(
+        insert, compiler, "", kw, cmd="INSERT INTO", sep=" WITH(TABLOCKX)"
+    )
 
 
 @compiles(CreateTableAsSelect)
 def visit_create_table_as_select(create: CreateTableAsSelect, compiler, **kw):
-    return _visit_create_obj_as_select(create, compiler, "TABLE", kw)
+    return _visit_fill_obj_as_select(create, compiler, "TABLE", kw)
 
 
 @compiles(CreateTableAsSelect, "postgresql")
 def visit_create_table_as_select_postgresql(
     create: CreateTableAsSelect, compiler, **kw
 ):
     if create.unlogged:
-        return _visit_create_obj_as_select(create, compiler, "UNLOGGED TABLE", kw)
+        return _visit_fill_obj_as_select(create, compiler, "UNLOGGED TABLE", kw)
     else:
-        return _visit_create_obj_as_select(create, compiler, "TABLE", kw)
+        return _visit_fill_obj_as_select(create, compiler, "TABLE", kw)
 
 
 @compiles(CreateTableAsSelect, "mssql")
 def visit_create_table_as_select_mssql(create: CreateTableAsSelect, compiler, **kw):
     name = compiler.preparer.quote(create.name)
     schema = compiler.preparer.format_schema(create.schema.get())
 
@@ -677,61 +726,21 @@
     select = compiler.sql_compiler.process(create.query, **kw)
 
     return insert_into_in_query(select, schema, name)
 
 
 @compiles(CreateTableAsSelect, "ibm_db_sa")
 def visit_create_table_as_select_ibm_db_sa(create: CreateTableAsSelect, compiler, **kw):
+    # Attention: for DB2, a CreateTableAsSelect must be followed by an InsertIntoSelect
+    # to actually fill data
     suffix = ") DEFINITION ONLY " + create.suffix
-    prepare_statement = _visit_create_obj_as_select(
+    return _visit_fill_obj_as_select(
         create, compiler, "TABLE", kw, prefix="(", suffix=suffix
     )
 
-    if create.early_not_null is not None:
-        not_null_cols = create.early_not_null
-        if isinstance(not_null_cols, str):
-            not_null_cols = [not_null_cols]
-        not_null_statements = _get_nullable_change_statements(
-            ChangeColumnNullable(
-                create.name,
-                create.schema,
-                column_names=not_null_cols,
-                nullable=False,
-            ),
-            compiler,
-        )
-    else:
-        not_null_statements = []
-
-    preparer = compiler.preparer
-    name = preparer.quote(create.name)
-    schema = preparer.format_schema(create.schema.get())
-
-    lock_statements = [f"LOCK TABLE {schema}.{name} IN EXCLUSIVE MODE"]
-    if create.source_tables is not None:
-        src_tables = [
-            f"{preparer.format_schema(tbl['schema'])}.{preparer.quote(tbl['name'])}"
-            for tbl in create.source_tables
-            if tbl["shared_lock_allowed"]
-        ]
-        lock_statements += [f"LOCK TABLE {ref} IN SHARE MODE" for ref in src_tables]
-
-    kw["literal_binds"] = True
-    select = compiler.sql_compiler.process(create.query, **kw)
-    create_statement = f"INSERT INTO {schema}.{name}\n{select}"
-
-    return join_ddl_statements(
-        [prepare_statement]
-        + not_null_statements
-        + lock_statements
-        + [create_statement],
-        compiler,
-        **kw,
-    )
-
 
 @compiles(CreateTableWithSuffix, "ibm_db_sa")
 def visit_create_table_with_suffix(create: CreateTableWithSuffix, compiler, **kw):
     _ = kw
     name = compiler.preparer.quote(create.name)
     schema = compiler.preparer.format_schema(create.schema.get())
     statement = (
@@ -743,15 +752,15 @@
         + f"\n) {create.suffix}"
     )
     return statement
 
 
 @compiles(CreateViewAsSelect)
 def visit_create_view_as_select(create: CreateViewAsSelect, compiler, **kw):
-    return _visit_create_obj_as_select(create, compiler, "VIEW", kw)
+    return _visit_fill_obj_as_select(create, compiler, "VIEW", kw)
 
 
 def insert_into_in_query(select_sql, schema, table):
     into = f"INTO {schema}.{table}"
     into_point = None
     # insert INTO before first FROM, WHERE, GROUP BY, WINDOW, HAVING,
     #                          ORDER BY, UNION, EXCEPT, INTERSECT
@@ -826,22 +835,15 @@
     from_name = compiler.preparer.quote(copy_table.from_name)
     from_schema = compiler.preparer.format_schema(copy_table.from_schema.get())
     query = sa.select("*").select_from(sa.text(f"{from_schema}.{from_name}"))
     create = CreateTableAsSelect(
         copy_table.to_name,
         copy_table.to_schema,
         query,
-        early_not_null=copy_table.early_not_null,
-        source_tables=[
-            dict(
-                name=copy_table.from_name,
-                schema=copy_table.from_schema.get(),
-                shared_lock_allowed=True,
-            )
-        ],
+        unlogged=copy_table.unlogged,
         suffix=copy_table.suffix,
     )
     return compiler.process(create, **kw)
 
 
 @compiles(RenameTable)
 def visit_rename_table(rename_table: RenameTable, compiler, **kw):
@@ -1119,36 +1121,89 @@
     return f"ALTER TABLE {schema}.{table} {alter_columns}"
 
 
 @compiles(ChangeColumnNullable, "ibm_db_sa")
 def visit_change_column_nullable(change: ChangeColumnNullable, compiler, **kw):
     _ = kw
     statements = _get_nullable_change_statements(change, compiler)
+    table = compiler.preparer.quote(change.table_name)
+    schema = compiler.preparer.format_schema(change.schema.get())
+    statements.append(f"call sysproc.admin_cmd('REORG TABLE {schema}.{table}')")
+    return join_ddl_statements(statements, compiler, **kw)
+
+
+@compiles(ChangeColumnNullable, "duckdb")
+def visit_change_column_nullable(change: ChangeColumnNullable, compiler, **kw):
+    _ = kw
+    statements = _get_nullable_change_statements(change, compiler)
     return join_ddl_statements(statements, compiler, **kw)
 
 
 @compiles(ChangeTableLogged, "postgresql")
 def visit_change_table_logged(change: ChangeTableLogged, compiler, **kw):
     _ = kw
     table_name = compiler.preparer.quote(change.table_name)
     schema = compiler.preparer.format_schema(change.schema.get())
     logged = "LOGGED" if change.logged else "UNLOGGED"
     return f"ALTER TABLE {schema}.{table_name} SET {logged}"
 
 
+@compiles(LockTable)
+def visit_lock_table_postgres(lock_table: LockTable, compiler, **kw):
+    _ = kw
+    preparer = compiler.preparer
+    name = preparer.quote(lock_table.name)
+    schema = preparer.format_schema(lock_table.schema)
+
+    return f"LOCK TABLE {schema}.{name} IN ACCESS EXCLUSIVE MODE"
+
+
+@compiles(LockTable, "ibm_db_sa")
+def visit_lock_table_ibm_db_sa(lock_table: LockTable, compiler, **kw):
+    _ = kw
+    preparer = compiler.preparer
+    name = preparer.quote(lock_table.name)
+    schema = preparer.format_schema(lock_table.schema)
+
+    return f"LOCK TABLE {schema}.{name} IN EXCLUSIVE MODE"
+
+
+@compiles(LockSourceTable)
+def visit_lock_source_table_postgres(
+    lock_source_table: LockSourceTable, compiler, **kw
+):
+    _ = kw
+    preparer = compiler.preparer
+    name = preparer.quote(lock_source_table.name)
+    schema = preparer.format_schema(lock_source_table.schema)
+
+    return f"LOCK TABLE {schema}.{name} IN SHARE MODE"
+
+
+@compiles(LockSourceTable, "ibm_db_sa")
+def visit_lock_source_table_ibm_db_sa(
+    lock_source_table: LockSourceTable, compiler, **kw
+):
+    _ = kw
+    preparer = compiler.preparer
+    name = preparer.quote(lock_source_table.name)
+    schema = preparer.format_schema(lock_source_table.schema)
+
+    return f"LOCK TABLE {schema}.{name} IN SHARE MODE"
+
+
 def _get_nullable_change_statements(change, compiler):
     table = compiler.preparer.quote(change.table_name)
     schema = compiler.preparer.format_schema(change.schema.get())
     statements = [
         f"ALTER TABLE {schema}.{table} ALTER COLUMN"
         f" {compiler.preparer.quote(col)}"
         f" {'SET' if not nullable else 'DROP'} NOT NULL"
         for col, nullable in zip(change.column_names, change.nullable)
     ]
-    statements.append(f"call sysproc.admin_cmd('REORG TABLE {schema}.{table}')")
     return statements
 
 
 def _mssql_update_definition(
     conn: sa.Connection,
     name: str,
     old_schema: Schema,
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/duckdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,67 +40,78 @@
             name,
             sa.BigInteger(),
             sequence,
             server_default=sequence.next_value(),
             primary_key=True,
         )
 
+    def _default_isolation_level(self) -> str | None:
+        return None  # "READ UNCOMMITTED" does not exist in DuckDB
+
     def _init_database(self):
         if not self.create_database_if_not_exists:
             return
 
         # Duckdb already creates the database file automatically
         # However, the parent directory doesn't get created automatically
         database = self.engine_url.database
         if database == ":memory:":
             return
 
         database_path = Path(database)
         database_path.parent.mkdir(parents=True, exist_ok=True)
 
+    def dialect_requests_empty_creation(self, table: Table, is_sql: bool) -> bool:
+        _ = table, is_sql
+        return False  # DuckDB is not good with stable type arithmetic
+
 
 @DuckDBTableStore.register_table(pd)
 class PandasTableHook(PandasTableHook):
     @classmethod
     def _execute_materialize(
         cls,
         df: pd.DataFrame,
         store: DuckDBTableStore,
         table: Table[pd.DataFrame],
         schema: Schema,
         dtypes: dict[str, DType],
     ):
         engine = store.engine
-        dtypes = {name: dtype.to_sql() for name, dtype in dtypes.items()}
+        dtypes = cls._get_dialect_dtypes(dtypes, table)
         if table.type_map:
             dtypes.update(table.type_map)
 
         store.check_materialization_details_supported(
             resolve_materialization_details_label(table)
         )
 
         # Create empty table with correct schema
-        df[:0].to_sql(
-            table.name,
-            engine,
-            schema=schema.get(),
-            index=False,
-            dtype=dtypes,
+        cls._dialect_create_empty_table(store, df, table, schema, dtypes)
+        store.add_indexes_and_set_nullable(
+            table, schema, on_empty_table=True, table_cols=df.columns
         )
 
         # Copy dataframe directly to duckdb
         # This is SIGNIFICANTLY faster than using pandas.to_sql
         table_name = engine.dialect.identifier_preparer.quote(table.name)
         schema_name = engine.dialect.identifier_preparer.format_schema(schema.get())
 
         connection_uri = store.engine_url.render_as_string(hide_password=False)
         connection_uri = connection_uri.replace("duckdb:///", "", 1)
         with duckdb.connect(connection_uri) as conn:
             conn.execute(f"INSERT INTO {schema_name}.{table_name} SELECT * FROM df")
 
+        store.add_indexes_and_set_nullable(
+            table,
+            schema,
+            on_empty_table=False,
+            table_cols=df.columns,
+        )
+
 
 try:
     import polars
 except ImportError as e:
     warnings.warn(str(e), ImportWarning)
     polars = None
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/ibm_db2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from __future__ import annotations
 
-import time
+from collections.abc import Iterable
 from dataclasses import dataclass
 from enum import Enum
+from typing import Any
 
 import pandas as pd
 import sqlalchemy as sa
 import sqlalchemy.exc
 
 from pydiverse.pipedag.backend.table.sql.ddl import (
-    AddPrimaryKey,
-    ChangeColumnNullable,
     CreateTableWithSuffix,
+    LockSourceTable,
+    LockTable,
     Schema,
 )
 from pydiverse.pipedag.backend.table.sql.hooks import PandasTableHook
 from pydiverse.pipedag.backend.table.sql.reflection import PipedagDB2Reflection
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
 from pydiverse.pipedag.materialize import Table
@@ -82,45 +83,85 @@
 
     Takes the same arguments as
     :py:class:`SQLTableStore <pydiverse.pipedag.backend.table.SQLTableStore>`
     """
 
     _dialect_name = "ibm_db_sa"
 
-    def add_primary_key(
+    def _default_isolation_level(self):
+        return "UNCOMMITTED READ"
+
+    def lock_table(
+        self, table: Table | str, schema: Schema | str, conn: Any = None
+    ) -> list:
+        """
+        For some dialects, it might be beneficial to lock a table before writing to it.
+        """
+        stmt = LockTable(table.name if isinstance(table, Table) else table, schema)
+        if conn is not None:
+            self.execute(stmt, conn=conn)
+        return [stmt]
+
+    def lock_source_table(
+        self, table: Table | str, schema: Schema | str, conn: Any = None
+    ) -> list:
+        """
+        For some dialects, it might be beneficial to lock source tables before reading.
+        """
+        stmt = LockSourceTable(
+            table.name if isinstance(table, Table) else table, schema
+        )
+        if conn is not None:
+            self.execute(stmt, conn=conn)
+        return [stmt]
+
+    def dialect_requests_empty_creation(self, table: Table, is_sql: bool) -> bool:
+        if is_sql:
+            # IBM DB2 does not support CREATE TABLE AS SELECT without INSERT INTO
+            return True
+        else:
+            label = resolve_materialization_details_label(table)
+            return (
+                (label is not None and len(label.strip()) > 0)
+                or table.nullable is not None
+                or table.non_nullable is not None
+                or (table.primary_key is not None and len(table.primary_key) > 0)
+            )
+
+    def get_forced_nullability_columns(
+        self, table: Table, table_cols: Iterable[str], report_nullable_cols=False
+    ) -> tuple[list[str], list[str]]:
+        # ibm_db2 dialect has literals as non-nullable types by default, so we also need
+        # the list of nullable columns to fix
+        nullable_cols, non_nullable_cols = self._process_table_nullable_parameters(
+            table, table_cols
+        )
+        # add primery key columns to non_nullable_cols
+        if table.primary_key:
+            primary_key = (
+                table.primary_key
+                if isinstance(table.primary_key, list)
+                else [table.primary_key]
+            )
+            non_nullable_cols += primary_key
+            nullable_cols = [
+                col for col in nullable_cols if col not in table.primary_key
+            ]
+        return nullable_cols, non_nullable_cols
+
+    def add_indexes_and_set_nullable(
         self,
-        table_name: str,
+        table: Table,
         schema: Schema,
-        key_columns: list[str],
         *,
-        name: str | None = None,
-        early_not_null_possible: bool = False,
+        on_empty_table: bool | None = None,
+        table_cols: Iterable[str] | None = None,
     ):
-        if not early_not_null_possible:
-            for retry_iteration in range(4):
-                # retry operation since it might have been terminated as a
-                # deadlock victim
-                try:
-                    self.execute(
-                        ChangeColumnNullable(
-                            table_name, schema, key_columns, nullable=False
-                        )
-                    )
-                    break
-                except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
-                    if retry_iteration == 3:
-                        raise
-                    time.sleep(retry_iteration * retry_iteration * 1.1)
-        self.execute(AddPrimaryKey(table_name, schema, key_columns, name))
-
-    def add_indexes(
-        self, table: Table, schema: Schema, *, early_not_null_possible: bool = False
-    ):
-        super().add_indexes(
-            table, schema, early_not_null_possible=early_not_null_possible
+        super().add_indexes_and_set_nullable(
+            table, schema, on_empty_table=on_empty_table, table_cols=table_cols
         )
         table_name = self.engine.dialect.identifier_preparer.quote(table.name)
         schema_name = self.engine.dialect.identifier_preparer.quote_schema(schema.get())
         query = (
             f"CALL SYSPROC.ADMIN_CMD('RUNSTATS ON TABLE {schema_name}.{table_name}"
             f" ON ALL COLUMNS WITH DISTRIBUTION ON ALL COLUMNS AND UNSAMPLED"
             f" DETAILED INDEXES ALL SET PROFILE');"
@@ -199,55 +240,50 @@
         compression_suffix = " ".join(compression)
         return " ".join((table_space_suffix, compression_suffix))
 
 
 @IBMDB2TableStore.register_table(pd)
 class PandasTableHook(PandasTableHook):
     @classmethod
-    def _execute_materialize(
-        cls,
-        df: pd.DataFrame,
-        store: IBMDB2TableStore,
-        table: Table[pd.DataFrame],
-        schema: Schema,
-        dtypes: dict[str, DType],
-    ):
+    def _get_dialect_dtypes(cls, dtypes: dict[str, DType], table: Table[pd.DataFrame]):
         # Default string target is CLOB which can't be used for indexing.
         # -> Convert indexed string columns to VARCHAR(256)
         index_columns = set()
         if indexes := table.indexes:
             index_columns |= {col for index in indexes for col in index}
         if primary_key := table.primary_key:
             index_columns |= set(primary_key)
 
-        dtypes = ({name: dtype.to_sql() for name, dtype in dtypes.items()}) | (
+        return ({name: dtype.to_sql() for name, dtype in dtypes.items()}) | (
             {
                 name: (
                     sa.String(length=256)
                     if name in index_columns
                     else sa.String(length=32_672)
                 )
                 for name, dtype in dtypes.items()
                 if dtype == DType.STRING
             }
         )
 
-        if table.type_map:
-            dtypes.update(table.type_map)
-
-        engine = store.engine
+    @classmethod
+    def _dialect_create_empty_table(
+        cls,
+        store: SQLTableStore,
+        df: pd.DataFrame,
+        table: Table[pd.DataFrame],
+        schema: Schema,
+        dtypes: dict[str, DType],
+    ):
         suffix = store.get_create_table_suffix(
             resolve_materialization_details_label(table)
         )
-        if suffix:
-            store.execute(CreateTableWithSuffix(table.name, schema, dtypes, suffix))
-
-        # noinspection PyTypeChecker
-        df.to_sql(
-            table.name,
-            engine,
-            schema=schema.get(),
-            index=False,
-            dtype=dtypes,
-            chunksize=100_000,
-            if_exists="append" if suffix else "fail",
+        store.execute(
+            CreateTableWithSuffix(
+                table.name,
+                schema,
+                dtypes,
+                table.nullable,
+                table.non_nullable,
+                suffix,
+            )
         )
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/mssql.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import re
+from collections.abc import Iterable
 from typing import Any
 
 import pandas as pd
 import sqlalchemy as sa
 import sqlalchemy.dialects.mssql
 
 from pydiverse.pipedag.backend.table.sql.ddl import (
@@ -17,15 +18,14 @@
 )
 from pydiverse.pipedag.backend.table.sql.hooks import IbisTableHook, PandasTableHook
 from pydiverse.pipedag.backend.table.sql.reflection import PipedagMSSqlReflection
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
 from pydiverse.pipedag.backend.table.util import DType
 from pydiverse.pipedag.materialize import Table
 from pydiverse.pipedag.materialize.container import RawSql
-from pydiverse.pipedag.materialize.details import resolve_materialization_details_label
 
 
 class MSSqlTableStore(SQLTableStore):
     """
     SQLTableStore that supports `Microsoft SQL Server`_.
 
     In addition to the arguments of
@@ -83,30 +83,15 @@
     def add_primary_key(
         self,
         table_name: str,
         schema: Schema,
         key_columns: list[str],
         *,
         name: str | None = None,
-        early_not_null_possible: bool = False,
     ):
-        _ = early_not_null_possible  # not needed for this dialect
-        sql_types = self.reflect_sql_types(key_columns, table_name, schema)
-        # impose some varchar(max) limit to allow use in primary key / index
-        # TODO: consider making cap_varchar_max a config option
-        self.execute(
-            ChangeColumnTypes(
-                table_name,
-                schema,
-                key_columns,
-                sql_types,
-                nullable=False,
-                cap_varchar_max=1024,
-            )
-        )
         self.execute(AddPrimaryKey(table_name, schema, key_columns, name))
 
     def add_index(
         self,
         table_name: str,
         schema: Schema,
         index_columns: list[str],
@@ -123,14 +108,97 @@
             self.execute(
                 ChangeColumnTypes(
                     table_name, schema, index_columns, sql_types, cap_varchar_max=1024
                 )
             )
         self.execute(AddIndex(table_name, schema, index_columns, name))
 
+    def dialect_requests_empty_creation(self, table: Table, is_sql: bool) -> bool:
+        _ = is_sql
+        return (
+            table.nullable is not None
+            or table.non_nullable is not None
+            or (table.primary_key is not None and len(table.primary_key) > 0)
+        )
+
+    def get_forced_nullability_columns(
+        self, table: Table, table_cols: Iterable[str], report_nullable_cols=False
+    ) -> tuple[list[str], list[str]]:
+        # mssql dialect has literals as non-nullable types by default, so we also need
+        # the list of nullable columns as well
+        return self._process_table_nullable_parameters(table, table_cols)
+
+    def add_indexes_and_set_nullable(
+        self,
+        table: Table,
+        schema: Schema,
+        *,
+        on_empty_table: bool | None = None,
+        table_cols: Iterable[str] | None = None,
+    ):
+        if on_empty_table is None or on_empty_table:
+            # Set non-nullable and primary key on empty table
+            key_columns = (
+                [table.primary_key]
+                if isinstance(table.primary_key, str)
+                else table.primary_key
+                if table.primary_key is not None
+                else []
+            )
+            # reflect sql types because mssql cannot just change nullable flag
+            inspector = sa.inspect(self.engine)
+            columns = inspector.get_columns(table.name, schema=schema.get())
+            table_cols = [d["name"] for d in columns]
+            types = {d["name"]: d["type"] for d in columns}
+            nullable_cols, non_nullable_cols = self.get_forced_nullability_columns(
+                table, table_cols
+            )
+            non_nullable_cols = [
+                col for col in non_nullable_cols if col not in key_columns
+            ]
+            sql_types = [types[col] for col in nullable_cols]
+            if len(nullable_cols) > 0:
+                self.execute(
+                    ChangeColumnTypes(
+                        table.name,
+                        schema,
+                        nullable_cols,
+                        sql_types,
+                        nullable=True,
+                    )
+                )
+            sql_types = [types[col] for col in non_nullable_cols]
+            if len(non_nullable_cols) > 0:
+                self.execute(
+                    ChangeColumnTypes(
+                        table.name,
+                        schema,
+                        non_nullable_cols,
+                        sql_types,
+                        nullable=False,
+                    )
+                )
+            if len(key_columns) > 0:
+                sql_types = [types[col] for col in key_columns]
+                # impose some varchar(max) limit to allow use in primary key / index
+                # TODO: consider making cap_varchar_max a config option
+                self.execute(
+                    ChangeColumnTypes(
+                        table.name,
+                        schema,
+                        key_columns,
+                        sql_types,
+                        nullable=False,
+                        cap_varchar_max=1024,
+                    )
+                )
+            self.add_table_primary_key(table, schema)
+        if on_empty_table is None or not on_empty_table:
+            self.add_table_indexes(table, schema)
+
     def execute_raw_sql(self, raw_sql: RawSql):
         if self.disable_pytsql:
             self.__execute_raw_sql_fallback(raw_sql)
         else:
             self.__execute_raw_sql_pytsql(raw_sql)
 
     def __execute_raw_sql_fallback(self, raw_sql: RawSql):
@@ -229,46 +297,24 @@
         table_name, schema = super().resolve_alias(table, stage_name)
         return PipedagMSSqlReflection.resolve_alias(self.engine, table_name, schema)
 
 
 @MSSqlTableStore.register_table(pd)
 class PandasTableHook(PandasTableHook):
     @classmethod
-    def _execute_materialize(
-        cls,
-        df: pd.DataFrame,
-        store: MSSqlTableStore,
-        table: Table[pd.DataFrame],
-        schema: Schema,
-        dtypes: dict[str, DType],
-    ):
-        dtypes = ({name: dtype.to_sql() for name, dtype in dtypes.items()}) | (
+    def _get_dialect_dtypes(cls, dtypes: dict[str, DType], table: Table[pd.DataFrame]):
+        _ = table
+        return ({name: dtype.to_sql() for name, dtype in dtypes.items()}) | (
             {
                 name: sa.dialects.mssql.DATETIME2()
                 for name, dtype in dtypes.items()
                 if dtype == DType.DATETIME
             }
         )
 
-        if table.type_map:
-            dtypes.update(table.type_map)
-
-        store.check_materialization_details_supported(
-            resolve_materialization_details_label(table)
-        )
-
-        df.to_sql(
-            table.name,
-            store.engine,
-            schema=schema.get(),
-            index=False,
-            dtype=dtypes,
-            chunksize=100_000,
-        )
-
 
 try:
     import ibis
 except ImportError:
     ibis = None
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/dialects/postgres.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import csv
 from dataclasses import dataclass
 from io import StringIO
+from typing import Any
 
 import pandas as pd
-import sqlalchemy as sa
 
 from pydiverse.pipedag.backend.table.sql.ddl import (
     ChangeTableLogged,
-    CreateTableAsSelect,
+    LockSourceTable,
+    LockTable,
     Schema,
 )
 from pydiverse.pipedag.backend.table.sql.hooks import (
     PandasTableHook,
     SQLAlchemyTableHook,
 )
 from pydiverse.pipedag.backend.table.sql.sql import SQLTableStore
@@ -62,14 +63,38 @@
             materialization_details_label,
             self.default_materialization_details,
             "unlogged",
             self.strict_materialization_details,
             self.logger,
         )
 
+    def lock_table(
+        self, table: Table | str, schema: Schema | str, conn: Any = None
+    ) -> list:
+        """
+        For some dialects, it might be beneficial to lock a table before writing to it.
+        """
+        stmt = LockTable(table.name if isinstance(table, Table) else table, schema)
+        if conn is not None:
+            self.execute(stmt, conn=conn)
+        return [stmt]
+
+    def lock_source_table(
+        self, table: Table | str, schema: Schema | str, conn: Any = None
+    ) -> list:
+        """
+        For some dialects, it might be beneficial to lock source tables before reading.
+        """
+        stmt = LockSourceTable(
+            table.name if isinstance(table, Table) else table, schema
+        )
+        if conn is not None:
+            self.execute(stmt, conn=conn)
+        return [stmt]
+
     def check_materialization_details_supported(self, label: str | None) -> None:
         _ = label
         return
 
     def _set_materialization_details(
         self, materialization_details: dict[str, dict[str | list[str]]] | None
     ) -> None:
@@ -81,71 +106,40 @@
                 self.logger,
             )
         )
 
 
 @PostgresTableStore.register_table()
 class SQLAlchemyTableHook(SQLAlchemyTableHook):
-    @classmethod
-    def materialize(
-        cls,
-        store: PostgresTableStore,
-        table: Table[sa.sql.expression.TextClause | sa.Text],
-        stage_name,
-    ):
-        obj = table.obj
-        if isinstance(table.obj, (sa.Table, sa.sql.expression.Alias)):
-            obj = sa.select("*").select_from(table.obj)
-
-        store.check_materialization_details_supported(
-            resolve_materialization_details_label(table)
-        )
-
-        schema = store.get_schema(stage_name)
-        store.execute(
-            CreateTableAsSelect(
-                table.name,
-                schema,
-                obj,
-                unlogged=store.get_unlogged(
-                    resolve_materialization_details_label(table)
-                ),
-            )
-        )
-        store.add_indexes(table, schema, early_not_null_possible=True)
+    pass  # postges is our reference dialect
 
 
 @PostgresTableStore.register_table(pd)
 class PandasTableHook(PandasTableHook):
     @classmethod
     def _execute_materialize(
         cls,
         df: pd.DataFrame,
         store: PostgresTableStore,
         table: Table[pd.DataFrame],
         schema: Schema,
         dtypes: dict[str, DType],
     ):
-        engine = store.engine
         dtypes = {name: dtype.to_sql() for name, dtype in dtypes.items()}
         if table.type_map:
             dtypes.update(table.type_map)
 
         # Create empty table
-        df[:0].to_sql(
-            table.name,
-            engine,
-            schema=schema.get(),
-            index=False,
-            dtype=dtypes,
+        cls._dialect_create_empty_table(store, df, table, schema, dtypes)
+        store.add_indexes_and_set_nullable(
+            table, schema, on_empty_table=True, table_cols=df.columns
         )
 
         if store.get_unlogged(resolve_materialization_details_label(table)):
-            with engine.begin() as conn:
-                conn.execute(ChangeTableLogged(table.name, schema, False))
+            store.execute(ChangeTableLogged(table.name, schema, False))
 
         # COPY data
         # TODO: For python 3.12, there is csv.QUOTE_STRINGS
         #       This would make everything a bit safer, because then we could represent
         #       the string "\\N" (backslash + capital n).
         s_buf = StringIO()
         df.to_csv(
@@ -153,21 +147,23 @@
             na_rep="\\N",
             header=False,
             index=False,
             quoting=csv.QUOTE_MINIMAL,
         )
         s_buf.seek(0)
 
+        engine = store.engine
         table_name = engine.dialect.identifier_preparer.quote(table.name)
         schema_name = engine.dialect.identifier_preparer.format_schema(schema.get())
 
         dbapi_conn = engine.raw_connection()
         try:
             with dbapi_conn.cursor() as cur:
                 sql = (
                     f"COPY {schema_name}.{table_name} FROM STDIN"
                     " WITH (FORMAT CSV, NULL '\\N')"
                 )
+                store.logger.info("Executing bulk load", query=sql)
                 cur.copy_expert(sql=sql, file=s_buf)
             dbapi_conn.commit()
         finally:
             dbapi_conn.close()
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/hooks.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from packaging.version import Version
 
 from pydiverse.pipedag import ConfigContext
 from pydiverse.pipedag._typing import T
 from pydiverse.pipedag.backend.table.base import AutoVersionSupport, TableHook
 from pydiverse.pipedag.backend.table.sql.ddl import (
     CreateTableAsSelect,
+    InsertIntoSelect,
     Schema,
 )
 from pydiverse.pipedag.backend.table.sql.sql import (
     ExternalTableReference,
     SQLTableStore,
 )
 from pydiverse.pipedag.backend.table.util import (
@@ -47,71 +48,103 @@
     def can_retrieve(cls, type_) -> bool:
         return type_ == sa.Table
 
     @classmethod
     def materialize(
         cls,
         store: SQLTableStore,
-        table: Table[sa.sql.expression.TextClause | sa.Text],
+        table: Table[sa.sql.expression.TextClause | sa.sql.expression.Selectable],
         stage_name,
     ):
         obj = table.obj
         if isinstance(table.obj, (sa.Table, sa.sql.expression.Alias)):
             obj = sa.select("*").select_from(table.obj)
+            tbl = table.obj if isinstance(table.obj, sa.Table) else table.obj.original
+            source_tables = [
+                dict(
+                    name=tbl.name,
+                    schema=tbl.schema,
+                    shared_lock_allowed=table.shared_lock_allowed,
+                )
+            ]
+        else:
+            source_tables = [
+                dict(
+                    name=tbl.name,
+                    schema=store.get_schema(tbl.stage.current_name).get()
+                    if tbl.external_schema is None
+                    else tbl.external_schema,
+                    shared_lock_allowed=tbl.shared_lock_allowed,
+                )
+                for tbl in TaskContext.get().input_tables
+            ]
 
-        source_tables = [
-            dict(
-                name=tbl.name,
-                schema=store.get_schema(tbl.stage.current_name).get()
-                if tbl.external_schema is None
-                else tbl.external_schema,
-                shared_lock_allowed=tbl.shared_lock_allowed,
-            )
-            for tbl in TaskContext.get().input_tables
-        ]
         schema = store.get_schema(stage_name)
 
         store.check_materialization_details_supported(
             resolve_materialization_details_label(table)
         )
 
-        store.execute(
-            CreateTableAsSelect(
-                table.name,
-                schema,
-                obj,
-                early_not_null=table.primary_key,
-                source_tables=source_tables,
-                suffix=store.get_create_table_suffix(
-                    resolve_materialization_details_label(table)
-                ),
-            )
+        suffix = store.get_create_table_suffix(
+            resolve_materialization_details_label(table)
         )
-        store.add_indexes(table, schema, early_not_null_possible=True)
+        unlogged = store.get_unlogged(resolve_materialization_details_label(table))
+        if store.dialect_requests_empty_creation(table, is_sql=True):
+            limit_query = store.get_limit_query(obj, rows=0)
+            store.execute(
+                CreateTableAsSelect(
+                    table.name,
+                    schema,
+                    limit_query,
+                    unlogged=unlogged,
+                    suffix=suffix,
+                )
+            )
+            store.add_indexes_and_set_nullable(table, schema, on_empty_table=True)
+            statements = store.lock_table(table, schema)
+            statements += store.lock_source_tables(source_tables)
+            statements += [
+                InsertIntoSelect(
+                    table.name,
+                    schema,
+                    obj,
+                )
+            ]
+            store.execute(
+                statements,
+                truncate_printed_select=True,
+            )
+            store.add_indexes_and_set_nullable(table, schema, on_empty_table=False)
+        else:
+            statements = store.lock_source_tables(source_tables)
+            statements += [
+                CreateTableAsSelect(
+                    table.name,
+                    schema,
+                    obj,
+                    unlogged=unlogged,
+                    suffix=suffix,
+                )
+            ]
+            store.execute(statements)
+            store.add_indexes_and_set_nullable(table, schema)
 
     @classmethod
     def retrieve(
-        cls, store, table: Table, stage_name: str, as_type: type[sa.Table]
+        cls,
+        store: SQLTableStore,
+        table: Table,
+        stage_name: str,
+        as_type: type[sa.Table],
     ) -> sa.sql.expression.Selectable:
         table_name, schema = store.resolve_alias(table, stage_name)
         alias_name = TaskContext.get().name_disambiguator.get_name(table_name)
 
-        for retry_iteration in range(4):
-            # retry operation since it might have been terminated as a deadlock victim
-            try:
-                return sa.Table(
-                    table_name,
-                    sa.MetaData(),
-                    schema=schema,
-                    autoload_with=store.engine,
-                ).alias(alias_name)
-            except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
-                if retry_iteration == 3:
-                    raise
-                time.sleep(retry_iteration * retry_iteration * 1.2)
+        tbl = store.reflect_table(table_name, schema)
+        return tbl.alias(alias_name)
 
     @classmethod
     def lazy_query_str(cls, store, obj) -> str:
         if isinstance(obj, sa.sql.expression.FromClause):
             query = sa.select("*").select_from(obj)
         else:
             query = obj
@@ -244,40 +277,78 @@
         cls._execute_materialize(
             df,
             store=store,
             table=table,
             schema=schema,
             dtypes=dtypes,
         )
-        store.add_indexes(table, schema)
+
+    @classmethod
+    def _get_dialect_dtypes(cls, dtypes: dict[str, DType], table: Table[pd.DataFrame]):
+        _ = table
+        return {name: dtype.to_sql() for name, dtype in dtypes.items()}
+
+    @classmethod
+    def _dialect_create_empty_table(
+        cls,
+        store: SQLTableStore,
+        df: pd.DataFrame,
+        table: Table[pd.DataFrame],
+        schema: Schema,
+        dtypes: dict[str, DType],
+    ):
+        df[:0].to_sql(
+            table.name,
+            store.engine,
+            schema=schema.get(),
+            index=False,
+            dtype=dtypes,
+        )
 
     @classmethod
     def _execute_materialize(
         cls,
         df: pd.DataFrame,
         store: SQLTableStore,
         table: Table[pd.DataFrame],
         schema: Schema,
         dtypes: dict[str, DType],
     ):
-        dtypes = {name: dtype.to_sql() for name, dtype in dtypes.items()}
+        dtypes = cls._get_dialect_dtypes(dtypes, table)
         if table.type_map:
             dtypes.update(table.type_map)
 
         store.check_materialization_details_supported(
             resolve_materialization_details_label(table)
         )
 
-        df.to_sql(
-            table.name,
-            store.engine,
-            schema=schema.get(),
-            index=False,
-            dtype=dtypes,
-            chunksize=100_000,
+        if early := store.dialect_requests_empty_creation(table, is_sql=False):
+            cls._dialect_create_empty_table(store, df, table, schema, dtypes)
+            store.add_indexes_and_set_nullable(
+                table, schema, on_empty_table=True, table_cols=df.columns
+            )
+
+        with store.engine_connect() as conn:
+            with conn.begin():
+                if early:
+                    store.lock_table(table, schema, conn)
+                df.to_sql(
+                    table.name,
+                    conn,
+                    schema=schema.get(),
+                    index=False,
+                    dtype=dtypes,
+                    chunksize=100_000,
+                    if_exists="append" if early else "fail",
+                )
+        store.add_indexes_and_set_nullable(
+            table,
+            schema,
+            on_empty_table=False if early else None,
+            table_cols=df.columns,
         )
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
@@ -312,23 +383,17 @@
     def _build_retrieve_query(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
         backend: PandasDTypeBackend,
     ) -> tuple[Any, dict[str, DType]]:
-        engine = store.engine
         table_name, schema = store.resolve_alias(table, stage_name)
 
-        sql_table = sa.Table(
-            table_name,
-            sa.MetaData(),
-            schema=schema,
-            autoload_with=engine,
-        ).alias("tbl")
+        sql_table = store.reflect_table(table_name, schema).alias("tbl")
 
         cols = {col.name: col for col in sql_table.columns}
         dtypes = {name: DType.from_sql(col.type) for name, col in cols.items()}
 
         cols, dtypes = cls._adjust_cols_retrieve(cols, dtypes, backend)
 
         query = sa.select(*cols.values()).select_from(sql_table)
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/reflection.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/reflection.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/sql/sql.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/sql/sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 from __future__ import annotations
 
 import json
 import textwrap
+import time
 import warnings
 from collections.abc import Iterable
 from contextlib import contextmanager
 from typing import Any
 
 import sqlalchemy as sa
 import sqlalchemy.exc
 
 from pydiverse.pipedag import Stage, Table
 from pydiverse.pipedag.backend.table.base import BaseTableStore
 from pydiverse.pipedag.backend.table.sql.ddl import (
     AddIndex,
     AddPrimaryKey,
+    ChangeColumnNullable,
     CopyTable,
     CreateAlias,
     CreateDatabase,
     CreateSchema,
     DropAlias,
     DropSchema,
     DropSchemaContent,
     DropTable,
     RenameSchema,
     RenameTable,
     Schema,
     split_ddl_statement,
 )
 from pydiverse.pipedag.context import RunContext
-from pydiverse.pipedag.context.context import ConfigContext, StageCommitTechnique
+from pydiverse.pipedag.context.context import (
+    CacheValidationMode,
+    ConfigContext,
+    StageCommitTechnique,
+)
 from pydiverse.pipedag.context.run_context import DeferredTableStoreOp
 from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.materialize.container import RawSql
 from pydiverse.pipedag.materialize.core import MaterializingTask
-from pydiverse.pipedag.materialize.details import (
-    resolve_materialization_details_label,
-)
 from pydiverse.pipedag.materialize.metadata import (
     LazyTableMetadata,
     RawSqlMetadata,
     TaskMetadata,
 )
 from pydiverse.pipedag.util.hashing import stable_hash
 
@@ -373,66 +376,136 @@
         except sa.exc.DBAPIError:
             # This happens if multiple instances try to create the database
             # at the same time.
             with self.engine.connect() as conn:
                 # Verify database actually exists
                 conn.exec_driver_sql("SELECT 1")
 
+    def _default_isolation_level(self) -> str | None:
+        # we never want database transactional behavior (concurrent read+write)
+        return "READ UNCOMMITTED"
+
     def _create_engine(self):
+        kwargs = {}
+        if self._default_isolation_level() is not None:
+            kwargs["isolation_level"] = self._default_isolation_level()
+
         # future=True enables SQLAlchemy 2.0 behaviour with version 1.4
         return sa.create_engine(
             self.engine_url,
             future=True,
             pool_size=self.sqlalchemy_pool_size,
             pool_timeout=self.squalchemy_pool_timeout,
+            **kwargs,
         )
 
     @contextmanager
     def engine_connect(self) -> sa.Connection:
         with self.engine.connect() as conn:
             yield conn
             conn.commit()
 
     def get_schema(self, name: str) -> Schema:
         return Schema(name, self.schema_prefix, self.schema_suffix)
 
-    def _execute(self, query, conn: sa.engine.Connection):
+    def _execute(
+        self, query, conn: sa.engine.Connection, truncate_printed_select=False
+    ):
         if self.print_sql:
             if isinstance(query, str):
                 query_str = query
             else:
                 query_str = str(
                     query.compile(self.engine, compile_kwargs={"literal_binds": True})
                 )
-            pretty_query_str = self.format_sql_string(query_str)
+            pretty_query_str = self.format_sql_string(
+                query_str, truncate_printed_select
+            )
             self.logger.info("Executing sql", query=pretty_query_str)
 
         if isinstance(query, str):
             return conn.execute(sa.text(query))
         else:
             return conn.execute(query)
 
-    def execute(self, query, *, conn: sa.engine.Connection = None):
+    def execute(
+        self,
+        query: str
+        | sqlalchemy.sql.expression.Selectable
+        | sqlalchemy.sql.expression.TextClause
+        | sqlalchemy.sql.ddl.DDLElement
+        | list[
+            str
+            | sqlalchemy.sql.expression.Selectable
+            | sqlalchemy.sql.expression.TextClause
+            | sqlalchemy.sql.ddl.DDLElement
+        ],
+        *,
+        conn: sa.engine.Connection = None,
+        truncate_printed_select=False,
+    ):
         if conn is None:
             with self.engine_connect() as conn:
-                return self.execute(query, conn=conn)
+                return self.execute(
+                    query,
+                    conn=conn,
+                    truncate_printed_select=truncate_printed_select,
+                )
 
-        if isinstance(query, sa.schema.DDLElement):
-            # Some custom DDL statements contain multiple statements.
-            # They are all seperated using a special seperator.
-            query_str = str(
-                query.compile(self.engine, compile_kwargs={"literal_binds": True})
-            )
+        if isinstance(query, sa.schema.DDLElement) or isinstance(query, list):
+            if not isinstance(query, list):
+                query = [query]
+
+            @contextmanager
+            def transactional():
+                if conn.in_transaction():
+                    yield
+                else:
+                    with conn.begin():
+                        yield
+
+            with transactional():
+                # execute multiple statements in one transaction
+                for cur_query in query:
+                    if isinstance(cur_query, sa.schema.DDLElement):
+                        # Some custom DDL statements contain multiple statements.
+                        # They are all seperated using a special seperator.
+                        query_str = str(
+                            cur_query.compile(
+                                self.engine, compile_kwargs={"literal_binds": True}
+                            )
+                        )
 
-            with conn.begin():
-                for part in split_ddl_statement(query_str):
-                    self._execute(part, conn)
+                        for part in split_ddl_statement(query_str):
+                            self._execute(part, conn, truncate_printed_select)
+                    else:
+                        self._execute(cur_query, conn, truncate_printed_select)
             return
 
-        return self._execute(query, conn)
+        return self._execute(query, conn, truncate_printed_select)
+
+    def reflect_table(self, table_name: str, schema: str | Schema) -> sa.Table:
+        if isinstance(schema, Schema):
+            schema = schema.get()
+        tbl = None
+        for retry_iteration in range(4):
+            # retry operation since it might have been terminated as a deadlock victim
+            try:
+                tbl = sa.Table(
+                    table_name,
+                    sa.MetaData(),
+                    schema=schema,
+                    autoload_with=self.engine,
+                )
+                break
+            except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
+                if retry_iteration == 3:
+                    raise
+                time.sleep(retry_iteration * retry_iteration * 1.2)
+        return tbl
 
     def check_materialization_details_supported(self, label: str | None) -> None:
         if label is None:
             return
         error_msg = (
             f"Materialization details are not supported"
             f" for store {type(self).__name__}."
@@ -458,51 +531,226 @@
             if self.strict_materialization_details:
                 raise TypeError(
                     f"{error_msg} To suppress this exception, "
                     f"use strict_materialization_details=False"
                 )
             self.logger.error(error_msg)
 
+    def get_unlogged(self, materialization_details_label: str | None):
+        _ = materialization_details_label
+        return False  # only available for some dialects
+
     def get_create_table_suffix(self, materialization_details_label: str | None) -> str:
         """
         This method can be used to append materialization tables to CREATE TABLE
         statements by dialects that support it.
 
         :param materialization_details_label:
             A label that can be controlled on table or stage level to reference
             options layed out in detail in configuration
         :return:
             Suffix that is appended to CREATE TABLE statement as string
         """
         return ""
 
-    def add_indexes(
-        self, table: Table, schema: Schema, *, early_not_null_possible: bool = False
+    def get_limit_query(
+        self,
+        query: sa.sql.expression.Selectable | sa.sql.expression.TextClause,
+        rows: int,
+    ) -> sa.sql.expression.Select:
+        if isinstance(query, sa.sql.expression.TextClause):
+            return (
+                sa.select(sa.text("*"))
+                .limit(rows)
+                .select_from(sa.text("(" + str(query) + ") AS A"))
+            )
+        else:
+            return sa.select(sa.text("*")).limit(rows).select_from(query.alias("A"))
+
+    def lock_table(
+        self, table: Table | str, schema: Schema | str, conn: Any = None
+    ) -> list:
+        """
+        For some dialects, it might be beneficial to lock a table before writing to it.
+
+        :returns
+            A list of SQLAlchemy statements that should be executed if conn=None
+        """
+        _ = table, schema, conn
+        return []
+
+    def lock_source_table(
+        self, table: Table | str, schema: Schema | str, conn: Any = None
+    ) -> list:
+        """
+        For some dialects, it might be beneficial to lock source tables before reading.
+
+        :returns
+            A list of SQLAlchemy statements that should be executed if conn=None
+        """
+        _ = table, schema, conn
+        return []
+
+    def lock_source_tables(
+        self, tables: list[dict[str, str]], conn: Any = None
+    ) -> list:
+        """
+        For some dialects, it might be beneficial to lock source tables before reading.
+
+        :returns
+            A list of SQLAlchemy statements that should be executed if conn=None
+        """
+        stmts = []
+        for table in tables:
+            if table["shared_lock_allowed"]:
+                stmts += self.lock_source_table(table["name"], table["schema"], conn)
+        return stmts
+
+    def get_forced_nullability_columns(
+        self, table: Table, table_cols: Iterable[str]
+    ) -> tuple[list[str], list[str]]:
+        """
+        Get the columns that should be forced to be nullable or non-nullable.
+
+        This is typically applied on the materialized empty table, but may also
+        be applied after filling the table by some dialects. Some dialects may
+        choose to add primary key columns to non_nullable_cols if they need it
+        to set the primary key. However, some dialects do this separately because
+        they also need to change the type of primary key columns. Some dialects
+        only return non-nullable columns because all columns will be nullable
+        after initial materialization.
+
+        :param table:
+            Table to be materialized. It includes attributes like nullable,
+            non_nullable, and primary_key which may influence the return value.
+        :param table_cols:
+            The list of all columns in the table. If nullable and non_nullable is
+            specified, all columns must be mentioned. If only one of them is set,
+            the other one is calculated as the remaining set.
+        :return:
+            A tuple of two lists. The first list contains the columns that should
+            be forced to be nullable, the second list contains the columns that
+            should be forced to be non-nullable. Most dialects will not need to
+            force nullable columns because very column is nullable by default.
+        """
+        _, non_nullable_cols = self._process_table_nullable_parameters(
+            table, table_cols
+        )
+
+        # in most dialects columns are nullable by default
+        return [], non_nullable_cols
+
+    @staticmethod
+    def _process_table_nullable_parameters(table: Table, table_cols: Iterable[str]):
+        name = f'"{table.name}"'
+        nullable_set = set(table.nullable or [])
+        non_nullable_set = set(table.non_nullable or [])
+        table_cols_set = set(table_cols)
+
+        for prefix, col_set, cols in [
+            ("", nullable_set, table.nullable),
+            ("non_", non_nullable_set, table.non_nullable),
+        ]:
+            if invalid_cols := col_set - table_cols_set:
+                raise ValueError(
+                    f"The columns {invalid_cols} in Table({name},"
+                    f" {prefix}nullable={cols}) aren't contained in the table"
+                    f" columns: {table_cols}"
+                )
+
+        if table.nullable is not None and table.non_nullable is not None:
+            # If both are specified, they aren't allowed to intersect and
+            # their union must be the set of all columns.
+            if intersection := nullable_set & non_nullable_set:
+                raise ValueError(
+                    f"The columns {intersection} are both set to be nullable and non"
+                    f" nullable in Table({name}, nullable={table.nullable},"
+                    f" non_nullable={table.non_nullable})"
+                )
+            if missing_cols := table_cols_set - nullable_set - non_nullable_set:
+                raise ValueError(
+                    f"When setting Table({name}, nullable={table.nullable},"
+                    f" non_nullable={table.non_nullable}), all columns of the"
+                    f" table must be mentioned. Missing columns: {missing_cols}"
+                )
+            nullable = table.nullable
+            non_nullable = table.non_nullable
+        elif table.nullable is not None:
+            non_nullable = [c for c in table_cols if c not in nullable_set]
+            nullable = table.nullable
+        elif table.non_nullable is not None:
+            nullable = [c for c in table_cols if c not in non_nullable_set]
+            non_nullable = table.non_nullable
+        else:
+            nullable = []
+            non_nullable = []
+
+        return nullable, non_nullable
+
+    def dialect_requests_empty_creation(self, table: Table, is_sql: bool) -> bool:
+        _ = is_sql
+        return table.nullable is not None or table.non_nullable is not None
+
+    def add_indexes_and_set_nullable(
+        self,
+        table: Table,
+        schema: Schema,
+        *,
+        on_empty_table: bool | None = None,
+        table_cols: Iterable[str] | None = None,
     ):
-        if table.primary_key is not None:
-            key = table.primary_key
-            if isinstance(key, str):
-                key = [key]
-            self.add_primary_key(
-                table.name, schema, key, early_not_null_possible=early_not_null_possible
+        if on_empty_table is None or on_empty_table:
+            # By default, we set non-nullable on empty table
+            if table_cols is None:
+                # reflect table:
+                inspector = sa.inspect(self.engine)
+                columns = inspector.get_columns(table.name, schema=schema.get())
+                table_cols = [col["name"] for col in columns]
+            nullable_cols, non_nullable_cols = self.get_forced_nullability_columns(
+                table, table_cols
             )
+            if len(nullable_cols) > 0:
+                # some dialects represent literals as non-nullable types
+                self.execute(
+                    ChangeColumnNullable(
+                        table.name, schema, nullable_cols, nullable=True
+                    )
+                )
+            if len(non_nullable_cols) > 0:
+                self.execute(
+                    ChangeColumnNullable(
+                        table.name, schema, non_nullable_cols, nullable=False
+                    )
+                )
+        if on_empty_table is None or not on_empty_table:
+            # By default, we set indexes after loading full table. This can be
+            # overridden by dialect
+            self.add_table_primary_key(table, schema)
+            self.add_table_indexes(table, schema)
+
+    def add_table_indexes(self, table: Table, schema: Schema):
         if table.indexes is not None:
             for index in table.indexes:
                 self.add_index(table.name, schema, index)
 
+    def add_table_primary_key(self, table: Table, schema: Schema):
+        if table.primary_key is not None:
+            key = table.primary_key
+            if isinstance(key, str):
+                key = [key]
+            self.add_primary_key(table.name, schema, key)
+
     def add_primary_key(
         self,
         table_name: str,
         schema: Schema,
         key_columns: list[str],
         *,
         name: str | None = None,
-        early_not_null_possible: bool = False,
     ):
-        _ = early_not_null_possible  # only used for some dialects
         self.execute(AddPrimaryKey(table_name, schema, key_columns, name))
 
     def add_index(
         self,
         table_name: str,
         schema: Schema,
         index_columns: list[str],
@@ -551,15 +799,17 @@
         inspector = sa.inspect(self.engine)
         columns = inspector.get_columns(table_name, schema=schema.get())
         types = {d["name"]: d["type"] for d in columns}
         sql_types = [types[col] for col in col_names]
         return sql_types
 
     @staticmethod
-    def format_sql_string(query_str: str) -> str:
+    def format_sql_string(query_str: str, truncate_select=False) -> str:
+        if truncate_select and "SELECT" in query_str:
+            query_str = query_str.split("SELECT")[0] + "SELECT ...\n"
         return textwrap.dedent(query_str).strip()
 
     def execute_raw_sql(self, raw_sql: RawSql):
         """Executed raw SQL statements in the associated transaction stage"""
         for statement in raw_sql.sql.split(raw_sql.separator):
             if not statement.strip():
                 # Skip empty queries
@@ -805,31 +1055,22 @@
                 f"Can't copy table '{from_name}' (schema: '{from_schema}') to "
                 f"transaction because no such table exists.\n"
                 f"Tables in schema: {available_tables}"
             )
             self.logger.error(msg)
             raise CacheError(msg)
 
-        self.check_materialization_details_supported(
-            resolve_materialization_details_label(table)
-        )
-
-        self.execute(
-            CopyTable(
-                from_name,
-                from_schema,
-                table.name,
-                self.get_schema(table.stage.transaction_name),
-                early_not_null=table.primary_key,
-                suffix=self.get_create_table_suffix(
-                    resolve_materialization_details_label(table)
-                ),
-            )
-        )
-        self.add_indexes(table, self.get_schema(table.stage.transaction_name))
+        from_tbl = sa.Table(from_name, sa.MetaData(), schema=from_schema.get())
+        dest_tbl = table.copy_without_obj()
+        dest_tbl.obj = from_tbl
+        dest_tbl.shared_lock_allowed = True
+
+        # Copy table via executing a select statement with respective hook
+        hook = self.get_m_table_hook(type(dest_tbl.obj))
+        hook.materialize(self, dest_tbl, dest_tbl.stage.transaction_name)
 
     def _deferred_copy_table(
         self,
         table: Table,
         from_schema: Schema,
         from_name: str,
     ):
@@ -986,14 +1227,17 @@
                 for name in tables_to_copy:
                     self.execute(
                         CopyTable(
                             name,
                             src_schema,
                             name,
                             dest_schema,
+                            unlogged=self.get_unlogged(
+                                target_stage.materialization_details
+                            ),
                             suffix=self.get_create_table_suffix(
                                 target_stage.materialization_details
                             ),
                         ),
                         conn=conn,
                     )
                     self.copy_indexes(
@@ -1086,15 +1330,18 @@
     ) -> TaskMetadata:
         if self.disable_caching:
             raise CacheError(
                 "Caching is disabled, so we also don't even try to retrieve task"
                 f" cache: {task}"
             )
 
-        ignore_cache_function = ConfigContext.get().ignore_cache_function
+        ignore_cache_function = (
+            ConfigContext.get().cache_validation.mode
+            == CacheValidationMode.IGNORE_FRESH_INPUT
+        )
         try:
             with self.engine_connect() as conn:
                 result = (
                     conn.execute(
                         self.tasks_table.select()
                         .where(self.tasks_table.c.name == task.name)
                         .where(self.tasks_table.c.stage == task.stage.name)
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/backend/table/util/dtype.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/backend/table/util/dtype.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
+from collections.abc import Mapping
 from contextvars import ContextVar, Token
 from enum import Enum
 from functools import cached_property
 from threading import Lock
 from typing import TYPE_CHECKING, ClassVar
 
 import structlog
 from attrs import define, evolve, field, frozen
 from box import Box
 
+from pydiverse.pipedag.util import deep_merge
 from pydiverse.pipedag.util.import_ import import_object, load_object
 from pydiverse.pipedag.util.naming import NameDisambiguator
 
 if TYPE_CHECKING:
     from pydiverse.pipedag._typing import T
     from pydiverse.pipedag.backend import BaseLockManager
     from pydiverse.pipedag.context.run_context import StageLockStateHandler
@@ -96,18 +98,48 @@
     name_disambiguator: NameDisambiguator = field(factory=NameDisambiguator)
     override_version: str | None = None
 
     _context_var = ContextVar("task_context")
 
 
 class StageCommitTechnique(Enum):
+    """
+    - SCHEMA_SWAP: We prepare output in a `<stage>__tmp` schema and then swap
+      schemas for `<stage>` and `<stage>__tmp` with three rename operations.
+    - READ_VIEWS: We use two schemas, `<stage>__odd` and `<stage>__even`, and
+      fill schema `<stage>` just with views to one of those schemas.
+    """
+
     SCHEMA_SWAP = 0
     READ_VIEWS = 1
 
 
+class CacheValidationMode(Enum):
+    """
+    - NORMAL: Normal cache invalidation.
+    - ASSERT_NO_FRESH_INPUT: Same as IGNORE_FRESH_INPUT and additionally fail if tasks
+      having a cache function would still be executed (change in version or lazy query
+      ).
+    - IGNORE_FRESH_INPUT: Ignore the output of cache functions that help determine
+      the availability of fresh input. With `disable_cache_function=False`, it still
+      calls cache functions, so cache invalidation works interchangeably between
+      IGNORE_FRESH_INPUT and NORMAL.
+    - FORCE_FRESH_INPUT: Consider all cache function outputs as different and thus make
+      source tasks cache invalid.
+    - FORCE_CACHE_INVALID: Disable caching and thus force all tasks as cache invalid.
+      This option implies FORCE_FRESH_INPUT.
+    """
+
+    NORMAL = 0
+    ASSERT_NO_FRESH_INPUT = 1
+    IGNORE_FRESH_INPUT = 2
+    FORCE_FRESH_INPUT = 3
+    FORCE_CACHE_INVALID = 4
+
+
 @frozen(slots=False)
 class ConfigContext(BaseAttrsContext):
     """Configuration context for running a particular pipedag instance.
 
     To create a `ConfigContext` instance use :py:meth:`PipedagConfig.get`.
 
     ..
@@ -149,33 +181,27 @@
     pipedag_name: str
     flow_name: str | None
     instance_name: str
 
     # per instance attributes
     fail_fast: bool
     strict_result_get_locking: bool
-    ignore_task_version: bool
     instance_id: str  # may be used as database name or locking ID
     stage_commit_technique: StageCommitTechnique
+    cache_validation: Box
     network_interface: str
     disable_kroki: bool
     kroki_url: str | None
     attrs: Box
 
     table_hook_args: Box
 
-    # run specific options
-    ignore_cache_function: bool = False
-
     # INTERNAL FLAGS - ONLY FOR PIPEDAG USE
     # When set to True, exceptions raised in a flow don't get logged
     _swallow_exceptions: bool = False
-    # When set to True, indicates that all tasks should get run, independent
-    # of their cache validity
-    _force_task_execution: bool = False
 
     @cached_property
     def auto_table(self) -> tuple[type, ...]:
         return tuple(map(import_object, self._config_dict.get("auto_table", ())))
 
     @cached_property
     def auto_blob(self) -> tuple[type, ...]:
@@ -225,14 +251,19 @@
         new instance with some values mutated.
 
         Wrapper around |attrs.evolve()|_.
 
         .. |attrs.evolve()| replace:: ``attrs.evolve()``
         .. _attrs.evolve(): https://www.attrs.org/en/stable/api.html#attrs.evolve
         """
+        dicts = {}
+        for name, value in changes.items():
+            if isinstance(value, Mapping):
+                dicts[name] = deep_merge(getattr(self, name), value)
+        changes.update(dicts)
         evolved = evolve(self, **changes)
 
         # Transfer cached properties
         cached_properties = ["auto_table", "auto_blob", "store"]
         for name in cached_properties:
             if name in self.__dict__:
                 evolved.__dict__[name] = self.__dict__[name]
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/context/run_context.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/config.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing import TYPE_CHECKING, Any
 
 import sqlalchemy as sa
 import structlog
 import yaml
 from box import Box
 
+from pydiverse.pipedag.context.context import CacheValidationMode
 from pydiverse.pipedag.util.deep_merge import deep_merge
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.context import ConfigContext
 
 
 # noinspection PyPep8Naming
@@ -142,39 +143,57 @@
             default={
                 "fail_fast": False,
                 "network_interface": "127.0.0.1",
                 "disable_kroki": True,
                 "kroki_url": "https://kroki.io",
                 "per_user_template": "{id}_{username}",
                 "strict_result_get_locking": True,
-                "ignore_task_version": False,
+                "cache_validation": dict(
+                    mode="normal",
+                    disable_cache_function=False,
+                    ignore_task_version=False,
+                ),
                 "stage_commit_technique": "SCHEMA_SWAP",
                 "auto_table": [],
                 "auto_blob": [],
                 "attrs": {},
             },
         ).copy()
 
         # check enums
         # Alternative: could be a feature of __get_merged_config_dict
         # in case default value is set to Enum
         from pydiverse.pipedag.context.context import StageCommitTechnique
 
-        config["stage_commit_technique"] = (
-            config["stage_commit_technique"].strip().upper()
-        )
-        if not hasattr(StageCommitTechnique, config["stage_commit_technique"]):
-            raise ValueError(
-                "Found unknown setting stage_commit_technique:"
-                f" '{config['stage_commit_technique']}'; Expected one of:"
-                f" {', '.join([v.name for v in StageCommitTechnique])}"
-            )
+        for parent_cfg, enum_name, enum_type in [
+            (config, "stage_commit_technique", StageCommitTechnique),
+            (config["cache_validation"], "mode", CacheValidationMode),
+        ]:
+            parent_cfg[enum_name] = parent_cfg[enum_name].strip().upper()
+            if not hasattr(enum_type, parent_cfg[enum_name]):
+                raise ValueError(
+                    f"Found unknown setting {enum_name}: '{parent_cfg[enum_name]}';"
+                    f" Expected one of: {', '.join([v.name for v in enum_type])}"
+                )
         stage_commit_technique = getattr(
             StageCommitTechnique, config["stage_commit_technique"]
         )
+        cache_validation = copy.deepcopy(config["cache_validation"])
+        cache_validation["mode"] = getattr(
+            CacheValidationMode, config["cache_validation"]["mode"]
+        )
+
+        if (
+            cache_validation["mode"] == CacheValidationMode.NORMAL
+            and cache_validation["disable_cache_function"]
+        ):
+            raise ValueError(
+                "cache_validation.disable_cache_function=True is not allowed in "
+                "combination with cache_validation.mode=NORMAL"
+            )
 
         # TODO: Delegate selecting where variables can be expanded to the
         #  corresponding classes.
         #    eg. SQLTableStore._expand_env_vars = ["url", "url_attrs_file"]
         #    eg. SQLTableStore._expand_vars = ["url", "schema_prefix", "schema_suffix"]
 
         # First expand all environment variables
@@ -207,20 +226,20 @@
         config = self.__expand_variables(config)
 
         # Construct final ConfigContext
         config_context = ConfigContext(
             config_dict=config,
             pipedag_name=self.name,
             flow_name=flow,
-            strict_result_get_locking=config["strict_result_get_locking"],
-            ignore_task_version=config["ignore_task_version"],
             instance_name=instance,
+            fail_fast=config["fail_fast"],
+            strict_result_get_locking=config["strict_result_get_locking"],
             instance_id=config["instance_id"],
             stage_commit_technique=stage_commit_technique,
-            fail_fast=config["fail_fast"],
+            cache_validation=Box(cache_validation, frozen_box=True),
             network_interface=config["network_interface"],
             disable_kroki=config.get("disable_kroki"),
             kroki_url=config.get("kroki_url"),
             attrs=Box(config["attrs"], frozen_box=True),
             table_hook_args=Box(
                 config["table_store"].get("hook_args", {}), frozen_box=True
             ),
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/flow.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from pydiverse.pipedag.context import (
     ConfigContext,
     DAGContext,
     FinalTaskState,
     RunContextServer,
 )
+from pydiverse.pipedag.context.context import CacheValidationMode
 from pydiverse.pipedag.core.config import PipedagConfig
 from pydiverse.pipedag.errors import DuplicateNameError, FlowError
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core import Result, Stage, Task
     from pydiverse.pipedag.core.stage import CommitStageTask
     from pydiverse.pipedag.core.task import TaskGetItem
@@ -205,15 +206,17 @@
 
     def run(
         self,
         *components: Task | TaskGetItem | Stage,
         config: ConfigContext = None,
         orchestration_engine: OrchestrationEngine = None,
         fail_fast: bool | None = None,
-        ignore_cache_function: bool = False,
+        cache_validation_mode: CacheValidationMode | None = None,
+        disable_cache_function: bool | None = None,
+        ignore_task_version: bool | None = None,
         **kwargs,
     ) -> Result:
         """Execute the flow.
         This will execute the flow and all tasks within using the orchestration engine.
 
         :param components: An optional selection of tasks or stages that should
             get executed. If no values are provided, all tasks and stages get executed.
@@ -231,17 +234,27 @@
         :param orchestration_engine:
             The orchestration engine to use. If no engine is provided, the
             orchestration engine from the config gets used.
         :param fail_fast:
             Whether exceptions should get raised or swallowed.
             If set to True, exceptions that occur get immediately raised and the
             flow gets aborted.
-        :param ignore_cache_function:
-            When set to True, the task's cache function gets ignored when determining
-            the cache validity of a task.
+        :param cache_validation_mode:
+            Override the cache validation mode. See :py:class:`CacheValidationMode`.
+            For None, the cache validation mode from the config gets used.
+            See :doc:`/reference/config` :ref:`section-cache_validation` for more
+            information.
+        :param disable_cache_function:
+            Override the disable_cache_function setting from the config.
+            See :doc:`/reference/config` :ref:`section-cache_validation` for more
+            information.
+        :param ignore_task_version:
+            Override the ignore_task_version setting from the config.
+            See :doc:`/reference/config` :ref:`section-cache_validation` for more
+            information.
         :param kwargs:
             Other keyword arguments that get passed on directly to the
             ``run()`` method of the orchestration engine. Consequently, these
             keyword arguments are engine dependant.
         :return:
             A :py:class:`Result` object for the current flow run.
 
@@ -274,26 +287,44 @@
         # Get the ConfigContext to use
         if config is None:
             try:
                 config = ConfigContext.get()
             except LookupError:
                 config = PipedagConfig.default.get(flow=self.name)
 
+        # update cache_validation_mode
+        if cache_validation_mode is None and subflow.is_tasks_subflow:
+            # If subflow consists of a subset of tasks (-> not a subset of stages)
+            # then we want to skip cache validity checking to ensure the tasks
+            # always get executed.
+            cache_validation_mode = CacheValidationMode.FORCE_CACHE_INVALID
+
         # Evolve config using the arguments passed to flow.run
         config = config.evolve(
             fail_fast=(fail_fast if fail_fast is not None else config.fail_fast),
-            ignore_cache_function=ignore_cache_function,
-            force_task_execution=(
-                # If subflow consists of a subset of tasks (-> not a subset of stages)
-                # then we want to skip cache validity checking to ensure the tasks
-                # always get executed.
-                subflow.is_tasks_subflow
-            ),
+            cache_validation={
+                k: v
+                for k, v in [
+                    ("mode", cache_validation_mode),
+                    ("disable_cache_function", disable_cache_function),
+                    ("ignore_task_version", ignore_task_version),
+                ]
+                if v is not None
+            },
         )
 
+        if (
+            config.cache_validation.mode == CacheValidationMode.NORMAL
+            and config.cache_validation.disable_cache_function
+        ):
+            raise ValueError(
+                "disable_cache_function=True is not allowed in combination with "
+                f"cache_validation_mode=NORMAL: {config.cache_validation}"
+            )
+
         with config, RunContextServer(subflow):
             if orchestration_engine is None:
                 orchestration_engine = config.create_orchestration_engine()
             result = orchestration_engine.run(subflow, **kwargs)
 
             visualization_url = result.visualize_url()
             self.logger.info("Flow visualization", url=visualization_url)
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/result.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/stage.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/core/task.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/engine/dask.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/dask.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/management/cli.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/cli.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/management/commands/clear_metadata.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/clear_metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/management/commands/delete_schemas.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/management/commands/delete_schemas.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 @dataclass(frozen=True)
 class TaskCacheInfo:
     task: MaterializingTask
     input_hash: str
     cache_fn_hash: str
     cache_key: str
+    assert_no_materialization: bool
+    force_task_execution: bool
 
 
 def task_cache_key(task: MaterializingTask, input_hash: str, cache_fn_hash: str):
     """Cache key used to judge cache validity of the current task output.
 
     Also referred to as `task_hash`.
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/container.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     :param primary_key: Optional name of the primary key that should be
         used when materializing this table. Only supported by some table stores.
     :param indexes: Optional list of indexes to create. Each provided index should be
         a list of column names. Only supported by some table stores.
     :param type_map: Optional map of column names to types. Depending on the table
         store this will allow you to control the datatype as which the specified
         columns get materialized.
+    :param nullable: List of columns that should be nullable. If nullable is not None,
+        all other columns will be non-nullable.
+    :param non_nullable: List of columns that should be non-nullable. If non_nullable
+        is not None, all other columns will be nullable.
     :param materialization_details: The label of the materialization_details to be used.
         Overwrites the label given by the stage.
 
     .. seealso:: You can specify which types of objects should automatically get
         converted to tables using the :ref:`auto_table` config option.
     """
 
@@ -48,26 +52,30 @@
         self,
         obj: T | None = None,
         name: str | None = None,
         *,
         primary_key: str | list[str] | None = None,
         indexes: list[list[str]] | None = None,
         type_map: dict[str, Any] | None = None,
+        nullable: list[str] | None = None,
+        non_nullable: list[str] | None = None,
         materialization_details: str | None = None,
     ):
         self._name = None
         self.stage: Stage | None = None
         self.external_schema: str | None = None
         self.shared_lock_allowed: bool = True
 
         self.obj = obj
         self.name = name
         self.primary_key = primary_key
         self.indexes = indexes
         self.type_map = type_map
+        self.nullable = nullable
+        self.non_nullable = non_nullable
         self.materialization_details = materialization_details
 
         # Check that indexes is of type list[list[str]]
         indexes_type_error = TypeError(
             "Table argument 'indexes' must be of type list[list[str]]. "
             "Make sure you provide a 2d list, not just a 1d list."
         )
@@ -76,14 +84,26 @@
                 raise indexes_type_error
             for index in self.indexes:
                 if not isinstance(index, (list, tuple)):
                     raise indexes_type_error
                 for col in index:
                     if not isinstance(col, str):
                         raise indexes_type_error
+        for arg, name in [
+            (self.nullable, "nullable"),
+            (self.non_nullable, "non_nullable"),
+        ]:
+            type_error = TypeError(
+                f"Table argument '{name}' must be of type list[str]."
+            )
+            if arg is not None:
+                if not isinstance(arg, Iterable) or isinstance(arg, str):
+                    raise type_error
+                if not all(isinstance(x, str) for x in arg):
+                    raise type_error
 
         from pydiverse.pipedag.backend.table.sql import ExternalTableReference
 
         # ExternalTableReference can reference a table from an external schema
         if isinstance(self.obj, ExternalTableReference):
             self.external_schema = self.obj.schema
             if self.name is not None:
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/core.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import inspect
 import uuid
 from functools import partial
 from typing import TYPE_CHECKING, Any, Callable, overload
 
 from pydiverse.pipedag._typing import CallableT
 from pydiverse.pipedag.context import ConfigContext, RunContext, TaskContext
+from pydiverse.pipedag.context.context import CacheValidationMode
 from pydiverse.pipedag.core.task import Task, TaskGetItem, UnboundTask
 from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.materialize.cache import TaskCacheInfo, task_cache_key
 from pydiverse.pipedag.materialize.container import Blob, RawSql, Table
 from pydiverse.pipedag.util import deep_map
 from pydiverse.pipedag.util.computation_tracing import (
     ComputationTraceRef,
@@ -497,43 +498,74 @@
 
         # Compute the cache key for the task inputs
         input_json = store.json_encode(bound.arguments)
         input_hash = stable_hash("INPUT", input_json)
 
         cache_fn_hash = ""
         if task.cache is not None:
-            cache_fn_output = store.json_encode(task.cache(*args, **kwargs))
-            cache_fn_hash = stable_hash("CACHE_FN", cache_fn_output)
+            if config_context.cache_validation.disable_cache_function:
+                # choose random cache_fn_hash to ensure downstream tasks are
+                # invalidated for FORCE_FRESH_INPUT
+                cache_fn_hash = stable_hash("CACHE_FN", uuid.uuid4().hex)
+            else:
+                cache_fn_output = store.json_encode(task.cache(*args, **kwargs))
+                cache_fn_hash = stable_hash("CACHE_FN", cache_fn_output)
 
         memo_cache_key = task_cache_key(task, input_hash, cache_fn_hash)
 
         # Check if this task has already been run with the same inputs
         # If yes, return memoized result. This prevents DuplicateNameExceptions
         with run_context.task_memo(task, memo_cache_key) as (success, memo):
             if success:
                 task.logger.info(
                     "Task has already been run with the same inputs."
                     " Using memoized results."
                 )
 
                 return memo
 
-            if task.version is AUTO_VERSION:
-                assert not task.lazy
-
-                auto_version = self.compute_auto_version(task, store, bound)
-                task.version = auto_version
-                task.logger.info("Assigned auto version to task", version=auto_version)
-
             # Cache Lookup (only required if task isn't lazy)
-            force_task_execution = config_context._force_task_execution
+            force_task_execution = (
+                config_context.cache_validation.mode
+                == CacheValidationMode.FORCE_CACHE_INVALID
+                or (
+                    config_context.cache_validation.mode
+                    == CacheValidationMode.FORCE_FRESH_INPUT
+                    and task.cache is not None
+                )
+            )
             skip_cache_lookup = (
-                config_context.ignore_task_version or task.version is None
+                config_context.cache_validation.ignore_task_version
+                and task.version != AUTO_VERSION
+            ) or task.version is None
+            assert_no_fresh_input = (
+                config_context.cache_validation.mode
+                == CacheValidationMode.ASSERT_NO_FRESH_INPUT
             )
 
+            if task.version is AUTO_VERSION:
+                if (
+                    force_task_execution
+                    and config_context.cache_validation.disable_cache_function
+                ):
+                    task.version = None
+                    skip_cache_lookup = True
+                    task.logger.info(
+                        "Skipping determination of auto version of task due to forced "
+                        "execution and disable_cache_function=True"
+                    )
+                else:
+                    assert not task.lazy
+
+                    auto_version = self.compute_auto_version(task, store, bound)
+                    task.version = auto_version
+                    task.logger.info(
+                        "Assigned auto version to task", version=auto_version
+                    )
+
             if not task.lazy and not skip_cache_lookup and not force_task_execution:
                 try:
                     cached_output, cache_metadata = store.retrieve_cached_output(
                         task, input_hash, cache_fn_hash
                     )
                     store.copy_cached_output_to_transaction_stage(
                         cached_output, cache_metadata, task
@@ -542,28 +574,40 @@
                     task.logger.info("Found task in cache. Using cached result.")
                     TaskContext.get().is_cache_valid = True
                     return cached_output
                 except CacheError as e:
                     task.logger.info("Failed to retrieve task from cache", cause=str(e))
                     TaskContext.get().is_cache_valid = False
 
+            if not task.lazy:
+                if assert_no_fresh_input and task.cache is not None:
+                    raise AssertionError(
+                        "cache_validation.mode=ASSERT_NO_FRESH_INPUT is a "
+                        "protection mechanism to prevent execution of "
+                        "source tasks to keep pipeline input stable. However,"
+                        "this task was still triggered."
+                    ) from None
+
             if task.lazy:
                 # For lazy tasks, is_cache_valid gets set to false during the
                 # store.materialize_task procedure
                 TaskContext.get().is_cache_valid = True
 
-                if config_context.ignore_cache_function:
+                if (
+                    config_context.cache_validation.mode
+                    == CacheValidationMode.IGNORE_FRESH_INPUT
+                ):
                     # `cache_fn_hash` is not used for cache retrieval if
                     # ignore_cache_function is set to True.
                     # In that case, cache_metadata.cache_fn_hash may be different
                     # from the cache_fn_hash of the current task run.
 
                     try:
                         _, cache_metadata = store.retrieve_cached_output(
-                            task, input_hash, cache_fn_hash
+                            task, input_hash, ""
                         )
                         cache_fn_hash = cache_metadata.cache_fn_hash
                     except CacheError as e:
                         task.logger.info(
                             "Failed to retrieve task from cache", cause=str(e)
                         )
 
@@ -574,14 +618,16 @@
                 task.version = uuid.uuid4().hex
 
             task_cache_info = TaskCacheInfo(
                 task=task,
                 input_hash=input_hash,
                 cache_fn_hash=cache_fn_hash,
                 cache_key=task_cache_key(task, input_hash, cache_fn_hash),
+                assert_no_materialization=assert_no_fresh_input,
+                force_task_execution=force_task_execution,
             )
 
             # Compute the input_tables value of the TaskContext
             input_tables = []
 
             def _input_tables_visitor(x):
                 if isinstance(x, Table):
@@ -744,14 +790,16 @@
         self, task: MaterializingTask, store: PipeDAGStore, output
     ):
         task_cache_info = TaskCacheInfo(
             task=task,
             input_hash="AUTO_VERSION",
             cache_fn_hash="AUTO_VERSION",
             cache_key="AUTO_VERSION",
+            assert_no_materialization=False,
+            force_task_execution=False,
         )
 
         # Replace computation tracer proxy objects in output
         def replace_proxy(x):
             if isinstance(x, ComputationTracerProxy):
                 return {
                     "__pipedag_type__": "computation_tracer_proxy",
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/debug.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/debug.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/details.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/details.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/materialize/store.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/computation_tracing.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/computation_tracing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 But for snippets, license restrictions exist:
 https://www.ictrecht.nl/en/blog/what-is-the-license-status-of-stackoverflow-code-snippets
 """  # noqa: E501
 from __future__ import annotations
 
 from collections.abc import Iterable, Mapping
 
+from box import Box
+
 
 def deep_merge(x, y, check_enum=False):
-    if type(x) != type(y):
+    if type(x) != type(y) and not (isinstance(x, Mapping) and isinstance(y, Mapping)):
         raise TypeError(
             f"deep_merge failed due to type mismatch '{x}' (type: {type(x)}) vs. '{y}'"
             f" (type: {type(y)})"
         )
 
-    if isinstance(x, Mapping):
+    if isinstance(x, Box):
+        z = Box(_deep_merge_dict(x, y), frozen_box=True)
+    elif isinstance(x, Mapping):
         z = _deep_merge_dict(x, y)
     elif isinstance(x, Iterable) and not isinstance(x, str):
         z = _deep_merge_iterable(x, y)
     else:
         z = y  # update
 
     return z
```

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/hashing.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/hashing.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/import_.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/import_.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/ipc.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/json.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/json.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/naming.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/src/pydiverse/pipedag/util/structlog.py` & `pydiverse_pipedag-0.8.0/src/pydiverse/pipedag/util/structlog.py`

 * *Files identical despite different names*

### Comparing `pydiverse_pipedag-0.7.2/PKG-INFO` & `pydiverse_pipedag-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.7.2
+Version: 0.8.0
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -185,14 +185,14 @@
 (i.e. containerized Postgres), please look [here](https://pydiversepipedag.readthedocs.io/en/latest/database_testing.html).
 
 ## Troubleshooting
 
 ### Installing mssql odbc driver for linux
 
 Installing with
-instructions [here](https://docs.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server?view=sql-server-ver16#suse18)
+instructions [here](https://docs.microsoft.com/en-us/sql/connect/odbc/linux-mac/installing-the-microsoft-odbc-driver-for-sql-server)
 worked.
 But `odbcinst -j` revealed that it installed the configuration in `/etc/unixODBC/*`. But conda installed pyodbc brings
 its own `odbcinst` executable and that shows odbc config files are expected in `/etc/*`. Symlinks were enough to fix the
 problem. Try `python -c 'import pyodbc;print(pyodbc.drivers())'` and see whether you get more than an empty list.
 Furthermore, make sure you use 127.0.0.1 instead of localhost. It seems that /etc/hosts is ignored.
```

