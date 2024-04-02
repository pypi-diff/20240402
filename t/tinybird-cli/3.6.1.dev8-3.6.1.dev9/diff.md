# Comparing `tmp/tinybird-cli-3.6.1.dev8.tar.gz` & `tmp/tinybird-cli-3.6.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinybird-cli-3.6.1.dev8.tar", last modified: Wed Mar 27 17:34:15 2024, max compression
+gzip compressed data, was "tinybird-cli-3.6.1.dev9.tar", last modified: Thu Mar 28 15:05:40 2024, max compression
```

## Comparing `tinybird-cli-3.6.1.dev8.tar` & `tinybird-cli-3.6.1.dev9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:34:15.664631 tinybird-cli-3.6.1.dev8/
--rw-r--r--   0 root         (0) root         (0)    67840 2024-03-27 17:34:15.664631 tinybird-cli-3.6.1.dev8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 17:34:15.664631 tinybird-cli-3.6.1.dev8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:34:15.660631 tinybird-cli-3.6.1.dev8/tinybird/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-03-27 17:34:14.000000 tinybird-cli-3.6.1.dev8/tinybird/__cli__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:34:15.661631 tinybird-cli-3.6.1.dev8/tinybird/ch_utils/
--rw-rw-rw-   0 root         (0) root         (0)     3657 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/ch_utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    39699 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/ch_utils/engine.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/check_pypi.py
--rw-rw-rw-   0 root         (0) root         (0)    46575 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/client.py
--rw-rw-rw-   0 root         (0) root         (0)     2003 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/config.py
--rw-rw-rw-   0 root         (0) root         (0)     6258 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/connector_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:34:15.661631 tinybird-cli-3.6.1.dev8/tinybird/data_connectors/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/data_connectors/credentials.py
--rw-rw-rw-   0 root         (0) root         (0)   211971 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/datafile.py
--rw-rw-rw-   0 root         (0) root         (0)     7060 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/datatypes.py
--rw-rw-rw-   0 root         (0) root         (0)    59111 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/feedback_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     4707 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/git_settings.py
--rw-rw-rw-   0 root         (0) root         (0)    41181 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/sql.py
--rw-rw-rw-   0 root         (0) root         (0)    76994 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/sql_template.py
--rw-rw-rw-   0 root         (0) root         (0)     9121 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/sql_template_fmt.py
--rw-rw-rw-   0 root         (0) root         (0)    11523 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/sql_toolset.py
--rw-rw-rw-   0 root         (0) root         (0)    27763 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/syncasync.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:34:15.663631 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/
--rw-rw-rw-   0 root         (0) root         (0)     8561 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    37863 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/branch.py
--rw-rw-rw-   0 root         (0) root         (0)    14087 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/cicd.py
--rw-rw-rw-   0 root         (0) root         (0)    64836 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    78344 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/common.py
--rw-rw-rw-   0 root         (0) root         (0)    11484 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/config.py
--rw-rw-rw-   0 root         (0) root         (0)    28107 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/connection.py
--rw-rw-rw-   0 root         (0) root         (0)    31944 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/datasource.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2964 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/job.py
--rw-rw-rw-   0 root         (0) root         (0)    26168 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/pipe.py
--rw-rw-rw-   0 root         (0) root         (0)     2010 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/regions.py
--rw-rw-rw-   0 root         (0) root         (0)    10490 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/telemetry.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:34:15.663631 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/tinyunit/
--rw-rw-rw-   0 root         (0) root         (0)    11667 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/tinyunit/tinyunit.py
--rw-rw-rw-   0 root         (0) root         (0)     1868 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/token.py
--rw-rw-rw-   0 root         (0) root         (0)    10081 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/workspace.py
--rw-rw-rw-   0 root         (0) root         (0)     8268 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/workspace_members.py
--rw-rw-rw-   0 root         (0) root         (0)    41982 2024-03-27 17:34:10.000000 tinybird-cli-3.6.1.dev8/tinybird/tornado_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 17:34:15.664631 tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    67840 2024-03-27 17:34:15.000000 tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1419 2024-03-27 17:34:15.000000 tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 17:34:15.000000 tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-03-27 17:34:15.000000 tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      732 2024-03-27 17:34:15.000000 tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-03-27 17:34:15.000000 tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:05:40.978076 tinybird-cli-3.6.1.dev9/
+-rw-r--r--   0 root         (0) root         (0)    67926 2024-03-28 15:05:40.978076 tinybird-cli-3.6.1.dev9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 15:05:40.978076 tinybird-cli-3.6.1.dev9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:05:40.975076 tinybird-cli-3.6.1.dev9/tinybird/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-03-28 15:05:39.000000 tinybird-cli-3.6.1.dev9/tinybird/__cli__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:05:40.975076 tinybird-cli-3.6.1.dev9/tinybird/ch_utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3657 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/ch_utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    39699 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/ch_utils/engine.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/check_pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)    46575 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2003 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6258 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/connector_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:05:40.975076 tinybird-cli-3.6.1.dev9/tinybird/data_connectors/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/data_connectors/credentials.py
+-rw-rw-rw-   0 root         (0) root         (0)   211971 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/datafile.py
+-rw-rw-rw-   0 root         (0) root         (0)     7060 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/datatypes.py
+-rw-rw-rw-   0 root         (0) root         (0)    59111 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/feedback_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     4707 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/git_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    41181 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    76994 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/sql_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     9121 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/sql_template_fmt.py
+-rw-rw-rw-   0 root         (0) root         (0)    11523 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/sql_toolset.py
+-rw-rw-rw-   0 root         (0) root         (0)    27763 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/syncasync.py
+-rw-rw-rw-   0 root         (0) root         (0)      674 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:05:40.977075 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    37863 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/branch.py
+-rw-rw-rw-   0 root         (0) root         (0)    14087 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/cicd.py
+-rw-rw-rw-   0 root         (0) root         (0)    64836 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    78344 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    11484 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    28107 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31944 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/datasource.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2964 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/job.py
+-rw-rw-rw-   0 root         (0) root         (0)    26168 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/pipe.py
+-rw-rw-rw-   0 root         (0) root         (0)     2010 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/regions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10490 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/telemetry.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:05:40.977075 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/tinyunit/
+-rw-rw-rw-   0 root         (0) root         (0)    11667 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/tinyunit/tinyunit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/token.py
+-rw-rw-rw-   0 root         (0) root         (0)    10081 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/workspace.py
+-rw-rw-rw-   0 root         (0) root         (0)     8268 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/workspace_members.py
+-rw-rw-rw-   0 root         (0) root         (0)    41982 2024-03-28 15:05:32.000000 tinybird-cli-3.6.1.dev9/tinybird/tornado_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 15:05:40.977075 tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    67926 2024-03-28 15:05:40.000000 tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1419 2024-03-28 15:05:40.000000 tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 15:05:40.000000 tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-03-28 15:05:40.000000 tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      732 2024-03-28 15:05:40.000000 tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-03-28 15:05:40.000000 tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/top_level.txt
```

### Comparing `tinybird-cli-3.6.1.dev8/PKG-INFO` & `tinybird-cli-3.6.1.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.6.1.dev8
+Version: 3.6.1.dev9
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -15,14 +15,20 @@
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 
 ---------
 
+3.6.1.dev9
+************
+
+- `Fixed` Added correct URL for checking available regions
+
+
 3.6.1.dev8
 ************
 
 - `Fixed` Report better error message on `tb diff` when two Datafiles have the same name
 
 3.6.1.dev7
 ************
```

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/ch_utils/constants.py` & `tinybird-cli-3.6.1.dev9/tinybird/ch_utils/constants.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/ch_utils/engine.py` & `tinybird-cli-3.6.1.dev9/tinybird/ch_utils/engine.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/check_pypi.py` & `tinybird-cli-3.6.1.dev9/tinybird/check_pypi.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/client.py` & `tinybird-cli-3.6.1.dev9/tinybird/client.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/config.py` & `tinybird-cli-3.6.1.dev9/tinybird/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/connector_settings.py` & `tinybird-cli-3.6.1.dev9/tinybird/connector_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/connectors.py` & `tinybird-cli-3.6.1.dev9/tinybird/connectors.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/context.py` & `tinybird-cli-3.6.1.dev9/tinybird/context.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/data_connectors/credentials.py` & `tinybird-cli-3.6.1.dev9/tinybird/data_connectors/credentials.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/datafile.py` & `tinybird-cli-3.6.1.dev9/tinybird/datafile.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/datatypes.py` & `tinybird-cli-3.6.1.dev9/tinybird/datatypes.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/feedback_manager.py` & `tinybird-cli-3.6.1.dev9/tinybird/feedback_manager.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/git_settings.py` & `tinybird-cli-3.6.1.dev9/tinybird/git_settings.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/sql.py` & `tinybird-cli-3.6.1.dev9/tinybird/sql.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/sql_template.py` & `tinybird-cli-3.6.1.dev9/tinybird/sql_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/sql_template_fmt.py` & `tinybird-cli-3.6.1.dev9/tinybird/sql_template_fmt.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/sql_toolset.py` & `tinybird-cli-3.6.1.dev9/tinybird/sql_toolset.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/syncasync.py` & `tinybird-cli-3.6.1.dev9/tinybird/syncasync.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/auth.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from tinybird.tb_cli_modules.regions import Region
 
 
 @cli.group(invoke_without_command=True)
 @click.option("--token", help="Use auth token, defaults to TB_TOKEN envvar, then to the .tinyb file")
 @click.option(
     "--host",
-    help="Set custom host if it's different than https://api.tinybird.co. Check https://docs.tinybird.co/cli.html for the available list of regions",
+    help="Set custom host if it's different than https://api.tinybird.co. Check https://www.tinybird.co/docs/api-reference/overview#regions-and-endpoints for the available list of regions",
 )
 @click.option("--region", envvar="TB_REGION", help="Set region. Run 'tb auth ls' to show available regions")
 @click.option(
     "--connector",
     type=click.Choice(["bigquery", "snowflake"], case_sensitive=True),
     help="Set credentials for one of the supported connectors",
 )
```

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/branch.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/branch.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/cicd.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/cicd.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/cli.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/cli.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/common.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/common.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/config.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/config.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/connection.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/connection.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/datasource.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/datasource.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/exceptions.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/job.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/job.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/pipe.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/pipe.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/regions.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/regions.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/telemetry.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/telemetry.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/test.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/test.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/tinyunit/tinyunit.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/tinyunit/tinyunit.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/tinyunit/tinyunit_lib.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/token.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/token.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/workspace.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/workspace.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tb_cli_modules/workspace_members.py` & `tinybird-cli-3.6.1.dev9/tinybird/tb_cli_modules/workspace_members.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird/tornado_template.py` & `tinybird-cli-3.6.1.dev9/tinybird/tornado_template.py`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/PKG-INFO` & `tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinybird-cli
-Version: 3.6.1.dev8
+Version: 3.6.1.dev9
 Summary: Tinybird Command Line Tool
 Home-page: https://www.tinybird.co/docs/cli/introduction.html
 Author: Tinybird
 Author-email: support@tinybird.co
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: bigquery
@@ -15,14 +15,20 @@
 
 The Tinybird command-line tool allows you to use all the Tinybird functionality directly from the command line. Additionally, it includes several functions to create and manage data projects easily.
 
 Changelog
 
 ---------
 
+3.6.1.dev9
+************
+
+- `Fixed` Added correct URL for checking available regions
+
+
 3.6.1.dev8
 ************
 
 - `Fixed` Report better error message on `tb diff` when two Datafiles have the same name
 
 3.6.1.dev7
 ************
```

### Comparing `tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/SOURCES.txt` & `tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tinybird-cli-3.6.1.dev8/tinybird_cli.egg-info/requires.txt` & `tinybird-cli-3.6.1.dev9/tinybird_cli.egg-info/requires.txt`

 * *Files identical despite different names*

