# Comparing `tmp/hcs-core-0.1.223.tar.gz` & `tmp/hcs-core-0.1.224.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcs-core-0.1.223.tar", last modified: Tue Mar 26 16:37:51 2024, max compression
+gzip compressed data, was "hcs-core-0.1.224.tar", last modified: Tue Apr  2 21:19:33 2024, max compression
```

## Comparing `hcs-core-0.1.223.tar` & `hcs-core-0.1.224.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.654057 hcs-core-0.1.223/
--rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-03-26 16:37:51.653134 hcs-core-0.1.223/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)       25 2023-12-28 17:19:26.000000 hcs-core-0.1.223/README.md
--rw-r--r--   0 nanw       (501) staff       (20)        7 2024-03-26 16:37:47.000000 hcs-core-0.1.223/VERSION
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.584763 hcs-core-0.1.223/hcs_core/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.608373 hcs-core-0.1.223/hcs_core/ctxp/
--rw-r--r--   0 nanw       (501) staff       (20)      790 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/_init.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.613458 hcs-core-0.1.223/hcs_core/ctxp/built_in_cmds/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/built_in_cmds/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     3086 2024-03-05 02:25:06.000000 hcs-core-0.1.223/hcs_core/ctxp/built_in_cmds/_ut.py
--rw-r--r--   0 nanw       (501) staff       (20)     2387 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/built_in_cmds/context.py
--rw-r--r--   0 nanw       (501) staff       (20)     4034 2024-02-28 02:33:27.000000 hcs-core-0.1.223/hcs_core/ctxp/built_in_cmds/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     2274 2024-03-08 00:26:01.000000 hcs-core-0.1.223/hcs_core/ctxp/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     5791 2024-02-28 02:35:31.000000 hcs-core-0.1.223/hcs_core/ctxp/cli_processor.py
--rw-r--r--   0 nanw       (501) staff       (20)      936 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/config.py
--rw-r--r--   0 nanw       (501) staff       (20)     1160 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    14088 2024-03-19 14:27:19.000000 hcs-core-0.1.223/hcs_core/ctxp/data_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2856 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)     1623 2024-03-08 00:26:01.000000 hcs-core-0.1.223/hcs_core/ctxp/extension.py
--rw-r--r--   0 nanw       (501) staff       (20)     6432 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/fstore.py
--rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/init.py
--rw-r--r--   0 nanw       (501) staff       (20)     3792 2024-03-08 00:26:01.000000 hcs-core-0.1.223/hcs_core/ctxp/jsondot.py
--rw-r--r--   0 nanw       (501) staff       (20)     6342 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/logger.py
--rw-r--r--   0 nanw       (501) staff       (20)     6518 2024-03-05 02:25:06.000000 hcs-core-0.1.223/hcs_core/ctxp/profile.py
--rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/profile_store.py
--rw-r--r--   0 nanw       (501) staff       (20)     1767 2024-02-23 06:13:37.000000 hcs-core-0.1.223/hcs_core/ctxp/recent.py
--rw-r--r--   0 nanw       (501) staff       (20)     1597 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/ctxp/state.py
--rw-r--r--   0 nanw       (501) staff       (20)     7933 2024-03-26 16:37:21.000000 hcs-core-0.1.223/hcs_core/ctxp/util.py
--rw-r--r--   0 nanw       (501) staff       (20)     3245 2024-02-28 02:35:31.000000 hcs-core-0.1.223/hcs_core/ctxp/var_template.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.622932 hcs-core-0.1.223/hcs_core/plan/
--rw-r--r--   0 nanw       (501) staff       (20)      203 2024-03-15 15:37:00.000000 hcs-core-0.1.223/hcs_core/plan/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)      125 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/plan/actions.py
--rw-r--r--   0 nanw       (501) staff       (20)     1298 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/plan/base_provider.py
--rw-r--r--   0 nanw       (501) staff       (20)      116 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/plan/context.py
--rw-r--r--   0 nanw       (501) staff       (20)    20914 2024-03-15 15:37:00.000000 hcs-core-0.1.223/hcs_core/plan/core.py
--rw-r--r--   0 nanw       (501) staff       (20)    12918 2024-03-26 16:37:21.000000 hcs-core-0.1.223/hcs_core/plan/dag.py
--rw-r--r--   0 nanw       (501) staff       (20)     7784 2024-02-23 06:13:37.000000 hcs-core-0.1.223/hcs_core/plan/helper.py
--rw-r--r--   0 nanw       (501) staff       (20)     5363 2024-03-26 16:37:21.000000 hcs-core-0.1.223/hcs_core/plan/kop.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.625478 hcs-core-0.1.223/hcs_core/plan/provider/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/plan/provider/__init__.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.630118 hcs-core-0.1.223/hcs_core/plan/provider/dev/
--rw-r--r--   0 nanw       (501) staff       (20)       30 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/plan/provider/dev/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)       34 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/plan/provider/dev/_prepare.py
--rw-r--r--   0 nanw       (501) staff       (20)     1994 2024-03-26 16:37:21.000000 hcs-core-0.1.223/hcs_core/plan/provider/dev/dummy.py
--rw-r--r--   0 nanw       (501) staff       (20)     1104 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/plan/provider/dev/fibonacci.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.640454 hcs-core-0.1.223/hcs_core/sglib/
--rw-r--r--   0 nanw       (501) staff       (20)      654 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/sglib/__init__.py
--rw-r--r--   0 nanw       (501) staff       (20)     5194 2024-02-14 19:34:51.000000 hcs-core-0.1.223/hcs_core/sglib/auth.py
--rw-r--r--   0 nanw       (501) staff       (20)     1790 2024-02-14 19:34:51.000000 hcs-core-0.1.223/hcs_core/sglib/cli_options.py
--rw-r--r--   0 nanw       (501) staff       (20)     8332 2024-03-26 16:37:21.000000 hcs-core-0.1.223/hcs_core/sglib/client_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     8043 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/sglib/csp.py
--rw-r--r--   0 nanw       (501) staff       (20)     5167 2024-02-23 06:13:37.000000 hcs-core-0.1.223/hcs_core/sglib/ez_client.py
--rw-r--r--   0 nanw       (501) staff       (20)      901 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/sglib/hcs_client.py
--rw-r--r--   0 nanw       (501) staff       (20)    10056 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/sglib/login_support.py
--rw-r--r--   0 nanw       (501) staff       (20)      684 2024-02-08 22:31:51.000000 hcs-core-0.1.223/hcs_core/sglib/payload_util.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.650949 hcs-core-0.1.223/hcs_core/util/
--rw-r--r--   0 nanw       (501) staff       (20)        0 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/util/__init__.py
--rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/util/check_license.py
--rw-r--r--   0 nanw       (501) staff       (20)     3482 2024-03-05 02:25:06.000000 hcs-core-0.1.223/hcs_core/util/duration.py
--rw-r--r--   0 nanw       (501) staff       (20)      838 2024-03-26 16:37:21.000000 hcs-core-0.1.223/hcs_core/util/exit.py
--rw-r--r--   0 nanw       (501) staff       (20)     1755 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/util/hcs_constants.py
--rw-r--r--   0 nanw       (501) staff       (20)     8438 2024-03-07 07:01:47.000000 hcs-core-0.1.223/hcs_core/util/job_view.py
--rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/util/pki_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1946 2024-02-23 06:13:37.000000 hcs-core-0.1.223/hcs_core/util/query_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     2958 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/util/scheduler.py
--rw-r--r--   0 nanw       (501) staff       (20)     1239 2024-03-15 19:16:39.000000 hcs-core-0.1.223/hcs_core/util/ssl_util.py
--rw-r--r--   0 nanw       (501) staff       (20)     1727 2023-11-28 18:47:04.000000 hcs-core-0.1.223/hcs_core/util/versions.py
-drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-03-26 16:37:51.652062 hcs-core-0.1.223/hcs_core.egg-info/
--rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-03-26 16:37:51.000000 hcs-core-0.1.223/hcs_core.egg-info/PKG-INFO
--rw-r--r--   0 nanw       (501) staff       (20)     1810 2024-03-26 16:37:51.000000 hcs-core-0.1.223/hcs_core.egg-info/SOURCES.txt
--rw-r--r--   0 nanw       (501) staff       (20)        1 2024-03-26 16:37:51.000000 hcs-core-0.1.223/hcs_core.egg-info/dependency_links.txt
--rw-r--r--   0 nanw       (501) staff       (20)      265 2024-03-26 16:37:51.000000 hcs-core-0.1.223/hcs_core.egg-info/requires.txt
--rw-r--r--   0 nanw       (501) staff       (20)        9 2024-03-26 16:37:51.000000 hcs-core-0.1.223/hcs_core.egg-info/top_level.txt
--rw-r--r--   0 nanw       (501) staff       (20)     1250 2023-12-28 17:19:26.000000 hcs-core-0.1.223/pyproject.toml
--rw-r--r--   0 nanw       (501) staff       (20)      265 2023-11-28 18:47:04.000000 hcs-core-0.1.223/requirements.txt
--rw-r--r--   0 nanw       (501) staff       (20)       38 2024-03-26 16:37:51.654382 hcs-core-0.1.223/setup.cfg
--rw-r--r--   0 nanw       (501) staff       (20)      808 2023-12-28 17:19:26.000000 hcs-core-0.1.223/setup.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.514640 hcs-core-0.1.224/
+-rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-04-02 21:19:33.513996 hcs-core-0.1.224/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)       25 2023-12-28 17:19:26.000000 hcs-core-0.1.224/README.md
+-rw-r--r--   0 nanw       (501) staff       (20)        7 2024-04-02 21:19:29.000000 hcs-core-0.1.224/VERSION
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.411988 hcs-core-0.1.224/hcs_core/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.437372 hcs-core-0.1.224/hcs_core/ctxp/
+-rw-r--r--   0 nanw       (501) staff       (20)      790 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1155 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/_init.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.440425 hcs-core-0.1.224/hcs_core/ctxp/built_in_cmds/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/built_in_cmds/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3086 2024-03-05 02:25:06.000000 hcs-core-0.1.224/hcs_core/ctxp/built_in_cmds/_ut.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2387 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/built_in_cmds/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)     4034 2024-02-28 02:33:27.000000 hcs-core-0.1.224/hcs_core/ctxp/built_in_cmds/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2274 2024-03-08 00:26:01.000000 hcs-core-0.1.224/hcs_core/ctxp/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5791 2024-02-28 02:35:31.000000 hcs-core-0.1.224/hcs_core/ctxp/cli_processor.py
+-rw-r--r--   0 nanw       (501) staff       (20)      936 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/config.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1160 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    14088 2024-03-19 14:27:19.000000 hcs-core-0.1.224/hcs_core/ctxp/data_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2856 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1623 2024-03-08 00:26:01.000000 hcs-core-0.1.224/hcs_core/ctxp/extension.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6432 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/fstore.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1200 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/init.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3792 2024-03-08 00:26:01.000000 hcs-core-0.1.224/hcs_core/ctxp/jsondot.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6346 2024-04-02 21:19:29.000000 hcs-core-0.1.224/hcs_core/ctxp/logger.py
+-rw-r--r--   0 nanw       (501) staff       (20)     6518 2024-03-05 02:25:06.000000 hcs-core-0.1.224/hcs_core/ctxp/profile.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1565 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/profile_store.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1767 2024-02-23 06:13:37.000000 hcs-core-0.1.224/hcs_core/ctxp/recent.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1597 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/ctxp/state.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7933 2024-03-26 16:37:21.000000 hcs-core-0.1.224/hcs_core/ctxp/util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3245 2024-02-28 02:35:31.000000 hcs-core-0.1.224/hcs_core/ctxp/var_template.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.462398 hcs-core-0.1.224/hcs_core/plan/
+-rw-r--r--   0 nanw       (501) staff       (20)      203 2024-03-15 15:37:00.000000 hcs-core-0.1.224/hcs_core/plan/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)      125 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/plan/actions.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1298 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/plan/base_provider.py
+-rw-r--r--   0 nanw       (501) staff       (20)      116 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/plan/context.py
+-rw-r--r--   0 nanw       (501) staff       (20)    20914 2024-03-15 15:37:00.000000 hcs-core-0.1.224/hcs_core/plan/core.py
+-rw-r--r--   0 nanw       (501) staff       (20)    12918 2024-03-26 16:37:21.000000 hcs-core-0.1.224/hcs_core/plan/dag.py
+-rw-r--r--   0 nanw       (501) staff       (20)     7784 2024-02-23 06:13:37.000000 hcs-core-0.1.224/hcs_core/plan/helper.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5363 2024-03-26 16:37:21.000000 hcs-core-0.1.224/hcs_core/plan/kop.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.463301 hcs-core-0.1.224/hcs_core/plan/provider/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/plan/provider/__init__.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.479760 hcs-core-0.1.224/hcs_core/plan/provider/dev/
+-rw-r--r--   0 nanw       (501) staff       (20)       30 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/plan/provider/dev/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)       34 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/plan/provider/dev/_prepare.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1994 2024-03-26 16:37:21.000000 hcs-core-0.1.224/hcs_core/plan/provider/dev/dummy.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1104 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/plan/provider/dev/fibonacci.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.487276 hcs-core-0.1.224/hcs_core/sglib/
+-rw-r--r--   0 nanw       (501) staff       (20)      654 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/sglib/__init__.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5194 2024-02-14 19:34:51.000000 hcs-core-0.1.224/hcs_core/sglib/auth.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1790 2024-02-14 19:34:51.000000 hcs-core-0.1.224/hcs_core/sglib/cli_options.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8357 2024-04-02 21:19:29.000000 hcs-core-0.1.224/hcs_core/sglib/client_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8043 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/sglib/csp.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5167 2024-02-23 06:13:37.000000 hcs-core-0.1.224/hcs_core/sglib/ez_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)      901 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/sglib/hcs_client.py
+-rw-r--r--   0 nanw       (501) staff       (20)    10056 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/sglib/login_support.py
+-rw-r--r--   0 nanw       (501) staff       (20)      684 2024-02-08 22:31:51.000000 hcs-core-0.1.224/hcs_core/sglib/payload_util.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.511821 hcs-core-0.1.224/hcs_core/util/
+-rw-r--r--   0 nanw       (501) staff       (20)        0 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/util/__init__.py
+-rwxr-xr-x   0 nanw       (501) staff       (20)     2535 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/util/check_license.py
+-rw-r--r--   0 nanw       (501) staff       (20)     3482 2024-03-05 02:25:06.000000 hcs-core-0.1.224/hcs_core/util/duration.py
+-rw-r--r--   0 nanw       (501) staff       (20)      838 2024-03-26 16:37:21.000000 hcs-core-0.1.224/hcs_core/util/exit.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1755 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/util/hcs_constants.py
+-rw-r--r--   0 nanw       (501) staff       (20)     8438 2024-03-07 07:01:47.000000 hcs-core-0.1.224/hcs_core/util/job_view.py
+-rw-r--r--   0 nanw       (501) staff       (20)     5288 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/util/pki_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1946 2024-02-23 06:13:37.000000 hcs-core-0.1.224/hcs_core/util/query_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     2958 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/util/scheduler.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1239 2024-03-15 19:16:39.000000 hcs-core-0.1.224/hcs_core/util/ssl_util.py
+-rw-r--r--   0 nanw       (501) staff       (20)     1727 2023-11-28 18:47:04.000000 hcs-core-0.1.224/hcs_core/util/versions.py
+drwxr-xr-x   0 nanw       (501) staff       (20)        0 2024-04-02 21:19:33.512850 hcs-core-0.1.224/hcs_core.egg-info/
+-rw-r--r--   0 nanw       (501) staff       (20)     1371 2024-04-02 21:19:33.000000 hcs-core-0.1.224/hcs_core.egg-info/PKG-INFO
+-rw-r--r--   0 nanw       (501) staff       (20)     1810 2024-04-02 21:19:33.000000 hcs-core-0.1.224/hcs_core.egg-info/SOURCES.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        1 2024-04-02 21:19:33.000000 hcs-core-0.1.224/hcs_core.egg-info/dependency_links.txt
+-rw-r--r--   0 nanw       (501) staff       (20)      265 2024-04-02 21:19:33.000000 hcs-core-0.1.224/hcs_core.egg-info/requires.txt
+-rw-r--r--   0 nanw       (501) staff       (20)        9 2024-04-02 21:19:33.000000 hcs-core-0.1.224/hcs_core.egg-info/top_level.txt
+-rw-r--r--   0 nanw       (501) staff       (20)     1250 2023-12-28 17:19:26.000000 hcs-core-0.1.224/pyproject.toml
+-rw-r--r--   0 nanw       (501) staff       (20)      265 2023-11-28 18:47:04.000000 hcs-core-0.1.224/requirements.txt
+-rw-r--r--   0 nanw       (501) staff       (20)       38 2024-04-02 21:19:33.514752 hcs-core-0.1.224/setup.cfg
+-rw-r--r--   0 nanw       (501) staff       (20)      808 2023-12-28 17:19:26.000000 hcs-core-0.1.224/setup.py
```

### Comparing `hcs-core-0.1.223/PKG-INFO` & `hcs-core-0.1.224/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.223
+Version: 0.1.224
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/__init__.py` & `hcs-core-0.1.224/hcs_core/ctxp/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/_init.py` & `hcs-core-0.1.224/hcs_core/ctxp/_init.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/built_in_cmds/_ut.py` & `hcs-core-0.1.224/hcs_core/ctxp/built_in_cmds/_ut.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/built_in_cmds/context.py` & `hcs-core-0.1.224/hcs_core/ctxp/built_in_cmds/context.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/built_in_cmds/profile.py` & `hcs-core-0.1.224/hcs_core/ctxp/built_in_cmds/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/cli_options.py` & `hcs-core-0.1.224/hcs_core/ctxp/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/cli_processor.py` & `hcs-core-0.1.224/hcs_core/ctxp/cli_processor.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/config.py` & `hcs-core-0.1.224/hcs_core/ctxp/config.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/context.py` & `hcs-core-0.1.224/hcs_core/ctxp/context.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/data_util.py` & `hcs-core-0.1.224/hcs_core/ctxp/data_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/duration.py` & `hcs-core-0.1.224/hcs_core/ctxp/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/extension.py` & `hcs-core-0.1.224/hcs_core/ctxp/extension.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/fstore.py` & `hcs-core-0.1.224/hcs_core/ctxp/fstore.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/init.py` & `hcs-core-0.1.224/hcs_core/ctxp/init.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/jsondot.py` & `hcs-core-0.1.224/hcs_core/ctxp/jsondot.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/logger.py` & `hcs-core-0.1.224/hcs_core/ctxp/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,16 @@
 
 import os
 import re
 import logging
 import coloredlogs
 from logging.handlers import RotatingFileHandler
 
-LOG_FORMAT_SIMPLE = "%(levelname)-4s %(asctime)s %(name)-16s %(message)s"
-LOG_FORMAT_LONG = (
-    "%(color_on)s%(asctime)s [%(process)-5d:%(threadName)-12s] %(levelname)-7s [%(name)-16s] %(message)s%(color_off)s"
-)
+LOG_FORMAT_SIMPLE = "%(levelname).4s %(asctime)s %(name)-16s %(message)s"
+LOG_FORMAT_LONG = "%(color_on)s%(asctime)s.%(msecs)03d [%(process)-5d:%(threadName)-12s] %(levelname)-7s [%(name)-16s] %(message)s%(color_off)s"
 DATE_FORMAT_SIMPLE = "%H:%M:%S"
 
 
 def mask_password(msg: str) -> str:
     msg = re.sub(r"(\"password\"\s*:\s*\"?)(.*?)(\"?[\s*,? | \s*\}])", r"\1******\3", msg)
     return msg
```

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/profile.py` & `hcs-core-0.1.224/hcs_core/ctxp/profile.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/profile_store.py` & `hcs-core-0.1.224/hcs_core/ctxp/profile_store.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/recent.py` & `hcs-core-0.1.224/hcs_core/ctxp/recent.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/state.py` & `hcs-core-0.1.224/hcs_core/ctxp/state.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/util.py` & `hcs-core-0.1.224/hcs_core/ctxp/util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/ctxp/var_template.py` & `hcs-core-0.1.224/hcs_core/ctxp/var_template.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/plan/base_provider.py` & `hcs-core-0.1.224/hcs_core/plan/base_provider.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/plan/core.py` & `hcs-core-0.1.224/hcs_core/plan/core.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/plan/dag.py` & `hcs-core-0.1.224/hcs_core/plan/dag.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/plan/helper.py` & `hcs-core-0.1.224/hcs_core/plan/helper.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/plan/kop.py` & `hcs-core-0.1.224/hcs_core/plan/kop.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/plan/provider/dev/dummy.py` & `hcs-core-0.1.224/hcs_core/plan/provider/dev/dummy.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/plan/provider/dev/fibonacci.py` & `hcs-core-0.1.224/hcs_core/plan/provider/dev/fibonacci.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/sglib/__init__.py` & `hcs-core-0.1.224/hcs_core/sglib/__init__.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/sglib/auth.py` & `hcs-core-0.1.224/hcs_core/sglib/auth.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/sglib/cli_options.py` & `hcs-core-0.1.224/hcs_core/sglib/cli_options.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/sglib/client_util.py` & `hcs-core-0.1.224/hcs_core/sglib/client_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
     def list(self, org_id: str, **kwargs):
         if org_id:
             kwargs["org_id"] = org_id
 
         def _get_page(query_string):
             url = self._base_context + "?" + query_string
+            # print(url)
             return self._client.get(url)
 
         return PageRequest(_get_page, **kwargs).get()
 
     def create(self, payload: dict | str, headers: dict = None, **kwargs):
         url = with_query(f"{self._base_context}", **kwargs)
         # print(url)
```

### Comparing `hcs-core-0.1.223/hcs_core/sglib/csp.py` & `hcs-core-0.1.224/hcs_core/sglib/csp.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/sglib/ez_client.py` & `hcs-core-0.1.224/hcs_core/sglib/ez_client.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/sglib/hcs_client.py` & `hcs-core-0.1.224/hcs_core/sglib/hcs_client.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/sglib/login_support.py` & `hcs-core-0.1.224/hcs_core/sglib/login_support.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/sglib/payload_util.py` & `hcs-core-0.1.224/hcs_core/sglib/payload_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/check_license.py` & `hcs-core-0.1.224/hcs_core/util/check_license.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/duration.py` & `hcs-core-0.1.224/hcs_core/util/duration.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/exit.py` & `hcs-core-0.1.224/hcs_core/util/exit.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/hcs_constants.py` & `hcs-core-0.1.224/hcs_core/util/hcs_constants.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/job_view.py` & `hcs-core-0.1.224/hcs_core/util/job_view.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/pki_util.py` & `hcs-core-0.1.224/hcs_core/util/pki_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/query_util.py` & `hcs-core-0.1.224/hcs_core/util/query_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/scheduler.py` & `hcs-core-0.1.224/hcs_core/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/ssl_util.py` & `hcs-core-0.1.224/hcs_core/util/ssl_util.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core/util/versions.py` & `hcs-core-0.1.224/hcs_core/util/versions.py`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/hcs_core.egg-info/PKG-INFO` & `hcs-core-0.1.224/hcs_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcs-core
-Version: 0.1.223
+Version: 0.1.224
 Summary: Horizon Cloud Service CLI module.
 Author-email: Nanw1103 <nanw1103@gmail.com>
 Project-URL: Homepage, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: Bug Tracker, https://github.com/vmware/horizon-cloud-service-cli/issues
 Project-URL: documentation, https://readthedocs.org
 Project-URL: repository, https://github.com/vmware/horizon-cloud-service-cli
 Project-URL: changelog, https://github.com/vmware/horizon-cloud-service-cli/blob/main/CHANGELOG.md
```

### Comparing `hcs-core-0.1.223/hcs_core.egg-info/SOURCES.txt` & `hcs-core-0.1.224/hcs_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/pyproject.toml` & `hcs-core-0.1.224/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hcs-core-0.1.223/setup.py` & `hcs-core-0.1.224/setup.py`

 * *Files identical despite different names*

