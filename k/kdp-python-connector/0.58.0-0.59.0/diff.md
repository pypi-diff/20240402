# Comparing `tmp/kdp-python-connector-0.58.0.tar.gz` & `tmp/kdp-python-connector-0.59.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-python-connector-0.58.0.tar", last modified: Mon Apr  1 15:54:35 2024, max compression
+gzip compressed data, was "kdp-python-connector-0.59.0.tar", last modified: Mon Apr  1 18:20:02 2024, max compression
```

## Comparing `kdp-python-connector-0.58.0.tar` & `kdp-python-connector-0.59.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.876899 kdp-python-connector-0.58.0/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.848899 kdp-python-connector-0.58.0/.github/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      234 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/pull_request_template.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.848899 kdp-python-connector-0.58.0/.github/workflows/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6788 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/build-internal.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6340 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/build-public.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5028 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/release-internal.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4044 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/release-public.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3956 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.github/workflows/release.yaml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1869 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.gitignore
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/.nojekyll
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-01 15:54:35.876899 kdp-python-connector-0.58.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      272 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.852899 kdp-python-connector-0.58.0/datafiles/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13666 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/datafiles/actorfilms.csv
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.856899 kdp-python-connector-0.58.0/docs/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/.nojekyll
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      634 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/Makefile
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/conf.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/index.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/kdp_connector.configuration.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1581 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/kdp_connector.connectors.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      447 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/kdp_connector.rst
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      765 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/make.bat
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/docs/modules.rst
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.860899 kdp-python-connector-0.58.0/kdp_connector/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.860899 kdp-python-connector-0.58.0/kdp_connector/configuration/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3069 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/authenticationUtil.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/configurationUtil.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/keycloak_authentication.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      549 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/configuration/proxy_authentication.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.868899 kdp-python-connector-0.58.0/kdp_connector/connectors/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      669 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/Storage.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1585 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/audit_log.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3620 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/audit_log_configs.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7467 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/batch_write.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2205 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/index_management.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/ingest_job_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8752 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/kdp_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2302 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4760 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/read.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1892 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/connectors/upload.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25203 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/kdp_connector/main.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.872899 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1496 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-01 15:54:35.000000 kdp-python-connector-0.58.0/kdp_python_connector.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/pyproject.toml
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/requirements.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-01 15:54:35.876899 kdp-python-connector-0.58.0/setup.cfg
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 15:54:35.872899 kdp-python-connector-0.58.0/test/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      446 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/test/README.md
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4014 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/test/test_ingest.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1504 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/test/test_keycloak.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2024-04-01 15:54:25.000000 kdp-python-connector-0.58.0/test/test_read.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.448806 kdp-python-connector-0.59.0/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.436806 kdp-python-connector-0.59.0/.github/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      234 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/.github/pull_request_template.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.440806 kdp-python-connector-0.59.0/.github/workflows/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7347 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/.github/workflows/build-internal.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6899 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/.github/workflows/build-public.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5028 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/.github/workflows/release-internal.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4044 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/.github/workflows/release-public.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3956 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/.github/workflows/release.yaml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1869 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/.gitignore
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/.nojekyll
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-01 18:20:02.448806 kdp-python-connector-0.59.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      272 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.440806 kdp-python-connector-0.59.0/datafiles/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13666 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/datafiles/actorfilms.csv
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.440806 kdp-python-connector-0.59.0/docs/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/docs/.nojekyll
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      634 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/docs/Makefile
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2189 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/docs/conf.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      486 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/docs/index.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      684 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/docs/kdp_connector.configuration.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1581 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/docs/kdp_connector.connectors.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      447 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/docs/kdp_connector.rst
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      765 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/docs/make.bat
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/docs/modules.rst
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.440806 kdp-python-connector-0.59.0/kdp_connector/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       80 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.448806 kdp-python-connector-0.59.0/kdp_connector/configuration/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/configuration/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3069 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/configuration/authenticationUtil.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/configuration/configurationUtil.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2025 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/configuration/keycloak_authentication.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      454 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/configuration/proxy_authentication.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.448806 kdp-python-connector-0.59.0/kdp_connector/connectors/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      669 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/Storage.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1585 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/audit_log.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3620 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/audit_log_configs.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7467 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/batch_write.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2205 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/index_management.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2332 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/ingest_job_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8752 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/kdp_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2302 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4760 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/read.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1892 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/connectors/upload.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    25203 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/kdp_connector/main.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.448806 kdp-python-connector-0.59.0/kdp_python_connector.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      757 2024-04-01 18:20:02.000000 kdp-python-connector-0.59.0/kdp_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1496 2024-04-01 18:20:02.000000 kdp-python-connector-0.59.0/kdp_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-01 18:20:02.000000 kdp-python-connector-0.59.0/kdp_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       59 2024-04-01 18:20:02.000000 kdp-python-connector-0.59.0/kdp_python_connector.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-01 18:20:02.000000 kdp-python-connector-0.59.0/kdp_python_connector.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/pyproject.toml
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       32 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/requirements.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-01 18:20:02.448806 kdp-python-connector-0.59.0/setup.cfg
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-01 18:20:02.448806 kdp-python-connector-0.59.0/test/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      446 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/test/README.md
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4014 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/test/test_ingest.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1504 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/test/test_keycloak.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4926 2024-04-01 18:19:52.000000 kdp-python-connector-0.59.0/test/test_read.py
```

### Comparing `kdp-python-connector-0.58.0/.github/workflows/build-internal.yaml` & `kdp-python-connector-0.59.0/.github/workflows/build-public.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-name: KDP Python Connector Build (internal)
+name: KDP Python Connector Build (public)
 
 on:
   push:
   repository_dispatch:
-    types: [ build-connector, build-internal-connector ]
+    types: [ build-connector, build-public-connector ]
+
 
 env:
   VERSION: ${{ github.event.client_payload.version || '0.0.1' }}
-  PACKAGE_NAME: kdp-python-connector-internal
+  PACKAGE_NAME: kdp-python-connector
   CODE_ARTIFACT_DOMAIN: kdp
   CODE_ARTIFACT_REPO: kdp-python-connector
-  CODE_ARTIFACT_URL: https://us-west-2.console.aws.amazon.com/codesuite/codeartifact/d/365668498277/kdp/r/kdp-python-connector-internal/p/pypi/kdp-python-connector/versions?region=us-west-2&package-versions-meta=eyJmIjp7fSwicyI6e30sIm4iOjIwLCJpIjowfQ
+  CODE_ARTIFACT_URL: https://us-west-2.console.aws.amazon.com/codesuite/codeartifact/d/365668498277/kdp/r/kdp-python-connector/p/pypi/kdp-python-connector/versions?region=us-west-2&package-versions-meta=eyJmIjp7fSwicyI6e30sIm4iOjIwLCJpIjowfQ
   BRANCH_REF: ${{ github.event.client_payload.pythonConnectorRef || 'main' }}
-  PYTHON_CLIENT_VERSION: ${{ github.event.client_payload.pythonClientVersion || '4.122.0' }}
+  PYTHON_CLIENT_VERSION: ${{ github.event.client_payload.pythonClientVersion }}
   PYTHON_CLIENT_CODE_ARTIFACT_REPO: kdp-api-python-client
-  PYTHON_CLIENT_PACKAGE_NAME: kdp-api-python-client-internal
+  PYTHON_CLIENT_PACKAGE_NAME: kdp-api-python-client
 
 
 jobs:
-  build_internal_connector:
-    name: Build Internal Connector
+  build_public_connector:
+    name: Build Public Connector
     runs-on: self-hosted-aws-x86
 
     strategy:
       matrix:
         python-version: [ '3.8.x', '3.9.x' ]
 
     steps:
@@ -33,37 +34,38 @@
       - name: Checkout branch
         uses: actions/checkout@v4
         with:
           ref: ${{ env.BRANCH_REF }}
           fetch-depth: 0
 
       - name: Echo Payload
-        run: echo "Starting Build of Internal Connector with VERSION $VERSION BRANCH $BRANCH_REF"
-
-      - name: Update Package Name to internal package name in pyproject.toml
-        run: |
-          DEFAULT_PACKAGE_NAME=`cat pyproject.toml | grep ^name | cut -d '"' -f 2`
-          echo "Updating DEFAULT_PACKAGE_NAME: $DEFAULT_PACKAGE_NAME to NEW_PACKAGE_NAME: ${{ env.PACKAGE_NAME }} in pyproject.toml"          
-          sed -i "s+name = \"$DEFAULT_PACKAGE_NAME\"+name = \"${{ env.PACKAGE_NAME }}\"+g" pyproject.toml  
+        run: echo "Starting Build of Public Connector with VERSION $VERSION BRANCH $BRANCH_REF"
 
       - name: Update Python Connector Version Number in pyproject.toml
         run: |
           OLD_VERSION=`cat pyproject.toml | grep ^version | cut -d '"' -f 2`
           OLD_VERSION="\"$OLD_VERSION\""          
           NEW_VERSION="\"${{ env.VERSION }}\""
           echo "Updating OLD_VERSION: $OLD_VERSION to NEW_VERSION: $NEW_VERSION in pyproject.toml"          
           sed -i "s+version = $OLD_VERSION+version = $NEW_VERSION+g" pyproject.toml
 
       - name: Update Python Client Version in Dependencies in pyproject.toml
-        if: ${{ env.PYTHON_CLIENT_VERSION != '0.0.1' }}
+        if: ${{ env.PYTHON_CLIENT_VERSION != null || env.PYTHON_CLIENT_VERSION != '' }}
         run: |
           OLD_CLIENT_VERSION=`cat pyproject.toml | grep -F kdp-api-python-client | egrep -o "([0-9]{1,}\.)+[0-9]{1,}"`
           echo "Updating python client OLD_CLIENT_VERSION: $OLD_CLIENT_VERSION to NEW_CLIENT_VERSION: ${{ env.PYTHON_CLIENT_VERSION }} in pyproject.toml"
           sed -i "s+kdp-api-python-client ~= $OLD_CLIENT_VERSION+kdp-api-python-client ~= ${{ env.PYTHON_CLIENT_VERSION }}+g" pyproject.toml 
 
+      - name: Update Python Client Version to use pyproject.toml version if it was not provided
+        if: ${{ env.PYTHON_CLIENT_VERSION == null || env.PYTHON_CLIENT_VERSION == '' }}
+        run: |
+          PREVIOUS_CLIENT_VERSION=`cat pyproject.toml | grep -F kdp-api-python-client | egrep -o "([0-9]{1,}\.)+[0-9]{1,}"`
+          echo "PYTHON_CLIENT_VERSION not provided, setting to PREVIOUS_CLIENT_VERSION: $PREVIOUS_CLIENT_VERSION from pyproject.toml"
+          echo "PYTHON_CLIENT_VERSION=$PREVIOUS_CLIENT_VERSION" >> $GITHUB_ENV   
+
       - name: Show python project toml file content after updates
         run: |
           cat pyproject.toml
 
       - name: Remove and create new requirements.txt
         run: |
           rm requirements.txt
@@ -86,31 +88,31 @@
           python-version: ${{ matrix.python-version }}
 
       - name: install required dependencies for python client
         run: |
           python -m pip install --force-reinstall --user --upgrade python-dateutil urllib3==2.0.7 pydantic typing-extensions    
 
       - name: Install kdp-api-python-client package from AWS code artifact
-        run: |  
+        run: |
           aws codeartifact login --tool pip --domain ${{ env.CODE_ARTIFACT_DOMAIN }} --repository ${{ env.PYTHON_CLIENT_CODE_ARTIFACT_REPO }}
           pip install --no-cache-dir ${{ env.PYTHON_CLIENT_PACKAGE_NAME }}==${{ env.PYTHON_CLIENT_VERSION }}
           pip config list
           pip config --user set global.index-url https://pypi.org/simple
-          pip config list
+          pip config list          
 
       - name: Install dependencies
         run: |
           python -m pip install --user --upgrade build    
           pip install twine
 
       - name: Install Python Connector
         id: install-python-connector
         run: |
           pip install -r requirements.txt
-          python -m build --no-isolation       
+          python -m build --no-isolation           
 
       - name: Run tests
         id: run-unit-tests
         working-directory: ./test
         run: |
           python3 -m unittest
         continue-on-error: true
@@ -130,15 +132,15 @@
           --package ${{ env.PACKAGE_NAME }} --versions ${{ env.VERSION }}
         continue-on-error: true
 
       - name: reset pip config to default
         run: |
           pip config list
           pip config --user set global.index-url https://pypi.org/simple
-          pip config list  
+          pip config list      
 
       - name: Build and publish
         if: ${{ matrix.python-version == '3.9.x' }}
         run: |
           export TWINE_USERNAME=aws
           export TWINE_PASSWORD=`aws codeartifact get-authorization-token --domain ${{ env.CODE_ARTIFACT_DOMAIN }} --query authorizationToken --output text`
           export TWINE_REPOSITORY_URL=`aws codeartifact get-repository-endpoint --domain ${{ env.CODE_ARTIFACT_DOMAIN }} --repository ${{ env.CODE_ARTIFACT_REPO }} --format pypi --query repositoryEndpoint --output text`
@@ -146,8 +148,8 @@
 
       - name: Add logging to markdown
         if: always()
         run: |
           echo '<h4>Build Settings for python version: ${{ matrix.python-version }}</h4>' >> $GITHUB_STEP_SUMMARY
           echo '<a href="${{ env.CODE_ARTIFACT_URL }}">PYTHON-CONNECTOR AWS CODE ARTIFACT REPO</a>' >> $GITHUB_STEP_SUMMARY
           echo '<br />VERSION: ${{ env.VERSION }} <br />' >> $GITHUB_STEP_SUMMARY
-          echo 'PYTHON CONNECTOR BRANCH_NAME: ${{ env.BRANCH_REF }} <br />' >> $GITHUB_STEP_SUMMARY           
+          echo 'PYTHON CONNECTOR BRANCH_NAME: ${{ env.BRANCH_REF }} <br />' >> $GITHUB_STEP_SUMMARY
```

### Comparing `kdp-python-connector-0.58.0/.github/workflows/build-public.yaml` & `kdp-python-connector-0.59.0/.github/workflows/build-internal.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-name: KDP Python Connector Build (public)
+name: KDP Python Connector Build (internal)
 
 on:
   push:
   repository_dispatch:
-    types: [ build-connector, build-public-connector ]
-
+    types: [ build-connector, build-internal-connector ]
 
 env:
   VERSION: ${{ github.event.client_payload.version || '0.0.1' }}
-  PACKAGE_NAME: kdp-python-connector
+  PACKAGE_NAME: kdp-python-connector-internal
   CODE_ARTIFACT_DOMAIN: kdp
   CODE_ARTIFACT_REPO: kdp-python-connector
-  CODE_ARTIFACT_URL: https://us-west-2.console.aws.amazon.com/codesuite/codeartifact/d/365668498277/kdp/r/kdp-python-connector/p/pypi/kdp-python-connector/versions?region=us-west-2&package-versions-meta=eyJmIjp7fSwicyI6e30sIm4iOjIwLCJpIjowfQ
+  CODE_ARTIFACT_URL: https://us-west-2.console.aws.amazon.com/codesuite/codeartifact/d/365668498277/kdp/r/kdp-python-connector-internal/p/pypi/kdp-python-connector/versions?region=us-west-2&package-versions-meta=eyJmIjp7fSwicyI6e30sIm4iOjIwLCJpIjowfQ
   BRANCH_REF: ${{ github.event.client_payload.pythonConnectorRef || 'main' }}
-  PYTHON_CLIENT_VERSION: ${{ github.event.client_payload.pythonClientVersion || '4.122.0' }}
+  PYTHON_CLIENT_VERSION: ${{ github.event.client_payload.pythonClientVersion }}
   PYTHON_CLIENT_CODE_ARTIFACT_REPO: kdp-api-python-client
-  PYTHON_CLIENT_PACKAGE_NAME: kdp-api-python-client
+  PYTHON_CLIENT_PACKAGE_NAME: kdp-api-python-client-internal
 
 
 jobs:
-  build_public_connector:
-    name: Build Public Connector
+  build_internal_connector:
+    name: Build Internal Connector
     runs-on: self-hosted-aws-x86
 
     strategy:
       matrix:
         python-version: [ '3.8.x', '3.9.x' ]
 
     steps:
@@ -34,31 +33,44 @@
       - name: Checkout branch
         uses: actions/checkout@v4
         with:
           ref: ${{ env.BRANCH_REF }}
           fetch-depth: 0
 
       - name: Echo Payload
-        run: echo "Starting Build of Public Connector with VERSION $VERSION BRANCH $BRANCH_REF"
+        run: echo "Starting Build of Internal Connector with VERSION $VERSION BRANCH $BRANCH_REF"
+
+      - name: Update Package Name to internal package name in pyproject.toml
+        run: |
+          DEFAULT_PACKAGE_NAME=`cat pyproject.toml | grep ^name | cut -d '"' -f 2`
+          echo "Updating DEFAULT_PACKAGE_NAME: $DEFAULT_PACKAGE_NAME to NEW_PACKAGE_NAME: ${{ env.PACKAGE_NAME }} in pyproject.toml"          
+          sed -i "s+name = \"$DEFAULT_PACKAGE_NAME\"+name = \"${{ env.PACKAGE_NAME }}\"+g" pyproject.toml  
 
       - name: Update Python Connector Version Number in pyproject.toml
         run: |
           OLD_VERSION=`cat pyproject.toml | grep ^version | cut -d '"' -f 2`
           OLD_VERSION="\"$OLD_VERSION\""          
           NEW_VERSION="\"${{ env.VERSION }}\""
           echo "Updating OLD_VERSION: $OLD_VERSION to NEW_VERSION: $NEW_VERSION in pyproject.toml"          
           sed -i "s+version = $OLD_VERSION+version = $NEW_VERSION+g" pyproject.toml
 
       - name: Update Python Client Version in Dependencies in pyproject.toml
-        if: ${{ env.PYTHON_CLIENT_VERSION != '0.0.1' }}
+        if: ${{ env.PYTHON_CLIENT_VERSION != null || env.PYTHON_CLIENT_VERSION != '' }}
         run: |
           OLD_CLIENT_VERSION=`cat pyproject.toml | grep -F kdp-api-python-client | egrep -o "([0-9]{1,}\.)+[0-9]{1,}"`
           echo "Updating python client OLD_CLIENT_VERSION: $OLD_CLIENT_VERSION to NEW_CLIENT_VERSION: ${{ env.PYTHON_CLIENT_VERSION }} in pyproject.toml"
           sed -i "s+kdp-api-python-client ~= $OLD_CLIENT_VERSION+kdp-api-python-client ~= ${{ env.PYTHON_CLIENT_VERSION }}+g" pyproject.toml 
 
+      - name: Update Python Client Version to use pyproject.toml version if it was not provided
+        if: ${{ env.PYTHON_CLIENT_VERSION == null || env.PYTHON_CLIENT_VERSION == '' }}
+        run: |
+          PREVIOUS_CLIENT_VERSION=`cat pyproject.toml | grep -F kdp-api-python-client | egrep -o "([0-9]{1,}\.)+[0-9]{1,}"`
+          echo "PYTHON_CLIENT_VERSION not provided, setting to PREVIOUS_CLIENT_VERSION: $PREVIOUS_CLIENT_VERSION from pyproject.toml"
+          echo "PYTHON_CLIENT_VERSION=$PREVIOUS_CLIENT_VERSION" >> $GITHUB_ENV   
+
       - name: Show python project toml file content after updates
         run: |
           cat pyproject.toml
 
       - name: Remove and create new requirements.txt
         run: |
           rm requirements.txt
@@ -81,31 +93,31 @@
           python-version: ${{ matrix.python-version }}
 
       - name: install required dependencies for python client
         run: |
           python -m pip install --force-reinstall --user --upgrade python-dateutil urllib3==2.0.7 pydantic typing-extensions    
 
       - name: Install kdp-api-python-client package from AWS code artifact
-        run: |
+        run: |  
           aws codeartifact login --tool pip --domain ${{ env.CODE_ARTIFACT_DOMAIN }} --repository ${{ env.PYTHON_CLIENT_CODE_ARTIFACT_REPO }}
           pip install --no-cache-dir ${{ env.PYTHON_CLIENT_PACKAGE_NAME }}==${{ env.PYTHON_CLIENT_VERSION }}
           pip config list
           pip config --user set global.index-url https://pypi.org/simple
-          pip config list          
+          pip config list
 
       - name: Install dependencies
         run: |
           python -m pip install --user --upgrade build    
           pip install twine
 
       - name: Install Python Connector
         id: install-python-connector
         run: |
           pip install -r requirements.txt
-          python -m build --no-isolation           
+          python -m build --no-isolation       
 
       - name: Run tests
         id: run-unit-tests
         working-directory: ./test
         run: |
           python3 -m unittest
         continue-on-error: true
@@ -125,15 +137,15 @@
           --package ${{ env.PACKAGE_NAME }} --versions ${{ env.VERSION }}
         continue-on-error: true
 
       - name: reset pip config to default
         run: |
           pip config list
           pip config --user set global.index-url https://pypi.org/simple
-          pip config list      
+          pip config list  
 
       - name: Build and publish
         if: ${{ matrix.python-version == '3.9.x' }}
         run: |
           export TWINE_USERNAME=aws
           export TWINE_PASSWORD=`aws codeartifact get-authorization-token --domain ${{ env.CODE_ARTIFACT_DOMAIN }} --query authorizationToken --output text`
           export TWINE_REPOSITORY_URL=`aws codeartifact get-repository-endpoint --domain ${{ env.CODE_ARTIFACT_DOMAIN }} --repository ${{ env.CODE_ARTIFACT_REPO }} --format pypi --query repositoryEndpoint --output text`
@@ -141,8 +153,8 @@
 
       - name: Add logging to markdown
         if: always()
         run: |
           echo '<h4>Build Settings for python version: ${{ matrix.python-version }}</h4>' >> $GITHUB_STEP_SUMMARY
           echo '<a href="${{ env.CODE_ARTIFACT_URL }}">PYTHON-CONNECTOR AWS CODE ARTIFACT REPO</a>' >> $GITHUB_STEP_SUMMARY
           echo '<br />VERSION: ${{ env.VERSION }} <br />' >> $GITHUB_STEP_SUMMARY
-          echo 'PYTHON CONNECTOR BRANCH_NAME: ${{ env.BRANCH_REF }} <br />' >> $GITHUB_STEP_SUMMARY          
+          echo 'PYTHON CONNECTOR BRANCH_NAME: ${{ env.BRANCH_REF }} <br />' >> $GITHUB_STEP_SUMMARY
```

### Comparing `kdp-python-connector-0.58.0/.github/workflows/release-internal.yaml` & `kdp-python-connector-0.59.0/.github/workflows/release-internal.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/.github/workflows/release-public.yaml` & `kdp-python-connector-0.59.0/.github/workflows/release-public.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/.github/workflows/release.yaml` & `kdp-python-connector-0.59.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/.gitignore` & `kdp-python-connector-0.59.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/PKG-INFO` & `kdp-python-connector-0.59.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdp-python-connector
-Version: 0.58.0
+Version: 0.59.0
 Summary: Python Connector for KDP Platform
 Author-email: Koverse development team <developer@koverse.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `kdp-python-connector-0.58.0/datafiles/actorfilms.csv` & `kdp-python-connector-0.59.0/datafiles/actorfilms.csv`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/docs/Makefile` & `kdp-python-connector-0.59.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/docs/conf.py` & `kdp-python-connector-0.59.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/docs/kdp_connector.configuration.rst` & `kdp-python-connector-0.59.0/docs/kdp_connector.configuration.rst`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/docs/kdp_connector.connectors.rst` & `kdp-python-connector-0.59.0/docs/kdp_connector.connectors.rst`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/docs/make.bat` & `kdp-python-connector-0.59.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/configuration/authenticationUtil.py` & `kdp-python-connector-0.59.0/kdp_connector/configuration/authenticationUtil.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/configuration/configurationUtil.py` & `kdp-python-connector-0.59.0/kdp_connector/configuration/configurationUtil.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/configuration/keycloak_authentication.py` & `kdp-python-connector-0.59.0/kdp_connector/configuration/keycloak_authentication.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/Storage.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/Storage.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/audit_log.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/audit_log.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/audit_log_configs.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/audit_log_configs.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/batch_write.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/batch_write.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/index_management.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/index_management.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/ingest_job_api.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/ingest_job_api.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/kdp_api.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/kdp_api.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/query.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/query.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/read.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/read.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/connectors/upload.py` & `kdp-python-connector-0.59.0/kdp_connector/connectors/upload.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_connector/main.py` & `kdp-python-connector-0.59.0/kdp_connector/main.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/kdp_python_connector.egg-info/PKG-INFO` & `kdp-python-connector-0.59.0/kdp_python_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kdp-python-connector
-Version: 0.58.0
+Version: 0.59.0
 Summary: Python Connector for KDP Platform
 Author-email: Koverse development team <developer@koverse.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `kdp-python-connector-0.58.0/kdp_python_connector.egg-info/SOURCES.txt` & `kdp-python-connector-0.59.0/kdp_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/pyproject.toml` & `kdp-python-connector-0.59.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-version = "0.58.0"
+version = "0.59.0"
 dependencies = [
   'kdp-api-python-client ~= 4.124.0',
   'pandas ~= 1.4.2',
   'numpy ~= 1.22.4'
 ]
 
 [tool.setuptools.packages.find]
```

### Comparing `kdp-python-connector-0.58.0/test/test_ingest.py` & `kdp-python-connector-0.59.0/test/test_ingest.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/test/test_keycloak.py` & `kdp-python-connector-0.59.0/test/test_keycloak.py`

 * *Files identical despite different names*

### Comparing `kdp-python-connector-0.58.0/test/test_read.py` & `kdp-python-connector-0.59.0/test/test_read.py`

 * *Files identical despite different names*

