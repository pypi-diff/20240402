# Comparing `tmp/ckanext-ingest-1.3.0.tar.gz` & `tmp/ckanext-ingest-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-ingest-1.3.0.tar", last modified: Sat Mar 25 18:15:52 2023, max compression
+gzip compressed data, was "ckanext-ingest-1.4.0.tar", last modified: Mon Apr  1 23:52:43 2024, max compression
```

## Comparing `ckanext-ingest-1.3.0.tar` & `ckanext-ingest-1.4.0.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.552726 ckanext-ingest-1.3.0/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34499 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      129 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2715 2023-03-25 18:15:52.552726 ckanext-ingest-1.3.0/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2054 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/README.rst
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.542725 ckanext-ingest-1.3.0/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.542725 ckanext-ingest-1.3.0/ckanext/ingest/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1654 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/artifact.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2794 2023-03-25 17:09:22.000000 ckanext-ingest-1.3.0/ckanext/ingest/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      385 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.542725 ckanext-ingest-1.3.0/ckanext/ingest/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2155 2023-03-25 18:04:53.000000 ckanext-ingest-1.3.0/ckanext/ingest/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      509 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1962 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      620 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/logic/validators.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1954 2023-03-25 17:09:22.000000 ckanext-ingest-1.3.0/ckanext/ingest/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3442 2023-03-25 17:11:05.000000 ckanext-ingest-1.3.0/ckanext/ingest/record.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      388 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/registry.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.542725 ckanext-ingest-1.3.0/ckanext/ingest/strategy/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      682 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/strategy/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1409 2023-03-25 17:09:22.000000 ckanext-ingest-1.3.0/ckanext/ingest/strategy/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      784 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/strategy/csv.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3143 2023-03-25 17:09:22.000000 ckanext-ingest-1.3.0/ckanext/ingest/strategy/xlsx.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1441 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/strategy/zip.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.542725 ckanext-ingest-1.3.0/ckanext/ingest/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.542725 ckanext-ingest-1.3.0/ckanext/ingest/templates/ingest/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      713 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/templates/ingest/index.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.542725 ckanext-ingest-1.3.0/ckanext/ingest/templates/ingest/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      636 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/templates/ingest/snippets/ingest_form.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.552726 ckanext-ingest-1.3.0/ckanext/ingest/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.552726 ckanext-ingest-1.3.0/ckanext/ingest/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1987 2023-03-25 17:09:22.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/logic/test_auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/logic/test_schema.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.552726 ckanext-ingest-1.3.0/ckanext/ingest/tests/strategy/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/strategy/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/strategy/test_base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/strategy/test_csv.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/strategy/test_xlsx.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/strategy/test_zip.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/test_artifact.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)       96 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/test_record.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/test_registry.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/ckanext/ingest/tests/test_transform.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2944 2023-03-25 17:09:22.000000 ckanext-ingest-1.3.0/ckanext/ingest/transform.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      308 2023-03-25 17:09:20.000000 ckanext-ingest-1.3.0/ckanext/ingest/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1705 2023-03-25 17:09:22.000000 ckanext-ingest-1.3.0/ckanext/ingest/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-25 18:15:52.552726 ckanext-ingest-1.3.0/ckanext_ingest.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2715 2023-03-25 18:15:52.000000 ckanext-ingest-1.3.0/ckanext_ingest.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1653 2023-03-25 18:15:52.000000 ckanext-ingest-1.3.0/ckanext_ingest.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-03-25 18:15:52.000000 ckanext-ingest-1.3.0/ckanext_ingest.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      116 2023-03-25 18:15:52.000000 ckanext-ingest-1.3.0/ckanext_ingest.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-03-25 18:15:52.000000 ckanext-ingest-1.3.0/ckanext_ingest.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       52 2023-03-25 18:15:52.000000 ckanext-ingest-1.3.0/ckanext_ingest.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-03-25 18:15:52.000000 ckanext-ingest-1.3.0/ckanext_ingest.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2820 2023-03-25 17:09:17.000000 ckanext-ingest-1.3.0/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1691 2023-03-25 18:15:52.552726 ckanext-ingest-1.3.0/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      236 2022-09-29 11:29:37.000000 ckanext-ingest-1.3.0/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34499 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      129 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21087 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    20348 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      202 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext/ingest/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1701 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/artifact.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      637 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      745 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      326 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext/ingest/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4666 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      675 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2438 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      539 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/logic/validators.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1712 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3125 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/record.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5187 2024-04-01 23:51:58.000000 ckanext-ingest-1.4.0/ckanext/ingest/shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext/ingest/strategy/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/strategy/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      998 2024-04-01 23:51:58.000000 ckanext-ingest-1.4.0/ckanext/ingest/strategy/csv.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2624 2024-04-01 23:51:58.000000 ckanext-ingest-1.4.0/ckanext/ingest/strategy/xlsx.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3529 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/strategy/zip.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.798652 ckanext-ingest-1.4.0/ckanext/ingest/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext/ingest/templates/ingest/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      713 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/templates/ingest/index.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext/ingest/templates/ingest/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      636 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/templates/ingest/snippets/ingest_form.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext/ingest/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext/ingest/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2005 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/logic/test_auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/logic/test_schema.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext/ingest/tests/strategy/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/strategy/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/strategy/test_base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/strategy/test_csv.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/strategy/test_xlsx.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/strategy/test_zip.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/test_artifact.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       57 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/test_record.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/test_registry.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/tests/test_transform.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4718 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/transform.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1779 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/ckanext/ingest/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/ckanext_ingest.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    21087 2024-04-01 23:52:43.000000 ckanext-ingest-1.4.0/ckanext_ingest.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1619 2024-04-01 23:52:43.000000 ckanext-ingest-1.4.0/ckanext_ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-01 23:52:43.000000 ckanext-ingest-1.4.0/ckanext_ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      116 2024-04-01 23:52:43.000000 ckanext-ingest-1.4.0/ckanext_ingest.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-01 23:52:43.000000 ckanext-ingest-1.4.0/ckanext_ingest.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2024-04-01 23:52:43.000000 ckanext-ingest-1.4.0/ckanext_ingest.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-01 23:52:43.000000 ckanext-ingest-1.4.0/ckanext_ingest.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4119 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1676 2024-04-01 23:52:43.801985 ckanext-ingest-1.4.0/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      237 2024-04-01 23:51:40.000000 ckanext-ingest-1.4.0/setup.py
```

### Comparing `ckanext-ingest-1.3.0/LICENSE` & `ckanext-ingest-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-ingest-1.3.0/ckanext/ingest/artifact.py` & `ckanext-ingest-1.4.0/ckanext/ingest/artifact.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,71 +7,71 @@
 
 
 def make_artifacts(report: str) -> Artifacts:
     return Type[report].value()
 
 
 class Artifacts:
-    def fail(self, data):
+    def fail(self, data: Any):
         pass
 
-    def success(self, data):
+    def success(self, data: Any):
         pass
 
-    def collect(self):
+    def collect(self) -> Any:
         pass
 
 
 class DetailedArtifacts(Artifacts):
     collection: list[dict[str, Any]]
 
     def __init__(self):
         self.collection = []
 
-    def fail(self, data):
+    def fail(self, data: Any):
         rec = {"success": False}
         rec.update(data)
         self.collection.append(rec)
 
-    def success(self, data):
+    def success(self, data: Any):
         rec = {"success": True}
         rec.update(data)
         self.collection.append(rec)
 
     def collect(self):
         return self.collection
 
 
 class TmpArtifacts(Artifacts):
     def __init__(self):
         self.output = tempfile.NamedTemporaryFile("w", delete=False)
 
-    def fail(self, data):
+    def fail(self, data: Any):
         rec = {"success": False}
         rec.update(data)
         self.output.write(json.dumps(rec) + "\n")
 
-    def success(self, data):
+    def success(self, data: Any):
         rec = {"success": True}
         rec.update(data)
         self.output.write(json.dumps(rec) + "\n")
 
     def collect(self):
         self.output.close()
         return {"report_path": self.output.name}
 
 
 class StatArtifacts(Artifacts):
     succeed: int = 0
     failed: int = 0
 
-    def fail(self, data):
+    def fail(self, data: Any):
         self.failed += 1
 
-    def success(self, data):
+    def success(self, data: Any):
         self.succeed += 1
 
     def collect(self):
         return {
             "fail": self.failed,
             "success": self.succeed,
         }
```

### Comparing `ckanext-ingest-1.3.0/ckanext/ingest/logic/action.py` & `ckanext-ingest-1.4.0/ckanext/ingest/views.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,62 @@
 from __future__ import annotations
 
-import itertools
-import logging
-import mimetypes
 from typing import Any
 
-import ckan.plugins.toolkit as tk
-from ckan.logic import validate
+from flask import Blueprint
+from flask.views import MethodView
 
-from ckanext.toolbelt.decorators import Collector
+import ckan.plugins.toolkit as tk
+from ckan.lib import base
+from ckan.logic import parse_params
 
-from .. import strategy
-from ..artifact import make_artifacts
-from . import schema
+from . import config
 
-log = logging.getLogger(__name__)
-action, get_actions = Collector("ingest").split()
+ingest = Blueprint("ingest", __name__)
 
 
-@action
-@validate(schema.extract_records)
-def extract_records(context, data_dict) -> list[dict[str, Any]]:
-    tk.check_access("ingest_extract_records", context, data_dict)
-    records = _extract_records(data_dict)
+class IngestView(MethodView):
+    def _check_access(self):
+        try:
+            tk.check_access("ingest_web_ui", {"user": tk.g.user})
+        except tk.NotAuthorized:
+            tk.abort(401, tk._("Unauthorized to ingest data"))
+
+    def _render(self, errors: dict[str, Any] | None = None):
+        data: dict[str, Any] = {
+            "user_dict": tk.g.userobj,
+            "errors": errors,
+            "base_template": config.base_template(),
+        }
+        return base.render("ingest/index.html", extra_vars=data)
+
+    def get(self):
+        self._check_access()
+        return self._render()
 
-    return [r.data for r in records]
+    def post(self):
+        self._check_access()
 
+        try:
+            data = parse_params(tk.request.form)
+            data.update(parse_params(tk.request.files))
+            result = tk.get_action("ingest_import_records")({}, data)
+
+            for id_ in result:
+                pkg = tk.get_action("package_show")({}, {"id": id_})
+                tk.h.flash_success(
+                    "Success: <a href='{url}'>{title}</a>".format(
+                        title=pkg["title"],
+                        url=tk.h.url_for(pkg["type"] + ".read", id=pkg["name"]),
+                    ),
+                    True,
+                )
 
-@action
-@validate(schema.import_records)
-def import_records(context, data_dict):
-    tk.check_access("ingest_import_records", context, data_dict)
+            return tk.redirect_to("ingest.index")
 
-    start = data_dict.get("start", 0)
-    rows = data_dict.get("rows")
-    if rows is not None:
-        rows += start
+        except tk.ValidationError as e:
+            errors = e.error_summary
 
-    artifacts = make_artifacts(data_dict["report"])
-    records = _extract_records(data_dict)
+        return self._render(errors), 409
 
-    for record in itertools.islice(records, start, rows):
-        record.set_options(data_dict)
-        record.fill(data_dict["defaults"], data_dict["overrides"])
-        try:
-            result = record.ingest({"user": context["user"]})
-        except tk.ValidationError as e:
-            artifacts.fail({"error": e.error_dict, "source": record.raw})
-        except tk.ObjectNotFound as e:
-            artifacts.fail(
-                {
-                    "error": e.message or "Package does not exists",
-                    "source": record.raw,
-                }
-            )
-
-        else:
-            artifacts.success({"result": result})
-
-    return artifacts.collect()
-
-
-def _extract_records(data_dict: dict[str, Any]):
-    mime, _encoding = mimetypes.guess_type(data_dict["source"].filename)
-    if not mime:
-        mime = data_dict["source"].content_type
-
-    handler = strategy.get_handler(mime, data_dict["source"])
-
-    if not handler:
-        raise tk.ValidationError(
-            {"source": [tk._("Unsupported MIMEType {mime}").format(mime=mime)]}
-        )
 
-    return handler.parse(data_dict["source"], data_dict["extras"])
+ingest.add_url_rule("/ingest/from-source", view_func=IngestView.as_view("index"))
```

### Comparing `ckanext-ingest-1.3.0/ckanext/ingest/logic/validators.py` & `ckanext-ingest-1.4.0/ckanext/ingest/logic/validators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from __future__ import annotations
 
 import uuid
+from typing import Any
 
-import ckan.lib.munge as munge
-
-from ckanext.toolbelt.decorators import Collector
+from ckan.lib import munge
 
 NAMESPACE_INGEST = uuid.uuid5(uuid.NAMESPACE_DNS, "ingest")
 
-validator, get_validators = Collector("ingest").split()
-
 
-@validator
-def into_uuid(value):
+def ingest_into_uuid(value: str):
     return str(uuid.uuid5(NAMESPACE_INGEST, value))
 
 
-@validator
-def munge_name(value):
+def ingest_munge_name(value: str):
     return munge.munge_name(value)
 
 
-@validator
-def strip_prefix(prefix):
-    def validator(value):
+def ingest_strip_prefix(prefix: str):
+    def validator(value: Any):
         if isinstance(value, str) and value.startswith(prefix):
             value = value[len(prefix) :]
         return value
 
     return validator
```

### Comparing `ckanext-ingest-1.3.0/ckanext/ingest/templates/ingest/index.html` & `ckanext-ingest-1.4.0/ckanext/ingest/templates/ingest/index.html`

 * *Files identical despite different names*

### Comparing `ckanext-ingest-1.3.0/ckanext/ingest/templates/ingest/snippets/ingest_form.html` & `ckanext-ingest-1.4.0/ckanext/ingest/templates/ingest/snippets/ingest_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-ingest-1.3.0/ckanext/ingest/tests/logic/test_action.py` & `ckanext-ingest-1.4.0/ckanext/ingest/tests/logic/test_action.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import mimetypes
 import os
 from typing import Optional
 
 import pytest
-from werkzeug.datastructures import FileStorage
 
 import ckan.plugins.toolkit as tk
 from ckan.tests.helpers import call_action
 
+from ckanext.ingest import shared
+
 
 @pytest.fixture(scope="session")
 def source():
     data = os.path.join(os.path.dirname(__file__), "data")
 
     def reader(filename: str, mime: Optional[str] = None):
         if mime is None:
             mime, _enc = mimetypes.guess_type(filename)
 
-        src = open(os.path.join(data, filename), "rb")
-        return FileStorage(src, content_type=mime)
+        src = open(os.path.join(data, filename), "rb")  # noqa
+        return shared.make_storage(src, mimetype=mime)
 
     return reader
 
 
 class TestExtractRecords:
     @pytest.mark.parametrize(
-        "filename", ["example.csv", "example.zip", "zipped_zip.zip"]
+        "filename",
+        ["example.csv", "example.zip", "zipped_zip.zip"],
     )
     def test_basic(self, source, filename):
         records = call_action("ingest_extract_records", source=source(filename))
+
         assert records == [
             {"name": "hello", "title": "Hello", "type": "dataset"},
             {"name": "world", "title": "World", "type": "dataset"},
         ]
 
     def test_no_source(self, source):
         with pytest.raises(tk.ValidationError):
@@ -42,15 +45,16 @@
         records = call_action("ingest_extract_records", source=source("unmapped.csv"))
         assert records == [{"type": "dataset"}, {"type": "dataset"}]
 
 
 @pytest.mark.usefixtures("clean_db")
 class TestImportRecords:
     @pytest.mark.parametrize(
-        "filename", ["example.csv", "example.zip", "zipped_zip.zip"]
+        "filename",
+        ["example.csv", "example.zip", "zipped_zip.zip"],
     )
     def test_basic(self, source, filename):
         result = call_action("ingest_import_records", source=source(filename))
         assert result == {"fail": 0, "success": 2}
 
     def test_no_source(self, source):
         with pytest.raises(tk.ValidationError):
```

### Comparing `ckanext-ingest-1.3.0/ckanext_ingest.egg-info/SOURCES.txt` & `ckanext-ingest-1.4.0/ckanext_ingest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 ckanext/__init__.py
 ckanext/ingest/__init__.py
 ckanext/ingest/artifact.py
 ckanext/ingest/cli.py
+ckanext/ingest/config.py
 ckanext/ingest/interfaces.py
 ckanext/ingest/plugin.py
 ckanext/ingest/record.py
-ckanext/ingest/registry.py
+ckanext/ingest/shared.py
 ckanext/ingest/transform.py
-ckanext/ingest/utils.py
 ckanext/ingest/views.py
 ckanext/ingest/logic/__init__.py
 ckanext/ingest/logic/action.py
 ckanext/ingest/logic/auth.py
 ckanext/ingest/logic/schema.py
 ckanext/ingest/logic/validators.py
 ckanext/ingest/strategy/__init__.py
-ckanext/ingest/strategy/base.py
 ckanext/ingest/strategy/csv.py
 ckanext/ingest/strategy/xlsx.py
 ckanext/ingest/strategy/zip.py
 ckanext/ingest/templates/ingest/index.html
 ckanext/ingest/templates/ingest/snippets/ingest_form.html
 ckanext/ingest/tests/__init__.py
 ckanext/ingest/tests/test_artifact.py
```

### Comparing `ckanext-ingest-1.3.0/setup.cfg` & `ckanext-ingest-1.4.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [metadata]
 name = ckanext-ingest
-version = 1.3.0
+version = 1.4.0
 description = 
-long_description = file: README.rst
-long_description_content_type = text/x-rst
+long_description = file: README.md
+long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-ingest
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
 classifiers = 
 	Development Status :: 4 - Beta
 	License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 keywords = 
 	CKAN
 
 [options]
-python_requires = >= 3.7
+python_requires = >= 3.8
 install_requires = 
 	typing_extensions
-	ckanext-toolbelt
 packages = find:
 namespace_packages = ckanext
 include_package_data = True
 
 [options.entry_points]
 ckan.plugins = 
 	ingest = ckanext.ingest.plugin:IngestPlugin
```

