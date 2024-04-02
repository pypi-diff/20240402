# Comparing `tmp/etos_environment_provider-3.2.2.tar.gz` & `tmp/etos_environment_provider-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_environment_provider-3.2.2.tar", last modified: Mon Mar 11 13:56:00 2024, max compression
+gzip compressed data, was "etos_environment_provider-4.0.0.tar", last modified: Thu Mar 28 07:12:42 2024, max compression
```

## Comparing `etos_environment_provider-3.2.2.tar` & `etos_environment_provider-4.0.0.tar`

### file list

```diff
@@ -1,161 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.040532 etos_environment_provider-3.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.016532 etos_environment_provider-3.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.020532 etos_environment_provider-3.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/.github/workflows/build-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-11 13:56:00.040532 etos_environment_provider-3.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.020532 etos_environment_provider-3.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.020532 etos_environment_provider-3.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.016532 etos_environment_provider-3.2.2/manifests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.020532 etos_environment_provider-3.2.2/manifests/base/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.024532 etos_environment_provider-3.2.2/manifests/base/api/
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/manifests/base/api/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/manifests/base/api/service-account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/manifests/base/api/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/manifests/base/kustomization.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.024532 etos_environment_provider-3.2.2/manifests/base/worker/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/manifests/base/worker/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/manifests/base/worker/service-account.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-03-11 13:56:00.044532 etos_environment_provider-3.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.016532 etos_environment_provider-3.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.024532 etos_environment_provider-3.2.2/src/environment_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22823 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/environment_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.024532 etos_environment_provider-3.2.2/src/environment_provider/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/join.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/json_dumps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/log_area.py
--rw-r--r--   0 runner    (1001) docker     (127)    10029 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/lib/uuid_generate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.024532 etos_environment_provider-3.2.2/src/environment_provider/splitter/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider/splitter/split.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.028532 etos_environment_provider-3.2.2/src/environment_provider_api/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.028532 etos_environment_provider-3.2.2/src/environment_provider_api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/backend/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/backend/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/backend/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/backend/register.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.028532 etos_environment_provider-3.2.2/src/environment_provider_api/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/middleware/json_translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/middleware/require_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    14279 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/environment_provider_api/webserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.040532 etos_environment_provider-3.2.2/src/etos_environment_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-03-11 13:55:59.000000 etos_environment_provider-3.2.2/src/etos_environment_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-03-11 13:56:00.000000 etos_environment_provider-3.2.2/src/etos_environment_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 13:55:59.000000 etos_environment_provider-3.2.2/src/etos_environment_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 13:55:59.000000 etos_environment_provider-3.2.2/src/etos_environment_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-11 13:55:59.000000 etos_environment_provider-3.2.2/src/etos_environment_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-11 13:55:59.000000 etos_environment_provider-3.2.2/src/etos_environment_provider.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.028532 etos_environment_provider-3.2.2/src/execution_space_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/execution_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/execution_space_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.028532 etos_environment_provider-3.2.2/src/execution_space_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.032532 etos_environment_provider-3.2.2/src/execution_space_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/utilities/instructions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/execution_space_provider/utilities/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.032532 etos_environment_provider-3.2.2/src/iut_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/iut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/iut_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.032532 etos_environment_provider-3.2.2/src/iut_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.032532 etos_environment_provider-3.2.2/src/iut_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12054 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/utilities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/iut_provider/utilities/prepare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.036532 etos_environment_provider-3.2.2/src/log_area_provider/
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/log_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/log_area_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.036532 etos_environment_provider-3.2.2/src/log_area_provider/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/schemas/external_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/schemas/jsontas_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.036532 etos_environment_provider-3.2.2/src/log_area_provider/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/utilities/checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/utilities/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/utilities/external_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/utilities/jsontas_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/src/log_area_provider/utilities/list.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.036532 etos_environment_provider-3.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.040532 etos_environment_provider-3.2.2/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/backend/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/backend/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10750 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/backend/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/backend/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.040532 etos_environment_provider-3.2.2/tests/external_execution_space/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/external_execution_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/external_execution_space/test_external_execution_space.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.040532 etos_environment_provider-3.2.2/tests/external_iut/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/external_iut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24107 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/external_iut/test_external_iut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.040532 etos_environment_provider-3.2.2/tests/external_log_area/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/external_log_area/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/external_log_area/test_external_log_area.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.040532 etos_environment_provider-3.2.2/tests/library/
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/library/fake_celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/library/fake_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/library/fake_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/library/fake_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/library/graphql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:56:00.040532 etos_environment_provider-3.2.2/tests/splitter/
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/splitter/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/tercc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15724 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/test_environment_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11636 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/test_webserver_configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7549 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/test_webserver_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tests/test_webserver_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-11 13:55:54.000000 etos_environment_provider-3.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.014511 etos_environment_provider-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.990511 etos_environment_provider-4.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.github/workflows/build-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)    10850 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-28 07:12:42.014511 etos_environment_provider-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7634 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9233 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.994511 etos_environment_provider-4.0.0/manifests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/manifests/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/manifests/base/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/api/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/api/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/api/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.998511 etos_environment_provider-4.0.0/manifests/base/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/worker/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/manifests/base/worker/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-28 07:12:42.014511 etos_environment_provider-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:41.994511 etos_environment_provider-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.002511 etos_environment_provider-4.0.0/src/environment_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22823 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/environment_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.002511 etos_environment_provider-4.0.0/src/environment_provider/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/json_dumps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/log_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7280 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/lib/uuid_generate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.002511 etos_environment_provider-4.0.0/src/environment_provider/splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/environment_provider/splitter/split.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.014511 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-28 07:12:41.000000 etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/execution_space_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/execution_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/execution_space_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/execution_space_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8247 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/execution_space_provider/utilities/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/iut_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/iut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/iut_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/iut_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.006511 etos_environment_provider-4.0.0/src/iut_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12054 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/iut_provider/utilities/prepare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/src/log_area_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/log_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/log_area_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/src/log_area_provider/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/schemas/external_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/schemas/jsontas_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/src/log_area_provider/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/external_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/jsontas_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/src/log_area_provider/utilities/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/external_execution_space/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_execution_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_execution_space/test_external_execution_space.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/external_iut/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_iut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24107 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_iut/test_external_iut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/external_log_area/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_log_area/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24737 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/external_log_area/test_external_log_area.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/library/fake_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/library/fake_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/library/graphql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 07:12:42.010511 etos_environment_provider-4.0.0/tests/splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/splitter/test_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/tercc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tests/test_environment_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-28 07:12:36.000000 etos_environment_provider-4.0.0/tox.ini
```

### Comparing `etos_environment_provider-3.2.2/.coveragerc` & `etos_environment_provider-4.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/.github/workflows/build-push.yml` & `etos_environment_provider-4.0.0/.github/workflows/build-push.yml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/.github/workflows/main.yml` & `etos_environment_provider-4.0.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/.gitignore` & `etos_environment_provider-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/LICENSE.txt` & `etos_environment_provider-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/PKG-INFO` & `etos_environment_provider-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_environment_provider
-Version: 3.2.2
+Version: 4.0.0
 Summary: Environment provider for ETOS.
 Home-page: https://github.com/eiffel-community/etos-environment-provider
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
@@ -17,15 +17,14 @@
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: eventlet~=0.33
 Requires-Dist: celery~=5.3
 Requires-Dist: cryptography<43.0.0,>=42.0.4
 Requires-Dist: gevent~=23.7
 Requires-Dist: gunicorn~=19.9
-Requires-Dist: falcon~=3.1
 Requires-Dist: jsontas~=1.3
 Requires-Dist: packageurl-python~=0.11
 Requires-Dist: etcd3gw~=2.3
 Requires-Dist: etos_lib==4.0.0
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `etos_environment_provider-3.2.2/README.rst` & `etos_environment_provider-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/docs/Makefile` & `etos_environment_provider-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/docs/conf.py` & `etos_environment_provider-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/manifests/base/api/deployment.yaml` & `etos_environment_provider-4.0.0/manifests/base/api/deployment.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/manifests/base/kustomization.yaml` & `etos_environment_provider-4.0.0/manifests/base/kustomization.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/manifests/base/worker/deployment.yaml` & `etos_environment_provider-4.0.0/manifests/base/worker/deployment.yaml`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/setup.cfg` & `etos_environment_provider-4.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	eventlet~=0.33
 	celery~=5.3
 	cryptography>=42.0.4,<43.0.0
 	gevent~=23.7
 	gunicorn~=19.9
-	falcon~=3.1
 	jsontas~=1.3
 	packageurl-python~=0.11
 	etcd3gw~=2.3
 	etos_lib==4.0.0
 python_requires = >=3.8
 
 [options.package_data]
```

### Comparing `etos_environment_provider-3.2.2/setup.py` & `etos_environment_provider-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/__init__.py` & `etos_environment_provider-4.0.0/src/environment_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/environment_provider.py` & `etos_environment_provider-4.0.0/src/environment_provider/environment_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/__init__.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/celery.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/celery.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/config.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/config.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/database.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/encrypt.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/encrypt.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/graphql.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/graphql.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/join.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/join.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/json_dumps.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/json_dumps.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/log_area.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/registry.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/registry.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 from collections import OrderedDict
 from typing import Optional
 
 import jsonschema
 from etos_lib.etos import ETOS
 from jsontas.jsontas import JsonTas
 
-from execution_space_provider import ExecutionSpaceProvider, execution_space_provider_schema
-from iut_provider import IutProvider, iut_provider_schema
-from log_area_provider import LogAreaProvider, log_area_provider_schema
+from execution_space_provider import ExecutionSpaceProvider
+from iut_provider import IutProvider
+from log_area_provider import LogAreaProvider
 
 from .database import ETCDPath
 
 
 class ProviderRegistry:
     """Environment provider registry."""
 
@@ -124,43 +124,14 @@
         """
         self.logger.info("Getting execution space provider %r", provider_id)
         provider = self.providers.join(f"execution-space/{provider_id}").read()
         if provider:
             return json.loads(provider, object_pairs_hook=OrderedDict)
         return None
 
-    def register_log_area_provider(self, ruleset: dict) -> None:
-        """Register a new log area provider.
-
-        :param ruleset: Log area JSON definition to register.
-        """
-        data = self.validate(ruleset, log_area_provider_schema(ruleset))
-        self.logger.info("Registering %r", data["log"]["id"])
-        self.providers.join(f"log-area/{data['log']['id']}").write(json.dumps(data))
-
-    def register_iut_provider(self, ruleset: dict) -> None:
-        """Register a new IUT provider.
-
-        :param ruleset: IUT provider JSON definition to register.
-        """
-        data = self.validate(ruleset, iut_provider_schema(ruleset))
-        self.logger.info("Registering %r", data["iut"]["id"])
-        self.providers.join(f"iut/{data['iut']['id']}").write(json.dumps(data))
-
-    def register_execution_space_provider(self, ruleset: dict) -> None:
-        """Register a new execution space provider.
-
-        :param ruleset: Execution space provider JSON definition to register.
-        """
-        data = self.validate(ruleset, execution_space_provider_schema(ruleset))
-        self.logger.info("Registering %r", data["execution_space"]["id"])
-        self.providers.join(f"execution-space/{data['execution_space']['id']}").write(
-            json.dumps(data)
-        )
-
     def execution_space_provider(self) -> Optional[ExecutionSpaceProvider]:
         """Get the execution space provider configured to suite ID.
 
         :return: Execution space provider object.
         """
         provider_json = self.testrun.join("provider/execution-space").read()
         if provider_json:
@@ -210,40 +181,7 @@
 
         :return: Dataset JSON data.
         """
         dataset = self.testrun.join("provider/dataset").read()
         if dataset:
             return json.loads(dataset)
         return None
-
-    # pylint:disable=too-many-arguments
-    def configure_environment_provider_for_suite(
-        self,
-        iut_provider: dict,
-        log_area_provider: dict,
-        execution_space_provider: dict,
-        dataset: dict,
-    ) -> None:
-        """Configure environment provider for a suite ID with providers and dataset.
-
-        :param iut_provider: IUT provider definition to configure for suite ID.
-        :param log_area_provider: Log area provider definition to configure for suite ID.
-        :param execution_space_provider: Execution space provider definition to configure
-                                         for suite ID.
-        :param dataset: Dataset to configure for suite ID.
-        """
-        self.logger.info("Configuring environment provider.")
-        self.logger.info("Dataset: %r", dataset)
-        self.logger.info("IUT provider: %r", iut_provider.get("iut", {}).get("id"))
-        self.logger.info(
-            "Execution space provider: %r",
-            execution_space_provider.get("execution_space", {}).get("id"),
-        )
-        self.logger.info("Log area provider: %r", log_area_provider.get("log", {}).get("id"))
-        self.logger.info("Expire: 3600")
-
-        self.testrun.join("provider/dataset").write(json.dumps(dataset), expire=3600)
-        self.testrun.join("provider/iut").write(json.dumps(iut_provider), expire=3600)
-        self.testrun.join("provider/log-area").write(json.dumps(log_area_provider), expire=3600)
-        self.testrun.join("provider/execution-space").write(
-            json.dumps(execution_space_provider), expire=3600
-        )
```

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/test_suite.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/test_suite.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/lib/uuid_generate.py` & `etos_environment_provider-4.0.0/src/environment_provider/lib/uuid_generate.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/splitter/__init__.py` & `etos_environment_provider-4.0.0/src/environment_provider/splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider/splitter/split.py` & `etos_environment_provider-4.0.0/src/environment_provider/splitter/split.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/environment_provider_api/backend/__init__.py` & `etos_environment_provider-4.0.0/tests/external_log_area/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Backend services for the environment provider webserver."""
+"""External log area provider tests."""
```

### Comparing `etos_environment_provider-3.2.2/src/environment_provider_api/backend/environment.py` & `etos_environment_provider-4.0.0/src/environment_provider/environment.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,57 +14,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Backend for the environment requests."""
 import json
 import traceback
 from typing import Optional, Union
 
-from celery import Celery
 from etos_lib import ETOS
-from falcon import Request
 from jsontas.jsontas import JsonTas
 
-from environment_provider.environment_provider import get_environment
 from environment_provider.lib.database import ETCDPath
 from environment_provider.lib.registry import ProviderRegistry
 from execution_space_provider import ExecutionSpaceProvider
 from execution_space_provider.execution_space import ExecutionSpace
 from iut_provider import IutProvider
 from iut_provider.iut import Iut
 from log_area_provider import LogAreaProvider
 from log_area_provider.log_area import LogArea
 
 
-def get_environment_id(request: Request) -> Optional[str]:
-    """Get the environment ID from request.
-
-    :param request: The falcon request object.
-    :return: The ID of the environment.
-    """
-    return request.get_param("id")
-
-
-def get_release_id(request: Request) -> Optional[str]:
-    """Get the task ID to release, from request.
-
-    :param request: The falcon request object.
-    :return: The ID of the environment to release.
-    """
-    return request.get_param("release")
-
-
-def get_single_release_id(request: Request) -> Optional[str]:
-    """Get the environment ID to release, from request.
-
-    :param request: The falcon request object.
-    :return: The ID of the environment to release.
-    """
-    return request.get_param("single_release")
-
-
 def checkin_provider(
     item: dict, provider: Union[IutProvider, ExecutionSpaceProvider, LogAreaProvider]
 ) -> tuple[bool, Optional[Exception]]:
     """Check in a provider.
 
     :param item: Item to check in.
     :param provider: The provider to use for check in.
@@ -130,50 +100,21 @@
     :param jsontas: JSONTas instance.
     :return: Release status and a message if status is False.
     """
     failure = None
     registry = ProviderRegistry(etos, jsontas, suite_id)
     for suite, metadata in registry.testrun.join("suite").read_all():
         suite = json.loads(suite)
-        try:
-            failure = release_environment(etos, jsontas, registry, suite)
-        except json.JSONDecodeError as exception:
-            failure = exception
+        for sub_suite in suite.get("sub_suites", []):
+            try:
+                failure = release_environment(etos, jsontas, registry, sub_suite)
+            except json.JSONDecodeError as exception:
+                failure = exception
         ETCDPath(metadata.get("key")).delete()
     registry.testrun.delete_all()
 
     if failure:
         # Return the traceback from exception stored in failure.
         return False, "".join(
             traceback.format_exception(failure, value=failure, tb=failure.__traceback__)
         )
     return True, ""
-
-
-def check_environment_status(celery_worker: Celery, environment_id: str) -> dict:
-    """Check the status of the environment that is being requested.
-
-    :param celery_worker: The worker holding the task results.
-    :param environment_id: The environment ID to check status on.
-    :return: A dictionary of status and and result.
-    """
-    task_result = celery_worker.AsyncResult(environment_id)
-    result = task_result.result
-    status = task_result.status
-    if isinstance(result, Exception):
-        status = "FAILURE"
-        result = str(result)
-    elif result and result.get("error") is not None:
-        status = "FAILURE"
-    if result:
-        task_result.get()
-    return {"status": status, "result": result}
-
-
-def request_environment(suite_id: str, suite_runner_ids: list[str]) -> str:
-    """Request an environment for a test suite ID.
-
-    :param suite_id: Suite ID to request an environment for.
-    :param suite_runner_ids: Suite runner correlation IDs.
-    :return: The task ID for the request.
-    """
-    return get_environment.delay(suite_id, suite_runner_ids).id
```

### Comparing `etos_environment_provider-3.2.2/src/environment_provider_api/middleware/__init__.py` & `etos_environment_provider-4.0.0/src/iut_provider/utilities/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,10 +9,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ETOS environment provider API middleware module."""
-from .json_translator import JSONTranslator
-from .require_json import RequireJSON
+"""Utilities for the IUT provider."""
```

### Comparing `etos_environment_provider-3.2.2/src/environment_provider_api/middleware/json_translator.py` & `etos_environment_provider-4.0.0/src/iut_provider/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,24 +9,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""JSON translator module."""
-import falcon
+"""ETOS IUT provider module."""
+import pathlib
 
-# pylint: disable=too-few-public-methods
+from .iut_provider import IutProvider
 
+__all__ = ["IutProvider", "iut_provider_schema"]
 
-class JSONTranslator:
-    """Translate request media to JSON."""
+IUT_PROVIDER_SCHEMA = (
+    pathlib.Path(__file__).parent.resolve().joinpath("./schemas/jsontas_schema.json")
+)
+EXTERNAL_IUT_PROVIDER_SCHEMA = (
+    pathlib.Path(__file__).parent.resolve().joinpath("./schemas/external_schema.json")
+)
 
-    def process_request(self, req: falcon.Request, _) -> None:
-        """Process request."""
-        if req.content_length in (None, 0):
-            return
 
-        body = req.media
-        if not body:
-            raise falcon.HTTPBadRequest("Empty request body", "A valid JSON document is required.")
+def iut_provider_schema(ruleset: dict) -> pathlib.Path:
+    """Get IUT provider schema for json validation.
+
+    :param ruleset: Ruleset to get an IUT provider schema for.
+    """
+    if ruleset.get("iut", {}).get("type", "jsontas") == "external":
+        return EXTERNAL_IUT_PROVIDER_SCHEMA
+    else:
+        return IUT_PROVIDER_SCHEMA
```

### Comparing `etos_environment_provider-3.2.2/src/environment_provider_api/middleware/require_json.py` & `etos_environment_provider-4.0.0/tests/splitter/test_splitter.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,30 +9,51 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Require JSON module."""
-import falcon
+"""Integration tests for the environment provider splitter."""
+import logging
+import unittest
 
-# pylint: disable=too-few-public-methods
+from etos_lib import ETOS
 
+from environment_provider.splitter.split import Splitter
 
-class RequireJSON:
-    """Require Accept: application/json headers for this API."""
 
-    def process_request(self, req: falcon.Request, _) -> None:
-        """Process request."""
-        if not req.client_accepts_json:
-            raise falcon.HTTPNotAcceptable(
-                "This API only supports responses encoded as JSON.",
-                href="http://docs.examples.com/api/json",
-            )
+class TestSplitter(unittest.TestCase):
+    """Test the environment provider slitter."""
+
+    logger = logging.getLogger(__name__)
+
+    def test_assign_iuts(self) -> None:
+        """Test that that a test runner never gets 0 number of IUTs assigned.
+
+        Approval criteria:
+            - A test runner shall never had 0 number of IUTs assigned.
 
-        if req.method in ("POST", "PUT"):
-            if req.content_type is None or "application/json" not in req.content_type:
-                raise falcon.HTTPUnsupportedMediaType(
-                    "This API only supports requests encoded as JSON.",
-                    href="http://docs.examples.com/api/json",
-                )
+        Test steps::
+            1. Assign IUTs to the provided test runners.
+            2. Verify that no test runner get 0 assigned IUTs.
+        """
+        iuts = ["iut1", "iut2"]
+        test_runners = {
+            "runner1": {"iuts": {}, "unsplit_recipes": [1]},
+            "runner2": {"iuts": {}, "unsplit_recipes": [2, 3, 4, 5]},
+        }
+
+        etos = ETOS("testing_etos", "testing_etos", "testing_etos")
+        etos.config.set("TOTAL_TEST_COUNT", 5)
+        etos.config.set("NUMBER_OF_IUTS", len(iuts))
+
+        self.logger.info("STEP: Assign IUTs to the provided test runners.")
+        _ = Splitter(etos, {}).assign_iuts(test_runners, iuts)
+
+        self.logger.info("STEP: Verify that no test runner get 0 assigned IUTs.")
+        for test_runner in test_runners.values():
+            self.assertNotEqual(
+                test_runner.get("number_of_iuts"),
+                0,
+                f"'number_of_iuts' is 0, test_runner got 0 assigned IUTs. {test_runner}]",
+            )
```

### Comparing `etos_environment_provider-3.2.2/src/environment_provider_api/webserver.py` & `etos_environment_provider-4.0.0/src/iut_provider/utilities/external_provider.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,360 +9,308 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ETOS Environment Provider webserver module."""
-import json
+"""IUT provider for external providers."""
 import logging
 import os
-from pathlib import Path
-from typing import Iterator
-
-import falcon
-from celery import Celery
-from etos_lib.etos import ETOS
-from etos_lib.logging.logger import FORMAT_CONFIG
+import time
+from copy import deepcopy
+from json.decoder import JSONDecodeError
+
+import requests
+from etos_lib import ETOS
+from etos_lib.lib.http import Http
 from jsontas.jsontas import JsonTas
+from packageurl import PackageURL
+from requests.exceptions import HTTPError
+from urllib3.util import Retry
+
+from ..exceptions import IutCheckinFailed, IutCheckoutFailed, IutNotAvailable
+from ..iut import Iut
+
+
+class ExternalProvider:
+    """A generic IUT provider facility for getting IUTs from an external source.
+
+    The ruleset must provide this structure:
+
+    {
+        "status": {
+            "host": "host to status endpoint"
+        },
+        "start": {
+            "host": "host to start endpoint"
+        },
+        "stop": {
+            "host": "host to stop endpoint"
+        }
+    }
+    """
 
-from environment_provider.lib.celery import APP
-from environment_provider.lib.database import ETCDPath
-from environment_provider.lib.registry import ProviderRegistry
-
-from .backend.common import get_suite_id, get_suite_runner_ids
-from .backend.configure import (
-    configure,
-    get_configuration,
-    get_dataset,
-    get_execution_space_provider_id,
-    get_iut_provider_id,
-    get_log_area_provider_id,
-)
-from .backend.environment import (
-    check_environment_status,
-    get_environment_id,
-    get_release_id,
-    get_single_release_id,
-    release_environment,
-    release_full_environment,
-    request_environment,
-)
-from .backend.register import (
-    get_execution_space_provider,
-    get_iut_provider,
-    get_log_area_provider,
-    register,
-)
-from .middleware import JSONTranslator, RequireJSON
-
-
-class Webserver:
-    """Environment provider base endpoint."""
-
-    logger = logging.getLogger(__name__)
-
-    def __init__(self, celery_worker: Celery) -> None:
-        """Init with a db class.
-
-        :param celery_worker: The celery app to use.
-        """
-        self.celery_worker = celery_worker
-
-    def release_by_environment_id(self, response: falcon.Response, environment_id: str) -> None:
-        """Release a single environment.
+    logger = logging.getLogger("External IUTProvider")
 
-        This is a backwards compatibility layer for the ESR so that it can still continue working
-        with just sending in the environment ID.
+    def __init__(self, etos: ETOS, jsontas: JsonTas, ruleset: dict) -> None:
+        """Initialize IUT provider.
 
-        :param response: Response object to edit and return.
-        :param environment_id: Environment to release.
-        """
-        environment = ETCDPath(f"/environment/{environment_id}")
-        testrun_id = environment.join("testrun-id").read()
-        suite_id = environment.join("suite-id").read()
-        if testrun_id is None or suite_id is None:
-            self.logger.warning("Environment for %r already checked in", environment_id)
-            return
-        try:
-            self.release_single(response, environment_id, testrun_id.decode(), suite_id.decode())
-        finally:
-            environment.delete_all()
-
-    def release_single(
-        self, response: falcon.Response, environment_id: str, testrun_id: str, suite_id: str
-    ) -> None:
-        """Release a single environment using suite and test run IDs.
-
-        :param response: Response object to edit and return.
-        :param environment_id: Environment to release.
-        :param testrun_id: ID of the testrun where the environment to release resides.
-        :param suite_id: Test suite started ID where the environment to release resides.
-        """
-        etos = ETOS(
-            "ETOS Environment Provider",
-            os.getenv("HOSTNAME"),
-            "Environment Provider",
-        )
-        jsontas = JsonTas()
-        registry = ProviderRegistry(etos, jsontas, testrun_id)
-        suite = ETCDPath(
-            f"/testrun/{testrun_id}/suite/{suite_id}/subsuite/{environment_id}/suite"
-        ).read()
-        if suite is None:
-            self.logger.warning(
-                f"/testrun/{testrun_id}/suite/{suite_id}/subsuite/{environment_id}/suite"
+        :param etos: ETOS library instance.
+        :param jsontas: JSONTas instance used to evaluate the rulesets.
+        :param ruleset: JSONTas ruleset for handling IUTs.
+        """
+        self.etos = etos
+        self.etos.config.set("iuts", [])
+        self.dataset = jsontas.dataset
+        self.ruleset = ruleset
+        self.id = self.ruleset.get("id")  # pylint:disable=invalid-name
+        self.context = self.etos.config.get("environment_provider_context")
+        self.identifier = self.etos.config.get("SUITE_ID")
+        self.http = Http(
+            retry=Retry(
+                total=None,
+                read=0,
+                connect=10,  # With 1 as backoff_factor, will retry for 1023s
+                status=10,  # With 1 as backoff_factor, will retry for 1023s
+                backoff_factor=1,
+                other=0,
+                allowed_methods=["POST", "GET"],
+                status_forcelist=Retry.RETRY_AFTER_STATUS_CODES,  # 413, 429, 503
             )
-        try:
-            failure = release_environment(etos, jsontas, registry, json.loads(suite))
-        except json.JSONDecodeError as exc:
-            self.logger.error("Failed to decode test suite JSON: %r", suite)
-            failure = exc
-
-        if failure:
-            response.media = {
-                "error": "Failed to release environment",
-                "details": "".join(
-                    traceback.format_exception(failure, value=failure, tb=failure.__traceback__)
-                ),
-                "status": "FAILURE",
-            }
-            return
-
-        response.status = falcon.HTTP_200
-        response.media = {"status": "SUCCESS"}
-
-    def release_full(self, response: falcon.Response, testrun_id: str) -> None:
-        """Release a full test environment using test run ID.
-
-        :param response: Response object to edit and return.
-        :param testrun_id: Testrun to release.
-        """
-        etos = ETOS(
-            "ETOS Environment Provider",
-            os.getenv("HOSTNAME"),
-            "Environment Provider",
         )
-        jsontas = JsonTas()
-
-        task_id = ETCDPath(f"/testrun/{testrun_id}/environment-provider/task-id").read().decode()
-        task_result = None
-        if task_id is not None:
-            task_result = self.celery_worker.AsyncResult(task_id)
-            task_result.forget()
-
-        success, message = release_full_environment(etos, jsontas, testrun_id)
-        if not success:
-            self.logger.error(message)
-            response.media = {
-                "error": "Failed to release environment",
-                "details": message,
-                "status": task_result.status if task_result else "PENDING",
-            }
-            return
-
-        response.status = falcon.HTTP_200
-        response.media = {"status": task_result.status if task_result else "PENDING"}
-
-    def release_by_task_id(self, response: falcon.Response, task_id: str) -> None:
-        """Release a full environment.
-
-        This is a backwards compatibility layer for the ESR to continue to release using the task
-        ID that the environment provider returns when requesting an environment.
-
-        :param response: Response object to edit and return.
-        :param task_id: Task to release.
-        """
-        suite_id = ETCDPath(f"/environment/{task_id}/suite-id").read()
-        if suite_id is None:
-            self.logger.warning("Environment for %r already checked in", task_id)
-            return
-        self.release_full(response, suite_id.decode())
-        ETCDPath(f"/environment/{task_id}/suite-id").delete()
-
-    def on_get(self, request: falcon.Request, response: falcon.Response) -> None:
-        """GET endpoint for environment provider API.
+        self.logger.info("Initialized external IUT provider %r", self.id)
 
-        Get environment task or release environment.
+    @property
+    def identity(self) -> PackageURL:
+        """IUT Identity.
 
-        :param request: Falcon request object.
-        :param response: Falcon response object.
+        :return: IUT identity as PURL object.
         """
-        task_id = get_environment_id(request)
-        release = get_release_id(request)
-        single_release = get_single_release_id(request)
-        if not any([task_id, release, single_release]):
-            raise falcon.HTTPBadRequest(
-                title="Missing parameters",
-                description="'id', 'release' or 'single_release' are required parameters.",
-            )
-        if single_release:
-            self.release_by_environment_id(response, single_release)
-        elif release:
-            self.release_by_task_id(response, release)
-        else:
-            result = check_environment_status(self.celery_worker, task_id)
-            response.status = falcon.HTTP_200
-            response.media = result
-
-    @staticmethod
-    def on_post(request: falcon.Request, response: falcon.Response) -> None:
-        """POST endpoint for environment provider API.
+        return self.dataset.get("identity")
 
-        Create a new environment and return it.
+    def checkin(self, iut: Iut) -> None:
+        """Check in IUTs.
 
-        :param request: Falcon request object.
-        :param response: Falcon response object.
+        :param iut: IUT to checkin.
         """
-        suite_id = get_suite_id(request)
-        suite_runner_ids = get_suite_runner_ids(request)
-        if not all([suite_runner_ids, suite_id]):
-            raise falcon.HTTPBadRequest(
-                title="Missing parameters",
-                description="the 'suite_id' and 'suite_runner_ids' parameters are required.",
-            )
-
-        task_id = request_environment(suite_id, suite_runner_ids)
-
-        # TODO: This shall be removed when API version v1 is used by the ESR and API.
-        ETCDPath(f"/environment/{task_id}/suite-id").write(suite_id)
-        ETCDPath(f"/testrun/{suite_id}/environment-provider/task-id").write(task_id)
+        end = self.etos.config.get("WAIT_FOR_IUT_TIMEOUT")
+        if end is None:
+            end = os.getenv("ENVIRONMENT_PROVIDER_WAIT_FOR_IUT_TIMEOUT")
+        if end is None:
+            end = 3600
+        end = int(end)
 
-        response.status = falcon.HTTP_200
-        response.media = {"result": "success", "data": {"id": task_id}}
-
-
-class Configure:
-    """Configure endpoint for environment provider. Configure an environment for checkout.
-
-    This endpoint should be called before attempting to checkout an environment so that
-    the environment provider is configured to handle it.
-    """
+        if not isinstance(iut, list):
+            self.logger.debug("Check in IUT %r (timeout %ds)", iut, end)
+            iut = [iut]
+        else:
+            self.logger.debug("Check in IUTs %r (timeout %ds)", iut, end)
+        iuts = [iut.as_dict for iut in iut]
 
-    logger = logging.getLogger(__name__)
+        host = self.ruleset.get("stop", {}).get("host")
+        timeout = time.time() + end
+        first_iteration = True
+        while time.time() < timeout:
+            if first_iteration:
+                first_iteration = False
+            else:
+                time.sleep(2)
+            try:
+                response = requests.post(host, json=iuts, headers={"X-ETOS-ID": self.identifier})
+                if response.status_code == requests.codes["no_content"]:
+                    return
+                response = response.json()
+                if response.get("error") is not None:
+                    raise IutCheckinFailed(f"Unable to check in {iuts} ({response.get('error')})")
+            except ConnectionError:
+                self.logger.error("Error connecting to %r", host)
+                continue
+        raise TimeoutError(f"Unable to stop external provider {self.id!r}")
 
-    def on_post(self, request: falcon.Request, response: falcon.Response) -> None:
-        """Verify that all parameters are available and configure the provider registry.
+    def checkin_all(self) -> None:
+        """Check in all IUTs.
 
-        :param request: Falcon request object.
-        :param response: Falcon response object.
+        This method does the same as 'checkin'. It exists for API consistency.
         """
-        etos = ETOS("ETOS Environment Provider", os.getenv("HOSTNAME"), "Environment Provider")
-        jsontas = JsonTas()
-        suite_id = get_suite_id(request)
-        if suite_id is None:
-            self.logger.error("Missing suite_id in request")
-            raise falcon.HTTPBadRequest(
-                title="Bad request", description="missing suite_id in request"
+        self.logger.debug("Checking in all checked out IUTs")
+        self.checkin(self.dataset.get("iuts", []))
+
+    def start(self, minimum_amount: int, maximum_amount: int) -> str:
+        """Send a start request to an external IUT provider.
+
+        :param minimum_amount: The minimum amount of IUTs to request.
+        :param maximum_amount: The maximum amount of IUTs to request.
+        :return: The ID of the external IUT provider request.
+        """
+        self.logger.debug("Start external IUT provider")
+        data = {
+            "minimum_amount": minimum_amount,
+            "maximum_amount": maximum_amount,
+            "identity": self.identity.to_string(),
+            "artifact_id": self.dataset.get("artifact_id"),
+            "artifact_created": self.dataset.get("artifact_created"),
+            "artifact_published": self.dataset.get("artifact_published"),
+            "tercc": self.dataset.get("tercc"),
+            "dataset": self.dataset.get("dataset"),
+            "context": self.dataset.get("context"),
+        }
+        try:
+            response = self.http.post(
+                self.ruleset.get("start", {}).get("host"),
+                json=data,
+                headers={"X-ETOS-ID": self.identifier},
             )
-        registry = ProviderRegistry(etos, jsontas, suite_id)
-        FORMAT_CONFIG.identifier = suite_id
-
-        success, message = configure(
-            registry,
-            get_iut_provider_id(request),
-            get_execution_space_provider_id(request),
-            get_log_area_provider_id(request),
-            get_dataset(request),
+            response.raise_for_status()
+            return response.json().get("id")
+        except (HTTPError, JSONDecodeError) as error:
+            raise Exception(f"Could not start external provider {self.id!r}") from error
+
+    def wait(self, provider_id: str) -> dict:
+        """Wait for external IUT provider to finish its request.
+
+        :param provider_id: The ID of the external IUT provider request.
+        :return: The response from the external IUT provider.
+        """
+        self.logger.debug(
+            "Waiting for external IUT provider (%ds timeout)",
+            self.etos.config.get("WAIT_FOR_IUT_TIMEOUT"),
         )
-        if not success:
-            self.logger.error(message)
-            raise falcon.HTTPBadRequest(title="Bad request", description=message)
-        response.status = falcon.HTTP_200
 
-    def on_get(self, request: falcon.Request, response: falcon.Response) -> None:
-        """Get an already configured environment based on suite ID.
+        host = self.ruleset.get("status", {}).get("host")
+        timeout = time.time() + self.etos.config.get("WAIT_FOR_IUT_TIMEOUT")
 
-        Use only to verify that the environment has been configured properly.
+        response = None
+        while time.time() < timeout:
+            time.sleep(2)
+            try:
+                response = requests.get(
+                    host,
+                    params={"id": provider_id},
+                    headers={"X-ETOS-ID": self.identifier},
+                )
+                self.check_error(response)
+                response = response.json()
+            except ConnectionError:
+                self.logger.error("Error connecting to %r", host)
+                continue
 
-        :param request: Falcon request object.
-        :param response: Falcon response object.
-        """
-        etos = ETOS("ETOS Environment Provider", os.getenv("HOSTNAME"), "Environment Provider")
-        jsontas = JsonTas()
-        suite_id = get_suite_id(request)
-        if suite_id is None:
-            raise falcon.HTTPBadRequest(
-                title="Missing parameters", description="'suite_id' is a required parameter."
+            if response.get("status") == "FAILED":
+                raise IutCheckoutFailed(response.get("description"))
+            if response.get("status") == "DONE":
+                break
+        else:
+            raise TimeoutError(
+                f"Status request timed out after {self.etos.config.get('WAIT_FOR_IUT_TIMEOUT')}s"
             )
+        return response
 
-        registry = ProviderRegistry(etos, jsontas, suite_id)
-
-        FORMAT_CONFIG.identifier = suite_id
-        response.status = falcon.HTTP_200
-        response.media = get_configuration(registry)
-
-
-class Register:  # pylint:disable=too-few-public-methods
-    """Register one or several new providers to the environment provider."""
+    def check_error(self, response: dict) -> None:
+        """Check response for errors and try to translate them to something usable.
 
-    logger = logging.getLogger(__name__)
-
-    def __init__(self) -> None:
-        """Load providers."""
-        self.load_providers_from_disk()
-
-    def providers(self, directory: Path) -> Iterator[dict]:
-        """Read provider json files from a directory.
-
-        :param directory: Directory to read provider json files from.
-        :return: An iterator of the json files.
+        :param response: The response from the external IUT provider.
         """
+        self.logger.debug("Checking response from external IUT provider")
         try:
-            filenames = os.listdir(directory)
-        except FileNotFoundError:
-            return
-        for provider_filename in filenames:
-            if not directory.joinpath(provider_filename).is_file():
-                self.logger.warn("Not a file: %r", provider_filename)
-                continue
-            with directory.joinpath(provider_filename).open() as provider_file:
-                yield json.load(provider_file)
-
-    def load_providers_from_disk(self) -> None:
-        """Register provider files from file system, should environment variables be set."""
-        etos = ETOS("ETOS Environment Provider", os.getenv("HOSTNAME"), "Environment Provider")
-        jsontas = JsonTas()
-        registry = ProviderRegistry(etos, jsontas, None)
-
-        if os.getenv("EXECUTION_SPACE_PROVIDERS"):
-            for provider in self.providers(Path(os.getenv("EXECUTION_SPACE_PROVIDERS"))):
-                register(registry, execution_space_provider=provider)
-        if os.getenv("LOG_AREA_PROVIDERS"):
-            for provider in self.providers(Path(os.getenv("LOG_AREA_PROVIDERS"))):
-                register(registry, log_area_provider=provider)
-        if os.getenv("IUT_PROVIDERS"):
-            for provider in self.providers(Path(os.getenv("IUT_PROVIDERS"))):
-                register(registry, iut_provider=provider)
-
-    def on_post(self, request: falcon.Request, response: falcon.Response) -> None:
-        """Register a new provider.
-
-        :param request: Falcon request object.
-        :param response: Falcon response object.
+            if response.json().get("error") is not None:
+                self.logger.error(response.json().get("error"))
+        except JSONDecodeError:
+            self.logger.error("Could not parse response as JSON")
+
+        if response.status_code == requests.codes["not_found"]:
+            raise IutNotAvailable(f"External provider {self.id!r} did not respond properly")
+        if response.status_code == requests.codes["bad_request"]:
+            raise RuntimeError(f"IUT provider for {self.id!r} is not properly configured")
+
+        # This should work, no other errors found.
+        # If this does not work, propagate JSONDecodeError up the stack.
+        self.logger.debug("Status for response %r", response.json().get("status"))
+
+    def build_iuts(self, response: dict) -> list[Iut]:
+        """Build IUT objects from external IUT provider response.
+
+        :param response: The response from the external IUT provider.
+        :return: A list of IUTs.
+        """
+        iuts = []
+        for iut in response.get("iuts", []):
+            if iut.get("identity") is None:
+                iut["identity"] = self.identity
+            else:
+                iut["identity"] = PackageURL.from_string(iut.get("identity"))
+            iuts.append(Iut(provider_id=self.id, **iut))
+        return iuts
+
+    def request_and_wait_for_iuts(
+        self, minimum_amount: int = 0, maximum_amount: int = 100
+    ) -> list[Iut]:
+        """Wait for IUTs from an external IUT provider.
+
+        :raises: IutNotAvailable: If there are no available IUTs.
+
+        :param minimum_amount: Minimum amount of IUTs to checkout.
+        :param maximum_amount: Maximum amount of IUTs to checkout.
+        :return: List of checked out IUTs.
         """
-        etos = ETOS("ETOS Environment Provider", os.getenv("HOSTNAME"), "Environment Provider")
-        jsontas = JsonTas()
-        registry = ProviderRegistry(etos, jsontas, None)
-        registered = register(
-            registry,
-            iut_provider=get_iut_provider(request),
-            log_area_provider=get_log_area_provider(request),
-            execution_space_provider=get_execution_space_provider(request),
-        )
-        if registered is False:
-            raise falcon.HTTPBadRequest(
-                title="Missing parameters",
-                description="At least one of 'iut_provider', 'log_area_provider' "
-                "& 'execution_space_provider' is a required parameter.",
+        try:
+            provider_id = self.start(minimum_amount, maximum_amount)
+            response = self.wait(provider_id)
+            iuts = self.build_iuts(response)
+            if len(iuts) < minimum_amount:
+                raise IutNotAvailable(self.identity.to_string())
+            if len(iuts) > maximum_amount:
+                self.logger.warning(
+                    "Too many IUTs from external IUT provider %r. (Expected: %d, Got %d)",
+                    self.id,
+                    maximum_amount,
+                    len(iuts),
+                )
+                extra = iuts[maximum_amount:]
+                iuts = iuts[:maximum_amount]
+                for iut in extra:
+                    self.checkin(iut)
+            self.dataset.add("iuts", deepcopy(iuts))
+        except:  # pylint:disable=bare-except
+            self.checkin_all()
+            raise
+        return iuts
+
+    def wait_for_and_checkout_iuts(
+        self, minimum_amount: int = 0, maximum_amount: int = 100
+    ) -> list[Iut]:
+        """Wait for IUTs from an external IUT provider.
+
+        See: `request_and_wait_for_iuts`
+
+        :raises: IutNotAvailable: If there are no available IUTs.
+
+        :param minimum_amount: Minimum amount of IUTs to checkout.
+        :param maximum_amount: Maximum amount of IUTs to checkout.
+        :return: List of checked out IUTs.
+        """
+        error = None
+        triggered = None
+        try:
+            triggered = self.etos.events.send_activity_triggered(
+                f"Checkout IUTs from {self.id}",
+                {"CONTEXT": self.context},
+                executionType="AUTOMATED",
+                categories=["EnvironmentProvider", "IUTProvider", "External"],
+                triggers=[
+                    {
+                        "type": "OTHER",
+                        "description": f"Checking out IUTs",
+                    }
+                ],
             )
-        response.status = falcon.HTTP_204
-
-
-FALCON_APP = falcon.App(middleware=[RequireJSON(), JSONTranslator()])
-WEBSERVER = Webserver(APP)
-CONFIGURE = Configure()
-REGISTER = Register()
-FALCON_APP.add_route("/", WEBSERVER)
-FALCON_APP.add_route("/configure", CONFIGURE)
-FALCON_APP.add_route("/register", REGISTER)
+            self.etos.events.send_activity_started(triggered)
+            return self.request_and_wait_for_iuts(minimum_amount, maximum_amount)
+        except Exception as exception:
+            error = exception
+            raise
+        finally:
+            if error is None:
+                outcome = {"conclusion": "SUCCESSFUL"}
+            else:
+                outcome = {"conclusion": "UNSUCCESSFUL", "description": str(error)}
+            if triggered is not None:
+                self.etos.events.send_activity_finished(triggered, outcome)
```

### Comparing `etos_environment_provider-3.2.2/src/etos_environment_provider.egg-info/PKG-INFO` & `etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_environment_provider
-Version: 3.2.2
+Version: 4.0.0
 Summary: Environment provider for ETOS.
 Home-page: https://github.com/eiffel-community/etos-environment-provider
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
@@ -17,15 +17,14 @@
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: eventlet~=0.33
 Requires-Dist: celery~=5.3
 Requires-Dist: cryptography<43.0.0,>=42.0.4
 Requires-Dist: gevent~=23.7
 Requires-Dist: gunicorn~=19.9
-Requires-Dist: falcon~=3.1
 Requires-Dist: jsontas~=1.3
 Requires-Dist: packageurl-python~=0.11
 Requires-Dist: etcd3gw~=2.3
 Requires-Dist: etos_lib==4.0.0
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `etos_environment_provider-3.2.2/src/etos_environment_provider.egg-info/SOURCES.txt` & `etos_environment_provider-4.0.0/src/etos_environment_provider.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 manifests/base/kustomization.yaml
 manifests/base/api/deployment.yaml
 manifests/base/api/service-account.yaml
 manifests/base/api/service.yaml
 manifests/base/worker/deployment.yaml
 manifests/base/worker/service-account.yaml
 src/environment_provider/__init__.py
+src/environment_provider/environment.py
 src/environment_provider/environment_provider.py
 src/environment_provider/lib/__init__.py
 src/environment_provider/lib/celery.py
 src/environment_provider/lib/config.py
 src/environment_provider/lib/database.py
 src/environment_provider/lib/encrypt.py
 src/environment_provider/lib/graphql.py
@@ -41,25 +42,14 @@
 src/environment_provider/lib/json_dumps.py
 src/environment_provider/lib/log_area.py
 src/environment_provider/lib/registry.py
 src/environment_provider/lib/test_suite.py
 src/environment_provider/lib/uuid_generate.py
 src/environment_provider/splitter/__init__.py
 src/environment_provider/splitter/split.py
-src/environment_provider_api/.gitignore
-src/environment_provider_api/__init__.py
-src/environment_provider_api/webserver.py
-src/environment_provider_api/backend/__init__.py
-src/environment_provider_api/backend/common.py
-src/environment_provider_api/backend/configure.py
-src/environment_provider_api/backend/environment.py
-src/environment_provider_api/backend/register.py
-src/environment_provider_api/middleware/__init__.py
-src/environment_provider_api/middleware/json_translator.py
-src/environment_provider_api/middleware/require_json.py
 src/etos_environment_provider.egg-info/PKG-INFO
 src/etos_environment_provider.egg-info/SOURCES.txt
 src/etos_environment_provider.egg-info/dependency_links.txt
 src/etos_environment_provider.egg-info/not-zip-safe
 src/etos_environment_provider.egg-info/requires.txt
 src/etos_environment_provider.egg-info/top_level.txt
 src/execution_space_provider/__init__.py
@@ -100,28 +90,18 @@
 src/log_area_provider/utilities/external_provider.py
 src/log_area_provider/utilities/jsontas_provider.py
 src/log_area_provider/utilities/list.py
 tests/__init__.py
 tests/conftest.py
 tests/tercc.py
 tests/test_environment_provider.py
-tests/test_webserver_configure.py
-tests/test_webserver_environment.py
-tests/test_webserver_register.py
-tests/backend/__init__.py
-tests/backend/test_common.py
-tests/backend/test_configure.py
-tests/backend/test_environment.py
-tests/backend/test_register.py
 tests/external_execution_space/__init__.py
 tests/external_execution_space/test_external_execution_space.py
 tests/external_iut/__init__.py
 tests/external_iut/test_external_iut.py
 tests/external_log_area/__init__.py
 tests/external_log_area/test_external_log_area.py
 tests/library/__init__.py
-tests/library/fake_celery.py
 tests/library/fake_database.py
-tests/library/fake_request.py
 tests/library/fake_server.py
 tests/library/graphql_handler.py
 tests/splitter/test_splitter.py
```

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/__init__.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/exceptions.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/execution_space.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/execution_space.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/execution_space_provider.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/execution_space_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/schemas/external_schema.json` & `etos_environment_provider-4.0.0/src/execution_space_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.0.0/src/execution_space_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/utilities/__init__.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/utilities/checkin.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/utilities/checkout.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/utilities/external_provider.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/external_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/utilities/instructions.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/instructions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/execution_space_provider/utilities/list.py` & `etos_environment_provider-4.0.0/src/execution_space_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/__init__.py` & `etos_environment_provider-4.0.0/src/log_area_provider/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,31 +9,31 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ETOS IUT provider module."""
+"""ETOS log area provider module."""
 import pathlib
 
-from .iut_provider import IutProvider
+from .log_area_provider import LogAreaProvider
 
-__all__ = ["IutProvider", "iut_provider_schema"]
+__all__ = ["LogAreaProvider", "log_area_provider_schema"]
 
-IUT_PROVIDER_SCHEMA = (
+LOG_AREA_PROVIDER_SCHEMA = (
     pathlib.Path(__file__).parent.resolve().joinpath("./schemas/jsontas_schema.json")
 )
-EXTERNAL_IUT_PROVIDER_SCHEMA = (
+EXTERNAL_LOG_AREA_PROVIDER_SCHEMA = (
     pathlib.Path(__file__).parent.resolve().joinpath("./schemas/external_schema.json")
 )
 
 
-def iut_provider_schema(ruleset: dict) -> pathlib.Path:
-    """Get IUT provider schema for json validation.
+def log_area_provider_schema(ruleset: dict) -> pathlib.Path:
+    """Get log area provider schema for json validation.
 
-    :param ruleset: Ruleset to get an IUT provider schema for.
+    :param ruleset: Ruleset to get a log area provider schema for.
     """
-    if ruleset.get("iut", {}).get("type", "jsontas") == "external":
-        return EXTERNAL_IUT_PROVIDER_SCHEMA
+    if ruleset.get("log", {}).get("type", "jsontas") == "external":
+        return EXTERNAL_LOG_AREA_PROVIDER_SCHEMA
     else:
-        return IUT_PROVIDER_SCHEMA
+        return LOG_AREA_PROVIDER_SCHEMA
```

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/exceptions.py` & `etos_environment_provider-4.0.0/src/iut_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/iut.py` & `etos_environment_provider-4.0.0/src/iut_provider/iut.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/iut_provider.py` & `etos_environment_provider-4.0.0/src/iut_provider/iut_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/schemas/external_schema.json` & `etos_environment_provider-4.0.0/src/iut_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.0.0/src/iut_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/utilities/__init__.py` & `etos_environment_provider-4.0.0/tests/external_execution_space/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Utilities for the IUT provider."""
+"""External execution space tests."""
```

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/utilities/checkin.py` & `etos_environment_provider-4.0.0/src/iut_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/utilities/checkout.py` & `etos_environment_provider-4.0.0/src/iut_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/utilities/external_provider.py` & `etos_environment_provider-4.0.0/src/log_area_provider/utilities/external_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""IUT provider for external providers."""
+"""External log area provider."""
 import logging
 import os
 import time
 from copy import deepcopy
 from json.decoder import JSONDecodeError
 
 import requests
 from etos_lib import ETOS
 from etos_lib.lib.http import Http
 from jsontas.jsontas import JsonTas
 from packageurl import PackageURL
 from requests.exceptions import HTTPError
 from urllib3.util import Retry
 
-from ..exceptions import IutCheckinFailed, IutCheckoutFailed, IutNotAvailable
-from ..iut import Iut
+from ..exceptions import LogAreaCheckinFailed, LogAreaCheckoutFailed, LogAreaNotAvailable
+from ..log_area import LogArea
 
 
 class ExternalProvider:
-    """A generic IUT provider facility for getting IUTs from an external source.
+    """A log area provider facility for getting log areas from an external source.
 
     The ruleset must provide this structure:
 
     {
         "status": {
             "host": "host to status endpoint"
         },
@@ -46,25 +46,25 @@
         },
         "stop": {
             "host": "host to stop endpoint"
         }
     }
     """
 
-    logger = logging.getLogger("External IUTProvider")
+    logger = logging.getLogger("External LogAreaProvider")
 
     def __init__(self, etos: ETOS, jsontas: JsonTas, ruleset: dict) -> None:
-        """Initialize IUT provider.
+        """Initialize log area provider.
 
         :param etos: ETOS library instance.
         :param jsontas: JSONTas instance used to evaluate the rulesets.
-        :param ruleset: JSONTas ruleset for handling IUTs.
+        :param ruleset: JSONTas ruleset for handling log areas.
         """
         self.etos = etos
-        self.etos.config.set("iuts", [])
+        self.etos.config.set("logs", [])
         self.dataset = jsontas.dataset
         self.ruleset = ruleset
         self.id = self.ruleset.get("id")  # pylint:disable=invalid-name
         self.context = self.etos.config.get("environment_provider_context")
         self.identifier = self.etos.config.get("SUITE_ID")
         self.http = Http(
             retry=Retry(
@@ -74,79 +74,83 @@
                 status=10,  # With 1 as backoff_factor, will retry for 1023s
                 backoff_factor=1,
                 other=0,
                 allowed_methods=["POST", "GET"],
                 status_forcelist=Retry.RETRY_AFTER_STATUS_CODES,  # 413, 429, 503
             )
         )
-        self.logger.info("Initialized external IUT provider %r", self.id)
+        self.logger.info("Initialized external log area provider %r", self.id)
 
     @property
     def identity(self) -> PackageURL:
-        """IUT Identity.
+        """IUT identity.
 
         :return: IUT identity as PURL object.
         """
         return self.dataset.get("identity")
 
-    def checkin(self, iut: Iut) -> None:
-        """Check in IUTs.
+    def checkin(self, log_area: LogArea) -> None:
+        """Check in log areas.
 
-        :param iut: IUT to checkin.
+        :param log_area: Log area to check in.
         """
-        end = self.etos.config.get("WAIT_FOR_IUT_TIMEOUT")
+        end = self.etos.config.get("WAIT_FOR_LOG_AREA_TIMEOUT")
         if end is None:
-            end = os.getenv("ENVIRONMENT_PROVIDER_WAIT_FOR_IUT_TIMEOUT")
+            end = os.getenv("ENVIRONMENT_PROVIDER_WAIT_FOR_LOG_AREA_TIMEOUT")
         if end is None:
             end = 3600
         end = int(end)
 
-        if not isinstance(iut, list):
-            self.logger.debug("Check in IUT %r (timeout %ds)", iut, end)
-            iut = [iut]
+        if not isinstance(log_area, list):
+            self.logger.debug("Check in log area %r (timeout %ds)", log_area, end)
+            log_area = [log_area]
         else:
-            self.logger.debug("Check in IUTs %r (timeout %ds)", iut, end)
-        iuts = [iut.as_dict for iut in iut]
+            self.logger.debug("Check in log areas %r (timeout %ds)", log_area, end)
+        log_areas = [log_area.as_dict for log_area in log_area]
 
         host = self.ruleset.get("stop", {}).get("host")
         timeout = time.time() + end
         first_iteration = True
         while time.time() < timeout:
             if first_iteration:
                 first_iteration = False
             else:
                 time.sleep(2)
             try:
-                response = requests.post(host, json=iuts, headers={"X-ETOS-ID": self.identifier})
+                response = requests.post(
+                    host, json=log_areas, headers={"X-ETOS-ID": self.identifier}
+                )
                 if response.status_code == requests.codes["no_content"]:
                     return
                 response = response.json()
                 if response.get("error") is not None:
-                    raise IutCheckinFailed(f"Unable to check in {iuts} ({response.get('error')})")
+                    raise LogAreaCheckinFailed(
+                        f"Unable to check in {log_areas} ({response.get('error')})"
+                    )
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
         raise TimeoutError(f"Unable to stop external provider {self.id!r}")
 
     def checkin_all(self) -> None:
-        """Check in all IUTs.
+        """Check in all log areas.
 
         This method does the same as 'checkin'. It exists for API consistency.
         """
-        self.logger.debug("Checking in all checked out IUTs")
-        self.checkin(self.dataset.get("iuts", []))
+        self.logger.debug("Checking in all checked out log areas")
+        self.checkin(self.dataset.get("logs", []))
 
     def start(self, minimum_amount: int, maximum_amount: int) -> str:
-        """Send a start request to an external IUT provider.
+        """Send a start request to an external log area provider.
 
-        :param minimum_amount: The minimum amount of IUTs to request.
-        :param maximum_amount: The maximum amount of IUTs to request.
-        :return: The ID of the external IUT provider request.
+        :param minimum_amount: Minimum amount of log areas to request.
+        :param maximum_amount: Maximum amount of log areas to request.
+        :return: The ID of the external log area provider request.
         """
-        self.logger.debug("Start external IUT provider")
+        self.logger.debug("Start external log area provider")
         data = {
             "minimum_amount": minimum_amount,
             "maximum_amount": maximum_amount,
             "identity": self.identity.to_string(),
             "artifact_id": self.dataset.get("artifact_id"),
             "artifact_created": self.dataset.get("artifact_created"),
             "artifact_published": self.dataset.get("artifact_published"),
@@ -162,152 +166,155 @@
             )
             response.raise_for_status()
             return response.json().get("id")
         except (HTTPError, JSONDecodeError) as error:
             raise Exception(f"Could not start external provider {self.id!r}") from error
 
     def wait(self, provider_id: str) -> dict:
-        """Wait for external IUT provider to finish its request.
+        """Wait for external log area provider to finish its request.
 
-        :param provider_id: The ID of the external IUT provider request.
-        :return: The response from the external IUT provider.
+        :param provider_id: The ID of the external log area provider request.
+        :type provider_id: str
+        :return: The response from the external log area provider.
+        :rtype: dict
         """
         self.logger.debug(
-            "Waiting for external IUT provider (%ds timeout)",
-            self.etos.config.get("WAIT_FOR_IUT_TIMEOUT"),
+            "Waiting for external log area provider (%ds timeout)",
+            self.etos.config.get("WAIT_FOR_LOG_AREA_TIMEOUT"),
         )
 
         host = self.ruleset.get("status", {}).get("host")
-        timeout = time.time() + self.etos.config.get("WAIT_FOR_IUT_TIMEOUT")
+        timeout = time.time() + self.etos.config.get("WAIT_FOR_LOG_AREA_TIMEOUT")
 
         response = None
+        first_iteration = True
         while time.time() < timeout:
-            time.sleep(2)
+            if first_iteration:
+                first_iteration = False
+            else:
+                time.sleep(2)
             try:
                 response = requests.get(
                     host,
                     params={"id": provider_id},
                     headers={"X-ETOS-ID": self.identifier},
                 )
                 self.check_error(response)
                 response = response.json()
             except ConnectionError:
                 self.logger.error("Error connecting to %r", host)
                 continue
 
             if response.get("status") == "FAILED":
-                raise IutCheckoutFailed(response.get("description"))
+                raise LogAreaCheckoutFailed(response.get("description"))
             if response.get("status") == "DONE":
                 break
         else:
             raise TimeoutError(
-                f"Status request timed out after {self.etos.config.get('WAIT_FOR_IUT_TIMEOUT')}s"
+                "Status request timed out after "
+                f"{self.etos.config.get('WAIT_FOR_LOG_AREA_TIMEOUT')}s"
             )
         return response
 
     def check_error(self, response: dict) -> None:
         """Check response for errors and try to translate them to something usable.
 
-        :param response: The response from the external IUT provider.
+        :param response: The response from the external log area provider.
         """
-        self.logger.debug("Checking response from external IUT provider")
+        self.logger.debug("Checking response from external log area provider")
         try:
             if response.json().get("error") is not None:
                 self.logger.error(response.json().get("error"))
         except JSONDecodeError:
             self.logger.error("Could not parse response as JSON")
 
         if response.status_code == requests.codes["not_found"]:
-            raise IutNotAvailable(f"External provider {self.id!r} did not respond properly")
+            raise LogAreaNotAvailable(f"External provider {self.id!r} did not respond properly")
         if response.status_code == requests.codes["bad_request"]:
-            raise RuntimeError(f"IUT provider for {self.id!r} is not properly configured")
+            raise RuntimeError(f"Log area provider for {self.id!r} is not properly configured")
 
         # This should work, no other errors found.
         # If this does not work, propagate JSONDecodeError up the stack.
         self.logger.debug("Status for response %r", response.json().get("status"))
 
-    def build_iuts(self, response: dict) -> list[Iut]:
-        """Build IUT objects from external IUT provider response.
+    def build_log_areas(self, response: dict) -> list[LogArea]:
+        """Build log area objects from external log area provider response.
 
-        :param response: The response from the external IUT provider.
-        :return: A list of IUTs.
+        :param response: The response from the external log area provider.
+        :return: A list of log areas.
         """
-        iuts = []
-        for iut in response.get("iuts", []):
-            if iut.get("identity") is None:
-                iut["identity"] = self.identity
-            else:
-                iut["identity"] = PackageURL.from_string(iut.get("identity"))
-            iuts.append(Iut(provider_id=self.id, **iut))
-        return iuts
+        return [
+            LogArea(provider_id=self.id, **log_area) for log_area in response.get("log_areas", [])
+        ]
 
-    def request_and_wait_for_iuts(
+    def request_and_wait_for_log_areas(
         self, minimum_amount: int = 0, maximum_amount: int = 100
-    ) -> list[Iut]:
-        """Wait for IUTs from an external IUT provider.
+    ) -> list[LogArea]:
+        """Wait for log areas from an external log area provider.
 
-        :raises: IutNotAvailable: If there are no available IUTs.
+        :raises: LogAreaNotAvailable: If there are not available log areas after timeout.
 
-        :param minimum_amount: Minimum amount of IUTs to checkout.
-        :param maximum_amount: Maximum amount of IUTs to checkout.
-        :return: List of checked out IUTs.
+        :param minimum_amount: Minimum amount of log areas to checkout.
+        :param maximum_amount: Maximum amount of log areas to checkout.
+        :return: List of checked out log areas.
         """
         try:
             provider_id = self.start(minimum_amount, maximum_amount)
             response = self.wait(provider_id)
-            iuts = self.build_iuts(response)
-            if len(iuts) < minimum_amount:
-                raise IutNotAvailable(self.identity.to_string())
-            if len(iuts) > maximum_amount:
+            log_areas = self.build_log_areas(response)
+            if len(log_areas) < minimum_amount:
+                raise LogAreaNotAvailable(self.id)
+            if len(log_areas) > maximum_amount:
                 self.logger.warning(
-                    "Too many IUTs from external IUT provider %r. (Expected: %d, Got %d)",
+                    "Too many log areas from external log area provider "
+                    "%r. (Expected: %d, Got %d)",
                     self.id,
                     maximum_amount,
-                    len(iuts),
+                    len(log_areas),
                 )
-                extra = iuts[maximum_amount:]
-                iuts = iuts[:maximum_amount]
-                for iut in extra:
-                    self.checkin(iut)
-            self.dataset.add("iuts", deepcopy(iuts))
+                extra = log_areas[maximum_amount:]
+                log_areas = log_areas[:maximum_amount]
+                for log_area in extra:
+                    self.checkin(log_area)
+            self.dataset.add("logs", deepcopy(log_areas))
         except:  # pylint:disable=bare-except
             self.checkin_all()
             raise
-        return iuts
+        return log_areas
 
-    def wait_for_and_checkout_iuts(
+    def wait_for_and_checkout_log_areas(
         self, minimum_amount: int = 0, maximum_amount: int = 100
-    ) -> list[Iut]:
-        """Wait for IUTs from an external IUT provider.
+    ) -> list[LogArea]:
+        """Wait for log areas from an external log area provider.
 
-        See: `request_and_wait_for_iuts`
+        See: `request_and_wait_for_log_areas`
 
-        :raises: IutNotAvailable: If there are no available IUTs.
+        :raises: LogAreaNotAvailable: If there are not available log areas after timeout.
 
-        :param minimum_amount: Minimum amount of IUTs to checkout.
-        :param maximum_amount: Maximum amount of IUTs to checkout.
-        :return: List of checked out IUTs.
+        :param minimum_amount: Minimum amount of log areas to checkout.
+        :param maximum_amount: Maximum amount of log areas to checkout.
+        :return: List of checked out log areas.
         """
         error = None
         triggered = None
         try:
             triggered = self.etos.events.send_activity_triggered(
-                f"Checkout IUTs from {self.id}",
+                f"Checkout log areas from {self.id}",
                 {"CONTEXT": self.context},
                 executionType="AUTOMATED",
-                categories=["EnvironmentProvider", "IUTProvider", "External"],
+                categories=["EnvironmentProvider", "LogAreaProvider", "External"],
                 triggers=[
                     {
                         "type": "OTHER",
-                        "description": f"Checking out IUTs",
+                        "description": f"Checking out log areas",
                     }
                 ],
             )
             self.etos.events.send_activity_started(triggered)
-            return self.request_and_wait_for_iuts(minimum_amount, maximum_amount)
+            return self.request_and_wait_for_log_areas(minimum_amount, maximum_amount)
         except Exception as exception:
             error = exception
             raise
         finally:
             if error is None:
                 outcome = {"conclusion": "SUCCESSFUL"}
             else:
```

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.0.0/src/iut_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/utilities/list.py` & `etos_environment_provider-4.0.0/src/iut_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/iut_provider/utilities/prepare.py` & `etos_environment_provider-4.0.0/src/iut_provider/utilities/prepare.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/exceptions.py` & `etos_environment_provider-4.0.0/src/log_area_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/log_area.py` & `etos_environment_provider-4.0.0/src/log_area_provider/log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/log_area_provider.py` & `etos_environment_provider-4.0.0/src/log_area_provider/log_area_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/schemas/external_schema.json` & `etos_environment_provider-4.0.0/src/log_area_provider/schemas/external_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/schemas/jsontas_schema.json` & `etos_environment_provider-4.0.0/src/log_area_provider/schemas/jsontas_schema.json`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/utilities/__init__.py` & `etos_environment_provider-4.0.0/src/log_area_provider/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/utilities/checkin.py` & `etos_environment_provider-4.0.0/src/log_area_provider/utilities/checkin.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/utilities/checkout.py` & `etos_environment_provider-4.0.0/src/log_area_provider/utilities/checkout.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/utilities/jsontas_provider.py` & `etos_environment_provider-4.0.0/src/log_area_provider/utilities/jsontas_provider.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/src/log_area_provider/utilities/list.py` & `etos_environment_provider-4.0.0/src/log_area_provider/utilities/list.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/tests/__init__.py` & `etos_environment_provider-4.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/tests/backend/__init__.py` & `etos_environment_provider-4.0.0/tests/external_iut/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Tests for the backend services."""
+"""External IUT tests."""
```

### Comparing `etos_environment_provider-3.2.2/tests/external_execution_space/__init__.py` & `etos_environment_provider-4.0.0/tests/library/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""External execution space tests."""
+"""Library helpers for testing."""
```

### Comparing `etos_environment_provider-3.2.2/tests/external_execution_space/test_external_execution_space.py` & `etos_environment_provider-4.0.0/tests/external_execution_space/test_external_execution_space.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/tests/external_iut/test_external_iut.py` & `etos_environment_provider-4.0.0/tests/external_iut/test_external_iut.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/tests/external_log_area/test_external_log_area.py` & `etos_environment_provider-4.0.0/tests/external_log_area/test_external_log_area.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/tests/library/fake_database.py` & `etos_environment_provider-4.0.0/tests/library/fake_database.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/tests/library/fake_server.py` & `etos_environment_provider-4.0.0/tests/library/fake_server.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/tests/library/graphql_handler.py` & `etos_environment_provider-4.0.0/tests/library/graphql_handler.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/tests/tercc.py` & `etos_environment_provider-4.0.0/tests/tercc.py`

 * *Files identical despite different names*

### Comparing `etos_environment_provider-3.2.2/tests/test_environment_provider.py` & `etos_environment_provider-4.0.0/tests/test_environment_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,18 +20,15 @@
 import os
 import unittest
 
 from etos_lib.lib.config import Config
 from etos_lib.lib.debug import Debug
 
 from environment_provider.environment_provider import get_environment
-from environment_provider_api.webserver import Webserver
-from tests.library.fake_celery import FakeCelery
 from tests.library.fake_database import FakeDatabase
-from tests.library.fake_request import FakeRequest, FakeResponse
 from tests.library.fake_server import FakeServer
 from tests.library.graphql_handler import GraphQLHandler
 
 from .tercc import TERCC, TERCC_PERMUTATION, TERCC_SUB_SUITES
 
 IUT_PROVIDER = {
     "iut": {
@@ -156,15 +153,14 @@
         self.logger.info("STEP: Start up a fake server.")
         with FakeServer(None, None, handler) as server:
             database.put(
                 f"/testrun/{suite_id}/provider/dataset",
                 json.dumps({"host": server.host}),
             )
             os.environ["ETOS_GRAPHQL_SERVER"] = server.host
-            os.environ["ETOS_ENVIRONMENT_PROVIDER"] = server.host
             os.environ["ETOS_API"] = server.host
 
             self.logger.info("STEP: Run the environment provider.")
             result = get_environment(suite_id, suite_runner_ids)
             print(result)
         self.assertIsNone(result.get("error"))
 
@@ -205,15 +201,14 @@
         self.logger.info("STEP: Start up a fake server.")
         with FakeServer(None, None, handler) as server:
             database.put(
                 f"/testrun/{suite_id}/provider/dataset",
                 json.dumps({"host": server.host}),
             )
             os.environ["ETOS_GRAPHQL_SERVER"] = server.host
-            os.environ["ETOS_ENVIRONMENT_PROVIDER"] = server.host
             os.environ["ETOS_API"] = server.host
 
             self.logger.info("STEP: Run the environment provider.")
             result = get_environment(suite_id, suite_runner_ids)
             print(result)
         self.assertIsNone(result.get("error"))
 
@@ -257,15 +252,14 @@
         self.logger.info("STEP: Start up a fake server.")
         with FakeServer(None, None, handler) as server:
             database.put(
                 f"/testrun/{suite_id}/provider/dataset",
                 json.dumps({"host": server.host}),
             )
             os.environ["ETOS_GRAPHQL_SERVER"] = server.host
-            os.environ["ETOS_ENVIRONMENT_PROVIDER"] = server.host
             os.environ["ETOS_API"] = server.host
 
             self.logger.info("STEP: Run the environment provider.")
             result = get_environment(suite_id, suite_runner_ids)
         self.assertIsNone(result.get("error"))
 
         self.logger.info("STEP: Verify that two environments were sent.")
@@ -307,107 +301,20 @@
         self.logger.info("STEP: Start up a fake server.")
         with FakeServer(None, None, handler) as server:
             database.put(
                 f"/testrun/{suite_id}/provider/dataset",
                 json.dumps({"host": server.host}),
             )
             os.environ["ETOS_GRAPHQL_SERVER"] = server.host
-            os.environ["ETOS_ENVIRONMENT_PROVIDER"] = server.host
             os.environ["ETOS_API"] = server.host
 
             self.logger.info("STEP: Run the environment provider.")
             result = get_environment(suite_id, suite_runner_ids)
             print(result)
         self.assertIsNone(result.get("error"))
 
         self.logger.info("STEP: Verify that two environments were sent.")
         environments = []
         for event in Debug().events_published:
             if event.meta.type == "EiffelEnvironmentDefinedEvent":
                 environments.append(event)
         self.assertEqual(len(environments), 2)
-
-    def test_release_environment(self):  # pylint:disable=too-many-locals
-        """Test that it is possible to release an environment.
-
-        Approval criteria:
-            - It shall be possible to release an environment.
-
-        Test steps:
-            1. Start up a fake server.
-            2. Run the environment provider.
-            3. Verify that two environments were sent.
-            4. Store the environments in celery task.
-            5. Send a release request for that environment.
-            6. Verify that the environment was released.
-        """
-        tercc = TERCC_SUB_SUITES
-        database = FakeDatabase()
-        Config().set("database", database)
-
-        suite_id = tercc["meta"]["id"]
-        suite_runner_ids = ["14ffc8d7-572a-4f2f-9382-923de2bcf50a"]
-        task_id = "d9689ea5-837b-48c1-87b1-3de122b3f2fe"
-        database.put(f"/environment/{task_id}/suite-id", suite_id)
-        database.put(
-            f"/environment/provider/iut/{IUT_PROVIDER['iut']['id']}", json.dumps(IUT_PROVIDER)
-        )
-        database.put(
-            f"/environment/provider/log-area/{LOG_AREA_PROVIDER['log']['id']}",
-            json.dumps(LOG_AREA_PROVIDER),
-        )
-        database.put(
-            (
-                "/environment/provider/execution-space/"
-                f"{EXECUTION_SPACE_PROVIDER['execution_space']['id']}"
-            ),
-            json.dumps(EXECUTION_SPACE_PROVIDER),
-        )
-        database.put(f"/testrun/{suite_id}/environment-provider/task-id", task_id)
-
-        database.put(f"/testrun/{suite_id}/tercc", json.dumps(tercc))
-        database.put(f"/testrun/{suite_id}/provider/iut", json.dumps(IUT_PROVIDER))
-        database.put(f"/testrun/{suite_id}/provider/log-area", json.dumps(LOG_AREA_PROVIDER))
-        database.put(
-            f"/testrun/{suite_id}/provider/execution-space", json.dumps(EXECUTION_SPACE_PROVIDER)
-        )
-
-        handler = functools.partial(GraphQLHandler, tercc)
-
-        self.logger.info("STEP: Start up a fake server.")
-        with FakeServer(None, None, handler) as server:
-            database.put(
-                f"/testrun/{suite_id}/provider/dataset",
-                json.dumps({"host": server.host}),
-            )
-            os.environ["ETOS_GRAPHQL_SERVER"] = server.host
-            os.environ["ETOS_ENVIRONMENT_PROVIDER"] = server.host
-            os.environ["ETOS_API"] = server.host
-
-            self.logger.info("STEP: Run the environment provider.")
-            result = get_environment(suite_id, suite_runner_ids)
-            print(result)
-        self.assertIsNone(result.get("error"))
-
-        self.logger.info("STEP: Verify that two environments were sent.")
-        environments = []
-        for event in Debug().events_published:
-            if event.meta.type == "EiffelEnvironmentDefinedEvent":
-                environments.append(event)
-        self.assertEqual(len(environments), 2)
-
-        request = FakeRequest()
-        request.fake_params = {"release": task_id}
-        response = FakeResponse()
-
-        self.logger.info("STEP: Store the environments in celery task.")
-        test_status = "SUCCESS"
-        worker = FakeCelery(task_id, test_status, result)
-
-        self.logger.info("STEP: Send a release request for that environment.")
-        environment = Webserver(worker)
-        environment.on_get(request, response)
-
-        self.logger.info("STEP: Verify that the environment was released.")
-        self.assertDictEqual(response.media, {"status": test_status})
-        self.assertIsNone(worker.results.get(task_id))
-        self.assertListEqual(database.get_prefix("/testrun"), [])
```

### Comparing `etos_environment_provider-3.2.2/tox.ini` & `etos_environment_provider-4.0.0/tox.ini`

 * *Files identical despite different names*

