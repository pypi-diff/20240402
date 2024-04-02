# Comparing `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.8.tar.gz` & `tmp/odoo13-addon-photovoltaic_api-13.0.1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.8.tar", last modified: Thu Sep 28 07:27:05 2023, max compression
+gzip compressed data, was "odoo13-addon-photovoltaic_api-13.0.1.1.9.tar", last modified: Wed Dec 13 18:14:16 2023, max compression
```

## Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8.tar` & `odoo13-addon-photovoltaic_api-13.0.1.1.9.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.467578 odoo13-addon-photovoltaic_api-13.0.1.1.8/
--rw-r--r--   0 root         (0) root         (0)      448 2023-09-28 07:27:05.466578 odoo13-addon-photovoltaic_api-13.0.1.1.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.458578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.458578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.460578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.460578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/controllers/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/controllers/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.460578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/data/
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/data/data.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.461578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/models/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.462578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/contract.py
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/info.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1353 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
--rw-rw-rw-   0 root         (0) root         (0)     1991 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.463578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/security/
--rw-rw-rw-   0 root         (0) root         (0)     2578 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/security/ir.model.access.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.464578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4683 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/account.py
--rw-rw-rw-   0 root         (0) root         (0)     4970 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/allocations.py
--rw-rw-rw-   0 root         (0) root         (0)     3533 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/bank_account.py
--rw-rw-rw-   0 root         (0) root         (0)     5989 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/contracts.py
--rw-rw-rw-   0 root         (0) root         (0)     2057 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/info.py
--rw-rw-rw-   0 root         (0) root         (0)     4925 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/powerstation.py
--rw-rw-rw-   0 root         (0) root         (0)     5686 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.465578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/tests/
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1640 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/tests/common.py
--rw-rw-rw-   0 root         (0) root         (0)     6052 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/tests/test_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 07:27:05.466578 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo13_addon_photovoltaic_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      448 2023-09-28 07:27:05.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1850 2023-09-28 07:27:05.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-28 07:27:05.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-28 07:27:05.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      212 2023-09-28 07:27:05.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo13_addon_photovoltaic_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-09-28 07:27:05.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-28 07:27:05.467578 odoo13-addon-photovoltaic_api-13.0.1.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-09-28 07:26:47.000000 odoo13-addon-photovoltaic_api-13.0.1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.485269 odoo13-addon-photovoltaic_api-13.0.1.1.9/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-12-13 18:14:16.485269 odoo13-addon-photovoltaic_api-13.0.1.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.475270 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.475270 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.477270 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.478269 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/controllers/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.478269 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/data/data.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.478269 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/models/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/models/auth_jwt_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.480270 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/allocation.py
+-rw-rw-rw-   0 root         (0) root         (0)      148 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/info.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/list_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/power_station.py
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.481269 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)     2578 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/security/ir.model.access.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.483270 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4683 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     4970 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/allocations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3533 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/bank_account.py
+-rw-rw-rw-   0 root         (0) root         (0)     3821 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/contacts.py
+-rw-rw-rw-   0 root         (0) root         (0)     5989 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/contracts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2057 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     4925 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/powerstation.py
+-rw-rw-rw-   0 root         (0) root         (0)     5687 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.483270 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1640 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/tests/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     6052 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/tests/test_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-13 18:14:16.485269 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo13_addon_photovoltaic_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-12-13 18:14:16.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo13_addon_photovoltaic_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-12-13 18:14:16.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-13 18:14:16.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo13_addon_photovoltaic_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-13 18:14:16.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo13_addon_photovoltaic_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      212 2023-12-13 18:14:16.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo13_addon_photovoltaic_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-12-13 18:14:16.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo13_addon_photovoltaic_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-13 18:14:16.485269 odoo13-addon-photovoltaic_api-13.0.1.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-12-13 18:13:58.000000 odoo13-addon-photovoltaic_api-13.0.1.1.9/setup.py
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/CHANGELOG.md` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/__manifest__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/__manifest__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     'name': 'Photovoltaic API',
-    'version': '13.0.1.1.8',
+    'version': '13.0.1.1.9',
     'depends': [
         'base_rest',
         'auth_api_key',
         'auth_jwt',
         'base_rest_pydantic',
         'pydantic',
         'photovoltaic_mgmt',
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/data/data.xml` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/data/data.xml`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/__init__.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/contract.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Optional
 from datetime import date
 from . import OrmModel
 from .power_station import PowerStationShort
 
+
 class Contract(OrmModel):
     id: int
     name: str
     date: date
     power_plant: PowerStationShort
     peak_power: float
     stage: str
@@ -15,8 +16,8 @@
     eq_family_consumption: float
     sent_state: Optional[str]
     product_mode: str
     payment_period: Optional[str]
     investment: float
     bank_account: str
     percentage_invested: float
-    crece_solar_activated: bool
+    crece_solar_activated: bool
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/power_station.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/power_station.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/pydantic_models/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/pydantic_models/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 from typing import List, Optional
 
-from pydantic import EmailStr, Field
+from pydantic import Field
 
 from .bank_account import BankAccountOut
 from .info import Country, State
 from . import OrmModel
 
 
 class UserShort(OrmModel):
-    id:                Optional[int]
-    firstname:         Optional[str]
-    lastname:          Optional[str]
-    vat:               Optional[str]
-    gender:            Optional[str] = Field(alias='gender_partner')
-    birthday:          Optional[str]
-    alias:             Optional[str]
+    id:        Optional[int]
+    firstname: Optional[str]
+    lastname:  Optional[str]
+    vat:       Optional[str]
+    gender:    Optional[str] = Field(alias='gender_partner')
+    birthday:  Optional[str]
+    alias:     Optional[str]
 
 class UserIn(OrmModel):
-    person_type:    Optional[int]= Field(alias='person_type_id')
-    firstname:      Optional[str]
-    lastname:       Optional[str]
-    street:         Optional[str]
-    street2:        Optional[str] = Field(alias='additional_street')
-    zip:            Optional[str]
-    city:           Optional[str]
-    state_id:       Optional[int]
-    country_id:     Optional[int]
-    email:          Optional[str]
-    phone:          Optional[str]
-    mobile:         Optional[str]
-    alias:          Optional[str]
-    vat:            Optional[str]
-    gender_partner: Optional[str] = Field(alias='gender')
-    birthday:       Optional[str]
-    representative: Optional[UserShort]
-    about_us:       Optional[str]
-    interests:      Optional[List[str]]
+    id:                   Optional[int]
+    person_type:          Optional[int] = Field(alias='person_type_id')
+    firstname:            Optional[str]
+    lastname:             Optional[str]
+    street:               Optional[str]
+    street2:              Optional[str] = Field(alias='additional_street')
+    zip:                  Optional[str]
+    city:                 Optional[str]
+    state_id:             Optional[int]
+    country_id:           Optional[int]
+    email:                Optional[str]
+    phone:                Optional[str]
+    mobile:               Optional[str]
+    alias:                Optional[str]
+    vat:                  Optional[str]
+    gender_partner:       Optional[str] = Field(alias='gender')
+    birthday:             Optional[str]
+    representative:       Optional[UserShort]
+    about_us:             Optional[str]
+    interests:            Optional[List[str]]
+    comment:              Optional[str]
+    personal_data_policy: Optional[bool]
+    promotions:           Optional[bool] = False
+    message_notes:        Optional[str] # Notes
 
 class UserOut(OrmModel):
     id:                int
     person_type:       str
     firstname:         str
     lastname:          str
     street:            str
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/security/ir.model.access.csv` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/allocations.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/allocations.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/bank_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/bank_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/contracts.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/contracts.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/info.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/info.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/powerstation.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/powerstation.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/services/user.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/services/user.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -135,8 +135,8 @@
             'allow_promotions': {'type': 'boolean'}
         }
 
     def _validator_mailchimp(self):
         return {
             'type': {'type': 'string'},
             "data[email]": {'type': 'string'}
-        }
+        }
```

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/tests/common.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/tests/common.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo/addons/photovoltaic_api/tests/test_account.py` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo/addons/photovoltaic_api/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `odoo13-addon-photovoltaic_api-13.0.1.1.8/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt` & `odoo13-addon-photovoltaic_api-13.0.1.1.9/odoo13_addon_photovoltaic_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 odoo/addons/photovoltaic_api/pydantic_models/power_station_production.py
 odoo/addons/photovoltaic_api/pydantic_models/user.py
 odoo/addons/photovoltaic_api/security/ir.model.access.csv
 odoo/addons/photovoltaic_api/services/__init__.py
 odoo/addons/photovoltaic_api/services/account.py
 odoo/addons/photovoltaic_api/services/allocations.py
 odoo/addons/photovoltaic_api/services/bank_account.py
+odoo/addons/photovoltaic_api/services/contacts.py
 odoo/addons/photovoltaic_api/services/contracts.py
 odoo/addons/photovoltaic_api/services/info.py
 odoo/addons/photovoltaic_api/services/powerstation.py
 odoo/addons/photovoltaic_api/services/user.py
 odoo/addons/photovoltaic_api/tests/__init__.py
 odoo/addons/photovoltaic_api/tests/common.py
 odoo/addons/photovoltaic_api/tests/test_account.py
```

