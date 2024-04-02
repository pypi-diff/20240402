# Comparing `tmp/invenio-users-resources-5.1.0.tar.gz` & `tmp/invenio-users-resources-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-users-resources-5.1.0.tar", last modified: Sat Mar 23 14:11:09 2024, max compression
+gzip compressed data, was "dist/invenio-users-resources-5.1.1.tar", last modified: Tue Apr  2 09:01:23 2024, max compression
```

## Comparing `invenio-users-resources-5.1.0.tar` & `invenio-users-resources-5.1.1.tar`

### file list

```diff
@@ -1,353 +1,353 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/entity_resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/notifications/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/notifications/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/dumpers/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/dumpers/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/domains/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/domains/domain-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/groups/group-v2.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/users/
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/users/user-v2.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/domains/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/domains/domain-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/groups/group-v2.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/users/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/users/user-v2.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/domains/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/domains/domain-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/groups/group-v2.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/users/
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/users/user-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/records/systemfields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/domains/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/domains/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/domains/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/groups/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/groups/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/users/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/users/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/resources/users/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/domains/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/domains/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/domains/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/domains/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/domains/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/domains/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/groups/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/groups/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/groups/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/groups/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/groups/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/users/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/users/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/users/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/users/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/users/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/users/search_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/users/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/services/users/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/templates/avatar.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/invenio_users_resources/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8060 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/invenio_users_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/tests/resources/test_resources_domains.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/tests/resources/test_resources_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/tests/resources/test_resources_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/tests/services/test_service_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-23 14:11:09.000000 invenio-users-resources-5.1.0/tests/services/users/
--rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/tests/services/users/test_service_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/tests/services/users/test_user_moderation.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/tests/test_invenio_users_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-23 14:11:01.000000 invenio-users-resources-5.1.0/tests/test_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/entity_resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/notifications/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/notifications/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14136 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/dumpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/dumpers/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/domains/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/domains/domain-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/groups/group-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/users/user-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/domains/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/domains/domain-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/groups/group-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/users/user-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/domains/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/domains/domain-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/groups/group-v2.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/users/user-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/records/systemfields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/domains/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/domains/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/domains/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/groups/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/groups/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/users/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/users/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/resources/users/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/domains/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/domains/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/domains/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/domains/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/domains/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/domains/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/groups/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/groups/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/groups/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/groups/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8803 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/users/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/users/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/users/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/users/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/users/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/users/search_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/users/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/services/users/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/templates/avatar.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/invenio_users_resources/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/invenio_users_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1401 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3361 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    12524 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/tests/resources/test_resources_domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/tests/resources/test_resources_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/tests/resources/test_resources_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/tests/services/test_service_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:01:23.000000 invenio-users-resources-5.1.1/tests/services/users/
+-rw-r--r--   0 runner    (1001) docker     (127)     8771 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/tests/services/users/test_service_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/tests/services/users/test_user_moderation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/tests/test_invenio_users_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-02 09:01:16.000000 invenio-users-resources-5.1.1/tests/test_notifications.py
```

### Comparing `invenio-users-resources-5.1.0/.editorconfig` & `invenio-users-resources-5.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/.github/workflows/pypi-publish.yml` & `invenio-users-resources-5.1.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/.github/workflows/tests.yml` & `invenio-users-resources-5.1.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/.tx/config` & `invenio-users-resources-5.1.1/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/CHANGES.rst` & `invenio-users-resources-5.1.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
     Invenio-Users-Resources is free software; you can redistribute it
     and/or modify it under the terms of the MIT License; see LICENSE file for
     more details.
 
 Changes
 =======
 
+Version 5.1.1 (released 2024-04-02)
+
+- config: enable user administration panel by default
+
 Version 5.1.0 (released 2024-03-23)
 
 - mappings: change "dynamic" values to string
 - resolvers: pick resolved fields for group
 - init: move record_once to finalize_app
 
 Version 5.0.3 (released 2024-02-23)
```

### Comparing `invenio-users-resources-5.1.0/CONTRIBUTING.rst` & `invenio-users-resources-5.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/LICENSE` & `invenio-users-resources-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/MANIFEST.in` & `invenio-users-resources-5.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/PKG-INFO` & `invenio-users-resources-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-users-resources
-Version: 5.1.0
+Version: 5.1.1
 Summary: Invenio module providing management APIs for users and roles/groups.
 Home-page: https://github.com/inveniosoftware/invenio-users-resources
 Author: CERN/TU Wien/JRC
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             Invenio-Users-Resources is free software; you can redistribute it
             and/or modify it under the terms of the MIT License; see LICENSE file for
             more details.
         
         Changes
         =======
         
+        Version 5.1.1 (released 2024-04-02)
+        
+        - config: enable user administration panel by default
+        
         Version 5.1.0 (released 2024-03-23)
         
         - mappings: change "dynamic" values to string
         - resolvers: pick resolved fields for group
         - init: move record_once to finalize_app
         
         Version 5.0.3 (released 2024-02-23)
```

### Comparing `invenio-users-resources-5.1.0/README.rst` & `invenio-users-resources-5.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/docs/Makefile` & `invenio-users-resources-5.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/docs/conf.py` & `invenio-users-resources-5.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/docs/index.rst` & `invenio-users-resources-5.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/docs/make.bat` & `invenio-users-resources-5.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/config.py` & `invenio-users-resources-5.1.1/invenio_users_resources/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         "ui": {
             "field": "visibility",
         },
     },
 }
 """Invenio requests facets."""
 
-USERS_RESOURCES_ADMINISTRATION_ENABLED = False
+USERS_RESOURCES_ADMINISTRATION_ENABLED = True
 """Enable the user administration"""
 
 USERS_RESOURCES_MODERATION_LOCK_DEFAULT_TIMEOUT = 30
 """Default timeout, in seconds, to lock a user when moderating."""
 
 USERS_RESOURCES_MODERATION_LOCK_RENEWAL_TIMEOUT = 120
 """Renewal timeout, in seconds, to increase the lock time for a user when moderating."""
```

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/entity_resolvers.py` & `invenio-users-resources-5.1.1/invenio_users_resources/entity_resolvers.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/ext.py` & `invenio-users-resources-5.1.1/invenio_users_resources/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/forms.py` & `invenio-users-resources-5.1.1/invenio_users_resources/forms.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/models.py` & `invenio-users-resources-5.1.1/invenio_users_resources/models.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/notifications/filters.py` & `invenio-users-resources-5.1.1/invenio_users_resources/notifications/filters.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/notifications/generators.py` & `invenio-users-resources-5.1.1/invenio_users_resources/notifications/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/proxies.py` & `invenio-users-resources-5.1.1/invenio_users_resources/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/api.py` & `invenio-users-resources-5.1.1/invenio_users_resources/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/dumpers/email.py` & `invenio-users-resources-5.1.1/invenio_users_resources/records/dumpers/email.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/hooks.py` & `invenio-users-resources-5.1.1/invenio_users_resources/records/hooks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/domains/domain-v1.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/domains/domain-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/groups/group-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/groups/group-v2.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/groups/group-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v1/users/user-v2.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v1/users/user-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/domains/domain-v1.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/domains/domain-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/groups/group-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/groups/group-v2.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/groups/group-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/os-v2/users/user-v2.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/os-v2/users/user-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/domains/domain-v1.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/domains/domain-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/groups/group-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/groups/group-v2.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/groups/group-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/users/user-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/mappings/v7/users/user-v2.0.0.json` & `invenio-users-resources-5.1.1/invenio_users_resources/records/mappings/v7/users/user-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/models.py` & `invenio-users-resources-5.1.1/invenio_users_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/records/systemfields/__init__.py` & `invenio-users-resources-5.1.1/invenio_users_resources/records/systemfields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/resources/__init__.py` & `invenio-users-resources-5.1.1/invenio_users_resources/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/resources/domains/config.py` & `invenio-users-resources-5.1.1/invenio_users_resources/resources/domains/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/resources/domains/resource.py` & `invenio-users-resources-5.1.1/invenio_users_resources/resources/domains/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/resources/groups/config.py` & `invenio-users-resources-5.1.1/invenio_users_resources/resources/groups/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/resources/groups/resource.py` & `invenio-users-resources-5.1.1/invenio_users_resources/resources/groups/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/resources/users/config.py` & `invenio-users-resources-5.1.1/invenio_users_resources/resources/users/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/resources/users/resource.py` & `invenio-users-resources-5.1.1/invenio_users_resources/resources/users/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/__init__.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/common.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/common.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/domains/components.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/domains/components.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/domains/config.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/domains/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/domains/facets.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/domains/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/domains/service.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/domains/service.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/domains/tasks.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/domains/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/generators.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/groups/config.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/groups/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/groups/results.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/groups/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/groups/service.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/groups/service.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/groups/tasks.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/groups/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/params.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/params.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/permissions.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/results.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/schemas.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/users/config.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/users/config.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/users/facets.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/users/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/users/lock.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/users/lock.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/users/results.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/users/results.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/users/search_params.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/users/search_params.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/users/service.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/users/service.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/services/users/tasks.py` & `invenio-users-resources-5.1.1/invenio_users_resources/services/users/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html` & `invenio-users-resources-5.1.1/invenio_users_resources/templates/semantic-ui/invenio_users_resources/settings/notifications.html`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/messages.pot` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-users-resources-5.1.1/invenio_users_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources/views.py` & `invenio-users-resources-5.1.1/invenio_users_resources/views.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources.egg-info/PKG-INFO` & `invenio-users-resources-5.1.1/invenio_users_resources.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-users-resources
-Version: 5.1.0
+Version: 5.1.1
 Summary: Invenio module providing management APIs for users and roles/groups.
 Home-page: https://github.com/inveniosoftware/invenio-users-resources
 Author: CERN/TU Wien/JRC
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
@@ -42,14 +42,18 @@
             Invenio-Users-Resources is free software; you can redistribute it
             and/or modify it under the terms of the MIT License; see LICENSE file for
             more details.
         
         Changes
         =======
         
+        Version 5.1.1 (released 2024-04-02)
+        
+        - config: enable user administration panel by default
+        
         Version 5.1.0 (released 2024-03-23)
         
         - mappings: change "dynamic" values to string
         - resolvers: pick resolved fields for group
         - init: move record_once to finalize_app
         
         Version 5.0.3 (released 2024-02-23)
```

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources.egg-info/SOURCES.txt` & `invenio-users-resources-5.1.1/invenio_users_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources.egg-info/entry_points.txt` & `invenio-users-resources-5.1.1/invenio_users_resources.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/invenio_users_resources.egg-info/requires.txt` & `invenio-users-resources-5.1.1/invenio_users_resources.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/run-tests.sh` & `invenio-users-resources-5.1.1/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/setup.cfg` & `invenio-users-resources-5.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/tests/conftest.py` & `invenio-users-resources-5.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/tests/resources/test_resources_domains.py` & `invenio-users-resources-5.1.1/tests/resources/test_resources_domains.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/tests/resources/test_resources_groups.py` & `invenio-users-resources-5.1.1/tests/resources/test_resources_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/tests/resources/test_resources_users.py` & `invenio-users-resources-5.1.1/tests/resources/test_resources_users.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/tests/services/test_service_groups.py` & `invenio-users-resources-5.1.1/tests/services/test_service_groups.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/tests/services/users/test_service_users.py` & `invenio-users-resources-5.1.1/tests/services/users/test_service_users.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/tests/services/users/test_user_moderation.py` & `invenio-users-resources-5.1.1/tests/services/users/test_user_moderation.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/tests/test_invenio_users_resources.py` & `invenio-users-resources-5.1.1/tests/test_invenio_users_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-users-resources-5.1.0/tests/test_notifications.py` & `invenio-users-resources-5.1.1/tests/test_notifications.py`

 * *Files identical despite different names*

