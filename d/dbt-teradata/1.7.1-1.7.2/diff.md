# Comparing `tmp/dbt-teradata-1.7.1.tar.gz` & `tmp/dbt-teradata-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-teradata-1.7.1.tar", last modified: Thu Jan 11 18:01:12 2024, max compression
+gzip compressed data, was "dbt-teradata-1.7.2.tar", last modified: Tue Apr  2 12:15:40 2024, max compression
```

## Comparing `dbt-teradata-1.7.1.tar` & `dbt-teradata-1.7.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.093882 dbt-teradata-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    23794 2024-01-11 18:01:12.093882 dbt-teradata-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23577 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.085882 dbt-teradata-1.7.1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.085882 dbt-teradata-1.7.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.089882 dbt-teradata-1.7.1/dbt/adapters/teradata/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/adapters/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-11 18:01:09.000000 dbt-teradata-1.7.1/dbt/adapters/teradata/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/adapters/teradata/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/adapters/teradata/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/adapters/teradata/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/adapters/teradata/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.085882 dbt-teradata-1.7.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.089882 dbt-teradata-1.7.1/dbt/include/teradata/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.089882 dbt-teradata-1.7.1/dbt/include/teradata/macros/
--rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/columns.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.085882 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.089882 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.089882 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/seed/
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.089882 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/snapshot/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.089882 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/test/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/test/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/show.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.093882 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/generate_series.sql
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/type_string.sql
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-11 18:00:42.000000 dbt-teradata-1.7.1/dbt/include/teradata/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:01:12.093882 dbt-teradata-1.7.1/dbt_teradata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23794 2024-01-11 18:01:12.000000 dbt-teradata-1.7.1/dbt_teradata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-01-11 18:01:12.000000 dbt-teradata-1.7.1/dbt_teradata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 18:01:12.000000 dbt-teradata-1.7.1/dbt_teradata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-11 18:01:12.000000 dbt-teradata-1.7.1/dbt_teradata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-11 18:01:12.000000 dbt-teradata-1.7.1/dbt_teradata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 18:01:12.093882 dbt-teradata-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-01-11 18:01:09.000000 dbt-teradata-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.661891 dbt-teradata-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    23794 2024-04-02 12:15:40.661891 dbt-teradata-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23577 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.653890 dbt-teradata-1.7.2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.653890 dbt-teradata-1.7.2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.657891 dbt-teradata-1.7.2/dbt/adapters/teradata/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/adapters/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 12:15:38.000000 dbt-teradata-1.7.2/dbt/adapters/teradata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/adapters/teradata/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/adapters/teradata/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12666 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/adapters/teradata/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/adapters/teradata/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.653890 dbt-teradata-1.7.2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.657891 dbt-teradata-1.7.2/dbt/include/teradata/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.657891 dbt-teradata-1.7.2/dbt/include/teradata/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/columns.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.653890 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.657891 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.657891 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/seed/
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.657891 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/snapshot/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.657891 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/test/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/show.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.661891 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/generate_series.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/type_string.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-02 12:15:05.000000 dbt-teradata-1.7.2/dbt/include/teradata/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:15:40.661891 dbt-teradata-1.7.2/dbt_teradata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23794 2024-04-02 12:15:40.000000 dbt-teradata-1.7.2/dbt_teradata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-02 12:15:40.000000 dbt-teradata-1.7.2/dbt_teradata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:15:40.000000 dbt-teradata-1.7.2/dbt_teradata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-02 12:15:40.000000 dbt-teradata-1.7.2/dbt_teradata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 12:15:40.000000 dbt-teradata-1.7.2/dbt_teradata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:15:40.661891 dbt-teradata-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-02 12:15:38.000000 dbt-teradata-1.7.2/setup.py
```

### Comparing `dbt-teradata-1.7.1/LICENSE` & `dbt-teradata-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/PKG-INFO` & `dbt-teradata-1.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.7.1
+Version: 1.7.2
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dbt-teradata-1.7.1/README.md` & `dbt-teradata-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/adapters/teradata/__init__.py` & `dbt-teradata-1.7.2/dbt/adapters/teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/adapters/teradata/column.py` & `dbt-teradata-1.7.2/dbt/adapters/teradata/column.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/adapters/teradata/connections.py` & `dbt-teradata-1.7.2/dbt/adapters/teradata/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,22 +333,25 @@
                 # useful information, so raise it without modification.
                 raise
 
             raise dbt.exceptions.DbtRuntimeError(e) from e
 
     @classmethod
     def get_response(cls, cursor):
-        # There's no real way to get this from teradatasql, so just return "OK"
         num_rows = 0
+        activity = "success"
+        message = "OK"
         if cursor is not None and cursor.rowcount is not None:
-          num_rows = cursor.rowcount
+            num_rows = cursor.rowcount
+            activity = cursor.activityname
+            message = "activity: {}, rows_affected: {}".format(cursor.activityname, cursor.rowcount)
         return AdapterResponse(
-          _message="OK",
-          rows_affected = num_rows,
-          code='SUCCESS'
+          _message=message,
+          rows_affected=num_rows,
+          code=activity
         )
     '''
     overriding add_query method to disable
     transactional logic for dbt-teradata
     '''
     def add_query(
         self,
```

### Comparing `dbt-teradata-1.7.1/dbt/adapters/teradata/impl.py` & `dbt-teradata-1.7.2/dbt/adapters/teradata/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/adapters/teradata/relation.py` & `dbt-teradata-1.7.2/dbt/adapters/teradata/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/adapters.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/adapters.sql`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
       , {{ table_option }}
       {%- endif -%}
 
       {# below macro compares the contract information in schema and sql file of model #}
       {{ get_assert_columns_equivalent(sql) }}
 
       {# below macro loop through user_provided_columns to create DDL with data types and constraints #}
-      {{ get_table_columns_and_constraints() }} ;
+      {{ get_table_columns_and_constraints() }}
 
       {%- if with_statistics -%}
       AND STATISTICS
       {%- endif %}
       {% if index |length -%}
         {{ index }}
       {%- endif -%};
@@ -53,37 +53,52 @@
 
     insert into {{ relation }} (
       {{ adapter.dispatch('get_column_names', 'dbt')() }}
     )
     {{ get_select_subquery(sql) }}
     ;
   {% else %}
+    {#- Changing the code of this macro as in rows_affected are not getting populated in run_results.json -#}
+    {#- Changing it from (create table as) to (create with no data + insert+select) -#}
     {{ sql_header if sql_header is not none }}
-    CREATE {{ table_kind }} TABLE
-    {{ relation.include(database=False) }}
-    {% if table_option |length -%}
-    , {{ table_option }}
-    {%- endif -%}
-    {% if sql.strip().upper().startswith('WITH') %}
-      AS (
+    {% call statement('create_table') %}
+      CREATE {{ table_kind }} TABLE
+      {{ relation.include(database=False) }}
+      {% if table_option |length -%}
+      , {{ table_option }}
+      {%- endif -%}
+      {% if sql.strip().upper().startswith('WITH') %}
+        AS (
+          SELECT * FROM (
+            {{ sql }}
+          ) D
+        ) with no data
+      {% else %}
+        AS (
+            {{ sql }}
+          )with no data
+      {% endif %}
+      {%- if with_statistics -%}
+        AND STATISTICS
+      {%- endif %}
+      {% if index |length -%}
+        {{ index }}
+      {%- endif -%};
+    {% endcall %}
+
+    insert into {{ relation }}
+      {% if sql.strip().upper().startswith('WITH') %}
+
         SELECT * FROM (
           {{ sql }}
-        ) D
-      ) WITH DATA
+      ) D
     {% else %}
-      AS (
           {{ sql }}
-        ) WITH DATA
     {% endif %}
-    {%- if with_statistics -%}
-      AND STATISTICS
-    {%- endif %}
-    {% if index |length -%}
-    {{ index }}
-    {%- endif -%};
+    ;
   {% endif %}
 {% endmacro %}
 
 {% macro teradata__create_view_as(relation, sql) -%}
   {%- set sql_header = config.get('sql_header', none) -%}
   {% set contract_config = config.get('contract') %}
   {% if contract_config.enforced %}
@@ -163,14 +178,15 @@
         WHEN ColumnsV.ColumnType = 'I2' THEN 'SMALLINT'
         WHEN ColumnsV.ColumnType = 'AT' THEN 'TIME'
         WHEN ColumnsV.ColumnType = 'TS' THEN 'TIMESTAMP'
         WHEN ColumnsV.ColumnType = 'TZ' THEN 'TIME WITH TIME ZONE'
         WHEN ColumnsV.ColumnType = 'SZ' THEN 'TIMESTAMP WITH TIME ZONE'
         WHEN ColumnsV.ColumnType = 'UT' THEN 'USER‑DEFINED TYPE'
         WHEN ColumnsV.ColumnType = 'XM' THEN 'XML'
+        WHEN ColumnsV.ColumnType = 'JN' THEN 'JSON'
         ELSE 'N/A'
       END AS dtype,
       CASE
         WHEN ColumnsV.CharType = 1 THEN ColumnsV.ColumnLength
       END AS char_size,
       ColumnsV.DecimalTotalDigits AS numeric_precision,
       ColumnsV.DecimalFractionalDigits AS numeric_scale,
```

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/apply_grants.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/catalog.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/columns.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/incremental/helpers.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/incremental/incremental.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/incremental/strategies.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/incremental/strategies.sql`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 {% endmacro %}
 
 
 {% macro teradata__get_delete_insert_merge_sql(target_relation, tmp_relation, unique_key, dest_columns, incremental_predicates) %}
     {%- set dest_cols_csv = dest_columns | map(attribute='quoted') | join(', ') -%}
 
     {%- if unique_key -%}
+    {% call statement('delete_table') %}
         {% if unique_key is sequence and unique_key is not string %}
             delete from {{target_relation }}
             where (
                 {% for key in unique_key %}
                     {{ tmp_relation }}.{{ key }} = {{ target_relation }}.{{ key }}
                     {{ "and " if not loop.last}}
                 {% endfor %}
@@ -51,17 +52,16 @@
             {%- if incremental_predicates %}
                 {% for predicate in incremental_predicates %}
                     and {{ predicate }}
                 {% endfor %}
             {%- endif -%};
 
         {% endif %}
-        
+    {% endcall %}
     {%- endif %}
-
     INSERT INTO {{ target_relation }} ({{ dest_cols_csv }})
        SELECT {{ dest_cols_csv }}
        FROM {{ tmp_relation }}
     ;
 {%- endmacro %}
```

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/seed/seed.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/snapshot/helpers.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/snapshot/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/snapshot/strategies.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/materializations/test/test.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/metadata.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/dateadd.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/datediff.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/generate_series.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/generate_series.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt/include/teradata/macros/utils/split_part.sql` & `dbt-teradata-1.7.2/dbt/include/teradata/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/dbt_teradata.egg-info/PKG-INFO` & `dbt-teradata-1.7.2/dbt_teradata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.7.1
+Version: 1.7.2
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dbt-teradata-1.7.1/dbt_teradata.egg-info/SOURCES.txt` & `dbt-teradata-1.7.2/dbt_teradata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.7.1/setup.py` & `dbt-teradata-1.7.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 package_name = "dbt-teradata"
-package_version = "1.7.1"
+package_version = "1.7.2"
 description = """The Teradata adapter plugin for dbt (data build tool)"""
 
 
 setup(
     name=package_name,
     version=package_version,
 
@@ -42,15 +42,15 @@
             'macros/materializations/**/*.sql',
             'macros/utils/*.sql',
             'dbt_project.yml',
             'sample_profiles.yml',
         ],
     },
     install_requires=[
-        "dbt-core==1.7.4",
+        "dbt-core==1.7.11",
         "teradatasql>=16.20.0.0",
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
 
         'License :: OSI Approved :: Apache Software License',
```

