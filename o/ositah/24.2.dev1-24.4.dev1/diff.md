# Comparing `tmp/ositah-24.2.dev1.tar.gz` & `tmp/ositah-24.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ositah-24.2.dev1.tar", last modified: Mon Feb  5 19:34:21 2024, max compression
+gzip compressed data, was "ositah-24.4.dev1.tar", last modified: Tue Apr  2 15:12:47 2024, max compression
```

## Comparing `ositah-24.2.dev1.tar` & `ositah-24.4.dev1.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:21.071001 ositah-24.2.dev1/
--rw-rw-rw-   0        0        0       84 2022-11-13 21:10:36.000000 ositah-24.2.dev1/.gitignore
--rw-rw-rw-   0        0        0      371 2024-02-05 15:48:47.000000 ositah-24.2.dev1/.gitlab-ci.yml
--rw-rw-rw-   0        0        0     1550 2022-10-27 13:39:35.000000 ositah-24.2.dev1/LICENSE
--rw-rw-rw-   0        0        0     8098 2024-02-05 19:34:21.068997 ositah-24.2.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     7119 2022-11-13 21:13:24.000000 ositah-24.2.dev1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:20.800294 ositah-24.2.dev1/gunicorn.config/
--rw-rw-rw-   0        0        0      643 2022-11-13 21:10:36.000000 ositah-24.2.dev1/gunicorn.config/README.md
--rw-rw-rw-   0        0        0      141 2022-11-13 21:10:36.000000 ositah-24.2.dev1/gunicorn.config/gunicorn.ositah
--rw-rw-rw-   0        0        0      379 2022-11-13 21:10:36.000000 ositah-24.2.dev1/gunicorn.config/gunicorn@.service
--rw-rw-rw-   0        0        0      369 2022-11-13 21:10:36.000000 ositah-24.2.dev1/gunicorn.config/ositah.conf.py
--rw-rw-rw-   0        0        0     1337 2023-08-23 08:36:17.000000 ositah-24.2.dev1/noxfile.py
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:20.804001 ositah-24.2.dev1/ositah/
--rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-24.2.dev1/ositah/__init__.py
--rw-rw-rw-   0        0        0      428 2023-03-02 17:58:31.000000 ositah-24.2.dev1/ositah/app.py
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:20.843071 ositah-24.2.dev1/ositah/apps/
--rw-rw-rw-   0        0        0        0 2023-08-23 08:36:17.000000 ositah-24.2.dev1/ositah/apps/__init__.py
--rw-rw-rw-   0        0        0    28259 2023-02-26 18:01:44.000000 ositah-24.2.dev1/ositah/apps/analysis.py
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:20.852074 ositah-24.2.dev1/ositah/apps/configuration/
--rw-rw-rw-   0        0        0        0 2023-08-23 08:36:17.000000 ositah-24.2.dev1/ositah/apps/configuration/__init__.py
--rw-rw-rw-   0        0        0    33477 2023-08-23 08:36:17.000000 ositah-24.2.dev1/ositah/apps/configuration/callbacks.py
--rw-rw-rw-   0        0        0    20299 2024-02-05 19:27:14.000000 ositah-24.2.dev1/ositah/apps/configuration/main.py
--rw-rw-rw-   0        0        0     3862 2023-08-23 08:36:17.000000 ositah-24.2.dev1/ositah/apps/configuration/parameters.py
--rw-rw-rw-   0        0        0     3982 2023-08-23 08:36:17.000000 ositah-24.2.dev1/ositah/apps/configuration/tools.py
--rw-rw-rw-   0        0        0    47532 2024-02-05 19:27:14.000000 ositah-24.2.dev1/ositah/apps/export.py
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:20.861161 ositah-24.2.dev1/ositah/apps/validation/
--rw-rw-rw-   0        0        0        0 2023-08-23 08:36:17.000000 ositah-24.2.dev1/ositah/apps/validation/__init__.py
--rw-rw-rw-   0        0        0     9557 2023-08-23 14:34:42.000000 ositah-24.2.dev1/ositah/apps/validation/callbacks.py
--rw-rw-rw-   0        0        0     2896 2023-08-23 08:36:17.000000 ositah-24.2.dev1/ositah/apps/validation/main.py
--rw-rw-rw-   0        0        0     1003 2023-08-23 08:36:17.000000 ositah-24.2.dev1/ositah/apps/validation/parameters.py
--rw-rw-rw-   0        0        0    24770 2024-02-05 19:27:14.000000 ositah-24.2.dev1/ositah/apps/validation/tables.py
--rw-rw-rw-   0        0        0    18046 2024-02-05 19:19:00.000000 ositah-24.2.dev1/ositah/apps/validation/tools.py
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:20.869635 ositah-24.2.dev1/ositah/assets/
--rw-rw-rw-   0        0        0      503 2022-11-13 21:10:36.000000 ositah-24.2.dev1/ositah/assets/arrow_down_up.svg
--rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-24.2.dev1/ositah/assets/ositah.css
--rw-rw-rw-   0        0        0      593 2022-11-13 21:10:36.000000 ositah-24.2.dev1/ositah/assets/sort_ascending.svg
--rw-rw-rw-   0        0        0      618 2022-11-13 21:10:36.000000 ositah-24.2.dev1/ositah/assets/sort_descending.svg
--rw-rw-rw-   0        0        0    17478 2022-11-13 21:10:36.000000 ositah-24.2.dev1/ositah/assets/sorttable.js
--rw-rw-rw-   0        0        0    15725 2024-02-05 16:56:56.000000 ositah-24.2.dev1/ositah/main.py
--rw-rw-rw-   0        0        0     7471 2023-02-24 17:01:35.000000 ositah-24.2.dev1/ositah/ositah.example.cfg
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:20.870674 ositah-24.2.dev1/ositah/static/
--rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-24.2.dev1/ositah/static/style.css
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:20.875650 ositah-24.2.dev1/ositah/templates/
--rw-rw-rw-   0        0        0      714 2022-11-13 21:10:36.000000 ositah-24.2.dev1/ositah/templates/base.html
--rw-rw-rw-   0        0        0     1608 2022-11-13 21:10:36.000000 ositah-24.2.dev1/ositah/templates/bootstrap_login.html
--rw-rw-rw-   0        0        0     1033 2022-11-13 21:10:36.000000 ositah-24.2.dev1/ositah/templates/login_form.html
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:20.894649 ositah-24.2.dev1/ositah/utils/
--rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-24.2.dev1/ositah/utils/__init__.py
--rw-rw-rw-   0        0        0     4453 2023-03-11 12:02:31.000000 ositah-24.2.dev1/ositah/utils/agents.py
--rw-rw-rw-   0        0        0     9149 2023-03-11 12:02:31.000000 ositah-24.2.dev1/ositah/utils/authentication.py
--rw-rw-rw-   0        0        0      504 2023-03-11 12:02:31.000000 ositah-24.2.dev1/ositah/utils/cache.py
--rw-rw-rw-   0        0        0      295 2023-02-26 18:01:44.000000 ositah-24.2.dev1/ositah/utils/core.py
--rw-rw-rw-   0        0        0     1911 2024-02-05 19:29:26.000000 ositah-24.2.dev1/ositah/utils/exceptions.py
--rw-rw-rw-   0        0        0     1510 2023-03-11 12:02:31.000000 ositah-24.2.dev1/ositah/utils/hito_db.py
--rw-rw-rw-   0        0        0     8988 2024-02-05 19:19:00.000000 ositah-24.2.dev1/ositah/utils/hito_db_model.py
--rw-rw-rw-   0        0        0    12007 2024-02-05 19:27:14.000000 ositah-24.2.dev1/ositah/utils/menus.py
--rw-rw-rw-   0        0        0     4058 2023-03-15 09:13:49.000000 ositah-24.2.dev1/ositah/utils/period.py
--rw-rw-rw-   0        0        0    43479 2024-02-05 19:27:14.000000 ositah-24.2.dev1/ositah/utils/projects.py
--rw-rw-rw-   0        0        0     1186 2023-02-24 18:11:54.000000 ositah-24.2.dev1/ositah/utils/teams.py
--rw-rw-rw-   0        0        0    16372 2024-02-05 19:27:14.000000 ositah-24.2.dev1/ositah/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:21.068000 ositah-24.2.dev1/ositah.egg-info/
--rw-rw-rw-   0        0        0     8098 2024-02-05 19:34:20.000000 ositah-24.2.dev1/ositah.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1996 2024-02-05 19:34:20.000000 ositah-24.2.dev1/ositah.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-05 19:34:20.000000 ositah-24.2.dev1/ositah.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-02-05 19:34:20.000000 ositah-24.2.dev1/ositah.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      181 2024-02-05 19:34:20.000000 ositah-24.2.dev1/ositah.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-05 19:34:20.000000 ositah-24.2.dev1/ositah.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2024-02-05 19:31:09.000000 ositah-24.2.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-05 19:34:21.071001 ositah-24.2.dev1/setup.cfg
--rw-rw-rw-   0        0        0       41 2022-11-13 21:10:36.000000 ositah-24.2.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:21.048735 ositah-24.2.dev1/test-dash/
--rw-rw-rw-   0        0        0       87 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/README.md
--rw-rw-rw-   0        0        0     2965 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/accordion.py
--rw-rw-rw-   0        0        0     4387 2023-02-24 17:01:35.000000 ositah-24.2.dev1/test-dash/authentication.py
--rw-rw-rw-   0        0        0     2092 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/checkbox.py
--rw-rw-rw-   0        0        0     3581 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/checklist.py
--rw-rw-rw-   0        0        0      602 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/file-selector.py
--rw-rw-rw-   0        0        0     3068 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/file-upload.py
--rw-rw-rw-   0        0        0     2734 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/long_running_callback.py
--rw-rw-rw-   0        0        0     2394 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/pandas_split.py
--rw-rw-rw-   0        0        0     1888 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/pandas_split_bug_report.py
--rw-rw-rw-   0        0        0     1413 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/pattern-matching-callback.py
--rw-rw-rw-   0        0        0     4189 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/progess_bar.py
--rw-rw-rw-   0        0        0     2679 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/reset_table_checkboxes.py
--rw-rw-rw-   0        0        0     4377 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/sortable_table.py
--rw-rw-rw-   0        0        0     1159 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/sqlalchemy_test.py
-drwxrwxrwx   0        0        0        0 2024-02-05 19:34:21.065998 ositah-24.2.dev1/test-dash/templates/
--rw-rw-rw-   0        0        0      500 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/templates/base.html
--rw-rw-rw-   0        0        0      680 2022-11-13 21:10:36.000000 ositah-24.2.dev1/test-dash/templates/login_form.html
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.233688 ositah-24.4.dev1/
+-rw-rw-rw-   0        0        0       84 2022-11-13 21:10:36.000000 ositah-24.4.dev1/.gitignore
+-rw-rw-rw-   0        0        0      371 2024-02-05 15:48:47.000000 ositah-24.4.dev1/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0     1550 2022-10-27 13:39:35.000000 ositah-24.4.dev1/LICENSE
+-rw-rw-rw-   0        0        0     8098 2024-04-02 15:12:47.232686 ositah-24.4.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     7119 2022-11-13 21:13:24.000000 ositah-24.4.dev1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.129288 ositah-24.4.dev1/gunicorn.config/
+-rw-rw-rw-   0        0        0      643 2022-11-13 21:10:36.000000 ositah-24.4.dev1/gunicorn.config/README.md
+-rw-rw-rw-   0        0        0      141 2022-11-13 21:10:36.000000 ositah-24.4.dev1/gunicorn.config/gunicorn.ositah
+-rw-rw-rw-   0        0        0      379 2022-11-13 21:10:36.000000 ositah-24.4.dev1/gunicorn.config/gunicorn@.service
+-rw-rw-rw-   0        0        0      369 2022-11-13 21:10:36.000000 ositah-24.4.dev1/gunicorn.config/ositah.conf.py
+-rw-rw-rw-   0        0        0     1337 2023-08-23 08:36:17.000000 ositah-24.4.dev1/noxfile.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.134295 ositah-24.4.dev1/ositah/
+-rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-24.4.dev1/ositah/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-03-02 17:58:31.000000 ositah-24.4.dev1/ositah/app.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.148417 ositah-24.4.dev1/ositah/apps/
+-rw-rw-rw-   0        0        0        0 2023-08-23 08:36:17.000000 ositah-24.4.dev1/ositah/apps/__init__.py
+-rw-rw-rw-   0        0        0    28259 2023-02-26 18:01:44.000000 ositah-24.4.dev1/ositah/apps/analysis.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.156391 ositah-24.4.dev1/ositah/apps/configuration/
+-rw-rw-rw-   0        0        0        0 2023-08-23 08:36:17.000000 ositah-24.4.dev1/ositah/apps/configuration/__init__.py
+-rw-rw-rw-   0        0        0    33477 2023-08-23 08:36:17.000000 ositah-24.4.dev1/ositah/apps/configuration/callbacks.py
+-rw-rw-rw-   0        0        0    20299 2024-02-05 19:27:14.000000 ositah-24.4.dev1/ositah/apps/configuration/main.py
+-rw-rw-rw-   0        0        0     3862 2023-08-23 08:36:17.000000 ositah-24.4.dev1/ositah/apps/configuration/parameters.py
+-rw-rw-rw-   0        0        0     3982 2023-08-23 08:36:17.000000 ositah-24.4.dev1/ositah/apps/configuration/tools.py
+-rw-rw-rw-   0        0        0    47532 2024-02-05 19:27:14.000000 ositah-24.4.dev1/ositah/apps/export.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.162393 ositah-24.4.dev1/ositah/apps/validation/
+-rw-rw-rw-   0        0        0        0 2023-08-23 08:36:17.000000 ositah-24.4.dev1/ositah/apps/validation/__init__.py
+-rw-rw-rw-   0        0        0     9557 2023-08-23 14:34:42.000000 ositah-24.4.dev1/ositah/apps/validation/callbacks.py
+-rw-rw-rw-   0        0        0     2896 2023-08-23 08:36:17.000000 ositah-24.4.dev1/ositah/apps/validation/main.py
+-rw-rw-rw-   0        0        0     1003 2023-08-23 08:36:17.000000 ositah-24.4.dev1/ositah/apps/validation/parameters.py
+-rw-rw-rw-   0        0        0    24770 2024-02-05 19:27:14.000000 ositah-24.4.dev1/ositah/apps/validation/tables.py
+-rw-rw-rw-   0        0        0    18046 2024-02-05 19:19:00.000000 ositah-24.4.dev1/ositah/apps/validation/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.169392 ositah-24.4.dev1/ositah/assets/
+-rw-rw-rw-   0        0        0      503 2022-11-13 21:10:36.000000 ositah-24.4.dev1/ositah/assets/arrow_down_up.svg
+-rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-24.4.dev1/ositah/assets/ositah.css
+-rw-rw-rw-   0        0        0      593 2022-11-13 21:10:36.000000 ositah-24.4.dev1/ositah/assets/sort_ascending.svg
+-rw-rw-rw-   0        0        0      618 2022-11-13 21:10:36.000000 ositah-24.4.dev1/ositah/assets/sort_descending.svg
+-rw-rw-rw-   0        0        0    17478 2022-11-13 21:10:36.000000 ositah-24.4.dev1/ositah/assets/sorttable.js
+-rw-rw-rw-   0        0        0    15673 2024-04-02 15:10:54.000000 ositah-24.4.dev1/ositah/main.py
+-rw-rw-rw-   0        0        0     7472 2024-04-02 15:12:29.000000 ositah-24.4.dev1/ositah/ositah.example.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.171427 ositah-24.4.dev1/ositah/static/
+-rw-rw-rw-   0        0        0     1094 2022-11-13 21:10:36.000000 ositah-24.4.dev1/ositah/static/style.css
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.176391 ositah-24.4.dev1/ositah/templates/
+-rw-rw-rw-   0        0        0      714 2022-11-13 21:10:36.000000 ositah-24.4.dev1/ositah/templates/base.html
+-rw-rw-rw-   0        0        0     1608 2022-11-13 21:10:36.000000 ositah-24.4.dev1/ositah/templates/bootstrap_login.html
+-rw-rw-rw-   0        0        0     1033 2022-11-13 21:10:36.000000 ositah-24.4.dev1/ositah/templates/login_form.html
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.194160 ositah-24.4.dev1/ositah/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-24 18:11:54.000000 ositah-24.4.dev1/ositah/utils/__init__.py
+-rw-rw-rw-   0        0        0     4453 2023-03-11 12:02:31.000000 ositah-24.4.dev1/ositah/utils/agents.py
+-rw-rw-rw-   0        0        0     9149 2024-04-02 14:54:54.000000 ositah-24.4.dev1/ositah/utils/authentication.py
+-rw-rw-rw-   0        0        0      504 2023-03-11 12:02:31.000000 ositah-24.4.dev1/ositah/utils/cache.py
+-rw-rw-rw-   0        0        0      295 2023-02-26 18:01:44.000000 ositah-24.4.dev1/ositah/utils/core.py
+-rw-rw-rw-   0        0        0     1911 2024-02-05 19:29:26.000000 ositah-24.4.dev1/ositah/utils/exceptions.py
+-rw-rw-rw-   0        0        0     1510 2023-03-11 12:02:31.000000 ositah-24.4.dev1/ositah/utils/hito_db.py
+-rw-rw-rw-   0        0        0     8988 2024-02-05 19:19:00.000000 ositah-24.4.dev1/ositah/utils/hito_db_model.py
+-rw-rw-rw-   0        0        0    12007 2024-02-05 19:27:14.000000 ositah-24.4.dev1/ositah/utils/menus.py
+-rw-rw-rw-   0        0        0     4058 2023-03-15 09:13:49.000000 ositah-24.4.dev1/ositah/utils/period.py
+-rw-rw-rw-   0        0        0    43479 2024-02-05 19:27:14.000000 ositah-24.4.dev1/ositah/utils/projects.py
+-rw-rw-rw-   0        0        0     1186 2023-02-24 18:11:54.000000 ositah-24.4.dev1/ositah/utils/teams.py
+-rw-rw-rw-   0        0        0    16449 2024-04-02 15:12:29.000000 ositah-24.4.dev1/ositah/utils/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.230686 ositah-24.4.dev1/ositah.egg-info/
+-rw-rw-rw-   0        0        0     8098 2024-04-02 15:12:46.000000 ositah-24.4.dev1/ositah.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1996 2024-04-02 15:12:47.000000 ositah-24.4.dev1/ositah.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 15:12:46.000000 ositah-24.4.dev1/ositah.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-02 15:12:46.000000 ositah-24.4.dev1/ositah.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      181 2024-04-02 15:12:46.000000 ositah-24.4.dev1/ositah.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 15:12:46.000000 ositah-24.4.dev1/ositah.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:54.000000 ositah-24.4.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 15:12:47.233688 ositah-24.4.dev1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2022-11-13 21:10:36.000000 ositah-24.4.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.215176 ositah-24.4.dev1/test-dash/
+-rw-rw-rw-   0        0        0       87 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/README.md
+-rw-rw-rw-   0        0        0     2965 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/accordion.py
+-rw-rw-rw-   0        0        0     4387 2023-02-24 17:01:35.000000 ositah-24.4.dev1/test-dash/authentication.py
+-rw-rw-rw-   0        0        0     2092 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/checkbox.py
+-rw-rw-rw-   0        0        0     3581 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/checklist.py
+-rw-rw-rw-   0        0        0      602 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/file-selector.py
+-rw-rw-rw-   0        0        0     3068 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/file-upload.py
+-rw-rw-rw-   0        0        0     2734 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/long_running_callback.py
+-rw-rw-rw-   0        0        0     2394 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/pandas_split.py
+-rw-rw-rw-   0        0        0     1888 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/pandas_split_bug_report.py
+-rw-rw-rw-   0        0        0     1413 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/pattern-matching-callback.py
+-rw-rw-rw-   0        0        0     4189 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/progess_bar.py
+-rw-rw-rw-   0        0        0     2679 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/reset_table_checkboxes.py
+-rw-rw-rw-   0        0        0     4377 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/sortable_table.py
+-rw-rw-rw-   0        0        0     1159 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/sqlalchemy_test.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:12:47.229679 ositah-24.4.dev1/test-dash/templates/
+-rw-rw-rw-   0        0        0      500 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/templates/base.html
+-rw-rw-rw-   0        0        0      680 2022-11-13 21:10:36.000000 ositah-24.4.dev1/test-dash/templates/login_form.html
```

### Comparing `ositah-24.2.dev1/LICENSE` & `ositah-24.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/PKG-INFO` & `ositah-24.4.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ositah
-Version: 24.2.dev1
+Version: 24.4.dev1
 Summary: Outils de Suivi d'Activités basé sur Hito
 Author-email: Michel Jouvin <michel.jouvin@ijclab.in2p3.fr>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://gitlab.in2p3.fr/hito/ositah
 Project-URL: Bug Tracker, https://gitlab.in2p3.fr/hito/ositah/-/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ositah-24.2.dev1/README.md` & `ositah-24.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/gunicorn.config/README.md` & `ositah-24.4.dev1/gunicorn.config/README.md`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/noxfile.py` & `ositah-24.4.dev1/noxfile.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/analysis.py` & `ositah-24.4.dev1/ositah/apps/analysis.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/configuration/callbacks.py` & `ositah-24.4.dev1/ositah/apps/configuration/callbacks.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/configuration/main.py` & `ositah-24.4.dev1/ositah/apps/configuration/main.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/configuration/parameters.py` & `ositah-24.4.dev1/ositah/apps/configuration/parameters.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/configuration/tools.py` & `ositah-24.4.dev1/ositah/apps/configuration/tools.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/export.py` & `ositah-24.4.dev1/ositah/apps/export.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/validation/callbacks.py` & `ositah-24.4.dev1/ositah/apps/validation/callbacks.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/validation/main.py` & `ositah-24.4.dev1/ositah/apps/validation/main.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/validation/parameters.py` & `ositah-24.4.dev1/ositah/apps/validation/parameters.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/validation/tables.py` & `ositah-24.4.dev1/ositah/apps/validation/tables.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/apps/validation/tools.py` & `ositah-24.4.dev1/ositah/apps/validation/tools.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/assets/ositah.css` & `ositah-24.4.dev1/ositah/assets/ositah.css`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/assets/sort_ascending.svg` & `ositah-24.4.dev1/ositah/assets/sort_ascending.svg`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/assets/sort_descending.svg` & `ositah-24.4.dev1/ositah/assets/sort_descending.svg`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/assets/sorttable.js` & `ositah-24.4.dev1/ositah/assets/sorttable.js`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/main.py` & `ositah-24.4.dev1/ositah/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         title_class="text-danger",
     )
 
 
 # valid role missing jumbotron
 def valid_role_missing(msg):
     return ositah_jumbotron(
-        "You don't havea valid Hito role to OSITAH",
+        "You don't have a valid Hito role to OSITAH",
         msg,
         title_class="text-warning",
     )
 
 
 @app.callback(
     [
@@ -200,17 +200,15 @@
                 role_ok = True
                 user_session_data.role = role
                 break
         if role_ok:
             if not user_session_data.agent_teams:
                 if role == HITO_ROLE_TEAM_MGR:
                     # For a team manager, show only the teams he/she is a manager
-                    teams = Team.query.filter(
-                        Team.managers.any(email_auth=session["user_email"])
-                    ).all()
+                    teams = Team.query.filter(Team.managers.any(email=session["user_email"])).all()
                     if len(teams) == 0:
                         # A user with role ROLE_RESP but is not the manager of any team is degraded
                         # to ROLE_AGENT
                         role_ok = False
                         role_not_ok_msg = (
                             f"{user.prenom} {user.nom} n'est" " responsable d'aucune équipe"
                         )
```

### Comparing `ositah-24.2.dev1/ositah/ositah.example.cfg` & `ositah-24.4.dev1/ositah/ositah.example.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
       bind_dn: 'CN=Non-Interactive Queries,OU=SI,OU=Services techniques,OU=Laboratoire,DC=lal,DC=in2p3,DC=fr'
       password: 'ldap_bind_password'
     provider_name: "MyLab account"
 
 # Options related to declarations
 declaration:
   # Default date must be a date included into the selected validation period. It is a default, if no other explicitly select
-  default_date: 2021-07-01
+  #default_date: 2021-07-01
   # max_hours specifies the upper valid value for activities declared in hours
   max_hours: 400
   # Agent statut whose declaration is not mandatory
   optional_statutes:
     - benevole
     - emerite
     - stagiaire
```

### Comparing `ositah-24.2.dev1/ositah/static/style.css` & `ositah-24.4.dev1/ositah/static/style.css`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/templates/base.html` & `ositah-24.4.dev1/ositah/templates/base.html`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/templates/bootstrap_login.html` & `ositah-24.4.dev1/ositah/templates/bootstrap_login.html`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/templates/login_form.html` & `ositah-24.4.dev1/ositah/templates/login_form.html`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/agents.py` & `ositah-24.4.dev1/ositah/utils/agents.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/authentication.py` & `ositah-24.4.dev1/ositah/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/exceptions.py` & `ositah-24.4.dev1/ositah/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/hito_db.py` & `ositah-24.4.dev1/ositah/utils/hito_db.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/hito_db_model.py` & `ositah-24.4.dev1/ositah/utils/hito_db_model.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/menus.py` & `ositah-24.4.dev1/ositah/utils/menus.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/period.py` & `ositah-24.4.dev1/ositah/utils/period.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/projects.py` & `ositah-24.4.dev1/ositah/utils/projects.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/teams.py` & `ositah-24.4.dev1/ositah/utils/teams.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/ositah/utils/utils.py` & `ositah-24.4.dev1/ositah/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Convenience objects for OSITAH application
 
 from datetime import datetime
 from typing import List
 
 import dash_bootstrap_components as dbc
 from dash import html
+from dateutil.relativedelta import relativedelta
 from flask import session
 from flask_sqlalchemy import SQLAlchemy
 from hito_tools.exceptions import ConfigFileEmpty, ConfigMissingParam
 from hito_tools.nsip import nsip_session_init
 from hito_tools.utils import load_config_file
 
 from ositah.app import app
@@ -384,15 +385,15 @@
         for k in ["low", "suspect", "good"]:
             if k not in config["declaration"]["thresholds"]:
                 raise ConfigMissingParam(f"declaration/thresholds/{k}", file)
     else:
         config["declaration"]["thresholds"] = {"low": 50, "suspect": 75, "good": 100}
     # Default declaration period date defaults to current day if not explicitly defined
     if "default_date" not in config["declaration"]:
-        config["declaration"]["default_date"] = datetime.now()
+        config["declaration"]["default_date"] = datetime.now() - relativedelta(months=10)
     global_params.declaration_options = config["declaration"]
 
     if "validation" not in config:
         config["validation"] = {}
     if "override_period" not in config["validation"]:
         config["validation"]["override_period"] = []
     global_params.validation_params = config["validation"]
```

### Comparing `ositah-24.2.dev1/ositah.egg-info/PKG-INFO` & `ositah-24.4.dev1/ositah.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ositah
-Version: 24.2.dev1
+Version: 24.4.dev1
 Summary: Outils de Suivi d'Activités basé sur Hito
 Author-email: Michel Jouvin <michel.jouvin@ijclab.in2p3.fr>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://gitlab.in2p3.fr/hito/ositah
 Project-URL: Bug Tracker, https://gitlab.in2p3.fr/hito/ositah/-/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ositah-24.2.dev1/ositah.egg-info/SOURCES.txt` & `ositah-24.4.dev1/ositah.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/pyproject.toml` & `ositah-24.4.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools", "setuptools-scm",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ositah"
-version = "24.2.dev1"
+version = "24.4.dev1"
 description = "Outils de Suivi d'Activités basé sur Hito"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
```

### Comparing `ositah-24.2.dev1/test-dash/accordion.py` & `ositah-24.4.dev1/test-dash/accordion.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/authentication.py` & `ositah-24.4.dev1/test-dash/authentication.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/checkbox.py` & `ositah-24.4.dev1/test-dash/checkbox.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/checklist.py` & `ositah-24.4.dev1/test-dash/checklist.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/file-selector.py` & `ositah-24.4.dev1/test-dash/file-selector.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/file-upload.py` & `ositah-24.4.dev1/test-dash/file-upload.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/long_running_callback.py` & `ositah-24.4.dev1/test-dash/long_running_callback.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/pandas_split.py` & `ositah-24.4.dev1/test-dash/pandas_split.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/pandas_split_bug_report.py` & `ositah-24.4.dev1/test-dash/pandas_split_bug_report.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/pattern-matching-callback.py` & `ositah-24.4.dev1/test-dash/pattern-matching-callback.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/progess_bar.py` & `ositah-24.4.dev1/test-dash/progess_bar.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/reset_table_checkboxes.py` & `ositah-24.4.dev1/test-dash/reset_table_checkboxes.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/sortable_table.py` & `ositah-24.4.dev1/test-dash/sortable_table.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/sqlalchemy_test.py` & `ositah-24.4.dev1/test-dash/sqlalchemy_test.py`

 * *Files identical despite different names*

### Comparing `ositah-24.2.dev1/test-dash/templates/login_form.html` & `ositah-24.4.dev1/test-dash/templates/login_form.html`

 * *Files identical despite different names*

