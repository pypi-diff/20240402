# Comparing `tmp/yellowdog-python-examples-7.8.2.tar.gz` & `tmp/yellowdog-python-examples-7.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-7.8.2.tar", last modified: Tue Mar 26 08:48:53 2024, max compression
+gzip compressed data, was "yellowdog-python-examples-7.8.3.tar", last modified: Tue Apr  2 09:31:50 2024, max compression
```

## Comparing `yellowdog-python-examples-7.8.2.tar` & `yellowdog-python-examples-7.8.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-03-26 08:48:53.255630 yellowdog-python-examples-7.8.2/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-7.8.2/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-03-26 08:48:53.255561 yellowdog-python-examples-7.8.2/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1442 2023-08-28 09:06:52.000000 yellowdog-python-examples-7.8.2/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   144187 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     2140 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.2/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)      242 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2024-03-26 08:48:53.255952 yellowdog-python-examples-7.8.2/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-7.8.2/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-03-26 08:48:53.233999 yellowdog-python-examples-7.8.2/tests/
--rw-r--r--   0 pwt        (501) staff       (20)     2092 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/tests/test_create_remove.py
--rw-r--r--   0 pwt        (501) staff       (20)     1650 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.2/tests/test_demos.py
--rw-r--r--   0 pwt        (501) staff       (20)     6017 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.2/tests/test_dryruns.py
--rw-r--r--   0 pwt        (501) staff       (20)     1444 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/tests/test_entrypoints.py
--rw-r--r--   0 pwt        (501) staff       (20)      604 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/tests/test_gui.py
--rw-r--r--   0 pwt        (501) staff       (20)     1705 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/tests/test_list.py
--rw-r--r--   0 pwt        (501) staff       (20)      857 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/tests/test_objects.py
--rw-r--r--   0 pwt        (501) staff       (20)     1683 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/tests/test_variable_processing.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-03-26 08:48:53.254217 yellowdog-python-examples-7.8.2/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4179 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.2/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2024-03-25 12:45:42.000000 yellowdog-python-examples-7.8.2/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    45642 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/yd_commands/args.py
--rw-r--r--   0 pwt        (501) staff       (20)      797 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.2/yd_commands/boost.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7489 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.2/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      607 2023-11-15 10:24:00.000000 yellowdog-python-examples-7.8.2/yd_commands/check_imports.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2502 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/yd_commands/cloudwizard.py
--rw-r--r--   0 pwt        (501) staff       (20)    37774 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.2/yd_commands/cloudwizard_aws.py
--rw-r--r--   0 pwt        (501) staff       (20)      481 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/yd_commands/cloudwizard_aws_types.py
--rw-r--r--   0 pwt        (501) staff       (20)    31496 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.2/yd_commands/cloudwizard_azure.py
--rw-r--r--   0 pwt        (501) staff       (20)    13186 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.2/yd_commands/cloudwizard_common.py
--rw-r--r--   0 pwt        (501) staff       (20)    12181 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.2/yd_commands/cloudwizard_gcp.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2023-09-02 10:35:56.000000 yellowdog-python-examples-7.8.2/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)     3529 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.2/yd_commands/config_types.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    29810 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/yd_commands/create.py
--rw-r--r--   0 pwt        (501) staff       (20)    13603 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.2/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2479 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4715 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.2/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      329 2023-09-04 08:20:55.000000 yellowdog-python-examples-7.8.2/yd_commands/follow.py
--rw-r--r--   0 pwt        (501) staff       (20)     3526 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.2/yd_commands/follow_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1494 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/yd_commands/format_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      290 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.2/yd_commands/hold.py
--rw-r--r--   0 pwt        (501) staff       (20)      842 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/yd_commands/id_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    12170 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.2/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     5146 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/yd_commands/interactive.py
--rw-r--r--   0 pwt        (501) staff       (20)     1007 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/yd_commands/items.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-09-02 10:35:56.000000 yellowdog-python-examples-7.8.2/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    18438 2024-03-20 15:33:41.000000 yellowdog-python-examples-7.8.2/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)    15863 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.2/yd_commands/load_config.py
--rw-r--r--   0 pwt        (501) staff       (20)     3861 2024-03-22 10:21:47.000000 yellowdog-python-examples-7.8.2/yd_commands/load_resources.py
--rw-r--r--   0 pwt        (501) staff       (20)     8703 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)    31544 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/yd_commands/printing.py
--rw-r--r--   0 pwt        (501) staff       (20)     5782 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.2/yd_commands/property_names.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    17214 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.2/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)     4748 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    13555 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.2/yd_commands/remove.py
--rw-r--r--   0 pwt        (501) staff       (20)     5169 2023-09-04 08:20:55.000000 yellowdog-python-examples-7.8.2/yd_commands/resize.py
--rw-r--r--   0 pwt        (501) staff       (20)     3261 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.2/yd_commands/settings.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4811 2024-02-27 14:55:53.000000 yellowdog-python-examples-7.8.2/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      298 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.2/yd_commands/start.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4815 2024-02-14 11:33:32.000000 yellowdog-python-examples-7.8.2/yd_commands/start_hold_common.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    52008 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.2/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)    10720 2024-02-14 11:33:32.000000 yellowdog-python-examples-7.8.2/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     4797 2024-02-27 14:55:53.000000 yellowdog-python-examples-7.8.2/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2023-11-24 13:35:57.000000 yellowdog-python-examples-7.8.2/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     5352 2023-11-18 08:50:59.000000 yellowdog-python-examples-7.8.2/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3683 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     6732 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/yd_commands/utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     2486 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.2/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    18165 2024-03-20 15:33:41.000000 yellowdog-python-examples-7.8.2/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.2/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     3747 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.2/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-03-26 08:48:53.255063 yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-03-26 08:48:53.000000 yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1934 2024-03-26 08:48:53.000000 yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2024-03-26 08:48:53.000000 yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      860 2024-03-26 08:48:53.000000 yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)      253 2024-03-26 08:48:53.000000 yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2024-03-26 08:48:53.000000 yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-02 09:31:50.902096 yellowdog-python-examples-7.8.3/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-7.8.3/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-02 09:31:50.902030 yellowdog-python-examples-7.8.3/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1442 2023-08-28 09:06:52.000000 yellowdog-python-examples-7.8.3/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   144187 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     2140 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.3/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)      242 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2024-04-02 09:31:50.902379 yellowdog-python-examples-7.8.3/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-7.8.3/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-02 09:31:50.880643 yellowdog-python-examples-7.8.3/tests/
+-rw-r--r--   0 pwt        (501) staff       (20)     2092 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/tests/test_create_remove.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2374 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/tests/test_demos.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6017 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.3/tests/test_dryruns.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1656 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/tests/test_entrypoints.py
+-rw-r--r--   0 pwt        (501) staff       (20)      604 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/tests/test_gui.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1705 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/tests/test_list.py
+-rw-r--r--   0 pwt        (501) staff       (20)      857 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/tests/test_objects.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1683 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/tests/test_variable_processing.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-02 09:31:50.900540 yellowdog-python-examples-7.8.3/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4179 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.3/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2024-03-25 12:45:42.000000 yellowdog-python-examples-7.8.3/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    45701 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/args.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1012 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/boost.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7489 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.3/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      607 2023-11-15 10:24:00.000000 yellowdog-python-examples-7.8.3/yd_commands/check_imports.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2502 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard.py
+-rw-r--r--   0 pwt        (501) staff       (20)    38132 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_aws.py
+-rw-r--r--   0 pwt        (501) staff       (20)      481 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_aws_types.py
+-rw-r--r--   0 pwt        (501) staff       (20)    31534 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_azure.py
+-rw-r--r--   0 pwt        (501) staff       (20)    13236 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_common.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12227 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_gcp.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2023-09-02 10:35:56.000000 yellowdog-python-examples-7.8.3/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3529 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/config_types.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    29810 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/yd_commands/create.py
+-rw-r--r--   0 pwt        (501) staff       (20)    13603 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.3/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2479 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4715 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      329 2023-09-04 08:20:55.000000 yellowdog-python-examples-7.8.3/yd_commands/follow.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3526 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.3/yd_commands/follow_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1494 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/format_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      290 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.3/yd_commands/hold.py
+-rw-r--r--   0 pwt        (501) staff       (20)      842 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/id_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    12170 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.3/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5005 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/interactive.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1007 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/yd_commands/items.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-09-02 10:35:56.000000 yellowdog-python-examples-7.8.3/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    18464 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)    15959 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/load_config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3861 2024-03-22 10:21:47.000000 yellowdog-python-examples-7.8.3/yd_commands/load_resources.py
+-rw-r--r--   0 pwt        (501) staff       (20)     8703 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)    32348 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/printing.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5782 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/property_names.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    17214 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)     4748 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    13555 2024-03-26 08:47:18.000000 yellowdog-python-examples-7.8.3/yd_commands/remove.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5169 2023-09-04 08:20:55.000000 yellowdog-python-examples-7.8.3/yd_commands/resize.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3261 2024-03-22 08:21:55.000000 yellowdog-python-examples-7.8.3/yd_commands/settings.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4811 2024-02-27 14:55:53.000000 yellowdog-python-examples-7.8.3/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      298 2024-02-12 09:16:25.000000 yellowdog-python-examples-7.8.3/yd_commands/start.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5072 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/start_hold_common.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    52008 2024-03-06 17:14:28.000000 yellowdog-python-examples-7.8.3/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)    10720 2024-02-14 11:33:32.000000 yellowdog-python-examples-7.8.3/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     4797 2024-02-27 14:55:53.000000 yellowdog-python-examples-7.8.3/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2023-11-24 13:35:57.000000 yellowdog-python-examples-7.8.3/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5352 2023-11-18 08:50:59.000000 yellowdog-python-examples-7.8.3/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3683 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6732 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2486 2024-03-18 08:22:49.000000 yellowdog-python-examples-7.8.3/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    18199 2024-04-02 09:31:11.000000 yellowdog-python-examples-7.8.3/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2024-02-26 11:02:40.000000 yellowdog-python-examples-7.8.3/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3747 2024-02-08 14:04:26.000000 yellowdog-python-examples-7.8.3/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2024-04-02 09:31:50.901675 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     2686 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1934 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      860 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      253 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2024-04-02 09:31:50.000000 yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-7.8.2/LICENSE` & `yellowdog-python-examples-7.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/PKG-INFO` & `yellowdog-python-examples-7.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 7.8.2
+Version: 7.8.3
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: yellowdog-sdk>=8.0.0
 Requires-Dist: toml
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: PyPAC>=0.16.4
-Requires-Dist: rich>=13.5.2
+Requires-Dist: rich>=13.7.1
 Requires-Dist: requests
 Requires-Dist: boto3
 Requires-Dist: google-cloud-compute
 Requires-Dist: google-cloud-storage
 Requires-Dist: azure-identity
 Requires-Dist: azure-mgmt-resource
 Requires-Dist: azure-mgmt-network
```

### Comparing `yellowdog-python-examples-7.8.2/PYPI_README.md` & `yellowdog-python-examples-7.8.3/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/README.md` & `yellowdog-python-examples-7.8.3/README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/pyproject.toml` & `yellowdog-python-examples-7.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/setup.cfg` & `yellowdog-python-examples-7.8.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/tests/test_create_remove.py` & `yellowdog-python-examples-7.8.3/tests/test_create_remove.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/tests/test_demos.py` & `yellowdog-python-examples-7.8.3/tests/test_demos.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import pytest
 from cli_test_helpers import shell
 
 DEMO_DIR = "../python-examples-demos"
 CMD_SEQ = "yd-provision && yd-submit -f && yd-terminate -y && yd-delete -y"
+NEXTFLOW = "/Users/pwt/nextflow/nextflow"
 
 
 @pytest.mark.demos
 class TestDemos:
     def test_bash(self):
         result = shell(f"cd {DEMO_DIR}/bash && {CMD_SEQ}")
         assert result.exit_code == 0
@@ -47,7 +48,28 @@
     def test_powershell(self):
         result = shell(f"cd {DEMO_DIR}/powershell && {CMD_SEQ}")
         assert result.exit_code == 0
 
     def test_cmd_exe(self):
         result = shell(f"cd {DEMO_DIR}/cmd.exe && {CMD_SEQ}")
         assert result.exit_code == 0
+
+    def test_nextflow_image_montage(self):
+        result = shell(
+            f"cd {DEMO_DIR}/nextflow/image-montage && {NEXTFLOW} main.nf "
+            "&& cd .. && ./cleanup.sh"
+        )
+        assert result.exit_code == 0
+
+    def test_nextflow_salmon_rna(self):
+        result = shell(
+            f"cd {DEMO_DIR}/nextflow/salmon-rna && {NEXTFLOW} main.nf "
+            "&& cd .. && ./cleanup.sh"
+        )
+        assert result.exit_code == 0
+
+    def test_cmd_modelled_on_premise(self):
+        result = shell(
+            f"cd {DEMO_DIR}/modelled-on-premise && yd-instantiate "
+            "&& sleep 120 && yd-terminate -y"
+        )
+        assert result.exit_code == 0
```

### Comparing `yellowdog-python-examples-7.8.2/tests/test_dryruns.py` & `yellowdog-python-examples-7.8.3/tests/test_dryruns.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/tests/test_entrypoints.py` & `yellowdog-python-examples-7.8.3/tests/test_entrypoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,7 +38,13 @@
     assert result.exit_code == 0
     result = shell("yd-upload --help")
     assert result.exit_code == 0
     result = shell("yd-version")
     assert result.exit_code == 0
     result = shell("yd-cloudwizard --help")
     assert result.exit_code == 0
+    result = shell("yd-start --help")
+    assert result.exit_code == 0
+    result = shell("yd-hold --help")
+    assert result.exit_code == 0
+    result = shell("yd-boost --help")
+    assert result.exit_code == 0
```

### Comparing `yellowdog-python-examples-7.8.2/tests/test_gui.py` & `yellowdog-python-examples-7.8.3/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/tests/test_list.py` & `yellowdog-python-examples-7.8.3/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/tests/test_objects.py` & `yellowdog-python-examples-7.8.3/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/tests/test_variable_processing.py` & `yellowdog-python-examples-7.8.3/tests/test_variable_processing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/abort.py` & `yellowdog-python-examples-7.8.3/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/admin.py` & `yellowdog-python-examples-7.8.3/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/args.py` & `yellowdog-python-examples-7.8.3/yd_commands/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,16 +127,14 @@
             for module in [
                 "boost",
                 "resize",
                 "create",
                 "remove",
                 "cloudwizard",
                 "follow",
-                "hold",
-                "start",
             ]
         ):
             parser.add_argument(
                 "--namespace",
                 "-n",
                 type=str,
                 required=False,
@@ -334,22 +332,24 @@
                 "cancel",
                 "delete",
                 "shutdown",
                 "terminate",
                 "resize",
                 "cloudwizard",
                 "boost",
+                "hold",
+                "start",
             ]
         ):
             parser.add_argument(
                 "--yes",
                 "-y",
                 action="store_true",
                 required=False,
-                help="perform destructive actions without requiring user confirmation",
+                help="perform modifying actions without requiring user confirmation",
             )
 
         if any(module in sys.argv[0] for module in ["delete", "download"]):
             parser.add_argument(
                 "--all",
                 "-a",
                 action="store_true",
@@ -636,25 +636,26 @@
                 action="store_true",
                 required=False,
                 help="resize a compute requirement instead of a worker pool",
             )
 
         if "boost" in sys.argv[0]:
             parser.add_argument(
-                "allowance",
-                metavar="<allowance-ID>",
-                type=str,
-                help=("the YellowDog ID of the allowance to boost"),
-            )
-            parser.add_argument(
                 "boost_hours",
                 metavar="<boost hours>",
                 type=int,
                 help="the number of hours to boost the allowance by",
             )
+            parser.add_argument(
+                "allowances",
+                metavar="<allowance-ID> [<allowance-ID>]",
+                nargs="+",
+                type=str,
+                help="the YellowDog ID(s) of the allowance(s) to boost",
+            )
 
         if "shutdown" in sys.argv[0]:
             parser.add_argument(
                 "worker_pool_list",
                 nargs="*",
                 default="",
                 metavar="<worker-pool-name-or-ID>",
@@ -1397,16 +1398,16 @@
     @property
     @allow_missing_attribute
     def object_path_pattern(self) -> Optional[str]:
         return self.args.pattern
 
     @property
     @allow_missing_attribute
-    def allowance(self) -> str:
-        return self.args.allowance
+    def allowance_list(self) -> List[str]:
+        return self.args.allowances
 
     @property
     @allow_missing_attribute
     def boost_hours(self) -> int:
         return self.args.boost_hours
 
     @property
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/boost.py` & `yellowdog-python-examples-7.8.3/yd_commands/boost.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 #!/usr/bin/env python3
 
 """
 A script to boost allowances.
 """
 
 from yd_commands.interactive import confirmed
-from yd_commands.printing import print_log
+from yd_commands.printing import print_error, print_log
 from yd_commands.wrapper import ARGS_PARSER, CLIENT, main_wrapper
 
 
 @main_wrapper
 def main():
-    if not confirmed(
-        f"Boost Allowance {ARGS_PARSER.allowance} by {ARGS_PARSER.boost_hours} hours?"
-    ):
-        return
-
-    try:
-        CLIENT.allowances_client.boost_allowance_by_id(
-            ARGS_PARSER.allowance, ARGS_PARSER.boost_hours
-        )
-    except Exception as e:
-        raise Exception(f"Unable to boost Allowance {ARGS_PARSER.allowance}: {e}")
-
-    print_log(
-        f"Boosted Allowance {ARGS_PARSER.allowance} by {ARGS_PARSER.boost_hours} hours"
-    )
+
+    count = 0
+    for allowance in ARGS_PARSER.allowance_list:
+        if not confirmed(
+            f"Boost Allowance {allowance} by {ARGS_PARSER.boost_hours} hours?"
+        ):
+            continue
+        try:
+            CLIENT.allowances_client.boost_allowance_by_id(
+                allowance, ARGS_PARSER.boost_hours
+            )
+            print_log(
+                f"Boosted Allowance {allowance} by {ARGS_PARSER.boost_hours} hours"
+            )
+            count += 1
+        except Exception as e:
+            print_error(f"Unable to boost Allowance {allowance}: {e}")
+
+    if count > 1:
+        print_log(f"Boosted {count} allowances by {ARGS_PARSER.boost_hours} hours")
 
 
 # Standalone entry point
 if __name__ == "__main__":
     main()
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/cancel.py` & `yellowdog-python-examples-7.8.3/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/check_imports.py` & `yellowdog-python-examples-7.8.3/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/cloudwizard.py` & `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/cloudwizard_aws.py` & `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,50 +75,52 @@
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
 
 YELLOWDOG_POLICY = {
     "Version": "2012-10-17",
-    "Statement": [{
-        "Sid": "VisualEditor0",
-        "Effect": "Allow",
-        "Action": [
-            "EC2:CancelSpotInstanceRequests",
-            "EC2:CreateFleet",
-            "EC2:CreateLaunchTemplate",
-            "EC2:CreatePlacementGroup",
-            "EC2:CreateTags",
-            "EC2:DeleteFleets",
-            "EC2:DeleteLaunchTemplate",
-            "EC2:DeletePlacementGroup",
-            "EC2:DescribeFleets",
-            "EC2:DescribeInstanceTypes",
-            "EC2:DescribeInstances",
-            "EC2:DescribeLaunchTemplates",
-            "EC2:DescribePlacementGroups",
-            "EC2:DescribeSpotInstanceRequests",
-            "EC2:ModifyFleet",
-            "EC2:RebootInstances",
-            "EC2:RequestSpotInstances",
-            "EC2:RunInstances",
-            "EC2:StartInstances",
-            "EC2:StopInstances",
-            "EC2:TerminateInstances",
-            "S3:AbortMultipartUpload",
-            "S3:CreateBucket",
-            "S3:DeleteBucket",
-            "S3:DeleteObject",
-            "S3:GetObject",
-            "S3:ListBucketMultipartUploads",
-            "S3:ListMultipartUploadParts",
-            "S3:PutObject",
-        ],
-        "Resource": "*",
-    }],
+    "Statement": [
+        {
+            "Sid": "VisualEditor0",
+            "Effect": "Allow",
+            "Action": [
+                "EC2:CancelSpotInstanceRequests",
+                "EC2:CreateFleet",
+                "EC2:CreateLaunchTemplate",
+                "EC2:CreatePlacementGroup",
+                "EC2:CreateTags",
+                "EC2:DeleteFleets",
+                "EC2:DeleteLaunchTemplate",
+                "EC2:DeletePlacementGroup",
+                "EC2:DescribeFleets",
+                "EC2:DescribeInstanceTypes",
+                "EC2:DescribeInstances",
+                "EC2:DescribeLaunchTemplates",
+                "EC2:DescribePlacementGroups",
+                "EC2:DescribeSpotInstanceRequests",
+                "EC2:ModifyFleet",
+                "EC2:RebootInstances",
+                "EC2:RequestSpotInstances",
+                "EC2:RunInstances",
+                "EC2:StartInstances",
+                "EC2:StopInstances",
+                "EC2:TerminateInstances",
+                "S3:AbortMultipartUpload",
+                "S3:CreateBucket",
+                "S3:DeleteBucket",
+                "S3:DeleteObject",
+                "S3:GetObject",
+                "S3:ListBucketMultipartUploads",
+                "S3:ListMultipartUploadParts",
+                "S3:PutObject",
+            ],
+            "Resource": "*",
+        }
+    ],
 }
 
 
 class AWSConfig(CommonCloudConfig):
     """
     Class for managing the AWS configuration.
     """
@@ -178,20 +180,22 @@
 
     def set_ssh_ingress_rule(self, operation: str, selected_region: str = None):
         """
         Add or remove SSH ingress for all relevant security groups.
         A list of regions can be supplied as an argument.
         The 'operation' argument must be 'add-ssh' or 'remove-ssh'.
         """
-        ssh_ipv4_ingress_rule = [{
-            "IpProtocol": "tcp",
-            "FromPort": 22,
-            "ToPort": 22,
-            "IpRanges": [{"CidrIp": f"0.0.0.0/0"}],
-        }]
+        ssh_ipv4_ingress_rule = [
+            {
+                "IpProtocol": "tcp",
+                "FromPort": 22,
+                "ToPort": 22,
+                "IpRanges": [{"CidrIp": f"0.0.0.0/0"}],
+            }
+        ]
         for region in (
             AWS_YD_IMAGE_REGIONS if selected_region is None else [selected_region]
         ):
             ec2_client = boto3.client("ec2", region_name=region)
             # Collect the default security group for the region
             try:
                 response = ec2_client.describe_security_groups(Filters=[])
@@ -355,19 +359,21 @@
             print_error("No access keys loaded; can't create Credential")
 
         # Create namespace configuration (Keyring/Credential creation must come first)
         print_log(
             "Creating YellowDog Namespace Configuration"
             f" 'S3:{self._get_s3_bucket_name()}' -> '{YD_NAMESPACE}'"
         )
-        create_resources([
-            self._generate_yd_namespace_configuration(
-                namespace=YD_NAMESPACE, s3_bucket_name=self._get_s3_bucket_name()
-            )
-        ])
+        create_resources(
+            [
+                self._generate_yd_namespace_configuration(
+                    namespace=YD_NAMESPACE, s3_bucket_name=self._get_s3_bucket_name()
+                )
+            ]
+        )
 
         # Sequence the Compute Requirement Templates before the Compute Source
         # Templates for subsequent removals.
         # - Omit the Keyring to prevent overwrites if using 'yd-create' with the
         #   resource file.
         # - Omit the Credential for security reasons.
         self._save_resource_list(
@@ -386,19 +392,21 @@
             client=self._client, name_prefix=YD_RESOURCE_PREFIX
         )
 
         # Keyring is removed separately.
         self._remove_keyring(keyring_name=YD_KEYRING_NAME)
 
         # Remove the Namespace Configuration
-        remove_resources([
-            self._generate_yd_namespace_configuration(
-                YD_NAMESPACE, self._get_s3_bucket_name()
-            )
-        ])
+        remove_resources(
+            [
+                self._generate_yd_namespace_configuration(
+                    YD_NAMESPACE, self._get_s3_bucket_name()
+                )
+            ]
+        )
 
     def _gather_aws_network_information(self):
         """
         Collect network information about the enabled regions and AZs.
         """
         print_log(
             "Gathering network information for all AWS regions containing YellowDog VM"
@@ -957,31 +965,33 @@
 
     def _generate_s3_bucket_policy(self) -> str:
         """
         Generate the required policy statement to be attached to the S3 bucket.
         """
         assert self._aws_user is not None
         s3_bucket_name = self._get_s3_bucket_name()
-        return json.dumps({
-            "Version": "2012-10-17",
-            "Statement": [
-                {
-                    "Effect": "Allow",
-                    "Principal": {"AWS": self._aws_user.arn},
-                    "Action": "s3:*",
-                    "Resource": f"arn:aws:s3:::{s3_bucket_name}/*",
-                },
-                {
-                    "Effect": "Allow",
-                    "Principal": {"AWS": self._aws_user.arn},
-                    "Action": "s3:ListBucket",
-                    "Resource": f"arn:aws:s3:::{s3_bucket_name}",
-                },
-            ],
-        })
+        return json.dumps(
+            {
+                "Version": "2012-10-17",
+                "Statement": [
+                    {
+                        "Effect": "Allow",
+                        "Principal": {"AWS": self._aws_user.arn},
+                        "Action": "s3:*",
+                        "Resource": f"arn:aws:s3:::{s3_bucket_name}/*",
+                    },
+                    {
+                        "Effect": "Allow",
+                        "Principal": {"AWS": self._aws_user.arn},
+                        "Action": "s3:ListBucket",
+                        "Resource": f"arn:aws:s3:::{s3_bucket_name}",
+                    },
+                ],
+            }
+        )
 
     def _get_s3_bucket_name(self) -> str:
         """
         Get the unique name of the S3 bucket.
         """
         return (
             f"{S3_BUCKET_NAME_PREFIX}-{self._aws_user.user_id.lower()}"
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/cloudwizard_azure.py` & `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_azure.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,19 +487,21 @@
             except Exception as e:
                 print_error(
                     f"Unable to add credential '{YD_CREDENTIAL_NAME_STORAGE}': {e}"
                 )
 
         # Create namespace configuration (Keyring/Credential creation must come first)
         print_log(f"Creating YellowDog Namespace Configuration '{YD_NAMESPACE}'")
-        create_resources([
-            self._generate_yd_namespace_configuration(
-                namespace=YD_NAMESPACE, storage_blob_name=STORAGE_BLOB_NAME
-            )
-        ])
+        create_resources(
+            [
+                self._generate_yd_namespace_configuration(
+                    namespace=YD_NAMESPACE, storage_blob_name=STORAGE_BLOB_NAME
+                )
+            ]
+        )
 
         # Save the list of resources
         # Sequence the Compute Requirement Templates before the Compute Source
         # Templates for subsequent removals.
         # - Omit the Keyring to prevent overwrites if using 'yd-create' with the
         #   resource file
         # - Omit the Credential for security reasons
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/cloudwizard_common.py` & `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,20 +182,22 @@
                 },
                 {
                     "anyOf": [self._cloud_provider],
                     "attribute": "source.provider",
                     "type": "co.yellowdog.platform.model.StringAttributeConstraint",
                 },
             ],
-            "preferences": [{
-                "attribute": "yd.cost",
-                "rankOrder": "PREFER_LOWER",
-                "type": "co.yellowdog.platform.model.NumericAttributePreference",
-                "weight": 1,
-            }],
+            "preferences": [
+                {
+                    "attribute": "yd.cost",
+                    "rankOrder": "PREFER_LOWER",
+                    "type": "co.yellowdog.platform.model.NumericAttributePreference",
+                    "weight": 1,
+                }
+            ],
             "maximumSourceCount": 5,
             "minimumSourceCount": 1,
             "strategyType": f"co.yellowdog.platform.model.{strategy}ProvisionStrategy",
             "type": "co.yellowdog.platform.model.ComputeRequirementDynamicTemplate",
         }
 
     @staticmethod
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/cloudwizard_gcp.py` & `yellowdog-python-examples-7.8.3/yd_commands/cloudwizard_gcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,21 +154,23 @@
         """
         Remove YellowDog resources in the Platform account.
         """
         self._remove_yd_templates_by_prefix(
             client=self._client, name_prefix=YD_RESOURCE_PREFIX
         )
         self._remove_keyring(YD_KEYRING_NAME)
-        remove_resources([
-            self._generate_namespace_configuration(
-                YD_NAMESPACE,
-                self._generate_bucket_name(),
-                credential_name=f"{YD_KEYRING_NAME}/{YD_CREDENTIAL_NAME}",
-            )
-        ])
+        remove_resources(
+            [
+                self._generate_namespace_configuration(
+                    YD_NAMESPACE,
+                    self._generate_bucket_name(),
+                    credential_name=f"{YD_KEYRING_NAME}/{YD_CREDENTIAL_NAME}",
+                )
+            ]
+        )
 
     def _gather_regions(self):
         """
         Find the regions in the default VPC with default subnets.
         """
         try:
             networks = compute_v1.NetworksClient(credentials=self._credentials).list(
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/compact_json.py` & `yellowdog-python-examples-7.8.3/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/config_types.py` & `yellowdog-python-examples-7.8.3/yd_commands/config_types.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/create.py` & `yellowdog-python-examples-7.8.3/yd_commands/create.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/csv_data.py` & `yellowdog-python-examples-7.8.3/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/delete.py` & `yellowdog-python-examples-7.8.3/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/download.py` & `yellowdog-python-examples-7.8.3/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/follow_utils.py` & `yellowdog-python-examples-7.8.3/yd_commands/follow_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/format_json.py` & `yellowdog-python-examples-7.8.3/yd_commands/format_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/id_utils.py` & `yellowdog-python-examples-7.8.3/yd_commands/id_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/instantiate.py` & `yellowdog-python-examples-7.8.3/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/interactive.py` & `yellowdog-python-examples-7.8.3/yd_commands/interactive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-User interaction processing
+User interaction processing utilities.
 """
 
 from os import getenv
 from typing import List, Optional, Set, Union
 
 from yellowdog_client import PlatformClient
 
@@ -72,16 +72,14 @@
         cancel_string = "" if result_required else " or press <Return> to cancel"
         input_string = (
             f"Please select an item number{cancel_string}:"
             if single_result
             else (f"Please select items (e.g.: 1,2,4-7 / *){cancel_string}:")
         )
         selector_string = CONSOLE.input(print_string(input_string) + " ")
-        if selector_string == "":  # A quirk of Rich?
-            print()
         if selector_string.strip() == "*":
             selector_string = f"1-{len(objects)}"
         selector_list = selector_string.split(",")
         selector_set: Set[int] = set()
         error_flag = False
         for selector in selector_list:
             try:
@@ -152,15 +150,13 @@
             f"'{YD_YES}={yd_yes}': Action proceeding without user confirmation ({msg})"
         )
         return True
 
     # Seek user confirmation
     while True:
         response = CONSOLE.input(print_string(f"{msg} (y/N):") + " ")
-        if response == "":  # Seems to be a quirk of Rich
-            print()
         if response.lower() in ["y", "yes"]:
             print_log("Action confirmed by user")
             return True
         elif response.lower() in ["n", "no", ""]:
             print_log("Action cancelled by user")
             return False
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/items.py` & `yellowdog-python-examples-7.8.3/yd_commands/items.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-7.8.3/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/list.py` & `yellowdog-python-examples-7.8.3/yd_commands/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,18 +515,20 @@
     all_fields = sorted(list(all_fields))
     all_fields.insert(0, "type")
     all_fields.insert(0, "namespace")
 
     # Assemble and print the table
     headings = [field.capitalize() for field in all_fields]
     headings.insert(0, "#")
-    rows = sorted([
-        [index + 1] + [namespace.get(field, "") for field in all_fields]
-        for index, namespace in enumerate(namespace_list)
-    ])
+    rows = sorted(
+        [
+            [index + 1] + [namespace.get(field, "") for field in all_fields]
+            for index, namespace in enumerate(namespace_list)
+        ]
+    )
     print()
     CONSOLE_TABLE.print(
         indent(tabulate(rows, headings, tablefmt="simple_outline")),
     )
     print()
 
     if ARGS_PARSER.details:  # Print the details for non-default only
@@ -540,15 +542,15 @@
     """
     allowances_search = AllowanceSearch()
     search_client: SearchClient = CLIENT.allowances_client.get_allowances(
         allowances_search
     )
     allowances: List[Allowance] = search_client.list_all()
     if len(allowances) == 0:
-        print_log("No allowances to display")
+        print_log("No Allowances to display")
         return
 
     if not ARGS_PARSER.details:
         print_numbered_object_list(CLIENT, allowances)
         return
 
     for allowance in select(CLIENT, allowances):
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/load_config.py` & `yellowdog-python-examples-7.8.3/yd_commands/load_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Common utility functions, mostly related to loading configuration data.
 """
 
 import os
 from os import getenv
-from os.path import dirname, relpath
+from os.path import dirname, join, relpath
 from sys import exit
 from typing import Dict, Optional
 
 from toml import TomlDecodeError
 
 from yd_commands.args import ARGS_PARSER
 from yd_commands.config_types import (
@@ -37,26 +37,26 @@
     add_substitutions_without_overwriting,
     load_toml_file_with_variable_substitutions,
     process_variable_substitutions,
     process_variable_substitutions_insitu,
 )
 
 # CLI > YD_CONF > 'config.toml'
-config_file = relpath(
+CONFIG_FILE = relpath(
     getenv("YD_CONF", "config.toml")
     if ARGS_PARSER.config_file is None
     else ARGS_PARSER.config_file
 )
 
 try:
-    CONFIG_FILE_DIR = dirname(config_file)
-    print_log(f"Loading configuration data from: '{config_file}'")
-    CONFIG_TOML: Dict = load_toml_file_with_variable_substitutions(config_file)
+    CONFIG_FILE_DIR = dirname(CONFIG_FILE)
+    print_log(f"Loading configuration data from: '{CONFIG_FILE}'")
+    CONFIG_TOML: Dict = load_toml_file_with_variable_substitutions(CONFIG_FILE)
     try:
-        validate_properties(CONFIG_TOML, f"'{config_file}'")
+        validate_properties(CONFIG_TOML, f"'{CONFIG_FILE}'")
     except Exception as e:
         print_error(e)
         exit(1)
 
 except FileNotFoundError as e:
     if ARGS_PARSER.config_file is not None:
         print_error(e)
@@ -67,15 +67,15 @@
         "or in environment variables"
     )
     CONFIG_TOML = {COMMON_SECTION: {}}
     CONFIG_FILE_DIR = os.getcwd()
 
 except (PermissionError, TomlDecodeError) as e:
     print_error(
-        f"Unable to load configuration data from '{config_file}': {e}",
+        f"Unable to load configuration data from '{CONFIG_FILE}': {e}",
     )
     exit(1)
 
 except Exception as e:
     print_error(e)
     exit(1)
 
@@ -83,15 +83,15 @@
 def load_config_common() -> ConfigCommon:
     """
     Load the configuration values for the 'common' section.
     """
     try:
         common_section = CONFIG_TOML.get(COMMON_SECTION, {})
 
-        # Check for IMPORT directive (common section in a separate file)
+        # Check for IMPORT directive ('common' section in a separate file)
         common_section_import_file = common_section.get(IMPORT_COMMON, None)
         if common_section_import_file is not None:
             common_section = import_toml(common_section_import_file)
 
         # Replace common section properties with command line or
         # environment variable overrides. Precedence is:
         # command line > environment variable > config file
@@ -156,14 +156,15 @@
 
     except KeyError as e:
         print_error(f"Missing configuration data: {e}")
         exit(1)
 
 
 def import_toml(filename: str) -> Dict:
+    filename = relpath(join(CONFIG_FILE_DIR, process_variable_substitutions(filename)))
     print_log(f"Loading imported common configuration data from: '{filename}'")
     try:
         common_config: Dict = load_toml_file_with_variable_substitutions(filename)
         return common_config[COMMON_SECTION]
     except (FileNotFoundError, PermissionError, TomlDecodeError) as e:
         print_error(f"Unable to load imported common configuration data: {e}")
         exit(1)
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/load_resources.py` & `yellowdog-python-examples-7.8.3/yd_commands/load_resources.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/object_utilities.py` & `yellowdog-python-examples-7.8.3/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/printing.py` & `yellowdog-python-examples-7.8.3/yd_commands/printing.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,79 +242,87 @@
         "Namespace",
         "Tag",
         "Status (Tgt/Exp)",
         "ID",
     ]
     table = []
     for index, cr in enumerate(cr_list):
-        table.append([
-            index + 1,
-            cr.name,
-            cr.namespace,
-            cr.tag,
-            (
-                f"{cr.status}"
-                if cr.nextStatus is None
-                else (f"{cr.status} -> {cr.nextStatus}")
-            )
-            + f" ({cr.targetInstanceCount:,d}/{cr.expectedInstanceCount:,d})",
-            cr.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                cr.name,
+                cr.namespace,
+                cr.tag,
+                (
+                    f"{cr.status}"
+                    if cr.nextStatus is None
+                    else (f"{cr.status} -> {cr.nextStatus}")
+                )
+                + f" ({cr.targetInstanceCount:,d}/{cr.expectedInstanceCount:,d})",
+                cr.id,
+            ]
+        )
     return headers, table
 
 
 def work_requirement_table(
     wr_summary_list: List[WorkRequirementSummary],
 ) -> (List[str], List[List]):
     headers = ["#", "Work Requirement Name", "Namespace", "Tag", "Status", "ID"]
     table = []
     for index, wr_summary in enumerate(wr_summary_list):
         namespace = "" if wr_summary.namespace is None else wr_summary.namespace
         tag = "" if wr_summary.tag is None else wr_summary.tag
-        table.append([
-            index + 1,
-            wr_summary.name,
-            namespace,
-            tag,
-            str(wr_summary.status),
-            wr_summary.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                wr_summary.name,
+                namespace,
+                tag,
+                str(wr_summary.status),
+                wr_summary.id,
+            ]
+        )
     return headers, table
 
 
 def task_group_table(
     task_group_list: List[TaskGroup],
 ) -> (List[str], List[List]):
     headers = ["#", "Task Group Name", "Status", "ID"]
     table = []
     for index, task_group in enumerate(task_group_list):
         status_msg = str(task_group.status)
         if task_group.starved:
             status_msg += "/STARVED"
         if task_group.waitingOnDependency:
             status_msg += "/WAITING"
-        table.append([
-            index + 1,
-            task_group.name,
-            status_msg,
-            task_group.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                task_group.name,
+                status_msg,
+                task_group.id,
+            ]
+        )
     return headers, table
 
 
 def task_table(task_list: List[Task]) -> (List[str], List[List]):
     headers = ["#", "Task Name", "Status", "ID"]
     table = []
     for index, task in enumerate(task_list):
-        table.append([
-            index + 1,
-            task.name,
-            str(task.status),
-            task.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                task.name,
+                str(task.status),
+                task.id,
+            ]
+        )
     return headers, table
 
 
 def worker_pool_table(
     client: PlatformClient, worker_pool_summaries: List[WorkerPoolSummary]
 ) -> (List[str], List[List]):
     headers = [
@@ -337,22 +345,24 @@
         try:
             max_nodes = str(worker_pool.properties.maxNodes)
         except:
             max_nodes = "_"
         node_summary: NodeSummary = worker_pool.nodeSummary
         nodes_running = node_summary.statusCounts[NodeStatus.RUNNING]
 
-        table.append([
-            index + 1,
-            worker_pool_summary.name,
-            f"{worker_pool_summary.type.split('.')[-1:][0].replace('WorkerPool', '')}",
-            f"{worker_pool_summary.status}",
-            f"{min_nodes}/{nodes_running}/{max_nodes}",
-            worker_pool_summary.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                worker_pool_summary.name,
+                f"{worker_pool_summary.type.split('.')[-1:][0].replace('WorkerPool', '')}",
+                f"{worker_pool_summary.status}",
+                f"{min_nodes}/{nodes_running}/{max_nodes}",
+                worker_pool_summary.id,
+            ]
+        )
     return headers, table
 
 
 def compute_requirement_template_table(
     crt_summaries: List[ComputeRequirementTemplateSummary],
 ) -> (List[str], List[List]):
     headers = [
@@ -371,22 +381,24 @@
             type = None
         try:
             strategy_type = crt_summary.strategyType.split(".")[-1].replace(
                 "ProvisionStrategy", ""
             )
         except:
             strategy_type = None
-        table.append([
-            index + 1,
-            crt_summary.name,
-            crt_summary.namespace,
-            type,
-            strategy_type,
-            crt_summary.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                crt_summary.name,
+                crt_summary.namespace,
+                type,
+                strategy_type,
+                crt_summary.id,
+            ]
+        )
     return headers, table
 
 
 def compute_source_template_table(
     cst_summaries: List[ComputeSourceTemplateSummary],
 ) -> (List[str], List[List]):
     headers = [
@@ -403,42 +415,46 @@
             type = cst_summary.sourceType.split(".")[-1]
         except:
             type = None
         try:
             provider = cst_summary.provider
         except:
             provider = None
-        table.append([
-            index + 1,
-            cst_summary.name,
-            cst_summary.namespace,
-            provider,
-            type,
-            cst_summary.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                cst_summary.name,
+                cst_summary.namespace,
+                provider,
+                type,
+                cst_summary.id,
+            ]
+        )
     return headers, table
 
 
 def keyring_table(
     keyring_summaries: List[KeyringSummary],
 ) -> (List[str], List[List]):
     headers = [
         "#",
         "Name",
         "Description",
         "ID",
     ]
     table = []
     for index, keyring in enumerate(keyring_summaries):
-        table.append([
-            index + 1,
-            keyring.name,
-            keyring.description,
-            keyring.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                keyring.name,
+                keyring.description,
+                keyring.id,
+            ]
+        )
     return headers, table
 
 
 def image_family_table(
     image_family_summaries: List[MachineImageFamilySummary],
 ) -> (List[str], List[str]):
     headers = [
@@ -447,22 +463,24 @@
         "Access",
         "Namespace",
         "OS Type",
         "ID",
     ]
     table = []
     for index, image_family in enumerate(image_family_summaries):
-        table.append([
-            index + 1,
-            image_family.name,
-            image_family.access,
-            image_family.namespace,
-            image_family.osType,
-            image_family.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                image_family.name,
+                image_family.access,
+                image_family.namespace,
+                image_family.osType,
+                image_family.id,
+            ]
+        )
     return headers, table
 
 
 def object_path_table(
     object_paths: List[ObjectPath],
 ) -> (List[str], List[str]):
     headers = ["#", "Name"]
@@ -481,22 +499,24 @@
         "Provider",
         "Instance Type",
         "Private IP",
         "Public IP",
     ]
     table = []
     for index, instance in enumerate(instances):
-        table.append([
-            index + 1,
-            instance.type.split(".")[-1],
-            instance.provider,
-            instance.instanceType,
-            instance.privateIpAddress,
-            instance.publicIpAddress,
-        ])
+        table.append(
+            [
+                index + 1,
+                instance.type.split(".")[-1],
+                instance.provider,
+                instance.instanceType,
+                instance.privateIpAddress,
+                instance.publicIpAddress,
+            ]
+        )
     return headers, table
 
 
 def allowances_table(
     allowances: List[Allowance],
 ) -> (List[str], List[str]):
     headers = [
@@ -507,48 +527,52 @@
         "Remaining Hrs",
         "Limit",
         "Reset",
         "ID",
     ]
     table = []
     for index, allowance in enumerate(allowances):
-        table.append([
-            index + 1,
-            allowance.type.split(".")[-1],
-            allowance.description,
-            allowance.allowedHours,
-            allowance.remainingHours,
-            allowance.limitEnforcement,
-            (
-                f"{allowance.resetInterval} {allowance.resetType}"
-                if allowance.resetInterval is not None
-                else ""
-            ),
-            allowance.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                allowance.type.split(".")[-1],
+                allowance.description,
+                allowance.allowedHours,
+                allowance.remainingHours,
+                allowance.limitEnforcement,
+                (
+                    f"{allowance.resetInterval} {allowance.resetType}"
+                    if allowance.resetInterval is not None
+                    else ""
+                ),
+                allowance.id,
+            ]
+        )
     return headers, table
 
 
 def aws_availability_zone_table(
     aws_azs: List[AWSAvailabilityZone],
 ) -> (List[str], List[str]):
     headers = [
         "#",
         "Availability Zone",
         "Default Subnet ID",
         "Default Security Group ID",
     ]
     table = []
     for index, az in enumerate(aws_azs):
-        table.append([
-            index + 1,
-            az.az,
-            az.default_subnet_id,
-            az.default_sec_grp.id,
-        ])
+        table.append(
+            [
+                index + 1,
+                az.az,
+                az.default_subnet_id,
+                az.default_sec_grp.id,
+            ]
+        )
     return headers, table
 
 
 def print_numbered_object_list(
     client: PlatformClient,
     objects: List[Union[Item, str]],
     object_type_name: Optional[str] = None,
@@ -786,33 +810,37 @@
     """
     if not isinstance(result, ComputeRequirementDynamicTemplateTestResult):
         print_log("Reports are only available for Dynamic Templates")
         return
 
     report: BestComputeSourceReport = result.report
     sources: List[BestComputeSourceReportSource] = report.sources
-    source_table = [[
-        "#",
-        "Rank",
-        "Provider",
-        "Type",
-        "Region",
-        "InstanceType",
-        "Source Name",
-    ]]
+    source_table = [
+        [
+            "#",
+            "Rank",
+            "Provider",
+            "Type",
+            "Region",
+            "InstanceType",
+            "Source Name",
+        ]
+    ]
     for index, source in enumerate(sources):
-        source_table.append([
-            index + 1,
-            source.rank,
-            source.provider,
-            source.type,
-            source.region,
-            source.instanceType,
-            source.name,
-        ])
+        source_table.append(
+            [
+                index + 1,
+                source.rank,
+                source.provider,
+                source.type,
+                source.region,
+                source.instanceType,
+                source.name,
+            ]
+        )
     print(flush=True)
     print_table_core(
         indent(tabulate(source_table, headers="firstrow", tablefmt="simple_outline"))
     )
     print(flush=True)
 
 
@@ -835,19 +863,21 @@
     if ARGS_PARSER.quiet:
         return
 
     headers = ["#", "Source Object", "Target Object"]
     table = []
     # Yes, I know I shouldn't be accessing '_source_file_entries'
     for index, file_entry in enumerate(upload_batch_builder._source_file_entries):
-        table.append([
-            index + 1,
-            file_entry.source_file_path,
-            f"{upload_batch_builder.namespace}{NAMESPACE_PREFIX_SEPARATOR}{file_entry.default_object_name}",
-        ])
+        table.append(
+            [
+                index + 1,
+                file_entry.source_file_path,
+                f"{upload_batch_builder.namespace}{NAMESPACE_PREFIX_SEPARATOR}{file_entry.default_object_name}",
+            ]
+        )
     print(flush=True)
     print_table_core(
         indent(
             tabulate(table, headers=headers, tablefmt="simple_outline"),
             indent_width=4,
         )
     )
@@ -872,23 +902,25 @@
     for index, object_entry in enumerate(download_batch_builder._source_object_entries):
         object_source = f"{object_entry.namespace}{NAMESPACE_PREFIX_SEPARATOR}{object_entry.object_name}"
         object_target = (
             f"{object_entry.object_name.replace('/', directory_separator)}"
             if flatten_downloads is False
             else f"{object_entry.object_name.split('/')[-1:][0]}"
         )
-        table.append([
-            index + 1,
-            object_source,
-            relpath(
-                f"{download_batch_builder.destination_folder}"
-                f"{directory_separator}"
-                f"{object_target}"
-            ),
-        ])
+        table.append(
+            [
+                index + 1,
+                object_source,
+                relpath(
+                    f"{download_batch_builder.destination_folder}"
+                    f"{directory_separator}"
+                    f"{object_target}"
+                ),
+            ]
+        )
         counter += 1
 
     print(flush=True)
 
     if ARGS_PARSER.no_format:
         print(
             indent(
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/property_names.py` & `yellowdog-python-examples-7.8.3/yd_commands/property_names.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/provision.py` & `yellowdog-python-examples-7.8.3/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/provision_utils.py` & `yellowdog-python-examples-7.8.3/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/remove.py` & `yellowdog-python-examples-7.8.3/yd_commands/remove.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/resize.py` & `yellowdog-python-examples-7.8.3/yd_commands/resize.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/settings.py` & `yellowdog-python-examples-7.8.3/yd_commands/settings.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/shutdown.py` & `yellowdog-python-examples-7.8.3/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/start_hold_common.py` & `yellowdog-python-examples-7.8.3/yd_commands/start_hold_common.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 
 """
 Core functionality for starting and holding Work Requirements.
 """
 
 from typing import List
 
-from yellowdog_client.model import WorkRequirementStatus, WorkRequirementSummary
+from yellowdog_client.model import (
+    WorkRequirement,
+    WorkRequirementStatus,
+    WorkRequirementSummary,
+)
 
 from yd_commands.follow_utils import follow_ids
-from yd_commands.interactive import select
+from yd_commands.interactive import confirmed, select
 from yd_commands.object_utilities import (
     get_filtered_work_requirements,
     get_work_requirement_summary_by_name_or_id,
 )
 from yd_commands.printing import print_error, print_log, print_warning
+from yd_commands.utils import link_entity
 from yd_commands.wrapper import ARGS_PARSER, CLIENT, CONFIG_COMMON
 
 
 def start_work_requirements():
     required_state = WorkRequirementStatus.HELD
     action_function = CLIENT.work_client.start_work_requirement_by_id
     wr_ids = _start_or_hold_work_requirements("Start", required_state, action_function)
@@ -33,74 +38,75 @@
     if ARGS_PARSER.follow:
         follow_ids(wr_ids)
 
 
 def _start_or_hold_work_requirements(
     action: str, required_state: WorkRequirementStatus, action_function: callable
 ) -> List[str]:
-    """
-    Return the list of YDIDs.
-    """
 
     if len(ARGS_PARSER.work_requirement_names) > 0:
         return _start_or_hold_work_requirements_by_name_or_id(
             action=action,
             required_state=required_state,
             action_function=action_function,
             names_or_ids=ARGS_PARSER.work_requirement_names,
         )
 
     print_log(
-        f"Applying action '{action}' to Work Requirements with "
+        f"{action}ing Work Requirements with "
         f"'{CONFIG_COMMON.namespace}' in namespace and "
         f"'{CONFIG_COMMON.name_tag}' in tag"
     )
 
     selected_work_requirement_summaries: List[WorkRequirementSummary] = (
         get_filtered_work_requirements(
             client=CLIENT,
             namespace=CONFIG_COMMON.namespace,
             tag=CONFIG_COMMON.name_tag,
             include_filter=[required_state],
         )
     )
 
-    processed_count = 0
+    count = 0
     work_requirement_ids: List[str] = []
 
     if len(selected_work_requirement_summaries) > 0:
         selected_work_requirement_summaries = select(
             CLIENT, selected_work_requirement_summaries
         )
 
-    if len(selected_work_requirement_summaries) > 0:
+    if len(selected_work_requirement_summaries) > 0 and confirmed(
+        f"{action} {len(selected_work_requirement_summaries)} Work Requirement(s)?"
+    ):
         for work_summary in selected_work_requirement_summaries:
             if work_summary.status == required_state:
                 try:
                     action_function(work_summary.id)
-                    processed_count += 1
-                    work_requirement_ids.append(work_summary.id)
+                    work_requirement: WorkRequirement = (
+                        CLIENT.work_client.get_work_requirement_by_id(work_summary.id)
+                    )
+                    count += 1
                     print_log(
-                        f"Applied action '{action}' to Work Requirement '{work_summary.name}'"
+                        f"Applied {action} to "
+                        f"{link_entity(CONFIG_COMMON.url, work_requirement)} "
+                        f"('{work_summary.name}')"
                     )
                 except Exception as e:
                     print_error(
-                        f"Unable to apply action '{action}' to Work Requirement '{work_summary.name}': {e}"
+                        f"Failed to {action} Work Requirement '{work_summary.name}': {e}"
                     )
+            work_requirement_ids.append(work_summary.id)
 
-        if processed_count > 1:
-            print_log(
-                f"Applied action '{action}' to {processed_count} Work Requirements"
-            )
+        if count > 0:
+            print_log(f"{action} applied to {count} Work Requirement(s)")
+        else:
+            print_log(f"No Work Requirements to {action}")
 
     else:
-        print_log(
-            f"No matching Work Requirements eligible for action '{action}'"
-            f" (state must be '{required_state}')"
-        )
+        print_log(f"No Work Requirements available to {action}")
 
     return work_requirement_ids
 
 
 def _start_or_hold_work_requirements_by_name_or_id(
     action: str,
     required_state: WorkRequirementStatus,
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/submit.py` & `yellowdog-python-examples-7.8.3/yd_commands/submit.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/submit_utils.py` & `yellowdog-python-examples-7.8.3/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/terminate.py` & `yellowdog-python-examples-7.8.3/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/type_check.py` & `yellowdog-python-examples-7.8.3/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/upload.py` & `yellowdog-python-examples-7.8.3/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/upload_utils.py` & `yellowdog-python-examples-7.8.3/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/utils.py` & `yellowdog-python-examples-7.8.3/yd_commands/utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/validate_properties.py` & `yellowdog-python-examples-7.8.3/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/variables.py` & `yellowdog-python-examples-7.8.3/yd_commands/variables.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,18 +430,20 @@
     with open(resolve_filename(files_directory, filename), "r") as f:
         config = toml_load(f)
 
     # Add any variable substitutions in the TOML file before processing the
     # file as a whole
     try:
         # Convert all values to strings before adding
-        add_substitutions_without_overwriting({
-            var_name: str(var_value)
-            for var_name, var_value in config[COMMON_SECTION][VARIABLES].items()
-        })
+        add_substitutions_without_overwriting(
+            {
+                var_name: str(var_value)
+                for var_name, var_value in config[COMMON_SECTION][VARIABLES].items()
+            }
+        )
     except KeyError:
         pass
 
     # Repeat processing to resolve nested variables
     for _ in range(TOML_VAR_NESTED_DEPTH):
         process_variable_substitutions_insitu(config, prefix=prefix, postfix=postfix)
```

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/version.py` & `yellowdog-python-examples-7.8.3/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yd_commands/wrapper.py` & `yellowdog-python-examples-7.8.3/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 7.8.2
+Version: 7.8.3
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: yellowdog-sdk>=8.0.0
 Requires-Dist: toml
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: PyPAC>=0.16.4
-Requires-Dist: rich>=13.5.2
+Requires-Dist: rich>=13.7.1
 Requires-Dist: requests
 Requires-Dist: boto3
 Requires-Dist: google-cloud-compute
 Requires-Dist: google-cloud-storage
 Requires-Dist: azure-identity
 Requires-Dist: azure-mgmt-resource
 Requires-Dist: azure-mgmt-network
```

### Comparing `yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-7.8.2/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-7.8.3/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

