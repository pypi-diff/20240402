# Comparing `tmp/dbt-odps-winwin-1.0.8.tar.gz` & `tmp/dbt-odps-winwin-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-odps-winwin-1.0.8.tar", last modified: Tue Jan  9 08:04:50 2024, max compression
+gzip compressed data, was "dbt-odps-winwin-1.0.9.tar", last modified: Thu Feb  1 23:04:26 2024, max compression
```

## Comparing `dbt-odps-winwin-1.0.8.tar` & `dbt-odps-winwin-1.0.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.271290 dbt-odps-winwin-1.0.8/
--rw-r--r--   0 leezhongshan   (501) staff       (20)       47 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/MANIFEST.in
--rw-r--r--   0 leezhongshan   (501) staff       (20)     4041 2024-01-09 08:04:50.271216 dbt-odps-winwin-1.0.8/PKG-INFO
--rw-r--r--   0 leezhongshan   (501) staff       (20)     3710 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/README.md
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.261113 dbt-odps-winwin-1.0.8/dbt/
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.261044 dbt-odps-winwin-1.0.8/dbt/adapters/
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.263992 dbt-odps-winwin-1.0.8/dbt/adapters/odps/
--rw-r--r--   0 leezhongshan   (501) staff       (20)      621 2023-12-18 07:33:56.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/__init__.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)       18 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/__version__.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)     2087 2023-12-18 07:33:56.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/colums.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)     5079 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/connections.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)     3752 2024-01-09 07:08:04.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/date.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)     1961 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/dbapi.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)      175 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/errors.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)     7604 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/impl.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)     1566 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/relation.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)     1556 2024-01-09 07:08:04.000000 dbt-odps-winwin-1.0.8/dbt/adapters/odps/utils.py
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.261160 dbt-odps-winwin-1.0.8/dbt/include/
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.265060 dbt-odps-winwin-1.0.8/dbt/include/odps/
--rw-r--r--   0 leezhongshan   (501) staff       (20)       52 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/__init__.py
--rw-r--r--   0 leezhongshan   (501) staff       (20)       73 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/dbt_project.yml
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.265691 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/
--rw-r--r--   0 leezhongshan   (501) staff       (20)    11570 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/adapters.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     1553 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/apply_grants.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      982 2023-12-18 07:33:56.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/catalog.sql
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.266340 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.267111 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/incremental/
--rw-r--r--   0 leezhongshan   (501) staff       (20)     4729 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     2378 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/incremental/on_schema_change.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     6034 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     2070 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/incremental/validate.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     4354 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/seed.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     6916 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/snapshot.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     2795 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/table.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      697 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/view.sql
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.270263 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/
--rw-r--r--   0 leezhongshan   (501) staff       (20)      719 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/any_value.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      192 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/array_append.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      127 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/array_concat.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      425 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/array_construct.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      665 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/bool_or.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      720 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      669 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/concat.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      682 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/date_trunc.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     1077 2024-01-09 07:08:04.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/dateadd.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     3069 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/datediff.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      428 2024-01-09 08:02:06.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/dateutil.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      689 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      742 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/hash.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     1208 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/last_day.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      514 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/listagg.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      724 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/position.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      896 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/right.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)     1140 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/split_part.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      662 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/timestamps.sql
--rw-r--r--   0 leezhongshan   (501) staff       (20)      292 2024-01-09 07:08:04.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/macros.yml
--rw-r--r--   0 leezhongshan   (501) staff       (20)      476 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.8/dbt/include/odps/profile_template.yml
-drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-01-09 08:04:50.270984 dbt-odps-winwin-1.0.8/dbt_odps_winwin.egg-info/
--rw-r--r--   0 leezhongshan   (501) staff       (20)     4041 2024-01-09 08:04:50.000000 dbt-odps-winwin-1.0.8/dbt_odps_winwin.egg-info/PKG-INFO
--rw-r--r--   0 leezhongshan   (501) staff       (20)     2094 2024-01-09 08:04:50.000000 dbt-odps-winwin-1.0.8/dbt_odps_winwin.egg-info/SOURCES.txt
--rw-r--r--   0 leezhongshan   (501) staff       (20)        1 2024-01-09 08:04:50.000000 dbt-odps-winwin-1.0.8/dbt_odps_winwin.egg-info/dependency_links.txt
--rw-r--r--   0 leezhongshan   (501) staff       (20)       33 2024-01-09 08:04:50.000000 dbt-odps-winwin-1.0.8/dbt_odps_winwin.egg-info/requires.txt
--rw-r--r--   0 leezhongshan   (501) staff       (20)        4 2024-01-09 08:04:50.000000 dbt-odps-winwin-1.0.8/dbt_odps_winwin.egg-info/top_level.txt
--rw-r--r--   0 leezhongshan   (501) staff       (20)       79 2024-01-09 08:04:50.271537 dbt-odps-winwin-1.0.8/setup.cfg
--rw-r--r--   0 leezhongshan   (501) staff       (20)     2922 2024-01-09 08:04:13.000000 dbt-odps-winwin-1.0.8/setup.py
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.140125 dbt-odps-winwin-1.0.9/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       47 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/MANIFEST.in
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     4041 2024-02-01 23:04:26.140006 dbt-odps-winwin-1.0.9/PKG-INFO
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     3710 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/README.md
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.119128 dbt-odps-winwin-1.0.9/dbt/
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.119004 dbt-odps-winwin-1.0.9/dbt/adapters/
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.127224 dbt-odps-winwin-1.0.9/dbt/adapters/odps/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      621 2023-12-18 07:33:56.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/__init__.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       18 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/__version__.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     2087 2023-12-18 07:33:56.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/colums.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     5079 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/connections.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     3752 2024-01-09 07:08:04.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/date.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     1961 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/dbapi.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      175 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/errors.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     7604 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/impl.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     1566 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/relation.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     1556 2024-01-09 07:08:04.000000 dbt-odps-winwin-1.0.9/dbt/adapters/odps/utils.py
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.119210 dbt-odps-winwin-1.0.9/dbt/include/
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.128551 dbt-odps-winwin-1.0.9/dbt/include/odps/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       52 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/__init__.py
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       73 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/dbt_project.yml
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.129452 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)    11986 2024-02-01 23:00:51.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/adapters.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     1553 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/apply_grants.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      982 2023-12-18 07:33:56.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/catalog.sql
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.130813 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.132145 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/incremental/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     4729 2024-02-01 22:59:56.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     2378 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/incremental/on_schema_change.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     6034 2023-12-25 09:21:01.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     2070 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     4354 2024-01-09 15:49:47.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/seed.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     6916 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/snapshot.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     2795 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/table.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      697 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/view.sql
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.137939 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      719 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/any_value.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      192 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/array_append.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      127 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/array_concat.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      425 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/array_construct.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      665 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/bool_or.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      720 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      669 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/concat.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      682 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/date_trunc.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     1077 2024-01-09 07:08:04.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/dateadd.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     3069 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/datediff.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      428 2024-01-09 08:02:06.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/dateutil.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      689 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      742 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/hash.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     1208 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/last_day.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      514 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/listagg.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      724 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/position.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      896 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/right.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     1140 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/split_part.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      662 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/timestamps.sql
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      292 2024-01-09 07:08:04.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/macros.yml
+-rw-r--r--   0 leezhongshan   (501) staff       (20)      476 2023-12-14 01:22:18.000000 dbt-odps-winwin-1.0.9/dbt/include/odps/profile_template.yml
+drwxr-xr-x   0 leezhongshan   (501) staff       (20)        0 2024-02-01 23:04:26.139479 dbt-odps-winwin-1.0.9/dbt_odps_winwin.egg-info/
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     4041 2024-02-01 23:04:26.000000 dbt-odps-winwin-1.0.9/dbt_odps_winwin.egg-info/PKG-INFO
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     2094 2024-02-01 23:04:26.000000 dbt-odps-winwin-1.0.9/dbt_odps_winwin.egg-info/SOURCES.txt
+-rw-r--r--   0 leezhongshan   (501) staff       (20)        1 2024-02-01 23:04:26.000000 dbt-odps-winwin-1.0.9/dbt_odps_winwin.egg-info/dependency_links.txt
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       33 2024-02-01 23:04:26.000000 dbt-odps-winwin-1.0.9/dbt_odps_winwin.egg-info/requires.txt
+-rw-r--r--   0 leezhongshan   (501) staff       (20)        4 2024-02-01 23:04:26.000000 dbt-odps-winwin-1.0.9/dbt_odps_winwin.egg-info/top_level.txt
+-rw-r--r--   0 leezhongshan   (501) staff       (20)       79 2024-02-01 23:04:26.140578 dbt-odps-winwin-1.0.9/setup.cfg
+-rw-r--r--   0 leezhongshan   (501) staff       (20)     2922 2024-02-01 23:01:24.000000 dbt-odps-winwin-1.0.9/setup.py
```

### Comparing `dbt-odps-winwin-1.0.8/PKG-INFO` & `dbt-odps-winwin-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-odps-winwin
-Version: 1.0.8
+Version: 1.0.9
 Summary: The ODPS (MaxCompute)  adapter plugin for dbt
 Home-page: https://github.com/winwin-inc/dbt-odps
 Author: leezhongshan
 Author-email: leezhongshan0316@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: pyodps==0.11.5b2
```

### Comparing `dbt-odps-winwin-1.0.8/README.md` & `dbt-odps-winwin-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/adapters/odps/__init__.py` & `dbt-odps-winwin-1.0.9/dbt/adapters/odps/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/adapters/odps/colums.py` & `dbt-odps-winwin-1.0.9/dbt/adapters/odps/colums.py`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/adapters/odps/connections.py` & `dbt-odps-winwin-1.0.9/dbt/adapters/odps/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/adapters/odps/date.py` & `dbt-odps-winwin-1.0.9/dbt/adapters/odps/date.py`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/adapters/odps/dbapi.py` & `dbt-odps-winwin-1.0.9/dbt/adapters/odps/dbapi.py`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/adapters/odps/impl.py` & `dbt-odps-winwin-1.0.9/dbt/adapters/odps/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/adapters/odps/relation.py` & `dbt-odps-winwin-1.0.9/dbt/adapters/odps/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/adapters/odps/utils.py` & `dbt-odps-winwin-1.0.9/dbt/adapters/odps/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/adapters.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/adapters.sql`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,23 @@
 {% macro odps__list_views_without_caching(schema) %}
   {% call statement('list_views_without_caching', fetch_result=True) -%}
     select table_name from information_schema.TABLES where table_type = 'VIRTUAL_VIEW'
   {% endcall %}
   {% do return(load_result('list_views_without_caching').table) %}
 {% endmacro %}
 
+{% macro odps_get_desc_from_config() %}
+{%- set tab_cols = config.get('columns', validator=validation.any[list, basestring]) -%}
+{%- set tab_cols_dict = {} -%}
+{%- for item in tab_cols -%}
+{%- do tab_cols_dict.setdefault(item.name,item.description) -%}
+{%- endfor -%}
+{%- do return(tab_cols_dict) -%}
+{% endmacro %}
+
 {% macro odps__get_columns_from_query(sql) %}
 {%- set partition_cols = config.get('partition_by', validator=validation.any[list, basestring]) -%}
   {%- set partition_col_names = [] -%}
   {%- if partition_cols is not none %}
     {%- if partition_cols is mapping  -%}
     {%- set partition_cols = [partition_cols] -%}
     {%- endif -%}
@@ -257,16 +266,17 @@
     {%- endif -%}
   {%- endfor -%}
   {% do return(columns) %}
 {% endmacro %}
 
 {% macro odps__get_table_columns_and_constraints_from_query(sql) -%}
 (
+    {% set tab_cols = odps_get_desc_from_config() %}
     {% for c in odps__get_columns_from_query(sql) -%}
-    {{ c.name }} {{ c.dtype }}{{ "," if not loop.last or raw_model_constraints }}
+    {{ c.name }} {{ c.dtype }} {{ "COMMENT" }} '{{ tab_cols.get(c.name) }}' {{ "," if not loop.last or raw_model_constraints }}
     {% endfor %}
 )
 {%- endmacro %}
 
 {% macro odps__get_assert_columns_equivalent(sql) -%}
   {{ return(odps_assert_columns_equivalent(sql)) }}
 {%- endmacro %}
```

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/apply_grants.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/catalog.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/incremental/incremental.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/incremental/on_schema_change.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/incremental/strategies.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/incremental/validate.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/seed.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/snapshot.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/table.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/materializations/view.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/any_value.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/any_value.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/bool_or.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/bool_or.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/cast_bool_to_text.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/cast_bool_to_text.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/concat.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/concat.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/date_trunc.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/date_trunc.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/dateadd.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/datediff.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/escape_single_quotes.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/escape_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/hash.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/last_day.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/listagg.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/position.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/right.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/right.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/split_part.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt/include/odps/macros/utils/timestamps.sql` & `dbt-odps-winwin-1.0.9/dbt/include/odps/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/dbt_odps_winwin.egg-info/PKG-INFO` & `dbt-odps-winwin-1.0.9/dbt_odps_winwin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-odps-winwin
-Version: 1.0.8
+Version: 1.0.9
 Summary: The ODPS (MaxCompute)  adapter plugin for dbt
 Home-page: https://github.com/winwin-inc/dbt-odps
 Author: leezhongshan
 Author-email: leezhongshan0316@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: pyodps==0.11.5b2
```

### Comparing `dbt-odps-winwin-1.0.8/dbt_odps_winwin.egg-info/SOURCES.txt` & `dbt-odps-winwin-1.0.9/dbt_odps_winwin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-odps-winwin-1.0.8/setup.py` & `dbt-odps-winwin-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from setuptools import find_namespace_packages, setup,Command
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf8") as f:
     long_description = f.read()
 
-package_version = "1.0.8"
+package_version = "1.0.9"
 here = os.path.abspath(os.path.dirname(__file__))
 
 
 def _get_plugin_version_dict():
     _version_path = os.path.join(this_directory, "dbt", "adapters", "odps", "__version__.py")
     _semver = r"""(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)"""
     _pre = r"""((?P<prekind>a|b|rc)(?P<pre>\d+))?"""
```

