# Comparing `tmp/dune_client-1.6.0.tar.gz` & `tmp/dune_client-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_client-1.6.0.tar", last modified: Tue Mar 19 12:40:56 2024, max compression
+gzip compressed data, was "dune_client-1.7.0.tar", last modified: Tue Apr  2 12:09:40 2024, max compression
```

## Comparing `dune_client-1.6.0.tar` & `dune_client-1.7.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.615543 dune_client-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-19 12:40:49.000000 dune_client-1.6.0/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.607543 dune_client-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.611543 dune_client-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-19 12:40:49.000000 dune_client-1.6.0/.github/workflows/pull-request.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-19 12:40:49.000000 dune_client-1.6.0/.github/workflows/py-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-19 12:40:49.000000 dune_client-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-19 12:40:49.000000 dune_client-1.6.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-19 12:40:49.000000 dune_client-1.6.0/COPYRIGHT.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-19 12:40:49.000000 dune_client-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-19 12:40:49.000000 dune_client-1.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-03-19 12:40:56.615543 dune_client-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-03-19 12:40:49.000000 dune_client-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.611543 dune_client-1.6.0/dune_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.615543 dune_client-1.6.0/dune_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/api/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/api/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/api/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/api/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/client_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.615543 dune_client-1.6.0/dune_client/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/file/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/file/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.615543 dune_client-1.6.0/dune_client/viz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-19 12:40:49.000000 dune_client-1.6.0/dune_client/viz/graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.615543 dune_client-1.6.0/dune_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-03-19 12:40:56.000000 dune_client-1.6.0/dune_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-19 12:40:56.000000 dune_client-1.6.0/dune_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 12:40:56.000000 dune_client-1.6.0/dune_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 12:40:56.000000 dune_client-1.6.0/dune_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-19 12:40:56.000000 dune_client-1.6.0/dune_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-19 12:40:56.000000 dune_client-1.6.0/dune_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-19 12:40:49.000000 dune_client-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.615543 dune_client-1.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-19 12:40:49.000000 dune_client-1.6.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-19 12:40:49.000000 dune_client-1.6.0/requirements/prod.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-19 12:40:56.615543 dune_client-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-19 12:40:49.000000 dune_client-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.607543 dune_client-1.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.615543 dune_client-1.6.0/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/e2e/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15678 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/e2e/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.615543 dune_client-1.6.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/fixtures/sample_table_insert.csv
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/fixtures/sample_table_insert.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 12:40:56.615543 dune_client-1.6.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/unit/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/unit/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/unit/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-19 12:40:49.000000 dune_client-1.6.0/tests/unit/test_viz_sankey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.863785 dune_client-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 12:09:33.000000 dune_client-1.7.0/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.851785 dune_client-1.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.855785 dune_client-1.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-02 12:09:33.000000 dune_client-1.7.0/.github/workflows/pull-request.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 12:09:33.000000 dune_client-1.7.0/.github/workflows/py-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 12:09:33.000000 dune_client-1.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 12:09:33.000000 dune_client-1.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-02 12:09:33.000000 dune_client-1.7.0/COPYRIGHT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 12:09:33.000000 dune_client-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 12:09:33.000000 dune_client-1.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-02 12:09:40.863785 dune_client-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-02 12:09:33.000000 dune_client-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.855785 dune_client-1.7.0/dune_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/dune_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16080 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/api/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/client_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/dune_client/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/file/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/dune_client/viz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-02 12:09:33.000000 dune_client-1.7.0/dune_client/viz/graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.863785 dune_client-1.7.0/dune_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 12:09:40.000000 dune_client-1.7.0/dune_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-02 12:09:33.000000 dune_client-1.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 12:09:33.000000 dune_client-1.7.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 12:09:33.000000 dune_client-1.7.0/requirements/prod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-02 12:09:40.863785 dune_client-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 12:09:33.000000 dune_client-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.851785 dune_client-1.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/e2e/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/e2e/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.859785 dune_client-1.7.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/fixtures/sample_table_insert.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/fixtures/sample_table_insert.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:09:40.863785 dune_client-1.7.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-02 12:09:33.000000 dune_client-1.7.0/tests/unit/test_viz_sankey.py
```

### Comparing `dune_client-1.6.0/.github/workflows/pull-request.yaml` & `dune_client-1.7.0/.github/workflows/pull-request.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/.github/workflows/py-publish.yaml` & `dune_client-1.7.0/.github/workflows/py-publish.yaml`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/LICENSE` & `dune_client-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/PKG-INFO` & `dune_client-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune_client
-Version: 1.6.0
+Version: 1.7.0
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/duneanalytics/dune-client
 Author: Benjamin H. Smith & Dune Analytics
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/duneanalytics/dune-client/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dune_client-1.6.0/README.md` & `dune_client-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/api/base.py` & `dune_client-1.7.0/dune_client/api/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,7 +205,18 @@
         response = self.http.patch(
             url=url,
             json=params,
             headers=self.default_headers(),
             timeout=self.request_timeout,
         )
         return self._handle_response(response)
+
+    def _delete(self, route: str) -> Any:
+        """Generic interface for the DELETE method of a Dune API request"""
+        url = self._route_url(route)
+        self.logger.debug(f"DELETE received input url={url}")
+        response = self.http.delete(
+            url=url,
+            headers=self.default_headers(),
+            timeout=self.request_timeout,
+        )
+        return self._handle_response(response)
```

### Comparing `dune_client-1.6.0/dune_client/api/execution.py` & `dune_client-1.7.0/dune_client/api/execution.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/api/extensions.py` & `dune_client-1.7.0/dune_client/api/extensions.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/api/query.py` & `dune_client-1.7.0/dune_client/api/query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/api/table.py` & `dune_client-1.7.0/dune_client/api/table.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """
 Table API endpoints enables users to
 create and insert data into Dune.
 """
 
 from __future__ import annotations
-from typing import List, Dict, Any, IO
+from typing import List, Dict, IO
 
 from dune_client.api.base import BaseRouter
-from dune_client.models import DuneError
+from dune_client.models import (
+    DuneError,
+    InsertTableResult,
+    CreateTableResult,
+    DeleteTableResult,
+)
 
 
 class TableAPI(BaseRouter):
     """
     Implementation of Table endpoints - Plus subscription only
     https://docs.dune.com/api-reference/tables/
     """
@@ -50,50 +55,61 @@
     def create_table(
         self,
         namespace: str,
         table_name: str,
         schema: List[Dict[str, str]],
         description: str = "",
         is_private: bool = False,
-    ) -> Any:
+    ) -> CreateTableResult:
         """
         https://docs.dune.com/api-reference/tables/endpoint/create
         The create table endpoint allows you to create an empty table
         with a specific schema in Dune.
 
         The only limitations are:
         - If a table already exists with the same name, the request will fail.
         - Column names in the table can’t start with a special character or a digit.
         """
 
-        return self._post(
+        result_json = self._post(
             route="/table/create",
             params={
                 "namespace": namespace,
                 "table_name": table_name,
                 "schema": schema,
                 "description": description,
                 "is_private": is_private,
             },
         )
+        return CreateTableResult.from_dict(result_json)
 
     def insert_table(
         self,
         namespace: str,
         table_name: str,
         data: IO[bytes],
         content_type: str,
-    ) -> Any:
+    ) -> InsertTableResult:
         """
         https://docs.dune.com/api-reference/tables/endpoint/insert
         The insert table endpoint allows you to insert data into an existing table in Dune.
 
         The only limitations are:
         - The file has to be in json or csv format
         - The file has to have the same schema as the table
         """
 
-        return self._post(
+        result_json = self._post(
             route=f"/table/{namespace}/{table_name}/insert",
             headers={"Content-Type": content_type},
             data=data,
         )
+        return InsertTableResult.from_dict(result_json)
+
+    def delete_table(self, namespace: str, table_name: str) -> DeleteTableResult:
+        """
+        https://docs.dune.com/api-reference/tables/endpoint/delete
+        The delete table endpoint allows you to delete an existing table in Dune.
+        """
+
+        response_json = self._delete(route=f"/table/{namespace}/{table_name}")
+        return DeleteTableResult.from_dict(response_json)
```

### Comparing `dune_client-1.6.0/dune_client/client.py` & `dune_client-1.7.0/dune_client/client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/client_async.py` & `dune_client-1.7.0/dune_client/client_async.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/file/base.py` & `dune_client-1.7.0/dune_client/file/base.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/file/interface.py` & `dune_client-1.7.0/dune_client/file/interface.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/interface.py` & `dune_client-1.7.0/dune_client/interface.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/models.py` & `dune_client-1.7.0/dune_client/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging.config
 from dataclasses import dataclass
 from datetime import datetime
 from enum import Enum
 from io import BytesIO
 from os import SEEK_END
 from typing import Optional, Any, Union, List, Dict
-
+from dataclasses_json import DataClassJsonMixin
 from dateutil.parser import parse
 
 from dune_client.types import DuneRecord
 
 log = logging.getLogger(__name__)
 logging.basicConfig(
     format="%(asctime)s %(levelname)s %(name)s %(message)s", level=logging.INFO
@@ -350,7 +350,37 @@
         assert self.execution_id == other.execution_id
         assert self.result is not None
         assert other.result is not None
         self.result += other.result
         self.next_uri = other.next_uri
         self.next_offset = other.next_offset
         return self
+
+
+@dataclass
+class CreateTableResult(DataClassJsonMixin):
+    """
+    Data type returned by table/create operation
+    """
+
+    example_query: str
+    full_name: str
+    namespace: str
+    table_name: str
+
+
+@dataclass
+class InsertTableResult(DataClassJsonMixin):
+    """
+    Data type returned by table/insert operation
+    """
+
+    rows_written: int
+
+
+@dataclass
+class DeleteTableResult(DataClassJsonMixin):
+    """
+    Data type returned by table/delete operation
+    """
+
+    message: str
```

### Comparing `dune_client-1.6.0/dune_client/query.py` & `dune_client-1.7.0/dune_client/query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/types.py` & `dune_client-1.7.0/dune_client/types.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/util.py` & `dune_client-1.7.0/dune_client/util.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client/viz/graphs.py` & `dune_client-1.7.0/dune_client/viz/graphs.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/dune_client.egg-info/PKG-INFO` & `dune_client-1.7.0/dune_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune_client
-Version: 1.6.0
+Version: 1.7.0
 Summary: A simple framework for interacting with Dune Analytics official API service.
 Home-page: https://github.com/duneanalytics/dune-client
 Author: Benjamin H. Smith & Dune Analytics
 Author-email: ben@cow.fi
 License: Apache License Version 2.0
 Project-URL: Tracker, https://github.com/duneanalytics/dune-client/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dune_client-1.6.0/dune_client.egg-info/SOURCES.txt` & `dune_client-1.7.0/dune_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/setup.cfg` & `dune_client-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/tests/e2e/test_async_client.py` & `dune_client-1.7.0/tests/e2e/test_async_client.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/tests/e2e/test_client.py` & `dune_client-1.7.0/tests/e2e/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import pandas
 
 from dune_client.models import (
     ExecutionState,
     ExecutionResponse,
     ExecutionStatusResponse,
     DuneError,
+    InsertTableResult,
+    CreateTableResult,
+    DeleteTableResult,
 )
 from dune_client.types import QueryParameter
 from dune_client.client import DuneClient
 from dune_client.query import QueryBase
 
 dotenv.load_dotenv()
 
@@ -121,15 +124,15 @@
         results = dune.run_query(new_query)
         self.assertEqual(
             results.get_rows(),
             [
                 {
                     "text_field": "different word",
                     "number_field": 22,
-                    "date_field": "1991-01-01T00:00:00Z",
+                    "date_field": "1991-01-01 00:00:00.000",
                     "list_field": "Option 2",
                 }
             ],
         )
 
     def test_endpoints(self):
         dune = DuneClient(self.valid_api_key)
@@ -220,27 +223,27 @@
         self.assertGreater(len(results), 0)
 
     def test_get_latest_result_with_query_id(self):
         dune = DuneClient(self.valid_api_key)
         results = dune.get_latest_result(self.query.query_id).get_rows()
         self.assertGreater(len(results), 0)
 
-    @unittest.skip("This is a plus subscription endpoint.")
+    @unittest.skip("Requires custom namespace and table_name input.")
     def test_upload_csv_success(self):
         client = DuneClient(self.valid_api_key)
         self.assertEqual(
             client.upload_csv(
                 table_name="e2e-test",
                 description="best data",
                 data="column1,column2\nvalue1,value2\nvalue3,value4",
             ),
             True,
         )
 
-    @unittest.skip("This is a plus subscription endpoint.")
+    @unittest.skip("Requires custom namespace and table_name input.")
     def test_create_table_success(self):
         # Make sure the table doesn't already exist.
         # You will need to change the namespace to your own.
         client = DuneClient(self.valid_api_key)
 
         namespace = "test"
         table_name = "dataset_e2e_test"
@@ -252,54 +255,77 @@
                 description="e2e test table",
                 schema=[
                     {"name": "date", "type": "timestamp"},
                     {"name": "dgs10", "type": "double"},
                 ],
                 is_private=False,
             ),
-            {
-                "namespace": namespace,
-                "table_name": table_name,
-                "full_name": f"dune.{namespace}.{table_name}",
-                "example_query": f"select * from dune.{namespace}.{table_name} limit 10",
-            },
+            CreateTableResult.from_dict(
+                {
+                    "namespace": namespace,
+                    "table_name": table_name,
+                    "full_name": f"dune.{namespace}.{table_name}",
+                    "example_query": f"select * from dune.{namespace}.{table_name} limit 10",
+                }
+            ),
         )
 
-    @unittest.skip("This is a plus subscription endpoint.")
+    @unittest.skip("Requires custom namespace and table_name input.")
     def test_insert_table_csv_success(self):
         # Make sure the table already exists and csv matches table schema.
         # You will need to change the namespace to your own.
         client = DuneClient(self.valid_api_key)
         with open("./tests/fixtures/sample_table_insert.csv", "rb") as data:
             self.assertEqual(
                 client.insert_table(
                     namespace="test",
                     table_name="dataset_e2e_test",
                     data=data,
                     content_type="text/csv",
                 ),
-                None,
+                InsertTableResult(rows_written=1),
             )
 
-    @unittest.skip("This is a plus subscription endpoint.")
+    @unittest.skip("Requires custom namespace and table_name input.")
     def test_insert_table_json_success(self):
         # Make sure the table already exists and json matches table schema.
         # You will need to change the namespace to your own.
         client = DuneClient(self.valid_api_key)
         with open("./tests/fixtures/sample_table_insert.json", "rb") as data:
             self.assertEqual(
                 client.insert_table(
                     namespace="test",
                     table_name="dataset_e2e_test",
                     data=data,
                     content_type="application/x-ndjson",
                 ),
-                None,
+                InsertTableResult(rows_written=1),
             )
 
+    @unittest.skip("Requires custom namespace and table_name input.")
+    def test_delete_table_success(self):
+        # Make sure the table doesn't already exist.
+        # You will need to change the namespace to your own.
+        client = DuneClient(self.valid_api_key)
+
+        namespace = "test"
+        table_name = "dataset_e2e_test"
+
+        self.assertEqual(
+            client.delete_table(
+                namespace=namespace,
+                table_name=table_name,
+            ),
+            DeleteTableResult.from_dict(
+                {
+                    "message": "Table teamwaddah.waddah_test3 successfully deleted",
+                }
+            ),
+        )
+
     def test_download_csv_with_pagination(self):
         # Arrange
         client = DuneClient(self.valid_api_key)
         client.run_query(self.multi_rows_query)
 
         # Act
         result_csv = client.download_csv(self.multi_rows_query.query_id, batch_size=1)
@@ -346,15 +372,15 @@
         # Expect that the csv returns the latest execution results (i.e. those that were just run)
         self.assertEqual(
             pandas.read_csv(result_csv.data).to_dict(orient="records"),
             [
                 {
                     "text_field": "different word",
                     "number_field": 22,
-                    "date_field": "1991-01-01T00:00:00Z",
+                    "date_field": "1991-01-01 00:00:00.000",
                     "list_field": "Option 2",
                 }
             ],
         )
 
     def test_download_csv_success_with_params(self):
         client = DuneClient(self.valid_api_key)
@@ -368,15 +394,15 @@
         # Specifically 1991-01-01 00:00:00.000
         #           vs 1991-01-01 00:00:00
         #################################################################
         self.assertEqual(
             pandas.read_csv(result_csv.data).to_dict(orient="records"),
             [
                 {
-                    "date_field": "2022-05-04T00:00:00Z",
+                    "date_field": "2022-05-04 00:00:00.000",
                     "list_field": "Option 1",
                     "number_field": 3.1415926535,
                     "text_field": "Plain Text",
                 }
             ],
         )
```

### Comparing `dune_client-1.6.0/tests/unit/test_file.py` & `dune_client-1.7.0/tests/unit/test_file.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/tests/unit/test_models.py` & `dune_client-1.7.0/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/tests/unit/test_query.py` & `dune_client-1.7.0/tests/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/tests/unit/test_types.py` & `dune_client-1.7.0/tests/unit/test_types.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/tests/unit/test_utils.py` & `dune_client-1.7.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dune_client-1.6.0/tests/unit/test_viz_sankey.py` & `dune_client-1.7.0/tests/unit/test_viz_sankey.py`

 * *Files identical despite different names*

