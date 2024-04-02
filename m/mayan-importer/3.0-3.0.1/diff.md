# Comparing `tmp/mayan-importer-3.0.tar.gz` & `tmp/mayan-importer-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayan-importer-3.0.tar", last modified: Mon Apr  1 10:02:43 2024, max compression
+gzip compressed data, was "mayan-importer-3.0.1.tar", last modified: Mon Apr  1 12:00:03 2024, max compression
```

## Comparing `mayan-importer-3.0.tar` & `mayan-importer-3.0.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.330866 mayan-importer-3.0/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6341 2024-04-01 10:00:26.000000 mayan-importer-3.0/HISTORY.rst
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.0/LICENSE
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.0/MANIFEST.in
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9231 2024-04-01 10:02:43.330866 mayan-importer-3.0/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.0/README.rst
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.324866 mayan-importer-3.0/importer/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/admin.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/api_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7455 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/apps.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7228 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/classes.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/dependencies.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/events.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/exceptions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      997 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/forms.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1366 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/icons.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8712 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5779 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/links.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      904 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/literals.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.327866 mayan-importer-3.0/importer/migrations/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/migrations/0001_initial.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/migrations/0002_auto_20200908_0458.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/migrations/0003_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0004_auto_20200908_0853.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0005_importsetup_state.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0006_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0007_auto_20200924_0802.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0008_auto_20200924_0903.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0009_importsetupaction.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      289 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0010_remove_importsetup_metadata_map.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0011_auto_20201004_0042.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0012_importsetupitem_documents.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0013_auto_20201225_0155.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0014_auto_20201227_0610.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0015_auto_20220901_0932.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/migrations/0016_importsetup_item_time_buffer.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/migrations/0017_delete_importsetuplog.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/migrations/0018_auto_20240401_0808.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.0/importer/migrations/__init__.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.328866 mayan-importer-3.0/importer/models/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      134 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4220 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/import_setup_item_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2882 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/import_setup_item_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5737 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/import_setup_model_mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2470 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/models/import_setup_models.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/permissions.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/queues.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/serializers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2794 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tasks.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.329866 mayan-importer-3.0/importer/tests/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1559 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/importers.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      408 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/literals.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8729 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/mixins.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/tests/test_import_setup_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7881 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/test_import_setup_item_api.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    12253 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/test_import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6425 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/tests/test_import_setup_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5600 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/urls.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.329866 mayan-importer-3.0/importer/views/
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.0/importer/views/__init__.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    16658 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/views/import_setup_item_views.py
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4343 2024-04-01 10:00:47.000000 mayan-importer-3.0/importer/views/import_setup_views.py
-drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:02:43.330866 mayan-importer-3.0/mayan_importer.egg-info/
--rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9231 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/PKG-INFO
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2148 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/SOURCES.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/dependency_links.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/not-zip-safe
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/requires.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-04-01 10:02:43.000000 mayan-importer-3.0/mayan_importer.egg-info/top_level.txt
--rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-04-01 10:02:43.331866 mayan-importer-3.0/setup.cfg
--rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3036 2024-04-01 10:00:07.000000 mayan-importer-3.0/setup.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 12:00:03.405440 mayan-importer-3.0.1/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6341 2024-04-01 10:00:26.000000 mayan-importer-3.0.1/HISTORY.rst
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      555 2020-10-02 10:42:37.000000 mayan-importer-3.0.1/LICENSE
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       39 2020-10-02 10:42:37.000000 mayan-importer-3.0.1/MANIFEST.in
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9233 2024-04-01 12:00:03.405440 mayan-importer-3.0.1/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1628 2020-10-02 10:42:37.000000 mayan-importer-3.0.1/README.rst
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 12:00:03.399440 mayan-importer-3.0.1/importer/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       49 2020-10-02 10:42:37.000000 mayan-importer-3.0.1/importer/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      405 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/admin.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4643 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/api_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7455 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/apps.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7145 2024-04-01 11:57:21.000000 mayan-importer-3.0.1/importer/classes.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      145 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/dependencies.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1729 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/events.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       93 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/exceptions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      997 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/forms.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1366 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/icons.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8712 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5779 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/links.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      904 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/literals.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 12:00:03.402440 mayan-importer-3.0.1/importer/migrations/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4126 2020-10-02 10:42:37.000000 mayan-importer-3.0.1/importer/migrations/0001_initial.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1475 2020-10-02 10:42:37.000000 mayan-importer-3.0.1/importer/migrations/0002_auto_20200908_0458.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      669 2020-10-02 10:42:37.000000 mayan-importer-3.0.1/importer/migrations/0003_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      795 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0004_auto_20200908_0853.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      607 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0005_importsetup_state.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      333 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0006_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      428 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0007_auto_20200924_0802.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      603 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0008_auto_20200924_0903.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2451 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0009_importsetupaction.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      289 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0010_remove_importsetup_metadata_map.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      568 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0011_auto_20201004_0042.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      522 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0012_importsetupitem_documents.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1796 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0013_auto_20201225_0155.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      396 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0014_auto_20201227_0610.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      848 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0015_auto_20220901_0932.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      526 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/migrations/0016_importsetup_item_time_buffer.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      239 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/migrations/0017_delete_importsetuplog.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1064 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/migrations/0018_auto_20240401_0808.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2020-10-02 10:42:37.000000 mayan-importer-3.0.1/importer/migrations/__init__.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 12:00:03.402440 mayan-importer-3.0.1/importer/models/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      134 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/models/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4220 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/models/import_setup_item_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2882 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/models/import_setup_item_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5737 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/models/import_setup_model_mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2470 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/models/import_setup_models.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1386 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/permissions.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1197 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/queues.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     3473 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/serializers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2794 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/tasks.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 12:00:03.404440 mayan-importer-3.0.1/importer/tests/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/tests/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     1559 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/tests/importers.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      408 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/tests/literals.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8729 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/tests/mixins.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     8233 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/tests/test_import_setup_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     7881 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/tests/test_import_setup_item_api.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    12253 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/tests/test_import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     6425 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/tests/test_import_setup_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     5600 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/urls.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 12:00:03.404440 mayan-importer-3.0.1/importer/views/
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        0 2023-04-12 05:57:59.000000 mayan-importer-3.0.1/importer/views/__init__.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)    16658 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/views/import_setup_item_views.py
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     4343 2024-04-01 10:00:47.000000 mayan-importer-3.0.1/importer/views/import_setup_views.py
+drwxrwxr-x   0 rosarior  (1000) rosarior  (1000)        0 2024-04-01 12:00:03.405440 mayan-importer-3.0.1/mayan_importer.egg-info/
+-rw-r--r--   0 rosarior  (1000) rosarior  (1000)     9233 2024-04-01 12:00:03.000000 mayan-importer-3.0.1/mayan_importer.egg-info/PKG-INFO
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)     2148 2024-04-01 12:00:03.000000 mayan-importer-3.0.1/mayan_importer.egg-info/SOURCES.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-01 12:00:03.000000 mayan-importer-3.0.1/mayan_importer.egg-info/dependency_links.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        1 2024-04-01 12:00:03.000000 mayan-importer-3.0.1/mayan_importer.egg-info/not-zip-safe
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)       16 2024-04-01 12:00:03.000000 mayan-importer-3.0.1/mayan_importer.egg-info/requires.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)        9 2024-04-01 12:00:03.000000 mayan-importer-3.0.1/mayan_importer.egg-info/top_level.txt
+-rw-rw-r--   0 rosarior  (1000) rosarior  (1000)      129 2024-04-01 12:00:03.406440 mayan-importer-3.0.1/setup.cfg
+-rwxrwxr-x   0 rosarior  (1000) rosarior  (1000)     3038 2024-04-01 11:59:50.000000 mayan-importer-3.0.1/setup.py
```

### Comparing `mayan-importer-3.0/HISTORY.rst` & `mayan-importer-3.0.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/LICENSE` & `mayan-importer-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/PKG-INFO` & `mayan-importer-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.0
+Version: 3.0.1
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mayan-importer-3.0/README.rst` & `mayan-importer-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/api_views.py` & `mayan-importer-3.0.1/importer/api_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/apps.py` & `mayan-importer-3.0.1/importer/apps.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/classes.py` & `mayan-importer-3.0.1/importer/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,18 +168,17 @@
 
         queryset = self.model._meta.default_manager.filter(**filter_kwargs)
 
         filename = '{}-export.csv'.format(
             self.get_model_full_name()
         )
 
+        label = _(message='Export of %s to CSV') % save_file_title
         download_file = DownloadFile(
-            content_object=queryset.first(), filename=filename,
-            label=_(message='Export of %s to CSV') % save_file_title,
-            permission=permission_import_setup_view.stored_permission
+            filename=filename, label=label, user=user
         )
         download_file._event_actor = user
         download_file.save()
 
         with NamedTemporaryFile(mode='r+') as temporary_file_object:
             writer = csv.DictWriter(
                 f=temporary_file_object, fieldnames=field_names
```

### Comparing `mayan-importer-3.0/importer/events.py` & `mayan-importer-3.0.1/importer/events.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/forms.py` & `mayan-importer-3.0.1/importer/forms.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/icons.py` & `mayan-importer-3.0.1/importer/icons.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/importers.py` & `mayan-importer-3.0.1/importer/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/links.py` & `mayan-importer-3.0.1/importer/links.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/literals.py` & `mayan-importer-3.0.1/importer/literals.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0001_initial.py` & `mayan-importer-3.0.1/importer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0002_auto_20200908_0458.py` & `mayan-importer-3.0.1/importer/migrations/0002_auto_20200908_0458.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0003_importsetup_metadata_map.py` & `mayan-importer-3.0.1/importer/migrations/0003_importsetup_metadata_map.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0004_auto_20200908_0853.py` & `mayan-importer-3.0.1/importer/migrations/0004_auto_20200908_0853.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0005_importsetup_state.py` & `mayan-importer-3.0.1/importer/migrations/0005_importsetup_state.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0008_auto_20200924_0903.py` & `mayan-importer-3.0.1/importer/migrations/0008_auto_20200924_0903.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0009_importsetupaction.py` & `mayan-importer-3.0.1/importer/migrations/0009_importsetupaction.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0011_auto_20201004_0042.py` & `mayan-importer-3.0.1/importer/migrations/0011_auto_20201004_0042.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0012_importsetupitem_documents.py` & `mayan-importer-3.0.1/importer/migrations/0012_importsetupitem_documents.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0013_auto_20201225_0155.py` & `mayan-importer-3.0.1/importer/migrations/0013_auto_20201225_0155.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0015_auto_20220901_0932.py` & `mayan-importer-3.0.1/importer/migrations/0015_auto_20220901_0932.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0016_importsetup_item_time_buffer.py` & `mayan-importer-3.0.1/importer/migrations/0016_importsetup_item_time_buffer.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/migrations/0018_auto_20240401_0808.py` & `mayan-importer-3.0.1/importer/migrations/0018_auto_20240401_0808.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/models/import_setup_item_model_mixins.py` & `mayan-importer-3.0.1/importer/models/import_setup_item_model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/models/import_setup_item_models.py` & `mayan-importer-3.0.1/importer/models/import_setup_item_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/models/import_setup_model_mixins.py` & `mayan-importer-3.0.1/importer/models/import_setup_model_mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/models/import_setup_models.py` & `mayan-importer-3.0.1/importer/models/import_setup_models.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/permissions.py` & `mayan-importer-3.0.1/importer/permissions.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/queues.py` & `mayan-importer-3.0.1/importer/queues.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/serializers.py` & `mayan-importer-3.0.1/importer/serializers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/tasks.py` & `mayan-importer-3.0.1/importer/tasks.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/tests/importers.py` & `mayan-importer-3.0.1/importer/tests/importers.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/tests/mixins.py` & `mayan-importer-3.0.1/importer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/tests/test_import_setup_api.py` & `mayan-importer-3.0.1/importer/tests/test_import_setup_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/tests/test_import_setup_item_api.py` & `mayan-importer-3.0.1/importer/tests/test_import_setup_item_api.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/tests/test_import_setup_item_views.py` & `mayan-importer-3.0.1/importer/tests/test_import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/tests/test_import_setup_views.py` & `mayan-importer-3.0.1/importer/tests/test_import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/urls.py` & `mayan-importer-3.0.1/importer/urls.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/views/import_setup_item_views.py` & `mayan-importer-3.0.1/importer/views/import_setup_item_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/importer/views/import_setup_views.py` & `mayan-importer-3.0.1/importer/views/import_setup_views.py`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/mayan_importer.egg-info/PKG-INFO` & `mayan-importer-3.0.1/mayan_importer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayan-importer
-Version: 3.0
+Version: 3.0.1
 Summary: Mayan EDMS importer
 Home-page: https://gitlab.com/mayan-edms/importer
 Author: Roberto Rosario
 Author-email: roberto.rosario@mayan-edms.com
 License: Apache 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mayan-importer-3.0/mayan_importer.egg-info/SOURCES.txt` & `mayan-importer-3.0.1/mayan_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayan-importer-3.0/setup.py` & `mayan-importer-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,10 +94,10 @@
     license='Apache 2.0',
     long_description=readme + '\n\n' + history,
     name=PACKAGE_NAME,
     packages=find_packages(PACKAGE_DIR),
     platforms=['any'],
     python_requires='!=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
     url='https://gitlab.com/mayan-edms/importer',
-    version='3.0',
+    version='3.0.1',
     zip_safe=False,
 )
```

