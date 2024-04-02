# Comparing `tmp/clickhouse-connect-0.7.5.tar.gz` & `tmp/clickhouse-connect-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.7.5.tar", last modified: Thu Mar 28 20:33:16 2024, max compression
+gzip compressed data, was "clickhouse-connect-0.7.6.tar", last modified: Tue Apr  2 00:36:41 2024, max compression
```

## Comparing `clickhouse-connect-0.7.5.tar` & `clickhouse-connect-0.7.6.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.082875 clickhouse-connect-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-28 20:33:16.082875 clickhouse-connect-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.074875 clickhouse-connect-0.7.5/clickhouse_connect/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.074875 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.074875 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13683 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.074875 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.074875 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.078875 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/special.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/datatypes/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.078875 clickhouse-connect-0.7.5/clickhouse_connect/dbapi/
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/dbapi/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.082875 clickhouse-connect-0.7.5/clickhouse_connect/driver/
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    41812 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/dataconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/ddl.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/external.py
--rw-r--r--   0 runner    (1001) docker     (127)    22430 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/httputil.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/insert.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/npconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/npquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    20670 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driver/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.082875 clickhouse-connect-0.7.5/clickhouse_connect/driverc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driverc/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driverc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driverc/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driverc/buffer.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driverc/dataconv.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/driverc/npconv.pyx
--rwxr-xr-x   0 runner    (1001) docker     (127)     1163 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/json_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.082875 clickhouse-connect-0.7.5/clickhouse_connect/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/tools/datagen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/clickhouse_connect/tools/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 20:33:16.074875 clickhouse-connect-0.7.5/clickhouse_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-03-28 20:33:16.000000 clickhouse-connect-0.7.5/clickhouse_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-03-28 20:33:16.000000 clickhouse-connect-0.7.5/clickhouse_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 20:33:16.000000 clickhouse-connect-0.7.5/clickhouse_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 20:33:16.000000 clickhouse-connect-0.7.5/clickhouse_connect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 20:33:16.000000 clickhouse-connect-0.7.5/clickhouse_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-28 20:33:16.000000 clickhouse-connect-0.7.5/clickhouse_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 20:33:16.082875 clickhouse-connect-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-28 20:33:14.000000 clickhouse-connect-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.738039 clickhouse-connect-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-02 00:36:41.738039 clickhouse-connect-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.730039 clickhouse-connect-0.7.6/clickhouse_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.730039 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.730039 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.730039 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.734039 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.734039 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/datatypes/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.734039 clickhouse-connect-0.7.6/clickhouse_connect/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/dbapi/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.738039 clickhouse-connect-0.7.6/clickhouse_connect/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41812 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/dataconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22430 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/httputil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/npconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/npquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20682 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driver/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.738039 clickhouse-connect-0.7.6/clickhouse_connect/driverc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driverc/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driverc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driverc/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driverc/buffer.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driverc/dataconv.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/driverc/npconv.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1163 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/json_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.738039 clickhouse-connect-0.7.6/clickhouse_connect/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/tools/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/clickhouse_connect/tools/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:36:41.730039 clickhouse-connect-0.7.6/clickhouse_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-02 00:36:41.000000 clickhouse-connect-0.7.6/clickhouse_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-02 00:36:41.000000 clickhouse-connect-0.7.6/clickhouse_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:36:41.000000 clickhouse-connect-0.7.6/clickhouse_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 00:36:41.000000 clickhouse-connect-0.7.6/clickhouse_connect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 00:36:41.000000 clickhouse-connect-0.7.6/clickhouse_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 00:36:41.000000 clickhouse-connect-0.7.6/clickhouse_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:36:41.738039 clickhouse-connect-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-02 00:36:40.000000 clickhouse-connect-0.7.6/setup.py
```

### Comparing `clickhouse-connect-0.7.5/LICENSE` & `clickhouse-connect-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/PKG-INFO` & `clickhouse-connect-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.7.5
+Version: 0.7.6
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.7.5/README.md` & `clickhouse-connect-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/datatypes/base.py` & `clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
         SqlaDateTime.__init__(self)
 
 
 class DateTime64(ChSqlaType, SqlaDateTime):
     def __init__(self, precision: int = None, tz: str = None, type_def: TypeDef = None):
         """
         Date time constructor with precision and timezone parameters if not constructed with TypeDef
-        :param precision:   Usually 3/6/9 for mill/micro/nansecond precision on ClickHouse side
+        :param precision:   Usually 3/6/9 for mill/micro/nanosecond precision on ClickHouse side
         :param tz: Timezone string as defined in pytz
         :param type_def: TypeDef from parse_name function
         """
         if not type_def:
             if tz:
                 pytz.timezone(tz)
                 type_def = TypeDef(values=(precision, f"'{tz}'"))
```

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/ddl/custom.py` & `clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py` & `clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,18 @@
     def __init__(self, order_by: str = None, primary_key: str = None,
                  partition_by: str = None, sample_by: str = None):
         if not order_by and not primary_key:
             raise ArgumentError(None, 'Either PRIMARY KEY or ORDER BY must be specified')
         super().__init__(locals())
 
 
+class SharedMergeTree(MergeTree):
+    pass
+
+
 class SummingMergeTree(MergeTree):
     pass
 
 
 class AggregatingMergeTree(MergeTree):
     pass
```

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/dialect.py` & `clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/inspector.py` & `clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `clickhouse-connect-0.7.6/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/common.py` & `clickhouse-connect-0.7.6/clickhouse_connect/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/datatypes/base.py` & `clickhouse-connect-0.7.6/clickhouse_connect/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/datatypes/container.py` & `clickhouse-connect-0.7.6/clickhouse_connect/datatypes/container.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/datatypes/format.py` & `clickhouse-connect-0.7.6/clickhouse_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/datatypes/network.py` & `clickhouse-connect-0.7.6/clickhouse_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/datatypes/numeric.py` & `clickhouse-connect-0.7.6/clickhouse_connect/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/datatypes/registry.py` & `clickhouse-connect-0.7.6/clickhouse_connect/datatypes/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     elif base.startswith('Nested'):
         keys, values = parse_columns(base[6:])
         base = 'Nested'
     elif base.startswith('Tuple'):
         keys, values = parse_columns(base[5:])
         base = 'Tuple'
     elif base == 'Point':
-        values = ['Float64', 'Float64']
+        values = ('Float64', 'Float64')
     else:
         try:
             base, values, _ = parse_callable(base)
         except IndexError:
             raise InternalError(f'Can not parse ClickHouse data type: {name}') from None
     return base, name, TypeDef(tuple(wrappers), keys, values)
```

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/datatypes/special.py` & `clickhouse-connect-0.7.6/clickhouse_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/datatypes/string.py` & `clickhouse-connect-0.7.6/clickhouse_connect/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/datatypes/temporal.py` & `clickhouse-connect-0.7.6/clickhouse_connect/datatypes/temporal.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/dbapi/__init__.py` & `clickhouse-connect-0.7.6/clickhouse_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/dbapi/connection.py` & `clickhouse-connect-0.7.6/clickhouse_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/dbapi/cursor.py` & `clickhouse-connect-0.7.6/clickhouse_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/__init__.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/buffer.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/client.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/client.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/common.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/compression.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/context.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/context.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/ctypes.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/dataconv.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/dataconv.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/ddl.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/exceptions.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/external.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/external.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/httpclient.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/httpclient.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/httputil.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/httputil.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/insert.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/insert.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/models.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/npquery.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/npquery.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/options.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/parser.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/query.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,15 +335,15 @@
             self.source = None
         if self._block_gen is not None:
             self._block_gen.close()
             self._block_gen = None
 
 
 BS = '\\'
-must_escape = (BS, '\'', '`')
+must_escape = (BS, '\'', '`', '\t', '\n')
 
 
 def quote_identifier(identifier: str):
     first_char = identifier[0]
     if first_char in ('`', '"') and identifier[-1] == first_char:
         # Identifier is already quoted, assume that it's valid
         return identifier
```

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/summary.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/summary.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/tools.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/tools.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/transform.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/transform.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driver/types.py` & `clickhouse-connect-0.7.6/clickhouse_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driverc/buffer.pxd` & `clickhouse-connect-0.7.6/clickhouse_connect/driverc/buffer.pxd`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driverc/buffer.pyx` & `clickhouse-connect-0.7.6/clickhouse_connect/driverc/buffer.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/driverc/dataconv.pyx` & `clickhouse-connect-0.7.6/clickhouse_connect/driverc/dataconv.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/entry_points.py` & `clickhouse-connect-0.7.6/clickhouse_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/json_impl.py` & `clickhouse-connect-0.7.6/clickhouse_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/tools/datagen.py` & `clickhouse-connect-0.7.6/clickhouse_connect/tools/datagen.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect/tools/testing.py` & `clickhouse-connect-0.7.6/clickhouse_connect/tools/testing.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect.egg-info/PKG-INFO` & `clickhouse-connect-0.7.6/clickhouse_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.7.5
+Version: 0.7.6
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.7.5/clickhouse_connect.egg-info/SOURCES.txt` & `clickhouse-connect-0.7.6/clickhouse_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.5/setup.py` & `clickhouse-connect-0.7.6/setup.py`

 * *Files identical despite different names*

