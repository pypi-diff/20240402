# Comparing `tmp/gio_importer_v44-1.0.20.tar.gz` & `tmp/gio_importer_v44-1.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gio_importer_v44-1.0.20.tar", last modified: Fri Mar 15 02:18:38 2024, max compression
+gzip compressed data, was "gio_importer_v44-1.0.22.tar", last modified: Tue Apr  2 06:27:43 2024, max compression
```

## Comparing `gio_importer_v44-1.0.20.tar` & `gio_importer_v44-1.0.22.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:38.014836 gio_importer_v44-1.0.20/
--rw-r--r--   0 chengcheng   (501) staff       (20)     1061 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/LICENSE
--rw-r--r--   0 chengcheng   (501) staff       (20)       71 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/MANIFEST.in
--rw-r--r--   0 chengcheng   (501) staff       (20)    12106 2024-03-15 02:18:38.014670 gio_importer_v44-1.0.20/PKG-INFO
--rw-r--r--   0 chengcheng   (501) staff       (20)      792 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/README.md
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:37.965141 gio_importer_v44-1.0.20/gio_importer_v44.egg-info/
--rw-r--r--   0 chengcheng   (501) staff       (20)    12106 2024-03-15 02:18:37.000000 gio_importer_v44-1.0.20/gio_importer_v44.egg-info/PKG-INFO
--rw-r--r--   0 chengcheng   (501) staff       (20)     1405 2024-03-15 02:18:37.000000 gio_importer_v44-1.0.20/gio_importer_v44.egg-info/SOURCES.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)        1 2024-03-15 02:18:37.000000 gio_importer_v44-1.0.20/gio_importer_v44.egg-info/dependency_links.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)      197 2024-03-15 02:18:37.000000 gio_importer_v44-1.0.20/gio_importer_v44.egg-info/entry_points.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)       84 2024-03-15 02:18:37.000000 gio_importer_v44-1.0.20/gio_importer_v44.egg-info/requires.txt
--rw-r--r--   0 chengcheng   (501) staff       (20)       10 2024-03-15 02:18:37.000000 gio_importer_v44-1.0.20/gio_importer_v44.egg-info/top_level.txt
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:37.975577 gio_importer_v44-1.0.20/importers/
--rw-r--r--   0 chengcheng   (501) staff       (20)    11711 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/README.md
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/__init__.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:37.976813 gio_importer_v44-1.0.20/importers/clear_data/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/clear_data/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2820 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/clear_data/clear_data.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1714 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/clear_user.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:37.984460 gio_importer_v44-1.0.20/importers/common/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/common/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     5581 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/common/common_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2507 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/common/config_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2602 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/common/http_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      955 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/common/log_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      771 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/conf.cfg
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:37.995654 gio_importer_v44-1.0.20/importers/data_import/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/data_import/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    21815 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/data_import/data_ads.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    21732 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/data_import/data_events.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    11148 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/data_import/data_format_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    17799 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/data_import/data_item_variable.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     6455 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/data_import/data_model.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    15382 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/data_import/data_user_variable.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     6943 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/data_importer.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:38.003173 gio_importer_v44-1.0.20/importers/db_import/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/db_import/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     2718 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/db_import/database_import.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    14364 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/db_import/hive_import.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    14476 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/db_import/mysql_import.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:38.004294 gio_importer_v44-1.0.20/importers/example/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/example/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     5144 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/format_importer.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      472 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/log_conf.yaml
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:38.010260 gio_importer_v44-1.0.20/importers/meta/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/meta/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    10656 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/meta/check_util.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     8398 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/meta/data_center.py
--rw-r--r--   0 chengcheng   (501) staff       (20)    21399 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/meta/meta_create.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     4862 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/meta_importer.py
-drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-03-15 02:18:38.014246 gio_importer_v44-1.0.20/importers/saas_export/
--rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/saas_export/__init__.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     3303 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/saas_export/saas_meta.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1179 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/saas_export.py
--rw-r--r--   0 chengcheng   (501) staff       (20)      232 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/setup.py
--rw-r--r--   0 chengcheng   (501) staff       (20)     1372 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/trigger_job.py
--rw-r--r--   0 chengcheng   (501) staff       (20)       95 2024-03-14 06:06:37.000000 gio_importer_v44-1.0.20/importers/zk.py
--rw-r--r--   0 chengcheng   (501) staff       (20)       38 2024-03-15 02:18:38.014900 gio_importer_v44-1.0.20/setup.cfg
--rw-r--r--   0 chengcheng   (501) staff       (20)     1256 2024-03-15 02:18:19.000000 gio_importer_v44-1.0.20/setup.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.995811 gio_importer_v44-1.0.22/
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1061 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/LICENSE
+-rw-r--r--   0 chengcheng   (501) staff       (20)       71 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/MANIFEST.in
+-rw-r--r--   0 chengcheng   (501) staff       (20)    12106 2024-04-02 06:27:43.995588 gio_importer_v44-1.0.22/PKG-INFO
+-rw-r--r--   0 chengcheng   (501) staff       (20)      792 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/README.md
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.959004 gio_importer_v44-1.0.22/gio_importer_v44.egg-info/
+-rw-r--r--   0 chengcheng   (501) staff       (20)    12106 2024-04-02 06:27:43.000000 gio_importer_v44-1.0.22/gio_importer_v44.egg-info/PKG-INFO
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1405 2024-04-02 06:27:43.000000 gio_importer_v44-1.0.22/gio_importer_v44.egg-info/SOURCES.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)        1 2024-04-02 06:27:43.000000 gio_importer_v44-1.0.22/gio_importer_v44.egg-info/dependency_links.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)      197 2024-04-02 06:27:43.000000 gio_importer_v44-1.0.22/gio_importer_v44.egg-info/entry_points.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)       84 2024-04-02 06:27:43.000000 gio_importer_v44-1.0.22/gio_importer_v44.egg-info/requires.txt
+-rw-r--r--   0 chengcheng   (501) staff       (20)       10 2024-04-02 06:27:43.000000 gio_importer_v44-1.0.22/gio_importer_v44.egg-info/top_level.txt
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.974482 gio_importer_v44-1.0.22/importers/
+-rw-r--r--   0 chengcheng   (501) staff       (20)    11711 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/README.md
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/__init__.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.976291 gio_importer_v44-1.0.22/importers/clear_data/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/clear_data/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2820 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/clear_data/clear_data.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1714 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/clear_user.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.983949 gio_importer_v44-1.0.22/importers/common/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/common/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     5581 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/common/common_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2507 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/common/config_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2602 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/common/http_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      955 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/common/log_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      771 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/conf.cfg
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.989123 gio_importer_v44-1.0.22/importers/data_import/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/data_import/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    21814 2024-03-22 02:06:04.000000 gio_importer_v44-1.0.22/importers/data_import/data_ads.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    21731 2024-03-22 02:06:54.000000 gio_importer_v44-1.0.22/importers/data_import/data_events.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    11148 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/data_import/data_format_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    17799 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/data_import/data_item_variable.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     6455 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/data_import/data_model.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    15382 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/data_import/data_user_variable.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     6943 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/data_importer.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.991129 gio_importer_v44-1.0.22/importers/db_import/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/db_import/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     2717 2024-03-22 02:07:32.000000 gio_importer_v44-1.0.22/importers/db_import/database_import.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    14364 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/db_import/hive_import.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    14467 2024-03-22 02:11:11.000000 gio_importer_v44-1.0.22/importers/db_import/mysql_import.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.991749 gio_importer_v44-1.0.22/importers/example/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/example/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     5144 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/format_importer.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      472 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/log_conf.yaml
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.994439 gio_importer_v44-1.0.22/importers/meta/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/meta/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    10656 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/meta/check_util.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     8398 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/meta/data_center.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)    21399 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/meta/meta_create.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     4862 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/meta_importer.py
+drwxr-xr-x   0 chengcheng   (501) staff       (20)        0 2024-04-02 06:27:43.995203 gio_importer_v44-1.0.22/importers/saas_export/
+-rw-r--r--   0 chengcheng   (501) staff       (20)        0 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/saas_export/__init__.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     3303 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/saas_export/saas_meta.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1179 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/saas_export.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)      232 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/setup.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1372 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/trigger_job.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)       95 2024-03-22 01:45:40.000000 gio_importer_v44-1.0.22/importers/zk.py
+-rw-r--r--   0 chengcheng   (501) staff       (20)       38 2024-04-02 06:27:43.995872 gio_importer_v44-1.0.22/setup.cfg
+-rw-r--r--   0 chengcheng   (501) staff       (20)     1256 2024-04-02 06:27:04.000000 gio_importer_v44-1.0.22/setup.py
```

### Comparing `gio_importer_v44-1.0.20/LICENSE` & `gio_importer_v44-1.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/PKG-INFO` & `gio_importer_v44-1.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gio_importer_v44
-Version: 1.0.20
+Version: 1.0.22
 Summary: GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具
 Home-page: UNKNOWN
 Author: gio
 Author-email: dev-growing@startdt.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gio_importer_v44-1.0.20/README.md` & `gio_importer_v44-1.0.22/README.md`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/gio_importer_v44.egg-info/PKG-INFO` & `gio_importer_v44-1.0.22/gio_importer_v44.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gio-importer-v44
-Version: 1.0.20
+Version: 1.0.22
 Summary: GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具
 Home-page: UNKNOWN
 Author: gio
 Author-email: dev-growing@startdt.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `gio_importer_v44-1.0.20/gio_importer_v44.egg-info/SOURCES.txt` & `gio_importer_v44-1.0.22/gio_importer_v44.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/README.md` & `gio_importer_v44-1.0.22/importers/README.md`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/clear_data/clear_data.py` & `gio_importer_v44-1.0.22/importers/clear_data/clear_data.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/clear_user.py` & `gio_importer_v44-1.0.22/importers/clear_user.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/common/common_util.py` & `gio_importer_v44-1.0.22/importers/common/common_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/common/config_util.py` & `gio_importer_v44-1.0.22/importers/common/config_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/common/http_util.py` & `gio_importer_v44-1.0.22/importers/common/http_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/common/log_util.py` & `gio_importer_v44-1.0.22/importers/common/log_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/conf.cfg` & `gio_importer_v44-1.0.22/importers/conf.cfg`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/data_import/data_ads.py` & `gio_importer_v44-1.0.22/importers/data_import/data_ads.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             * 1000
         )
         event_end = (
             time_str_to_timestamp_of_tz(event_end, "%Y-%m-%d", BaseConfig.timezone)
             * 1000
             + ONE_DAY_MILLISECOND
         )
-    except TypeError and ValueError:
+    except (TypeError, ValueError):
         logger.error("[-s/--event_start]或[-e/--event_end]时间参数格式不对,格式为:YYYY-MM-DD")
         exit(-1)
     # 2. 数据源是否为事件
     ds = args.get("datasource_id")
     if "HISTORY_ADS_EVENT" in ds[1]:
         args["datasource_id"] = ds[1]["HISTORY_ADS_EVENT"]
     else:
```

### Comparing `gio_importer_v44-1.0.20/importers/data_import/data_events.py` & `gio_importer_v44-1.0.22/importers/data_import/data_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     event_end = args.get('event_end')
     if event_end is None:
         logger.error("[-e/--event_end]参数值未指定")
         exit(-1)
     try:
         event_start = time_str_to_timestamp_of_tz(event_start, '%Y-%m-%d', BaseConfig.timezone) * 1000
         event_end = time_str_to_timestamp_of_tz(event_end, '%Y-%m-%d', BaseConfig.timezone) * 1000 + ONE_DAY_MILLISECOND
-    except TypeError and ValueError:
+    except (TypeError, ValueError):
         logger.error("[-s/--event_start]或[-e/--event_end]时间参数格式不对,格式为:YYYY-MM-DD")
         exit(-1)
     # 2. 数据源是否为事件
     ds = args.get('datasource_id')
     if 'HISTORY_EVENT' in ds[1]:
         args['datasource_id'] = ds[1]['HISTORY_EVENT']
     else:
```

### Comparing `gio_importer_v44-1.0.20/importers/data_import/data_format_util.py` & `gio_importer_v44-1.0.22/importers/data_import/data_format_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/data_import/data_item_variable.py` & `gio_importer_v44-1.0.22/importers/data_import/data_item_variable.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/data_import/data_model.py` & `gio_importer_v44-1.0.22/importers/data_import/data_model.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/data_import/data_user_variable.py` & `gio_importer_v44-1.0.22/importers/data_import/data_user_variable.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/data_importer.py` & `gio_importer_v44-1.0.22/importers/data_importer.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/db_import/database_import.py` & `gio_importer_v44-1.0.22/importers/db_import/database_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def events(args):
     try:
         start = time_str_to_timestamp_of_tz(args.get('start_time'), '%Y-%m-%d', BaseConfig.timezone) * 1000
         end = time_str_to_timestamp_of_tz(args.get('end_time'), '%Y-%m-%d',
                                           BaseConfig.timezone) * 1000 + ONE_DAY_MILLISECOND
-    except TypeError and ValueError:
+    except (TypeError, ValueError):
         logger.error("[-s/--start_time]或[-e/--end_time]时间参数格式不对,格式为:YYYY-MM-DD")
         exit(-1)
     ds = args.get('datasource_id')
     if 'HISTORY_EVENT' in ds[1]:
         args['datasource_id'] = ds[1]['HISTORY_EVENT']
     else:
         logger.error("数据源不属于用户行为类型")
```

### Comparing `gio_importer_v44-1.0.20/importers/db_import/hive_import.py` & `gio_importer_v44-1.0.22/importers/db_import/hive_import.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/db_import/mysql_import.py` & `gio_importer_v44-1.0.22/importers/db_import/mysql_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 def event_mysql_import(args, start, end):
     """
        行为数据导入 ，MYSQL数据源
     """
     try:
         conn = mysql_connect(user=args.get('user'), password=args.get('password'), host=args.get('host'),
                              port=int(args.get('port')))
-    except MySQLError and OperationalError:
+    except (MySQLError, OperationalError):
         logger.error(" MYSQL连接失败。")
         exit(-1)
     cursor = conn.cursor()
     try:
         sql = args.get('sql')
         cursor.execute(sql)
         my_logger.info(sql)
-    except SyntaxError or MySQLError or OperationalError:
+    except (SyntaxError, MySQLError, OperationalError):
         logger.error("请检查SQL语句")
         exit(-1)
     desc = cursor.description
     desc_list = []
     for d in desc:
         desc_list.append(d[0])
     if 'event' not in desc_list or 'timestamp' not in desc_list:
@@ -144,23 +144,23 @@
 def user_mysql_import(args):
     """
        用户属性导入，MYSQL数据源
     """
     try:
         conn = mysql_connect(user=args.get('user'), password=args.get('password'), host=args.get('host'),
                              port=int(args.get('port')))
-    except MySQLError and OperationalError:
+    except (MySQLError, OperationalError):
         logger.error("MYSQL连接失败。")
         exit(-1)
     cursor = conn.cursor()
     try:
         sql = args.get('sql')
         cursor.execute(sql)
         my_logger.info(sql)
-    except SyntaxError or MySQLError or OperationalError:
+    except (SyntaxError, MySQLError, OperationalError):
         logger.error("请检查SQL语句")
         exit(-1)
     desc = cursor.description
     desc_list = []
     for d in desc:
         desc_list.append(d[0])
     if 'userId' not in desc_list:
@@ -243,23 +243,23 @@
 def item_mysql_import(args):
     """
            主体导入，MYSQL数据源
         """
     try:
         conn = mysql_connect(user=args.get('user'), password=args.get('password'), host=args.get('host'),
                              port=int(args.get('port')))
-    except MySQLError and OperationalError:
+    except (MySQLError, OperationalError):
         logger.error("MYSQL连接失败。")
         exit(-1)
     cursor = conn.cursor()
     try:
         sql = args.get('sql')
         cursor.execute(sql)
         my_logger.info(sql)
-    except SyntaxError or MySQLError or OperationalError:
+    except (SyntaxError, MySQLError, OperationalError):
         logger.error("请检查SQL语句")
         exit(-1)
     desc = cursor.description
     desc_list = []
     for d in desc:
         desc_list.append(d[0])
     if 'item_id' not in desc_list:
```

### Comparing `gio_importer_v44-1.0.20/importers/format_importer.py` & `gio_importer_v44-1.0.22/importers/format_importer.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/meta/check_util.py` & `gio_importer_v44-1.0.22/importers/meta/check_util.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/meta/data_center.py` & `gio_importer_v44-1.0.22/importers/meta/data_center.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/meta/meta_create.py` & `gio_importer_v44-1.0.22/importers/meta/meta_create.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/meta_importer.py` & `gio_importer_v44-1.0.22/importers/meta_importer.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/saas_export/saas_meta.py` & `gio_importer_v44-1.0.22/importers/saas_export/saas_meta.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/saas_export.py` & `gio_importer_v44-1.0.22/importers/saas_export.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/importers/trigger_job.py` & `gio_importer_v44-1.0.22/importers/trigger_job.py`

 * *Files identical despite different names*

### Comparing `gio_importer_v44-1.0.20/setup.py` & `gio_importer_v44-1.0.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'pyhive',
     'thrift',
     'sasl'
 ]
 
 setup(
     name='gio_importer_v44',
-    version='1.0.20',
+    version='1.0.22',
     description='GrowingIO Importer是GrowingIO CDP平台元数据创建和数据导入工具',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='gio',
     author_email='dev-growing@startdt.com',
     packages=find_packages(include=["importers*"]),
     include_package_data=True,
```

