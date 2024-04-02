# Comparing `tmp/squad-client-0.9.tar.gz` & `tmp/squad-client-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/squad-client-0.9.tar", last modified: Thu Oct 29 19:54:40 2020, max compression
+gzip compressed data, was "dist/squad-client-0.9.1.tar", last modified: Wed Nov 18 20:12:12 2020, max compression
```

## Comparing `squad-client-0.9.tar` & `squad-client-0.9.1.tar`

### file list

```diff
@@ -1,138 +1,141 @@
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      277 2020-10-29 19:54:40.000000 squad-client-0.9/PKG-INFO
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      102 2020-01-24 00:38:18.000000 squad-client-0.9/.coveragerc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      209 2020-04-09 13:23:00.000000 squad-client-0.9/.travis.yml
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client/
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client/core/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)    20551 2020-10-15 13:46:42.000000 squad-client-0.9/squad_client/core/models.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      598 2020-03-06 11:36:18.000000 squad-client-0.9/squad_client/core/command.py
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client/core/__pycache__/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1081 2020-03-06 11:37:17.000000 squad-client-0.9/squad_client/core/__pycache__/command.cpython-36.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)    14418 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/core/__pycache__/models.cpython-37.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)     2234 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/core/__pycache__/api.cpython-37.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     4377 2020-10-09 17:42:27.000000 squad-client-0.9/squad_client/core/__pycache__/api.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)    22050 2020-10-23 17:27:38.000000 squad-client-0.9/squad_client/core/__pycache__/models.cpython-36.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)     1043 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/core/__pycache__/command.cpython-37.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     4574 2020-10-09 17:29:40.000000 squad-client-0.9/squad_client/core/api.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       20 2020-10-29 19:52:30.000000 squad-client-0.9/squad_client/version.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      728 2020-10-09 17:29:40.000000 squad-client-0.9/squad_client/utils.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      194 2020-10-09 17:29:40.000000 squad-client-0.9/squad_client/exceptions.py
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client/commands/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     5295 2020-10-09 17:29:40.000000 squad-client-0.9/squad_client/commands/create_or_update_project.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      884 2020-04-09 13:23:00.000000 squad-client-0.9/squad_client/commands/test.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1714 2020-04-09 13:23:00.000000 squad-client-0.9/squad_client/commands/report.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1055 2020-04-09 13:23:00.000000 squad-client-0.9/squad_client/commands/shell.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      211 2020-04-08 12:25:25.000000 squad-client-0.9/squad_client/commands/__init__.py
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client/commands/__pycache__/
--rw-r--r--   0 chaws     (1000) chaws     (1000)     1204 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/commands/__pycache__/test.cpython-37.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1213 2020-04-09 13:54:36.000000 squad-client-0.9/squad_client/commands/__pycache__/test.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2060 2020-04-09 13:54:36.000000 squad-client-0.9/squad_client/commands/__pycache__/report.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1329 2020-04-09 13:54:36.000000 squad-client-0.9/squad_client/commands/__pycache__/shell.cpython-36.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)     1121 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/commands/__pycache__/shell.cpython-37.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     3111 2020-07-28 19:54:33.000000 squad-client-0.9/squad_client/commands/__pycache__/create_project.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      511 2020-04-08 12:37:15.000000 squad-client-0.9/squad_client/commands/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)     1993 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/commands/__pycache__/report.cpython-37.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)      470 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/commands/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     3801 2020-10-09 17:42:27.000000 squad-client-0.9/squad_client/commands/__pycache__/create_or_update_project.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     5372 2020-10-29 19:53:47.000000 squad-client-0.9/squad_client/commands/__pycache__/submit.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     7456 2020-10-29 19:51:48.000000 squad-client-0.9/squad_client/commands/submit.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     3575 2020-04-08 12:25:25.000000 squad-client-0.9/squad_client/report.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)        0 2020-01-14 19:11:04.000000 squad-client-0.9/squad_client/__init__.py
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client/__pycache__/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      248 2020-01-24 00:48:18.000000 squad-client-0.9/squad_client/__pycache__/settings.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2014 2020-10-09 17:42:26.000000 squad-client-0.9/squad_client/__pycache__/manage.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     3955 2020-04-08 12:37:15.000000 squad-client-0.9/squad_client/__pycache__/report.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      751 2020-10-09 17:42:27.000000 squad-client-0.9/squad_client/__pycache__/exceptions.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     3730 2020-10-23 17:27:38.000000 squad-client-0.9/squad_client/__pycache__/shortcuts.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1219 2020-10-09 17:42:27.000000 squad-client-0.9/squad_client/__pycache__/utils.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2268 2020-01-28 12:21:43.000000 squad-client-0.9/squad_client/__pycache__/api.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      150 2020-01-24 00:47:27.000000 squad-client-0.9/squad_client/__pycache__/__init__.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)    13743 2020-01-28 13:21:24.000000 squad-client-0.9/squad_client/__pycache__/models.cpython-36.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)     3921 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/__pycache__/report.cpython-37.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)      116 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      168 2020-10-29 19:52:30.000000 squad-client-0.9/squad_client/__pycache__/version.cpython-36.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)      214 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/__pycache__/settings.cpython-37.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)      575 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/__pycache__/exceptions.cpython-37.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)      918 2020-03-05 23:28:24.000000 squad-client-0.9/squad_client/__pycache__/utils.cpython-37.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     5091 2020-10-23 17:19:16.000000 squad-client-0.9/squad_client/shortcuts.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      280 2020-01-20 21:18:16.000000 squad-client-0.9/squad_client/settings.py
--rwxrwxr-x   0 chaws     (1000) chaws     (1000)     2007 2020-10-09 17:29:40.000000 squad-client-0.9/squad_client/manage.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       73 2020-10-09 17:29:40.000000 squad-client-0.9/.gitignore
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client.egg-info/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      277 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client.egg-info/PKG-INFO
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     4251 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client.egg-info/SOURCES.txt
--rw-rw-r--   0 chaws     (1000) chaws     (1000)        1 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client.egg-info/dependency_links.txt
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       46 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client.egg-info/requires.txt
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       13 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client.egg-info/top_level.txt
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       59 2020-10-29 19:54:40.000000 squad-client-0.9/squad_client.egg-info/entry_points.txt
--rw-rw-r--   0 chaws     (1000) chaws     (1000)    53248 2020-03-06 09:18:49.000000 squad-client-0.9/.coverage
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1233 2020-04-08 12:25:25.000000 squad-client-0.9/setup.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     4671 2020-10-29 19:53:47.000000 squad-client-0.9/CHANGELOG.md
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/tests/
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/tests/data/
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/tests/data/submit/
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/tests/data/submit/tuxbuild/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2888 2020-10-29 19:51:48.000000 squad-client-0.9/tests/data/submit/tuxbuild/malformed.json
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2889 2020-10-29 19:51:48.000000 squad-client-0.9/tests/data/submit/tuxbuild/build.json
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       55 2020-04-08 12:25:25.000000 squad-client-0.9/tests/squad_settings.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      285 2020-04-08 12:25:25.000000 squad-client-0.9/tests/test_code_quality.py
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/tests/submit_results/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       77 2020-10-29 19:51:48.000000 squad-client-0.9/tests/submit_results/sample_results.txt
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      117 2020-04-16 11:50:41.000000 squad-client-0.9/tests/submit_results/sample_results_malformed.json
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       77 2020-04-16 11:50:41.000000 squad-client-0.9/tests/submit_results/sample_results.yaml
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       22 2020-04-16 11:50:41.000000 squad-client-0.9/tests/submit_results/sample_metrics.json
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       73 2020-04-16 11:50:41.000000 squad-client-0.9/tests/submit_results/sample_results_malformed.yaml
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       99 2020-04-16 11:50:41.000000 squad-client-0.9/tests/submit_results/sample_metadata.json
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       11 2020-04-16 11:50:41.000000 squad-client-0.9/tests/submit_results/sample_log.log
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      117 2020-04-16 11:50:41.000000 squad-client-0.9/tests/submit_results/sample_results.json
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2581 2020-04-08 12:25:25.000000 squad-client-0.9/tests/test_report.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     9966 2020-10-09 18:24:25.000000 squad-client-0.9/tests/test_shortcuts.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)        0 2020-03-06 09:18:49.000000 squad-client-0.9/tests/test_docker.py
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/tests/commands/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     6266 2020-10-09 17:29:40.000000 squad-client-0.9/tests/commands/test_create_or_update_project.py
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/tests/commands/__pycache__/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     4692 2020-07-29 02:10:41.000000 squad-client-0.9/tests/commands/__pycache__/test_create_or_update_project.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      766 2020-10-29 19:51:48.000000 squad-client-0.9/tests/__init__.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2751 2020-10-29 19:51:48.000000 squad-client-0.9/tests/fixtures.py
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/tests/__pycache__/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      443 2020-04-08 12:37:15.000000 squad-client-0.9/tests/__pycache__/settings.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      663 2020-04-08 13:29:02.000000 squad-client-0.9/tests/__pycache__/test_code_quality.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      146 2020-03-06 09:59:37.000000 squad-client-0.9/tests/__pycache__/test_docker.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1708 2020-04-09 15:47:15.000000 squad-client-0.9/tests/__pycache__/test_api.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      340 2020-01-28 12:30:29.000000 squad-client-0.9/tests/__pycache__/test_utils.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2789 2020-04-08 13:29:02.000000 squad-client-0.9/tests/__pycache__/test_report.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1592 2020-03-19 20:23:58.000000 squad-client-0.9/tests/__pycache__/test_squad_admin.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      827 2020-10-29 19:53:47.000000 squad-client-0.9/tests/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 chaws     (1000) chaws     (1000)      413 2020-03-05 23:28:24.000000 squad-client-0.9/tests/__pycache__/__init__.cpython-37.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     7429 2020-10-09 18:24:35.000000 squad-client-0.9/tests/__pycache__/test_shortcuts.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     9212 2020-10-15 13:41:15.000000 squad-client-0.9/tests/__pycache__/test_models.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     5217 2020-04-08 12:37:15.000000 squad-client-0.9/tests/__pycache__/squad_service.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2639 2020-04-03 14:05:10.000000 squad-client-0.9/tests/__pycache__/test_squad_service.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     9374 2020-10-29 19:53:54.000000 squad-client-0.9/tests/__pycache__/test_submit.cpython-36.pyc
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     5038 2020-04-08 12:25:25.000000 squad-client-0.9/tests/squad_service.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     8865 2020-10-29 19:51:48.000000 squad-client-0.9/tests/test_submit.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      210 2020-03-06 09:18:49.000000 squad-client-0.9/tests/sample_script.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1068 2020-04-09 13:23:00.000000 squad-client-0.9/tests/test_api.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      318 2020-04-08 12:25:25.000000 squad-client-0.9/tests/settings.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       68 2020-01-28 12:30:02.000000 squad-client-0.9/tests/test_utils.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     6117 2020-10-15 13:26:59.000000 squad-client-0.9/tests/test_models.py
--rw-r--r--   0 chaws     (1000) chaws     (1000)   671744 2020-10-29 19:54:39.000000 squad-client-0.9/tests/squad.sqlite3
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      282 2020-02-18 08:05:20.000000 squad-client-0.9/COPYRIGHTS
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      158 2020-10-29 19:54:40.000000 squad-client-0.9/setup.cfg
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      371 2020-03-25 22:40:16.000000 squad-client-0.9/Dockerfile
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/scripts/
--rwxrwxr-x   0 chaws     (1000) chaws     (1000)     2053 2020-10-09 17:29:40.000000 squad-client-0.9/scripts/release
--rwxrwxr-x   0 chaws     (1000) chaws     (1000)      426 2020-10-09 17:29:40.000000 squad-client-0.9/scripts/upload
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      335 2020-04-16 12:52:59.000000 squad-client-0.9/MANIFEST.in
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     2503 2020-10-09 17:29:40.000000 squad-client-0.9/README.md
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       42 2020-10-09 17:29:40.000000 squad-client-0.9/requirements-dev.txt
--rwxrwxr-x   0 chaws     (1000) chaws     (1000)       90 2020-04-16 11:50:41.000000 squad-client-0.9/manage.py
-drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-10-29 19:54:40.000000 squad-client-0.9/examples/
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      787 2020-01-21 20:33:18.000000 squad-client-0.9/examples/example_template.html
--rwxrwxr-x   0 chaws     (1000) chaws     (1000)      652 2020-04-08 12:25:25.000000 squad-client-0.9/examples/example_report.py
--rwxrwxr-x   0 chaws     (1000) chaws     (1000)     3774 2020-10-09 17:29:40.000000 squad-client-0.9/examples/build_report.py
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       95 2020-03-06 09:18:49.000000 squad-client-0.9/examples/my_template.html.jinja2
--rw-rw-r--   0 chaws     (1000) chaws     (1000)      235 2020-03-06 09:18:49.000000 squad-client-0.9/examples/report.yml
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     7491 2020-10-09 17:29:40.000000 squad-client-0.9/examples/build_report_template.html
--rw-rw-r--   0 chaws     (1000) chaws     (1000)       46 2020-10-09 17:29:40.000000 squad-client-0.9/requirements.txt
--rw-rw-r--   0 chaws     (1000) chaws     (1000)     1073 2020-02-18 08:05:20.000000 squad-client-0.9/LICENSE
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      279 2020-11-18 20:12:11.000000 squad-client-0.9.1/PKG-INFO
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      102 2020-01-24 00:38:18.000000 squad-client-0.9.1/.coveragerc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      209 2020-04-09 13:23:00.000000 squad-client-0.9.1/.travis.yml
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client/
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client/core/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)    20551 2020-10-15 13:46:42.000000 squad-client-0.9.1/squad_client/core/models.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      598 2020-03-06 11:36:18.000000 squad-client-0.9.1/squad_client/core/command.py
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client/core/__pycache__/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1081 2020-03-06 11:37:17.000000 squad-client-0.9.1/squad_client/core/__pycache__/command.cpython-36.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)    14418 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/core/__pycache__/models.cpython-37.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)     2234 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/core/__pycache__/api.cpython-37.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     4377 2020-10-09 17:42:27.000000 squad-client-0.9.1/squad_client/core/__pycache__/api.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)    22050 2020-10-23 17:27:38.000000 squad-client-0.9.1/squad_client/core/__pycache__/models.cpython-36.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)     1043 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/core/__pycache__/command.cpython-37.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     4574 2020-10-09 17:29:40.000000 squad-client-0.9.1/squad_client/core/api.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       22 2020-11-18 20:08:49.000000 squad-client-0.9.1/squad_client/version.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      728 2020-10-09 17:29:40.000000 squad-client-0.9.1/squad_client/utils.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      194 2020-10-09 17:29:40.000000 squad-client-0.9.1/squad_client/exceptions.py
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client/commands/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     5295 2020-10-09 17:29:40.000000 squad-client-0.9.1/squad_client/commands/create_or_update_project.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      884 2020-04-09 13:23:00.000000 squad-client-0.9.1/squad_client/commands/test.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1714 2020-04-09 13:23:00.000000 squad-client-0.9.1/squad_client/commands/report.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1055 2020-04-09 13:23:00.000000 squad-client-0.9.1/squad_client/commands/shell.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      211 2020-04-08 12:25:25.000000 squad-client-0.9.1/squad_client/commands/__init__.py
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client/commands/__pycache__/
+-rw-r--r--   0 chaws     (1000) chaws     (1000)     1204 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/commands/__pycache__/test.cpython-37.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1213 2020-04-09 13:54:36.000000 squad-client-0.9.1/squad_client/commands/__pycache__/test.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2060 2020-04-09 13:54:36.000000 squad-client-0.9.1/squad_client/commands/__pycache__/report.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1329 2020-04-09 13:54:36.000000 squad-client-0.9.1/squad_client/commands/__pycache__/shell.cpython-36.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)     1121 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/commands/__pycache__/shell.cpython-37.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     3111 2020-07-28 19:54:33.000000 squad-client-0.9.1/squad_client/commands/__pycache__/create_project.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      511 2020-04-08 12:37:15.000000 squad-client-0.9.1/squad_client/commands/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)     1993 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/commands/__pycache__/report.cpython-37.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)      470 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/commands/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     3801 2020-10-09 17:42:27.000000 squad-client-0.9.1/squad_client/commands/__pycache__/create_or_update_project.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     5647 2020-11-18 20:11:11.000000 squad-client-0.9.1/squad_client/commands/__pycache__/submit.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     7782 2020-11-18 20:06:39.000000 squad-client-0.9.1/squad_client/commands/submit.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     3575 2020-04-08 12:25:25.000000 squad-client-0.9.1/squad_client/report.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)        0 2020-01-14 19:11:04.000000 squad-client-0.9.1/squad_client/__init__.py
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client/__pycache__/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      248 2020-01-24 00:48:18.000000 squad-client-0.9.1/squad_client/__pycache__/settings.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2014 2020-10-09 17:42:26.000000 squad-client-0.9.1/squad_client/__pycache__/manage.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     3955 2020-04-08 12:37:15.000000 squad-client-0.9.1/squad_client/__pycache__/report.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      751 2020-10-09 17:42:27.000000 squad-client-0.9.1/squad_client/__pycache__/exceptions.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     3730 2020-10-23 17:27:38.000000 squad-client-0.9.1/squad_client/__pycache__/shortcuts.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1219 2020-10-09 17:42:27.000000 squad-client-0.9.1/squad_client/__pycache__/utils.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2268 2020-01-28 12:21:43.000000 squad-client-0.9.1/squad_client/__pycache__/api.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      150 2020-01-24 00:47:27.000000 squad-client-0.9.1/squad_client/__pycache__/__init__.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)    13743 2020-01-28 13:21:24.000000 squad-client-0.9.1/squad_client/__pycache__/models.cpython-36.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)     3921 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/__pycache__/report.cpython-37.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)      116 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      170 2020-11-18 20:08:49.000000 squad-client-0.9.1/squad_client/__pycache__/version.cpython-36.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)      214 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/__pycache__/settings.cpython-37.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)      575 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/__pycache__/exceptions.cpython-37.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)      918 2020-03-05 23:28:24.000000 squad-client-0.9.1/squad_client/__pycache__/utils.cpython-37.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     5091 2020-10-23 17:19:16.000000 squad-client-0.9.1/squad_client/shortcuts.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      280 2020-01-20 21:18:16.000000 squad-client-0.9.1/squad_client/settings.py
+-rwxrwxr-x   0 chaws     (1000) chaws     (1000)     2007 2020-10-09 17:29:40.000000 squad-client-0.9.1/squad_client/manage.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       73 2020-10-09 17:29:40.000000 squad-client-0.9.1/.gitignore
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client.egg-info/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      279 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client.egg-info/PKG-INFO
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     4386 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)        1 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       46 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client.egg-info/requires.txt
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       13 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client.egg-info/top_level.txt
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       59 2020-11-18 20:12:11.000000 squad-client-0.9.1/squad_client.egg-info/entry_points.txt
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)    53248 2020-03-06 09:18:49.000000 squad-client-0.9.1/.coverage
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1233 2020-04-08 12:25:25.000000 squad-client-0.9.1/setup.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     4956 2020-11-18 20:11:00.000000 squad-client-0.9.1/CHANGELOG.md
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/tests/
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/tests/data/
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/tests/data/submit/
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/tests/data/submit/tuxbuild/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2888 2020-10-29 19:51:48.000000 squad-client-0.9.1/tests/data/submit/tuxbuild/malformed.json
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2889 2020-10-29 19:51:48.000000 squad-client-0.9.1/tests/data/submit/tuxbuild/build.json
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      776 2020-11-18 20:06:39.000000 squad-client-0.9.1/tests/data/submit/tuxbuild/empty_kconfig.json
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      744 2020-11-18 20:06:39.000000 squad-client-0.9.1/tests/data/submit/tuxbuild/missing_kconfig.json
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2419 2020-11-18 20:06:39.000000 squad-client-0.9.1/tests/data/submit/tuxbuild/buildset.json
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       55 2020-04-08 12:25:25.000000 squad-client-0.9.1/tests/squad_settings.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      285 2020-04-08 12:25:25.000000 squad-client-0.9.1/tests/test_code_quality.py
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/tests/submit_results/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       77 2020-10-29 19:51:48.000000 squad-client-0.9.1/tests/submit_results/sample_results.txt
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      117 2020-04-16 11:50:41.000000 squad-client-0.9.1/tests/submit_results/sample_results_malformed.json
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       77 2020-04-16 11:50:41.000000 squad-client-0.9.1/tests/submit_results/sample_results.yaml
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       22 2020-04-16 11:50:41.000000 squad-client-0.9.1/tests/submit_results/sample_metrics.json
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       73 2020-04-16 11:50:41.000000 squad-client-0.9.1/tests/submit_results/sample_results_malformed.yaml
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       99 2020-04-16 11:50:41.000000 squad-client-0.9.1/tests/submit_results/sample_metadata.json
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       11 2020-04-16 11:50:41.000000 squad-client-0.9.1/tests/submit_results/sample_log.log
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      117 2020-04-16 11:50:41.000000 squad-client-0.9.1/tests/submit_results/sample_results.json
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2581 2020-04-08 12:25:25.000000 squad-client-0.9.1/tests/test_report.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     9966 2020-10-09 18:24:25.000000 squad-client-0.9.1/tests/test_shortcuts.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)        0 2020-03-06 09:18:49.000000 squad-client-0.9.1/tests/test_docker.py
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/tests/commands/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     6266 2020-10-09 17:29:40.000000 squad-client-0.9.1/tests/commands/test_create_or_update_project.py
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/tests/commands/__pycache__/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     4692 2020-07-29 02:10:41.000000 squad-client-0.9.1/tests/commands/__pycache__/test_create_or_update_project.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      766 2020-10-29 19:51:48.000000 squad-client-0.9.1/tests/__init__.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2751 2020-10-29 19:51:48.000000 squad-client-0.9.1/tests/fixtures.py
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/tests/__pycache__/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      443 2020-04-08 12:37:15.000000 squad-client-0.9.1/tests/__pycache__/settings.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      663 2020-04-08 13:29:02.000000 squad-client-0.9.1/tests/__pycache__/test_code_quality.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      146 2020-03-06 09:59:37.000000 squad-client-0.9.1/tests/__pycache__/test_docker.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1708 2020-04-09 15:47:15.000000 squad-client-0.9.1/tests/__pycache__/test_api.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      340 2020-01-28 12:30:29.000000 squad-client-0.9.1/tests/__pycache__/test_utils.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2789 2020-04-08 13:29:02.000000 squad-client-0.9.1/tests/__pycache__/test_report.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1592 2020-03-19 20:23:58.000000 squad-client-0.9.1/tests/__pycache__/test_squad_admin.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      827 2020-10-29 19:53:47.000000 squad-client-0.9.1/tests/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 chaws     (1000) chaws     (1000)      413 2020-03-05 23:28:24.000000 squad-client-0.9.1/tests/__pycache__/__init__.cpython-37.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     7429 2020-10-09 18:24:35.000000 squad-client-0.9.1/tests/__pycache__/test_shortcuts.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     9212 2020-10-15 13:41:15.000000 squad-client-0.9.1/tests/__pycache__/test_models.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     5217 2020-04-08 12:37:15.000000 squad-client-0.9.1/tests/__pycache__/squad_service.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2639 2020-04-03 14:05:10.000000 squad-client-0.9.1/tests/__pycache__/test_squad_service.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)    10848 2020-11-18 20:11:18.000000 squad-client-0.9.1/tests/__pycache__/test_submit.cpython-36.pyc
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     5038 2020-04-08 12:25:25.000000 squad-client-0.9.1/tests/squad_service.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)    10276 2020-11-18 20:06:39.000000 squad-client-0.9.1/tests/test_submit.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      210 2020-03-06 09:18:49.000000 squad-client-0.9.1/tests/sample_script.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1068 2020-04-09 13:23:00.000000 squad-client-0.9.1/tests/test_api.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      318 2020-04-08 12:25:25.000000 squad-client-0.9.1/tests/settings.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       68 2020-01-28 12:30:02.000000 squad-client-0.9.1/tests/test_utils.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     6117 2020-10-15 13:26:59.000000 squad-client-0.9.1/tests/test_models.py
+-rw-r--r--   0 chaws     (1000) chaws     (1000)   671744 2020-11-18 20:12:11.000000 squad-client-0.9.1/tests/squad.sqlite3
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      282 2020-02-18 08:05:20.000000 squad-client-0.9.1/COPYRIGHTS
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      158 2020-11-18 20:12:11.000000 squad-client-0.9.1/setup.cfg
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      371 2020-03-25 22:40:16.000000 squad-client-0.9.1/Dockerfile
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/scripts/
+-rwxrwxr-x   0 chaws     (1000) chaws     (1000)     2053 2020-10-09 17:29:40.000000 squad-client-0.9.1/scripts/release
+-rwxrwxr-x   0 chaws     (1000) chaws     (1000)      426 2020-10-09 17:29:40.000000 squad-client-0.9.1/scripts/upload
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      335 2020-04-16 12:52:59.000000 squad-client-0.9.1/MANIFEST.in
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     2503 2020-10-09 17:29:40.000000 squad-client-0.9.1/README.md
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       42 2020-10-09 17:29:40.000000 squad-client-0.9.1/requirements-dev.txt
+-rwxrwxr-x   0 chaws     (1000) chaws     (1000)       90 2020-04-16 11:50:41.000000 squad-client-0.9.1/manage.py
+drwxrwxr-x   0 chaws     (1000) chaws     (1000)        0 2020-11-18 20:12:11.000000 squad-client-0.9.1/examples/
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      787 2020-01-21 20:33:18.000000 squad-client-0.9.1/examples/example_template.html
+-rwxrwxr-x   0 chaws     (1000) chaws     (1000)      652 2020-04-08 12:25:25.000000 squad-client-0.9.1/examples/example_report.py
+-rwxrwxr-x   0 chaws     (1000) chaws     (1000)     3774 2020-10-09 17:29:40.000000 squad-client-0.9.1/examples/build_report.py
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       95 2020-03-06 09:18:49.000000 squad-client-0.9.1/examples/my_template.html.jinja2
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)      235 2020-03-06 09:18:49.000000 squad-client-0.9.1/examples/report.yml
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     7491 2020-10-09 17:29:40.000000 squad-client-0.9.1/examples/build_report_template.html
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)       46 2020-10-09 17:29:40.000000 squad-client-0.9.1/requirements.txt
+-rw-rw-r--   0 chaws     (1000) chaws     (1000)     1073 2020-02-18 08:05:20.000000 squad-client-0.9.1/LICENSE
```

### Comparing `squad-client-0.9/squad_client/core/models.py` & `squad-client-0.9.1/squad_client/core/models.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/core/command.py` & `squad-client-0.9.1/squad_client/core/command.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/core/__pycache__/command.cpython-36.pyc` & `squad-client-0.9.1/squad_client/core/__pycache__/command.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/core/__pycache__/models.cpython-37.pyc` & `squad-client-0.9.1/squad_client/core/__pycache__/models.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/core/__pycache__/api.cpython-37.pyc` & `squad-client-0.9.1/squad_client/core/__pycache__/api.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/core/__pycache__/api.cpython-36.pyc` & `squad-client-0.9.1/squad_client/core/__pycache__/api.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/core/__pycache__/models.cpython-36.pyc` & `squad-client-0.9.1/squad_client/core/__pycache__/models.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/core/__pycache__/command.cpython-37.pyc` & `squad-client-0.9.1/squad_client/core/__pycache__/command.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/core/api.py` & `squad-client-0.9.1/squad_client/core/api.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/utils.py` & `squad-client-0.9.1/squad_client/utils.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/create_or_update_project.py` & `squad-client-0.9.1/squad_client/commands/create_or_update_project.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/test.py` & `squad-client-0.9.1/squad_client/commands/test.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/report.py` & `squad-client-0.9.1/squad_client/commands/report.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/shell.py` & `squad-client-0.9.1/squad_client/commands/shell.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/__pycache__/test.cpython-37.pyc` & `squad-client-0.9.1/squad_client/commands/__pycache__/test.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/__pycache__/test.cpython-36.pyc` & `squad-client-0.9.1/squad_client/commands/__pycache__/test.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/__pycache__/report.cpython-36.pyc` & `squad-client-0.9.1/squad_client/commands/__pycache__/report.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/__pycache__/shell.cpython-36.pyc` & `squad-client-0.9.1/squad_client/commands/__pycache__/shell.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/__pycache__/shell.cpython-37.pyc` & `squad-client-0.9.1/squad_client/commands/__pycache__/shell.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/__pycache__/create_project.cpython-36.pyc` & `squad-client-0.9.1/squad_client/commands/__pycache__/create_project.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/__pycache__/report.cpython-37.pyc` & `squad-client-0.9.1/squad_client/commands/__pycache__/report.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/__pycache__/create_or_update_project.cpython-36.pyc` & `squad-client-0.9.1/squad_client/commands/__pycache__/create_or_update_project.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/commands/__pycache__/submit.cpython-36.pyc` & `squad-client-0.9.1/squad_client/commands/__pycache__/submit.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 541d 9b5f 201d 0000 e300 0000  3...T.._ .......
+00000000: 330d 0d0a cf7e b55f 661e 0000 e300 0000  3....~._f.......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 5c00 0000 6400 6401 6c00 5a00 6400  .s\...d.d.l.Z.d.
 00000030: 6401 6c01 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6502 6a09 8300 5a0a 4700  m.Z...e.j...Z.G.
 00000070: 6404 6405 8400 6405 6508 8303 5a0b 6401  d.d...d.e...Z.d.
@@ -164,173 +164,190 @@
 00000a30: 6669 6c65 da01 6572 1800 0000 7218 0000  file..er....r...
 00000a40: 0072 1900 0000 5a11 5f5f 7265 6164 5f69  .r....Z.__read_i
 00000a50: 6e70 7574 5f66 696c 654e 0000 0073 1e00  nput_fileN...s..
 00000a60: 0000 0001 0a01 0402 1001 0801 0e01 0402  ................
 00000a70: 1401 1401 0401 0c01 0201 0c01 1001 2e02  ................
 00000a80: 7a1f 5375 626d 6974 436f 6d6d 616e 642e  z.SubmitCommand.
 00000a90: 5f5f 7265 6164 5f69 6e70 7574 5f66 696c  __read_input_fil
-00000aa0: 6563 0200 0000 0000 0000 0a00 0000 1100  ec..............
-00000ab0: 0000 4300 0000 73c2 0000 007c 006a 007c  ..C...s....|.j.|
+00000aa0: 6563 0200 0000 0000 0000 0c00 0000 1100  ec..............
+00000ab0: 0000 4300 0000 731c 0100 007c 006a 007c  ..C...s....|.j.|
 00000ac0: 0183 0173 0e64 0053 0064 007d 0279 4e74  ...s.d.S.d.}.yNt
 00000ad0: 017c 0183 018f 3c7d 0369 007d 0474 026a  .|....<}.i.}.t.j
 00000ae0: 037c 0383 017d 0578 227c 0544 005d 1a7d  .|...}.x"|.D.].}
 00000af0: 067c 006a 047c 0683 017d 077c 0664 0119  .|.j.|...}.|.d..
 00000b00: 007c 047c 073c 0071 3257 007c 047d 0257  .|.|.<.q2W.|.}.W
-00000b10: 0064 0051 0052 0058 0057 006e 5c04 0074  .d.Q.R.X.W.n\..t
-00000b20: 026a 056b 0a72 9001 007d 0801 007a 1274  .j.k.r...}...z.t
-00000b30: 066a 0764 027c 0883 0201 0057 0059 0064  .j.d.|.....W.Y.d
-00000b40: 0064 007d 087e 0858 006e 2e04 0074 086b  .d.}.~.X.n...t.k
-00000b50: 0a72 bc01 007d 0901 007a 1274 066a 0764  .r...}...z.t.j.d
-00000b60: 037c 0983 0201 0057 0059 0064 0064 007d  .|.....W.Y.d.d.}
-00000b70: 097e 0958 006e 0258 007c 0253 0029 044e  .~.X.n.X.|.S.).N
-00000b80: 5a0c 6275 696c 645f 7374 6174 7573 7a17  Z.build_statusz.
-00000b90: 4661 696c 6564 2074 6f20 6c6f 6164 206a  Failed to load j
-00000ba0: 736f 6e3a 2025 737a 1746 6169 6c65 6420  son: %sz.Failed 
-00000bb0: 746f 206f 7065 6e20 6669 6c65 3a20 2573  to open file: %s
-00000bc0: 2909 7226 0000 0072 2e00 0000 7228 0000  ).r&...r....r(..
-00000bd0: 0072 2900 0000 da17 5f67 6574 5f74 7578  .r)....._get_tux
-00000be0: 6275 696c 645f 7465 7374 5f6e 616d 6572  build_test_namer
-00000bf0: 2c00 0000 721d 0000 0072 1e00 0000 da07  ,...r....r......
-00000c00: 4f53 4572 726f 7229 0a72 1400 0000 721b  OSError).r....r.
-00000c10: 0000 00da 0464 6174 61da 0166 da02 7462  .....data..f..tb
-00000c20: da06 6275 696c 6473 da01 62da 046e 616d  ..builds..b..nam
-00000c30: 655a 036a 6465 5a03 6f73 6572 1800 0000  eZ.jdeZ.oser....
-00000c40: 7218 0000 0072 1900 0000 da13 5f6c 6f61  r....r......_loa
-00000c50: 645f 7475 7862 7569 6c64 5f6a 736f 6e62  d_tuxbuild_jsonb
-00000c60: 0000 0073 2000 0000 0001 0a01 0402 0401  ...s ...........
-00000c70: 0201 0a01 0401 0a02 0a01 0a01 1002 1202  ................
-00000c80: 1201 1c02 1001 1e02 7a21 5375 626d 6974  ........z!Submit
-00000c90: 436f 6d6d 616e 642e 5f6c 6f61 645f 7475  Command._load_tu
-00000ca0: 7862 7569 6c64 5f6a 736f 6e63 0200 0000  xbuild_jsonc....
-00000cb0: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
-00000cc0: 7352 0000 0064 017d 0274 006a 0174 026a  sR...d.}.t.j.t.j
-00000cd0: 037c 0164 0219 0064 0364 0085 0219 0083  .|.d...d.d......
-00000ce0: 016a 0483 0083 016a 0583 0064 0464 0585  .j.....j...d.d..
-00000cf0: 0219 007d 0364 067c 027c 0164 0719 007c  ...}.d.|.|.d...|
-00000d00: 0164 0819 007c 0164 0219 0064 0419 007c  .d...|.d...d...|
-00000d10: 0366 0516 0053 0029 094e da05 6275 696c  .f...S.).N..buil
-00000d20: 64da 076b 636f 6e66 6967 e901 0000 0072  d..kconfig.....r
-00000d30: 0100 0000 e908 0000 007a 0e25 732f 2573  .........z.%s/%s
-00000d40: 2d25 732d 2573 2d25 735a 0b74 6172 6765  -%s-%s-%sZ.targe
-00000d50: 745f 6172 6368 5a09 746f 6f6c 6368 6169  t_archZ.toolchai
-00000d60: 6e29 06da 0768 6173 686c 6962 da04 7368  n)...hashlib..sh
-00000d70: 6131 7228 0000 00da 0564 756d 7073 da06  a1r(.....dumps..
-00000d80: 656e 636f 6465 da09 6865 7864 6967 6573  encode..hexdiges
-00000d90: 7429 0472 1400 0000 723b 0000 00da 0573  t).r....r;.....s
-00000da0: 7569 7465 5a0c 6b63 6f6e 6669 675f 6861  uiteZ.kconfig_ha
-00000db0: 7368 7218 0000 0072 1800 0000 7219 0000  shr....r....r...
-00000dc0: 0072 3200 0000 7a00 0000 7308 0000 0000  .r2...z...s.....
-00000dd0: 0104 012c 0202 017a 2553 7562 6d69 7443  ...,...z%SubmitC
-00000de0: 6f6d 6d61 6e64 2e5f 6765 745f 7475 7862  ommand._get_tuxb
-00000df0: 7569 6c64 5f74 6573 745f 6e61 6d65 6302  uild_test_namec.
-00000e00: 0000 0000 0000 000a 0000 0010 0000 0043  ...............C
-00000e10: 0000 0073 7402 0000 6900 7d02 6900 7d03  ...st...i.}.i.}.
-00000e20: 6400 7d04 6400 7d05 7c01 6a00 7236 7c01  d.}.d.}.|.j.r6|.
-00000e30: 6a01 732a 7402 6a03 6401 8301 0100 6402  j.s*t.j.d.....d.
-00000e40: 5300 7c01 6a00 7c01 6a01 6901 7d02 7c01  S.|.j.|.j.i.}.|.
-00000e50: 6a04 726c 7c01 6a05 6403 6b02 7254 7c00  j.rl|.j.d.k.rT|.
-00000e60: 6a06 7c01 6a04 8301 7d02 6e0c 7c00 6a07  j.|.j...}.n.|.j.
-00000e70: 7c01 6a04 8301 7d02 7c02 6400 6b08 726c  |.j...}.|.d.k.rl
-00000e80: 6402 5300 7c01 6a08 728a 7c00 6a07 7c01  d.S.|.j.r.|.j.|.
-00000e90: 6a08 8301 7d03 7c03 6400 6b08 728a 6402  j...}.|.d.k.r.d.
-00000ea0: 5300 7c01 6a00 6400 6b08 72b6 7c01 6a04  S.|.j.d.k.r.|.j.
-00000eb0: 6400 6b08 72b6 7c01 6a08 6400 6b08 72b6  d.k.r.|.j.d.k.r.
-00000ec0: 7402 6a03 6404 8301 0100 6402 5300 7c01  t.j.d.....d.S.|.
-00000ed0: 6a09 72d4 7c00 6a07 7c01 6a09 8301 7d04  j.r.|.j.|.j...}.
-00000ee0: 7c04 6400 6b08 72d4 6402 5300 7c01 6a0a  |.d.k.r.d.S.|.j.
-00000ef0: 9001 720c 7c00 6a0b 7c01 6a0a 8301 73ec  ..r.|.j.|.j...s.
-00000f00: 6402 5300 740c 7c01 6a0a 6405 8302 8f0e  d.S.t.|.j.d.....
-00000f10: 7d06 7c06 6a0d 8300 7d05 5700 6400 5100  }.|.j...}.W.d.Q.
-00000f20: 5200 5800 7820 7c01 6a0e 4400 5d16 7d07  R.X.x |.j.D.].}.
-00000f30: 7c00 6a0b 7c07 8301 9001 7314 6402 5300  |.j.|.....s.d.S.
-00000f40: 9001 7114 5700 7c02 9001 728c 7856 740f  ..q.W.|...r.xVt.
-00000f50: 7c02 6a10 8300 8301 4400 5d46 5c02 7d08  |.j.....D.]F\.}.
-00000f60: 7d09 7411 7c08 8301 7412 6b09 9001 7266  }.t.|...t.k...rf
-00000f70: 7402 6a03 6406 8301 0100 6402 5300 7411  t.j.d.....d.S.t.
-00000f80: 7c09 8301 7412 7413 6702 6b07 9001 7242  |...t.t.g.k...rB
-00000f90: 7402 6a03 6407 8301 0100 6402 5300 9001  t.j.d.....d.S...
-00000fa0: 7142 5700 7c03 9001 72ec 7858 740f 7c03  qBW.|...r.xXt.|.
-00000fb0: 6a10 8300 8301 4400 5d48 5c02 7d08 7d09  j.....D.]H\.}.}.
-00000fc0: 7411 7c08 8301 7412 6b09 9001 72c4 7402  t.|...t.k...r.t.
-00000fd0: 6a03 6406 8301 0100 6402 5300 7411 7c09  j.d.....d.S.t.|.
-00000fe0: 8301 7414 7415 7416 6703 6b07 9001 72a0  ..t.t.t.g.k...r.
-00000ff0: 7402 6a03 6408 8301 0100 6402 5300 9001  t.j.d.....d.S...
-00001000: 71a0 5700 7c04 9002 724a 7856 740f 7c04  q.W.|...rJxVt.|.
-00001010: 6a10 8300 8301 4400 5d46 5c02 7d08 7d09  j.....D.]F\.}.}.
-00001020: 7411 7c08 8301 7412 6b09 9002 7224 7402  t.|...t.k...r$t.
-00001030: 6a03 6406 8301 0100 6402 5300 7411 7c09  j.d.....d.S.t.|.
-00001040: 8301 7412 7413 6702 6b07 9002 7200 7402  ..t.t.g.k...r.t.
-00001050: 6a03 6407 8301 0100 6402 5300 9002 7100  j.d.....d.S...q.
-00001060: 5700 7417 6409 7c01 6a18 7c01 6a19 6602  W.t.d.|.j.|.j.f.
-00001070: 1600 7c01 6a1a 7c01 6a1b 7c02 7c03 7c05  ..|.j.|.j.|.|.|.
-00001080: 7c04 640a 8d07 0100 640b 5300 290c 4e7a  |.d.....d.S.).Nz
-00001090: 1d54 6573 7420 7265 7375 6c74 2076 616c  .Test result val
-000010a0: 7565 2069 7320 7265 7175 6972 6564 4672  ue is requiredFr
-000010b0: 0b00 0000 7a3f 4174 206c 6561 7374 206f  ....z?At least o
-000010c0: 6e65 206f 6620 2d2d 7265 7375 6c74 2d6e  ne of --result-n
-000010d0: 616d 652c 202d 2d72 6573 756c 7473 2c20  ame, --results, 
-000010e0: 2d2d 6d65 7472 6963 7320 6973 2072 6571  --metrics is req
-000010f0: 7569 7265 6472 2500 0000 7a17 4e6f 6e2d  uiredr%...z.Non-
-00001100: 7374 7269 6e67 206b 6579 2064 6574 6563  string key detec
-00001110: 7465 647a 1d49 6e63 6f6d 7061 7469 626c  tedz.Incompatibl
-00001120: 6520 7265 7375 6c74 7320 6465 7465 6374  e results detect
-00001130: 6564 7a1d 496e 636f 6d70 6174 6962 6c65  edz.Incompatible
-00001140: 206d 6574 7269 6373 2064 6574 6563 7465   metrics detecte
-00001150: 647a 0525 732f 2573 2907 da12 6772 6f75  dz.%s/%s)...grou
-00001160: 705f 7072 6f6a 6563 745f 736c 7567 da0d  p_project_slug..
-00001170: 6275 696c 645f 7665 7273 696f 6eda 0865  build_version..e
-00001180: 6e76 5f73 6c75 67da 0574 6573 7473 da07  nv_slug..tests..
-00001190: 6d65 7472 6963 73da 036c 6f67 da08 6d65  metrics..log..me
-000011a0: 7461 6461 7461 5429 1c5a 0b72 6573 756c  tadataT).Z.resul
-000011b0: 745f 6e61 6d65 da0c 7265 7375 6c74 5f76  t_name..result_v
-000011c0: 616c 7565 721d 0000 0072 1e00 0000 da07  aluer....r......
-000011d0: 7265 7375 6c74 735a 0e72 6573 756c 7473  resultsZ.results
-000011e0: 5f6c 6179 6f75 7472 3a00 0000 da1f 5f53  _layoutr:....._S
-000011f0: 7562 6d69 7443 6f6d 6d61 6e64 5f5f 7265  ubmitCommand__re
-00001200: 6164 5f69 6e70 7574 5f66 696c 6572 4900  ad_input_filerI.
-00001210: 0000 724b 0000 00da 046c 6f67 7372 2600  ..rK.....logsr&.
-00001220: 0000 722e 0000 00da 0472 6561 64da 0b61  ..r......read..a
-00001230: 7474 6163 686d 656e 7473 da04 6974 6572  ttachments..iter
-00001240: da05 6974 656d 73da 0474 7970 65da 0373  ..items..type..s
-00001250: 7472 da04 6469 6374 da05 666c 6f61 74da  tr..dict..float.
-00001260: 0369 6e74 da04 6c69 7374 7202 0000 00da  .int..listr.....
-00001270: 0567 726f 7570 da07 7072 6f6a 6563 7472  .group..projectr
-00001280: 3b00 0000 da0b 656e 7669 726f 6e6d 656e  ;.....environmen
-00001290: 7429 0a72 1400 0000 da04 6172 6773 5a0c  t).r......argsZ.
-000012a0: 7265 7375 6c74 735f 6469 6374 da0c 6d65  results_dict..me
-000012b0: 7472 6963 735f 6469 6374 5a0d 6d65 7461  trics_dictZ.meta
-000012c0: 6461 7461 5f64 6963 745a 096c 6f67 735f  data_dictZ.logs_
-000012d0: 6669 6c65 5a10 6c6f 6773 5f66 696c 655f  fileZ.logs_file_
-000012e0: 736f 7572 6365 da08 6669 6c65 6e61 6d65  source..filename
-000012f0: da03 6b65 79da 0576 616c 7565 7218 0000  ..key..valuer...
-00001300: 0072 1800 0000 7219 0000 00da 0372 756e  .r....r......run
-00001310: 8200 0000 7388 0000 0000 0104 0104 0104  ....s...........
-00001320: 0104 0106 0106 010a 0104 010c 0206 010a  ................
-00001330: 010e 020c 0208 0104 0206 010c 0108 0104  ................
-00001340: 021e 0104 0106 0204 0206 010c 0108 0104  ................
-00001350: 0208 010c 0104 010e 0112 020c 010c 010a  ................
-00001360: 0206 0216 010e 010a 0104 0112 010a 010a  ................
-00001370: 0206 0216 010e 010a 0104 0114 010a 010a  ................
-00001380: 0206 0216 010e 010a 0104 0112 010a 010a  ................
-00001390: 0202 010e 0104 0104 0102 0102 0102 0108  ................
-000013a0: 037a 1153 7562 6d69 7443 6f6d 6d61 6e64  .z.SubmitCommand
-000013b0: 2e72 756e 290c da08 5f5f 6e61 6d65 5f5f  .run)...__name__
-000013c0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000013d0: 7175 616c 6e61 6d65 5f5f da07 636f 6d6d  qualname__..comm
-000013e0: 616e 64da 0968 656c 705f 7465 7874 7211  and..help_textr.
-000013f0: 0000 0072 2600 0000 724e 0000 0072 3a00  ...r&...rN...r:.
-00001400: 0000 7232 0000 0072 6200 0000 da0d 5f5f  ..r2...rb.....__
-00001410: 636c 6173 7363 656c 6c5f 5f72 1800 0000  classcell__r....
-00001420: 7218 0000 0029 0172 1700 0000 7219 0000  r....).r....r...
-00001430: 0072 0400 0000 0d00 0000 7310 0000 0008  .r........s.....
-00001440: 0104 0104 020c 3308 0a08 1408 1808 0872  ......3........r
-00001450: 0400 0000 290c 723f 0000 0072 2800 0000  ....).r?...r(...
-00001460: da07 6c6f 6767 696e 6772 1a00 0000 722a  ..loggingr....r*
-00001470: 0000 00da 1673 7175 6164 5f63 6c69 656e  .....squad_clien
-00001480: 742e 7368 6f72 7463 7574 7372 0200 0000  t.shortcutsr....
-00001490: da19 7371 7561 645f 636c 6965 6e74 2e63  ..squad_client.c
-000014a0: 6f72 652e 636f 6d6d 616e 6472 0300 0000  ore.commandr....
-000014b0: da09 6765 744c 6f67 6765 7272 1d00 0000  ..getLoggerr....
-000014c0: 7204 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
-000014d0: 1800 0000 7219 0000 00da 083c 6d6f 6475  ....r......<modu
-000014e0: 6c65 3e01 0000 0073 1000 0000 0801 0801  le>....s........
-000014f0: 0801 0801 0801 0c01 0c03 0803            ............
+00000b10: 0064 0051 0052 0058 0057 006e b604 0074  .d.Q.R.X.W.n...t
+00000b20: 056b 0a72 8e01 007d 0801 007a 1274 066a  .k.r...}...z.t.j
+00000b30: 0764 027c 0883 0201 0057 0059 0064 0064  .d.|.....W.Y.d.d
+00000b40: 007d 087e 0858 006e 8a04 0074 086b 0a72  .}.~.X.n...t.k.r
+00000b50: ba01 007d 0901 007a 1274 066a 0764 037c  ...}...z.t.j.d.|
+00000b60: 0983 0201 0057 0059 0064 0064 007d 097e  .....W.Y.d.d.}.~
+00000b70: 0958 006e 5e04 0074 026a 096b 0a72 e801  .X.n^..t.j.k.r..
+00000b80: 007d 0a01 007a 1274 066a 0764 047c 0a83  .}...z.t.j.d.|..
+00000b90: 0201 0057 0059 0064 0064 007d 0a7e 0a58  ...W.Y.d.d.}.~.X
+00000ba0: 006e 3004 0074 0a6b 0a90 0172 1601 007d  .n0..t.k...r...}
+00000bb0: 0b01 007a 1274 066a 0764 057c 0b83 0201  ...z.t.j.d.|....
+00000bc0: 0057 0059 0064 0064 007d 0b7e 0b58 006e  .W.Y.d.d.}.~.X.n
+00000bd0: 0258 007c 0253 0029 064e 5a0c 6275 696c  .X.|.S.).NZ.buil
+00000be0: 645f 7374 6174 7573 7a3f 4661 696c 6564  d_statusz?Failed
+00000bf0: 2074 6f20 6c6f 6164 2074 7578 6275 696c   to load tuxbuil
+00000c00: 6420 6a73 6f6e 2064 7565 2074 6f20 6120  d json due to a 
+00000c10: 6d69 7373 696e 6720 6b63 6f6e 6669 6720  missing kconfig 
+00000c20: 7661 6c75 653a 2025 737a 3a46 6169 6c65  value: %sz:Faile
+00000c30: 6420 746f 206c 6f61 6420 7475 7862 7569  d to load tuxbui
+00000c40: 6c64 206a 736f 6e20 6475 6520 746f 2061  ld json due to a
+00000c50: 206d 6973 7369 6e67 2076 6172 6961 626c   missing variabl
+00000c60: 653a 2025 737a 1746 6169 6c65 6420 746f  e: %sz.Failed to
+00000c70: 206c 6f61 6420 6a73 6f6e 3a20 2573 7a17   load json: %sz.
+00000c80: 4661 696c 6564 2074 6f20 6f70 656e 2066  Failed to open f
+00000c90: 696c 653a 2025 7329 0b72 2600 0000 722e  ile: %s).r&...r.
+00000ca0: 0000 0072 2800 0000 7229 0000 00da 175f  ...r(...r)....._
+00000cb0: 6765 745f 7475 7862 7569 6c64 5f74 6573  get_tuxbuild_tes
+00000cc0: 745f 6e61 6d65 da0a 496e 6465 7845 7272  t_name..IndexErr
+00000cd0: 6f72 721d 0000 0072 1e00 0000 da08 4b65  orr....r......Ke
+00000ce0: 7945 7272 6f72 722c 0000 00da 074f 5345  yErrorr,.....OSE
+00000cf0: 7272 6f72 290c 7214 0000 0072 1b00 0000  rror).r....r....
+00000d00: da04 6461 7461 da01 66da 0274 62da 0662  ..data..f..tb..b
+00000d10: 7569 6c64 73da 0162 da04 6e61 6d65 5a02  uilds..b..nameZ.
+00000d20: 6965 5a02 6b65 5a03 6a64 655a 036f 7365  ieZ.keZ.jdeZ.ose
+00000d30: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+00000d40: 135f 6c6f 6164 5f74 7578 6275 696c 645f  ._load_tuxbuild_
+00000d50: 6a73 6f6e 6200 0000 7328 0000 0000 010a  jsonb...s(......
+00000d60: 0104 0204 0102 010a 0104 010a 020a 010a  ................
+00000d70: 0110 0212 0210 011c 0210 011c 0212 011c  ................
+00000d80: 0212 011e 027a 2153 7562 6d69 7443 6f6d  .....z!SubmitCom
+00000d90: 6d61 6e64 2e5f 6c6f 6164 5f74 7578 6275  mand._load_tuxbu
+00000da0: 696c 645f 6a73 6f6e 6302 0000 0000 0000  ild_jsonc.......
+00000db0: 0004 0000 0007 0000 0043 0000 0073 7400  .........C...st.
+00000dc0: 0000 6401 7d02 7400 7c01 6402 1900 6403  ..d.}.t.|.d...d.
+00000dd0: 6400 8502 1900 8301 7256 6404 7c01 6402  d.......rVd.|.d.
+00000de0: 1900 6405 1900 7401 6a02 7403 6a04 7c01  ..d...t.j.t.j.|.
+00000df0: 6402 1900 6403 6400 8502 1900 8301 6a05  d...d.d.......j.
+00000e00: 8300 8301 6a06 8300 6405 6406 8502 1900  ....j...d.d.....
+00000e10: 6602 1600 7d03 6e0c 7c01 6402 1900 6405  f...}.n.|.d...d.
+00000e20: 1900 7d03 6407 7c02 7c01 6408 1900 7c03  ..}.d.|.|.d...|.
+00000e30: 6603 1600 5300 2909 4eda 0562 7569 6c64  f...S.).N..build
+00000e40: da07 6b63 6f6e 6669 67e9 0100 0000 7a05  ..kconfig.....z.
+00000e50: 2573 2d25 7372 0100 0000 e908 0000 007a  %s-%sr.........z
+00000e60: 0825 732f 2573 2d25 735a 0974 6f6f 6c63  .%s/%s-%sZ.toolc
+00000e70: 6861 696e 2907 da03 6c65 6eda 0768 6173  hain)...len..has
+00000e80: 686c 6962 da04 7368 6131 7228 0000 00da  hlib..sha1r(....
+00000e90: 0564 756d 7073 da06 656e 636f 6465 da09  .dumps..encode..
+00000ea0: 6865 7864 6967 6573 7429 0472 1400 0000  hexdigest).r....
+00000eb0: 723d 0000 00da 0573 7569 7465 723e 0000  r=.....suiter>..
+00000ec0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
+00000ed0: 7232 0000 0080 0000 0073 0c00 0000 0001  r2.......s......
+00000ee0: 0402 1401 3e02 0c02 0201 7a25 5375 626d  ....>.....z%Subm
+00000ef0: 6974 436f 6d6d 616e 642e 5f67 6574 5f74  itCommand._get_t
+00000f00: 7578 6275 696c 645f 7465 7374 5f6e 616d  uxbuild_test_nam
+00000f10: 6563 0200 0000 0000 0000 0a00 0000 1000  ec..............
+00000f20: 0000 4300 0000 7374 0200 0069 007d 0269  ..C...st...i.}.i
+00000f30: 007d 0364 007d 0464 007d 057c 016a 0072  .}.d.}.d.}.|.j.r
+00000f40: 367c 016a 0173 2a74 026a 0364 0183 0101  6|.j.s*t.j.d....
+00000f50: 0064 0253 007c 016a 007c 016a 0169 017d  .d.S.|.j.|.j.i.}
+00000f60: 027c 016a 0472 6c7c 016a 0564 036b 0272  .|.j.rl|.j.d.k.r
+00000f70: 547c 006a 067c 016a 0483 017d 026e 0c7c  T|.j.|.j...}.n.|
+00000f80: 006a 077c 016a 0483 017d 027c 0264 006b  .j.|.j...}.|.d.k
+00000f90: 0872 6c64 0253 007c 016a 0872 8a7c 006a  .rld.S.|.j.r.|.j
+00000fa0: 077c 016a 0883 017d 037c 0364 006b 0872  .|.j...}.|.d.k.r
+00000fb0: 8a64 0253 007c 016a 0064 006b 0872 b67c  .d.S.|.j.d.k.r.|
+00000fc0: 016a 0464 006b 0872 b67c 016a 0864 006b  .j.d.k.r.|.j.d.k
+00000fd0: 0872 b674 026a 0364 0483 0101 0064 0253  .r.t.j.d.....d.S
+00000fe0: 007c 016a 0972 d47c 006a 077c 016a 0983  .|.j.r.|.j.|.j..
+00000ff0: 017d 047c 0464 006b 0872 d464 0253 007c  .}.|.d.k.r.d.S.|
+00001000: 016a 0a90 0172 0c7c 006a 0b7c 016a 0a83  .j...r.|.j.|.j..
+00001010: 0173 ec64 0253 0074 0c7c 016a 0a64 0583  .s.d.S.t.|.j.d..
+00001020: 028f 0e7d 067c 066a 0d83 007d 0557 0064  ...}.|.j...}.W.d
+00001030: 0051 0052 0058 0078 207c 016a 0e44 005d  .Q.R.X.x |.j.D.]
+00001040: 167d 077c 006a 0b7c 0783 0190 0173 1464  .}.|.j.|.....s.d
+00001050: 0253 0090 0171 1457 007c 0290 0172 8c78  .S...q.W.|...r.x
+00001060: 5674 0f7c 026a 1083 0083 0144 005d 465c  Vt.|.j.....D.]F\
+00001070: 027d 087d 0974 117c 0883 0174 126b 0990  .}.}.t.|...t.k..
+00001080: 0172 6674 026a 0364 0683 0101 0064 0253  .rft.j.d.....d.S
+00001090: 0074 117c 0983 0174 1274 1367 026b 0790  .t.|...t.t.g.k..
+000010a0: 0172 4274 026a 0364 0783 0101 0064 0253  .rBt.j.d.....d.S
+000010b0: 0090 0171 4257 007c 0390 0172 ec78 5874  ...qBW.|...r.xXt
+000010c0: 0f7c 036a 1083 0083 0144 005d 485c 027d  .|.j.....D.]H\.}
+000010d0: 087d 0974 117c 0883 0174 126b 0990 0172  .}.t.|...t.k...r
+000010e0: c474 026a 0364 0683 0101 0064 0253 0074  .t.j.d.....d.S.t
+000010f0: 117c 0983 0174 1474 1574 1667 036b 0790  .|...t.t.t.g.k..
+00001100: 0172 a074 026a 0364 0883 0101 0064 0253  .r.t.j.d.....d.S
+00001110: 0090 0171 a057 007c 0490 0272 4a78 5674  ...q.W.|...rJxVt
+00001120: 0f7c 046a 1083 0083 0144 005d 465c 027d  .|.j.....D.]F\.}
+00001130: 087d 0974 117c 0883 0174 126b 0990 0272  .}.t.|...t.k...r
+00001140: 2474 026a 0364 0683 0101 0064 0253 0074  $t.j.d.....d.S.t
+00001150: 117c 0983 0174 1274 1367 026b 0790 0272  .|...t.t.g.k...r
+00001160: 0074 026a 0364 0783 0101 0064 0253 0090  .t.j.d.....d.S..
+00001170: 0271 0057 0074 1764 097c 016a 187c 016a  .q.W.t.d.|.j.|.j
+00001180: 1966 0216 007c 016a 1a7c 016a 1b7c 027c  .f...|.j.|.j.|.|
+00001190: 037c 057c 0464 0a8d 0701 0064 0b53 0029  .|.|.d.....d.S.)
+000011a0: 0c4e 7a1d 5465 7374 2072 6573 756c 7420  .Nz.Test result 
+000011b0: 7661 6c75 6520 6973 2072 6571 7569 7265  value is require
+000011c0: 6446 720b 0000 007a 3f41 7420 6c65 6173  dFr....z?At leas
+000011d0: 7420 6f6e 6520 6f66 202d 2d72 6573 756c  t one of --resul
+000011e0: 742d 6e61 6d65 2c20 2d2d 7265 7375 6c74  t-name, --result
+000011f0: 732c 202d 2d6d 6574 7269 6373 2069 7320  s, --metrics is 
+00001200: 7265 7175 6972 6564 7225 0000 007a 174e  requiredr%...z.N
+00001210: 6f6e 2d73 7472 696e 6720 6b65 7920 6465  on-string key de
+00001220: 7465 6374 6564 7a1d 496e 636f 6d70 6174  tectedz.Incompat
+00001230: 6962 6c65 2072 6573 756c 7473 2064 6574  ible results det
+00001240: 6563 7465 647a 1d49 6e63 6f6d 7061 7469  ectedz.Incompati
+00001250: 626c 6520 6d65 7472 6963 7320 6465 7465  ble metrics dete
+00001260: 6374 6564 7a05 2573 2f25 7329 07da 1267  ctedz.%s/%s)...g
+00001270: 726f 7570 5f70 726f 6a65 6374 5f73 6c75  roup_project_slu
+00001280: 67da 0d62 7569 6c64 5f76 6572 7369 6f6e  g..build_version
+00001290: da08 656e 765f 736c 7567 da05 7465 7374  ..env_slug..test
+000012a0: 73da 076d 6574 7269 6373 da03 6c6f 67da  s..metrics..log.
+000012b0: 086d 6574 6164 6174 6154 291c 5a0b 7265  .metadataT).Z.re
+000012c0: 7375 6c74 5f6e 616d 65da 0c72 6573 756c  sult_name..resul
+000012d0: 745f 7661 6c75 6572 1d00 0000 721e 0000  t_valuer....r...
+000012e0: 00da 0772 6573 756c 7473 5a0e 7265 7375  ...resultsZ.resu
+000012f0: 6c74 735f 6c61 796f 7574 723c 0000 00da  lts_layoutr<....
+00001300: 1f5f 5375 626d 6974 436f 6d6d 616e 645f  ._SubmitCommand_
+00001310: 5f72 6561 645f 696e 7075 745f 6669 6c65  _read_input_file
+00001320: 724c 0000 0072 4e00 0000 da04 6c6f 6773  rL...rN.....logs
+00001330: 7226 0000 0072 2e00 0000 da04 7265 6164  r&...r......read
+00001340: da0b 6174 7461 6368 6d65 6e74 73da 0469  ..attachments..i
+00001350: 7465 72da 0569 7465 6d73 da04 7479 7065  ter..items..type
+00001360: da03 7374 72da 0464 6963 74da 0566 6c6f  ..str..dict..flo
+00001370: 6174 da03 696e 74da 046c 6973 7472 0200  at..int..listr..
+00001380: 0000 da05 6772 6f75 70da 0770 726f 6a65  ....group..proje
+00001390: 6374 723d 0000 00da 0b65 6e76 6972 6f6e  ctr=.....environ
+000013a0: 6d65 6e74 290a 7214 0000 00da 0461 7267  ment).r......arg
+000013b0: 735a 0c72 6573 756c 7473 5f64 6963 74da  sZ.results_dict.
+000013c0: 0c6d 6574 7269 6373 5f64 6963 745a 0d6d  .metrics_dictZ.m
+000013d0: 6574 6164 6174 615f 6469 6374 5a09 6c6f  etadata_dictZ.lo
+000013e0: 6773 5f66 696c 655a 106c 6f67 735f 6669  gs_fileZ.logs_fi
+000013f0: 6c65 5f73 6f75 7263 65da 0866 696c 656e  le_source..filen
+00001400: 616d 65da 036b 6579 da05 7661 6c75 6572  ame..key..valuer
+00001410: 1800 0000 7218 0000 0072 1900 0000 da03  ....r....r......
+00001420: 7275 6e8c 0000 0073 8800 0000 0001 0401  run....s........
+00001430: 0401 0401 0401 0601 0601 0a01 0401 0c02  ................
+00001440: 0601 0a01 0e02 0c02 0801 0402 0601 0c01  ................
+00001450: 0801 0402 1e01 0401 0602 0402 0601 0c01  ................
+00001460: 0801 0402 0801 0c01 0401 0e01 1202 0c01  ................
+00001470: 0c01 0a02 0602 1601 0e01 0a01 0401 1201  ................
+00001480: 0a01 0a02 0602 1601 0e01 0a01 0401 1401  ................
+00001490: 0a01 0a02 0602 1601 0e01 0a01 0401 1201  ................
+000014a0: 0a01 0a02 0201 0e01 0401 0401 0201 0201  ................
+000014b0: 0201 0803 7a11 5375 626d 6974 436f 6d6d  ....z.SubmitComm
+000014c0: 616e 642e 7275 6e29 0cda 085f 5f6e 616d  and.run)...__nam
+000014d0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+000014e0: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0763  .__qualname__..c
+000014f0: 6f6d 6d61 6e64 da09 6865 6c70 5f74 6578  ommand..help_tex
+00001500: 7472 1100 0000 7226 0000 0072 5100 0000  tr....r&...rQ...
+00001510: 723c 0000 0072 3200 0000 7265 0000 00da  r<...r2...re....
+00001520: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7218  .__classcell__r.
+00001530: 0000 0072 1800 0000 2901 7217 0000 0072  ...r....).r....r
+00001540: 1900 0000 7204 0000 000d 0000 0073 1000  ....r........s..
+00001550: 0000 0801 0401 0402 0c33 080a 0814 081e  .........3......
+00001560: 080c 7204 0000 0029 0c72 4200 0000 7228  ..r....).rB...r(
+00001570: 0000 00da 076c 6f67 6769 6e67 721a 0000  .....loggingr...
+00001580: 0072 2a00 0000 da16 7371 7561 645f 636c  .r*.....squad_cl
+00001590: 6965 6e74 2e73 686f 7274 6375 7473 7202  ient.shortcutsr.
+000015a0: 0000 00da 1973 7175 6164 5f63 6c69 656e  .....squad_clien
+000015b0: 742e 636f 7265 2e63 6f6d 6d61 6e64 7203  t.core.commandr.
+000015c0: 0000 00da 0967 6574 4c6f 6767 6572 721d  .....getLoggerr.
+000015d0: 0000 0072 0400 0000 7218 0000 0072 1800  ...r....r....r..
+000015e0: 0000 7218 0000 0072 1900 0000 da08 3c6d  ..r....r......<m
+000015f0: 6f64 756c 653e 0100 0000 7310 0000 0008  odule>....s.....
+00001600: 0108 0108 0108 0108 010c 010c 0308 03    ...............
```

### Comparing `squad-client-0.9/squad_client/commands/submit.py` & `squad-client-0.9.1/squad_client/commands/submit.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,28 +107,38 @@
 
                 for b in builds:
                     name = self._get_tuxbuild_test_name(b)
                     tb[name] = b["build_status"]
 
                 data = tb
 
+        except IndexError as ie:
+            logger.error("Failed to load tuxbuild json due to a missing kconfig value: %s", ie)
+
+        except KeyError as ke:
+            logger.error("Failed to load tuxbuild json due to a missing variable: %s", ke)
+
         except json.JSONDecodeError as jde:
             logger.error("Failed to load json: %s", jde)
 
         except OSError as ose:
             logger.error("Failed to open file: %s", ose)
 
         return data
 
     def _get_tuxbuild_test_name(self, build):
         suite = "build"
-        kconfig_hash = hashlib.sha1(json.dumps(build["kconfig"][1:]).encode()).hexdigest()[0:8]
 
-        return "%s/%s-%s-%s-%s" % (
-            suite, build["target_arch"], build["toolchain"], build["kconfig"][0], kconfig_hash,
+        if len(build["kconfig"][1:]):
+            kconfig = "%s-%s" % (build["kconfig"][0], hashlib.sha1(json.dumps(build["kconfig"][1:]).encode()).hexdigest()[0:8])
+        else:
+            kconfig = build["kconfig"][0]
+
+        return "%s/%s-%s" % (
+            suite, build["toolchain"], kconfig,
         )
 
     def run(self, args):
         results_dict = {}
         metrics_dict = {}
         metadata_dict = None
         logs_file = None
```

### Comparing `squad-client-0.9/squad_client/report.py` & `squad-client-0.9.1/squad_client/report.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/manage.cpython-36.pyc` & `squad-client-0.9.1/squad_client/__pycache__/manage.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/report.cpython-36.pyc` & `squad-client-0.9.1/squad_client/__pycache__/report.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/exceptions.cpython-36.pyc` & `squad-client-0.9.1/squad_client/__pycache__/exceptions.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/shortcuts.cpython-36.pyc` & `squad-client-0.9.1/squad_client/__pycache__/shortcuts.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/utils.cpython-36.pyc` & `squad-client-0.9.1/squad_client/__pycache__/utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/api.cpython-36.pyc` & `squad-client-0.9.1/squad_client/__pycache__/api.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/models.cpython-36.pyc` & `squad-client-0.9.1/squad_client/__pycache__/models.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/report.cpython-37.pyc` & `squad-client-0.9.1/squad_client/__pycache__/report.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/exceptions.cpython-37.pyc` & `squad-client-0.9.1/squad_client/__pycache__/exceptions.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/__pycache__/utils.cpython-37.pyc` & `squad-client-0.9.1/squad_client/__pycache__/utils.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/shortcuts.py` & `squad-client-0.9.1/squad_client/shortcuts.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client/manage.py` & `squad-client-0.9.1/squad_client/manage.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/squad_client.egg-info/SOURCES.txt` & `squad-client-0.9.1/squad_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,18 @@
 tests/__pycache__/test_squad_admin.cpython-36.pyc
 tests/__pycache__/test_squad_service.cpython-36.pyc
 tests/__pycache__/test_submit.cpython-36.pyc
 tests/__pycache__/test_utils.cpython-36.pyc
 tests/commands/test_create_or_update_project.py
 tests/commands/__pycache__/test_create_or_update_project.cpython-36.pyc
 tests/data/submit/tuxbuild/build.json
+tests/data/submit/tuxbuild/buildset.json
+tests/data/submit/tuxbuild/empty_kconfig.json
 tests/data/submit/tuxbuild/malformed.json
+tests/data/submit/tuxbuild/missing_kconfig.json
 tests/submit_results/sample_log.log
 tests/submit_results/sample_metadata.json
 tests/submit_results/sample_metrics.json
 tests/submit_results/sample_results.json
 tests/submit_results/sample_results.txt
 tests/submit_results/sample_results.yaml
 tests/submit_results/sample_results_malformed.json
```

### Comparing `squad-client-0.9/.coverage` & `squad-client-0.9.1/.coverage`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/setup.py` & `squad-client-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/CHANGELOG.md` & `squad-client-0.9.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+# 0.9.1
+
+This 0.9.1 release fixes a small bug and changes tuxbuild submission
+slightly.
+
+Complete list of changes going in:
+
+* Remove the arch from the test name when using tuxbuild json
+* Gracefully handle some tuxbuild json config errors
+* Do not show the hash for an empty kconfig
+
 # 0.9
 
 This 0.9 release adds support for TuxBuild input for submitting test results
 to SQUAD.
 
 Complete list of changes going in:
```

### Comparing `squad-client-0.9/tests/data/submit/tuxbuild/malformed.json` & `squad-client-0.9.1/tests/data/submit/tuxbuild/malformed.json`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/data/submit/tuxbuild/build.json` & `squad-client-0.9.1/tests/data/submit/tuxbuild/build.json`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/test_report.py` & `squad-client-0.9.1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/test_shortcuts.py` & `squad-client-0.9.1/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/commands/test_create_or_update_project.py` & `squad-client-0.9.1/tests/commands/test_create_or_update_project.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/commands/__pycache__/test_create_or_update_project.cpython-36.pyc` & `squad-client-0.9.1/tests/commands/__pycache__/test_create_or_update_project.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__init__.py` & `squad-client-0.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/fixtures.py` & `squad-client-0.9.1/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/test_code_quality.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/test_code_quality.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/test_api.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/test_api.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/test_report.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/test_report.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/test_squad_admin.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/test_squad_admin.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/__init__.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/test_shortcuts.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/test_shortcuts.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/test_models.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/test_models.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/squad_service.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/squad_service.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/test_squad_service.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/test_squad_service.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/__pycache__/test_submit.cpython-36.pyc` & `squad-client-0.9.1/tests/__pycache__/test_submit.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a 541d 9b5f a122 0000 e300 0000  3...T.._."......
+00000000: 330d 0d0a cf7e b55f 2428 0000 e300 0000  3....~._$(......
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 9400 0000 6400 6401 6c00 5a00 6400  .s....d.d.l.Z.d.
 00000030: 6401 6c01 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6404 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6405 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000060: 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0f 5a0f 0100 6400 6406 6c10 6d11 5a11  m.Z...d.d.l.m.Z.
@@ -98,489 +98,581 @@
 00000610: 744e 2905 da08 5f5f 6e61 6d65 5f5f da0a  tN)...__name__..
 00000620: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000630: 616c 6e61 6d65 5f5f 721b 0000 0072 3b00  alname__r....r;.
 00000640: 0000 7219 0000 0072 1900 0000 7219 0000  ..r....r....r...
 00000650: 0072 1a00 0000 7211 0000 0010 0000 0073  .r....r........s
 00000660: 0400 0000 0802 0804 7211 0000 0063 0000  ........r....c..
 00000670: 0000 0000 0000 0000 0000 0900 0000 4000  ..............@.
-00000680: 0000 73a4 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
+00000680: 0000 73bc 0000 0065 005a 0164 005a 0264  ..s....e.Z.d.Z.d
 00000690: 0165 036a 0416 005a 0564 025a 0664 0364  .e.j...Z.d.Z.d.d
-000006a0: 0484 005a 0764 2664 0664 0784 015a 0864  ...Z.d&d.d...Z.d
+000006a0: 0484 005a 0764 2c64 0664 0784 015a 0864  ...Z.d,d.d...Z.d
 000006b0: 0864 0984 005a 0964 0a64 0b84 005a 0a64  .d...Z.d.d...Z.d
 000006c0: 0c64 0d84 005a 0b64 0e64 0f84 005a 0c64  .d...Z.d.d...Z.d
 000006d0: 1064 1184 005a 0d64 1264 1384 005a 0e64  .d...Z.d.d...Z.d
 000006e0: 1464 1584 005a 0f64 1664 1784 005a 1064  .d...Z.d.d...Z.d
 000006f0: 1864 1984 005a 1164 1a64 1b84 005a 1264  .d...Z.d.d...Z.d
 00000700: 1c64 1d84 005a 1364 1e64 1f84 005a 1464  .d...Z.d.d...Z.d
 00000710: 2064 2184 005a 1564 2264 2384 005a 1664   d!..Z.d"d#..Z.d
-00000720: 2464 2584 005a 1764 0553 0029 27da 1153  $d%..Z.d.S.)'..S
-00000730: 7562 6d69 7443 6f6d 6d61 6e64 5465 7374  ubmitCommandTest
-00000740: 7a13 6874 7470 3a2f 2f6c 6f63 616c 686f  z.http://localho
-00000750: 7374 3a25 7372 1200 0000 6301 0000 0000  st:%sr....c.....
-00000760: 0000 0001 0000 0004 0000 0043 0000 0073  ...........C...s
-00000770: 1e00 0000 7400 8300 7c00 5f01 7402 6a03  ....t...|._.t.j.
-00000780: 7c00 6a04 7c00 6a05 6401 8d02 0100 6400  |.j.|.j.d.....d.
-00000790: 5300 2902 4e29 0272 1300 0000 7214 0000  S.).N).r....r...
-000007a0: 0029 0672 0500 0000 7215 0000 0072 0400  .).r....r....r..
-000007b0: 0000 7216 0000 00da 0e74 6573 7469 6e67  ..r......testing
-000007c0: 5f73 6572 7665 72da 0d74 6573 7469 6e67  _server..testing
-000007d0: 5f74 6f6b 656e 2901 7218 0000 0072 1900  _token).r....r..
-000007e0: 0000 7219 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-000007f0: 0046 0000 0073 0400 0000 0001 0801 7a17  .F...s........z.
-00000800: 5375 626d 6974 436f 6d6d 616e 6454 6573  SubmitCommandTes
-00000810: 742e 7365 7455 704e 630a 0000 0000 0000  t.setUpNc.......
-00000820: 000e 0000 000e 0000 0043 0000 0073 3a01  .........C...s:.
-00000830: 0000 6401 6402 7c00 6a00 6403 7c00 6a01  ..d.d.|.j.d.|.j.
-00000840: 6404 6405 6406 6407 6408 6409 640a 640b  d.d.d.d.d.d.d.d.
-00000850: 640c 670e 7d0a 7c08 7234 7c0a 640d 7c08  d.g.}.|.r4|.d.|.
-00000860: 6702 3700 7d0a 7c01 7244 7c0a 640e 7c01  g.7.}.|.rD|.d.|.
-00000870: 6702 3700 7d0a 7c02 7254 7c0a 640f 7c02  g.7.}.|.rT|.d.|.
-00000880: 6702 3700 7d0a 7c05 7264 7c0a 6410 7c05  g.7.}.|.rd|.d.|.
-00000890: 6702 3700 7d0a 7c06 7274 7c0a 6411 7c06  g.7.}.|.rt|.d.|.
-000008a0: 6702 3700 7d0a 7c07 7284 7c0a 6412 7c07  g.7.}.|.r.|.d.|.
-000008b0: 6702 3700 7d0a 7c03 7294 7c0a 6413 7c03  g.7.}.|.r.|.d.|.
-000008c0: 6702 3700 7d0a 7c04 72a4 7c0a 6414 7c04  g.7.}.|.r.|.d.|.
-000008d0: 6702 3700 7d0a 7402 6a03 7c0a 7402 6a04  g.7.}.t.j.|.t.j.
-000008e0: 7402 6a04 6415 8d03 7d0b 6416 7c0b 5f05  t.j.d...}.d.|._.
-000008f0: 791c 7c0b 6a06 8300 5c02 7d0c 7d0d 7c0b  y.|.j...\.}.}.|.
-00000900: 6a07 6417 6b02 7c0b 5f05 5700 6e42 0400  j.d.k.|._.W.nB..
-00000910: 7402 6a08 6b0a 9001 721c 0100 0100 0100  t.j.k...r.......
-00000920: 7c00 6a09 6a0a 6418 6419 6a0b 7c0a 8301  |.j.j.d.d.j.|...
-00000930: 1600 8301 0100 7c0b 6a0c 8300 0100 7c0b  ......|.j.....|.
-00000940: 6a06 8300 5c02 7d0c 7d0d 5900 6e02 5800  j...\.}.}.Y.n.X.
-00000950: 7c0c 6a0d 641a 8301 7c0b 5f0e 7c0d 6a0d  |.j.d...|._.|.j.
-00000960: 641a 8301 7c0b 5f0f 7c0b 5300 291b 4e7a  d...|._.|.S.).Nz
-00000970: 0b2e 2f6d 616e 6167 652e 7079 7a0c 2d2d  ../manage.pyz.--
-00000980: 7371 7561 642d 686f 7374 7a0d 2d2d 7371  squad-hostz.--sq
-00000990: 7561 642d 746f 6b65 6eda 0673 7562 6d69  uad-token..submi
-000009a0: 747a 072d 2d67 726f 7570 721c 0000 007a  tz.--groupr....z
-000009b0: 092d 2d70 726f 6a65 6374 721d 0000 007a  .--projectr....z
-000009c0: 072d 2d62 7569 6c64 5a09 6d79 5f62 7569  .--buildZ.my_bui
-000009d0: 6c64 367a 0d2d 2d65 6e76 6972 6f6e 6d65  ld6z.--environme
-000009e0: 6e74 5a0f 7465 7374 5f73 7562 6d69 745f  ntZ.test_submit_
-000009f0: 656e 767a 062d 2d6c 6f67 737a 092d 2d72  envz.--logsz.--r
-00000a00: 6573 756c 7473 7a10 2d2d 7265 7375 6c74  esultsz.--result
-00000a10: 732d 6c61 796f 7574 7a09 2d2d 6d65 7472  s-layoutz.--metr
-00000a20: 6963 737a 0a2d 2d6d 6574 6164 6174 617a  icsz.--metadataz
-00000a30: 0d2d 2d61 7474 6163 686d 656e 7473 7a0d  .--attachmentsz.
-00000a40: 2d2d 7265 7375 6c74 2d6e 616d 657a 0e2d  --result-namez.-
-00000a50: 2d72 6573 756c 742d 7661 6c75 6529 02da  -result-value)..
-00000a60: 0673 7464 6f75 74da 0673 7464 6572 7246  .stdout..stderrF
-00000a70: 7201 0000 007a 2752 756e 6e69 6e67 2022  r....z'Running "
-00000a80: 2573 2220 7469 6d65 206f 7574 2061 6674  %s" time out aft
-00000a90: 6572 2025 6920 7365 636f 6e64 7321 fa01  er %i seconds!..
-00000aa0: 207a 0575 7466 2d38 2910 7240 0000 0072   z.utf-8).r@...r
-00000ab0: 4100 0000 da02 7370 da05 506f 7065 6eda  A.....sp..Popen.
-00000ac0: 0450 4950 45da 026f 6bda 0b63 6f6d 6d75  .PIPE..ok..commu
-00000ad0: 6e69 6361 7465 da0a 7265 7475 726e 636f  nicate..returnco
-00000ae0: 6465 da0e 5469 6d65 6f75 7445 7870 6972  de..TimeoutExpir
-00000af0: 6564 da06 6c6f 6767 6572 da05 6572 726f  ed..logger..erro
-00000b00: 72da 046a 6f69 6eda 046b 696c 6cda 0664  r..join..kill..d
-00000b10: 6563 6f64 65da 036f 7574 da03 6572 7229  ecode..out..err)
-00000b20: 0e72 1800 0000 7239 0000 00da 0e72 6573  .r....r9.....res
-00000b30: 756c 7473 5f6c 6179 6f75 74da 0b72 6573  ults_layout..res
-00000b40: 756c 745f 6e61 6d65 da0c 7265 7375 6c74  ult_name..result
-00000b50: 5f76 616c 7565 da07 6d65 7472 6963 7372  _value..metricsr
-00000b60: 2f00 0000 da0b 6174 7461 6368 6d65 6e74  /.....attachment
-00000b70: 73da 046c 6f67 7372 2c00 0000 da04 6172  s..logsr,.....ar
-00000b80: 6776 da04 7072 6f63 7252 0000 0072 5300  gv..procrR...rS.
-00000b90: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000ba0: 00da 0d6d 616e 6167 655f 7375 626d 6974  ...manage_submit
-00000bb0: 4a00 0000 733c 0000 0000 020e 0116 0204  J...s<..........
-00000bc0: 010c 0104 010c 0104 010c 0104 010c 0104  ................
-00000bd0: 010c 0104 010c 0104 010c 0104 010c 0214  ................
-00000be0: 0106 0202 010c 0110 0112 0116 0108 0112  ................
-00000bf0: 020c 010c 017a 1f53 7562 6d69 7443 6f6d  .....z.SubmitCom
-00000c00: 6d61 6e64 5465 7374 2e6d 616e 6167 655f  mandTest.manage_
-00000c10: 7375 626d 6974 6301 0000 0000 0000 0002  submitc.........
-00000c20: 0000 0003 0000 0043 0000 0073 2600 0000  .......C...s&...
-00000c30: 7c00 6a00 8300 7d01 7c00 6a01 7c01 6a02  |.j...}.|.j.|.j.
-00000c40: 8301 0100 7c00 6a03 6401 7c01 6a04 8302  ....|.j.d.|.j...
-00000c50: 0100 6400 5300 2902 4e7a 3f41 7420 6c65  ..d.S.).Nz?At le
-00000c60: 6173 7420 6f6e 6520 6f66 202d 2d72 6573  ast one of --res
-00000c70: 756c 742d 6e61 6d65 2c20 2d2d 7265 7375  ult-name, --resu
-00000c80: 6c74 732c 202d 2d6d 6574 7269 6373 2069  lts, --metrics i
-00000c90: 7320 7265 7175 6972 6564 2905 725c 0000  s required).r\..
-00000ca0: 00da 0b61 7373 6572 7446 616c 7365 7249  ...assertFalserI
-00000cb0: 0000 00da 0861 7373 6572 7449 6e72 5300  .....assertInrS.
-00000cc0: 0000 2902 7218 0000 0072 5b00 0000 7219  ..).r....r[...r.
-00000cd0: 0000 0072 1900 0000 721a 0000 00da 1174  ...r....r......t
-00000ce0: 6573 745f 7375 626d 6974 5f65 6d70 7479  est_submit_empty
-00000cf0: 6f00 0000 7306 0000 0000 0108 010c 017a  o...s..........z
-00000d00: 2353 7562 6d69 7443 6f6d 6d61 6e64 5465  #SubmitCommandTe
-00000d10: 7374 2e74 6573 745f 7375 626d 6974 5f65  st.test_submit_e
-00000d20: 6d70 7479 6301 0000 0000 0000 0003 0000  mptyc...........
-00000d30: 0004 0000 0043 0000 0073 5a00 0000 7c00  .....C...sZ...|.
-00000d40: 6a00 6401 6402 6403 8d02 7d01 7c00 6a01  j.d.d.d...}.|.j.
-00000d50: 7c01 6a02 8301 0100 7c00 6a03 6404 7c01  |.j.....|.j.d.|.
-00000d60: 6a04 8302 0100 7405 7c00 6a06 6a07 6401  j.....t.|.j.j.d.
-00000d70: 6405 8d01 8301 7d02 7c00 6a08 6401 7c02  d.....}.|.j.d.|.
-00000d80: 6a09 8302 0100 7c00 6a08 6402 7c02 6a0a  j.....|.j.d.|.j.
-00000d90: 8302 0100 6400 5300 2906 4e7a 0b73 696e  ....d.S.).Nz.sin
-00000da0: 676c 652d 7465 7374 720e 0000 0029 0272  gle-testr....).r
-00000db0: 5500 0000 7256 0000 007a 0731 2074 6573  U...rV...z.1 tes
-00000dc0: 7473 2901 7222 0000 0029 0b72 5c00 0000  ts).r"...).r\...
-00000dd0: 7232 0000 0072 4900 0000 725e 0000 0072  r2...rI...r^...r
-00000de0: 5300 0000 720d 0000 0072 1500 0000 7231  S...r....r....r1
-00000df0: 0000 0072 3400 0000 7222 0000 0072 2900  ...r4...r"...r).
-00000e00: 0000 2903 7218 0000 0072 5b00 0000 7237  ..).r....r[...r7
-00000e10: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
-00000e20: 0000 da17 7465 7374 5f73 7562 6d69 745f  ....test_submit_
-00000e30: 7369 6e67 6c65 5f74 6573 7474 0000 0073  single_testt...s
-00000e40: 0c00 0000 0001 0e01 0c01 0e02 1201 0e01  ................
-00000e50: 7a29 5375 626d 6974 436f 6d6d 616e 6454  z)SubmitCommandT
-00000e60: 6573 742e 7465 7374 5f73 7562 6d69 745f  est.test_submit_
-00000e70: 7369 6e67 6c65 5f74 6573 7463 0100 0000  single_testc....
-00000e80: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00000e90: 732c 0000 007c 006a 0064 0164 0264 038d  s,...|.j.d.d.d..
-00000ea0: 027d 017c 006a 017c 016a 0283 0101 007c  .}.|.j.|.j.....|
-00000eb0: 006a 0364 047c 016a 0483 0201 0064 0053  .j.d.|.j.....d.S
-00000ec0: 0029 054e 7a13 7369 6e67 6c65 2d69 6e76  .).Nz.single-inv
-00000ed0: 616c 6964 2d74 6573 747a 096e 6f74 2d76  alid-testz.not-v
-00000ee0: 616c 6964 2902 7255 0000 0072 5600 0000  alid).rU...rV...
-00000ef0: 7a29 7265 7375 6c74 2d76 616c 7565 3a20  z)result-value: 
-00000f00: 696e 7661 6c69 6420 6368 6f69 6365 3a20  invalid choice: 
-00000f10: 276e 6f74 2d76 616c 6964 2729 0572 5c00  'not-valid').r\.
-00000f20: 0000 725d 0000 0072 4900 0000 725e 0000  ..r]...rI...r^..
-00000f30: 0072 5300 0000 2902 7218 0000 0072 5b00  .rS...).r....r[.
-00000f40: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00000f50: 00da 2074 6573 745f 7375 626d 6974 5f69  .. test_submit_i
-00000f60: 6e76 616c 6964 5f72 6573 756c 745f 7661  nvalid_result_va
-00000f70: 6c75 657d 0000 0073 0600 0000 0001 0e01  lue}...s........
-00000f80: 0c01 7a32 5375 626d 6974 436f 6d6d 616e  ..z2SubmitComman
-00000f90: 6454 6573 742e 7465 7374 5f73 7562 6d69  dTest.test_submi
-00000fa0: 745f 696e 7661 6c69 645f 7265 7375 6c74  t_invalid_result
-00000fb0: 5f76 616c 7565 6301 0000 0000 0000 0003  _valuec.........
-00000fc0: 0000 0004 0000 0043 0000 0073 9400 0000  .......C...s....
-00000fd0: 7c00 6a00 6401 6402 8d01 7d01 7c00 6a01  |.j.d.d...}.|.j.
-00000fe0: 7c01 6a02 8301 0100 7c00 6a03 6403 7c01  |.j.....|.j.d.|.
-00000ff0: 6a04 8302 0100 7405 7c00 6a06 6a07 6404  j.....t.|.j.j.d.
-00001000: 6405 8d01 8301 7d02 7c00 6a08 6404 7c02  d.....}.|.j.d.|.
-00001010: 6a09 8302 0100 7c00 6a08 6406 7c02 6a0a  j.....|.j.d.|.j.
-00001020: 8302 0100 7405 7c00 6a06 6a07 6407 6405  ....t.|.j.j.d.d.
-00001030: 8d01 8301 7d02 7c00 6a08 6407 7c02 6a09  ....}.|.j.d.|.j.
-00001040: 8302 0100 7c00 6a08 6408 7c02 6a0a 8302  ....|.j.d.|.j...
-00001050: 0100 7c00 6a08 6409 7c02 6a0b 8302 0100  ..|.j.d.|.j.....
-00001060: 6400 5300 290a 4e7a 2874 6573 7473 2f73  d.S.).Nz(tests/s
-00001070: 7562 6d69 745f 7265 7375 6c74 732f 7361  ubmit_results/sa
-00001080: 6d70 6c65 5f72 6573 756c 7473 2e6a 736f  mple_results.jso
-00001090: 6e29 0172 3900 0000 7a07 3220 7465 7374  n).r9...z.2 test
-000010a0: 737a 0b6a 736f 6e2d 7465 7374 2d31 2901  sz.json-test-1).
-000010b0: 7222 0000 0072 0e00 0000 7a0b 6a73 6f6e  r"...r....z.json
-000010c0: 2d74 6573 742d 3272 0f00 0000 7a0f 6a73  -test-2r....z.js
-000010d0: 6f6e 2d74 6573 742d 3220 6c6f 6729 0c72  on-test-2 log).r
-000010e0: 5c00 0000 7232 0000 0072 4900 0000 725e  \...r2...rI...r^
-000010f0: 0000 0072 5300 0000 720d 0000 0072 1500  ...rS...r....r..
-00001100: 0000 7231 0000 0072 3400 0000 7222 0000  ..r1...r4...r"..
-00001110: 0072 2900 0000 722a 0000 0029 0372 1800  .r)...r*...).r..
-00001120: 0000 725b 0000 0072 3700 0000 7219 0000  ..r[...r7...r...
-00001130: 0072 1900 0000 721a 0000 00da 1874 6573  .r....r......tes
-00001140: 745f 7375 626d 6974 5f72 6573 756c 7473  t_submit_results
-00001150: 5f6a 736f 6e82 0000 0073 1400 0000 0001  _json....s......
-00001160: 0c01 0c01 0e02 1201 0e01 0e02 1201 0e01  ................
-00001170: 0e01 7a2a 5375 626d 6974 436f 6d6d 616e  ..z*SubmitComman
-00001180: 6454 6573 742e 7465 7374 5f73 7562 6d69  dTest.test_submi
-00001190: 745f 7265 7375 6c74 735f 6a73 6f6e 6301  t_results_jsonc.
-000011a0: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
-000011b0: 0000 0073 2a00 0000 7c00 6a00 6401 6402  ...s*...|.j.d.d.
-000011c0: 8d01 7d01 7c00 6a01 7c01 6a02 8301 0100  ..}.|.j.|.j.....
-000011d0: 7c00 6a03 6403 7c01 6a04 8302 0100 6400  |.j.d.|.j.....d.
-000011e0: 5300 2904 4e7a 3274 6573 7473 2f73 7562  S.).Nz2tests/sub
-000011f0: 6d69 745f 7265 7375 6c74 732f 7361 6d70  mit_results/samp
-00001200: 6c65 5f72 6573 756c 7473 5f6d 616c 666f  le_results_malfo
-00001210: 726d 6564 2e6a 736f 6e29 0172 3900 0000  rmed.json).r9...
-00001220: 7a13 4661 696c 6564 2070 6172 7369 6e67  z.Failed parsing
-00001230: 2066 696c 6529 0572 5c00 0000 725d 0000   file).r\...r]..
-00001240: 0072 4900 0000 725e 0000 0072 5300 0000  .rI...r^...rS...
-00001250: 2902 7218 0000 0072 5b00 0000 7219 0000  ).r....r[...r...
-00001260: 0072 1900 0000 721a 0000 00da 2274 6573  .r....r....."tes
-00001270: 745f 7375 626d 6974 5f72 6573 756c 7473  t_submit_results
-00001280: 5f6d 616c 666f 726d 6564 5f6a 736f 6e90  _malformed_json.
-00001290: 0000 0073 0600 0000 0001 0c01 0c01 7a34  ...s..........z4
-000012a0: 5375 626d 6974 436f 6d6d 616e 6454 6573  SubmitCommandTes
-000012b0: 742e 7465 7374 5f73 7562 6d69 745f 7265  t.test_submit_re
-000012c0: 7375 6c74 735f 6d61 6c66 6f72 6d65 645f  sults_malformed_
-000012d0: 6a73 6f6e 6301 0000 0000 0000 0003 0000  jsonc...........
-000012e0: 0004 0000 0043 0000 0073 8e00 0000 7c00  .....C...s....|.
-000012f0: 6a00 6401 6402 6403 8d02 7d01 7c00 6a01  j.d.d.d...}.|.j.
-00001300: 7c01 6a02 7c01 6a03 6404 8d02 0100 7c00  |.j.|.j.d.....|.
-00001310: 6a04 6405 7c01 6a03 8302 0100 7405 7c00  j.d.|.j.....t.|.
-00001320: 6a06 6a07 6406 6407 8d01 8301 7d02 7c00  j.j.d.d.....}.|.
-00001330: 6a08 6408 7c02 6a09 8302 0100 7c00 6a08  j.d.|.j.....|.j.
-00001340: 6409 7c02 6a0a 8302 0100 7405 7c00 6a06  d.|.j.....t.|.j.
-00001350: 6a07 640a 6407 8d01 8301 7d02 7c00 6a08  j.d.d.....}.|.j.
-00001360: 640b 7c02 6a09 8302 0100 7c00 6a08 640c  d.|.j.....|.j.d.
-00001370: 7c02 6a0a 8302 0100 6400 5300 290d 4e7a  |.j.....d.S.).Nz
-00001380: 2574 6573 7473 2f64 6174 612f 7375 626d  %tests/data/subm
-00001390: 6974 2f74 7578 6275 696c 642f 6275 696c  it/tuxbuild/buil
-000013a0: 642e 6a73 6f6e da0d 7475 7862 7569 6c64  d.json..tuxbuild
-000013b0: 5f6a 736f 6e29 0272 3900 0000 7254 0000  _json).r9...rT..
-000013c0: 0029 01da 036d 7367 7a12 5375 626d 6974  .)...msgz.Submit
-000013d0: 7469 6e67 2032 2074 6573 7473 7a1c 7838  ting 2 testsz.x8
-000013e0: 362d 6763 632d 392d 6465 6663 6f6e 6669  6-gcc-9-defconfi
-000013f0: 672d 6239 3937 3963 6661 2901 7222 0000  g-b9979cfa).r"..
-00001400: 007a 2262 7569 6c64 2f78 3836 2d67 6363  .z"build/x86-gcc
-00001410: 2d39 2d64 6566 636f 6e66 6967 2d62 3939  -9-defconfig-b99
-00001420: 3739 6366 6172 0e00 0000 7a1e 6172 6d36  79cfar....z.arm6
-00001430: 342d 6763 632d 392d 6465 6663 6f6e 6669  4-gcc-9-defconfi
-00001440: 672d 3562 3039 3536 3865 7a24 6275 696c  g-5b09568ez$buil
-00001450: 642f 6172 6d36 342d 6763 632d 392d 6465  d/arm64-gcc-9-de
-00001460: 6663 6f6e 6669 672d 3562 3039 3536 3865  fconfig-5b09568e
-00001470: 720f 0000 0029 0b72 5c00 0000 7232 0000  r....).r\...r2..
-00001480: 0072 4900 0000 7253 0000 0072 5e00 0000  .rI...rS...r^...
-00001490: 720d 0000 0072 1500 0000 7231 0000 0072  r....r....r1...r
-000014a0: 3400 0000 7222 0000 0072 2900 0000 2903  4...r"...r)...).
-000014b0: 7218 0000 0072 5b00 0000 7237 0000 0072  r....r[...r7...r
-000014c0: 1900 0000 7219 0000 0072 1a00 0000 da21  ....r....r.....!
-000014d0: 7465 7374 5f73 7562 6d69 745f 7265 7375  test_submit_resu
-000014e0: 6c74 735f 7475 7862 7569 6c64 5f6a 736f  lts_tuxbuild_jso
-000014f0: 6e95 0000 0073 1200 0000 0001 0e01 1201  n....s..........
-00001500: 0e02 1201 0e01 0e02 1201 0e01 7a33 5375  ............z3Su
-00001510: 626d 6974 436f 6d6d 616e 6454 6573 742e  bmitCommandTest.
-00001520: 7465 7374 5f73 7562 6d69 745f 7265 7375  test_submit_resu
-00001530: 6c74 735f 7475 7862 7569 6c64 5f6a 736f  lts_tuxbuild_jso
-00001540: 6e63 0100 0000 0000 0000 0200 0000 0400  nc..............
-00001550: 0000 4300 0000 7332 0000 007c 006a 0064  ..C...s2...|.j.d
-00001560: 0164 0264 038d 027d 017c 006a 017c 016a  .d.d...}.|.j.|.j
-00001570: 027c 016a 0364 048d 0201 007c 006a 0464  .|.j.d.....|.j.d
-00001580: 057c 016a 0383 0201 0064 0053 0029 064e  .|.j.....d.S.).N
-00001590: 7a29 7465 7374 732f 6461 7461 2f73 7562  z)tests/data/sub
-000015a0: 6d69 742f 7475 7862 7569 6c64 2f6d 616c  mit/tuxbuild/mal
-000015b0: 666f 726d 6564 2e6a 736f 6e72 6400 0000  formed.jsonrd...
-000015c0: 2902 7239 0000 0072 5400 0000 2901 7265  ).r9...rT...).re
-000015d0: 0000 007a 1346 6169 6c65 6420 746f 206c  ...z.Failed to l
-000015e0: 6f61 6420 6a73 6f6e 2905 725c 0000 0072  oad json).r\...r
-000015f0: 5d00 0000 7249 0000 0072 5300 0000 725e  ]...rI...rS...r^
-00001600: 0000 0029 0272 1800 0000 725b 0000 0072  ...).r....r[...r
-00001610: 1900 0000 7219 0000 0072 1a00 0000 da2b  ....r....r.....+
-00001620: 7465 7374 5f73 7562 6d69 745f 7265 7375  test_submit_resu
-00001630: 6c74 735f 7475 7862 7569 6c64 5f6a 736f  lts_tuxbuild_jso
-00001640: 6e5f 6d61 6c66 6f72 6d65 64a2 0000 0073  n_malformed....s
-00001650: 0600 0000 0001 0e01 1201 7a3d 5375 626d  ..........z=Subm
-00001660: 6974 436f 6d6d 616e 6454 6573 742e 7465  itCommandTest.te
-00001670: 7374 5f73 7562 6d69 745f 7265 7375 6c74  st_submit_result
-00001680: 735f 7475 7862 7569 6c64 5f6a 736f 6e5f  s_tuxbuild_json_
-00001690: 6d61 6c66 6f72 6d65 6463 0100 0000 0000  malformedc......
-000016a0: 0000 0200 0000 0400 0000 4300 0000 732c  ..........C...s,
-000016b0: 0000 007c 006a 0064 0164 0264 038d 027d  ...|.j.d.d.d...}
-000016c0: 017c 006a 017c 016a 0283 0101 007c 006a  .|.j.|.j.....|.j
-000016d0: 0364 047c 016a 0483 0201 0064 0053 0029  .d.|.j.....d.S.)
-000016e0: 054e 7a27 7465 7374 732f 6461 7461 2f73  .Nz'tests/data/s
-000016f0: 7562 6d69 742f 7475 7862 7569 6c64 2f6d  ubmit/tuxbuild/m
-00001700: 6973 7369 6e67 2e6a 736f 6e72 6400 0000  issing.jsonrd...
-00001710: 2902 7239 0000 0072 5400 0000 7a44 5265  ).r9...rT...zDRe
-00001720: 7175 6573 7465 6420 6669 6c65 2074 6573  quested file tes
-00001730: 7473 2f64 6174 612f 7375 626d 6974 2f74  ts/data/submit/t
-00001740: 7578 6275 696c 642f 6d69 7373 696e 672e  uxbuild/missing.
-00001750: 6a73 6f6e 2064 6f65 736e 2774 2065 7869  json doesn't exi
-00001760: 7374 2905 725c 0000 0072 5d00 0000 7249  st).r\...r]...rI
-00001770: 0000 0072 5e00 0000 7253 0000 0029 0272  ...r^...rS...).r
-00001780: 1800 0000 725b 0000 0072 1900 0000 7219  ....r[...r....r.
-00001790: 0000 0072 1a00 0000 da29 7465 7374 5f73  ...r.....)test_s
-000017a0: 7562 6d69 745f 7265 7375 6c74 735f 7475  ubmit_results_tu
-000017b0: 7862 7569 6c64 5f6a 736f 6e5f 6d69 7373  xbuild_json_miss
-000017c0: 696e 67a7 0000 0073 0600 0000 0001 0e01  ing....s........
-000017d0: 0c01 7a3b 5375 626d 6974 436f 6d6d 616e  ..z;SubmitComman
-000017e0: 6454 6573 742e 7465 7374 5f73 7562 6d69  dTest.test_submi
-000017f0: 745f 7265 7375 6c74 735f 7475 7862 7569  t_results_tuxbui
-00001800: 6c64 5f6a 736f 6e5f 6d69 7373 696e 6763  ld_json_missingc
-00001810: 0100 0000 0000 0000 0200 0000 0300 0000  ................
-00001820: 4300 0000 732a 0000 007c 006a 0064 0164  C...s*...|.j.d.d
-00001830: 028d 017d 017c 006a 017c 016a 0283 0101  ...}.|.j.|.j....
-00001840: 007c 006a 0364 037c 016a 0483 0201 0064  .|.j.d.|.j.....d
-00001850: 0053 0029 044e 7264 0000 0029 0172 5400  .S.).Nrd...).rT.
-00001860: 0000 7a3f 4174 206c 6561 7374 206f 6e65  ..z?At least one
-00001870: 206f 6620 2d2d 7265 7375 6c74 2d6e 616d   of --result-nam
-00001880: 652c 202d 2d72 6573 756c 7473 2c20 2d2d  e, --results, --
-00001890: 6d65 7472 6963 7320 6973 2072 6571 7569  metrics is requi
-000018a0: 7265 6429 0572 5c00 0000 725d 0000 0072  red).r\...r]...r
-000018b0: 4900 0000 725e 0000 0072 5300 0000 2902  I...r^...rS...).
-000018c0: 7218 0000 0072 5b00 0000 7219 0000 0072  r....r[...r....r
-000018d0: 1900 0000 721a 0000 00da 3574 6573 745f  ....r.....5test_
-000018e0: 7375 626d 6974 5f72 6573 756c 7473 5f74  submit_results_t
-000018f0: 7578 6275 696c 645f 6a73 6f6e 5f72 6573  uxbuild_json_res
-00001900: 756c 7473 5f6f 7074 5f6d 6973 7369 6e67  ults_opt_missing
-00001910: ac00 0000 7306 0000 0000 010c 010c 017a  ....s..........z
-00001920: 4753 7562 6d69 7443 6f6d 6d61 6e64 5465  GSubmitCommandTe
-00001930: 7374 2e74 6573 745f 7375 626d 6974 5f72  st.test_submit_r
-00001940: 6573 756c 7473 5f74 7578 6275 696c 645f  esults_tuxbuild_
-00001950: 6a73 6f6e 5f72 6573 756c 7473 5f6f 7074  json_results_opt
-00001960: 5f6d 6973 7369 6e67 6301 0000 0000 0000  _missingc.......
-00001970: 0002 0000 0004 0000 0043 0000 0073 2c00  .........C...s,.
-00001980: 0000 7c00 6a00 6401 6402 6403 8d02 7d01  ..|.j.d.d.d...}.
-00001990: 7c00 6a01 7c01 6a02 8301 0100 7c00 6a03  |.j.|.j.....|.j.
-000019a0: 6404 7c01 6a04 8302 0100 6400 5300 2905  d.|.j.....d.S.).
-000019b0: 4e7a 2574 6573 7473 2f64 6174 612f 7375  Nz%tests/data/su
-000019c0: 626d 6974 2f74 7578 6275 696c 642f 6275  bmit/tuxbuild/bu
-000019d0: 696c 642e 6a73 6f6e 5a0a 6261 645f 6c61  ild.jsonZ.bad_la
-000019e0: 796f 7574 2902 7239 0000 0072 5400 0000  yout).r9...rT...
-000019f0: 7a37 6172 6775 6d65 6e74 202d 2d72 6573  z7argument --res
-00001a00: 756c 7473 2d6c 6179 6f75 743a 2069 6e76  ults-layout: inv
-00001a10: 616c 6964 2063 686f 6963 653a 2027 6261  alid choice: 'ba
-00001a20: 645f 6c61 796f 7574 2729 0572 5c00 0000  d_layout').r\...
-00001a30: 725d 0000 0072 4900 0000 725e 0000 0072  r]...rI...r^...r
-00001a40: 5300 0000 2902 7218 0000 0072 5b00 0000  S...).r....r[...
-00001a50: 7219 0000 0072 1900 0000 721a 0000 00da  r....r....r.....
-00001a60: 3074 6573 745f 7375 626d 6974 5f72 6573  0test_submit_res
-00001a70: 756c 7473 5f74 7578 6275 696c 645f 6a73  ults_tuxbuild_js
-00001a80: 6f6e 5f6c 6179 6f75 745f 6172 675f 6261  on_layout_arg_ba
-00001a90: 64b1 0000 0073 0600 0000 0001 0e01 0c01  d....s..........
-00001aa0: 7a42 5375 626d 6974 436f 6d6d 616e 6454  zBSubmitCommandT
-00001ab0: 6573 742e 7465 7374 5f73 7562 6d69 745f  est.test_submit_
-00001ac0: 7265 7375 6c74 735f 7475 7862 7569 6c64  results_tuxbuild
-00001ad0: 5f6a 736f 6e5f 6c61 796f 7574 5f61 7267  _json_layout_arg
-00001ae0: 5f62 6164 6301 0000 0000 0000 0003 0000  _badc...........
-00001af0: 0004 0000 0043 0000 0073 9400 0000 7c00  .....C...s....|.
-00001b00: 6a00 6401 6402 8d01 7d01 7c00 6a01 7c01  j.d.d...}.|.j.|.
-00001b10: 6a02 8301 0100 7c00 6a03 6403 7c01 6a04  j.....|.j.d.|.j.
-00001b20: 8302 0100 7405 7c00 6a06 6a07 6404 6405  ....t.|.j.j.d.d.
-00001b30: 8d01 8301 7d02 7c00 6a08 6404 7c02 6a09  ....}.|.j.d.|.j.
-00001b40: 8302 0100 7c00 6a08 6406 7c02 6a0a 8302  ....|.j.d.|.j...
-00001b50: 0100 7405 7c00 6a06 6a07 6407 6405 8d01  ..t.|.j.j.d.d...
-00001b60: 8301 7d02 7c00 6a08 6407 7c02 6a09 8302  ..}.|.j.d.|.j...
-00001b70: 0100 7c00 6a08 6408 7c02 6a0a 8302 0100  ..|.j.d.|.j.....
-00001b80: 7c00 6a08 6409 7c02 6a0b 8302 0100 6400  |.j.d.|.j.....d.
-00001b90: 5300 290a 4e7a 2874 6573 7473 2f73 7562  S.).Nz(tests/sub
-00001ba0: 6d69 745f 7265 7375 6c74 732f 7361 6d70  mit_results/samp
-00001bb0: 6c65 5f72 6573 756c 7473 2e79 616d 6c29  le_results.yaml)
-00001bc0: 0172 3900 0000 7a07 3220 7465 7374 737a  .r9...z.2 testsz
-00001bd0: 0b79 616d 6c2d 7465 7374 2d31 2901 7222  .yaml-test-1).r"
-00001be0: 0000 0072 0e00 0000 7a0b 7961 6d6c 2d74  ...r....z.yaml-t
-00001bf0: 6573 742d 3272 0f00 0000 7a0f 7961 6d6c  est-2r....z.yaml
-00001c00: 2d74 6573 742d 3220 6c6f 6729 0c72 5c00  -test-2 log).r\.
-00001c10: 0000 7232 0000 0072 4900 0000 725e 0000  ..r2...rI...r^..
-00001c20: 0072 5300 0000 720d 0000 0072 1500 0000  .rS...r....r....
-00001c30: 7231 0000 0072 3400 0000 7222 0000 0072  r1...r4...r"...r
-00001c40: 2900 0000 722a 0000 0029 0372 1800 0000  )...r*...).r....
-00001c50: 725b 0000 0072 3700 0000 7219 0000 0072  r[...r7...r....r
-00001c60: 1900 0000 721a 0000 00da 1874 6573 745f  ....r......test_
-00001c70: 7375 626d 6974 5f72 6573 756c 7473 5f79  submit_results_y
-00001c80: 616d 6cb6 0000 0073 1400 0000 0001 0c01  aml....s........
-00001c90: 0c01 0e02 1201 0e01 0e02 1201 0e01 0e01  ................
-00001ca0: 7a2a 5375 626d 6974 436f 6d6d 616e 6454  z*SubmitCommandT
-00001cb0: 6573 742e 7465 7374 5f73 7562 6d69 745f  est.test_submit_
-00001cc0: 7265 7375 6c74 735f 7961 6d6c 6301 0000  results_yamlc...
-00001cd0: 0000 0000 0002 0000 0003 0000 0043 0000  .............C..
-00001ce0: 0073 2a00 0000 7c00 6a00 6401 6402 8d01  .s*...|.j.d.d...
-00001cf0: 7d01 7c00 6a01 7c01 6a02 8301 0100 7c00  }.|.j.|.j.....|.
-00001d00: 6a03 6403 7c01 6a04 8302 0100 6400 5300  j.d.|.j.....d.S.
-00001d10: 2904 4e7a 3274 6573 7473 2f73 7562 6d69  ).Nz2tests/submi
-00001d20: 745f 7265 7375 6c74 732f 7361 6d70 6c65  t_results/sample
-00001d30: 5f72 6573 756c 7473 5f6d 616c 666f 726d  _results_malform
-00001d40: 6564 2e79 616d 6c29 0172 3900 0000 7a13  ed.yaml).r9...z.
-00001d50: 4661 696c 6564 2070 6172 7369 6e67 2066  Failed parsing f
-00001d60: 696c 6529 0572 5c00 0000 725d 0000 0072  ile).r\...r]...r
-00001d70: 4900 0000 725e 0000 0072 5300 0000 2902  I...r^...rS...).
-00001d80: 7218 0000 0072 5b00 0000 7219 0000 0072  r....r[...r....r
-00001d90: 1900 0000 721a 0000 00da 2274 6573 745f  ....r....."test_
-00001da0: 7375 626d 6974 5f72 6573 756c 7473 5f6d  submit_results_m
-00001db0: 616c 666f 726d 6564 5f79 616d 6cc4 0000  alformed_yaml...
-00001dc0: 0073 0600 0000 0001 0c01 0c01 7a34 5375  .s..........z4Su
-00001dd0: 626d 6974 436f 6d6d 616e 6454 6573 742e  bmitCommandTest.
-00001de0: 7465 7374 5f73 7562 6d69 745f 7265 7375  test_submit_resu
-00001df0: 6c74 735f 6d61 6c66 6f72 6d65 645f 7961  lts_malformed_ya
-00001e00: 6d6c 6301 0000 0000 0000 0003 0000 0003  mlc.............
-00001e10: 0000 0043 0000 0073 3200 0000 6401 7d01  ...C...s2...d.}.
-00001e20: 7c00 6a00 7c01 6402 8d01 7d02 7c00 6a01  |.j.|.d...}.|.j.
-00001e30: 7c02 6a02 8301 0100 7c00 6a03 6403 7c01  |.j.....|.j.d.|.
-00001e40: 1600 7c02 6a04 8302 0100 6400 5300 2904  ..|.j.....d.S.).
-00001e50: 4e7a 2774 6573 7473 2f73 7562 6d69 745f  Nz'tests/submit_
-00001e60: 7265 7375 6c74 732f 7361 6d70 6c65 5f72  results/sample_r
-00001e70: 6573 756c 7473 2e74 7874 2901 7239 0000  esults.txt).r9..
-00001e80: 007a 3546 696c 6520 2225 7322 2064 6f65  .z5File "%s" doe
-00001e90: 7320 6e6f 7420 6861 7665 2061 204a 534f  s not have a JSO
-00001ea0: 4e20 6f72 2059 414d 4c20 6669 6c65 2065  N or YAML file e
-00001eb0: 7874 656e 7369 6f6e 2905 725c 0000 0072  xtension).r\...r
-00001ec0: 5d00 0000 7249 0000 0072 5e00 0000 7253  ]...rI...r^...rS
-00001ed0: 0000 0029 0372 1800 0000 da01 7072 5b00  ...).r......pr[.
-00001ee0: 0000 7219 0000 0072 1900 0000 721a 0000  ..r....r....r...
-00001ef0: 00da 2174 6573 745f 7375 626d 6974 5f72  ..!test_submit_r
-00001f00: 6573 756c 7473 5f62 6164 5f65 7874 656e  esults_bad_exten
-00001f10: 7369 6f6e c900 0000 7308 0000 0000 0104  sion....s.......
-00001f20: 010c 010c 017a 3353 7562 6d69 7443 6f6d  .....z3SubmitCom
-00001f30: 6d61 6e64 5465 7374 2e74 6573 745f 7375  mandTest.test_su
-00001f40: 626d 6974 5f72 6573 756c 7473 5f62 6164  bmit_results_bad
-00001f50: 5f65 7874 656e 7369 6f6e 6301 0000 0000  _extensionc.....
-00001f60: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00001f70: 2a00 0000 7c00 6a00 6401 6402 8d01 7d01  *...|.j.d.d...}.
-00001f80: 7c00 6a01 7c01 6a02 8301 0100 7c00 6a03  |.j.|.j.....|.j.
-00001f90: 6403 7c01 6a04 8302 0100 6400 5300 2904  d.|.j.....d.S.).
-00001fa0: 4e7a 2874 6573 7473 2f73 7562 6d69 745f  Nz(tests/submit_
-00001fb0: 7265 7375 6c74 732f 7361 6d70 6c65 5f6d  results/sample_m
-00001fc0: 6574 7269 6373 2e6a 736f 6e29 0172 5700  etrics.json).rW.
-00001fd0: 0000 7a09 3120 6d65 7472 6963 7329 0572  ..z.1 metrics).r
-00001fe0: 5c00 0000 7232 0000 0072 4900 0000 725e  \...r2...rI...r^
-00001ff0: 0000 0072 5300 0000 2902 7218 0000 0072  ...rS...).r....r
-00002000: 5b00 0000 7219 0000 0072 1900 0000 721a  [...r....r....r.
-00002010: 0000 00da 1974 6573 745f 7375 626d 6974  .....test_submit
-00002020: 5f73 696e 676c 655f 6d65 7472 6963 cf00  _single_metric..
-00002030: 0000 7306 0000 0000 010c 010c 017a 2b53  ..s..........z+S
-00002040: 7562 6d69 7443 6f6d 6d61 6e64 5465 7374  ubmitCommandTest
-00002050: 2e74 6573 745f 7375 626d 6974 5f73 696e  .test_submit_sin
-00002060: 676c 655f 6d65 7472 6963 6301 0000 0000  gle_metricc.....
-00002070: 0000 0003 0000 0006 0000 0043 0000 0073  ...........C...s
-00002080: 7e00 0000 7c00 6a00 6401 6402 6403 6404  ~...|.j.d.d.d.d.
-00002090: 6405 8d04 7d01 7c00 6a01 7c01 6a02 7c01  d...}.|.j.|.j.|.
-000020a0: 6a03 6406 8d02 0100 7c00 6a04 6407 7c01  j.d.....|.j.d.|.
-000020b0: 6a03 8302 0100 7405 7c00 6a06 6a07 6408  j.....t.|.j.j.d.
-000020c0: 6409 8d01 8301 7d02 7c00 6a08 6408 7c02  d.....}.|.j.d.|.
-000020d0: 6a09 8302 0100 7c00 6a08 640a 740a 7c02  j.....|.j.d.t.|.
-000020e0: 6a0b 8300 8301 8302 0100 7c00 6a08 640b  j.........|.j.d.
-000020f0: 740a 7c02 6a0c 8300 8301 8302 0100 6400  t.|.j.........d.
-00002100: 5300 290c 4e7a 2874 6573 7473 2f73 7562  S.).Nz(tests/sub
-00002110: 6d69 745f 7265 7375 6c74 732f 7361 6d70  mit_results/samp
-00002120: 6c65 5f72 6573 756c 7473 2e6a 736f 6e7a  le_results.jsonz
-00002130: 2874 6573 7473 2f73 7562 6d69 745f 7265  (tests/submit_re
-00002140: 7375 6c74 732f 7361 6d70 6c65 5f6d 6574  sults/sample_met
-00002150: 7269 6373 2e6a 736f 6e7a 2974 6573 7473  rics.jsonz)tests
-00002160: 2f73 7562 6d69 745f 7265 7375 6c74 732f  /submit_results/
-00002170: 7361 6d70 6c65 5f6d 6574 6164 6174 612e  sample_metadata.
-00002180: 6a73 6f6e 7a23 7465 7374 732f 7375 626d  jsonz#tests/subm
-00002190: 6974 5f72 6573 756c 7473 2f73 616d 706c  it_results/sampl
-000021a0: 655f 6c6f 672e 6c6f 6729 0472 3900 0000  e_log.log).r9...
-000021b0: 7257 0000 0072 2f00 0000 7259 0000 0029  rW...r/...rY...)
-000021c0: 0172 6500 0000 7a12 3220 7465 7374 732c  .re...z.2 tests,
-000021d0: 2031 206d 6574 7269 6373 5a12 6a73 6f6e   1 metricsZ.json
-000021e0: 6d65 7461 6461 7461 6a6f 6269 6431 2901  metadatajobid1).
-000021f0: 7221 0000 00e9 0200 0000 7202 0000 0029  r!........r....)
-00002200: 0d72 5c00 0000 7232 0000 0072 4900 0000  .r\...r2...rI...
-00002210: 7253 0000 0072 5e00 0000 720d 0000 0072  rS...r^...r....r
-00002220: 1500 0000 da08 7465 7374 7275 6e73 7234  ......testrunsr4
-00002230: 0000 0072 2100 0000 7233 0000 0072 3100  ...r!...r3...r1.
-00002240: 0000 7257 0000 0029 0372 1800 0000 725b  ..rW...).r....r[
-00002250: 0000 0072 3600 0000 7219 0000 0072 1900  ...r6...r....r..
-00002260: 0000 721a 0000 00da 1674 6573 745f 7375  ..r......test_su
-00002270: 626d 6974 5f65 7665 7279 7468 696e 67d4  bmit_everything.
-00002280: 0000 0073 1400 0000 0001 0601 0201 0201  ...s............
-00002290: 0801 1201 0e02 1201 0e02 1401 7a28 5375  ............z(Su
-000022a0: 626d 6974 436f 6d6d 616e 6454 6573 742e  bmitCommandTest.
-000022b0: 7465 7374 5f73 7562 6d69 745f 6576 6572  test_submit_ever
-000022c0: 7974 6869 6e67 2909 4e4e 4e4e 4e4e 4e4e  ything).NNNNNNNN
-000022d0: 4e29 1872 3c00 0000 723d 0000 0072 3e00  N).r<...r=...r>.
-000022e0: 0000 7203 0000 0072 1700 0000 7240 0000  ..r....r....r@..
-000022f0: 0072 4100 0000 721b 0000 0072 5c00 0000  .rA...r....r\...
-00002300: 725f 0000 0072 6000 0000 7261 0000 0072  r_...r`...ra...r
-00002310: 6200 0000 7263 0000 0072 6600 0000 7267  b...rc...rf...rg
-00002320: 0000 0072 6800 0000 7269 0000 0072 6a00  ...rh...ri...rj.
-00002330: 0000 726b 0000 0072 6c00 0000 726e 0000  ..rk...rl...rn..
-00002340: 0072 6f00 0000 7272 0000 0072 1900 0000  .ro...rr...r....
-00002350: 7219 0000 0072 1900 0000 721a 0000 0072  r....r....r....r
-00002360: 3f00 0000 4100 0000 7328 0000 0008 020a  ?...A...s(......
-00002370: 0104 0208 0400 010a 2408 0508 0908 0508  ........$.......
-00002380: 0e08 0508 0d08 0508 0508 0508 0508 0e08  ................
-00002390: 0508 0608 0572 3f00 0000 2919 da08 756e  .....r?...)...un
-000023a0: 6974 7465 7374 da0a 7375 6270 726f 6365  ittest..subproce
-000023b0: 7373 7246 0000 00da 0072 0300 0000 da15  ssrF.....r......
-000023c0: 7371 7561 645f 636c 6965 6e74 2e63 6f72  squad_client.cor
-000023d0: 652e 6170 6972 0400 0000 da18 7371 7561  e.apir......squa
-000023e0: 645f 636c 6965 6e74 2e63 6f72 652e 6d6f  d_client.core.mo
-000023f0: 6465 6c73 7205 0000 0072 0600 0000 7207  delsr....r....r.
-00002400: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00002410: 0000 720b 0000 0072 0c00 0000 da12 7371  ..r....r......sq
-00002420: 7561 645f 636c 6965 6e74 2e75 7469 6c73  uad_client.utils
-00002430: 720d 0000 0072 2800 0000 da04 4641 494c  r....r(.....FAIL
-00002440: 5a05 5846 4149 4c5a 0453 4b49 50da 0854  Z.XFAILZ.SKIP..T
-00002450: 6573 7443 6173 6572 1100 0000 723f 0000  estCaser....r?..
-00002460: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
-00002470: 721a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00002480: 0000 0073 1600 0000 0801 0802 0c01 0c01  ...s............
-00002490: 2801 0c03 0401 0401 0401 0403 1231       (............1
+00000720: 2464 2584 005a 1764 2664 2784 005a 1864  $d%..Z.d&d'..Z.d
+00000730: 2864 2984 005a 1964 2a64 2b84 005a 1a64  (d)..Z.d*d+..Z.d
+00000740: 0553 0029 2dda 1153 7562 6d69 7443 6f6d  .S.)-..SubmitCom
+00000750: 6d61 6e64 5465 7374 7a13 6874 7470 3a2f  mandTestz.http:/
+00000760: 2f6c 6f63 616c 686f 7374 3a25 7372 1200  /localhost:%sr..
+00000770: 0000 6301 0000 0000 0000 0001 0000 0004  ..c.............
+00000780: 0000 0043 0000 0073 1e00 0000 7400 8300  ...C...s....t...
+00000790: 7c00 5f01 7402 6a03 7c00 6a04 7c00 6a05  |._.t.j.|.j.|.j.
+000007a0: 6401 8d02 0100 6400 5300 2902 4e29 0272  d.....d.S.).N).r
+000007b0: 1300 0000 7214 0000 0029 0672 0500 0000  ....r....).r....
+000007c0: 7215 0000 0072 0400 0000 7216 0000 00da  r....r....r.....
+000007d0: 0e74 6573 7469 6e67 5f73 6572 7665 72da  .testing_server.
+000007e0: 0d74 6573 7469 6e67 5f74 6f6b 656e 2901  .testing_token).
+000007f0: 7218 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000800: 1a00 0000 721b 0000 0046 0000 0073 0400  ....r....F...s..
+00000810: 0000 0001 0801 7a17 5375 626d 6974 436f  ......z.SubmitCo
+00000820: 6d6d 616e 6454 6573 742e 7365 7455 704e  mmandTest.setUpN
+00000830: 630a 0000 0000 0000 000e 0000 000e 0000  c...............
+00000840: 0043 0000 0073 3a01 0000 6401 6402 7c00  .C...s:...d.d.|.
+00000850: 6a00 6403 7c00 6a01 6404 6405 6406 6407  j.d.|.j.d.d.d.d.
+00000860: 6408 6409 640a 640b 640c 670e 7d0a 7c08  d.d.d.d.d.g.}.|.
+00000870: 7234 7c0a 640d 7c08 6702 3700 7d0a 7c01  r4|.d.|.g.7.}.|.
+00000880: 7244 7c0a 640e 7c01 6702 3700 7d0a 7c02  rD|.d.|.g.7.}.|.
+00000890: 7254 7c0a 640f 7c02 6702 3700 7d0a 7c05  rT|.d.|.g.7.}.|.
+000008a0: 7264 7c0a 6410 7c05 6702 3700 7d0a 7c06  rd|.d.|.g.7.}.|.
+000008b0: 7274 7c0a 6411 7c06 6702 3700 7d0a 7c07  rt|.d.|.g.7.}.|.
+000008c0: 7284 7c0a 6412 7c07 6702 3700 7d0a 7c03  r.|.d.|.g.7.}.|.
+000008d0: 7294 7c0a 6413 7c03 6702 3700 7d0a 7c04  r.|.d.|.g.7.}.|.
+000008e0: 72a4 7c0a 6414 7c04 6702 3700 7d0a 7402  r.|.d.|.g.7.}.t.
+000008f0: 6a03 7c0a 7402 6a04 7402 6a04 6415 8d03  j.|.t.j.t.j.d...
+00000900: 7d0b 6416 7c0b 5f05 791c 7c0b 6a06 8300  }.d.|._.y.|.j...
+00000910: 5c02 7d0c 7d0d 7c0b 6a07 6417 6b02 7c0b  \.}.}.|.j.d.k.|.
+00000920: 5f05 5700 6e42 0400 7402 6a08 6b0a 9001  _.W.nB..t.j.k...
+00000930: 721c 0100 0100 0100 7c00 6a09 6a0a 6418  r.......|.j.j.d.
+00000940: 6419 6a0b 7c0a 8301 1600 8301 0100 7c0b  d.j.|.........|.
+00000950: 6a0c 8300 0100 7c0b 6a06 8300 5c02 7d0c  j.....|.j...\.}.
+00000960: 7d0d 5900 6e02 5800 7c0c 6a0d 641a 8301  }.Y.n.X.|.j.d...
+00000970: 7c0b 5f0e 7c0d 6a0d 641a 8301 7c0b 5f0f  |._.|.j.d...|._.
+00000980: 7c0b 5300 291b 4e7a 0b2e 2f6d 616e 6167  |.S.).Nz../manag
+00000990: 652e 7079 7a0c 2d2d 7371 7561 642d 686f  e.pyz.--squad-ho
+000009a0: 7374 7a0d 2d2d 7371 7561 642d 746f 6b65  stz.--squad-toke
+000009b0: 6eda 0673 7562 6d69 747a 072d 2d67 726f  n..submitz.--gro
+000009c0: 7570 721c 0000 007a 092d 2d70 726f 6a65  upr....z.--proje
+000009d0: 6374 721d 0000 007a 072d 2d62 7569 6c64  ctr....z.--build
+000009e0: 5a09 6d79 5f62 7569 6c64 367a 0d2d 2d65  Z.my_build6z.--e
+000009f0: 6e76 6972 6f6e 6d65 6e74 5a0f 7465 7374  nvironmentZ.test
+00000a00: 5f73 7562 6d69 745f 656e 767a 062d 2d6c  _submit_envz.--l
+00000a10: 6f67 737a 092d 2d72 6573 756c 7473 7a10  ogsz.--resultsz.
+00000a20: 2d2d 7265 7375 6c74 732d 6c61 796f 7574  --results-layout
+00000a30: 7a09 2d2d 6d65 7472 6963 737a 0a2d 2d6d  z.--metricsz.--m
+00000a40: 6574 6164 6174 617a 0d2d 2d61 7474 6163  etadataz.--attac
+00000a50: 686d 656e 7473 7a0d 2d2d 7265 7375 6c74  hmentsz.--result
+00000a60: 2d6e 616d 657a 0e2d 2d72 6573 756c 742d  -namez.--result-
+00000a70: 7661 6c75 6529 02da 0673 7464 6f75 74da  value)...stdout.
+00000a80: 0673 7464 6572 7246 7201 0000 007a 2752  .stderrFr....z'R
+00000a90: 756e 6e69 6e67 2022 2573 2220 7469 6d65  unning "%s" time
+00000aa0: 206f 7574 2061 6674 6572 2025 6920 7365   out after %i se
+00000ab0: 636f 6e64 7321 fa01 207a 0575 7466 2d38  conds!.. z.utf-8
+00000ac0: 2910 7240 0000 0072 4100 0000 da02 7370  ).r@...rA.....sp
+00000ad0: da05 506f 7065 6eda 0450 4950 45da 026f  ..Popen..PIPE..o
+00000ae0: 6bda 0b63 6f6d 6d75 6e69 6361 7465 da0a  k..communicate..
+00000af0: 7265 7475 726e 636f 6465 da0e 5469 6d65  returncode..Time
+00000b00: 6f75 7445 7870 6972 6564 da06 6c6f 6767  outExpired..logg
+00000b10: 6572 da05 6572 726f 72da 046a 6f69 6eda  er..error..join.
+00000b20: 046b 696c 6cda 0664 6563 6f64 65da 036f  .kill..decode..o
+00000b30: 7574 da03 6572 7229 0e72 1800 0000 7239  ut..err).r....r9
+00000b40: 0000 00da 0e72 6573 756c 7473 5f6c 6179  .....results_lay
+00000b50: 6f75 74da 0b72 6573 756c 745f 6e61 6d65  out..result_name
+00000b60: da0c 7265 7375 6c74 5f76 616c 7565 da07  ..result_value..
+00000b70: 6d65 7472 6963 7372 2f00 0000 da0b 6174  metricsr/.....at
+00000b80: 7461 6368 6d65 6e74 73da 046c 6f67 7372  tachments..logsr
+00000b90: 2c00 0000 da04 6172 6776 da04 7072 6f63  ,.....argv..proc
+00000ba0: 7252 0000 0072 5300 0000 7219 0000 0072  rR...rS...r....r
+00000bb0: 1900 0000 721a 0000 00da 0d6d 616e 6167  ....r......manag
+00000bc0: 655f 7375 626d 6974 4a00 0000 733c 0000  e_submitJ...s<..
+00000bd0: 0000 020e 0116 0204 010c 0104 010c 0104  ................
+00000be0: 010c 0104 010c 0104 010c 0104 010c 0104  ................
+00000bf0: 010c 0104 010c 0214 0106 0202 010c 0110  ................
+00000c00: 0112 0116 0108 0112 020c 010c 017a 1f53  .............z.S
+00000c10: 7562 6d69 7443 6f6d 6d61 6e64 5465 7374  ubmitCommandTest
+00000c20: 2e6d 616e 6167 655f 7375 626d 6974 6301  .manage_submitc.
+00000c30: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000c40: 0000 0073 2600 0000 7c00 6a00 8300 7d01  ...s&...|.j...}.
+00000c50: 7c00 6a01 7c01 6a02 8301 0100 7c00 6a03  |.j.|.j.....|.j.
+00000c60: 6401 7c01 6a04 8302 0100 6400 5300 2902  d.|.j.....d.S.).
+00000c70: 4e7a 3f41 7420 6c65 6173 7420 6f6e 6520  Nz?At least one 
+00000c80: 6f66 202d 2d72 6573 756c 742d 6e61 6d65  of --result-name
+00000c90: 2c20 2d2d 7265 7375 6c74 732c 202d 2d6d  , --results, --m
+00000ca0: 6574 7269 6373 2069 7320 7265 7175 6972  etrics is requir
+00000cb0: 6564 2905 725c 0000 00da 0b61 7373 6572  ed).r\.....asser
+00000cc0: 7446 616c 7365 7249 0000 00da 0861 7373  tFalserI.....ass
+00000cd0: 6572 7449 6e72 5300 0000 2902 7218 0000  ertInrS...).r...
+00000ce0: 0072 5b00 0000 7219 0000 0072 1900 0000  .r[...r....r....
+00000cf0: 721a 0000 00da 1174 6573 745f 7375 626d  r......test_subm
+00000d00: 6974 5f65 6d70 7479 6f00 0000 7306 0000  it_emptyo...s...
+00000d10: 0000 0108 010c 017a 2353 7562 6d69 7443  .......z#SubmitC
+00000d20: 6f6d 6d61 6e64 5465 7374 2e74 6573 745f  ommandTest.test_
+00000d30: 7375 626d 6974 5f65 6d70 7479 6301 0000  submit_emptyc...
+00000d40: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00000d50: 0073 5a00 0000 7c00 6a00 6401 6402 6403  .sZ...|.j.d.d.d.
+00000d60: 8d02 7d01 7c00 6a01 7c01 6a02 8301 0100  ..}.|.j.|.j.....
+00000d70: 7c00 6a03 6404 7c01 6a04 8302 0100 7405  |.j.d.|.j.....t.
+00000d80: 7c00 6a06 6a07 6401 6405 8d01 8301 7d02  |.j.j.d.d.....}.
+00000d90: 7c00 6a08 6401 7c02 6a09 8302 0100 7c00  |.j.d.|.j.....|.
+00000da0: 6a08 6402 7c02 6a0a 8302 0100 6400 5300  j.d.|.j.....d.S.
+00000db0: 2906 4e7a 0b73 696e 676c 652d 7465 7374  ).Nz.single-test
+00000dc0: 720e 0000 0029 0272 5500 0000 7256 0000  r....).rU...rV..
+00000dd0: 007a 0731 2074 6573 7473 2901 7222 0000  .z.1 tests).r"..
+00000de0: 0029 0b72 5c00 0000 7232 0000 0072 4900  .).r\...r2...rI.
+00000df0: 0000 725e 0000 0072 5300 0000 720d 0000  ..r^...rS...r...
+00000e00: 0072 1500 0000 7231 0000 0072 3400 0000  .r....r1...r4...
+00000e10: 7222 0000 0072 2900 0000 2903 7218 0000  r"...r)...).r...
+00000e20: 0072 5b00 0000 7237 0000 0072 1900 0000  .r[...r7...r....
+00000e30: 7219 0000 0072 1a00 0000 da17 7465 7374  r....r......test
+00000e40: 5f73 7562 6d69 745f 7369 6e67 6c65 5f74  _submit_single_t
+00000e50: 6573 7474 0000 0073 0c00 0000 0001 0e01  estt...s........
+00000e60: 0c01 0e02 1201 0e01 7a29 5375 626d 6974  ........z)Submit
+00000e70: 436f 6d6d 616e 6454 6573 742e 7465 7374  CommandTest.test
+00000e80: 5f73 7562 6d69 745f 7369 6e67 6c65 5f74  _submit_single_t
+00000e90: 6573 7463 0100 0000 0000 0000 0200 0000  estc............
+00000ea0: 0400 0000 4300 0000 732c 0000 007c 006a  ....C...s,...|.j
+00000eb0: 0064 0164 0264 038d 027d 017c 006a 017c  .d.d.d...}.|.j.|
+00000ec0: 016a 0283 0101 007c 006a 0364 047c 016a  .j.....|.j.d.|.j
+00000ed0: 0483 0201 0064 0053 0029 054e 7a13 7369  .....d.S.).Nz.si
+00000ee0: 6e67 6c65 2d69 6e76 616c 6964 2d74 6573  ngle-invalid-tes
+00000ef0: 747a 096e 6f74 2d76 616c 6964 2902 7255  tz.not-valid).rU
+00000f00: 0000 0072 5600 0000 7a29 7265 7375 6c74  ...rV...z)result
+00000f10: 2d76 616c 7565 3a20 696e 7661 6c69 6420  -value: invalid 
+00000f20: 6368 6f69 6365 3a20 276e 6f74 2d76 616c  choice: 'not-val
+00000f30: 6964 2729 0572 5c00 0000 725d 0000 0072  id').r\...r]...r
+00000f40: 4900 0000 725e 0000 0072 5300 0000 2902  I...r^...rS...).
+00000f50: 7218 0000 0072 5b00 0000 7219 0000 0072  r....r[...r....r
+00000f60: 1900 0000 721a 0000 00da 2074 6573 745f  ....r..... test_
+00000f70: 7375 626d 6974 5f69 6e76 616c 6964 5f72  submit_invalid_r
+00000f80: 6573 756c 745f 7661 6c75 657d 0000 0073  esult_value}...s
+00000f90: 0600 0000 0001 0e01 0c01 7a32 5375 626d  ..........z2Subm
+00000fa0: 6974 436f 6d6d 616e 6454 6573 742e 7465  itCommandTest.te
+00000fb0: 7374 5f73 7562 6d69 745f 696e 7661 6c69  st_submit_invali
+00000fc0: 645f 7265 7375 6c74 5f76 616c 7565 6301  d_result_valuec.
+00000fd0: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
+00000fe0: 0000 0073 9400 0000 7c00 6a00 6401 6402  ...s....|.j.d.d.
+00000ff0: 8d01 7d01 7c00 6a01 7c01 6a02 8301 0100  ..}.|.j.|.j.....
+00001000: 7c00 6a03 6403 7c01 6a04 8302 0100 7405  |.j.d.|.j.....t.
+00001010: 7c00 6a06 6a07 6404 6405 8d01 8301 7d02  |.j.j.d.d.....}.
+00001020: 7c00 6a08 6404 7c02 6a09 8302 0100 7c00  |.j.d.|.j.....|.
+00001030: 6a08 6406 7c02 6a0a 8302 0100 7405 7c00  j.d.|.j.....t.|.
+00001040: 6a06 6a07 6407 6405 8d01 8301 7d02 7c00  j.j.d.d.....}.|.
+00001050: 6a08 6407 7c02 6a09 8302 0100 7c00 6a08  j.d.|.j.....|.j.
+00001060: 6408 7c02 6a0a 8302 0100 7c00 6a08 6409  d.|.j.....|.j.d.
+00001070: 7c02 6a0b 8302 0100 6400 5300 290a 4e7a  |.j.....d.S.).Nz
+00001080: 2874 6573 7473 2f73 7562 6d69 745f 7265  (tests/submit_re
+00001090: 7375 6c74 732f 7361 6d70 6c65 5f72 6573  sults/sample_res
+000010a0: 756c 7473 2e6a 736f 6e29 0172 3900 0000  ults.json).r9...
+000010b0: 7a07 3220 7465 7374 737a 0b6a 736f 6e2d  z.2 testsz.json-
+000010c0: 7465 7374 2d31 2901 7222 0000 0072 0e00  test-1).r"...r..
+000010d0: 0000 7a0b 6a73 6f6e 2d74 6573 742d 3272  ..z.json-test-2r
+000010e0: 0f00 0000 7a0f 6a73 6f6e 2d74 6573 742d  ....z.json-test-
+000010f0: 3220 6c6f 6729 0c72 5c00 0000 7232 0000  2 log).r\...r2..
+00001100: 0072 4900 0000 725e 0000 0072 5300 0000  .rI...r^...rS...
+00001110: 720d 0000 0072 1500 0000 7231 0000 0072  r....r....r1...r
+00001120: 3400 0000 7222 0000 0072 2900 0000 722a  4...r"...r)...r*
+00001130: 0000 0029 0372 1800 0000 725b 0000 0072  ...).r....r[...r
+00001140: 3700 0000 7219 0000 0072 1900 0000 721a  7...r....r....r.
+00001150: 0000 00da 1874 6573 745f 7375 626d 6974  .....test_submit
+00001160: 5f72 6573 756c 7473 5f6a 736f 6e82 0000  _results_json...
+00001170: 0073 1400 0000 0001 0c01 0c01 0e02 1201  .s..............
+00001180: 0e01 0e02 1201 0e01 0e01 7a2a 5375 626d  ..........z*Subm
+00001190: 6974 436f 6d6d 616e 6454 6573 742e 7465  itCommandTest.te
+000011a0: 7374 5f73 7562 6d69 745f 7265 7375 6c74  st_submit_result
+000011b0: 735f 6a73 6f6e 6301 0000 0000 0000 0002  s_jsonc.........
+000011c0: 0000 0003 0000 0043 0000 0073 2a00 0000  .......C...s*...
+000011d0: 7c00 6a00 6401 6402 8d01 7d01 7c00 6a01  |.j.d.d...}.|.j.
+000011e0: 7c01 6a02 8301 0100 7c00 6a03 6403 7c01  |.j.....|.j.d.|.
+000011f0: 6a04 8302 0100 6400 5300 2904 4e7a 3274  j.....d.S.).Nz2t
+00001200: 6573 7473 2f73 7562 6d69 745f 7265 7375  ests/submit_resu
+00001210: 6c74 732f 7361 6d70 6c65 5f72 6573 756c  lts/sample_resul
+00001220: 7473 5f6d 616c 666f 726d 6564 2e6a 736f  ts_malformed.jso
+00001230: 6e29 0172 3900 0000 7a13 4661 696c 6564  n).r9...z.Failed
+00001240: 2070 6172 7369 6e67 2066 696c 6529 0572   parsing file).r
+00001250: 5c00 0000 725d 0000 0072 4900 0000 725e  \...r]...rI...r^
+00001260: 0000 0072 5300 0000 2902 7218 0000 0072  ...rS...).r....r
+00001270: 5b00 0000 7219 0000 0072 1900 0000 721a  [...r....r....r.
+00001280: 0000 00da 2274 6573 745f 7375 626d 6974  ...."test_submit
+00001290: 5f72 6573 756c 7473 5f6d 616c 666f 726d  _results_malform
+000012a0: 6564 5f6a 736f 6e90 0000 0073 0600 0000  ed_json....s....
+000012b0: 0001 0c01 0c01 7a34 5375 626d 6974 436f  ......z4SubmitCo
+000012c0: 6d6d 616e 6454 6573 742e 7465 7374 5f73  mmandTest.test_s
+000012d0: 7562 6d69 745f 7265 7375 6c74 735f 6d61  ubmit_results_ma
+000012e0: 6c66 6f72 6d65 645f 6a73 6f6e 6301 0000  lformed_jsonc...
+000012f0: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+00001300: 0073 8e00 0000 7c00 6a00 6401 6402 6403  .s....|.j.d.d.d.
+00001310: 8d02 7d01 7c00 6a01 7c01 6a02 7c01 6a03  ..}.|.j.|.j.|.j.
+00001320: 6404 8d02 0100 7c00 6a04 6405 7c01 6a03  d.....|.j.d.|.j.
+00001330: 8302 0100 7405 7c00 6a06 6a07 6406 6407  ....t.|.j.j.d.d.
+00001340: 8d01 8301 7d02 7c00 6a08 6408 7c02 6a09  ....}.|.j.d.|.j.
+00001350: 8302 0100 7c00 6a08 6409 7c02 6a0a 8302  ....|.j.d.|.j...
+00001360: 0100 7405 7c00 6a06 6a07 640a 6407 8d01  ..t.|.j.j.d.d...
+00001370: 8301 7d02 7c00 6a08 640b 7c02 6a09 8302  ..}.|.j.d.|.j...
+00001380: 0100 7c00 6a08 640c 7c02 6a0a 8302 0100  ..|.j.d.|.j.....
+00001390: 6400 5300 290d 4e7a 2574 6573 7473 2f64  d.S.).Nz%tests/d
+000013a0: 6174 612f 7375 626d 6974 2f74 7578 6275  ata/submit/tuxbu
+000013b0: 696c 642f 6275 696c 642e 6a73 6f6e da0d  ild/build.json..
+000013c0: 7475 7862 7569 6c64 5f6a 736f 6e29 0272  tuxbuild_json).r
+000013d0: 3900 0000 7254 0000 0029 01da 036d 7367  9...rT...)...msg
+000013e0: 7a12 5375 626d 6974 7469 6e67 2032 2074  z.Submitting 2 t
+000013f0: 6573 7473 7a18 6763 632d 392d 6465 6663  estsz.gcc-9-defc
+00001400: 6f6e 6669 672d 6239 3937 3963 6661 2901  onfig-b9979cfa).
+00001410: 7222 0000 007a 1e62 7569 6c64 2f67 6363  r"...z.build/gcc
+00001420: 2d39 2d64 6566 636f 6e66 6967 2d62 3939  -9-defconfig-b99
+00001430: 3739 6366 6172 0e00 0000 7a18 6763 632d  79cfar....z.gcc-
+00001440: 392d 6465 6663 6f6e 6669 672d 3562 3039  9-defconfig-5b09
+00001450: 3536 3865 7a1e 6275 696c 642f 6763 632d  568ez.build/gcc-
+00001460: 392d 6465 6663 6f6e 6669 672d 3562 3039  9-defconfig-5b09
+00001470: 3536 3865 720f 0000 0029 0b72 5c00 0000  568er....).r\...
+00001480: 7232 0000 0072 4900 0000 7253 0000 0072  r2...rI...rS...r
+00001490: 5e00 0000 720d 0000 0072 1500 0000 7231  ^...r....r....r1
+000014a0: 0000 0072 3400 0000 7222 0000 0072 2900  ...r4...r"...r).
+000014b0: 0000 2903 7218 0000 0072 5b00 0000 7237  ..).r....r[...r7
+000014c0: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+000014d0: 0000 da21 7465 7374 5f73 7562 6d69 745f  ...!test_submit_
+000014e0: 7265 7375 6c74 735f 7475 7862 7569 6c64  results_tuxbuild
+000014f0: 5f6a 736f 6e95 0000 0073 1200 0000 0001  _json....s......
+00001500: 0e01 1201 0e02 1201 0e01 0e02 1201 0e01  ................
+00001510: 7a33 5375 626d 6974 436f 6d6d 616e 6454  z3SubmitCommandT
+00001520: 6573 742e 7465 7374 5f73 7562 6d69 745f  est.test_submit_
+00001530: 7265 7375 6c74 735f 7475 7862 7569 6c64  results_tuxbuild
+00001540: 5f6a 736f 6e63 0100 0000 0000 0000 0300  _jsonc..........
+00001550: 0000 0400 0000 4300 0000 73aa 0000 007c  ......C...s....|
+00001560: 006a 0064 0164 0264 038d 027d 017c 006a  .j.d.d.d...}.|.j
+00001570: 0164 047c 016a 0283 0201 0074 037c 006a  .d.|.j.....t.|.j
+00001580: 046a 0564 0564 068d 0183 017d 027c 006a  .j.d.d.....}.|.j
+00001590: 0664 077c 026a 0783 0201 007c 006a 0664  .d.|.j.....|.j.d
+000015a0: 087c 026a 0883 0201 0074 037c 006a 046a  .|.j.....t.|.j.j
+000015b0: 0564 0964 068d 0183 017d 027c 006a 0664  .d.d.....}.|.j.d
+000015c0: 0a7c 026a 0783 0201 007c 006a 0664 087c  .|.j.....|.j.d.|
+000015d0: 026a 0883 0201 0074 037c 006a 046a 0564  .j.....t.|.j.j.d
+000015e0: 0b64 068d 0183 017d 027c 006a 0664 0c7c  .d.....}.|.j.d.|
+000015f0: 026a 0783 0201 007c 006a 0664 087c 026a  .j.....|.j.d.|.j
+00001600: 0883 0201 0064 0053 0029 0d4e 7a28 7465  .....d.S.).Nz(te
+00001610: 7374 732f 6461 7461 2f73 7562 6d69 742f  sts/data/submit/
+00001620: 7475 7862 7569 6c64 2f62 7569 6c64 7365  tuxbuild/buildse
+00001630: 742e 6a73 6f6e 7264 0000 0029 0272 3900  t.jsonrd...).r9.
+00001640: 0000 7254 0000 007a 1253 7562 6d69 7474  ..rT...z.Submitt
+00001650: 696e 6720 3320 7465 7374 737a 1167 6363  ing 3 testsz.gcc
+00001660: 2d38 2d61 6c6c 6e6f 636f 6e66 6967 2901  -8-allnoconfig).
+00001670: 7222 0000 007a 1762 7569 6c64 2f67 6363  r"...z.build/gcc
+00001680: 2d38 2d61 6c6c 6e6f 636f 6e66 6967 720e  -8-allnoconfigr.
+00001690: 0000 007a 1067 6363 2d38 2d74 696e 7963  ...z.gcc-8-tinyc
+000016a0: 6f6e 6669 677a 1662 7569 6c64 2f67 6363  onfigz.build/gcc
+000016b0: 2d38 2d74 696e 7963 6f6e 6669 677a 1667  -8-tinyconfigz.g
+000016c0: 6363 2d38 2d78 3836 5f36 345f 6465 6663  cc-8-x86_64_defc
+000016d0: 6f6e 6669 677a 1c62 7569 6c64 2f67 6363  onfigz.build/gcc
+000016e0: 2d38 2d78 3836 5f36 345f 6465 6663 6f6e  -8-x86_64_defcon
+000016f0: 6669 6729 0972 5c00 0000 725e 0000 0072  fig).r\...r^...r
+00001700: 5300 0000 720d 0000 0072 1500 0000 7231  S...r....r....r1
+00001710: 0000 0072 3400 0000 7222 0000 0072 2900  ...r4...r"...r).
+00001720: 0000 2903 7218 0000 0072 5b00 0000 7237  ..).r....r[...r7
+00001730: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00001740: 0000 da2a 7465 7374 5f73 7562 6d69 745f  ...*test_submit_
+00001750: 7265 7375 6c74 735f 7475 7862 7569 6c64  results_tuxbuild
+00001760: 5f62 7569 6c64 7365 745f 6a73 6f6e a200  _buildset_json..
+00001770: 0000 7316 0000 0000 010e 010e 0212 010e  ..s.............
+00001780: 010e 0212 010e 010e 0212 010e 017a 3c53  .............z<S
+00001790: 7562 6d69 7443 6f6d 6d61 6e64 5465 7374  ubmitCommandTest
+000017a0: 2e74 6573 745f 7375 626d 6974 5f72 6573  .test_submit_res
+000017b0: 756c 7473 5f74 7578 6275 696c 645f 6275  ults_tuxbuild_bu
+000017c0: 696c 6473 6574 5f6a 736f 6e63 0100 0000  ildset_jsonc....
+000017d0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+000017e0: 7332 0000 007c 006a 0064 0164 0264 038d  s2...|.j.d.d.d..
+000017f0: 027d 017c 006a 017c 016a 027c 016a 0364  .}.|.j.|.j.|.j.d
+00001800: 048d 0201 007c 006a 0464 057c 016a 0383  .....|.j.d.|.j..
+00001810: 0201 0064 0053 0029 064e 7a29 7465 7374  ...d.S.).Nz)test
+00001820: 732f 6461 7461 2f73 7562 6d69 742f 7475  s/data/submit/tu
+00001830: 7862 7569 6c64 2f6d 616c 666f 726d 6564  xbuild/malformed
+00001840: 2e6a 736f 6e72 6400 0000 2902 7239 0000  .jsonrd...).r9..
+00001850: 0072 5400 0000 2901 7265 0000 007a 1346  .rT...).re...z.F
+00001860: 6169 6c65 6420 746f 206c 6f61 6420 6a73  ailed to load js
+00001870: 6f6e 2905 725c 0000 0072 5d00 0000 7249  on).r\...r]...rI
+00001880: 0000 0072 5300 0000 725e 0000 0029 0272  ...rS...r^...).r
+00001890: 1800 0000 725b 0000 0072 1900 0000 7219  ....r[...r....r.
+000018a0: 0000 0072 1a00 0000 da2b 7465 7374 5f73  ...r.....+test_s
+000018b0: 7562 6d69 745f 7265 7375 6c74 735f 7475  ubmit_results_tu
+000018c0: 7862 7569 6c64 5f6a 736f 6e5f 6d61 6c66  xbuild_json_malf
+000018d0: 6f72 6d65 64b2 0000 0073 0600 0000 0001  ormed....s......
+000018e0: 0e01 1201 7a3d 5375 626d 6974 436f 6d6d  ....z=SubmitComm
+000018f0: 616e 6454 6573 742e 7465 7374 5f73 7562  andTest.test_sub
+00001900: 6d69 745f 7265 7375 6c74 735f 7475 7862  mit_results_tuxb
+00001910: 7569 6c64 5f6a 736f 6e5f 6d61 6c66 6f72  uild_json_malfor
+00001920: 6d65 6463 0100 0000 0000 0000 0200 0000  medc............
+00001930: 0400 0000 4300 0000 732c 0000 007c 006a  ....C...s,...|.j
+00001940: 0064 0164 0264 038d 027d 017c 006a 017c  .d.d.d...}.|.j.|
+00001950: 016a 0283 0101 007c 006a 0364 047c 016a  .j.....|.j.d.|.j
+00001960: 0483 0201 0064 0053 0029 054e 7a27 7465  .....d.S.).Nz'te
+00001970: 7374 732f 6461 7461 2f73 7562 6d69 742f  sts/data/submit/
+00001980: 7475 7862 7569 6c64 2f6d 6973 7369 6e67  tuxbuild/missing
+00001990: 2e6a 736f 6e72 6400 0000 2902 7239 0000  .jsonrd...).r9..
+000019a0: 0072 5400 0000 7a44 5265 7175 6573 7465  .rT...zDRequeste
+000019b0: 6420 6669 6c65 2074 6573 7473 2f64 6174  d file tests/dat
+000019c0: 612f 7375 626d 6974 2f74 7578 6275 696c  a/submit/tuxbuil
+000019d0: 642f 6d69 7373 696e 672e 6a73 6f6e 2064  d/missing.json d
+000019e0: 6f65 736e 2774 2065 7869 7374 2905 725c  oesn't exist).r\
+000019f0: 0000 0072 5d00 0000 7249 0000 0072 5e00  ...r]...rI...r^.
+00001a00: 0000 7253 0000 0029 0272 1800 0000 725b  ..rS...).r....r[
+00001a10: 0000 0072 1900 0000 7219 0000 0072 1a00  ...r....r....r..
+00001a20: 0000 da29 7465 7374 5f73 7562 6d69 745f  ...)test_submit_
+00001a30: 7265 7375 6c74 735f 7475 7862 7569 6c64  results_tuxbuild
+00001a40: 5f6a 736f 6e5f 6d69 7373 696e 67b7 0000  _json_missing...
+00001a50: 0073 0600 0000 0001 0e01 0c01 7a3b 5375  .s..........z;Su
+00001a60: 626d 6974 436f 6d6d 616e 6454 6573 742e  bmitCommandTest.
+00001a70: 7465 7374 5f73 7562 6d69 745f 7265 7375  test_submit_resu
+00001a80: 6c74 735f 7475 7862 7569 6c64 5f6a 736f  lts_tuxbuild_jso
+00001a90: 6e5f 6d69 7373 696e 6763 0100 0000 0000  n_missingc......
+00001aa0: 0000 0200 0000 0300 0000 4300 0000 732a  ..........C...s*
+00001ab0: 0000 007c 006a 0064 0164 028d 017d 017c  ...|.j.d.d...}.|
+00001ac0: 006a 017c 016a 0283 0101 007c 006a 0364  .j.|.j.....|.j.d
+00001ad0: 037c 016a 0483 0201 0064 0053 0029 044e  .|.j.....d.S.).N
+00001ae0: 7264 0000 0029 0172 5400 0000 7a3f 4174  rd...).rT...z?At
+00001af0: 206c 6561 7374 206f 6e65 206f 6620 2d2d   least one of --
+00001b00: 7265 7375 6c74 2d6e 616d 652c 202d 2d72  result-name, --r
+00001b10: 6573 756c 7473 2c20 2d2d 6d65 7472 6963  esults, --metric
+00001b20: 7320 6973 2072 6571 7569 7265 6429 0572  s is required).r
+00001b30: 5c00 0000 725d 0000 0072 4900 0000 725e  \...r]...rI...r^
+00001b40: 0000 0072 5300 0000 2902 7218 0000 0072  ...rS...).r....r
+00001b50: 5b00 0000 7219 0000 0072 1900 0000 721a  [...r....r....r.
+00001b60: 0000 00da 3574 6573 745f 7375 626d 6974  ....5test_submit
+00001b70: 5f72 6573 756c 7473 5f74 7578 6275 696c  _results_tuxbuil
+00001b80: 645f 6a73 6f6e 5f72 6573 756c 7473 5f6f  d_json_results_o
+00001b90: 7074 5f6d 6973 7369 6e67 bc00 0000 7306  pt_missing....s.
+00001ba0: 0000 0000 010c 010c 017a 4753 7562 6d69  .........zGSubmi
+00001bb0: 7443 6f6d 6d61 6e64 5465 7374 2e74 6573  tCommandTest.tes
+00001bc0: 745f 7375 626d 6974 5f72 6573 756c 7473  t_submit_results
+00001bd0: 5f74 7578 6275 696c 645f 6a73 6f6e 5f72  _tuxbuild_json_r
+00001be0: 6573 756c 7473 5f6f 7074 5f6d 6973 7369  esults_opt_missi
+00001bf0: 6e67 6301 0000 0000 0000 0002 0000 0004  ngc.............
+00001c00: 0000 0043 0000 0073 2c00 0000 7c00 6a00  ...C...s,...|.j.
+00001c10: 6401 6402 6403 8d02 7d01 7c00 6a01 7c01  d.d.d...}.|.j.|.
+00001c20: 6a02 8301 0100 7c00 6a03 6404 7c01 6a04  j.....|.j.d.|.j.
+00001c30: 8302 0100 6400 5300 2905 4e7a 2574 6573  ....d.S.).Nz%tes
+00001c40: 7473 2f64 6174 612f 7375 626d 6974 2f74  ts/data/submit/t
+00001c50: 7578 6275 696c 642f 6275 696c 642e 6a73  uxbuild/build.js
+00001c60: 6f6e 5a0a 6261 645f 6c61 796f 7574 2902  onZ.bad_layout).
+00001c70: 7239 0000 0072 5400 0000 7a37 6172 6775  r9...rT...z7argu
+00001c80: 6d65 6e74 202d 2d72 6573 756c 7473 2d6c  ment --results-l
+00001c90: 6179 6f75 743a 2069 6e76 616c 6964 2063  ayout: invalid c
+00001ca0: 686f 6963 653a 2027 6261 645f 6c61 796f  hoice: 'bad_layo
+00001cb0: 7574 2729 0572 5c00 0000 725d 0000 0072  ut').r\...r]...r
+00001cc0: 4900 0000 725e 0000 0072 5300 0000 2902  I...r^...rS...).
+00001cd0: 7218 0000 0072 5b00 0000 7219 0000 0072  r....r[...r....r
+00001ce0: 1900 0000 721a 0000 00da 3074 6573 745f  ....r.....0test_
+00001cf0: 7375 626d 6974 5f72 6573 756c 7473 5f74  submit_results_t
+00001d00: 7578 6275 696c 645f 6a73 6f6e 5f6c 6179  uxbuild_json_lay
+00001d10: 6f75 745f 6172 675f 6261 64c1 0000 0073  out_arg_bad....s
+00001d20: 0600 0000 0001 0e01 0c01 7a42 5375 626d  ..........zBSubm
+00001d30: 6974 436f 6d6d 616e 6454 6573 742e 7465  itCommandTest.te
+00001d40: 7374 5f73 7562 6d69 745f 7265 7375 6c74  st_submit_result
+00001d50: 735f 7475 7862 7569 6c64 5f6a 736f 6e5f  s_tuxbuild_json_
+00001d60: 6c61 796f 7574 5f61 7267 5f62 6164 6301  layout_arg_badc.
+00001d70: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00001d80: 0000 0073 2c00 0000 7c00 6a00 6401 6402  ...s,...|.j.d.d.
+00001d90: 6403 8d02 7d01 7c00 6a01 7c01 6a02 8301  d...}.|.j.|.j...
+00001da0: 0100 7c00 6a03 6404 7c01 6a04 8302 0100  ..|.j.d.|.j.....
+00001db0: 6400 5300 2905 4e7a 2d74 6573 7473 2f64  d.S.).Nz-tests/d
+00001dc0: 6174 612f 7375 626d 6974 2f74 7578 6275  ata/submit/tuxbu
+00001dd0: 696c 642f 656d 7074 795f 6b63 6f6e 6669  ild/empty_kconfi
+00001de0: 672e 6a73 6f6e 7264 0000 0029 0272 3900  g.jsonrd...).r9.
+00001df0: 0000 7254 0000 007a 5446 6169 6c65 6420  ..rT...zTFailed 
+00001e00: 746f 206c 6f61 6420 7475 7862 7569 6c64  to load tuxbuild
+00001e10: 206a 736f 6e20 6475 6520 746f 2061 206d   json due to a m
+00001e20: 6973 7369 6e67 206b 636f 6e66 6967 2076  issing kconfig v
+00001e30: 616c 7565 3a20 6c69 7374 2069 6e64 6578  alue: list index
+00001e40: 206f 7574 206f 6620 7261 6e67 6529 0572   out of range).r
+00001e50: 5c00 0000 725d 0000 0072 4900 0000 725e  \...r]...rI...r^
+00001e60: 0000 0072 5300 0000 2902 7218 0000 0072  ...rS...).r....r
+00001e70: 5b00 0000 7219 0000 0072 1900 0000 721a  [...r....r....r.
+00001e80: 0000 00da 2f74 6573 745f 7375 626d 6974  ..../test_submit
+00001e90: 5f72 6573 756c 7473 5f74 7578 6275 696c  _results_tuxbuil
+00001ea0: 645f 6a73 6f6e 5f65 6d70 7479 5f6b 636f  d_json_empty_kco
+00001eb0: 6e66 6967 c600 0000 7306 0000 0000 010e  nfig....s.......
+00001ec0: 010c 017a 4153 7562 6d69 7443 6f6d 6d61  ...zASubmitComma
+00001ed0: 6e64 5465 7374 2e74 6573 745f 7375 626d  ndTest.test_subm
+00001ee0: 6974 5f72 6573 756c 7473 5f74 7578 6275  it_results_tuxbu
+00001ef0: 696c 645f 6a73 6f6e 5f65 6d70 7479 5f6b  ild_json_empty_k
+00001f00: 636f 6e66 6967 6301 0000 0000 0000 0002  configc.........
+00001f10: 0000 0004 0000 0043 0000 0073 2c00 0000  .......C...s,...
+00001f20: 7c00 6a00 6401 6402 6403 8d02 7d01 7c00  |.j.d.d.d...}.|.
+00001f30: 6a01 7c01 6a02 8301 0100 7c00 6a03 6404  j.|.j.....|.j.d.
+00001f40: 7c01 6a04 8302 0100 6400 5300 2905 4e7a  |.j.....d.S.).Nz
+00001f50: 2f74 6573 7473 2f64 6174 612f 7375 626d  /tests/data/subm
+00001f60: 6974 2f74 7578 6275 696c 642f 6d69 7373  it/tuxbuild/miss
+00001f70: 696e 675f 6b63 6f6e 6669 672e 6a73 6f6e  ing_kconfig.json
+00001f80: 7264 0000 0029 0272 3900 0000 7254 0000  rd...).r9...rT..
+00001f90: 007a 4146 6169 6c65 6420 746f 206c 6f61  .zAFailed to loa
+00001fa0: 6420 7475 7862 7569 6c64 206a 736f 6e20  d tuxbuild json 
+00001fb0: 6475 6520 746f 2061 206d 6973 7369 6e67  due to a missing
+00001fc0: 2076 6172 6961 626c 653a 2027 6b63 6f6e   variable: 'kcon
+00001fd0: 6669 6727 2905 725c 0000 0072 5d00 0000  fig').r\...r]...
+00001fe0: 7249 0000 0072 5e00 0000 7253 0000 0029  rI...r^...rS...)
+00001ff0: 0272 1800 0000 725b 0000 0072 1900 0000  .r....r[...r....
+00002000: 7219 0000 0072 1a00 0000 da31 7465 7374  r....r.....1test
+00002010: 5f73 7562 6d69 745f 7265 7375 6c74 735f  _submit_results_
+00002020: 7475 7862 7569 6c64 5f6a 736f 6e5f 6d69  tuxbuild_json_mi
+00002030: 7373 696e 675f 6b63 6f6e 6669 67cb 0000  ssing_kconfig...
+00002040: 0073 0600 0000 0001 0e01 0c01 7a43 5375  .s..........zCSu
+00002050: 626d 6974 436f 6d6d 616e 6454 6573 742e  bmitCommandTest.
+00002060: 7465 7374 5f73 7562 6d69 745f 7265 7375  test_submit_resu
+00002070: 6c74 735f 7475 7862 7569 6c64 5f6a 736f  lts_tuxbuild_jso
+00002080: 6e5f 6d69 7373 696e 675f 6b63 6f6e 6669  n_missing_kconfi
+00002090: 6763 0100 0000 0000 0000 0300 0000 0400  gc..............
+000020a0: 0000 4300 0000 7394 0000 007c 006a 0064  ..C...s....|.j.d
+000020b0: 0164 028d 017d 017c 006a 017c 016a 0283  .d...}.|.j.|.j..
+000020c0: 0101 007c 006a 0364 037c 016a 0483 0201  ...|.j.d.|.j....
+000020d0: 0074 057c 006a 066a 0764 0464 058d 0183  .t.|.j.j.d.d....
+000020e0: 017d 027c 006a 0864 047c 026a 0983 0201  .}.|.j.d.|.j....
+000020f0: 007c 006a 0864 067c 026a 0a83 0201 0074  .|.j.d.|.j.....t
+00002100: 057c 006a 066a 0764 0764 058d 0183 017d  .|.j.j.d.d.....}
+00002110: 027c 006a 0864 077c 026a 0983 0201 007c  .|.j.d.|.j.....|
+00002120: 006a 0864 087c 026a 0a83 0201 007c 006a  .j.d.|.j.....|.j
+00002130: 0864 097c 026a 0b83 0201 0064 0053 0029  .d.|.j.....d.S.)
+00002140: 0a4e 7a28 7465 7374 732f 7375 626d 6974  .Nz(tests/submit
+00002150: 5f72 6573 756c 7473 2f73 616d 706c 655f  _results/sample_
+00002160: 7265 7375 6c74 732e 7961 6d6c 2901 7239  results.yaml).r9
+00002170: 0000 007a 0732 2074 6573 7473 7a0b 7961  ...z.2 testsz.ya
+00002180: 6d6c 2d74 6573 742d 3129 0172 2200 0000  ml-test-1).r"...
+00002190: 720e 0000 007a 0b79 616d 6c2d 7465 7374  r....z.yaml-test
+000021a0: 2d32 720f 0000 007a 0f79 616d 6c2d 7465  -2r....z.yaml-te
+000021b0: 7374 2d32 206c 6f67 290c 725c 0000 0072  st-2 log).r\...r
+000021c0: 3200 0000 7249 0000 0072 5e00 0000 7253  2...rI...r^...rS
+000021d0: 0000 0072 0d00 0000 7215 0000 0072 3100  ...r....r....r1.
+000021e0: 0000 7234 0000 0072 2200 0000 7229 0000  ..r4...r"...r)..
+000021f0: 0072 2a00 0000 2903 7218 0000 0072 5b00  .r*...).r....r[.
+00002200: 0000 7237 0000 0072 1900 0000 7219 0000  ..r7...r....r...
+00002210: 0072 1a00 0000 da18 7465 7374 5f73 7562  .r......test_sub
+00002220: 6d69 745f 7265 7375 6c74 735f 7961 6d6c  mit_results_yaml
+00002230: d000 0000 7314 0000 0000 010c 010c 010e  ....s...........
+00002240: 0212 010e 010e 0212 010e 010e 017a 2a53  .............z*S
+00002250: 7562 6d69 7443 6f6d 6d61 6e64 5465 7374  ubmitCommandTest
+00002260: 2e74 6573 745f 7375 626d 6974 5f72 6573  .test_submit_res
+00002270: 756c 7473 5f79 616d 6c63 0100 0000 0000  ults_yamlc......
+00002280: 0000 0200 0000 0300 0000 4300 0000 732a  ..........C...s*
+00002290: 0000 007c 006a 0064 0164 028d 017d 017c  ...|.j.d.d...}.|
+000022a0: 006a 017c 016a 0283 0101 007c 006a 0364  .j.|.j.....|.j.d
+000022b0: 037c 016a 0483 0201 0064 0053 0029 044e  .|.j.....d.S.).N
+000022c0: 7a32 7465 7374 732f 7375 626d 6974 5f72  z2tests/submit_r
+000022d0: 6573 756c 7473 2f73 616d 706c 655f 7265  esults/sample_re
+000022e0: 7375 6c74 735f 6d61 6c66 6f72 6d65 642e  sults_malformed.
+000022f0: 7961 6d6c 2901 7239 0000 007a 1346 6169  yaml).r9...z.Fai
+00002300: 6c65 6420 7061 7273 696e 6720 6669 6c65  led parsing file
+00002310: 2905 725c 0000 0072 5d00 0000 7249 0000  ).r\...r]...rI..
+00002320: 0072 5e00 0000 7253 0000 0029 0272 1800  .r^...rS...).r..
+00002330: 0000 725b 0000 0072 1900 0000 7219 0000  ..r[...r....r...
+00002340: 0072 1a00 0000 da22 7465 7374 5f73 7562  .r....."test_sub
+00002350: 6d69 745f 7265 7375 6c74 735f 6d61 6c66  mit_results_malf
+00002360: 6f72 6d65 645f 7961 6d6c de00 0000 7306  ormed_yaml....s.
+00002370: 0000 0000 010c 010c 017a 3453 7562 6d69  .........z4Submi
+00002380: 7443 6f6d 6d61 6e64 5465 7374 2e74 6573  tCommandTest.tes
+00002390: 745f 7375 626d 6974 5f72 6573 756c 7473  t_submit_results
+000023a0: 5f6d 616c 666f 726d 6564 5f79 616d 6c63  _malformed_yamlc
+000023b0: 0100 0000 0000 0000 0300 0000 0300 0000  ................
+000023c0: 4300 0000 7332 0000 0064 017d 017c 006a  C...s2...d.}.|.j
+000023d0: 007c 0164 028d 017d 027c 006a 017c 026a  .|.d...}.|.j.|.j
+000023e0: 0283 0101 007c 006a 0364 037c 0116 007c  .....|.j.d.|...|
+000023f0: 026a 0483 0201 0064 0053 0029 044e 7a27  .j.....d.S.).Nz'
+00002400: 7465 7374 732f 7375 626d 6974 5f72 6573  tests/submit_res
+00002410: 756c 7473 2f73 616d 706c 655f 7265 7375  ults/sample_resu
+00002420: 6c74 732e 7478 7429 0172 3900 0000 7a35  lts.txt).r9...z5
+00002430: 4669 6c65 2022 2573 2220 646f 6573 206e  File "%s" does n
+00002440: 6f74 2068 6176 6520 6120 4a53 4f4e 206f  ot have a JSON o
+00002450: 7220 5941 4d4c 2066 696c 6520 6578 7465  r YAML file exte
+00002460: 6e73 696f 6e29 0572 5c00 0000 725d 0000  nsion).r\...r]..
+00002470: 0072 4900 0000 725e 0000 0072 5300 0000  .rI...r^...rS...
+00002480: 2903 7218 0000 00da 0170 725b 0000 0072  ).r......pr[...r
+00002490: 1900 0000 7219 0000 0072 1a00 0000 da21  ....r....r.....!
+000024a0: 7465 7374 5f73 7562 6d69 745f 7265 7375  test_submit_resu
+000024b0: 6c74 735f 6261 645f 6578 7465 6e73 696f  lts_bad_extensio
+000024c0: 6ee3 0000 0073 0800 0000 0001 0401 0c01  n....s..........
+000024d0: 0c01 7a33 5375 626d 6974 436f 6d6d 616e  ..z3SubmitComman
+000024e0: 6454 6573 742e 7465 7374 5f73 7562 6d69  dTest.test_submi
+000024f0: 745f 7265 7375 6c74 735f 6261 645f 6578  t_results_bad_ex
+00002500: 7465 6e73 696f 6e63 0100 0000 0000 0000  tensionc........
+00002510: 0200 0000 0300 0000 4300 0000 732a 0000  ........C...s*..
+00002520: 007c 006a 0064 0164 028d 017d 017c 006a  .|.j.d.d...}.|.j
+00002530: 017c 016a 0283 0101 007c 006a 0364 037c  .|.j.....|.j.d.|
+00002540: 016a 0483 0201 0064 0053 0029 044e 7a28  .j.....d.S.).Nz(
+00002550: 7465 7374 732f 7375 626d 6974 5f72 6573  tests/submit_res
+00002560: 756c 7473 2f73 616d 706c 655f 6d65 7472  ults/sample_metr
+00002570: 6963 732e 6a73 6f6e 2901 7257 0000 007a  ics.json).rW...z
+00002580: 0931 206d 6574 7269 6373 2905 725c 0000  .1 metrics).r\..
+00002590: 0072 3200 0000 7249 0000 0072 5e00 0000  .r2...rI...r^...
+000025a0: 7253 0000 0029 0272 1800 0000 725b 0000  rS...).r....r[..
+000025b0: 0072 1900 0000 7219 0000 0072 1a00 0000  .r....r....r....
+000025c0: da19 7465 7374 5f73 7562 6d69 745f 7369  ..test_submit_si
+000025d0: 6e67 6c65 5f6d 6574 7269 63e9 0000 0073  ngle_metric....s
+000025e0: 0600 0000 0001 0c01 0c01 7a2b 5375 626d  ..........z+Subm
+000025f0: 6974 436f 6d6d 616e 6454 6573 742e 7465  itCommandTest.te
+00002600: 7374 5f73 7562 6d69 745f 7369 6e67 6c65  st_submit_single
+00002610: 5f6d 6574 7269 6363 0100 0000 0000 0000  _metricc........
+00002620: 0300 0000 0600 0000 4300 0000 737e 0000  ........C...s~..
+00002630: 007c 006a 0064 0164 0264 0364 0464 058d  .|.j.d.d.d.d.d..
+00002640: 047d 017c 006a 017c 016a 027c 016a 0364  .}.|.j.|.j.|.j.d
+00002650: 068d 0201 007c 006a 0464 077c 016a 0383  .....|.j.d.|.j..
+00002660: 0201 0074 057c 006a 066a 0764 0864 098d  ...t.|.j.j.d.d..
+00002670: 0183 017d 027c 006a 0864 087c 026a 0983  ...}.|.j.d.|.j..
+00002680: 0201 007c 006a 0864 0a74 0a7c 026a 0b83  ...|.j.d.t.|.j..
+00002690: 0083 0183 0201 007c 006a 0864 0b74 0a7c  .......|.j.d.t.|
+000026a0: 026a 0c83 0083 0183 0201 0064 0053 0029  .j.........d.S.)
+000026b0: 0c4e 7a28 7465 7374 732f 7375 626d 6974  .Nz(tests/submit
+000026c0: 5f72 6573 756c 7473 2f73 616d 706c 655f  _results/sample_
+000026d0: 7265 7375 6c74 732e 6a73 6f6e 7a28 7465  results.jsonz(te
+000026e0: 7374 732f 7375 626d 6974 5f72 6573 756c  sts/submit_resul
+000026f0: 7473 2f73 616d 706c 655f 6d65 7472 6963  ts/sample_metric
+00002700: 732e 6a73 6f6e 7a29 7465 7374 732f 7375  s.jsonz)tests/su
+00002710: 626d 6974 5f72 6573 756c 7473 2f73 616d  bmit_results/sam
+00002720: 706c 655f 6d65 7461 6461 7461 2e6a 736f  ple_metadata.jso
+00002730: 6e7a 2374 6573 7473 2f73 7562 6d69 745f  nz#tests/submit_
+00002740: 7265 7375 6c74 732f 7361 6d70 6c65 5f6c  results/sample_l
+00002750: 6f67 2e6c 6f67 2904 7239 0000 0072 5700  og.log).r9...rW.
+00002760: 0000 722f 0000 0072 5900 0000 2901 7265  ..r/...rY...).re
+00002770: 0000 007a 1232 2074 6573 7473 2c20 3120  ...z.2 tests, 1 
+00002780: 6d65 7472 6963 735a 126a 736f 6e6d 6574  metricsZ.jsonmet
+00002790: 6164 6174 616a 6f62 6964 3129 0172 2100  adatajobid1).r!.
+000027a0: 0000 e902 0000 0072 0200 0000 290d 725c  .......r....).r\
+000027b0: 0000 0072 3200 0000 7249 0000 0072 5300  ...r2...rI...rS.
+000027c0: 0000 725e 0000 0072 0d00 0000 7215 0000  ..r^...r....r...
+000027d0: 00da 0874 6573 7472 756e 7372 3400 0000  ...testrunsr4...
+000027e0: 7221 0000 0072 3300 0000 7231 0000 0072  r!...r3...r1...r
+000027f0: 5700 0000 2903 7218 0000 0072 5b00 0000  W...).r....r[...
+00002800: 7236 0000 0072 1900 0000 7219 0000 0072  r6...r....r....r
+00002810: 1a00 0000 da16 7465 7374 5f73 7562 6d69  ......test_submi
+00002820: 745f 6576 6572 7974 6869 6e67 ee00 0000  t_everything....
+00002830: 7314 0000 0000 0106 0102 0102 0108 0112  s...............
+00002840: 010e 0212 010e 0214 017a 2853 7562 6d69  .........z(Submi
+00002850: 7443 6f6d 6d61 6e64 5465 7374 2e74 6573  tCommandTest.tes
+00002860: 745f 7375 626d 6974 5f65 7665 7279 7468  t_submit_everyth
+00002870: 696e 6729 094e 4e4e 4e4e 4e4e 4e4e 291b  ing).NNNNNNNNN).
+00002880: 723c 0000 0072 3d00 0000 723e 0000 0072  r<...r=...r>...r
+00002890: 0300 0000 7217 0000 0072 4000 0000 7241  ....r....r@...rA
+000028a0: 0000 0072 1b00 0000 725c 0000 0072 5f00  ...r....r\...r_.
+000028b0: 0000 7260 0000 0072 6100 0000 7262 0000  ..r`...ra...rb..
+000028c0: 0072 6300 0000 7266 0000 0072 6700 0000  .rc...rf...rg...
+000028d0: 7268 0000 0072 6900 0000 726a 0000 0072  rh...ri...rj...r
+000028e0: 6b00 0000 726c 0000 0072 6d00 0000 726e  k...rl...rm...rn
+000028f0: 0000 0072 6f00 0000 7271 0000 0072 7200  ...ro...rq...rr.
+00002900: 0000 7275 0000 0072 1900 0000 7219 0000  ..ru...r....r...
+00002910: 0072 1900 0000 721a 0000 0072 3f00 0000  .r....r....r?...
+00002920: 4100 0000 732e 0000 0008 020a 0104 0208  A...s...........
+00002930: 0400 010a 2408 0508 0908 0508 0e08 0508  ....$...........
+00002940: 0d08 1008 0508 0508 0508 0508 0508 0508  ................
+00002950: 0e08 0508 0608 0572 3f00 0000 2919 da08  .......r?...)...
+00002960: 756e 6974 7465 7374 da0a 7375 6270 726f  unittest..subpro
+00002970: 6365 7373 7246 0000 00da 0072 0300 0000  cessrF.....r....
+00002980: da15 7371 7561 645f 636c 6965 6e74 2e63  ..squad_client.c
+00002990: 6f72 652e 6170 6972 0400 0000 da18 7371  ore.apir......sq
+000029a0: 7561 645f 636c 6965 6e74 2e63 6f72 652e  uad_client.core.
+000029b0: 6d6f 6465 6c73 7205 0000 0072 0600 0000  modelsr....r....
+000029c0: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+000029d0: 0a00 0000 720b 0000 0072 0c00 0000 da12  ....r....r......
+000029e0: 7371 7561 645f 636c 6965 6e74 2e75 7469  squad_client.uti
+000029f0: 6c73 720d 0000 0072 2800 0000 da04 4641  lsr....r(.....FA
+00002a00: 494c 5a05 5846 4149 4c5a 0453 4b49 50da  ILZ.XFAILZ.SKIP.
+00002a10: 0854 6573 7443 6173 6572 1100 0000 723f  .TestCaser....r?
+00002a20: 0000 0072 1900 0000 7219 0000 0072 1900  ...r....r....r..
+00002a30: 0000 721a 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00002a40: 3e01 0000 0073 1600 0000 0801 0802 0c01  >....s..........
+00002a50: 0c01 2801 0c03 0401 0401 0401 0403 1231  ..(............1
```

### Comparing `squad-client-0.9/tests/squad_service.py` & `squad-client-0.9.1/tests/squad_service.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/test_submit.py` & `squad-client-0.9.1/tests/test_submit.py`

 * *Files 10% similar despite different names*

```diff
@@ -147,22 +147,38 @@
         self.assertIn('Failed parsing file', proc.err)
 
     def test_submit_results_tuxbuild_json(self):
         proc = self.manage_submit(results='tests/data/submit/tuxbuild/build.json', results_layout='tuxbuild_json')
         self.assertTrue(proc.ok, msg=proc.err)
         self.assertIn("Submitting 2 tests", proc.err)
 
-        test = first(self.squad.tests(name="x86-gcc-9-defconfig-b9979cfa"))
-        self.assertEqual("build/x86-gcc-9-defconfig-b9979cfa", test.name)
+        test = first(self.squad.tests(name="gcc-9-defconfig-b9979cfa"))
+        self.assertEqual("build/gcc-9-defconfig-b9979cfa", test.name)
         self.assertEqual("pass", test.status)
 
-        test = first(self.squad.tests(name="arm64-gcc-9-defconfig-5b09568e"))
-        self.assertEqual("build/arm64-gcc-9-defconfig-5b09568e", test.name)
+        test = first(self.squad.tests(name="gcc-9-defconfig-5b09568e"))
+        self.assertEqual("build/gcc-9-defconfig-5b09568e", test.name)
         self.assertEqual("fail", test.status)
 
+    def test_submit_results_tuxbuild_buildset_json(self):
+        proc = self.manage_submit(results='tests/data/submit/tuxbuild/buildset.json', results_layout='tuxbuild_json')
+        self.assertIn("Submitting 3 tests", proc.err)
+
+        test = first(self.squad.tests(name="gcc-8-allnoconfig"))
+        self.assertEqual("build/gcc-8-allnoconfig", test.name)
+        self.assertEqual("pass", test.status)
+
+        test = first(self.squad.tests(name="gcc-8-tinyconfig"))
+        self.assertEqual("build/gcc-8-tinyconfig", test.name)
+        self.assertEqual("pass", test.status)
+
+        test = first(self.squad.tests(name="gcc-8-x86_64_defconfig"))
+        self.assertEqual("build/gcc-8-x86_64_defconfig", test.name)
+        self.assertEqual("pass", test.status)
+
     def test_submit_results_tuxbuild_json_malformed(self):
         proc = self.manage_submit(results='tests/data/submit/tuxbuild/malformed.json', results_layout='tuxbuild_json')
         self.assertFalse(proc.ok, msg=proc.err)
         self.assertIn("Failed to load json", proc.err)
 
     def test_submit_results_tuxbuild_json_missing(self):
         proc = self.manage_submit(results="tests/data/submit/tuxbuild/missing.json", results_layout="tuxbuild_json")
@@ -175,14 +191,24 @@
         self.assertIn("At least one of --result-name, --results, --metrics is required", proc.err)
 
     def test_submit_results_tuxbuild_json_layout_arg_bad(self):
         proc = self.manage_submit(results="tests/data/submit/tuxbuild/build.json", results_layout="bad_layout")
         self.assertFalse(proc.ok)
         self.assertIn("argument --results-layout: invalid choice: 'bad_layout'", proc.err)
 
+    def test_submit_results_tuxbuild_json_empty_kconfig(self):
+        proc = self.manage_submit(results="tests/data/submit/tuxbuild/empty_kconfig.json", results_layout="tuxbuild_json")
+        self.assertFalse(proc.ok)
+        self.assertIn("Failed to load tuxbuild json due to a missing kconfig value: list index out of range", proc.err)
+
+    def test_submit_results_tuxbuild_json_missing_kconfig(self):
+        proc = self.manage_submit(results="tests/data/submit/tuxbuild/missing_kconfig.json", results_layout="tuxbuild_json")
+        self.assertFalse(proc.ok)
+        self.assertIn("Failed to load tuxbuild json due to a missing variable: 'kconfig'", proc.err)
+
     def test_submit_results_yaml(self):
         proc = self.manage_submit(results='tests/submit_results/sample_results.yaml')
         self.assertTrue(proc.ok)
         self.assertIn('2 tests', proc.err)
 
         test = first(self.squad.tests(name='yaml-test-1'))
         self.assertEqual('yaml-test-1', test.name)
```

### Comparing `squad-client-0.9/tests/test_api.py` & `squad-client-0.9.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/test_models.py` & `squad-client-0.9.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/tests/squad.sqlite3` & `squad-client-0.9.1/tests/squad.sqlite3`

 * *Files 18% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -1,201 +1,201 @@
 PRAGMA foreign_keys=OFF;
 BEGIN TRANSACTION;
 CREATE TABLE IF NOT EXISTS "django_migrations" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "app" varchar(255) NOT NULL, "name" varchar(255) NOT NULL, "applied" datetime NOT NULL);
-INSERT INTO django_migrations VALUES(1,'contenttypes','0001_initial','2020-10-29 19:53:48.306528');
-INSERT INTO django_migrations VALUES(2,'auth','0001_initial','2020-10-29 19:53:48.319951');
-INSERT INTO django_migrations VALUES(3,'admin','0001_initial','2020-10-29 19:53:48.330034');
-INSERT INTO django_migrations VALUES(4,'admin','0002_logentry_remove_auto_add','2020-10-29 19:53:48.339957');
-INSERT INTO django_migrations VALUES(5,'admin','0003_logentry_add_action_flag_choices','2020-10-29 19:53:48.349600');
-INSERT INTO django_migrations VALUES(6,'contenttypes','0002_remove_content_type_name','2020-10-29 19:53:48.364216');
-INSERT INTO django_migrations VALUES(7,'auth','0002_alter_permission_name_max_length','2020-10-29 19:53:48.369625');
-INSERT INTO django_migrations VALUES(8,'auth','0003_alter_user_email_max_length','2020-10-29 19:53:48.378200');
-INSERT INTO django_migrations VALUES(9,'auth','0004_alter_user_username_opts','2020-10-29 19:53:48.386218');
-INSERT INTO django_migrations VALUES(10,'auth','0005_alter_user_last_login_null','2020-10-29 19:53:48.393734');
-INSERT INTO django_migrations VALUES(11,'auth','0006_require_contenttypes_0002','2020-10-29 19:53:48.395673');
-INSERT INTO django_migrations VALUES(12,'auth','0007_alter_validators_add_error_messages','2020-10-29 19:53:48.403172');
-INSERT INTO django_migrations VALUES(13,'auth','0008_alter_user_username_max_length','2020-10-29 19:53:48.410792');
-INSERT INTO django_migrations VALUES(14,'auth','0009_alter_user_last_name_max_length','2020-10-29 19:53:48.418323');
-INSERT INTO django_migrations VALUES(15,'auth','0010_alter_group_name_max_length','2020-10-29 19:53:48.425621');
-INSERT INTO django_migrations VALUES(16,'auth','0011_update_proxy_permissions','2020-10-29 19:53:48.433172');
-INSERT INTO django_migrations VALUES(17,'authtoken','0001_initial','2020-10-29 19:53:48.463178');
-INSERT INTO django_migrations VALUES(18,'authtoken','0002_auto_20160226_1747','2020-10-29 19:53:48.484279');
-INSERT INTO django_migrations VALUES(19,'authtoken','0003_tokenproxy','2020-10-29 19:53:48.488554');
-INSERT INTO django_migrations VALUES(20,'core','0001_initial','2020-10-29 19:53:48.540285');
-INSERT INTO django_migrations VALUES(21,'core','0002_auto_20160525_1403','2020-10-29 19:53:48.554865');
-INSERT INTO django_migrations VALUES(22,'core','0003_testrun_log_file','2020-10-29 19:53:48.563139');
-INSERT INTO django_migrations VALUES(23,'core','0004_group_user_groups','2020-10-29 19:53:48.574059');
-INSERT INTO django_migrations VALUES(24,'core','0005_token','2020-10-29 19:53:48.587508');
-INSERT INTO django_migrations VALUES(25,'core','0006_auto_20160826_2242','2020-10-29 19:53:48.603711');
-INSERT INTO django_migrations VALUES(26,'core','0007_testrun_data_processed','2020-10-29 19:53:48.612431');
-INSERT INTO django_migrations VALUES(27,'core','0008_status','2020-10-29 19:53:48.629257');
-INSERT INTO django_migrations VALUES(28,'core','0009_testrun_status_recorded','2020-10-29 19:53:48.638078');
-INSERT INTO django_migrations VALUES(29,'core','0010_testrun_datetime','2020-10-29 19:53:48.655766');
-INSERT INTO django_migrations VALUES(30,'core','0011_testrun_metadata_fields','2020-10-29 19:53:48.682988');
-INSERT INTO django_migrations VALUES(31,'core','0012_build_datetime','2020-10-29 19:53:48.697220');
-INSERT INTO django_migrations VALUES(32,'core','0013_testrun_resubmit_url','2020-10-29 19:53:48.714234');
-INSERT INTO django_migrations VALUES(33,'core','0014_testrun_metadata_file','2020-10-29 19:53:48.724604');
-INSERT INTO django_migrations VALUES(34,'core','0015_attachment','2020-10-29 19:53:48.736296');
-INSERT INTO django_migrations VALUES(35,'core','0016_project_is_public','2020-10-29 19:53:48.744519');
-INSERT INTO django_migrations VALUES(36,'core','0017_slug_validator','2020-10-29 19:53:48.765672');
-INSERT INTO django_migrations VALUES(37,'core','0018_build_name','2020-10-29 19:53:48.775183');
-INSERT INTO django_migrations VALUES(38,'core','0019_build_version','2020-10-29 19:53:48.781850');
-INSERT INTO django_migrations VALUES(39,'core','0020_build_ordering','2020-10-29 19:53:48.793897');
-INSERT INTO django_migrations VALUES(40,'core','0021_global_tokens','2020-10-29 19:53:48.812199');
-INSERT INTO django_migrations VALUES(41,'core','0022_projectstatus','2020-10-29 19:53:48.824294');
-INSERT INTO django_migrations VALUES(42,'core','0023_subscription','2020-10-29 19:53:48.837820');
-INSERT INTO django_migrations VALUES(43,'core','0024_project_build_completion_threshold','2020-10-29 19:53:48.847882');
-INSERT INTO django_migrations VALUES(44,'core','0025_unique_testrun_job_id','2020-10-29 19:53:48.853955');
-INSERT INTO django_migrations VALUES(45,'core','0026_testrun_result_accept_null','2020-10-29 19:53:48.864984');
-INSERT INTO django_migrations VALUES(46,'core','0027_project_notification_strategy','2020-10-29 19:53:48.874174');
-INSERT INTO django_migrations VALUES(47,'core','0028_suite_and_test_name_length','2020-10-29 19:53:48.904852');
-INSERT INTO django_migrations VALUES(48,'core','0029_subscription_email_formats','2020-10-29 19:53:48.913498');
-INSERT INTO django_migrations VALUES(49,'core','0030_remove_project_build_completion_threshold','2020-10-29 19:53:48.922128');
-INSERT INTO django_migrations VALUES(50,'core','0031_environment_expected_test_runs','2020-10-29 19:53:48.930154');
-INSERT INTO django_migrations VALUES(51,'core','0032_testrun_completed','2020-10-29 19:53:48.938739');
-INSERT INTO django_migrations VALUES(52,'core','0033_drop_debversion','2020-10-29 19:53:48.948072');
-INSERT INTO django_migrations VALUES(53,'core','0034_prepare_to_remove_build_name','2020-10-29 19:53:48.952030');
-INSERT INTO django_migrations VALUES(54,'core','0035_remove_build_name','2020-10-29 19:53:48.964588');
-INSERT INTO django_migrations VALUES(55,'core','0036_status_tests_skip','2020-10-29 19:53:48.973058');
-INSERT INTO django_migrations VALUES(56,'core','0037_project_status_test_summary_fields','2020-10-29 19:53:48.995040');
-INSERT INTO django_migrations VALUES(57,'core','0038_populate_project_status_cache','2020-10-29 19:53:49.010511');
-INSERT INTO django_migrations VALUES(58,'core','0039_orderings','2020-10-29 19:53:49.023778');
-INSERT INTO django_migrations VALUES(59,'core','0040_remove_subscription_html','2020-10-29 19:53:49.031867');
-INSERT INTO django_migrations VALUES(60,'core','0041_projectstatus_notified','2020-10-29 19:53:49.039285');
-INSERT INTO django_migrations VALUES(61,'core','0042_set_projectstatus_notified','2020-10-29 19:53:49.042982');
-INSERT INTO django_migrations VALUES(62,'core','0043_project_status_build','2020-10-29 19:53:49.052420');
-INSERT INTO django_migrations VALUES(63,'core','0044_project_html_mail','2020-10-29 19:53:49.092019');
-INSERT INTO django_migrations VALUES(64,'core','0045_adminsubscription','2020-10-29 19:53:49.099120');
-INSERT INTO django_migrations VALUES(65,'core','0046_projectstatus_last_updated','2020-10-29 19:53:49.107133');
-INSERT INTO django_migrations VALUES(66,'core','0047_populate_projectstatus_last_updated','2020-10-29 19:53:49.111688');
-INSERT INTO django_migrations VALUES(67,'core','0048_moderate_notifications','2020-10-29 19:53:49.122750');
-INSERT INTO django_migrations VALUES(68,'core','0049_projectstatus_plural','2020-10-29 19:53:49.127310');
-INSERT INTO django_migrations VALUES(69,'core','0050_projectstatus_finished','2020-10-29 19:53:49.134037');
-INSERT INTO django_migrations VALUES(70,'core','0051_build_status','2020-10-29 19:53:49.142785');
-INSERT INTO django_migrations VALUES(71,'core','0052_recreate_projectstatus_data','2020-10-29 19:53:49.158516');
-INSERT INTO django_migrations VALUES(72,'core','0053_remove_projectstatus_previous','2020-10-29 19:53:49.167620');
-INSERT INTO django_migrations VALUES(73,'core','0054_custom_email_template','2020-10-29 19:53:49.178656');
-INSERT INTO django_migrations VALUES(74,'core','0055_emailtemplate_subject','2020-10-29 19:53:49.183950');
-INSERT INTO django_migrations VALUES(75,'core','0056_project_description','2020-10-29 19:53:49.193396');
-INSERT INTO django_migrations VALUES(76,'core','0057_projectstatus_has_metrics','2020-10-29 19:53:49.200199');
-INSERT INTO django_migrations VALUES(77,'core','0058_populate_projectstatus_has_metrics','2020-10-29 19:53:49.206689');
-INSERT INTO django_migrations VALUES(78,'core','0059_project_important_metadata_keys','2020-10-29 19:53:49.214847');
-INSERT INTO django_migrations VALUES(79,'core','0060_test_log','2020-10-29 19:53:49.223129');
-INSERT INTO django_migrations VALUES(80,'core','0061_project_enabled_plugins_list','2020-10-29 19:53:49.241033');
-INSERT INTO django_migrations VALUES(81,'ci','0001_initial','2020-10-29 19:53:49.254586');
-INSERT INTO django_migrations VALUES(82,'ci','0002_auto_20170406_1252','2020-10-29 19:53:49.263616');
-INSERT INTO django_migrations VALUES(83,'ci','0003_backend_name','2020-10-29 19:53:49.269388');
-INSERT INTO django_migrations VALUES(84,'ci','0004_testjob_failure','2020-10-29 19:53:49.280274');
-INSERT INTO django_migrations VALUES(85,'ci','0005_remove_listener_data','2020-10-29 19:53:49.289018');
-INSERT INTO django_migrations VALUES(86,'ci','0006_simplify_backend_loading','2020-10-29 19:53:49.294663');
-INSERT INTO django_migrations VALUES(87,'ci','0007_auto_20170517_1736','2020-10-29 19:53:49.304341');
-INSERT INTO django_migrations VALUES(88,'ci','0008_testjob_testrun','2020-10-29 19:53:49.316891');
-INSERT INTO django_migrations VALUES(89,'ci','0009_slug_pattern','2020-10-29 19:53:49.328643');
-INSERT INTO django_migrations VALUES(90,'ci','0010_testjob_can_resubmit','2020-10-29 19:53:49.339692');
-INSERT INTO django_migrations VALUES(91,'ci','0011_testjob_resubmitted_count','2020-10-29 19:53:49.351286');
-INSERT INTO django_migrations VALUES(92,'ci','0012_testjob_build','2020-10-29 19:53:49.362195');
-INSERT INTO django_migrations VALUES(93,'ci','0013_testjob_name','2020-10-29 19:53:49.374035');
-INSERT INTO django_migrations VALUES(94,'ci','0014_testjob_target_build','2020-10-29 19:53:49.386886');
-INSERT INTO django_migrations VALUES(95,'ci','0015_testjob_populate_target_build','2020-10-29 19:53:49.389954');
-INSERT INTO django_migrations VALUES(96,'ci','0016_backend_max_fetch_attempts','2020-10-29 19:53:49.401684');
-INSERT INTO django_migrations VALUES(97,'ci','0017_testjob_fetch_attempts','2020-10-29 19:53:49.418055');
-INSERT INTO django_migrations VALUES(98,'ci','0018_testjob_dates','2020-10-29 19:53:49.449469');
-INSERT INTO django_migrations VALUES(99,'ci','0019_add_fake_backend','2020-10-29 19:53:49.455367');
-INSERT INTO django_migrations VALUES(100,'ci','0020_backend_settings_field','2020-10-29 19:53:49.460787');
-INSERT INTO django_migrations VALUES(101,'ci','0021_testjob_parent_job','2020-10-29 19:53:49.475248');
-INSERT INTO django_migrations VALUES(102,'ci','0022_backend_poll_enabled','2020-10-29 19:53:49.481621');
-INSERT INTO django_migrations VALUES(103,'ci','0023_remove_testjob_build','2020-10-29 19:53:49.493876');
-INSERT INTO django_migrations VALUES(104,'ci','0024_fix_testjob_environment_validation','2020-10-29 19:53:49.506531');
-INSERT INTO django_migrations VALUES(105,'ci','0025_backend_listen_enabled','2020-10-29 19:53:49.512349');
-INSERT INTO django_migrations VALUES(106,'core','0062_project_allow_empty_enabled_plugin_list','2020-10-29 19:53:49.522754');
-INSERT INTO django_migrations VALUES(107,'core','0063_project_wait_before_notification','2020-10-29 19:53:49.542763');
-INSERT INTO django_migrations VALUES(108,'core','0064_project_notification_timeout','2020-10-29 19:53:49.555253');
-INSERT INTO django_migrations VALUES(109,'core','0065_projectstatus_notified_on_timeout','2020-10-29 19:53:49.563378');
-INSERT INTO django_migrations VALUES(110,'core','0066_environment_description','2020-10-29 19:53:49.571600');
-INSERT INTO django_migrations VALUES(111,'core','0067_accept_blank_suite_name','2020-10-29 19:53:49.593153');
-INSERT INTO django_migrations VALUES(112,'core','0068_suite_version','2020-10-29 19:53:49.623539');
-INSERT INTO django_migrations VALUES(113,'core','0069_suite_metadata','2020-10-29 19:53:49.666650');
-INSERT INTO django_migrations VALUES(114,'core','0070_create_suite_test_and_metric_metadata','2020-10-29 19:53:49.729473');
-INSERT INTO django_migrations VALUES(115,'core','0071_migrate_old_tokens','2020-10-29 19:53:49.746880');
-INSERT INTO django_migrations VALUES(116,'core','0072_group_description','2020-10-29 19:53:49.754735');
-INSERT INTO django_migrations VALUES(117,'core','0073_auto_20180420_1643','2020-10-29 19:53:49.780667');
-INSERT INTO django_migrations VALUES(118,'core','0074_add_indexes','2020-10-29 19:53:49.828253');
-INSERT INTO django_migrations VALUES(119,'core','0075_update_project_enabled_plugin_list','2020-10-29 19:53:49.838345');
-INSERT INTO django_migrations VALUES(120,'core','0076_patch_builds','2020-10-29 19:53:49.871987');
-INSERT INTO django_migrations VALUES(121,'core','0077_knownissue','2020-10-29 19:53:49.884672');
-INSERT INTO django_migrations VALUES(122,'core','0078_cache_test_run_counts','2020-10-29 19:53:49.905258');
-INSERT INTO django_migrations VALUES(123,'core','0079_init_cache_test_run_counts','2020-10-29 19:53:49.924527');
-INSERT INTO django_migrations VALUES(124,'core','0080_auto_20180810_0047','2020-10-29 19:53:49.938197');
-INSERT INTO django_migrations VALUES(125,'core','0081_status_has_metrics','2020-10-29 19:53:49.950391');
-INSERT INTO django_migrations VALUES(126,'core','0082_populate_status_has_metrics','2020-10-29 19:53:49.953530');
-INSERT INTO django_migrations VALUES(127,'core','0083_rename_knownissue_environments','2020-10-29 19:53:49.969045');
-INSERT INTO django_migrations VALUES(128,'core','0084_projectstatus_regressions_fixes','2020-10-29 19:53:49.983691');
-INSERT INTO django_migrations VALUES(129,'core','0085_projectstatus_defaults','2020-10-29 19:53:50.005999');
-INSERT INTO django_migrations VALUES(130,'core','0086_xfail','2020-10-29 19:53:50.023557');
-INSERT INTO django_migrations VALUES(131,'core','0087_test_known_issues','2020-10-29 19:53:50.040315');
-INSERT INTO django_migrations VALUES(132,'core','0088_user_subscriptions','2020-10-29 19:53:50.094559');
-INSERT INTO django_migrations VALUES(133,'core','0089_test_has_known_issues','2020-10-29 19:53:50.107582');
-INSERT INTO django_migrations VALUES(134,'core','0090_populate_test_has_known_issues','2020-10-29 19:53:50.110113');
-INSERT INTO django_migrations VALUES(135,'core','0091_notification_delivery_remove_unique_status','2020-10-29 19:53:50.126258');
-INSERT INTO django_migrations VALUES(136,'core','0092_annotation','2020-10-29 19:53:50.142468');
-INSERT INTO django_migrations VALUES(137,'core','0093_historicalemailtemplate','2020-10-29 19:53:50.159643');
-INSERT INTO django_migrations VALUES(138,'core','0094_populatehistoricalemailtemplate','2020-10-29 19:53:50.218359');
-INSERT INTO django_migrations VALUES(139,'core','0095_project_data_retention_days','2020-10-29 19:53:50.229019');
-INSERT INTO django_migrations VALUES(140,'core','0096_build_keep_data','2020-10-29 19:53:50.238906');
-INSERT INTO django_migrations VALUES(141,'core','0097_build_placeholder','2020-10-29 19:53:50.259571');
-INSERT INTO django_migrations VALUES(142,'core','0098_blank_annotation','2020-10-29 19:53:50.268443');
-INSERT INTO django_migrations VALUES(143,'core','0099_metricthreshold','2020-10-29 19:53:50.284839');
-INSERT INTO django_migrations VALUES(144,'core','0100_metric_is_outlier','2020-10-29 19:53:50.296607');
-INSERT INTO django_migrations VALUES(145,'core','0101_project_project_settings','2020-10-29 19:53:50.307807');
-INSERT INTO django_migrations VALUES(146,'core','0102_projectstatus_null_metric_summary','2020-10-29 19:53:50.317633');
-INSERT INTO django_migrations VALUES(147,'core','0103_populate_project_status','2020-10-29 19:53:50.339932');
-INSERT INTO django_migrations VALUES(148,'core','0104_delayedreport','2020-10-29 19:53:50.353678');
-INSERT INTO django_migrations VALUES(149,'core','0105_delayed_report_error_message','2020-10-29 19:53:50.364123');
-INSERT INTO django_migrations VALUES(150,'core','0106_delayedreport_output_subject','2020-10-29 19:53:50.375346');
-INSERT INTO django_migrations VALUES(151,'core','0107_move_notification_strategy','2020-10-29 19:53:50.417271');
-INSERT INTO django_migrations VALUES(152,'core','0108_add_email_template_validator','2020-10-29 19:53:50.450770');
-INSERT INTO django_migrations VALUES(153,'core','0109_group_member','2020-10-29 19:53:50.471117');
-INSERT INTO django_migrations VALUES(154,'core','0110_move_users_from_django_groups_to_squad_groups','2020-10-29 19:53:50.495491');
-INSERT INTO django_migrations VALUES(155,'core','0111_remove_group_user_groups','2020-10-29 19:53:50.505389');
-INSERT INTO django_migrations VALUES(156,'core','0112_user_namespaces','2020-10-29 19:53:50.517568');
-INSERT INTO django_migrations VALUES(157,'core','0113_group_project_blank_name_and_description','2020-10-29 19:53:50.542910');
-INSERT INTO django_migrations VALUES(158,'core','0114_project_enabled_plugin_list_can_be_blank','2020-10-29 19:53:50.553506');
-INSERT INTO django_migrations VALUES(159,'core','0115_fix_slug_validation','2020-10-29 19:53:50.582921');
-INSERT INTO django_migrations VALUES(160,'core','0116_make_group_membership_unique','2020-10-29 19:53:50.613667');
-INSERT INTO django_migrations VALUES(161,'core','0117_drop_obsolete_token_model','2020-10-29 19:53:50.625285');
-INSERT INTO django_migrations VALUES(162,'core','0118_project_is_archived','2020-10-29 19:53:50.634052');
-INSERT INTO django_migrations VALUES(163,'core','0119_i18n','2020-10-29 19:53:50.735322');
-INSERT INTO django_migrations VALUES(164,'core','0120_buildsummary','2020-10-29 19:53:50.747497');
-INSERT INTO django_migrations VALUES(165,'core','0121_add_password_patchsource','2020-10-29 19:53:50.757428');
-INSERT INTO django_migrations VALUES(166,'core','0122_fix_patchsource_url_and_token','2020-10-29 19:53:50.767069');
-INSERT INTO django_migrations VALUES(167,'core','0123_django_upgrade_missing_migrations','2020-10-29 19:53:50.815843');
-INSERT INTO django_migrations VALUES(168,'core','0124_set_default_expected_test_runs_to_zero','2020-10-29 19:53:50.827227');
-INSERT INTO django_migrations VALUES(169,'core','0125_fix_missing_status_has_metrics_for_testruns','2020-10-29 19:53:50.852451');
-INSERT INTO django_migrations VALUES(170,'core','0126_metricthreshold_environment','2020-10-29 19:53:50.879980');
-INSERT INTO django_migrations VALUES(171,'core','0127_metric_thresholds_migrate_data','2020-10-29 19:53:50.903898');
-INSERT INTO django_migrations VALUES(172,'core','0128_metric_thresholds_remove_proj_col','2020-10-29 19:53:50.942751');
-INSERT INTO django_migrations VALUES(173,'core','0129_projectstatus_nullable_notified_on_timeout','2020-10-29 19:53:50.953269');
-INSERT INTO django_migrations VALUES(174,'core','0130_project_status_baseline_next','2020-10-29 19:53:50.972382');
-INSERT INTO django_migrations VALUES(175,'core','0131_create_squad_auth_group_and_add_users','2020-10-29 19:53:51.062227');
-INSERT INTO django_migrations VALUES(176,'core','0132_attachment_mimetype','2020-10-29 19:53:51.080924');
-INSERT INTO django_migrations VALUES(177,'core','0133_append_project_permissions_to_squad_auth_group','2020-10-29 19:53:51.116012');
-INSERT INTO django_migrations VALUES(178,'core','0134_longer_metric_name','2020-10-29 19:53:51.127048');
-INSERT INTO django_migrations VALUES(179,'core','0135_add_privileged_access_level','2020-10-29 19:53:51.149496');
-INSERT INTO django_migrations VALUES(180,'core','0136_migrate_submitters_to_privileged','2020-10-29 19:53:51.175553');
-INSERT INTO django_migrations VALUES(181,'core','0137_patchsource_token_null','2020-10-29 19:53:51.181279');
-INSERT INTO django_migrations VALUES(182,'core','0138_metric_unit','2020-10-29 19:53:51.192585');
-INSERT INTO django_migrations VALUES(183,'core','0139_nullable_test_name','2020-10-29 19:53:51.211238');
-INSERT INTO django_migrations VALUES(184,'django_celery_results','0001_initial','2020-10-29 19:53:51.215868');
-INSERT INTO django_migrations VALUES(185,'django_celery_results','0002_add_task_name_args_kwargs','2020-10-29 19:53:51.227726');
-INSERT INTO django_migrations VALUES(186,'django_celery_results','0003_auto_20181106_1101','2020-10-29 19:53:51.232010');
-INSERT INTO django_migrations VALUES(187,'django_celery_results','0004_auto_20190516_0412','2020-10-29 19:53:51.320752');
-INSERT INTO django_migrations VALUES(188,'django_celery_results','0005_taskresult_worker','2020-10-29 19:53:51.327855');
-INSERT INTO django_migrations VALUES(189,'django_celery_results','0006_taskresult_date_created','2020-10-29 19:53:51.356936');
-INSERT INTO django_migrations VALUES(190,'django_celery_results','0007_remove_taskresult_hidden','2020-10-29 19:53:51.363795');
-INSERT INTO django_migrations VALUES(191,'sessions','0001_initial','2020-10-29 19:53:51.368158');
+INSERT INTO django_migrations VALUES(1,'contenttypes','0001_initial','2020-11-18 20:11:12.335989');
+INSERT INTO django_migrations VALUES(2,'auth','0001_initial','2020-11-18 20:11:12.356589');
+INSERT INTO django_migrations VALUES(3,'admin','0001_initial','2020-11-18 20:11:12.366250');
+INSERT INTO django_migrations VALUES(4,'admin','0002_logentry_remove_auto_add','2020-11-18 20:11:12.375000');
+INSERT INTO django_migrations VALUES(5,'admin','0003_logentry_add_action_flag_choices','2020-11-18 20:11:12.383421');
+INSERT INTO django_migrations VALUES(6,'contenttypes','0002_remove_content_type_name','2020-11-18 20:11:12.397719');
+INSERT INTO django_migrations VALUES(7,'auth','0002_alter_permission_name_max_length','2020-11-18 20:11:12.403259');
+INSERT INTO django_migrations VALUES(8,'auth','0003_alter_user_email_max_length','2020-11-18 20:11:12.411778');
+INSERT INTO django_migrations VALUES(9,'auth','0004_alter_user_username_opts','2020-11-18 20:11:12.419816');
+INSERT INTO django_migrations VALUES(10,'auth','0005_alter_user_last_login_null','2020-11-18 20:11:12.427263');
+INSERT INTO django_migrations VALUES(11,'auth','0006_require_contenttypes_0002','2020-11-18 20:11:12.429211');
+INSERT INTO django_migrations VALUES(12,'auth','0007_alter_validators_add_error_messages','2020-11-18 20:11:12.436666');
+INSERT INTO django_migrations VALUES(13,'auth','0008_alter_user_username_max_length','2020-11-18 20:11:12.444232');
+INSERT INTO django_migrations VALUES(14,'auth','0009_alter_user_last_name_max_length','2020-11-18 20:11:12.451784');
+INSERT INTO django_migrations VALUES(15,'auth','0010_alter_group_name_max_length','2020-11-18 20:11:12.458295');
+INSERT INTO django_migrations VALUES(16,'auth','0011_update_proxy_permissions','2020-11-18 20:11:12.488761');
+INSERT INTO django_migrations VALUES(17,'authtoken','0001_initial','2020-11-18 20:11:12.495578');
+INSERT INTO django_migrations VALUES(18,'authtoken','0002_auto_20160226_1747','2020-11-18 20:11:12.530095');
+INSERT INTO django_migrations VALUES(19,'authtoken','0003_tokenproxy','2020-11-18 20:11:12.533557');
+INSERT INTO django_migrations VALUES(20,'core','0001_initial','2020-11-18 20:11:12.586226');
+INSERT INTO django_migrations VALUES(21,'core','0002_auto_20160525_1403','2020-11-18 20:11:12.600459');
+INSERT INTO django_migrations VALUES(22,'core','0003_testrun_log_file','2020-11-18 20:11:12.607960');
+INSERT INTO django_migrations VALUES(23,'core','0004_group_user_groups','2020-11-18 20:11:12.618399');
+INSERT INTO django_migrations VALUES(24,'core','0005_token','2020-11-18 20:11:12.630121');
+INSERT INTO django_migrations VALUES(25,'core','0006_auto_20160826_2242','2020-11-18 20:11:12.644524');
+INSERT INTO django_migrations VALUES(26,'core','0007_testrun_data_processed','2020-11-18 20:11:12.652394');
+INSERT INTO django_migrations VALUES(27,'core','0008_status','2020-11-18 20:11:12.668426');
+INSERT INTO django_migrations VALUES(28,'core','0009_testrun_status_recorded','2020-11-18 20:11:12.678287');
+INSERT INTO django_migrations VALUES(29,'core','0010_testrun_datetime','2020-11-18 20:11:12.695481');
+INSERT INTO django_migrations VALUES(30,'core','0011_testrun_metadata_fields','2020-11-18 20:11:12.720588');
+INSERT INTO django_migrations VALUES(31,'core','0012_build_datetime','2020-11-18 20:11:12.734138');
+INSERT INTO django_migrations VALUES(32,'core','0013_testrun_resubmit_url','2020-11-18 20:11:12.741847');
+INSERT INTO django_migrations VALUES(33,'core','0014_testrun_metadata_file','2020-11-18 20:11:12.748778');
+INSERT INTO django_migrations VALUES(34,'core','0015_attachment','2020-11-18 20:11:12.759001');
+INSERT INTO django_migrations VALUES(35,'core','0016_project_is_public','2020-11-18 20:11:12.768166');
+INSERT INTO django_migrations VALUES(36,'core','0017_slug_validator','2020-11-18 20:11:12.790184');
+INSERT INTO django_migrations VALUES(37,'core','0018_build_name','2020-11-18 20:11:12.798758');
+INSERT INTO django_migrations VALUES(38,'core','0019_build_version','2020-11-18 20:11:12.805893');
+INSERT INTO django_migrations VALUES(39,'core','0020_build_ordering','2020-11-18 20:11:12.811156');
+INSERT INTO django_migrations VALUES(40,'core','0021_global_tokens','2020-11-18 20:11:12.822558');
+INSERT INTO django_migrations VALUES(41,'core','0022_projectstatus','2020-11-18 20:11:12.834616');
+INSERT INTO django_migrations VALUES(42,'core','0023_subscription','2020-11-18 20:11:12.848543');
+INSERT INTO django_migrations VALUES(43,'core','0024_project_build_completion_threshold','2020-11-18 20:11:12.857710');
+INSERT INTO django_migrations VALUES(44,'core','0025_unique_testrun_job_id','2020-11-18 20:11:12.863563');
+INSERT INTO django_migrations VALUES(45,'core','0026_testrun_result_accept_null','2020-11-18 20:11:12.877182');
+INSERT INTO django_migrations VALUES(46,'core','0027_project_notification_strategy','2020-11-18 20:11:12.886291');
+INSERT INTO django_migrations VALUES(47,'core','0028_suite_and_test_name_length','2020-11-18 20:11:12.917920');
+INSERT INTO django_migrations VALUES(48,'core','0029_subscription_email_formats','2020-11-18 20:11:12.925851');
+INSERT INTO django_migrations VALUES(49,'core','0030_remove_project_build_completion_threshold','2020-11-18 20:11:12.937668');
+INSERT INTO django_migrations VALUES(50,'core','0031_environment_expected_test_runs','2020-11-18 20:11:12.946261');
+INSERT INTO django_migrations VALUES(51,'core','0032_testrun_completed','2020-11-18 20:11:12.954080');
+INSERT INTO django_migrations VALUES(52,'core','0033_drop_debversion','2020-11-18 20:11:12.963996');
+INSERT INTO django_migrations VALUES(53,'core','0034_prepare_to_remove_build_name','2020-11-18 20:11:12.967703');
+INSERT INTO django_migrations VALUES(54,'core','0035_remove_build_name','2020-11-18 20:11:12.980306');
+INSERT INTO django_migrations VALUES(55,'core','0036_status_tests_skip','2020-11-18 20:11:12.988933');
+INSERT INTO django_migrations VALUES(56,'core','0037_project_status_test_summary_fields','2020-11-18 20:11:13.011148');
+INSERT INTO django_migrations VALUES(57,'core','0038_populate_project_status_cache','2020-11-18 20:11:13.026588');
+INSERT INTO django_migrations VALUES(58,'core','0039_orderings','2020-11-18 20:11:13.039859');
+INSERT INTO django_migrations VALUES(59,'core','0040_remove_subscription_html','2020-11-18 20:11:13.048194');
+INSERT INTO django_migrations VALUES(60,'core','0041_projectstatus_notified','2020-11-18 20:11:13.055613');
+INSERT INTO django_migrations VALUES(61,'core','0042_set_projectstatus_notified','2020-11-18 20:11:13.060208');
+INSERT INTO django_migrations VALUES(62,'core','0043_project_status_build','2020-11-18 20:11:13.070237');
+INSERT INTO django_migrations VALUES(63,'core','0044_project_html_mail','2020-11-18 20:11:13.108774');
+INSERT INTO django_migrations VALUES(64,'core','0045_adminsubscription','2020-11-18 20:11:13.116284');
+INSERT INTO django_migrations VALUES(65,'core','0046_projectstatus_last_updated','2020-11-18 20:11:13.123159');
+INSERT INTO django_migrations VALUES(66,'core','0047_populate_projectstatus_last_updated','2020-11-18 20:11:13.126958');
+INSERT INTO django_migrations VALUES(67,'core','0048_moderate_notifications','2020-11-18 20:11:13.138585');
+INSERT INTO django_migrations VALUES(68,'core','0049_projectstatus_plural','2020-11-18 20:11:13.144130');
+INSERT INTO django_migrations VALUES(69,'core','0050_projectstatus_finished','2020-11-18 20:11:13.150740');
+INSERT INTO django_migrations VALUES(70,'core','0051_build_status','2020-11-18 20:11:13.162108');
+INSERT INTO django_migrations VALUES(71,'core','0052_recreate_projectstatus_data','2020-11-18 20:11:13.178583');
+INSERT INTO django_migrations VALUES(72,'core','0053_remove_projectstatus_previous','2020-11-18 20:11:13.188187');
+INSERT INTO django_migrations VALUES(73,'core','0054_custom_email_template','2020-11-18 20:11:13.200011');
+INSERT INTO django_migrations VALUES(74,'core','0055_emailtemplate_subject','2020-11-18 20:11:13.205405');
+INSERT INTO django_migrations VALUES(75,'core','0056_project_description','2020-11-18 20:11:13.213488');
+INSERT INTO django_migrations VALUES(76,'core','0057_projectstatus_has_metrics','2020-11-18 20:11:13.219851');
+INSERT INTO django_migrations VALUES(77,'core','0058_populate_projectstatus_has_metrics','2020-11-18 20:11:13.227134');
+INSERT INTO django_migrations VALUES(78,'core','0059_project_important_metadata_keys','2020-11-18 20:11:13.235384');
+INSERT INTO django_migrations VALUES(79,'core','0060_test_log','2020-11-18 20:11:13.243921');
+INSERT INTO django_migrations VALUES(80,'core','0061_project_enabled_plugins_list','2020-11-18 20:11:13.252968');
+INSERT INTO django_migrations VALUES(81,'ci','0001_initial','2020-11-18 20:11:13.263839');
+INSERT INTO django_migrations VALUES(82,'ci','0002_auto_20170406_1252','2020-11-18 20:11:13.272785');
+INSERT INTO django_migrations VALUES(83,'ci','0003_backend_name','2020-11-18 20:11:13.279789');
+INSERT INTO django_migrations VALUES(84,'ci','0004_testjob_failure','2020-11-18 20:11:13.290761');
+INSERT INTO django_migrations VALUES(85,'ci','0005_remove_listener_data','2020-11-18 20:11:13.300024');
+INSERT INTO django_migrations VALUES(86,'ci','0006_simplify_backend_loading','2020-11-18 20:11:13.306064');
+INSERT INTO django_migrations VALUES(87,'ci','0007_auto_20170517_1736','2020-11-18 20:11:13.315304');
+INSERT INTO django_migrations VALUES(88,'ci','0008_testjob_testrun','2020-11-18 20:11:13.327719');
+INSERT INTO django_migrations VALUES(89,'ci','0009_slug_pattern','2020-11-18 20:11:13.339037');
+INSERT INTO django_migrations VALUES(90,'ci','0010_testjob_can_resubmit','2020-11-18 20:11:13.350201');
+INSERT INTO django_migrations VALUES(91,'ci','0011_testjob_resubmitted_count','2020-11-18 20:11:13.361869');
+INSERT INTO django_migrations VALUES(92,'ci','0012_testjob_build','2020-11-18 20:11:13.373925');
+INSERT INTO django_migrations VALUES(93,'ci','0013_testjob_name','2020-11-18 20:11:13.386311');
+INSERT INTO django_migrations VALUES(94,'ci','0014_testjob_target_build','2020-11-18 20:11:13.400308');
+INSERT INTO django_migrations VALUES(95,'ci','0015_testjob_populate_target_build','2020-11-18 20:11:13.402460');
+INSERT INTO django_migrations VALUES(96,'ci','0016_backend_max_fetch_attempts','2020-11-18 20:11:13.407960');
+INSERT INTO django_migrations VALUES(97,'ci','0017_testjob_fetch_attempts','2020-11-18 20:11:13.420171');
+INSERT INTO django_migrations VALUES(98,'ci','0018_testjob_dates','2020-11-18 20:11:13.451764');
+INSERT INTO django_migrations VALUES(99,'ci','0019_add_fake_backend','2020-11-18 20:11:13.458455');
+INSERT INTO django_migrations VALUES(100,'ci','0020_backend_settings_field','2020-11-18 20:11:13.465338');
+INSERT INTO django_migrations VALUES(101,'ci','0021_testjob_parent_job','2020-11-18 20:11:13.480402');
+INSERT INTO django_migrations VALUES(102,'ci','0022_backend_poll_enabled','2020-11-18 20:11:13.486459');
+INSERT INTO django_migrations VALUES(103,'ci','0023_remove_testjob_build','2020-11-18 20:11:13.499391');
+INSERT INTO django_migrations VALUES(104,'ci','0024_fix_testjob_environment_validation','2020-11-18 20:11:13.512635');
+INSERT INTO django_migrations VALUES(105,'ci','0025_backend_listen_enabled','2020-11-18 20:11:13.518746');
+INSERT INTO django_migrations VALUES(106,'core','0062_project_allow_empty_enabled_plugin_list','2020-11-18 20:11:13.530564');
+INSERT INTO django_migrations VALUES(107,'core','0063_project_wait_before_notification','2020-11-18 20:11:13.541392');
+INSERT INTO django_migrations VALUES(108,'core','0064_project_notification_timeout','2020-11-18 20:11:13.552231');
+INSERT INTO django_migrations VALUES(109,'core','0065_projectstatus_notified_on_timeout','2020-11-18 20:11:13.559854');
+INSERT INTO django_migrations VALUES(110,'core','0066_environment_description','2020-11-18 20:11:13.568936');
+INSERT INTO django_migrations VALUES(111,'core','0067_accept_blank_suite_name','2020-11-18 20:11:13.577821');
+INSERT INTO django_migrations VALUES(112,'core','0068_suite_version','2020-11-18 20:11:13.606079');
+INSERT INTO django_migrations VALUES(113,'core','0069_suite_metadata','2020-11-18 20:11:13.650758');
+INSERT INTO django_migrations VALUES(114,'core','0070_create_suite_test_and_metric_metadata','2020-11-18 20:11:13.710019');
+INSERT INTO django_migrations VALUES(115,'core','0071_migrate_old_tokens','2020-11-18 20:11:13.727004');
+INSERT INTO django_migrations VALUES(116,'core','0072_group_description','2020-11-18 20:11:13.734194');
+INSERT INTO django_migrations VALUES(117,'core','0073_auto_20180420_1643','2020-11-18 20:11:13.761714');
+INSERT INTO django_migrations VALUES(118,'core','0074_add_indexes','2020-11-18 20:11:13.807746');
+INSERT INTO django_migrations VALUES(119,'core','0075_update_project_enabled_plugin_list','2020-11-18 20:11:13.818819');
+INSERT INTO django_migrations VALUES(120,'core','0076_patch_builds','2020-11-18 20:11:13.852568');
+INSERT INTO django_migrations VALUES(121,'core','0077_knownissue','2020-11-18 20:11:13.865474');
+INSERT INTO django_migrations VALUES(122,'core','0078_cache_test_run_counts','2020-11-18 20:11:13.888107');
+INSERT INTO django_migrations VALUES(123,'core','0079_init_cache_test_run_counts','2020-11-18 20:11:13.907702');
+INSERT INTO django_migrations VALUES(124,'core','0080_auto_20180810_0047','2020-11-18 20:11:13.921835');
+INSERT INTO django_migrations VALUES(125,'core','0081_status_has_metrics','2020-11-18 20:11:13.938699');
+INSERT INTO django_migrations VALUES(126,'core','0082_populate_status_has_metrics','2020-11-18 20:11:13.941945');
+INSERT INTO django_migrations VALUES(127,'core','0083_rename_knownissue_environments','2020-11-18 20:11:13.958036');
+INSERT INTO django_migrations VALUES(128,'core','0084_projectstatus_regressions_fixes','2020-11-18 20:11:13.974770');
+INSERT INTO django_migrations VALUES(129,'core','0085_projectstatus_defaults','2020-11-18 20:11:13.997620');
+INSERT INTO django_migrations VALUES(130,'core','0086_xfail','2020-11-18 20:11:14.015332');
+INSERT INTO django_migrations VALUES(131,'core','0087_test_known_issues','2020-11-18 20:11:14.031872');
+INSERT INTO django_migrations VALUES(132,'core','0088_user_subscriptions','2020-11-18 20:11:14.088054');
+INSERT INTO django_migrations VALUES(133,'core','0089_test_has_known_issues','2020-11-18 20:11:14.101742');
+INSERT INTO django_migrations VALUES(134,'core','0090_populate_test_has_known_issues','2020-11-18 20:11:14.104303');
+INSERT INTO django_migrations VALUES(135,'core','0091_notification_delivery_remove_unique_status','2020-11-18 20:11:14.120724');
+INSERT INTO django_migrations VALUES(136,'core','0092_annotation','2020-11-18 20:11:14.136771');
+INSERT INTO django_migrations VALUES(137,'core','0093_historicalemailtemplate','2020-11-18 20:11:14.153119');
+INSERT INTO django_migrations VALUES(138,'core','0094_populatehistoricalemailtemplate','2020-11-18 20:11:14.212562');
+INSERT INTO django_migrations VALUES(139,'core','0095_project_data_retention_days','2020-11-18 20:11:14.222292');
+INSERT INTO django_migrations VALUES(140,'core','0096_build_keep_data','2020-11-18 20:11:14.232972');
+INSERT INTO django_migrations VALUES(141,'core','0097_build_placeholder','2020-11-18 20:11:14.253638');
+INSERT INTO django_migrations VALUES(142,'core','0098_blank_annotation','2020-11-18 20:11:14.262306');
+INSERT INTO django_migrations VALUES(143,'core','0099_metricthreshold','2020-11-18 20:11:14.279144');
+INSERT INTO django_migrations VALUES(144,'core','0100_metric_is_outlier','2020-11-18 20:11:14.290266');
+INSERT INTO django_migrations VALUES(145,'core','0101_project_project_settings','2020-11-18 20:11:14.301687');
+INSERT INTO django_migrations VALUES(146,'core','0102_projectstatus_null_metric_summary','2020-11-18 20:11:14.312303');
+INSERT INTO django_migrations VALUES(147,'core','0103_populate_project_status','2020-11-18 20:11:14.342861');
+INSERT INTO django_migrations VALUES(148,'core','0104_delayedreport','2020-11-18 20:11:14.357974');
+INSERT INTO django_migrations VALUES(149,'core','0105_delayed_report_error_message','2020-11-18 20:11:14.370251');
+INSERT INTO django_migrations VALUES(150,'core','0106_delayedreport_output_subject','2020-11-18 20:11:14.385820');
+INSERT INTO django_migrations VALUES(151,'core','0107_move_notification_strategy','2020-11-18 20:11:14.437672');
+INSERT INTO django_migrations VALUES(152,'core','0108_add_email_template_validator','2020-11-18 20:11:14.472347');
+INSERT INTO django_migrations VALUES(153,'core','0109_group_member','2020-11-18 20:11:14.492930');
+INSERT INTO django_migrations VALUES(154,'core','0110_move_users_from_django_groups_to_squad_groups','2020-11-18 20:11:14.518408');
+INSERT INTO django_migrations VALUES(155,'core','0111_remove_group_user_groups','2020-11-18 20:11:14.529243');
+INSERT INTO django_migrations VALUES(156,'core','0112_user_namespaces','2020-11-18 20:11:14.541743');
+INSERT INTO django_migrations VALUES(157,'core','0113_group_project_blank_name_and_description','2020-11-18 20:11:14.570388');
+INSERT INTO django_migrations VALUES(158,'core','0114_project_enabled_plugin_list_can_be_blank','2020-11-18 20:11:14.585298');
+INSERT INTO django_migrations VALUES(159,'core','0115_fix_slug_validation','2020-11-18 20:11:14.627545');
+INSERT INTO django_migrations VALUES(160,'core','0116_make_group_membership_unique','2020-11-18 20:11:14.659284');
+INSERT INTO django_migrations VALUES(161,'core','0117_drop_obsolete_token_model','2020-11-18 20:11:14.670734');
+INSERT INTO django_migrations VALUES(162,'core','0118_project_is_archived','2020-11-18 20:11:14.680260');
+INSERT INTO django_migrations VALUES(163,'core','0119_i18n','2020-11-18 20:11:14.790200');
+INSERT INTO django_migrations VALUES(164,'core','0120_buildsummary','2020-11-18 20:11:14.802976');
+INSERT INTO django_migrations VALUES(165,'core','0121_add_password_patchsource','2020-11-18 20:11:14.812582');
+INSERT INTO django_migrations VALUES(166,'core','0122_fix_patchsource_url_and_token','2020-11-18 20:11:14.821613');
+INSERT INTO django_migrations VALUES(167,'core','0123_django_upgrade_missing_migrations','2020-11-18 20:11:14.871703');
+INSERT INTO django_migrations VALUES(168,'core','0124_set_default_expected_test_runs_to_zero','2020-11-18 20:11:14.883283');
+INSERT INTO django_migrations VALUES(169,'core','0125_fix_missing_status_has_metrics_for_testruns','2020-11-18 20:11:14.908189');
+INSERT INTO django_migrations VALUES(170,'core','0126_metricthreshold_environment','2020-11-18 20:11:14.938337');
+INSERT INTO django_migrations VALUES(171,'core','0127_metric_thresholds_migrate_data','2020-11-18 20:11:14.963087');
+INSERT INTO django_migrations VALUES(172,'core','0128_metric_thresholds_remove_proj_col','2020-11-18 20:11:15.003328');
+INSERT INTO django_migrations VALUES(173,'core','0129_projectstatus_nullable_notified_on_timeout','2020-11-18 20:11:15.014171');
+INSERT INTO django_migrations VALUES(174,'core','0130_project_status_baseline_next','2020-11-18 20:11:15.034014');
+INSERT INTO django_migrations VALUES(175,'core','0131_create_squad_auth_group_and_add_users','2020-11-18 20:11:15.123040');
+INSERT INTO django_migrations VALUES(176,'core','0132_attachment_mimetype','2020-11-18 20:11:15.133156');
+INSERT INTO django_migrations VALUES(177,'core','0133_append_project_permissions_to_squad_auth_group','2020-11-18 20:11:15.165206');
+INSERT INTO django_migrations VALUES(178,'core','0134_longer_metric_name','2020-11-18 20:11:15.177871');
+INSERT INTO django_migrations VALUES(179,'core','0135_add_privileged_access_level','2020-11-18 20:11:15.189867');
+INSERT INTO django_migrations VALUES(180,'core','0136_migrate_submitters_to_privileged','2020-11-18 20:11:15.214446');
+INSERT INTO django_migrations VALUES(181,'core','0137_patchsource_token_null','2020-11-18 20:11:15.220438');
+INSERT INTO django_migrations VALUES(182,'core','0138_metric_unit','2020-11-18 20:11:15.232365');
+INSERT INTO django_migrations VALUES(183,'core','0139_nullable_test_name','2020-11-18 20:11:15.252179');
+INSERT INTO django_migrations VALUES(184,'django_celery_results','0001_initial','2020-11-18 20:11:15.256373');
+INSERT INTO django_migrations VALUES(185,'django_celery_results','0002_add_task_name_args_kwargs','2020-11-18 20:11:15.268829');
+INSERT INTO django_migrations VALUES(186,'django_celery_results','0003_auto_20181106_1101','2020-11-18 20:11:15.273426');
+INSERT INTO django_migrations VALUES(187,'django_celery_results','0004_auto_20190516_0412','2020-11-18 20:11:15.369463');
+INSERT INTO django_migrations VALUES(188,'django_celery_results','0005_taskresult_worker','2020-11-18 20:11:15.376174');
+INSERT INTO django_migrations VALUES(189,'django_celery_results','0006_taskresult_date_created','2020-11-18 20:11:15.406560');
+INSERT INTO django_migrations VALUES(190,'django_celery_results','0007_remove_taskresult_hidden','2020-11-18 20:11:15.413376');
+INSERT INTO django_migrations VALUES(191,'sessions','0001_initial','2020-11-18 20:11:15.417756');
 CREATE TABLE IF NOT EXISTS "auth_group_permissions" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "group_id" integer NOT NULL REFERENCES "auth_group" ("id") DEFERRABLE INITIALLY DEFERRED, "permission_id" integer NOT NULL REFERENCES "auth_permission" ("id") DEFERRABLE INITIALLY DEFERRED);
 INSERT INTO auth_group_permissions VALUES(1,1,1);
 INSERT INTO auth_group_permissions VALUES(2,1,2);
 INSERT INTO auth_group_permissions VALUES(3,1,3);
 INSERT INTO auth_group_permissions VALUES(4,1,4);
 INSERT INTO auth_group_permissions VALUES(5,1,5);
 INSERT INTO auth_group_permissions VALUES(6,1,6);
@@ -232,22 +232,23 @@
 INSERT INTO auth_group_permissions VALUES(37,1,37);
 INSERT INTO auth_group_permissions VALUES(38,1,38);
 INSERT INTO auth_group_permissions VALUES(39,1,39);
 CREATE TABLE IF NOT EXISTS "auth_user_groups" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "user_id" integer NOT NULL REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED, "group_id" integer NOT NULL REFERENCES "auth_group" ("id") DEFERRABLE INITIALLY DEFERRED);
 INSERT INTO auth_user_groups VALUES(1,1,1);
 CREATE TABLE IF NOT EXISTS "auth_user_user_permissions" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "user_id" integer NOT NULL REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED, "permission_id" integer NOT NULL REFERENCES "auth_permission" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "django_admin_log" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "action_time" datetime NOT NULL, "object_id" text NULL, "object_repr" varchar(200) NOT NULL, "change_message" text NOT NULL, "content_type_id" integer NULL REFERENCES "django_content_type" ("id") DEFERRABLE INITIALLY DEFERRED, "user_id" integer NOT NULL REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED, "action_flag" smallint unsigned NOT NULL CHECK ("action_flag" >= 0));
-INSERT INTO django_admin_log VALUES(1,'2020-10-29 19:54:10.885533','2','#12345','Test Run created',8,1,1);
-INSERT INTO django_admin_log VALUES(2,'2020-10-29 19:54:12.548504','3','#123','Test Run created',8,1,1);
-INSERT INTO django_admin_log VALUES(3,'2020-10-29 19:54:16.327860','4','#jsonmetadatajobid1','Test Run created',8,1,1);
-INSERT INTO django_admin_log VALUES(4,'2020-10-29 19:54:21.367692','5','#30f04b02-dae3-4c85-8812-33268b318e2a','Test Run created',8,1,1);
-INSERT INTO django_admin_log VALUES(5,'2020-10-29 19:54:27.001906','6','#0bccb805-c7c4-4bbb-ae3d-9c91aedcad38','Test Run created',8,1,1);
-INSERT INTO django_admin_log VALUES(6,'2020-10-29 19:54:35.660626','7','#f0048cfb-25fd-4854-9dc0-08e2bb664a56','Test Run created',8,1,1);
-INSERT INTO django_admin_log VALUES(7,'2020-10-29 19:54:37.747037','8','#163222e8-260b-4a46-a67a-95af09bf2dd7','Test Run created',8,1,1);
-INSERT INTO django_admin_log VALUES(8,'2020-10-29 19:54:39.734773','9','#de328702-1042-4127-883a-de81b49be598','Test Run created',8,1,1);
+INSERT INTO django_admin_log VALUES(1,'2020-11-18 20:11:35.710499','2','#12345','Test Run created',8,1,1);
+INSERT INTO django_admin_log VALUES(2,'2020-11-18 20:11:37.360500','3','#123','Test Run created',8,1,1);
+INSERT INTO django_admin_log VALUES(3,'2020-11-18 20:11:41.444549','4','#jsonmetadatajobid1','Test Run created',8,1,1);
+INSERT INTO django_admin_log VALUES(4,'2020-11-18 20:11:46.557343','5','#f2906910-3478-41c2-8767-b8771abaf3ad','Test Run created',8,1,1);
+INSERT INTO django_admin_log VALUES(5,'2020-11-18 20:11:52.341235','6','#53552722-34bf-41e7-9457-735a4beca4c3','Test Run created',8,1,1);
+INSERT INTO django_admin_log VALUES(6,'2020-11-18 20:11:54.507695','7','#b81ce6e3-d6c6-46a9-b287-8d6a49d1fed0','Test Run created',8,1,1);
+INSERT INTO django_admin_log VALUES(7,'2020-11-18 20:12:07.174403','8','#743847c4-5b29-48c4-b1a6-0a0bec4cb776','Test Run created',8,1,1);
+INSERT INTO django_admin_log VALUES(8,'2020-11-18 20:12:09.430487','9','#9339863d-8e4f-4f11-b90c-edb1cf024a7e','Test Run created',8,1,1);
+INSERT INTO django_admin_log VALUES(9,'2020-11-18 20:12:11.461834','10','#deb37471-8f6a-4e53-b6df-1dde80f69d18','Test Run created',8,1,1);
 CREATE TABLE IF NOT EXISTS "django_content_type" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "app_label" varchar(100) NOT NULL, "model" varchar(100) NOT NULL);
 INSERT INTO django_content_type VALUES(1,'core','annotation');
 INSERT INTO django_content_type VALUES(2,'core','attachment');
 INSERT INTO django_content_type VALUES(3,'core','build');
 INSERT INTO django_content_type VALUES(4,'core','environment');
 INSERT INTO django_content_type VALUES(5,'core','metric');
 INSERT INTO django_content_type VALUES(6,'core','status');
@@ -433,32 +434,33 @@
 INSERT INTO auth_permission VALUES(147,37,'delete_backend','Can delete backend');
 INSERT INTO auth_permission VALUES(148,37,'view_backend','Can view backend');
 INSERT INTO auth_permission VALUES(149,38,'add_taskresult','Can add task result');
 INSERT INTO auth_permission VALUES(150,38,'change_taskresult','Can change task result');
 INSERT INTO auth_permission VALUES(151,38,'delete_taskresult','Can delete task result');
 INSERT INTO auth_permission VALUES(152,38,'view_taskresult','Can view task result');
 CREATE TABLE IF NOT EXISTS "auth_user" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "password" varchar(128) NOT NULL, "last_login" datetime NULL, "is_superuser" bool NOT NULL, "username" varchar(150) NOT NULL UNIQUE, "first_name" varchar(30) NOT NULL, "email" varchar(254) NOT NULL, "is_staff" bool NOT NULL, "is_active" bool NOT NULL, "date_joined" datetime NOT NULL, "last_name" varchar(150) NOT NULL);
-INSERT INTO auth_user VALUES(1,'',NULL,1,'admin_user','','',0,1,'2020-10-29 19:53:53.697191','');
+INSERT INTO auth_user VALUES(1,'',NULL,1,'admin_user','','',0,1,'2020-11-18 20:11:17.786275','');
 CREATE TABLE IF NOT EXISTS "auth_group" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(150) NOT NULL UNIQUE);
 INSERT INTO auth_group VALUES(1,'squad');
 CREATE TABLE IF NOT EXISTS "authtoken_token" ("key" varchar(40) NOT NULL PRIMARY KEY, "created" datetime NOT NULL, "user_id" integer NOT NULL UNIQUE REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED);
-INSERT INTO authtoken_token VALUES('193cd8bb41ab9217714515954e8724f651ef8601','2020-10-29 19:53:53.705457',1);
+INSERT INTO authtoken_token VALUES('193cd8bb41ab9217714515954e8724f651ef8601','2020-11-18 20:11:17.795548',1);
 CREATE TABLE IF NOT EXISTS "core_testrun" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "created_at" datetime NOT NULL, "build_id" integer NOT NULL REFERENCES "core_build" ("id") DEFERRABLE INITIALLY DEFERRED, "environment_id" integer NOT NULL REFERENCES "core_environment" ("id") DEFERRABLE INITIALLY DEFERRED, "metrics_file" text NULL, "tests_file" text NULL, "log_file" text NULL, "data_processed" bool NOT NULL, "status_recorded" bool NOT NULL, "datetime" datetime NOT NULL, "build_url" varchar(2048) NULL, "job_id" varchar(128) NULL, "job_status" varchar(128) NULL, "job_url" varchar(2048) NULL, "resubmit_url" varchar(2048) NULL, "metadata_file" text NULL, "completed" bool NOT NULL);
-INSERT INTO core_testrun VALUES(1,'2020-10-29 19:53:53.757510',1,1,NULL,NULL,NULL,0,1,'2020-10-29 19:53:53.757386',NULL,NULL,NULL,NULL,NULL,NULL,1);
-INSERT INTO core_testrun VALUES(2,'2020-10-29 19:54:10.606119',1,1,'{"metrica": 42}','{"testa": "pass", "testb": {"log": "the log", "result": "pass"}}',NULL,1,1,'2020-10-29 19:54:10.605920',NULL,'12345',NULL,NULL,NULL,'{"job_id": "12345", "a-metadata-field": "value"}',1);
-INSERT INTO core_testrun VALUES(3,'2020-10-29 19:54:12.339907',1,1,'{"metric1": 42}','{"test1": {"log": "test1 log", "result": "pass"}}','really long log',1,1,'2020-10-29 19:54:12.339797',NULL,'123',NULL,NULL,NULL,'{"metadata1": "value1", "metadata2": "value2", "job_id": "123"}',1);
-INSERT INTO core_testrun VALUES(4,'2020-10-29 19:54:16.074271',6,3,'{"json-metric-1": 42}','{"json-test-1": "pass", "json-test-2": {"log": "json-test-2 log", "result": "fail"}}',replace('sample log\n','\n',char(10)),1,1,'2020-10-29 19:54:16.074161',NULL,'jsonmetadatajobid1',NULL,NULL,NULL,'{"json-metadata-field-1": "json-metadata-field-1-value", "job_id": "jsonmetadatajobid1"}',1);
-INSERT INTO core_testrun VALUES(5,'2020-10-29 19:54:21.153914',6,3,NULL,'{"json-test-1": "pass", "json-test-2": {"log": "json-test-2 log", "result": "fail"}}',NULL,1,1,'2020-10-29 19:54:21.153789',NULL,'30f04b02-dae3-4c85-8812-33268b318e2a',NULL,NULL,NULL,NULL,1);
-INSERT INTO core_testrun VALUES(6,'2020-10-29 19:54:26.733591',6,3,NULL,'{"build/x86-gcc-9-defconfig-b9979cfa": "pass", "build/arm64-gcc-9-defconfig-5b09568e": "fail"}',NULL,1,1,'2020-10-29 19:54:26.733474',NULL,'0bccb805-c7c4-4bbb-ae3d-9c91aedcad38',NULL,NULL,NULL,NULL,1);
-INSERT INTO core_testrun VALUES(7,'2020-10-29 19:54:35.417940',6,3,NULL,'{"yaml-test-1": "pass", "yaml-test-2": {"log": "yaml-test-2 log", "result": "fail"}}',NULL,1,1,'2020-10-29 19:54:35.417826',NULL,'f0048cfb-25fd-4854-9dc0-08e2bb664a56',NULL,NULL,NULL,NULL,1);
-INSERT INTO core_testrun VALUES(8,'2020-10-29 19:54:37.535521',6,3,'{"json-metric-1": 42}',NULL,NULL,1,1,'2020-10-29 19:54:37.535403',NULL,'163222e8-260b-4a46-a67a-95af09bf2dd7',NULL,NULL,NULL,NULL,1);
-INSERT INTO core_testrun VALUES(9,'2020-10-29 19:54:39.515451',6,3,NULL,'{"single-test": "pass"}',NULL,1,1,'2020-10-29 19:54:39.515336',NULL,'de328702-1042-4127-883a-de81b49be598',NULL,NULL,NULL,NULL,1);
+INSERT INTO core_testrun VALUES(1,'2020-11-18 20:11:17.849669',1,1,NULL,NULL,NULL,0,1,'2020-11-18 20:11:17.849524',NULL,NULL,NULL,NULL,NULL,NULL,1);
+INSERT INTO core_testrun VALUES(2,'2020-11-18 20:11:35.440650',1,1,'{"metrica": 42}','{"testa": "pass", "testb": {"log": "the log", "result": "pass"}}',NULL,1,1,'2020-11-18 20:11:35.440523',NULL,'12345',NULL,NULL,NULL,'{"job_id": "12345", "a-metadata-field": "value"}',1);
+INSERT INTO core_testrun VALUES(3,'2020-11-18 20:11:37.150036',1,1,'{"metric1": 42}','{"test1": {"log": "test1 log", "result": "pass"}}','really long log',1,1,'2020-11-18 20:11:37.149915',NULL,'123',NULL,NULL,NULL,'{"metadata1": "value1", "metadata2": "value2", "job_id": "123"}',1);
+INSERT INTO core_testrun VALUES(4,'2020-11-18 20:11:41.164580',6,3,'{"json-metric-1": 42}','{"json-test-1": "pass", "json-test-2": {"log": "json-test-2 log", "result": "fail"}}',replace('sample log\n','\n',char(10)),1,1,'2020-11-18 20:11:41.164465',NULL,'jsonmetadatajobid1',NULL,NULL,NULL,'{"json-metadata-field-1": "json-metadata-field-1-value", "job_id": "jsonmetadatajobid1"}',1);
+INSERT INTO core_testrun VALUES(5,'2020-11-18 20:11:46.339507',6,3,NULL,'{"json-test-1": "pass", "json-test-2": {"log": "json-test-2 log", "result": "fail"}}',NULL,1,1,'2020-11-18 20:11:46.339395',NULL,'f2906910-3478-41c2-8767-b8771abaf3ad',NULL,NULL,NULL,NULL,1);
+INSERT INTO core_testrun VALUES(6,'2020-11-18 20:11:52.057926',6,3,NULL,'{"build/gcc-8-allnoconfig": "pass", "build/gcc-8-tinyconfig": "pass", "build/gcc-8-x86_64_defconfig": "pass"}',NULL,1,1,'2020-11-18 20:11:52.057809',NULL,'53552722-34bf-41e7-9457-735a4beca4c3',NULL,NULL,NULL,NULL,1);
+INSERT INTO core_testrun VALUES(7,'2020-11-18 20:11:54.276798',6,3,NULL,'{"build/gcc-9-defconfig-b9979cfa": "pass", "build/gcc-9-defconfig-5b09568e": "fail"}',NULL,1,1,'2020-11-18 20:11:54.276687',NULL,'b81ce6e3-d6c6-46a9-b287-8d6a49d1fed0',NULL,NULL,NULL,NULL,1);
+INSERT INTO core_testrun VALUES(8,'2020-11-18 20:12:06.906351',6,3,NULL,'{"yaml-test-1": "pass", "yaml-test-2": {"log": "yaml-test-2 log", "result": "fail"}}',NULL,1,1,'2020-11-18 20:12:06.906205',NULL,'743847c4-5b29-48c4-b1a6-0a0bec4cb776',NULL,NULL,NULL,NULL,1);
+INSERT INTO core_testrun VALUES(9,'2020-11-18 20:12:09.214796',6,3,'{"json-metric-1": 42}',NULL,NULL,1,1,'2020-11-18 20:12:09.214666',NULL,'9339863d-8e4f-4f11-b90c-edb1cf024a7e',NULL,NULL,NULL,NULL,1);
+INSERT INTO core_testrun VALUES(10,'2020-11-18 20:12:11.252427',6,3,NULL,'{"single-test": "pass"}',NULL,1,1,'2020-11-18 20:12:11.252316',NULL,'deb37471-8f6a-4e53-b6df-1dde80f69d18',NULL,NULL,NULL,NULL,1);
 CREATE TABLE IF NOT EXISTS "core_adminsubscription" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "email" varchar(1024) NOT NULL, "project_id" integer NOT NULL REFERENCES "core_project" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "ci_testjob" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "definition" text NULL, "submitted" bool NOT NULL, "fetched" bool NOT NULL, "last_fetch_attempt" datetime NULL, "job_id" varchar(128) NULL, "job_status" varchar(128) NULL, "backend_id" integer NOT NULL REFERENCES "ci_backend" ("id") DEFERRABLE INITIALLY DEFERRED, "target_id" integer NOT NULL REFERENCES "core_project" ("id") DEFERRABLE INITIALLY DEFERRED, "failure" text NULL, "testrun_id" integer NULL REFERENCES "core_testrun" ("id") DEFERRABLE INITIALLY DEFERRED, "can_resubmit" bool NOT NULL, "resubmitted_count" integer NOT NULL, "name" varchar(256) NULL, "target_build_id" integer NULL REFERENCES "core_build" ("id") DEFERRABLE INITIALLY DEFERRED, "fetch_attempts" integer NOT NULL, "created_at" datetime NULL, "fetched_at" datetime NULL, "submitted_at" datetime NULL, "environment" varchar(100) NOT NULL, "parent_job_id" integer NULL REFERENCES "ci_testjob" ("id") DEFERRABLE INITIALLY DEFERRED);
-INSERT INTO ci_testjob VALUES(1,NULL,0,0,NULL,NULL,NULL,1,1,NULL,1,0,0,NULL,1,0,'2020-10-29 19:53:53.778107',NULL,NULL,'',NULL);
+INSERT INTO ci_testjob VALUES(1,NULL,0,0,NULL,NULL,NULL,1,1,NULL,1,0,0,NULL,1,0,'2020-11-18 20:11:17.873279',NULL,NULL,'',NULL);
 CREATE TABLE IF NOT EXISTS "ci_backend" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "url" varchar(200) NOT NULL, "username" varchar(128) NOT NULL, "token" varchar(1024) NOT NULL, "implementation_type" varchar(64) NOT NULL, "poll_interval" integer NOT NULL, "name" varchar(128) NOT NULL UNIQUE, "max_fetch_attempts" integer NOT NULL, "backend_settings" text NULL, "poll_enabled" bool NOT NULL, "listen_enabled" bool NOT NULL);
 INSERT INTO ci_backend VALUES(1,'','','','null',60,'',3,NULL,1,1);
 CREATE TABLE IF NOT EXISTS "core_suiteversion" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "version" varchar(40) NULL, "first_seen" datetime NOT NULL, "suite_id" integer NOT NULL REFERENCES "core_suite" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "core_suitemetadata" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "kind" varchar(6) NOT NULL, "name" varchar(256) NULL, "description" text NULL, "instructions_to_reproduce" text NULL, "suite" varchar(256) NOT NULL);
 INSERT INTO core_suitemetadata VALUES(1,'test','my_passed_test',NULL,NULL,'my_suite');
 INSERT INTO core_suitemetadata VALUES(2,'test','my_failed_test',NULL,NULL,'my_suite');
 INSERT INTO core_suitemetadata VALUES(3,'test','my_xfailed_test',NULL,NULL,'my_suite');
@@ -470,125 +472,133 @@
 INSERT INTO core_suitemetadata VALUES(9,'metric','metrica',NULL,NULL,'/');
 INSERT INTO core_suitemetadata VALUES(10,'test','test1',NULL,NULL,'/');
 INSERT INTO core_suitemetadata VALUES(11,'metric','metric1',NULL,NULL,'/');
 INSERT INTO core_suitemetadata VALUES(12,'test','json-test-1',NULL,NULL,'/');
 INSERT INTO core_suitemetadata VALUES(13,'test','json-test-2',NULL,NULL,'/');
 INSERT INTO core_suitemetadata VALUES(14,'metric','json-metric-1',NULL,NULL,'/');
 INSERT INTO core_suitemetadata VALUES(15,'suite','-',NULL,NULL,'build');
-INSERT INTO core_suitemetadata VALUES(16,'test','x86-gcc-9-defconfig-b9979cfa',NULL,NULL,'build');
-INSERT INTO core_suitemetadata VALUES(17,'test','arm64-gcc-9-defconfig-5b09568e',NULL,NULL,'build');
-INSERT INTO core_suitemetadata VALUES(18,'test','yaml-test-1',NULL,NULL,'/');
-INSERT INTO core_suitemetadata VALUES(19,'test','yaml-test-2',NULL,NULL,'/');
-INSERT INTO core_suitemetadata VALUES(20,'test','single-test',NULL,NULL,'/');
+INSERT INTO core_suitemetadata VALUES(16,'test','gcc-8-allnoconfig',NULL,NULL,'build');
+INSERT INTO core_suitemetadata VALUES(17,'test','gcc-8-tinyconfig',NULL,NULL,'build');
+INSERT INTO core_suitemetadata VALUES(18,'test','gcc-8-x86_64_defconfig',NULL,NULL,'build');
+INSERT INTO core_suitemetadata VALUES(19,'test','gcc-9-defconfig-b9979cfa',NULL,NULL,'build');
+INSERT INTO core_suitemetadata VALUES(20,'test','gcc-9-defconfig-5b09568e',NULL,NULL,'build');
+INSERT INTO core_suitemetadata VALUES(21,'test','yaml-test-1',NULL,NULL,'/');
+INSERT INTO core_suitemetadata VALUES(22,'test','yaml-test-2',NULL,NULL,'/');
+INSERT INTO core_suitemetadata VALUES(23,'test','single-test',NULL,NULL,'/');
 CREATE TABLE IF NOT EXISTS "core_knownissue" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "title" varchar(1024) NOT NULL, "test_name" varchar(1024) NOT NULL, "url" varchar(200) NULL, "notes" text NULL, "active" bool NOT NULL, "intermittent" bool NOT NULL);
 CREATE TABLE IF NOT EXISTS "core_knownissue_environments" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "knownissue_id" integer NOT NULL REFERENCES "core_knownissue" ("id") DEFERRABLE INITIALLY DEFERRED, "environment_id" integer NOT NULL REFERENCES "core_environment" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "core_status" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "tests_pass" integer NOT NULL, "tests_fail" integer NOT NULL, "metrics_summary" real NOT NULL, "suite_id" integer NULL REFERENCES "core_suite" ("id") DEFERRABLE INITIALLY DEFERRED, "test_run_id" integer NOT NULL REFERENCES "core_testrun" ("id") DEFERRABLE INITIALLY DEFERRED, "tests_skip" integer NOT NULL, "suite_version_id" integer NULL REFERENCES "core_suiteversion" ("id") DEFERRABLE INITIALLY DEFERRED, "has_metrics" bool NOT NULL, "tests_xfail" integer NOT NULL);
 INSERT INTO core_status VALUES(1,2,1,0.0,NULL,1,1,NULL,1,0);
 INSERT INTO core_status VALUES(2,2,1,0.0,1,1,1,NULL,0,0);
 INSERT INTO core_status VALUES(3,2,0,42.0000000000000071,NULL,2,0,NULL,1,0);
 INSERT INTO core_status VALUES(4,2,0,42.0000000000000071,3,2,0,NULL,1,0);
 INSERT INTO core_status VALUES(5,1,0,42.0000000000000071,NULL,3,0,NULL,1,0);
 INSERT INTO core_status VALUES(6,1,0,42.0000000000000071,3,3,0,NULL,1,0);
 INSERT INTO core_status VALUES(7,1,1,42.0000000000000071,NULL,4,0,NULL,1,0);
 INSERT INTO core_status VALUES(8,1,1,42.0000000000000071,3,4,0,NULL,1,0);
 INSERT INTO core_status VALUES(9,1,1,0.0,NULL,5,0,NULL,1,0);
 INSERT INTO core_status VALUES(10,1,1,0.0,3,5,0,NULL,0,0);
-INSERT INTO core_status VALUES(11,1,1,0.0,NULL,6,0,NULL,1,0);
-INSERT INTO core_status VALUES(12,1,1,0.0,4,6,0,NULL,0,0);
+INSERT INTO core_status VALUES(11,3,0,0.0,NULL,6,0,NULL,1,0);
+INSERT INTO core_status VALUES(12,3,0,0.0,4,6,0,NULL,0,0);
 INSERT INTO core_status VALUES(13,1,1,0.0,NULL,7,0,NULL,1,0);
-INSERT INTO core_status VALUES(14,1,1,0.0,3,7,0,NULL,0,0);
-INSERT INTO core_status VALUES(15,0,0,42.0000000000000071,NULL,8,0,NULL,1,0);
-INSERT INTO core_status VALUES(16,0,0,42.0000000000000071,3,8,0,NULL,1,0);
-INSERT INTO core_status VALUES(17,1,0,0.0,NULL,9,0,NULL,1,0);
-INSERT INTO core_status VALUES(18,1,0,0.0,3,9,0,NULL,0,0);
+INSERT INTO core_status VALUES(14,1,1,0.0,4,7,0,NULL,0,0);
+INSERT INTO core_status VALUES(15,1,1,0.0,NULL,8,0,NULL,1,0);
+INSERT INTO core_status VALUES(16,1,1,0.0,3,8,0,NULL,0,0);
+INSERT INTO core_status VALUES(17,0,0,42.0000000000000071,NULL,9,0,NULL,1,0);
+INSERT INTO core_status VALUES(18,0,0,42.0000000000000071,3,9,0,NULL,1,0);
+INSERT INTO core_status VALUES(19,1,0,0.0,NULL,10,0,NULL,1,0);
+INSERT INTO core_status VALUES(20,1,0,0.0,3,10,0,NULL,0,0);
 CREATE TABLE IF NOT EXISTS "core_test_known_issues" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "test_id" integer NOT NULL REFERENCES "core_test" ("id") DEFERRABLE INITIALLY DEFERRED, "knownissue_id" integer NOT NULL REFERENCES "core_knownissue" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "core_notificationdelivery" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "subject" varchar(40) NULL, "txt" varchar(40) NULL, "html" varchar(40) NULL, "status_id" integer NOT NULL REFERENCES "core_projectstatus" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "core_build" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "version" varchar(100) NOT NULL, "created_at" datetime NOT NULL, "project_id" integer NOT NULL REFERENCES "core_project" ("id") DEFERRABLE INITIALLY DEFERRED, "datetime" datetime NOT NULL, "patch_id" varchar(1024) NULL, "patch_source_id" integer NULL REFERENCES "core_patchsource" ("id") DEFERRABLE INITIALLY DEFERRED, "keep_data" bool NOT NULL, "patch_baseline_id" integer NULL REFERENCES "core_build" ("id") DEFERRABLE INITIALLY DEFERRED);
-INSERT INTO core_build VALUES(1,'my_build','2020-10-29 19:53:53.715409',1,'2020-10-29 19:53:53.715283',NULL,NULL,0,NULL);
-INSERT INTO core_build VALUES(2,'my_build2','2020-10-29 19:53:53.719642',1,'2020-10-29 19:53:53.719536',NULL,NULL,0,NULL);
-INSERT INTO core_build VALUES(3,'my_build3','2020-10-29 19:53:53.722848',1,'2020-10-29 19:53:53.722743',NULL,NULL,0,NULL);
-INSERT INTO core_build VALUES(4,'my_build4','2020-10-29 19:53:53.726047',1,'2020-10-29 19:53:53.725942',NULL,NULL,0,NULL);
-INSERT INTO core_build VALUES(5,'my_build5','2020-10-29 19:53:53.729327',1,'2020-10-29 19:53:53.729220',NULL,NULL,0,NULL);
-INSERT INTO core_build VALUES(6,'my_build6','2020-10-29 19:53:53.732619',1,'2020-10-29 19:53:53.732517',NULL,NULL,0,NULL);
+INSERT INTO core_build VALUES(1,'my_build','2020-11-18 20:11:17.807089',1,'2020-11-18 20:11:17.806946',NULL,NULL,0,NULL);
+INSERT INTO core_build VALUES(2,'my_build2','2020-11-18 20:11:17.811430',1,'2020-11-18 20:11:17.811322',NULL,NULL,0,NULL);
+INSERT INTO core_build VALUES(3,'my_build3','2020-11-18 20:11:17.814565',1,'2020-11-18 20:11:17.814462',NULL,NULL,0,NULL);
+INSERT INTO core_build VALUES(4,'my_build4','2020-11-18 20:11:17.817927',1,'2020-11-18 20:11:17.817666',NULL,NULL,0,NULL);
+INSERT INTO core_build VALUES(5,'my_build5','2020-11-18 20:11:17.822339',1,'2020-11-18 20:11:17.822177',NULL,NULL,0,NULL);
+INSERT INTO core_build VALUES(6,'my_build6','2020-11-18 20:11:17.826207',1,'2020-11-18 20:11:17.826061',NULL,NULL,0,NULL);
 CREATE TABLE IF NOT EXISTS "core_buildplaceholder" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "version" varchar(100) NOT NULL, "build_deleted_at" datetime NOT NULL, "project_id" integer NOT NULL REFERENCES "core_project" ("id") DEFERRABLE INITIALLY DEFERRED);
 CREATE TABLE IF NOT EXISTS "core_annotation" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "build_id" integer NOT NULL UNIQUE REFERENCES "core_build" ("id") DEFERRABLE INITIALLY DEFERRED, "description" varchar(1024) NULL);
 CREATE TABLE IF NOT EXISTS "core_delayedreport" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "output_format" varchar(32) NOT NULL, "email_recipient" varchar(254) NULL, "email_recipient_notified" bool NOT NULL, "callback" varchar(200) NULL, "callback_token" varchar(128) NULL, "callback_notified" bool NOT NULL, "data_retention_days" smallint unsigned NOT NULL CHECK ("data_retention_days" >= 0), "output_text" text NULL, "output_html" text NULL, "error_message" text NULL, "status_code" smallint unsigned NULL CHECK ("status_code" >= 0), "created_at" datetime NOT NULL, "baseline_id" integer NULL REFERENCES "core_projectstatus" ("id") DEFERRABLE INITIALLY DEFERRED, "build_id" integer NOT NULL REFERENCES "core_build" ("id") DEFERRABLE INITIALLY DEFERRED, "template_id" integer NULL REFERENCES "core_emailtemplate" ("id") DEFERRABLE INITIALLY DEFERRED, "output_subject" text NULL);
-INSERT INTO core_delayedreport VALUES(1,'',NULL,0,NULL,NULL,0,5,NULL,NULL,NULL,NULL,'2020-10-29 19:53:53.787488',NULL,1,NULL,NULL);
+INSERT INTO core_delayedreport VALUES(1,'',NULL,0,NULL,NULL,0,5,NULL,NULL,NULL,NULL,'2020-11-18 20:11:17.884331',NULL,1,NULL,NULL);
 CREATE TABLE IF NOT EXISTS "core_subscription" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "email" varchar(1024) NULL, "project_id" integer NOT NULL REFERENCES "core_project" ("id") DEFERRABLE INITIALLY DEFERRED, "user_id" integer NULL REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED, "notification_strategy" varchar(32) NOT NULL);
 CREATE TABLE IF NOT EXISTS "core_emailtemplate" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(100) NOT NULL UNIQUE, "plain_text" text NOT NULL, "html" text NULL, "subject" varchar(1024) NULL);
 INSERT INTO core_emailtemplate VALUES(1,'my_emailtemplate','',NULL,NULL);
 CREATE TABLE IF NOT EXISTS "core_historicalemailtemplate" ("id" integer NOT NULL, "name" varchar(100) NOT NULL, "plain_text" text NOT NULL, "html" text NULL, "history_id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "history_change_reason" varchar(100) NULL, "history_date" datetime NOT NULL, "history_type" varchar(1) NOT NULL, "history_user_id" integer NULL REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED, "subject" varchar(1024) NULL);
-INSERT INTO core_historicalemailtemplate VALUES(1,'my_emailtemplate','',NULL,1,NULL,'2020-10-29 19:53:53.781650','+',NULL,NULL);
+INSERT INTO core_historicalemailtemplate VALUES(1,'my_emailtemplate','',NULL,1,NULL,'2020-11-18 20:11:17.877382','+',NULL,NULL);
 CREATE TABLE IF NOT EXISTS "core_group" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(100) NULL, "description" text NULL, "slug" varchar(100) NOT NULL UNIQUE);
 INSERT INTO core_group VALUES(1,NULL,NULL,'my_group');
 INSERT INTO core_group VALUES(2,NULL,NULL,'my_other_group');
 CREATE TABLE IF NOT EXISTS "core_project" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(100) NULL, "group_id" integer NOT NULL REFERENCES "core_group" ("id") DEFERRABLE INITIALLY DEFERRED, "is_public" bool NOT NULL, "html_mail" bool NOT NULL, "moderate_notifications" bool NOT NULL, "custom_email_template_id" integer NULL REFERENCES "core_emailtemplate" ("id") DEFERRABLE INITIALLY DEFERRED, "description" text NULL, "important_metadata_keys" text NULL, "enabled_plugins_list" text NULL, "wait_before_notification" integer NULL, "notification_timeout" integer NULL, "data_retention_days" integer NOT NULL, "project_settings" text NULL, "is_archived" bool NOT NULL, "slug" varchar(100) NOT NULL);
 INSERT INTO core_project VALUES(1,NULL,1,1,1,0,NULL,NULL,NULL,NULL,NULL,NULL,0,NULL,0,'my_project');
 INSERT INTO core_project VALUES(2,NULL,1,0,1,0,NULL,NULL,NULL,NULL,NULL,NULL,0,NULL,0,'my_private_project');
 CREATE TABLE IF NOT EXISTS "core_buildsummary" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "metrics_summary" real NULL, "has_metrics" bool NOT NULL, "tests_pass" integer NOT NULL, "tests_fail" integer NOT NULL, "tests_xfail" integer NOT NULL, "tests_skip" integer NOT NULL, "test_runs_total" integer NOT NULL, "test_runs_completed" integer NOT NULL, "test_runs_incomplete" integer NOT NULL, "build_id" integer NOT NULL REFERENCES "core_build" ("id") DEFERRABLE INITIALLY DEFERRED, "environment_id" integer NOT NULL REFERENCES "core_environment" ("id") DEFERRABLE INITIALLY DEFERRED);
 INSERT INTO core_buildsummary VALUES(1,42.0000000000000071,1,5,1,0,1,3,3,0,1,1);
-INSERT INTO core_buildsummary VALUES(2,42.0000000000000071,1,5,4,0,0,6,6,0,6,3);
+INSERT INTO core_buildsummary VALUES(2,42.0000000000000071,1,8,4,0,0,7,7,0,6,3);
 CREATE TABLE IF NOT EXISTS "core_suite" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "slug" varchar(256) NOT NULL, "name" varchar(256) NULL, "project_id" integer NOT NULL REFERENCES "core_project" ("id") DEFERRABLE INITIALLY DEFERRED, "metadata_id" integer NULL REFERENCES "core_suitemetadata" ("id") DEFERRABLE INITIALLY DEFERRED);
 INSERT INTO core_suite VALUES(1,'my_suite',NULL,1,NULL);
 INSERT INTO core_suite VALUES(2,'my_other_suite',NULL,1,NULL);
 INSERT INTO core_suite VALUES(3,'/',NULL,1,6);
 INSERT INTO core_suite VALUES(4,'build',NULL,1,15);
 CREATE TABLE IF NOT EXISTS "core_environment" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "slug" varchar(100) NOT NULL, "name" varchar(100) NULL, "project_id" integer NOT NULL REFERENCES "core_project" ("id") DEFERRABLE INITIALLY DEFERRED, "description" text NULL, "expected_test_runs" integer NULL);
 INSERT INTO core_environment VALUES(1,'my_env',NULL,1,NULL,0);
 INSERT INTO core_environment VALUES(2,'my_other_env',NULL,1,NULL,0);
 INSERT INTO core_environment VALUES(3,'test_submit_env',NULL,1,NULL,0);
 CREATE TABLE IF NOT EXISTS "core_metricthreshold" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(1024) NOT NULL, "value" real NOT NULL, "is_higher_better" bool NOT NULL, "environment_id" integer NOT NULL REFERENCES "core_environment" ("id") DEFERRABLE INITIALLY DEFERRED);
 INSERT INTO core_metricthreshold VALUES(1,'',42.0,0,1);
 CREATE TABLE IF NOT EXISTS "core_projectstatus" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "created_at" datetime NOT NULL, "build_id" integer NOT NULL UNIQUE REFERENCES "core_build" ("id") DEFERRABLE INITIALLY DEFERRED, "tests_fail" integer NOT NULL, "tests_pass" integer NOT NULL, "tests_skip" integer NOT NULL, "metrics_summary" real NULL, "notified" bool NOT NULL, "last_updated" datetime NULL, "approved" bool NOT NULL, "finished" bool NOT NULL, "has_metrics" bool NOT NULL, "notified_on_timeout" bool NULL, "test_runs_completed" integer NOT NULL, "test_runs_incomplete" integer NOT NULL, "test_runs_total" integer NOT NULL, "fixes" text NULL, "regressions" text NULL, "tests_xfail" integer NOT NULL, "baseline_id" integer NULL REFERENCES "core_build" ("id") DEFERRABLE INITIALLY DEFERRED);
-INSERT INTO core_projectstatus VALUES(1,'2020-10-29 19:53:53.717290',1,1,5,1,42.0000000000000071,0,'2020-10-29 19:54:12.454552',0,0,1,NULL,3,0,3,NULL,NULL,0,NULL);
-INSERT INTO core_projectstatus VALUES(2,'2020-10-29 19:53:53.720609',2,0,0,0,NULL,0,NULL,0,0,0,NULL,0,0,0,NULL,NULL,0,NULL);
-INSERT INTO core_projectstatus VALUES(3,'2020-10-29 19:53:53.723814',3,0,0,0,NULL,0,NULL,0,0,0,NULL,0,0,0,NULL,NULL,0,NULL);
-INSERT INTO core_projectstatus VALUES(4,'2020-10-29 19:53:53.727008',4,0,0,0,NULL,0,NULL,0,0,0,NULL,0,0,0,NULL,NULL,0,NULL);
-INSERT INTO core_projectstatus VALUES(5,'2020-10-29 19:53:53.730290',5,0,0,0,NULL,0,NULL,0,0,0,NULL,0,0,0,NULL,NULL,0,NULL);
-INSERT INTO core_projectstatus VALUES(6,'2020-10-29 19:53:53.733579',6,4,5,0,42.0000000000000071,0,'2020-10-29 19:54:39.616964',0,1,1,NULL,6,0,6,NULL,NULL,0,NULL);
+INSERT INTO core_projectstatus VALUES(1,'2020-11-18 20:11:17.809130',1,1,5,1,42.0000000000000071,0,'2020-11-18 20:11:37.266629',0,0,1,NULL,3,0,3,NULL,NULL,0,NULL);
+INSERT INTO core_projectstatus VALUES(2,'2020-11-18 20:11:17.812398',2,0,0,0,NULL,0,NULL,0,0,0,NULL,0,0,0,NULL,NULL,0,NULL);
+INSERT INTO core_projectstatus VALUES(3,'2020-11-18 20:11:17.815573',3,0,0,0,NULL,0,NULL,0,0,0,NULL,0,0,0,NULL,NULL,0,NULL);
+INSERT INTO core_projectstatus VALUES(4,'2020-11-18 20:11:17.819683',4,0,0,0,NULL,0,NULL,0,0,0,NULL,0,0,0,NULL,NULL,0,NULL);
+INSERT INTO core_projectstatus VALUES(5,'2020-11-18 20:11:17.823687',5,0,0,0,NULL,0,NULL,0,0,0,NULL,0,0,0,NULL,NULL,0,NULL);
+INSERT INTO core_projectstatus VALUES(6,'2020-11-18 20:11:17.827338',6,4,8,0,42.0000000000000071,0,'2020-11-18 20:12:11.347719',0,1,1,NULL,7,0,7,NULL,NULL,0,NULL);
 CREATE TABLE IF NOT EXISTS "core_attachment" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "filename" varchar(1024) NOT NULL, "data" BLOB NOT NULL, "length" integer NOT NULL, "test_run_id" integer NOT NULL REFERENCES "core_testrun" ("id") DEFERRABLE INITIALLY DEFERRED, "mimetype" varchar(128) NOT NULL);
 CREATE TABLE IF NOT EXISTS "core_groupmember" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "member_since" date NOT NULL, "group_id" integer NOT NULL REFERENCES "core_group" ("id") DEFERRABLE INITIALLY DEFERRED, "user_id" integer NOT NULL REFERENCES "auth_user" ("id") DEFERRABLE INITIALLY DEFERRED, "access" varchar(10) NOT NULL);
 CREATE TABLE IF NOT EXISTS "core_patchsource" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "name" varchar(256) NOT NULL UNIQUE, "username" varchar(128) NOT NULL, "url" varchar(200) NOT NULL, "implementation" varchar(256) NOT NULL, "password" varchar(128) NULL, "token" varchar(1024) NULL);
 CREATE TABLE IF NOT EXISTS "core_metric" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "result" real NOT NULL, "measurements" text NOT NULL, "suite_id" integer NOT NULL REFERENCES "core_suite" ("id") DEFERRABLE INITIALLY DEFERRED, "test_run_id" integer NOT NULL REFERENCES "core_testrun" ("id") DEFERRABLE INITIALLY DEFERRED, "name" varchar(256) NOT NULL, "metadata_id" integer NULL REFERENCES "core_suitemetadata" ("id") DEFERRABLE INITIALLY DEFERRED, "is_outlier" bool NOT NULL, "unit" varchar(30) NULL);
 INSERT INTO core_metric VALUES(1,42.0,'42.0',3,2,'metrica',9,0,NULL);
 INSERT INTO core_metric VALUES(2,42.0,'42.0',3,3,'metric1',11,0,NULL);
 INSERT INTO core_metric VALUES(3,42.0,'42.0',3,4,'json-metric-1',14,0,NULL);
-INSERT INTO core_metric VALUES(4,42.0,'42.0',3,8,'json-metric-1',14,0,NULL);
+INSERT INTO core_metric VALUES(4,42.0,'42.0',3,9,'json-metric-1',14,0,NULL);
 CREATE TABLE IF NOT EXISTS "core_test" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "result" bool NULL, "suite_id" integer NOT NULL REFERENCES "core_suite" ("id") DEFERRABLE INITIALLY DEFERRED, "test_run_id" integer NOT NULL REFERENCES "core_testrun" ("id") DEFERRABLE INITIALLY DEFERRED, "log" text NULL, "metadata_id" integer NULL REFERENCES "core_suitemetadata" ("id") DEFERRABLE INITIALLY DEFERRED, "has_known_issues" bool NULL, "name" varchar(256) NULL);
 INSERT INTO core_test VALUES(1,1,1,1,NULL,1,NULL,NULL);
 INSERT INTO core_test VALUES(2,0,1,1,NULL,2,NULL,NULL);
 INSERT INTO core_test VALUES(3,1,1,1,NULL,3,1,NULL);
 INSERT INTO core_test VALUES(4,NULL,1,1,NULL,4,NULL,NULL);
 INSERT INTO core_test VALUES(5,1,3,2,NULL,7,0,NULL);
 INSERT INTO core_test VALUES(6,1,3,2,'the log',8,0,NULL);
 INSERT INTO core_test VALUES(7,1,3,3,'test1 log',10,0,NULL);
 INSERT INTO core_test VALUES(8,1,3,4,NULL,12,0,NULL);
 INSERT INTO core_test VALUES(9,0,3,4,'json-test-2 log',13,0,NULL);
 INSERT INTO core_test VALUES(10,1,3,5,NULL,12,0,NULL);
 INSERT INTO core_test VALUES(11,0,3,5,'json-test-2 log',13,0,NULL);
 INSERT INTO core_test VALUES(12,1,4,6,NULL,16,0,NULL);
-INSERT INTO core_test VALUES(13,0,4,6,NULL,17,0,NULL);
-INSERT INTO core_test VALUES(14,1,3,7,NULL,18,0,NULL);
-INSERT INTO core_test VALUES(15,0,3,7,'yaml-test-2 log',19,0,NULL);
-INSERT INTO core_test VALUES(16,1,3,9,NULL,20,0,NULL);
+INSERT INTO core_test VALUES(13,1,4,6,NULL,17,0,NULL);
+INSERT INTO core_test VALUES(14,1,4,6,NULL,18,0,NULL);
+INSERT INTO core_test VALUES(15,1,4,7,NULL,19,0,NULL);
+INSERT INTO core_test VALUES(16,0,4,7,NULL,20,0,NULL);
+INSERT INTO core_test VALUES(17,1,3,8,NULL,21,0,NULL);
+INSERT INTO core_test VALUES(18,0,3,8,'yaml-test-2 log',22,0,NULL);
+INSERT INTO core_test VALUES(19,1,3,10,NULL,23,0,NULL);
 CREATE TABLE IF NOT EXISTS "django_celery_results_taskresult" ("id" integer NOT NULL PRIMARY KEY AUTOINCREMENT, "task_id" varchar(255) NOT NULL UNIQUE, "status" varchar(50) NOT NULL, "content_type" varchar(128) NOT NULL, "content_encoding" varchar(64) NOT NULL, "result" text NULL, "date_done" datetime NOT NULL, "traceback" text NULL, "meta" text NULL, "task_args" text NULL, "task_kwargs" text NULL, "task_name" varchar(255) NULL, "worker" varchar(100) NULL, "date_created" datetime NOT NULL);
 CREATE TABLE IF NOT EXISTS "django_session" ("session_key" varchar(40) NOT NULL PRIMARY KEY, "session_data" text NOT NULL, "expire_date" datetime NOT NULL);
 DELETE FROM sqlite_sequence;
 INSERT INTO sqlite_sequence VALUES('django_migrations',191);
-INSERT INTO sqlite_sequence VALUES('django_admin_log',8);
+INSERT INTO sqlite_sequence VALUES('django_admin_log',9);
 INSERT INTO sqlite_sequence VALUES('django_content_type',38);
 INSERT INTO sqlite_sequence VALUES('auth_permission',152);
 INSERT INTO sqlite_sequence VALUES('auth_user',1);
 INSERT INTO sqlite_sequence VALUES('auth_group',1);
-INSERT INTO sqlite_sequence VALUES('core_testrun',9);
+INSERT INTO sqlite_sequence VALUES('core_testrun',10);
 INSERT INTO sqlite_sequence VALUES('ci_testjob',1);
 INSERT INTO sqlite_sequence VALUES('ci_backend',1);
-INSERT INTO sqlite_sequence VALUES('core_suitemetadata',20);
+INSERT INTO sqlite_sequence VALUES('core_suitemetadata',23);
 INSERT INTO sqlite_sequence VALUES('core_knownissue_environments',0);
-INSERT INTO sqlite_sequence VALUES('core_status',18);
+INSERT INTO sqlite_sequence VALUES('core_status',20);
 INSERT INTO sqlite_sequence VALUES('core_notificationdelivery',0);
 INSERT INTO sqlite_sequence VALUES('core_build',6);
 INSERT INTO sqlite_sequence VALUES('core_annotation',0);
 INSERT INTO sqlite_sequence VALUES('core_delayedreport',1);
 INSERT INTO sqlite_sequence VALUES('core_subscription',0);
 INSERT INTO sqlite_sequence VALUES('core_emailtemplate',1);
 INSERT INTO sqlite_sequence VALUES('core_historicalemailtemplate',1);
@@ -599,15 +609,15 @@
 INSERT INTO sqlite_sequence VALUES('core_metricthreshold',1);
 INSERT INTO sqlite_sequence VALUES('core_projectstatus',6);
 INSERT INTO sqlite_sequence VALUES('auth_group_permissions',39);
 INSERT INTO sqlite_sequence VALUES('core_attachment',0);
 INSERT INTO sqlite_sequence VALUES('core_groupmember',0);
 INSERT INTO sqlite_sequence VALUES('core_patchsource',0);
 INSERT INTO sqlite_sequence VALUES('core_metric',4);
-INSERT INTO sqlite_sequence VALUES('core_test',16);
+INSERT INTO sqlite_sequence VALUES('core_test',19);
 INSERT INTO sqlite_sequence VALUES('django_celery_results_taskresult',0);
 INSERT INTO sqlite_sequence VALUES('auth_user_groups',1);
 INSERT INTO sqlite_sequence VALUES('core_buildsummary',2);
 CREATE UNIQUE INDEX "auth_group_permissions_group_id_permission_id_0cd325b0_uniq" ON "auth_group_permissions" ("group_id", "permission_id");
 CREATE INDEX "auth_group_permissions_group_id_b120cbf9" ON "auth_group_permissions" ("group_id");
 CREATE INDEX "auth_group_permissions_permission_id_84c5c92e" ON "auth_group_permissions" ("permission_id");
 CREATE UNIQUE INDEX "auth_user_groups_user_id_group_id_94350c0c_uniq" ON "auth_user_groups" ("user_id", "group_id");
```

### Comparing `squad-client-0.9/scripts/release` & `squad-client-0.9.1/scripts/release`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/README.md` & `squad-client-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/examples/example_template.html` & `squad-client-0.9.1/examples/example_template.html`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/examples/example_report.py` & `squad-client-0.9.1/examples/example_report.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/examples/build_report.py` & `squad-client-0.9.1/examples/build_report.py`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/examples/build_report_template.html` & `squad-client-0.9.1/examples/build_report_template.html`

 * *Files identical despite different names*

### Comparing `squad-client-0.9/LICENSE` & `squad-client-0.9.1/LICENSE`

 * *Files identical despite different names*

