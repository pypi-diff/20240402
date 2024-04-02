# Comparing `tmp/edx-organizations-6.8.0.tar.gz` & `tmp/edx-organizations-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-organizations-6.8.0.tar", last modified: Mon Jan 25 20:33:13 2021, max compression
+gzip compressed data, was "edx-organizations-6.9.0.tar", last modified: Mon Feb  8 17:57:50 2021, max compression
```

## Comparing `edx-organizations-6.8.0.tar` & `edx-organizations-6.9.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.857115 edx-organizations-6.8.0/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    35136 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)      118 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3663 2021-01-25 20:33:13.857115 edx-organizations-6.8.0/PKG-INFO
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2325 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.849115 edx-organizations-6.8.0/edx_organizations.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3663 2021-01-25 20:33:13.000000 edx-organizations-6.8.0/edx_organizations.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1814 2021-01-25 20:33:13.000000 edx-organizations-6.8.0/edx_organizations.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-01-25 20:33:13.000000 edx-organizations-6.8.0/edx_organizations.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2021-01-25 20:33:13.000000 edx-organizations-6.8.0/edx_organizations.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2021-01-25 20:33:13.000000 edx-organizations-6.8.0/edx_organizations.egg-info/top_level.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.849115 edx-organizations-6.8.0/organizations/
--rw-rw-r--   0 travis    (2000) travis    (2000)       94 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2655 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/admin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11654 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21261 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/exceptions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.849115 edx-organizations-6.8.0/organizations/management/
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/management/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.849115 edx-organizations-6.8.0/organizations/management/commands/
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/management/commands/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1246 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/management/commands/add_organization.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.853115 edx-organizations-6.8.0/organizations/management/commands/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/management/commands/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1761 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/management/commands/tests/test_add_organization.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.853115 edx-organizations-6.8.0/organizations/migrations/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2317 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/0001_initial.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5006 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/0001_squashed_0007_historicalorganization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      490 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/0002_auto_20170117_1434.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1058 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/0002_unique_short_name.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      535 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/0003_auto_20170221_1138.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      606 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/0004_auto_20170413_2315.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      532 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/0005_auto_20171116_0640.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      536 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/0006_auto_20171207_0259.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2420 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/0007_historicalorganization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/migrations/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2758 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      404 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      475 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/resources.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2701 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/serializers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.853115 edx-organizations-6.8.0/organizations/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       50 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1018 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/tests/factories.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4953 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/tests/test_admin.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37984 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/tests/test_api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/tests/test_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1323 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/tests/test_models.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1153 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/tests/test_serializers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      844 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/tests/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      211 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/urls.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.853115 edx-organizations-6.8.0/organizations/v0/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/v0/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.853115 edx-organizations-6.8.0/organizations/v0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/v0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7361 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/v0/tests/test_views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      298 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/v0/urls.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2984 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/v0/views.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      812 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/organizations/validators.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-01-25 20:33:13.857115 edx-organizations-6.8.0/requirements/
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/requirements/base.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2128 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/requirements/base.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      468 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/requirements/constraints.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      253 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/requirements/test.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      328 2021-01-25 20:33:13.857115 edx-organizations-6.8.0/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1751 2021-01-25 20:31:33.000000 edx-organizations-6.8.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.683311 edx-organizations-6.9.0/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    35136 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/LICENSE
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      118 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3663 2021-02-08 17:57:50.683311 edx-organizations-6.9.0/PKG-INFO
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2325 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.675307 edx-organizations-6.9.0/edx_organizations.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3663 2021-02-08 17:57:50.000000 edx-organizations-6.9.0/edx_organizations.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1876 2021-02-08 17:57:50.000000 edx-organizations-6.9.0/edx_organizations.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-02-08 17:57:50.000000 edx-organizations-6.9.0/edx_organizations.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      117 2021-02-08 17:57:50.000000 edx-organizations-6.9.0/edx_organizations.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2021-02-08 17:57:50.000000 edx-organizations-6.9.0/edx_organizations.egg-info/top_level.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.675307 edx-organizations-6.9.0/organizations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       94 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3500 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/admin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11654 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21261 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/exceptions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.675307 edx-organizations-6.9.0/organizations/management/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/management/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.675307 edx-organizations-6.9.0/organizations/management/commands/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/management/commands/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1246 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/management/commands/add_organization.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.679309 edx-organizations-6.9.0/organizations/management/commands/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/management/commands/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1761 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/management/commands/tests/test_add_organization.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.679309 edx-organizations-6.9.0/organizations/migrations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2317 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0001_initial.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5006 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0001_squashed_0007_historicalorganization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      490 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0002_auto_20170117_1434.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1058 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0002_unique_short_name.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      535 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0003_auto_20170221_1138.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2146 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0003_historicalorganizationcourse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      606 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0004_auto_20170413_2315.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      532 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0005_auto_20171116_0640.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      536 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0006_auto_20171207_0259.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2420 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/0007_historicalorganization.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/migrations/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2793 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      404 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      475 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/resources.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2701 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/serializers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.679309 edx-organizations-6.9.0/organizations/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       50 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1018 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/tests/factories.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4953 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/tests/test_admin.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37984 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/tests/test_api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1402 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/tests/test_data.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1323 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/tests/test_models.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1153 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/tests/test_serializers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      844 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/tests/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      211 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/urls.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.679309 edx-organizations-6.9.0/organizations/v0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/v0/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.679309 edx-organizations-6.9.0/organizations/v0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/v0/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7361 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/v0/tests/test_views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      298 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/v0/urls.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2984 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/v0/views.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      812 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/organizations/validators.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-02-08 17:57:50.683311 edx-organizations-6.9.0/requirements/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      137 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/requirements/base.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2166 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/requirements/base.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      563 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/requirements/constraints.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      253 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/requirements/test.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      328 2021-02-08 17:57:50.683311 edx-organizations-6.9.0/setup.cfg
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1751 2021-02-08 17:56:19.000000 edx-organizations-6.9.0/setup.py
```

### Comparing `edx-organizations-6.8.0/LICENSE` & `edx-organizations-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/PKG-INFO` & `edx-organizations-6.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-organizations
-Version: 6.8.0
+Version: 6.9.0
 Summary: Organization management module for Open edX
 Home-page: https://github.com/edx/edx-organizations
 Author: edX
 Author-email: UNKNOWN
 License: AGPL
 Description: edx-organizations |Build Status| |Coverage Status|
         ==================================================
```

### Comparing `edx-organizations-6.8.0/README.rst` & `edx-organizations-6.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/edx_organizations.egg-info/PKG-INFO` & `edx-organizations-6.9.0/edx_organizations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: edx-organizations
-Version: 6.8.0
+Version: 6.9.0
 Summary: Organization management module for Open edX
 Home-page: https://github.com/edx/edx-organizations
 Author: edX
 Author-email: UNKNOWN
 License: AGPL
 Description: edx-organizations |Build Status| |Coverage Status|
         ==================================================
```

### Comparing `edx-organizations-6.8.0/edx_organizations.egg-info/SOURCES.txt` & `edx-organizations-6.9.0/edx_organizations.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 organizations/management/commands/tests/__init__.py
 organizations/management/commands/tests/test_add_organization.py
 organizations/migrations/0001_initial.py
 organizations/migrations/0001_squashed_0007_historicalorganization.py
 organizations/migrations/0002_auto_20170117_1434.py
 organizations/migrations/0002_unique_short_name.py
 organizations/migrations/0003_auto_20170221_1138.py
+organizations/migrations/0003_historicalorganizationcourse.py
 organizations/migrations/0004_auto_20170413_2315.py
 organizations/migrations/0005_auto_20171116_0640.py
 organizations/migrations/0006_auto_20171207_0259.py
 organizations/migrations/0007_historicalorganization.py
 organizations/migrations/__init__.py
 organizations/tests/__init__.py
 organizations/tests/factories.py
```

### Comparing `edx-organizations-6.8.0/organizations/api.py` & `edx-organizations-6.9.0/organizations/api.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/data.py` & `edx-organizations-6.9.0/organizations/data.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/exceptions.py` & `edx-organizations-6.9.0/organizations/exceptions.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/management/commands/add_organization.py` & `edx-organizations-6.9.0/organizations/management/commands/add_organization.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/management/commands/tests/test_add_organization.py` & `edx-organizations-6.9.0/organizations/management/commands/tests/test_add_organization.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/migrations/0001_initial.py` & `edx-organizations-6.9.0/organizations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/migrations/0001_squashed_0007_historicalorganization.py` & `edx-organizations-6.9.0/organizations/migrations/0001_squashed_0007_historicalorganization.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/migrations/0002_unique_short_name.py` & `edx-organizations-6.9.0/organizations/migrations/0002_unique_short_name.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/migrations/0003_auto_20170221_1138.py` & `edx-organizations-6.9.0/organizations/migrations/0003_auto_20170221_1138.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/migrations/0004_auto_20170413_2315.py` & `edx-organizations-6.9.0/organizations/migrations/0004_auto_20170413_2315.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/migrations/0005_auto_20171116_0640.py` & `edx-organizations-6.9.0/organizations/migrations/0005_auto_20171116_0640.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/migrations/0006_auto_20171207_0259.py` & `edx-organizations-6.9.0/organizations/migrations/0006_auto_20171207_0259.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/migrations/0007_historicalorganization.py` & `edx-organizations-6.9.0/organizations/migrations/0007_historicalorganization.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/models.py` & `edx-organizations-6.9.0/organizations/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,12 +56,14 @@
     (in the Django/ORM sense) the modeling and integrity is limited to that
     of specifying course identifier strings in this model.
     """
     course_id = models.CharField(max_length=255, db_index=True, verbose_name='Course ID')
     organization = models.ForeignKey(Organization, db_index=True, on_delete=models.CASCADE)
     active = models.BooleanField(default=True)
 
+    history = HistoricalRecords()
+
     class Meta:
         """ Meta class for this Django model """
         unique_together = (('course_id', 'organization'),)
         verbose_name = _('Link Course')
         verbose_name_plural = _('Link Courses')
```

### Comparing `edx-organizations-6.8.0/organizations/serializers.py` & `edx-organizations-6.9.0/organizations/serializers.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/tests/factories.py` & `edx-organizations-6.9.0/organizations/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/tests/test_admin.py` & `edx-organizations-6.9.0/organizations/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/tests/test_api.py` & `edx-organizations-6.9.0/organizations/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
             api.remove_organization(self.test_organization['id'])
 
         with self.assertRaises(exceptions.InvalidOrganizationException):
             api.get_organization(self.test_organization['id'])
 
     def test_add_organization_course(self):
         """ Unit Test: test_add_organization_course """
-        with self.assertNumQueries(2):
+        with self.assertNumQueries(3):
             api.add_organization_course(
                 self.test_organization,
                 self.test_course_key
             )
 
     def test_add_organization_course_active_exists(self):
         """ Unit Test: test_add_organization_course_active_exists """
@@ -249,15 +249,15 @@
     def test_add_organization_course_inactive_to_active(self):
         """ Unit Test: test_add_organization_course_inactive_to_active """
         api.add_organization_course(
             self.test_organization,
             self.test_course_key
         )
         api.remove_organization_course(self.test_organization, self.test_course_key)
-        with self.assertNumQueries(3):
+        with self.assertNumQueries(4):
             api.add_organization_course(
                 self.test_organization,
                 self.test_course_key
             )
 
     def test_add_organization_course_bogus_course_key(self):
         """ Unit Test: test_add_organization_course_bogus_course_key """
@@ -316,15 +316,15 @@
         """ Unit Test: test_remove_organization_course """
         api.add_organization_course(
             self.test_organization,
             self.test_course_key
         )
         organizations = api.get_course_organizations(self.test_course_key)
         self.assertEqual(len(organizations), 1)
-        with self.assertNumQueries(3):
+        with self.assertNumQueries(4):
             api.remove_organization_course(self.test_organization, self.test_course_key)
         organizations = api.get_course_organizations(self.test_course_key)
         self.assertEqual(len(organizations), 0)
 
     def test_remove_organization_course_missing_organization(self):
         """ Unit Test: test_remove_organization_course_missing_organization """
         with self.assertNumQueries(1):
@@ -351,15 +351,15 @@
         api.add_organization_course(
             self.test_organization,
             self.test_course_key
         )
         self.assertEqual(len(api.get_organization_courses(self.test_organization)), 1)
 
         # Remove the course dependency
-        with self.assertNumQueries(2):
+        with self.assertNumQueries(3):
             api.remove_course_references(self.test_course_key)
         self.assertEqual(len(api.get_organization_courses(self.test_organization)), 0)
 
     @patch.object(api.log, 'info')
     def test_ensure_organization_retrieves_known_org(self, mock_log_info):
         """
         Test that, with oranization auto-create enabled, ``ensure_organization``
```

### Comparing `edx-organizations-6.8.0/organizations/tests/test_data.py` & `edx-organizations-6.9.0/organizations/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/tests/test_models.py` & `edx-organizations-6.9.0/organizations/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/tests/test_serializers.py` & `edx-organizations-6.9.0/organizations/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/tests/utils.py` & `edx-organizations-6.9.0/organizations/tests/utils.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/v0/tests/test_views.py` & `edx-organizations-6.9.0/organizations/v0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/v0/views.py` & `edx-organizations-6.9.0/organizations/v0/views.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/organizations/validators.py` & `edx-organizations-6.9.0/organizations/validators.py`

 * *Files identical despite different names*

### Comparing `edx-organizations-6.8.0/requirements/base.txt` & `edx-organizations-6.9.0/requirements/base.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     # via pyjwt
 django-crum==0.7.9
     # via edx-django-utils
 django-model-utils==4.1.1
     # via -r requirements/base.in
 django-simple-history==2.12.0
     # via -r requirements/base.in
-django-waffle==2.0.0
+django-waffle==2.1.0
     # via
     #   edx-django-utils
     #   edx-drf-extensions
-django==2.2.17
+django==2.2.18
     # via
-    #   -c requirements/constraints.txt
+    #   -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
     #   -r requirements/base.in
     #   django-crum
     #   django-model-utils
     #   djangorestframework
     #   drf-jwt
     #   edx-django-utils
     #   edx-drf-extensions
@@ -39,25 +39,25 @@
     #   drf-jwt
     #   edx-drf-extensions
     #   rest-condition
 drf-jwt==1.17.3
     # via edx-drf-extensions
 edx-django-utils==3.13.0
     # via edx-drf-extensions
-edx-drf-extensions==6.3.0
+edx-drf-extensions==6.4.0
     # via -r requirements/base.in
-edx-opaque-keys==2.1.1
+edx-opaque-keys==2.2.0
     # via
     #   -r requirements/base.in
     #   edx-drf-extensions
 future==0.18.2
     # via pyjwkest
 idna==2.10
     # via requests
-newrelic==5.24.0.153
+newrelic==6.0.1.155
     # via edx-django-utils
 pbr==5.5.1
     # via stevedore
 pillow==8.1.0
     # via -r requirements/base.in
 psutil==5.8.0
     # via edx-django-utils
@@ -69,33 +69,32 @@
     # via edx-drf-extensions
 pyjwt[crypto]==1.7.1
     # via drf-jwt
 pymongo==3.11.2
     # via edx-opaque-keys
 python-dateutil==2.8.1
     # via edx-drf-extensions
-pytz==2020.5
+pytz==2021.1
     # via django
 requests==2.25.1
     # via
     #   edx-drf-extensions
     #   pyjwkest
 rest-condition==1.0.3
     # via edx-drf-extensions
 semantic-version==2.8.5
     # via edx-drf-extensions
 six==1.15.0
     # via
     #   cryptography
     #   django-simple-history
     #   edx-drf-extensions
-    #   edx-opaque-keys
     #   pyjwkest
     #   python-dateutil
 sqlparse==0.4.1
     # via django
 stevedore==3.3.0
     # via
     #   edx-django-utils
     #   edx-opaque-keys
-urllib3==1.26.2
+urllib3==1.26.3
     # via requests
```

### Comparing `edx-organizations-6.8.0/setup.py` & `edx-organizations-6.9.0/setup.py`

 * *Files identical despite different names*

