# Comparing `tmp/bride-of-frankensystem-1.9.3.0.tar.gz` & `tmp/bride-of-frankensystem-1.9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\colby\Desktop\git\bride-of-frankensystem\dist\.tmp-xbsxbw8f\bride-of-frankensystem-1.9.3.0.tar", last modified: Mon Apr  1 07:38:57 2024, max compression
+gzip compressed data, was "C:\Users\colby\Desktop\git\bride-of-frankensystem\dist\.tmp-nxzgry96\bride-of-frankensystem-1.9.3.1.tar", last modified: Tue Apr  2 00:06:14 2024, max compression
```

## Comparing `bride-of-frankensystem-1.9.3.0.tar` & `bride-of-frankensystem-1.9.3.1.tar`

### file list

```diff
@@ -1,710 +1,710 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/BOFS/
--rw-rw-rw-   0        0        0    13232 2024-04-01 07:15:19.000000 bride-of-frankensystem-1.9.3.0/BOFS/BOFSFlask.py
--rw-rw-rw-   0        0        0     3937 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.0/BOFS/BOFSSession.py
--rw-rw-rw-   0        0        0    10136 2024-03-27 03:40:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/JSONQuestionnaire.py
--rw-rw-rw-   0        0        0     5740 2024-04-01 07:10:51.000000 bride-of-frankensystem-1.9.3.0/BOFS/JSONTable.py
--rw-rw-rw-   0        0        0     5635 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.0/BOFS/PageList.py
--rw-rw-rw-   0        0        0      117 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.0/BOFS/__init__.py
--rw-rw-rw-   0        0        0       65 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.0/BOFS/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/
--rw-rw-rw-   0        0        0     7006 2024-03-27 03:35:45.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/QuestionnaireResults.py
--rw-rw-rw-   0        0        0       22 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/__init__.py
--rw-rw-rw-   0        0        0    10020 2024-03-27 03:35:45.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/export_helpers.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/
--rw-rw-rw-   0        0        0     1142 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/export.html
--rw-rw-rw-   0        0        0      304 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/export_csv.html
--rw-rw-rw-   0        0        0      967 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/login_admin.html
--rw-rw-rw-   0        0        0     1340 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/preview_questionnaire.html
--rw-rw-rw-   0        0        0      144 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/preview_questionnaire_simple.html
--rw-rw-rw-   0        0        0      809 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/progress.html
--rw-rw-rw-   0        0        0     1780 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/progress_ajax.html
--rw-rw-rw-   0        0        0     3017 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/progress_summary_ajax.html
--rw-rw-rw-   0        0        0     3517 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/questionnaire_results.html
--rw-rw-rw-   0        0        0     1388 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/results.html
--rw-rw-rw-   0        0        0     1359 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/table_ajax.html
--rw-rw-rw-   0        0        0     1020 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/table_view.html
--rw-rw-rw-   0        0        0     5358 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/template_admin.html
--rw-rw-rw-   0        0        0     3141 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/util.py
--rw-rw-rw-   0        0        0    14926 2024-03-27 04:06:09.000000 bride-of-frankensystem-1.9.3.0/BOFS/admin/views.py
--rw-rw-rw-   0        0        0     1286 2024-01-07 00:02:19.000000 bride-of-frankensystem-1.9.3.0/BOFS/cli.py
--rw-rw-rw-   0        0        0     3420 2024-01-07 00:04:27.000000 bride-of-frankensystem-1.9.3.0/BOFS/create_app.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/BOFS/default/
--rw-rw-rw-   0        0        0       22 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/default/__init__.py
--rw-rw-rw-   0        0        0     9106 2023-10-23 23:01:54.000000 bride-of-frankensystem-1.9.3.0/BOFS/default/models.py
--rw-rw-rw-   0        0        0    15407 2024-03-27 03:35:45.000000 bride-of-frankensystem-1.9.3.0/BOFS/default/views.py
--rw-rw-rw-   0        0        0     2036 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.0/BOFS/globals.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/img/
--rw-rw-rw-   0        0        0     1235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/img/check.png
--rw-rw-rw-   0        0        0    26229 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/img/spinner32.gif
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/js/
--rw-rw-rw-   0        0        0    58078 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/js/bootstrap.min.js
--rw-rw-rw-   0        0        0    88147 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/js/jquery-3.4.1.min.js
--rw-rw-rw-   0        0        0  1219235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/js/plotly-latest.min.js
--rw-rw-rw-   0        0        0    21009 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/js/popper.min.js
--rw-rw-rw-   0        0        0     9389 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/loading.gif
--rw-rw-rw-   0        0        0      253 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/logo.png
--rw-rw-rw-   0        0        0     2929 2023-10-09 16:15:27.000000 bride-of-frankensystem-1.9.3.0/BOFS/static/style.css
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/
--rw-rw-rw-   0        0        0     3650 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/consent.html
--rw-rw-rw-   0        0        0      651 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/end.html
--rw-rw-rw-   0        0        0     1188 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/external_id.html
--rw-rw-rw-   0        0        0      345 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/instructions.html
--rw-rw-rw-   0        0        0      319 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/questionnaire.html
--rw-rw-rw-   0        0        0     7904 2023-10-09 16:13:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/questionnaire_macro.html
--rw-rw-rw-   0        0        0     5623 2024-04-01 07:17:50.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/template.html
--rw-rw-rw-   0        0        0     3722 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/unity_webgl.html
--rw-rw-rw-   0        0        0     4224 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.0/BOFS/templates/unity_webgl_fullscreen.html
--rw-rw-rw-   0        0        0    11904 2024-01-29 02:11:16.000000 bride-of-frankensystem-1.9.3.0/BOFS/util.py
--rw-rw-rw-   0        0        0     7817 2022-05-18 16:56:46.000000 bride-of-frankensystem-1.9.3.0/LICENSE
--rw-rw-rw-   0        0        0    12477 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2731 2024-03-27 04:18:48.000000 bride-of-frankensystem-1.9.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/bride_of_frankensystem.egg-info/
--rw-rw-rw-   0        0        0    12477 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/bride_of_frankensystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    34046 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/bride_of_frankensystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/bride_of_frankensystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/bride_of_frankensystem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       85 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/bride_of_frankensystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/bride_of_frankensystem.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/docs/
--rw-rw-rw-   0        0        0     1040 2024-03-26 01:01:09.000000 bride-of-frankensystem-1.9.3.0/docs/conf.py
--rw-rw-rw-   0        0        0     1125 2024-04-01 07:37:11.000000 bride-of-frankensystem-1.9.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/venv/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/_distutils_hack/
--rw-rw-rw-   0        0        0     4741 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-rw-rw-   0        0        0       44 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/_distutils_hack/override.py
--rw-rw-rw-   0        0        0     5792 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/_virtualenv.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/
--rw-rw-rw-   0        0        0      357 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/
--rw-rw-rw-   0        0        0      573 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-rw-rw-   0        0        0     9950 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-rw-rw-   0        0        0     9441 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cache.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/
--rw-rw-rw-   0        0        0      132 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-rw-rw-   0        0        0     6399 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-rw-rw-   0        0        0     7790 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-rw-rw-   0        0        0    28391 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-rw-rw-   0        0        0      760 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-rw-rw-   0        0        0     2472 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-rw-rw-   0        0        0     2614 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-rw-rw-   0        0        0    10788 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-rw-rw-   0        0        0     8300 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-rw-rw-   0        0        0    17097 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-rw-rw-   0        0        0     5076 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-rw-rw-   0        0        0      116 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/
--rw-rw-rw-   0        0        0     3736 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-rw-rw-   0        0        0     7524 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-rw-rw-   0        0        0     1685 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-rw-rw-   0        0        0     2958 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-rw-rw-   0        0        0     8944 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-rw-rw-   0        0        0     6629 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-rw-rw-   0        0        0     4904 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-rw-rw-   0        0        0     2951 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-rw-rw-   0        0        0     1703 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-rw-rw-   0        0        0     1132 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-rw-rw-   0        0        0     4762 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-rw-rw-   0        0        0    27851 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-rw-rw-   0        0        0    12203 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-rw-rw-   0        0        0     5697 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-rw-rw-   0        0        0     8064 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-rw-rw-   0        0        0     3526 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-rw-rw-   0        0        0     6168 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-rw-rw-   0        0        0    13153 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/configuration.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/
--rw-rw-rw-   0        0        0      858 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-rw-rw-   0        0        0     1172 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-rw-rw-   0        0        0      767 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-rw-rw-   0        0        0     5598 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-rw-rw-   0        0        0     1115 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-rw-rw-   0        0        0    12762 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/index/
--rw-rw-rw-   0        0        0       30 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-rw-rw-   0        0        0    17534 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-rw-rw-   0        0        0    36344 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-rw-rw-   0        0        0     6557 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/index/sources.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/locations/
--rw-rw-rw-   0        0        0    14444 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-rw-rw-   0        0        0     5871 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-rw-rw-   0        0        0     7918 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-rw-rw-   0        0        0     1579 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-rw-rw-   0        0        0      340 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/main.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/metadata/
--rw-rw-rw-   0        0        0     1660 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-rw-rw-   0        0        0    11103 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/metadata/base.py
--rw-rw-rw-   0        0        0     5089 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/
--rw-rw-rw-   0        0        0       63 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-rw-rw-   0        0        0      990 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-rw-rw-   0        0        0     6350 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-rw-rw-   0        0        0     2520 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-rw-rw-   0        0        0     1030 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-rw-rw-   0        0        0     9817 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/link.py
--rw-rw-rw-   0        0        0      738 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-rw-rw-   0        0        0     4520 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-rw-rw-   0        0        0     1907 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-rw-rw-   0        0        0     3858 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-rw-rw-   0        0        0     3500 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/wheel.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:52.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/
--rw-rw-rw-   0        0        0       50 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-rw-rw-   0        0        0    12190 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-rw-rw-   0        0        0     2100 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-rw-rw-   0        0        0     6016 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/download.py
--rw-rw-rw-   0        0        0     7627 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-rw-rw-   0        0        0    16729 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/session.py
--rw-rw-rw-   0        0        0     4059 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-rw-rw-   0        0        0     1791 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-rw-rw-   0        0        0     1119 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-rw-rw-   0        0        0     1177 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-rw-rw-   0        0        0     1945 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-rw-rw-   0        0        0     1063 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-rw-rw-   0        0        0     1405 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-rw-rw-   0        0        0     3047 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-rw-rw-   0        0        0     5109 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-rw-rw-   0        0        0     9770 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/install/
--rw-rw-rw-   0        0        0       51 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-rw-rw-   0        0        0     1298 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-rw-rw-   0        0        0     4158 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
--rw-rw-rw-   0        0        0    27412 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-rw-rw-   0        0        0    23838 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-rw-rw-   0        0        0     7215 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/pyproject.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/
--rw-rw-rw-   0        0        0     2793 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-rw-rw-   0        0        0    15285 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-rw-rw-   0        0        0    17421 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-rw-rw-   0        0        0    33804 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-rw-rw-   0        0        0     7584 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-rw-rw-   0        0        0     4117 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_tracker.py
--rw-rw-rw-   0        0        0    23748 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-rw-rw-   0        0        0      583 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/base.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-rw-rw-   0        0        0    18312 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-rw-rw-   0        0        0     5220 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-rw-rw-   0        0        0    18210 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-rw-rw-   0        0        0    26806 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-rw-rw-   0        0        0     5705 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-rw-rw-   0        0        0     9205 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-rw-rw-   0        0        0     2526 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-rw-rw-   0        0        0     5455 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-rw-rw-   0        0        0     9580 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-rw-rw-   0        0        0     6393 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-rw-rw-   0        0        0     1015 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-rw-rw-   0        0        0     1665 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-rw-rw-   0        0        0     1884 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-rw-rw-   0        0        0     5377 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-rw-rw-   0        0        0      242 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-rw-rw-   0        0        0     3627 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-rw-rw-   0        0        0     3206 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-rw-rw-   0        0        0     1249 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
--rw-rw-rw-   0        0        0     2203 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-rw-rw-   0        0        0     1169 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-rw-rw-   0        0        0     1055 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-rw-rw-   0        0        0     5893 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-rw-rw-   0        0        0      716 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-rw-rw-   0        0        0     3110 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-rw-rw-   0        0        0     4811 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-rw-rw-   0        0        0      795 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-rw-rw-   0        0        0    11532 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-rw-rw-   0        0        0    20432 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-rw-rw-   0        0        0     1193 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-rw-rw-   0        0        0     2952 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-rw-rw-   0        0        0     3196 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/parallel.py
--rw-rw-rw-   0        0        0      987 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/pkg_resources.py
--rw-rw-rw-   0        0        0     4697 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-rw-rw-   0        0        0    10058 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-rw-rw-   0        0        0     7662 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-rw-rw-   0        0        0     8906 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-rw-rw-   0        0        0     1759 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-rw-rw-   0        0        0     3459 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-rw-rw-   0        0        0     6163 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/
--rw-rw-rw-   0        0        0      596 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-rw-rw-   0        0        0    17804 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-rw-rw-   0        0        0     4945 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-rw-rw-   0        0        0    11596 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-rw-rw-   0        0        0    22414 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-rw-rw-   0        0        0    12247 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/
--rw-rw-rw-   0        0        0     4708 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/
--rw-rw-rw-   0        0        0      302 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-rw-rw-   0        0        0     4882 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-rw-rw-   0        0        0      805 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
--rw-rw-rw-   0        0        0       86 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-rw-rw-   0        0        0     4153 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-rw-rw-   0        0        0      856 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-rw-rw-   0        0        0      695 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-rw-rw-   0        0        0    14149 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-rw-rw-   0        0        0     2533 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-rw-rw-   0        0        0     4070 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-rw-rw-   0        0        0     7091 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-rw-rw-   0        0        0      690 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:53.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/certifi/
--rw-rw-rw-   0        0        0       62 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-rw-rw-   0        0        0      255 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-rw-rw-   0        0        0     2840 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/
--rw-rw-rw-   0        0        0     3271 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-rw-rw-   0        0        0    31254 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-rw-rw-   0        0        0     1757 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-rw-rw-   0        0        0     9411 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-rw-rw-   0        0        0     3839 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-rw-rw-   0        0        0     5110 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/
--rw-rw-rw-   0        0        0        1 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-rw-rw-   0        0        0     2747 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-rw-rw-   0        0        0     3590 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-rw-rw-   0        0        0     1200 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/compat.py
--rw-rw-rw-   0        0        0     1855 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-rw-rw-   0        0        0     1661 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-rw-rw-   0        0        0     3950 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-rw-rw-   0        0        0    10510 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-rw-rw-   0        0        0     3749 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-rw-rw-   0        0        0    13546 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-rw-rw-   0        0        0     1748 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-rw-rw-   0        0        0    31621 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-rw-rw-   0        0        0     1747 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-rw-rw-   0        0        0    20715 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-rw-rw-   0        0        0     1754 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-rw-rw-   0        0        0    13838 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-rw-rw-   0        0        0    25777 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-rw-rw-   0        0        0    19643 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-rw-rw-   0        0        0   105697 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-rw-rw-   0        0        0    99571 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-rw-rw-   0        0        0    98776 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-rw-rw-   0        0        0   102498 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-rw-rw-   0        0        0   131180 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-rw-rw-   0        0        0   103312 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-rw-rw-   0        0        0    95946 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-rw-rw-   0        0        0     5370 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-rw-rw-   0        0        0     3413 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-rw-rw-   0        0        0     2012 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-rw-rw-   0        0        0    25481 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-rw-rw-   0        0        0    19474 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-rw-rw-   0        0        0     6136 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-rw-rw-   0        0        0     4309 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-rw-rw-   0        0        0     3774 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-rw-rw-   0        0        0    12503 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-rw-rw-   0        0        0     2766 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-rw-rw-   0        0        0      242 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/version.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/
--rw-rw-rw-   0        0        0      239 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-rw-rw-   0        0        0    10517 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/
--rw-rw-rw-   0        0        0      581 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/
--rw-rw-rw-   0        0        0      274 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/__init__.py
--rw-rw-rw-   0        0        0      971 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py
--rw-rw-rw-   0        0        0    25707 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py
--rw-rw-rw-   0        0        0    26854 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
--rw-rw-rw-   0        0        0    92628 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py
--rw-rw-rw-   0        0        0    41495 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-rw-rw-   0        0        0    51059 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-rw-rw-   0        0        0    20739 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-rw-rw-   0        0        0    51965 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-rw-rw-   0        0        0    14811 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-rw-rw-   0        0        0     4989 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-rw-rw-   0        0        0    39109 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-rw-rw-   0        0        0    10820 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-rw-rw-   0        0        0    17720 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rw-rw-rw-   0        0        0    67766 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-rw-rw-   0        0        0    23513 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rw-rw-rw-   0        0        0    42943 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-rw-rw-   0        0        0    48414 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distro.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/
--rw-rw-rw-   0        0        0     1160 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py
--rw-rw-rw-   0        0        0    16728 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py
--rw-rw-rw-   0        0        0    32353 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py
--rw-rw-rw-   0        0        0    77040 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/
--rw-rw-rw-   0        0        0      109 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/__init__.py
--rw-rw-rw-   0        0        0     1013 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py
--rw-rw-rw-   0        0        0     1775 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py
--rw-rw-rw-   0        0        0     4931 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py
--rw-rw-rw-   0        0        0    83464 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/__init__.py
--rw-rw-rw-   0        0        0      919 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rw-rw-rw-   0        0        0      286 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/base.py
--rw-rw-rw-   0        0        0     2945 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rw-rw-rw-   0        0        0     3643 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py
--rw-rw-rw-   0        0        0    10588 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
--rw-rw-rw-   0        0        0    26897 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
--rw-rw-rw-   0        0        0     1214 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py
--rw-rw-rw-   0        0        0   117186 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py
--rw-rw-rw-   0        0        0    15759 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/
--rw-rw-rw-   0        0        0      679 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
--rw-rw-rw-   0        0        0     1715 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
--rw-rw-rw-   0        0        0     1776 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/
--rw-rw-rw-   0        0        0     3592 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
--rw-rw-rw-   0        0        0    14565 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py
--rw-rw-rw-   0        0        0     8925 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
--rw-rw-rw-   0        0        0    12836 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
--rw-rw-rw-   0        0        0    14766 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/
--rw-rw-rw-   0        0        0     5719 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
--rw-rw-rw-   0        0        0     7476 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py
--rw-rw-rw-   0        0        0     1413 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
--rw-rw-rw-   0        0        0     4551 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
--rw-rw-rw-   0        0        0     6357 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rw-rw-rw-   0        0        0     2309 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/
--rw-rw-rw-   0        0        0      849 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-rw-rw-   0        0        0     3453 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-rw-rw-   0        0        0      360 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-rw-rw-   0        0        0    12826 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-rw-rw-   0        0        0    42350 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-rw-rw-   0        0        0     1933 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-rw-rw-   0        0        0       21 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-rw-rw-   0        0        0   201849 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:54.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/
--rw-rw-rw-   0        0        0     1118 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-rw-rw-   0        0        0       20 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/_version.py
--rw-rw-rw-   0        0        0     1081 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-rw-rw-   0        0        0     6088 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-rw-rw-   0        0        0    38026 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1629 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8487 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4676 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30964 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15714 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/
--rw-rw-rw-   0        0        0      130 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/__init__.py
--rw-rw-rw-   0        0        0     3457 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/build.py
--rw-rw-rw-   0        0        0     6084 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/check.py
--rw-rw-rw-   0        0        0     4098 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py
--rw-rw-rw-   0        0        0     1253 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/compat.py
--rw-rw-rw-   0        0        0     1129 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py
--rw-rw-rw-   0        0        0     6100 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/
--rw-rw-rw-   0        0        0      563 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-rw-rw-   0        0        0    11201 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-rw-rw-   0        0        0     2463 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/meta.py
--rw-rw-rw-   0        0        0    13429 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/
--rw-rw-rw-   0        0        0   108287 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      562 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/
--rw-rw-rw-   0        0        0    12859 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-rw-rw-   0        0        0     1140 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-rw-rw-   0        0        0     3994 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-rw-rw-   0        0        0     4922 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-rw-rw-   0        0        0     2619 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-rw-rw-   0        0        0     6905 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-rw-rw-   0        0        0       80 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-rw-rw-   0        0        0     6416 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/
--rw-rw-rw-   0        0        0     5294 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/__init__.py
--rw-rw-rw-   0        0        0     2942 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/bar.py
--rw-rw-rw-   0        0        0     2655 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/colors.py
--rw-rw-rw-   0        0        0     1613 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/counter.py
--rw-rw-rw-   0        0        0     1461 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/spinner.py
--rw-rw-rw-   0        0        0   273394 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pyparsing.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/
--rw-rw-rw-   0        0        0     5113 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-rw-rw-   0        0        0      441 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-rw-rw-   0        0        0     1096 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-rw-rw-   0        0        0    21548 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-rw-rw-   0        0        0     6402 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-rw-rw-   0        0        0    10207 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-rw-rw-   0        0        0      465 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-rw-rw-   0        0        0     2045 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-rw-rw-   0        0        0    18430 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-rw-rw-   0        0        0     3250 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-rw-rw-   0        0        0     3972 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-rw-rw-   0        0        0      757 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-rw-rw-   0        0        0    34924 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-rw-rw-   0        0        0      695 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-rw-rw-   0        0        0    30168 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-rw-rw-   0        0        0     4188 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-rw-rw-   0        0        0     3005 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-rw-rw-   0        0        0    31394 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/
--rw-rw-rw-   0        0        0      537 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-rw-rw-   0        0        0      156 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-rw-rw-   0        0        0     5872 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-rw-rw-   0        0        0     1364 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-rw-rw-   0        0        0    17540 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-rw-rw-   0        0        0     4794 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-rw-rw-   0        0        0    34549 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/six.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/
--rw-rw-rw-   0        0        0    18257 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-rw-rw-   0        0        0     3314 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-rw-rw-   0        0        0     1944 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-rw-rw-   0        0        0     1496 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-rw-rw-   0        0        0     1376 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-rw-rw-   0        0        0     1908 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-rw-rw-   0        0        0     1383 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-rw-rw-   0        0        0     6645 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-rw-rw-   0        0        0     2790 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-rw-rw-   0        0        0     2145 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-rw-rw-   0        0        0     6691 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tomli/
--rw-rw-rw-   0        0        0      230 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-rw-rw-   0        0        0    22415 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-rw-rw-   0        0        0     2681 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/
--rw-rw-rw-   0        0        0     2763 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-rw-rw-   0        0        0    10811 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-rw-rw-   0        0        0       63 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-rw-rw-   0        0        0    20080 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-rw-rw-   0        0        0    37587 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-rw-rw-   0        0        0      957 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-rw-rw-   0        0        0    17649 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-rw-rw-   0        0        0    13922 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-rw-rw-   0        0        0    11034 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-rw-rw-   0        0        0     4538 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-rw-rw-   0        0        0    16900 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-rw-rw-   0        0        0    34449 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-rw-rw-   0        0        0     7097 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-rw-rw-   0        0        0     8217 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-rw-rw-   0        0        0     8579 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-rw-rw-   0        0        0     2440 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
--rw-rw-rw-   0        0        0      108 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-rw-rw-   0        0        0     1417 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-rw-rw-   0        0        0    34666 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:55.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/
--rw-rw-rw-   0        0        0      927 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
--rw-rw-rw-   0        0        0     5679 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
--rw-rw-rw-   0        0        0    19763 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-rw-rw-   0        0        0     5985 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-rw-rw-   0        0        0    28203 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/
--rw-rw-rw-   0        0        0     1155 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-rw-rw-   0        0        0     4920 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-rw-rw-   0        0        0     1605 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-rw-rw-   0        0        0      498 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-rw-rw-   0        0        0     4123 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-rw-rw-   0        0        0     3510 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-rw-rw-   0        0        0    21391 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-rw-rw-   0        0        0    17177 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-rw-rw-   0        0        0     6931 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-rw-rw-   0        0        0    10003 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-rw-rw-   0        0        0    14047 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-rw-rw-   0        0        0     5404 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/
--rw-rw-rw-   0        0        0    10579 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-rw-rw-   0        0        0     8979 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-rw-rw-   0        0        0     1305 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-rw-rw-   0        0        0     6563 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-rw-rw-   0        0        0     4307 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/
--rw-rw-rw-   0        0        0   108573 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-rw-rw-   0        0        0    24701 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1629 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8496 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4706 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30964 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15710 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-rw-rw-   0        0        0   232055 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/extern/
--rw-rw-rw-   0        0        0     2362 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/tests/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:51.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/tests/data/
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/tests/data/my-test-package-source/
--rw-rw-rw-   0        0        0      104 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/
--rw-rw-rw-   0        0        0     7494 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/__init__.py
--rw-rw-rw-   0        0        0      218 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_deprecation_warning.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/
--rw-rw-rw-   0        0        0      536 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-rw-rw-   0        0        0    20818 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-rw-rw-   0        0        0     8572 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-rw-rw-   0        0        0    14894 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-rw-rw-   0        0        0    47644 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-rw-rw-   0        0        0    18079 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:56.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/
--rw-rw-rw-   0        0        0      799 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-rw-rw-   0        0        0     5562 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-rw-rw-   0        0        0     4913 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-rw-rw-   0        0        0    35579 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py
--rw-rw-rw-   0        0        0    21537 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-rw-rw-   0        0        0    16030 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rw-rw-rw-   0        0        0     5773 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-rw-rw-   0        0        0     8022 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-rw-rw-   0        0        0    31612 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-rw-rw-   0        0        0    16495 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-rw-rw-   0        0        0     5963 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-rw-rw-   0        0        0     5637 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-rw-rw-   0        0        0     2776 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-rw-rw-   0        0        0    13117 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-rw-rw-   0        0        0    30138 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-rw-rw-   0        0        0     2822 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-rw-rw-   0        0        0     2753 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-rw-rw-   0        0        0     1298 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-rw-rw-   0        0        0     8397 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-rw-rw-   0        0        0     2017 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-rw-rw-   0        0        0      671 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-rw-rw-   0        0        0    11712 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-rw-rw-   0        0        0    19005 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-rw-rw-   0        0        0     7597 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-rw-rw-   0        0        0     4827 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-rw-rw-   0        0        0     9282 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-rw-rw-   0        0        0    14547 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-rw-rw-   0        0        0      139 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-rw-rw-   0        0        0     3491 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-rw-rw-   0        0        0     7778 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-rw-rw-   0        0        0    50421 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-rw-rw-   0        0        0     3577 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-rw-rw-   0        0        0    10515 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-rw-rw-   0        0        0    17784 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-rw-rw-   0        0        0     8148 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-rw-rw-   0        0        0    13407 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-rw-rw-   0        0        0     1973 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-rw-rw-   0        0        0    30483 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-rw-rw-   0        0        0    23540 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-rw-rw-   0        0        0      455 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/py35compat.py
--rw-rw-rw-   0        0        0      212 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-rw-rw-   0        0        0     3498 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-rw-rw-   0        0        0    21103 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-rw-rw-   0        0        0    12483 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-rw-rw-   0        0        0    14538 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-rw-rw-   0        0        0    20655 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-rw-rw-   0        0        0    13015 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-rw-rw-   0        0        0     5277 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-rw-rw-   0        0        0     2392 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_imp.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
--rw-rw-rw-   0        0        0       82 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-rw-rw-   0        0        0   117968 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-rw-rw-   0        0        0    16256 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-rw-rw-   0        0        0    15130 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/
--rw-rw-rw-   0        0        0      661 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-rw-rw-   0        0        0      497 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-rw-rw-   0        0        0    11488 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-rw-rw-   0        0        0     4378 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-rw-rw-   0        0        0     1629 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-rw-rw-   0        0        0     8493 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-rw-rw-   0        0        0     4700 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-rw-rw-   0        0        0    30964 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-rw-rw-   0        0        0    15710 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-rw-rw-   0        0        0     4200 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-rw-rw-   0        0        0    14665 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
--rw-rw-rw-   0        0        0   232055 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py
--rw-rw-rw-   0        0        0     7077 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/archive_util.py
--rw-rw-rw-   0        0        0    10536 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/build_meta.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/
--rw-rw-rw-   0        0        0      217 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-rw-rw-   0        0        0     2381 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/alias.py
--rw-rw-rw-   0        0        0    16604 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-rw-rw-   0        0        0     1182 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-rw-rw-   0        0        0     4415 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-rw-rw-   0        0        0    13212 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-rw-rw-   0        0        0     8751 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-rw-rw-   0        0        0     7012 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/develop.py
--rw-rw-rw-   0        0        0      960 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-rw-rw-   0        0        0    85791 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-rw-rw-   0        0        0    26126 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-rw-rw-   0        0        0     4906 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/install.py
--rw-rw-rw-   0        0        0     2203 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-rw-rw-   0        0        0     3875 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-rw-rw-   0        0        0     2593 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-rw-rw-   0        0        0     4946 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-rw-rw-   0        0        0      468 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/register.py
--rw-rw-rw-   0        0        0     2128 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-rw-rw-   0        0        0      658 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-rw-rw-   0        0        0     6413 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-rw-rw-   0        0        0     5086 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-rw-rw-   0        0        0     8088 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/test.py
--rw-rw-rw-   0        0        0      462 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/upload.py
--rw-rw-rw-   0        0        0     7218 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/upload_docs.py
--rw-rw-rw-   0        0        0    23153 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/config.py
--rw-rw-rw-   0        0        0      949 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/dep_util.py
--rw-rw-rw-   0        0        0     5499 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/depends.py
--rw-rw-rw-   0        0        0    43154 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/dist.py
--rw-rw-rw-   0        0        0     1555 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/errors.py
--rw-rw-rw-   0        0        0     1684 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/extension.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/extern/
--rw-rw-rw-   0        0        0     2407 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-rw-rw-   0        0        0     4873 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/glob.py
--rw-rw-rw-   0        0        0     3824 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/installer.py
--rw-rw-rw-   0        0        0      812 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/launch.py
--rw-rw-rw-   0        0        0      863 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/logging.py
--rw-rw-rw-   0        0        0     5217 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/monkey.py
--rw-rw-rw-   0        0        0    50561 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/msvc.py
--rw-rw-rw-   0        0        0     3093 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/namespaces.py
--rw-rw-rw-   0        0        0    40092 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/package_index.py
--rw-rw-rw-   0        0        0      245 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/py34compat.py
--rw-rw-rw-   0        0        0    14348 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/sandbox.py
--rw-rw-rw-   0        0        0      941 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-rw-rw-   0        0        0      144 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/version.py
--rw-rw-rw-   0        0        0     8288 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/wheel.py
--rw-rw-rw-   0        0        0      714 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/windows_support.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/
--rw-rw-rw-   0        0        0       23 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/__init__.py
--rw-rw-rw-   0        0        0      417 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/__main__.py
--rw-rw-rw-   0        0        0    19075 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/bdist_wheel.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/cli/
--rw-rw-rw-   0        0        0     2572 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/cli/__init__.py
--rw-rw-rw-   0        0        0     9498 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/cli/convert.py
--rw-rw-rw-   0        0        0     3364 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/cli/pack.py
--rw-rw-rw-   0        0        0      673 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/cli/unpack.py
--rw-rw-rw-   0        0        0    15930 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/macosx_libfile.py
--rw-rw-rw-   0        0        0     4344 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/metadata.py
--rw-rw-rw-   0        0        0     1257 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/pkginfo.py
--rw-rw-rw-   0        0        0      938 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/vendored/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/vendored/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/vendored/packaging/
--rw-rw-rw-   0        0        0        0 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
--rw-rw-rw-   0        0        0     1812 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/vendored/packaging/_typing.py
--rw-rw-rw-   0        0        0    29560 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
--rw-rw-rw-   0        0        0     7574 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/wheelfile.py
-drwxrwxrwx   0        0        0        0 2024-04-01 07:38:57.000000 bride-of-frankensystem-1.9.3.0/venv/Scripts/
--rw-rw-rw-   0        0        0     1193 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.0/venv/Scripts/activate_this.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/BOFS/
+-rw-rw-rw-   0        0        0    13780 2024-04-01 22:34:46.000000 bride-of-frankensystem-1.9.3.1/BOFS/BOFSFlask.py
+-rw-rw-rw-   0        0        0     3937 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.1/BOFS/BOFSSession.py
+-rw-rw-rw-   0        0        0    10136 2024-03-27 03:40:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/JSONQuestionnaire.py
+-rw-rw-rw-   0        0        0     5740 2024-04-01 07:10:51.000000 bride-of-frankensystem-1.9.3.1/BOFS/JSONTable.py
+-rw-rw-rw-   0        0        0     5635 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.1/BOFS/PageList.py
+-rw-rw-rw-   0        0        0      117 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.1/BOFS/__init__.py
+-rw-rw-rw-   0        0        0       65 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.1/BOFS/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/
+-rw-rw-rw-   0        0        0     7006 2024-03-27 03:35:45.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/QuestionnaireResults.py
+-rw-rw-rw-   0        0        0       22 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/__init__.py
+-rw-rw-rw-   0        0        0    10020 2024-03-27 03:35:45.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/export_helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/
+-rw-rw-rw-   0        0        0     1142 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/export.html
+-rw-rw-rw-   0        0        0      304 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/export_csv.html
+-rw-rw-rw-   0        0        0      967 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/login_admin.html
+-rw-rw-rw-   0        0        0     1340 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/preview_questionnaire.html
+-rw-rw-rw-   0        0        0      144 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/preview_questionnaire_simple.html
+-rw-rw-rw-   0        0        0      809 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/progress.html
+-rw-rw-rw-   0        0        0     1780 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/progress_ajax.html
+-rw-rw-rw-   0        0        0     3017 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/progress_summary_ajax.html
+-rw-rw-rw-   0        0        0     3517 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/questionnaire_results.html
+-rw-rw-rw-   0        0        0     1388 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/results.html
+-rw-rw-rw-   0        0        0     1359 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/table_ajax.html
+-rw-rw-rw-   0        0        0     1020 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/table_view.html
+-rw-rw-rw-   0        0        0     5358 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/template_admin.html
+-rw-rw-rw-   0        0        0     3141 2024-01-19 17:54:15.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/util.py
+-rw-rw-rw-   0        0        0    14926 2024-03-27 04:06:09.000000 bride-of-frankensystem-1.9.3.1/BOFS/admin/views.py
+-rw-rw-rw-   0        0        0     1286 2024-01-07 00:02:19.000000 bride-of-frankensystem-1.9.3.1/BOFS/cli.py
+-rw-rw-rw-   0        0        0     3682 2024-04-01 21:58:33.000000 bride-of-frankensystem-1.9.3.1/BOFS/create_app.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/BOFS/default/
+-rw-rw-rw-   0        0        0       22 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/default/__init__.py
+-rw-rw-rw-   0        0        0     9106 2023-10-23 23:01:54.000000 bride-of-frankensystem-1.9.3.1/BOFS/default/models.py
+-rw-rw-rw-   0        0        0    16926 2024-04-01 21:51:40.000000 bride-of-frankensystem-1.9.3.1/BOFS/default/views.py
+-rw-rw-rw-   0        0        0     2036 2024-01-06 23:57:32.000000 bride-of-frankensystem-1.9.3.1/BOFS/globals.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/img/
+-rw-rw-rw-   0        0        0     1235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/img/check.png
+-rw-rw-rw-   0        0        0    26229 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/img/spinner32.gif
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/js/
+-rw-rw-rw-   0        0        0    58078 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0    88147 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/js/jquery-3.4.1.min.js
+-rw-rw-rw-   0        0        0  1219235 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/js/plotly-latest.min.js
+-rw-rw-rw-   0        0        0    21009 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/js/popper.min.js
+-rw-rw-rw-   0        0        0     9389 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/loading.gif
+-rw-rw-rw-   0        0        0      253 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/logo.png
+-rw-rw-rw-   0        0        0     2929 2023-10-09 16:15:27.000000 bride-of-frankensystem-1.9.3.1/BOFS/static/style.css
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/
+-rw-rw-rw-   0        0        0     3650 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/consent.html
+-rw-rw-rw-   0        0        0      651 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/end.html
+-rw-rw-rw-   0        0        0     1188 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/external_id.html
+-rw-rw-rw-   0        0        0      345 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/instructions.html
+-rw-rw-rw-   0        0        0      319 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/questionnaire.html
+-rw-rw-rw-   0        0        0     7904 2023-10-09 16:13:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/questionnaire_macro.html
+-rw-rw-rw-   0        0        0     5623 2024-04-01 07:17:50.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/template.html
+-rw-rw-rw-   0        0        0     3722 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/unity_webgl.html
+-rw-rw-rw-   0        0        0     4224 2023-09-28 18:15:44.000000 bride-of-frankensystem-1.9.3.1/BOFS/templates/unity_webgl_fullscreen.html
+-rw-rw-rw-   0        0        0    11904 2024-01-29 02:11:16.000000 bride-of-frankensystem-1.9.3.1/BOFS/util.py
+-rw-rw-rw-   0        0        0     7817 2022-05-18 16:56:46.000000 bride-of-frankensystem-1.9.3.1/LICENSE
+-rw-rw-rw-   0        0        0    12477 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2731 2024-03-27 04:18:48.000000 bride-of-frankensystem-1.9.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/bride_of_frankensystem.egg-info/
+-rw-rw-rw-   0        0        0    12477 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/bride_of_frankensystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    34046 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/bride_of_frankensystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/bride_of_frankensystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/bride_of_frankensystem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       85 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/bride_of_frankensystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/bride_of_frankensystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/docs/
+-rw-rw-rw-   0        0        0     1040 2024-03-26 01:01:09.000000 bride-of-frankensystem-1.9.3.1/docs/conf.py
+-rw-rw-rw-   0        0        0     1125 2024-04-02 00:05:36.000000 bride-of-frankensystem-1.9.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/venv/
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/_distutils_hack/
+-rw-rw-rw-   0        0        0     4741 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/_distutils_hack/override.py
+-rw-rw-rw-   0        0        0     5792 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/_virtualenv.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/
+-rw-rw-rw-   0        0        0      357 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/
+-rw-rw-rw-   0        0        0      573 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-rw-rw-   0        0        0     9950 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-rw-rw-   0        0        0     9441 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cache.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/
+-rw-rw-rw-   0        0        0      132 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-rw-rw-   0        0        0     6399 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-rw-rw-   0        0        0     7790 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-rw-rw-   0        0        0    28391 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-rw-rw-   0        0        0      760 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-rw-rw-   0        0        0     2472 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-rw-rw-   0        0        0     2614 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-rw-rw-   0        0        0    10788 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-rw-rw-   0        0        0     8300 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-rw-rw-   0        0        0    17097 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-rw-rw-   0        0        0     5076 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-rw-rw-   0        0        0      116 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/
+-rw-rw-rw-   0        0        0     3736 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-rw-rw-   0        0        0     7524 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-rw-rw-   0        0        0     1685 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-rw-rw-   0        0        0     2958 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-rw-rw-   0        0        0     8944 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-rw-rw-   0        0        0     6629 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-rw-rw-   0        0        0     4904 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-rw-rw-   0        0        0     2951 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-rw-rw-   0        0        0     1703 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-rw-rw-   0        0        0     1132 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-rw-rw-   0        0        0     4762 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-rw-rw-   0        0        0    27851 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-rw-rw-   0        0        0    12203 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-rw-rw-   0        0        0     5697 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-rw-rw-   0        0        0     8064 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-rw-rw-   0        0        0     3526 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-rw-rw-   0        0        0     6168 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-rw-rw-   0        0        0    13153 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/configuration.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/
+-rw-rw-rw-   0        0        0      858 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-rw-rw-   0        0        0     1172 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-rw-rw-   0        0        0      767 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-rw-rw-   0        0        0     5598 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-rw-rw-   0        0        0     1115 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-rw-rw-   0        0        0    12762 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/index/
+-rw-rw-rw-   0        0        0       30 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-rw-rw-   0        0        0    17534 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-rw-rw-   0        0        0    36344 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-rw-rw-   0        0        0     6557 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/index/sources.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/locations/
+-rw-rw-rw-   0        0        0    14444 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-rw-rw-   0        0        0     5871 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-rw-rw-   0        0        0     7918 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-rw-rw-   0        0        0     1579 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-rw-rw-   0        0        0      340 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/main.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/metadata/
+-rw-rw-rw-   0        0        0     1660 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-rw-rw-   0        0        0    11103 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/metadata/base.py
+-rw-rw-rw-   0        0        0     5089 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/
+-rw-rw-rw-   0        0        0       63 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-rw-rw-   0        0        0      990 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-rw-rw-   0        0        0     6350 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-rw-rw-   0        0        0     2520 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-rw-rw-   0        0        0     1030 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-rw-rw-   0        0        0     9817 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-rw-rw-   0        0        0      738 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-rw-rw-   0        0        0     4520 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-rw-rw-   0        0        0     1907 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-rw-rw-   0        0        0     3858 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-rw-rw-   0        0        0     3500 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/wheel.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/
+-rw-rw-rw-   0        0        0       50 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-rw-rw-   0        0        0    12190 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-rw-rw-   0        0        0     2100 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-rw-rw-   0        0        0     6016 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-rw-rw-   0        0        0     7627 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-rw-rw-   0        0        0    16729 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-rw-rw-   0        0        0     4059 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-rw-rw-   0        0        0     1791 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-rw-rw-   0        0        0     1177 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-rw-rw-   0        0        0     1945 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-rw-rw-   0        0        0     1063 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-rw-rw-   0        0        0     1405 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-rw-rw-   0        0        0     3047 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-rw-rw-   0        0        0     5109 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-rw-rw-   0        0        0     9770 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/freeze.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/install/
+-rw-rw-rw-   0        0        0       51 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-rw-rw-   0        0        0     1298 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-rw-rw-   0        0        0     4158 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
+-rw-rw-rw-   0        0        0    27412 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-rw-rw-   0        0        0    23838 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-rw-rw-   0        0        0     7215 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/pyproject.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/
+-rw-rw-rw-   0        0        0     2793 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-rw-rw-   0        0        0    15285 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-rw-rw-   0        0        0    17421 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-rw-rw-   0        0        0    33804 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-rw-rw-   0        0        0     7584 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-rw-rw-   0        0        0     4117 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_tracker.py
+-rw-rw-rw-   0        0        0    23748 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-rw-rw-   0        0        0      583 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/base.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-rw-rw-   0        0        0    18312 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:10.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-rw-rw-   0        0        0     5220 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-rw-rw-   0        0        0    18210 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-rw-rw-   0        0        0    26806 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-rw-rw-   0        0        0     5705 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-rw-rw-   0        0        0     9205 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-rw-rw-   0        0        0     2526 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-rw-rw-   0        0        0     5455 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-rw-rw-   0        0        0     9580 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-rw-rw-   0        0        0     6393 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-rw-rw-   0        0        0     1015 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-rw-rw-   0        0        0     1665 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-rw-rw-   0        0        0     1884 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-rw-rw-   0        0        0     5377 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-rw-rw-   0        0        0      242 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-rw-rw-   0        0        0     3627 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-rw-rw-   0        0        0     3206 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-rw-rw-   0        0        0     1249 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
+-rw-rw-rw-   0        0        0     2203 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-rw-rw-   0        0        0     1169 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-rw-rw-   0        0        0     1055 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-rw-rw-   0        0        0     5893 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-rw-rw-   0        0        0      716 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-rw-rw-   0        0        0     3110 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-rw-rw-   0        0        0     4811 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-rw-rw-   0        0        0      795 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-rw-rw-   0        0        0    11532 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-rw-rw-   0        0        0    20432 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-rw-rw-   0        0        0     1193 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-rw-rw-   0        0        0     2952 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-rw-rw-   0        0        0     3196 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/parallel.py
+-rw-rw-rw-   0        0        0      987 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/pkg_resources.py
+-rw-rw-rw-   0        0        0     4697 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-rw-rw-   0        0        0    10058 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-rw-rw-   0        0        0     7662 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-rw-rw-   0        0        0     8906 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-rw-rw-   0        0        0     1759 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-rw-rw-   0        0        0     3459 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-rw-rw-   0        0        0     6163 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/wheel.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/
+-rw-rw-rw-   0        0        0      596 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-rw-rw-   0        0        0    17804 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-rw-rw-   0        0        0     4945 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-rw-rw-   0        0        0    11596 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-rw-rw-   0        0        0    22414 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-rw-rw-   0        0        0    12247 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/wheel_builder.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/
+-rw-rw-rw-   0        0        0     4708 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/
+-rw-rw-rw-   0        0        0      302 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-rw-rw-   0        0        0     4882 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-rw-rw-   0        0        0      805 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/
+-rw-rw-rw-   0        0        0       86 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-rw-rw-   0        0        0     4153 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-rw-rw-   0        0        0      856 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-rw-rw-   0        0        0      695 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-rw-rw-   0        0        0    14149 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-rw-rw-   0        0        0     2533 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-rw-rw-   0        0        0     4070 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-rw-rw-   0        0        0     7091 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-rw-rw-   0        0        0      690 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/certifi/
+-rw-rw-rw-   0        0        0       62 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-rw-rw-   0        0        0      255 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-rw-rw-   0        0        0     2840 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/certifi/core.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/
+-rw-rw-rw-   0        0        0     3271 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-rw-rw-   0        0        0    31254 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-rw-rw-   0        0        0     1757 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-rw-rw-   0        0        0     9411 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-rw-rw-   0        0        0     3839 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-rw-rw-   0        0        0     5110 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/
+-rw-rw-rw-   0        0        0        1 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-rw-rw-   0        0        0     2747 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-rw-rw-   0        0        0     3590 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-rw-rw-   0        0        0     1200 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/compat.py
+-rw-rw-rw-   0        0        0     1855 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-rw-rw-   0        0        0     1661 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-rw-rw-   0        0        0     3950 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-rw-rw-   0        0        0    10510 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-rw-rw-   0        0        0     3749 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-rw-rw-   0        0        0    13546 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-rw-rw-   0        0        0     1748 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-rw-rw-   0        0        0    31621 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-rw-rw-   0        0        0     1747 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-rw-rw-   0        0        0    20715 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-rw-rw-   0        0        0     1754 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-rw-rw-   0        0        0    13838 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-rw-rw-   0        0        0    25777 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-rw-rw-   0        0        0    19643 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-rw-rw-   0        0        0   105697 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-rw-rw-   0        0        0    99571 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-rw-rw-   0        0        0    98776 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-rw-rw-   0        0        0   102498 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-rw-rw-   0        0        0   131180 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-rw-rw-   0        0        0   103312 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-rw-rw-   0        0        0    95946 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-rw-rw-   0        0        0     5370 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-rw-rw-   0        0        0     3413 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-rw-rw-   0        0        0     2012 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-rw-rw-   0        0        0    25481 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-rw-rw-   0        0        0    19474 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-rw-rw-   0        0        0     6136 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-rw-rw-   0        0        0     4309 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-rw-rw-   0        0        0     3774 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-rw-rw-   0        0        0    12503 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-rw-rw-   0        0        0     2766 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-rw-rw-   0        0        0      242 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/version.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/
+-rw-rw-rw-   0        0        0      239 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10517 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/
+-rw-rw-rw-   0        0        0      581 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/
+-rw-rw-rw-   0        0        0      274 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/__init__.py
+-rw-rw-rw-   0        0        0      971 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py
+-rw-rw-rw-   0        0        0    25707 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py
+-rw-rw-rw-   0        0        0    26854 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
+-rw-rw-rw-   0        0        0    92628 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py
+-rw-rw-rw-   0        0        0    41495 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-rw-rw-   0        0        0    51059 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-rw-rw-   0        0        0    20739 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-rw-rw-   0        0        0    51965 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-rw-rw-   0        0        0    14811 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-rw-rw-   0        0        0     4989 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-rw-rw-   0        0        0    39109 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-rw-rw-   0        0        0    10820 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-rw-rw-   0        0        0    17720 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rw-rw-rw-   0        0        0    67766 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-rw-rw-   0        0        0    23513 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rw-rw-rw-   0        0        0    42943 2023-10-08 23:07:03.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+-rw-rw-rw-   0        0        0    48414 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distro.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/
+-rw-rw-rw-   0        0        0     1160 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py
+-rw-rw-rw-   0        0        0    16728 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py
+-rw-rw-rw-   0        0        0    32353 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py
+-rw-rw-rw-   0        0        0    77040 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/
+-rw-rw-rw-   0        0        0      109 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/__init__.py
+-rw-rw-rw-   0        0        0     1013 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py
+-rw-rw-rw-   0        0        0     1775 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py
+-rw-rw-rw-   0        0        0     4931 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py
+-rw-rw-rw-   0        0        0    83464 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/__init__.py
+-rw-rw-rw-   0        0        0      919 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-rw-rw-   0        0        0      286 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/base.py
+-rw-rw-rw-   0        0        0     2945 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-rw-rw-   0        0        0     3643 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py
+-rw-rw-rw-   0        0        0    10588 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
+-rw-rw-rw-   0        0        0    26897 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
+-rw-rw-rw-   0        0        0     1214 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py
+-rw-rw-rw-   0        0        0   117186 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py
+-rw-rw-rw-   0        0        0    15759 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/
+-rw-rw-rw-   0        0        0      679 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
+-rw-rw-rw-   0        0        0     1715 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
+-rw-rw-rw-   0        0        0     1776 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:11.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/
+-rw-rw-rw-   0        0        0     3592 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-rw-rw-   0        0        0    14565 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py
+-rw-rw-rw-   0        0        0     8925 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
+-rw-rw-rw-   0        0        0    12836 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
+-rw-rw-rw-   0        0        0    14766 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/
+-rw-rw-rw-   0        0        0     5719 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
+-rw-rw-rw-   0        0        0     7476 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py
+-rw-rw-rw-   0        0        0     1413 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
+-rw-rw-rw-   0        0        0     4551 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
+-rw-rw-rw-   0        0        0     6357 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-rw-rw-   0        0        0     2309 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/
+-rw-rw-rw-   0        0        0      849 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-rw-rw-   0        0        0     3453 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-rw-rw-   0        0        0      360 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-rw-rw-   0        0        0    12826 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-rw-rw-   0        0        0    42350 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-rw-rw-   0        0        0     1933 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-rw-rw-   0        0        0       21 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-rw-rw-   0        0        0   201849 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/
+-rw-rw-rw-   0        0        0     1118 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-rw-rw-   0        0        0       20 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/_version.py
+-rw-rw-rw-   0        0        0     1081 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-rw-rw-   0        0        0     6088 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-rw-rw-   0        0        0    38026 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1629 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8487 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4676 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30964 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15714 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/version.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/
+-rw-rw-rw-   0        0        0      130 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/__init__.py
+-rw-rw-rw-   0        0        0     3457 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/build.py
+-rw-rw-rw-   0        0        0     6084 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/check.py
+-rw-rw-rw-   0        0        0     4098 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-rw-rw-   0        0        0     1253 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/compat.py
+-rw-rw-rw-   0        0        0     1129 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-rw-rw-   0        0        0     6100 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/in_process/
+-rw-rw-rw-   0        0        0      563 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-rw-rw-   0        0        0    11201 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-rw-rw-   0        0        0     2463 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/meta.py
+-rw-rw-rw-   0        0        0    13429 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/
+-rw-rw-rw-   0        0        0   108287 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      562 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/
+-rw-rw-rw-   0        0        0    12859 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-rw-rw-   0        0        0     1140 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-rw-rw-   0        0        0     3994 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-rw-rw-   0        0        0     4922 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-rw-rw-   0        0        0     2619 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-rw-rw-   0        0        0     6905 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-rw-rw-   0        0        0       80 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-rw-rw-   0        0        0     6416 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/
+-rw-rw-rw-   0        0        0     5294 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/__init__.py
+-rw-rw-rw-   0        0        0     2942 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/bar.py
+-rw-rw-rw-   0        0        0     2655 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/colors.py
+-rw-rw-rw-   0        0        0     1613 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/counter.py
+-rw-rw-rw-   0        0        0     1461 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/spinner.py
+-rw-rw-rw-   0        0        0   273394 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pyparsing.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/
+-rw-rw-rw-   0        0        0     5113 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-rw-rw-   0        0        0     1096 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-rw-rw-   0        0        0    21548 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-rw-rw-   0        0        0     6402 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-rw-rw-   0        0        0    10207 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-rw-rw-   0        0        0      465 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-rw-rw-   0        0        0     2045 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-rw-rw-   0        0        0    18430 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-rw-rw-   0        0        0     3250 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-rw-rw-   0        0        0     3972 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-rw-rw-   0        0        0      757 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-rw-rw-   0        0        0    34924 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-rw-rw-   0        0        0      695 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-rw-rw-   0        0        0    30168 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-rw-rw-   0        0        0     4188 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-rw-rw-   0        0        0     3005 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-rw-rw-   0        0        0    31394 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/
+-rw-rw-rw-   0        0        0      537 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-rw-rw-   0        0        0      156 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-rw-rw-   0        0        0     5872 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-rw-rw-   0        0        0     1364 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-rw-rw-   0        0        0    17540 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-rw-rw-   0        0        0     4794 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-rw-rw-   0        0        0    34549 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/six.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/
+-rw-rw-rw-   0        0        0    18257 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-rw-rw-   0        0        0     3314 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-rw-rw-   0        0        0     1944 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-rw-rw-   0        0        0     1496 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-rw-rw-   0        0        0     1376 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-rw-rw-   0        0        0     1908 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-rw-rw-   0        0        0     1383 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-rw-rw-   0        0        0     6645 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-rw-rw-   0        0        0     2790 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-rw-rw-   0        0        0     2145 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-rw-rw-   0        0        0     6691 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tomli/
+-rw-rw-rw-   0        0        0      230 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-rw-rw-   0        0        0    22415 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-rw-rw-   0        0        0     2681 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/
+-rw-rw-rw-   0        0        0     2763 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-rw-rw-   0        0        0    10811 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-rw-rw-   0        0        0       63 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-rw-rw-   0        0        0    20080 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-rw-rw-   0        0        0    37587 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-rw-rw-   0        0        0    17649 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-rw-rw-   0        0        0    13922 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-rw-rw-   0        0        0    11034 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-rw-rw-   0        0        0     4538 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-rw-rw-   0        0        0    16900 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-rw-rw-   0        0        0    34449 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-rw-rw-   0        0        0     7097 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-rw-rw-   0        0        0     8217 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-rw-rw-   0        0        0     8579 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-rw-rw-   0        0        0     2440 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/
+-rw-rw-rw-   0        0        0      108 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-rw-rw-   0        0        0     1417 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-rw-rw-   0        0        0    34666 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:12.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/
+-rw-rw-rw-   0        0        0      927 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
+-rw-rw-rw-   0        0        0     5679 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
+-rw-rw-rw-   0        0        0    19763 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-rw-rw-   0        0        0     5985 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-rw-rw-   0        0        0    28203 2023-10-08 23:07:04.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/
+-rw-rw-rw-   0        0        0     1155 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-rw-rw-   0        0        0     4920 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-rw-rw-   0        0        0     1605 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-rw-rw-   0        0        0      498 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-rw-rw-   0        0        0     4123 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-rw-rw-   0        0        0     3510 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-rw-rw-   0        0        0    21391 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-rw-rw-   0        0        0    17177 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-rw-rw-   0        0        0     6931 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-rw-rw-   0        0        0    10003 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-rw-rw-   0        0        0    14047 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-rw-rw-   0        0        0     5404 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/
+-rw-rw-rw-   0        0        0    10579 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-rw-rw-   0        0        0     8979 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-rw-rw-   0        0        0     1305 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-rw-rw-   0        0        0     6563 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-rw-rw-   0        0        0     4307 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/
+-rw-rw-rw-   0        0        0   108573 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+-rw-rw-rw-   0        0        0    24701 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1629 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8496 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4706 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30964 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15710 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-rw-rw-   0        0        0   232055 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/extern/
+-rw-rw-rw-   0        0        0     2362 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/extern/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/tests/
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:09.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/tests/data/
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/tests/data/my-test-package-source/
+-rw-rw-rw-   0        0        0      104 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/
+-rw-rw-rw-   0        0        0     7494 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/__init__.py
+-rw-rw-rw-   0        0        0      218 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_deprecation_warning.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/
+-rw-rw-rw-   0        0        0      536 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-rw-rw-   0        0        0    20818 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-rw-rw-   0        0        0     8572 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-rw-rw-   0        0        0    14894 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-rw-rw-   0        0        0    47644 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-rw-rw-   0        0        0    18079 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/cmd.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/
+-rw-rw-rw-   0        0        0      799 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-rw-rw-   0        0        0     5562 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-rw-rw-   0        0        0     4913 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-rw-rw-   0        0        0    35579 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rw-rw-rw-   0        0        0    21537 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0    16030 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rw-rw-rw-   0        0        0     5773 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-rw-rw-   0        0        0     8022 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-rw-rw-   0        0        0    31612 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-rw-rw-   0        0        0    16495 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-rw-rw-   0        0        0     5963 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-rw-rw-   0        0        0     5637 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-rw-rw-   0        0        0     2776 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-rw-rw-   0        0        0    13117 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-rw-rw-   0        0        0    30138 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-rw-rw-   0        0        0     2822 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-rw-rw-   0        0        0     2753 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     1298 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-rw-rw-   0        0        0     8397 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-rw-rw-   0        0        0     2017 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-rw-rw-   0        0        0      671 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-rw-rw-   0        0        0    11712 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-rw-rw-   0        0        0    19005 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-rw-rw-   0        0        0     7597 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-rw-rw-   0        0        0     4827 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-rw-rw-   0        0        0     9282 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-rw-rw-   0        0        0    14547 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-rw-rw-   0        0        0      139 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-rw-rw-   0        0        0     3491 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-rw-rw-   0        0        0     7778 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-rw-rw-   0        0        0    50421 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-rw-rw-   0        0        0     3577 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-rw-rw-   0        0        0    10515 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-rw-rw-   0        0        0    17784 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-rw-rw-   0        0        0     8148 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-rw-rw-   0        0        0    13407 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-rw-rw-   0        0        0     1973 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-rw-rw-   0        0        0    30483 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-rw-rw-   0        0        0    23540 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-rw-rw-   0        0        0      455 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/py35compat.py
+-rw-rw-rw-   0        0        0      212 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-rw-rw-   0        0        0     3498 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-rw-rw-   0        0        0    21103 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-rw-rw-   0        0        0    12483 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-rw-rw-   0        0        0    14538 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-rw-rw-   0        0        0    20655 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-rw-rw-   0        0        0    13015 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-rw-rw-   0        0        0     5277 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-rw-rw-   0        0        0     2392 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_imp.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:13.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/
+-rw-rw-rw-   0        0        0       82 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-rw-rw-   0        0        0   117968 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-rw-rw-   0        0        0    16256 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-rw-rw-   0        0        0    15130 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/
+-rw-rw-rw-   0        0        0      661 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-rw-rw-   0        0        0      497 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-rw-rw-   0        0        0    11488 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-rw-rw-   0        0        0     4378 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-rw-rw-   0        0        0     1629 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-rw-rw-   0        0        0     8493 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-rw-rw-   0        0        0     4700 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-rw-rw-   0        0        0    30964 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-rw-rw-   0        0        0    15710 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-rw-rw-   0        0        0     4200 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-rw-rw-   0        0        0    14665 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+-rw-rw-rw-   0        0        0   232055 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py
+-rw-rw-rw-   0        0        0     7077 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/archive_util.py
+-rw-rw-rw-   0        0        0    10536 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/build_meta.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/
+-rw-rw-rw-   0        0        0      217 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-rw-rw-   0        0        0     2381 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/alias.py
+-rw-rw-rw-   0        0        0    16604 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-rw-rw-   0        0        0     1182 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-rw-rw-   0        0        0     4415 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-rw-rw-   0        0        0    13212 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-rw-rw-   0        0        0     8751 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-rw-rw-   0        0        0     7012 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/develop.py
+-rw-rw-rw-   0        0        0      960 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-rw-rw-   0        0        0    85791 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-rw-rw-   0        0        0    26126 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-rw-rw-   0        0        0     4906 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/install.py
+-rw-rw-rw-   0        0        0     2203 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-rw-rw-   0        0        0     3875 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-rw-rw-   0        0        0     2593 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-rw-rw-   0        0        0     4946 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-rw-rw-   0        0        0      468 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/register.py
+-rw-rw-rw-   0        0        0     2128 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-rw-rw-   0        0        0      658 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-rw-rw-   0        0        0     6413 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-rw-rw-   0        0        0     5086 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-rw-rw-   0        0        0     8088 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/test.py
+-rw-rw-rw-   0        0        0      462 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/upload.py
+-rw-rw-rw-   0        0        0     7218 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/upload_docs.py
+-rw-rw-rw-   0        0        0    23153 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/config.py
+-rw-rw-rw-   0        0        0      949 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/dep_util.py
+-rw-rw-rw-   0        0        0     5499 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/depends.py
+-rw-rw-rw-   0        0        0    43154 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/dist.py
+-rw-rw-rw-   0        0        0     1555 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/errors.py
+-rw-rw-rw-   0        0        0     1684 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/extension.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/extern/
+-rw-rw-rw-   0        0        0     2407 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-rw-rw-   0        0        0     4873 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/glob.py
+-rw-rw-rw-   0        0        0     3824 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/installer.py
+-rw-rw-rw-   0        0        0      812 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/launch.py
+-rw-rw-rw-   0        0        0      863 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/logging.py
+-rw-rw-rw-   0        0        0     5217 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/monkey.py
+-rw-rw-rw-   0        0        0    50561 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/msvc.py
+-rw-rw-rw-   0        0        0     3093 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/namespaces.py
+-rw-rw-rw-   0        0        0    40092 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/package_index.py
+-rw-rw-rw-   0        0        0      245 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/py34compat.py
+-rw-rw-rw-   0        0        0    14348 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/sandbox.py
+-rw-rw-rw-   0        0        0      941 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-rw-rw-   0        0        0      144 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/version.py
+-rw-rw-rw-   0        0        0     8288 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/wheel.py
+-rw-rw-rw-   0        0        0      714 2023-10-08 23:07:02.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/windows_support.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/
+-rw-rw-rw-   0        0        0       23 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/__init__.py
+-rw-rw-rw-   0        0        0      417 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/__main__.py
+-rw-rw-rw-   0        0        0    19075 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/bdist_wheel.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/cli/
+-rw-rw-rw-   0        0        0     2572 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/cli/__init__.py
+-rw-rw-rw-   0        0        0     9498 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/cli/convert.py
+-rw-rw-rw-   0        0        0     3364 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/cli/pack.py
+-rw-rw-rw-   0        0        0      673 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/cli/unpack.py
+-rw-rw-rw-   0        0        0    15930 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/macosx_libfile.py
+-rw-rw-rw-   0        0        0     4344 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/metadata.py
+-rw-rw-rw-   0        0        0     1257 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/pkginfo.py
+-rw-rw-rw-   0        0        0      938 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/util.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/vendored/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/vendored/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/vendored/packaging/
+-rw-rw-rw-   0        0        0        0 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
+-rw-rw-rw-   0        0        0     1812 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/vendored/packaging/_typing.py
+-rw-rw-rw-   0        0        0    29560 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
+-rw-rw-rw-   0        0        0     7574 2023-10-08 23:07:01.000000 bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/wheelfile.py
+drwxrwxrwx   0        0        0        0 2024-04-02 00:06:14.000000 bride-of-frankensystem-1.9.3.1/venv/Scripts/
+-rw-rw-rw-   0        0        0     1193 2023-10-08 23:07:05.000000 bride-of-frankensystem-1.9.3.1/venv/Scripts/activate_this.py
```

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/BOFSFlask.py` & `bride-of-frankensystem-1.9.3.1/BOFS/BOFSFlask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import jinja2
 import json
 import toml
 import os
 import random
-from flask import Flask,  send_from_directory, Response
+from flask import Flask, send_from_directory, Response, Blueprint
 from flask_sqlalchemy import SQLAlchemy
 from flask_compress import Compress
 from BOFS import util
 from .BOFSSession import BOFSSessionInterface
 from .JSONQuestionnaire import JSONQuestionnaire
 from .JSONTable import JSONTable
 from .PageList import PageList
@@ -45,21 +45,21 @@
         self.add_url_rule("/consent.html", endpoint="consent_html", view_func=self.route_consent)
         self.register_error_handler(404, self.page_not_found)
 
         default_templates_path = os.path.join(self.bofs_path, "templates")
         project_templates_path = os.path.join(self.instance_path, 'templates')
 
         # Allows developers of BOFS deployments to override BOFS templates
-        my_loader = jinja2.ChoiceLoader([
+        self.my_loader = jinja2.ChoiceLoader([
             self.jinja_loader,
             jinja2.FileSystemLoader(default_templates_path),
             jinja2.FileSystemLoader(project_templates_path),
         ])
 
-        self.jinja_loader = my_loader
+        self.jinja_loader = self.my_loader
 
         self.jinja_env.add_extension("jinja2.ext.do")
 
         # allows flat_page_list variable to be accessible from all templates
         self.template_context_processors[None].append(self.inject_jinja_vars)
         self.before_request_funcs.setdefault(None, []).append(self.before_request_)
 
@@ -121,14 +121,25 @@
         elif filename.endswith(".toml"):
             self.config.from_file(filename, load=toml.load)
         elif filename.endswith(".json"):
             self.config.from_file(filename, load=json.load)
         else:
             print("Error: Cannot load configuration file.")
 
+    def load_empty_blueprint(self, blueprint_path):
+        print("Creating empty blueprint: %s" % blueprint_path)
+
+        blueprint_var = Blueprint(blueprint_path, blueprint_path,
+                                  static_url_path='/' + blueprint_path,
+                                  template_folder=os.path.join(blueprint_path, 'templates'),
+                                  static_folder=os.path.join(blueprint_path, 'static'))
+
+        self.register_blueprint(blueprint_var)
+        #self.my_loader.loaders.
+
     def load_blueprint(self, blueprint_path, blueprint_name=None, try_to_load_models=True) -> None:
         print("Loaded blueprint: %s" % blueprint_path)
 
         if blueprint_name is None:
             blueprint_name = blueprint_path
 
         blueprint = __import__(blueprint_path + ".views", fromlist=["views"])
```

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/BOFSSession.py` & `bride-of-frankensystem-1.9.3.1/BOFS/BOFSSession.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/JSONQuestionnaire.py` & `bride-of-frankensystem-1.9.3.1/BOFS/JSONQuestionnaire.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/JSONTable.py` & `bride-of-frankensystem-1.9.3.1/BOFS/JSONTable.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/PageList.py` & `bride-of-frankensystem-1.9.3.1/BOFS/PageList.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/QuestionnaireResults.py` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/QuestionnaireResults.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/export_helpers.py` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/export_helpers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/export.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/export.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/login_admin.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/login_admin.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/preview_questionnaire.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/preview_questionnaire.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/progress.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/progress.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/progress_ajax.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/progress_ajax.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/progress_summary_ajax.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/progress_summary_ajax.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/questionnaire_results.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/questionnaire_results.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/results.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/results.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/table_ajax.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/table_ajax.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/table_view.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/table_view.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/templates/template_admin.html` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/templates/template_admin.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/util.py` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/admin/views.py` & `bride-of-frankensystem-1.9.3.1/BOFS/admin/views.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/cli.py` & `bride-of-frankensystem-1.9.3.1/BOFS/cli.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/create_app.py` & `bride-of-frankensystem-1.9.3.1/BOFS/create_app.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,20 +69,26 @@
     for current_path in os.listdir(path):
         if current_path in ["static", "templates"]:  # We're inside a blueprint. Unlikely that there is another one here...
             continue
 
         considered_path = os.path.join(path, current_path)
 
         if os.path.isdir(considered_path):  # We should try this path..
+            found_views = False
+
             for subpath in os.listdir(considered_path):
                 if subpath == "views.py":
                     app.load_blueprint(current_path, current_path, False)
+                    found_views = True
                 if subpath == "models.py":
                     app.load_models(current_path)
 
+            if not found_views:  # If no views, then create a blank blueprint so we can still search the templates folder, etc.
+                app.load_empty_blueprint(current_path)
+
     app.load_blueprint('BOFS.default', 'default')
 
     with app.app_context():
         if not app.questionnaire_list_is_safe():
             print("Error! The same questionnaire was specified twice. Please add a tag to your questionnaire if this "
                   "was intentional.")
             return
```

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/default/models.py` & `bride-of-frankensystem-1.9.3.1/BOFS/default/models.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/default/views.py` & `bride-of-frankensystem-1.9.3.1/BOFS/default/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,16 +394,16 @@
 @default.route("/instructions/<pageName>", methods=['POST', 'GET'])
 @verify_correct_page
 @verify_session_valid
 def route_instructions(pageName):
     """
     ``/instructions/<pageName>``
 
-    Generic page to render instructions. The instructions are defined in HTML within a file and rendered in BOF using
-    the template. A button to redirect to the next page in the study is shown after the instructions.
+    Generic route to render instructions. The instructions are defined in HTML within a file and rendered in BOFS using
+    the the templating system. A button to redirect to the next page in the study is shown after the instructions.
 
     Instruction HTML files can be placed in the project root directory's templates folder in
     ``/templates/instructions/...`` or in one of your blueprint's templates folder in
     ``/<my_blueprint>/templates/instructions/...``.
 
     The files must be in HTML format and use the ``.html`` extension. The ``pageName`` specified is the filename for the
     instructions, without the file extension.
@@ -415,7 +415,37 @@
 
     jinja = current_app.jinja_env
     instructionsTemplate = jinja.get_or_select_template("instructions/%s.html" % pageName)
     instructionsHtml = instructionsTemplate.render()
 
     return render_template("instructions.html", instructions=instructionsHtml)
 
+
+@default.route("/simple/<pageName>", methods=['POST', 'GET'])
+@verify_correct_page
+@verify_session_valid
+def route_simple_html(pageName):
+    """
+    ``/simple/<pageName>``
+
+    Generic route to render simple Jinja 2 templates (or simple HTML pages) that do not need any additional Python code.
+    The pages are defined in HTML/Jinja 2 within a file and rendered in BOFS using the templating system. Unlike the
+    instruction pages, you are responsible for redirecting participants yourself (e.g., via a JavaScript redirect to
+    ``/redirect_next_page``. A generic POST request to this route (such as from a form submission) will also trigger a
+    redirection to the next page.
+
+    Simple HTML files can be placed in the project root directory's templates folder in
+    ``/templates/simple/...`` or in one of your blueprint's templates folder in
+    ``/<my_blueprint>/templates/simple/...``.
+
+    The files must be in HTML format and use the ``.html`` extension. The ``pageName`` specified is the filename for the
+    html file, without the file extension.
+
+    :param pageName: the name of the file to use to render the simple page (without the .html extension)
+    """
+    if request.method == "POST":
+        return redirect(join_urls('/redirect_from_page', request.path))
+
+    jinja = current_app.jinja_env
+    simple_html = jinja.get_or_select_template("simple/%s.html" % pageName).render()
+
+    return render_template("simple.html", simple_contents=simple_html)
```

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/globals.py` & `bride-of-frankensystem-1.9.3.1/BOFS/globals.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/static/img/check.png` & `bride-of-frankensystem-1.9.3.1/BOFS/static/img/check.png`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/static/img/spinner32.gif` & `bride-of-frankensystem-1.9.3.1/BOFS/static/img/spinner32.gif`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/static/js/bootstrap.min.js` & `bride-of-frankensystem-1.9.3.1/BOFS/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/static/js/jquery-3.4.1.min.js` & `bride-of-frankensystem-1.9.3.1/BOFS/static/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/static/js/plotly-latest.min.js` & `bride-of-frankensystem-1.9.3.1/BOFS/static/js/plotly-latest.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/static/js/popper.min.js` & `bride-of-frankensystem-1.9.3.1/BOFS/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/static/loading.gif` & `bride-of-frankensystem-1.9.3.1/BOFS/static/loading.gif`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/static/style.css` & `bride-of-frankensystem-1.9.3.1/BOFS/static/style.css`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/templates/consent.html` & `bride-of-frankensystem-1.9.3.1/BOFS/templates/consent.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/templates/end.html` & `bride-of-frankensystem-1.9.3.1/BOFS/templates/end.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/templates/external_id.html` & `bride-of-frankensystem-1.9.3.1/BOFS/templates/external_id.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/templates/questionnaire_macro.html` & `bride-of-frankensystem-1.9.3.1/BOFS/templates/questionnaire_macro.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/templates/template.html` & `bride-of-frankensystem-1.9.3.1/BOFS/templates/template.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/templates/unity_webgl.html` & `bride-of-frankensystem-1.9.3.1/BOFS/templates/unity_webgl.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/templates/unity_webgl_fullscreen.html` & `bride-of-frankensystem-1.9.3.1/BOFS/templates/unity_webgl_fullscreen.html`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/BOFS/util.py` & `bride-of-frankensystem-1.9.3.1/BOFS/util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/LICENSE` & `bride-of-frankensystem-1.9.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/PKG-INFO` & `bride-of-frankensystem-1.9.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bride-of-frankensystem
-Version: 1.9.3.0
+Version: 1.9.3.1
 Summary: A framework that allows for the development of custom online experiments and surveys.
 Author-email: Colby Johanson <colby.johanson@usask.ca>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bride-of-frankensystem-1.9.3.0/README.md` & `bride-of-frankensystem-1.9.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/bride_of_frankensystem.egg-info/PKG-INFO` & `bride-of-frankensystem-1.9.3.1/bride_of_frankensystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bride-of-frankensystem
-Version: 1.9.3.0
+Version: 1.9.3.1
 Summary: A framework that allows for the development of custom online experiments and surveys.
 Author-email: Colby Johanson <colby.johanson@usask.ca>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `bride-of-frankensystem-1.9.3.0/bride_of_frankensystem.egg-info/SOURCES.txt` & `bride-of-frankensystem-1.9.3.1/bride_of_frankensystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/docs/conf.py` & `bride-of-frankensystem-1.9.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/pyproject.toml` & `bride-of-frankensystem-1.9.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bride-of-frankensystem"
-version = "1.9.3.0"
+version = "1.9.3.1"
 description = "A framework that allows for the development of custom online experiments and surveys."
 readme = "README.md"
 authors = [{ name = "Colby Johanson", email = "colby.johanson@usask.ca" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Programming Language :: Python",
```

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/_distutils_hack/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/_virtualenv.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/__main__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/build_env.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cache.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/main.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/parser.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/cache.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/check.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/completion.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/debug.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/download.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/hash.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/help.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/index.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/install.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/list.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/search.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/show.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/configuration.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/base.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/exceptions.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/index/collector.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/index/sources.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/locations/base.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/metadata/base.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/candidate.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/format_control.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/index.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/link.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/scheme.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/target_python.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/models/wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/auth.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/cache.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/download.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/session.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/utils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/check.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/pyproject.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/constructors.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_file.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_install.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_set.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_tracker.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_tracker.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/base.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/_log.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/compat.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/logging.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/misc.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/models.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/parallel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/pkg_resources.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/urls.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/git.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/compat.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/misc.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/shutil.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/sysconfig.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/_backport/tarfile.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/distro.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/distro.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/constants.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/core.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/build.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/check.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/compat.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/compat.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/meta.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/bar.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/bar.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/colors.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/colors.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/counter.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/counter.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/progress/spinner.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/pyparsing.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/api.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/help.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/models.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/six.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_msi.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/bdist_wininst.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/config.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/core.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/dist.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/errors.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/extension.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/log.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/util.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/version.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_imp.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/archive_util.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/build_meta.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/alias.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/build_clib.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/build_ext.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/build_py.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/develop.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/dist_info.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/easy_install.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/egg_info.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/install.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/install_lib.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/install_scripts.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/py36compat.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/rotate.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/saveopts.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/sdist.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/setopt.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/test.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/command/upload_docs.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/config.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/config.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/dep_util.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/depends.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/dist.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/errors.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/extension.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/extern/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/glob.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/installer.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/launch.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/logging.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/monkey.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/msvc.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/namespaces.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/package_index.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/sandbox.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/unicode_utils.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/setuptools/windows_support.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/bdist_wheel.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/cli/__init__.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/cli/convert.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/cli/pack.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/cli/unpack.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/macosx_libfile.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/metadata.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/pkginfo.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/util.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/vendored/packaging/_typing.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/vendored/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Lib/site-packages/wheel/wheelfile.py` & `bride-of-frankensystem-1.9.3.1/venv/Lib/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `bride-of-frankensystem-1.9.3.0/venv/Scripts/activate_this.py` & `bride-of-frankensystem-1.9.3.1/venv/Scripts/activate_this.py`

 * *Files identical despite different names*

