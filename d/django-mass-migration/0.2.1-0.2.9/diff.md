# Comparing `tmp/django-mass-migration-0.2.1.tar.gz` & `tmp/django-mass-migration-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mass-migration-0.2.1.tar", last modified: Tue Apr  2 14:59:33 2024, max compression
+gzip compressed data, was "django-mass-migration-0.2.9.tar", last modified: Mon Jan  8 12:18:29 2024, max compression
```

## Comparing `django-mass-migration-0.2.1.tar` & `django-mass-migration-0.2.9.tar`

### file list

```diff
@@ -1,68 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.524439 django-mass-migration-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-02 14:59:33.524439 django-mass-migration-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.516439 django-mass-migration-0.2.1/django_mass_migration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-02 14:59:33.000000 django-mass-migration-0.2.1/django_mass_migration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-02 14:59:33.000000 django-mass-migration-0.2.1/django_mass_migration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:59:33.000000 django-mass-migration-0.2.1/django_mass_migration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 14:59:33.000000 django-mass-migration-0.2.1/django_mass_migration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 14:59:33.000000 django-mass-migration-0.2.1/django_mass_migration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/massmigration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/massmigration/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/backends/djangae.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/enforcement.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/massmigration/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/massmigration/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/management/commands/makemassmigration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/record_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.516439 django-mass-migration-0.2.1/massmigration/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.516439 django-mass-migration-0.2.1/massmigration/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.516439 django-mass-migration-0.2.1/massmigration/templates/admin/massmigration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/massmigration/templates/admin/massmigration/migrationrecord/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/massmigration/templates/massmigration/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/templates/massmigration/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/templates/massmigration/delete_migration.html
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/templates/massmigration/manage_migrations.html
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/templates/massmigration/migration_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/templates/massmigration/run_migration.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/massmigration/templates/migration_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/templates/migration_templates/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/templates/migration_templates/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/templates/migration_templates/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/massmigration/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/tests/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/massmigration/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/utils/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/utils/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/massmigration/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1286 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/scripts/release.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1590 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/scripts/run_tests_locally.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:59:33.524439 django-mass-migration-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-02 14:59:32.000000 django-mass-migration-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:33.520439 django-mass-migration-0.2.1/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-02 14:59:28.000000 django-mass-migration-0.2.1/testing/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.000546 django-mass-migration-0.2.9/django_mass_migration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7423 2024-01-08 12:18:28.000000 django-mass-migration-0.2.9/django_mass_migration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-01-08 12:18:28.000000 django-mass-migration-0.2.9/django_mass_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 12:18:28.000000 django-mass-migration-0.2.9/django_mass_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-08 12:18:28.000000 django-mass-migration-0.2.9/django_mass_migration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-08 12:18:28.000000 django-mass-migration-0.2.9/django_mass_migration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.000546 django-mass-migration-0.2.9/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.000546 django-mass-migration-0.2.9/massmigration/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/backends/djangae.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.000546 django-mass-migration-0.2.9/massmigration/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/massmigration/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/management/commands/makemassmigration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/record_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:28.996546 django-mass-migration-0.2.9/massmigration/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:28.996546 django-mass-migration-0.2.9/massmigration/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:28.996546 django-mass-migration-0.2.9/massmigration/templates/admin/massmigration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/massmigration/templates/admin/massmigration/migrationrecord/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/templates/admin/massmigration/migrationrecord/change_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/massmigration/templates/massmigration/
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/templates/massmigration/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/templates/massmigration/delete_migration.html
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/templates/massmigration/manage_migrations.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/templates/massmigration/migration_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/templates/massmigration/run_migration.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/massmigration/templates/migration_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/templates/migration_templates/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/templates/migration_templates/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/templates/migration_templates/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/massmigration/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/massmigration/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/utils/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/utils/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/massmigration/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1286 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/scripts/release.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1590 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/scripts/run_tests_locally.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-08 12:18:26.000000 django-mass-migration-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 12:18:29.004546 django-mass-migration-0.2.9/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-01-08 12:18:21.000000 django-mass-migration-0.2.9/testing/test_settings.py
```

### Comparing `django-mass-migration-0.2.1/LICENSE` & `django-mass-migration-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.2.1/PKG-INFO` & `django-mass-migration-0.2.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.2.1
+Version: 0.2.9
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -86,21 +86,14 @@
 
 ### custom
 
 If you want to take matters into your own hands you can write an entirely custom migration.
 These can still be tracked the same as the other operations, but the implementation of what your migration
 does and how your the backend handles it are up to you.
 
-Running with Multiple DBs
--------------------
-If your project connects to multiple databases it is possible to run your migrations against each database individually.
-The migrations are not forced on a specific DB but rather the `db_alias` is passed to both to `get_queryset(db_alias)` (for mappers migrations) and `operation` (for simple migrations) giving control back to the developer to customise what is retrieved for the migration.
-
-By default a migration can be run on any available database. That can be customised but setting `allowed_db_aliases` on the migration class.
-
 
 Applying Migrations
 -------------------
 
 There are two ways to apply a migration to the database:
 
 ### Via the Web UI
@@ -135,28 +128,17 @@
 
 ```python
 @requires_migration(("myapp", "0001_my_migration"))
 def my_function():
 	...
 ```
 
-
 This will raise `massmigration.exceptions.RequiredMigrationNotApplied` if the function is called before the migration is applied.
 
-### Multiple DBs Support
-When running on multiple databases, by default, the utilities assume that the migration must have been applied on all the databases specified by the Migration's `allowed_db_aliases` attribute.
-To customise that behaviour the decorators accept an optional `db_aliases` list to specify a subset of the aliases allowed for the migration and require only those to have been applied.
-
-```python
-@requires_migration(("myapp", "0001_my_migration"), db_aliases=["my_db_alias"])
-def my_function():
-	...
-```
-
-### Notes:
+Notes:
 * If the migration _is_ applied, then this will cache that fact, so it will only query the database the first time the function is called.
 * The migration identifier can either be a tuple of `(app_label, migration_name)` or can be a string of `"app_label:migration_name"`.
 * There is an optional second argument `skip_in_tests`, which defaults to `True`.
 
 
 #### `massmigration.enforcement.view_requires_migration`
```

### Comparing `django-mass-migration-0.2.1/README.md` & `django-mass-migration-0.2.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -67,21 +67,14 @@
 
 ### custom
 
 If you want to take matters into your own hands you can write an entirely custom migration.
 These can still be tracked the same as the other operations, but the implementation of what your migration
 does and how your the backend handles it are up to you.
 
-Running with Multiple DBs
--------------------
-If your project connects to multiple databases it is possible to run your migrations against each database individually.
-The migrations are not forced on a specific DB but rather the `db_alias` is passed to both to `get_queryset(db_alias)` (for mappers migrations) and `operation` (for simple migrations) giving control back to the developer to customise what is retrieved for the migration.
-
-By default a migration can be run on any available database. That can be customised but setting `allowed_db_aliases` on the migration class.
-
 
 Applying Migrations
 -------------------
 
 There are two ways to apply a migration to the database:
 
 ### Via the Web UI
@@ -116,28 +109,17 @@
 
 ```python
 @requires_migration(("myapp", "0001_my_migration"))
 def my_function():
 	...
 ```
 
-
 This will raise `massmigration.exceptions.RequiredMigrationNotApplied` if the function is called before the migration is applied.
 
-### Multiple DBs Support
-When running on multiple databases, by default, the utilities assume that the migration must have been applied on all the databases specified by the Migration's `allowed_db_aliases` attribute.
-To customise that behaviour the decorators accept an optional `db_aliases` list to specify a subset of the aliases allowed for the migration and require only those to have been applied.
-
-```python
-@requires_migration(("myapp", "0001_my_migration"), db_aliases=["my_db_alias"])
-def my_function():
-	...
-```
-
-### Notes:
+Notes:
 * If the migration _is_ applied, then this will cache that fact, so it will only query the database the first time the function is called.
 * The migration identifier can either be a tuple of `(app_label, migration_name)` or can be a string of `"app_label:migration_name"`.
 * There is an optional second argument `skip_in_tests`, which defaults to `True`.
 
 
 #### `massmigration.enforcement.view_requires_migration`
```

### Comparing `django-mass-migration-0.2.1/django_mass_migration.egg-info/PKG-INFO` & `django-mass-migration-0.2.9/django_mass_migration.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mass-migration
-Version: 0.2.1
+Version: 0.2.9
 Summary: Django app for long-running data migrations
 Home-page: https://github.com/adamalton/django-mass-migration
 Author: Adam Alton
 Keywords: django,djangae,django-gcloud-connectors,Google App Engine
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -86,21 +86,14 @@
 
 ### custom
 
 If you want to take matters into your own hands you can write an entirely custom migration.
 These can still be tracked the same as the other operations, but the implementation of what your migration
 does and how your the backend handles it are up to you.
 
-Running with Multiple DBs
--------------------
-If your project connects to multiple databases it is possible to run your migrations against each database individually.
-The migrations are not forced on a specific DB but rather the `db_alias` is passed to both to `get_queryset(db_alias)` (for mappers migrations) and `operation` (for simple migrations) giving control back to the developer to customise what is retrieved for the migration.
-
-By default a migration can be run on any available database. That can be customised but setting `allowed_db_aliases` on the migration class.
-
 
 Applying Migrations
 -------------------
 
 There are two ways to apply a migration to the database:
 
 ### Via the Web UI
@@ -135,28 +128,17 @@
 
 ```python
 @requires_migration(("myapp", "0001_my_migration"))
 def my_function():
 	...
 ```
 
-
 This will raise `massmigration.exceptions.RequiredMigrationNotApplied` if the function is called before the migration is applied.
 
-### Multiple DBs Support
-When running on multiple databases, by default, the utilities assume that the migration must have been applied on all the databases specified by the Migration's `allowed_db_aliases` attribute.
-To customise that behaviour the decorators accept an optional `db_aliases` list to specify a subset of the aliases allowed for the migration and require only those to have been applied.
-
-```python
-@requires_migration(("myapp", "0001_my_migration"), db_aliases=["my_db_alias"])
-def my_function():
-	...
-```
-
-### Notes:
+Notes:
 * If the migration _is_ applied, then this will cache that fact, so it will only query the database the first time the function is called.
 * The migration identifier can either be a tuple of `(app_label, migration_name)` or can be a string of `"app_label:migration_name"`.
 * There is an optional second argument `skip_in_tests`, which defaults to `True`.
 
 
 #### `massmigration.enforcement.view_requires_migration`
```

### Comparing `django-mass-migration-0.2.1/django_mass_migration.egg-info/SOURCES.txt` & `django-mass-migration-0.2.9/django_mass_migration.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,16 @@
 massmigration/templates/massmigration/migration_detail.html
 massmigration/templates/massmigration/run_migration.html
 massmigration/templates/migration_templates/custom.py
 massmigration/templates/migration_templates/mapper.py
 massmigration/templates/migration_templates/simple.py
 massmigration/tests/__init__.py
 massmigration/tests/test_commands.py
-massmigration/tests/test_loader.py
 massmigration/utils/__init__.py
 massmigration/utils/apps.py
 massmigration/utils/functional.py
 massmigration/utils/permissions.py
 massmigration/utils/test.py
 massmigration/utils/transaction.py
 scripts/release.py
 scripts/run_tests_locally.py
-testing/__init__.py
 testing/test_settings.py
```

### Comparing `django-mass-migration-0.2.1/massmigration/admin.py` & `django-mass-migration-0.2.9/massmigration/admin.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.2.1/massmigration/api.py` & `django-mass-migration-0.2.9/massmigration/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,37 +14,37 @@
 
 
 def get_all_migrations() -> List[BaseMigration]:
     """ Returns a list of all migrations from all installed apps, ordered by app. """
     return store.all
 
 
-def migration_is_applied(migration: BaseMigration, db_alias: str) -> bool:
+def migration_is_applied(migration: BaseMigration) -> bool:
     """ Is the given migration applied? """
-    return enforcement.migration_is_applied(migration.key, db_alias)
+    return enforcement.migration_is_applied(migration.key)
 
 
-def migration_was_started(migration: BaseMigration, db_alias: str) -> bool:
+def migration_was_started(migration: BaseMigration) -> bool:
     """ Has the given migration ever been initiated (even if it hasn't finished or it failed)? """
-    return MigrationRecord.objects.using(db_alias).filter(key=migration.key).exists()
+    return MigrationRecord.objects.filter(key=migration.key).exists()
 
 
-def migration_is_in_progress(migration: BaseMigration, db_alias: str) -> bool:
+def migration_is_in_progress(migration: BaseMigration) -> bool:
     """ Is the given migration currently running (started but not yet finished and not errored)? """
-    return MigrationRecord.objects.using(db_alias).filter(
+    return MigrationRecord.objects.filter(
         key=migration.key, is_applied=False, has_error=False
     ).exists()
 
 
-def can_start_migration(migration: BaseMigration, db_alias: str) -> bool:
+def can_start_migration(migration: BaseMigration) -> bool:
     """ Can the given migration be started? I.e. either it's never been started or all previous
         attempts have errored.
     """
-    return not MigrationRecord.objects.using(db_alias).filter(key=migration.key).exclude(
+    return not MigrationRecord.objects.filter(key=migration.key).exclude(
         has_error=True
     ).exists()
 
 
-def initiate_migration(migration: BaseMigration, db_alias: str) -> bool:
+def initiate_migration(migration: BaseMigration) -> bool:
     if migration_is_in_progress(migration):
-        raise MigrationAlreadyStarted(f"Migration {migration.key} on db '{db_alias}' is already running.")
-    migration.launch(db_alias)
+        raise MigrationAlreadyStarted(f"Migration {migration.key} is already running.")
+    migration.launch()
```

### Comparing `django-mass-migration-0.2.1/massmigration/backends/base.py` & `django-mass-migration-0.2.9/massmigration/backends/base.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.2.1/massmigration/backends/djangae.py` & `django-mass-migration-0.2.9/massmigration/backends/djangae.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,53 +26,52 @@
 
 
 class DjangaeBackend(BackendBase):
     """ Backend for running operations on Google Cloud Tasks in Djangae projects.
         Works with SQL, Cloud Datastore and Firestore.
     """
 
-    def run_simple(self, migration, db_alias):
-        defer(migration.wrapped_operation, db_alias, _queue=self._get_queue_name(migration), _using=db_alias)
+    def run_simple(self, migration):
+        defer(migration.wrapped_operation, _queue=self._get_queue_name(migration))
         logger.info("Deferred task to run single-task migration %s", migration.key)
 
-    def run_mapper(self, migration, db_alias):
+    def run_mapper(self, migration):
         # Use `defer_iteration_with_finalize` to do the processing with whichever key_ranges_getter
         # is appropriate for the DB.
-        queryset = migration.get_queryset(db_alias)
+        queryset = migration.get_queryset()
         key_ranges_getter = self._key_ranges_getter(queryset)
-        with get_transaction(db_alias).atomic(using=db_alias):
-            attempt_uuid = migration.mark_as_started(db_alias)
+        with get_transaction().atomic():
+            attempt_uuid = migration.mark_as_started()
             defer_iteration_with_finalize(
                 queryset,
                 self._call_mapper_wrapped_operation,
                 self._mark_mapper_as_finished,
                 key_ranges_getter=key_ranges_getter,
                 migration=migration,
                 attempt_uuid=attempt_uuid,
-                db_alias=db_alias,
                 _queue=self._get_queue_name(migration),
                 _transactional=True,
             )
             logger.info("Deferred task to run mapper migration %s", migration.key)
 
     def _get_queue_name(self, migration):
         """ Get the queue name from settings, or the override on the migration, if set."""
         queue = getattr(migration, "queue_name", None)
         if not queue:
             queue = getattr(settings, "MASSMIGRATION_TASK_QUEUE", None)
         if not queue:
             raise NotImplementedError("Please configure settings.MASSMIGRATION_TASK_QUEUE.")
         return queue
 
-    def _call_mapper_wrapped_operation(self, instance, migration, attempt_uuid, db_alias):
-        migration.wrapped_operation(instance, attempt_uuid, db_alias)
+    def _call_mapper_wrapped_operation(self, instance, migration, attempt_uuid):
+        migration.wrapped_operation(instance, attempt_uuid)
 
-    def _mark_mapper_as_finished(self, migration, attempt_uuid, db_alias):
+    def _mark_mapper_as_finished(self, migration, attempt_uuid):
         logger.info("Marking migration %s (attempt %s) as finished.", migration.key, attempt_uuid)
-        migration.mark_as_finished(db_alias)
+        migration.mark_as_finished()
 
     def _key_ranges_getter(self, queryset):
         # TODO: this could be better at handling the different cases
         connection = router.db_for_write(queryset.model)
         engine = settings.DATABASES[connection]["ENGINE"]
         pk_field = queryset.model._meta.pk
         if isinstance(pk_field, models.UUIDField):
```

### Comparing `django-mass-migration-0.2.1/massmigration/loader.py` & `django-mass-migration-0.2.9/massmigration/tests/test_commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,66 @@
 # Standard library
 import os
-import re
+import shutil
 
 # Third party
 from django.apps.registry import apps
-from django.utils.module_loading import import_string
+from django.core.management import execute_from_command_line
+from django.test import TestCase
 
 # Mass Migration
-from .constants import MIGRATIONS_FOLDER
+from massmigration.constants import MIGRATIONS_FOLDER
 
 
-class MigrationsStore:
-    """ Stores a cache of the installed migrations to save us loading them from the filesystem
-        repeatedly. Also allows us to access them by key.
-    """
-
-    def __init__(self):
-        self._loaded = False
-        self._all = []
-        self._by_key = {}
-
-    @property
-    def all(self):
-        if not self._loaded:
-            self.load()
-        return self._all
-
-    @property
-    def by_key(self):
-        if not self._loaded:
-            self.load()
-        return self._by_key
-
-    def load(self):
-        """ Load all the migration instances from all migration files found in installed apps. """
-        for app_config in apps.get_app_configs():
-            migrations_path = os.path.join(app_config.path, MIGRATIONS_FOLDER)
-            if os.path.isdir(migrations_path):
-                items = os.listdir(migrations_path)
-                for item in sorted(items):
-                    migration_id = migration_id_from_filename(item)
-                    if migration_id:
-                        migration = load_migration(app_config, migration_id)
-                        self._all.append(migration)
-                        self._by_key[migration.key] = migration
-        self._loaded = True
-
-
-store = MigrationsStore()
-
-
-def migration_id_from_filename(filename):
-    if filename.endswith(".py"):
-        migration_id = re.sub(r"\.py$", "", filename)
-        if is_valid_migration_id(migration_id):
-            return migration_id
-    return None
-
-
-def is_valid_migration_name(name):
-    """ Is the given name (supplied without leading number) a valid name for a migration? """
-    return bool(re.match(r"^[a-z0-9_]+$", name))
-
-
-def is_valid_migration_id(name):
-    return bool(re.match(r"^\d{1,5}_[a-z0-9_]+$", name))
-
-
-def load_migration(app_config, filename):
-    """ Return in instance of the migration class from the given filename from the given app_config.
-    """
-    module_str = app_config.name
-    migration_id = migration_id_from_filename(filename)
-    class_path_str = f"{module_str}.{MIGRATIONS_FOLDER}.{migration_id}.Migration"
-    cls = import_string(class_path_str)
-    app_label = app_config.label
-    instance = cls(app_label, migration_id)
-    return instance
+class MakeMassMigrationTestCase(TestCase):
+    """ Tests for the 'makemassmigration' command. """
+
+    def tearDown(self):
+        super().tearDown()
+        self.delete_massmigrations_folder()
+
+    def migrations_folder_path(self, app_name="massmigration"):
+        """ The expected folder path where the command will put the migration files. """
+        app = apps.get_app_config(app_name)
+        return os.path.join(app.path, MIGRATIONS_FOLDER)
+
+    def delete_massmigrations_folder(self, app_name="massmigration"):
+        """ Delete the folder which the command puts the migration files into. """
+        path = self.migrations_folder_path(app_name)
+        if os.path.exists(path):
+            shutil.rmtree(path)
+
+    def get_migration_file(self, file_name, app_name="massmigration"):
+        """ Return the file contents of the given migration file. """
+        file_path = os.path.join(self.migrations_folder_path(app_name), file_name)
+        with open(file_path) as file:
+            return file.read()
+
+    def assert_migration_file_exists(self, file_name, app_name="massmigration"):
+        file_path = os.path.join(self.migrations_folder_path(app_name), file_name)
+        if not os.path.exists(file_path):
+            self.fail(f"Migration file not found at {file_path}")
+
+    def run_command(self, file_name, *args, app_name="massmigration"):
+        execute_from_command_line([
+            "django-admin",
+            "makemassmigration",
+            app_name,
+            file_name,
+            *args,
+        ])
+
+    def test_increments_numbers(self):
+        self.run_command("first_migration")
+        self.assert_migration_file_exists("0001_first_migration.py")
+        self.run_command("second_migration")
+        self.assert_migration_file_exists("0002_second_migration.py")
+
+    def test_uses_correct_template(self):
+        for index, (template, expected_base_class) in enumerate([
+            ("simple", "SimpleMigration"),
+            ("mapper", "MapperMigration"),
+            ("custom", "BaseMigration"),
+        ]):
+            self.run_command("my_migration", "--template", template)
+            file_contents = self.get_migration_file(f"000{index + 1}_my_migration.py")
+            self.assertIn(f"\nclass Migration({expected_base_class}):\n", file_contents)
```

### Comparing `django-mass-migration-0.2.1/massmigration/management/commands/makemassmigration.py` & `django-mass-migration-0.2.9/massmigration/management/commands/makemassmigration.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.2.1/massmigration/migrations.py` & `django-mass-migration-0.2.9/massmigration/migrations.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,67 +7,36 @@
 from django.conf import settings
 from django.db import models
 from django.utils.module_loading import import_string
 
 # Mass Migration
 from . import record_cache
 from .constants import DEFAULT_BACKEND
-from .exceptions import (
-    CannotRunOnDB,
-    DbAliasNotAllowed,
-    DependentMigrationNotApplied,
-    MigrationAlreadyStarted
-)
+from .exceptions import DependentMigrationNotApplied, MigrationAlreadyStarted
 from .models import MigrationRecord
 from .utils.transaction import get_transaction
 
 
 logger = logging.getLogger(__name__)
 
 
-# TODO: Is there a better place for this?
-def get_all_db_aliases():
-    return list(settings.DATABASES.keys())
-
-
 class BaseMigration:
     """ An operation to be performed on the database. """
 
-    allowed_db_aliases = None
-
     dependencies = []  # A list of (app_label, migration_name) pairs
 
     # This can be set to make a migration run on a specific backend, rather than the one that's
     # specified in the Django settings
     backend: str = None
 
     # This specifies the name of the method on the backend class which should be called to run this
     # migration. Custom migration types can be run on custom backends which support them by using
     # this attribute.
     backend_method: str = None
 
-    def __init_subclass__(cls, **kwargs):
-        super().__init_subclass__(**kwargs)
-        all_db_aliases = get_all_db_aliases()
-
-        if (
-            cls.allowed_db_aliases is not None and  # If not set, then all dbs are allowed
-            any([allowed_db not in all_db_aliases for allowed_db in cls.allowed_db_aliases])
-        ):
-            raise DbAliasNotAllowed(
-                    f"Migration {self.key} provided invalid value(s) in `allowed_database_aliases`. "
-                    f"Got <{cls.allowed_db_aliases}> while the available dbs are {', '.join(all_db_aliases)}. "
-                )
-
-    @classmethod
-    def get_allowed_db_aliases(cls):
-        if cls.allowed_db_aliases is None:
-            return get_all_db_aliases()
-        return cls.allowed_db_aliases
-
     def __init__(self, app_label, name):
         self.app_label = app_label
         self.name = name
 
     @property
     def key(self):
         """ A string which uniquely identifies this migration in the system. """
@@ -86,124 +55,112 @@
             DEFAULT_BACKEND
         )
 
     def get_backend(self):
         backend_class = import_string(self.backend_str)
         return backend_class()
 
-    def launch(self, db_alias):
+    def launch(self):
         """ Pass the migration to the backend to perform the data operation(s).
             This is what should be called by the web interface to trigger the migration.
         """
-        allowed_db_aliases = self.get_allowed_db_aliases()
-        if db_alias not in allowed_db_aliases:
-            raise CannotRunOnDB(
-                f"Migration {self.key} can't run on {db_alias}. "
-                f"The allowed DBs for this migration are {', '.join(allowed_db_aliases)}. "
-            )
-
-        self.check_dependencies(db_alias)
+        self.check_dependencies()
         backend = self.get_backend()
         method = getattr(backend, self.backend_method)
-        method(self, db_alias)
+        method(self)
         logger.info("Launched migration %s on backend %s", self.key, backend.__class__)
 
-    def can_be_started(self, db_alias) -> bool:
-        return not MigrationRecord.objects.using(db_alias).filter(key=self.key).exists()
+    def can_be_started(self) -> bool:
+        return not MigrationRecord.objects.filter(key=self.key).exists()
 
-    def mark_as_started(self, db_alias) -> UUID:
+    def mark_as_started(self) -> UUID:
         """ Mark the migration as started in the database. Return the attempt UUID. """
-        with get_transaction(db_alias).atomic(using=db_alias):
-            if not self.can_be_started(db_alias):
+        with get_transaction().atomic():
+            if not self.can_be_started():
                 raise MigrationAlreadyStarted(
                     f"Migration {self.__class__.__name__} has already been initiated."
                 )
-            migration = MigrationRecord.objects.using(db_alias).create(
-                key=self.key,
-            )
+            migration = MigrationRecord.objects.create(key=self.key)
             return migration.attempt_uuid
 
     @retry_on_error()
-    def mark_as_errored(self, db_alias, error=None):
+    def mark_as_errored(self, error=None):
         """ Mark the migration as errored in the database. """
         # TODO: Generate a proper traceback here
         error_str = f"{error.__class__.__name__}: {error}"
-        MigrationRecord.objects.using(db_alias).filter(key=self.key).update(has_error=True, last_error=error_str)
+        MigrationRecord.objects.filter(key=self.key).update(has_error=True, last_error=error_str)
 
     @retry_on_error()
-    def mark_as_finished(self, db_alias):
+    def mark_as_finished(self):
         """ Mark the migration as applied/finalized in the database. """
-        with get_transaction(db_alias).atomic(using=db_alias):
-            migration = MigrationRecord.objects.using(db_alias).get(key=self.key)
+        with get_transaction().atomic():
+            migration = MigrationRecord.objects.get(key=self.key)
             if migration.is_applied:
                 logger.warning("Migration %s is already marked as applied.", self.key)
             else:
                 migration.is_applied = True
                 migration.save()
                 logger.info("Migration %s finished. Marked it as applied.", self.key)
 
-    def check_dependencies(self, db_alias):
+    def check_dependencies(self):
         """ Make sure that any migrations which this migration depends on have been applied. """
         # TODO: check that the specified migrations actually exist in the code.
         dependency_keys = [MigrationRecord.key_from_name_tuple(x) for x in self.dependencies]
-        applied_keys = MigrationRecord.objects.using(db_alias).filter(
+        applied_keys = MigrationRecord.objects.filter(
             is_applied=True, key__in=dependency_keys
         ).values_list("pk", flat=True)
         for dependency_key in dependency_keys:
             if dependency_key not in applied_keys:
                 raise DependentMigrationNotApplied(
                     f"Migration {self.key} depends on migration {dependency_key}, which has not "
                     "yet been applied."
                 )
 
-    def get_migration_record(self, db_alias):
-        return MigrationRecord.objects.using(db_alias).filter(key=self.key).first()
-
 
 class SimpleMigration(BaseMigration):
     """ A migration which only needs to apply a very quick and simple change to the database which
         can be applied by one call of one function which can run in the time and memory constraints
         of one task.
     """
 
     backend_method = "run_simple"
 
-    def operation(self, db_alias):
+    def operation(self):
         raise NotImplementedError("The `operation` method must be implemented by subclasses.")
 
-    def wrapped_operation(self, db_alias):
+    def wrapped_operation(self):
         logger.info("Running operation for migration %s", self.key)
-        self.mark_as_started(db_alias)
+        self.mark_as_started()
         try:
-            self.operation(db_alias)
+            self.operation()
         except Exception as error:
-            self.mark_as_errored(db_alias, error)
+            self.mark_as_errored(error)
         else:
-            self.mark_as_finished(db_alias)
+            self.mark_as_finished()
 
 
 class MapperMigration(BaseMigration):
     """ A migration which calls a function on each object in a queryset. """
 
     backend_method = "run_mapper"
 
-    def get_queryset(self, db_alias):
+    def get_queryset(self):
         """ Returns the Django queryset which is to be mapped over. """
         raise NotImplementedError("The `get_queryset` method must be implemented by subclasses.")
 
-    def operation(self, obj: models.Model, db_alias: str) -> None:
+    def operation(self, obj: models.Model) -> None:
         """ This is what will get called on each model instance in the queryset. """
         raise NotImplementedError("The `operation` method must be implemented by subclasses.")
 
-    def wrapped_operation(self, obj, attempt_uuid, db_alias):
+    def wrapped_operation(self, obj, attempt_uuid):
         """ Call self.operation() on the object, but wrap it to catch any errors and set the
             migration as failed if necessary.
         """
         key = self.key
-        record = record_cache.get_record(self.key, db_alias)
+        record = record_cache.get_record(key)
         if record is None:
             logger.warning(
                 "Migration %s no longer exists in the DB. Skipping processing operation.", key
             )
         elif record.attempt_uuid != attempt_uuid:
             logger.warning(
                 "Migration %s now has attempt %s. Skipping processing operation from attempt %s.",
@@ -220,16 +177,16 @@
             logger.info(
                 "Running operation for migration %s on %s (pk=%r).",
                 key,
                 obj.__class__.__name__,
                 obj.pk,
             )
             try:
-                self.operation(obj, db_alias)
+                self.operation(obj)
             except Exception as error:
                 logger.exception(
                     "Error in migration %s trying to process object %s (pk=%r).",
                     key,
                     obj.__class__.__name__,
                     obj.pk,
                 )
-                self.mark_as_errored(error, db_alias)
+                self.mark_as_errored(error)
```

### Comparing `django-mass-migration-0.2.1/massmigration/models.py` & `django-mass-migration-0.2.9/massmigration/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 # Djangae Migrations
 from .fields import ComputedCharField, ComputedDateTimeField
 from .utils.apps import get_app_label_choices
 from .utils.functional import MemoizedLazyList
 
 
 class MigrationRecord(models.Model):
-    """ Stores a record of a particular migration being applied to the database.
-    The assumption is these models are stored on the same DB the migration has been applied to.
-    """
+    """ Stores a record of a particular migration being applied to the database. """
 
     class Status(models.TextField):
         APPLIED = "APPLIED"
         ERRORED = "ERRORED"
         RUNNING = "RUNNING"
         NOT_RUN = "NOT_RUN"  # Can't be returned by this object, as this object won't exist
```

### Comparing `django-mass-migration-0.2.1/massmigration/record_cache.py` & `django-mass-migration-0.2.9/massmigration/record_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,38 +8,38 @@
 # Mass Migration
 from massmigration.models import MigrationRecord
 
 
 DEFAULT_CACHE_TIMEOUT = 60
 
 
-def get_record(key, db_alias):
+def get_record(key):
     """ Get the MigrationRecord for the given key. This is designed to be called heavily, i.e. for
         every object in a MapperMigration, so the result is cached with a best-effort attempt to
         refresh that cache when the record changes, but with no guarantee of it.
     """
-    cache_key = get_cache_key(key, db_alias)
+    cache_key = get_cache_key(key)
     record = cache.get(cache_key)
     if not record:
         record = MigrationRecord.objects.filter(key=key).first()
         cache.set(cache_key, record, cache_timeout())
     return record
 
 
-def get_cache_key(migration_key, db_alias):
-    return f"massmigration_record:{migration_key}:{db_alias}"
+def get_cache_key(migration_key):
+    return f"massmigration_record:{migration_key}"
 
 
 def cache_timeout():
     return getattr(settings, "MASSMIGRATION_RECORD_CACHE_TIMEOUT", DEFAULT_CACHE_TIMEOUT)
 
 
 def record_post_save(sender, **kwargs):
     """ Update the cache when a MigrationRecord is changed (the relevant scenarios being when it's
         marked as started, marked as errored or marked as finished).
     """
     record = kwargs["instance"]
-    cache_key = get_cache_key(record.key, record._state.db)
+    cache_key = get_cache_key(record.key)
     cache.set(cache_key, record, cache_timeout())
 
 
 post_save.connect(record_post_save, sender=MigrationRecord)
```

### Comparing `django-mass-migration-0.2.1/massmigration/templates/massmigration/base.html` & `django-mass-migration-0.2.9/massmigration/templates/massmigration/base.html`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.2.1/massmigration/templates/massmigration/delete_migration.html` & `django-mass-migration-0.2.9/massmigration/templates/massmigration/delete_migration.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 {% extends "massmigration/base.html" %}
 
 {% block content %}
 
 <h1>Cancel/Delete Migration</h1>
 <h2>{{migration.key}}</h2>
 <p>{{migration.description}}</p>
-<p>Database: {{db_alias}}</p>
 <p class="pt">
-	This will delete the <em>record</em> for the migration in the '{{db_alias}}' database.
+	This will delete the <em>record</em> for the migration in the database.
 </p>
 <p>
 	Once you have deleted the record, you will be able to run the migration again.
 </p>
 <h3>If your migration might still be running...</h3>
 <p>
 	<strong>For simple migrations</strong>, deleting the migration record does not interrupt the processing of the migration on the backend.
```

### Comparing `django-mass-migration-0.2.1/massmigration/templates/massmigration/manage_migrations.html` & `django-mass-migration-0.2.9/massmigration/templates/massmigration/manage_migrations.html`

 * *Files 25% similar despite different names*

```diff
@@ -2,50 +2,30 @@
 
 {% block content %}
 
 <h1>Migrations</h1>
 <table class="table">
 	<thead>
 		<tr>
-			<th rowspan="2">App</th>
-			<th rowspan="2">Migration</th>
-			<th colspan="{{available_db_aliases|length}}">Database</th>
-		</tr>
-		<tr>
-			{% for db_alias in available_db_aliases %}
-				<th>{{db_alias}}</th>
-			{% endfor %}
+			<th>App</th>
+			<th>Migration</th>
+			<th>Status</th>
+			<th>Actions</th>
 		</tr>
 	</thead>
 	<tbody>
-		{% for migration in migrations %}
-			<tr>
-				<td>{{migration.app_label}}</td>
-				<td>{{migration.name}}</td>
-				{% for db_alias, migration_for_alias in migration.records_map.items %}
-					{% if migration_for_alias.is_allowed_on_db_alias %}
-					 	{% with migration_record=migration_for_alias.record %}
-						<td>
-							<div>
-								<a href="{% url 'massmigration_detail' key=migration.key db_alias=db_alias%}">Detail</a>
-							</div>
-							<div>{% if migration_record %}{{migration_record.status}}{% else %}NOT RUN{% endif %}</div>
-							<div>
-								{% if not migration_record %}
-									<a href="{% url 'massmigration_run' key=migration.key db_alias=db_alias %}">Run...</a>
-								{% else %}
-									<a href="{% url 'massmigration_delete' key=migration.key db_alias=db_alias %}">Delete...</a>
-								{% endif %}
-							</div>
-						</td>
-						{% endwith %}
-					{% else %}
-						<td>Not allowed on DB</td>
-					{% endif %}
-
-				{% endfor %}
-			</tr>
-		{% endfor %}
+	{% for migration in migrations %}
+		<tr>
+			<td>{{migration.app_label}}</td>
+			<td><a href="{% url 'massmigration_detail' key=migration.key %}">{{migration.name}}</a></td>
+			<td>{% if migration.record %}{{migration.record.status}}{% else %}NOT RUN{% endif %}</td>
+			<td>
+				{% if not migration.record %}<a href="{% url 'massmigration_run' key=migration.key %}">Run...</a>
+				{% else %}<a href="{% url 'massmigration_delete' key=migration.key %}">Delete...</a>
+				{% endif %}
+			</td>
+		</tr>
+	{% endfor %}
 	</tbody>
 </table>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,9 @@
 {% extends "massmigration/base.html" %} {% block content %}
 ************ MMiiggrraattiioonnss ************
-AApppp                    MMiiggrraattiioonn         DDaattaabbaassee
-                                         {{{{ddbb__aalliiaass}}}}
-                                         _D_e_t_a_i_l
-                                         {% if migration_record %}{
-                                         {migration_record.status}}
-{                      {                 {% else %}NOT RUN{% endif  Not allowed
-{migration.app_label}} {migration.name}} %}                         on DB
-                                         {% if not migration_record
-                                         %} _R_u_n_._._. {% else %}
-                                         _D_e_l_e_t_e_._._. {% endif %}
+AApppp                    MMiiggrraattiioonn         SSttaattuuss                     AAccttiioonnss
+                                         {% if migration.record %}{ {% if not
+{                      _{                 {migration.record.status}} migration.record
+{migration.app_label}} _{_m_i_g_r_a_t_i_o_n_._n_a_m_e_}_} {% else %}NOT RUN{% endif  %}_R_u_n_._._. {% else
+                                         %}                         %}_D_e_l_e_t_e_._._. {%
+                                                                    endif %}
 {% endblock %}
```

### Comparing `django-mass-migration-0.2.1/massmigration/templates/massmigration/migration_detail.html` & `django-mass-migration-0.2.9/massmigration/templates/massmigration/migration_detail.html`

 * *Files 18% similar despite different names*

```diff
@@ -8,23 +8,19 @@
 <table class="table mt">
 
 	<tr scope="row">
 		<th>Backend</th>
 		<td>{{migration.backend_str}}</td>
 	</tr>
 	<tr scope="row">
-		<th>Database</th>
-		<td>{{db_alias}}</td>
-	</tr>
-	<tr scope="row">
 		<th>Dependencies</th>
 		<td>
 			{% for dependency in dependencies %}
 				<div>
-					<a href="{% url 'massmigration_detail' key=dependency.key db_alias=db_alias %}">{{dependency.key}}</a>
+					<a href="{% url 'massmigration_detail' key=dependency.key %}">{{dependency.key}}</a>
 					({% if dependency.record %}{{dependency.record.status}}{% else %}NOT RUN{% endif %})
 				</div>
 			{% empty %}
 				None
 			{% endfor %}
 		</td>
 	</tr>
@@ -51,13 +47,13 @@
 	<tr scope="row">
 		<th>Last error</th>
 		<td><code>{{record.last_error|default:'-'}}</code></td>
 	</tr>
 </table>
 <h2>Actions</h2>
 <p>
-	{% if not record %}<a href="{% url 'massmigration_run' key=migration.key db_alias=db_alias %}">Run...</a>
-	{% else %}<a href="{% url 'massmigration_delete' key=migration.key db_alias=db_alias %}">Cancel/Delete...</a>
+	{% if not record %}<a href="{% url 'massmigration_run' key=migration.key %}">Run...</a>
+	{% else %}<a href="{% url 'massmigration_delete' key=migration.key %}">Cancel/Delete...</a>
 	{% endif %}
 </p>
 
-{% endblock %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {% extends "massmigration/base.html" %} {% block content %}
 ************ MMiiggrraattiioonn {{{{mmiiggrraattiioonn..kkeeyy}}}} ************
 {{migration.description}}
 BBaacckkeenndd      {{migration.backend_str}}
-DDaattaabbaassee     {{db_alias}}
              {% for dependency in dependencies %}
 DDeeppeennddeenncciieess _{_{_d_e_p_e_n_d_e_n_c_y_._k_e_y_}_} ({% if dependency.record %}{
              {dependency.record.status}}{% else %}NOT RUN{% endif %})
              {% empty %} None {% endfor %}
 SSttaattuuss       {% if record %}{{record.status}}{% else %}NOT RUN{% endif %}
 SSttaarrtteedd aatt   {{record.initiated_at|default:'-'}}
 FFiinniisshheedd aatt  {{record.applied_at|default:'-'}}
```

### Comparing `django-mass-migration-0.2.1/massmigration/templates/migration_templates/custom.py` & `django-mass-migration-0.2.9/massmigration/templates/migration_templates/custom.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,28 +7,22 @@
     # This can be set to make a migration run on a specific backend, rather than the one that's
     # that's specified in the Django settings
     backend: str = None
 
     # For a custom migration, you must set this, and your backend must have this method.
     backend_method: str = NotImplemented
 
-    # This can be set to specify the list of database aliases on which the migration can be applied.
-    # The migration is not forced on a specific DB but rather the `db_alias` for the DB is passed to `launch`
-    # allowing to customise what is retrieved by the migration.
-    # If None the migration can be applied to all databases.
-    allowed_db_aliases: list = None
-
     dependencies = [{% for dependency in dependencies %}
         ("{{dependency.0}}", "{{dependency.1}}"),{% endfor %}
     ]
 
-    def launch(self, db_alias):
-        self.check_dependencies(db_alias)
-        self.mark_as_started(db_alias)
+    def launch(self):
+        self.check_dependencies()
+        self.mark_as_started()
 
         # PUT YOUR CODE HERE.
         # It should defer whatever operation(s) you want to perform to a backend which knows how to
         # perform them.
-        # When done, or when an error occurs, the backend must call mark_as_finished(db_alias) or
-        # mark_as_errored_(db_alias) on this object as appropriate.
+        # When done, or when an error occurs, the backend must call mark_as_finished() or
+        # mark_as_errored_() on this object as appropriate.
 
         raise NotImplementedError
```

### Comparing `django-mass-migration-0.2.1/massmigration/templates/migration_templates/mapper.py` & `django-mass-migration-0.2.9/massmigration/templates/migration_templates/mapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,19 @@
 class Migration(MapperMigration):
     """ YOUR DESCRIPTION HERE. This will appear in the Django admin. """
 
     # This can be set to make a migration run on a specific backend, rather than the one that's
     # that's specified in the Django settings
     backend: str = None
 
-    # This can be set to specify the list of database aliases on which the migration can be applied.
-    # The migration is not forced on a specific DB but rather the `db_alias` for the DB is passed to `get_queryset`
-    # allowing to customise what is retrieved by the migration.
-    # If None the migration can be applied to all databases.
-    allowed_db_aliases: list = None
-
-
     dependencies = [{% for dependency in dependencies %}
         ("{{dependency.0}}", "{{dependency.1}}"),{% endfor %}
     ]
 
-    def get_queryset(self, db_alias):
+    def get_queryset(self):
 
         # PUT YOUR CODE HERE.
         # It must return a queryset for the objects which you wish to perform the operation on.
 
         raise NotImplementedError
 
     def operation(self, obj):
```

### Comparing `django-mass-migration-0.2.1/massmigration/templates/migration_templates/simple.py` & `django-mass-migration-0.2.9/massmigration/templates/migration_templates/simple.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,25 +4,19 @@
 class Migration(SimpleMigration):
     """ YOUR DESCRIPTION HERE. This will appear in the Django admin. """
 
     # This can be set to make a migration run on a specific backend, rather than the one that's
     # that's specified in the Django settings
     backend: str = None
 
-    # This can be set to specify the list of database aliases on which the migration can be applied.
-    # The migration is not forced on a specific DB but rather the `db_alias` for the DB is passed to `operation`
-    # allowing to customise what is retrieved by the migration.
-    # If None the migration can be applied to all databases.
-    allowed_db_aliases: list = None
-
     dependencies = [{% for dependency in dependencies %}
         ("{{dependency.0}}", "{{dependency.1}}"),{% endfor %}
     ]
 
-    def operation(self, db_alias):
+    def operation(self):
 
         # PUT YOUR CODE HERE.
         # It should perform the entire migration operation in this single step.
         # This must be complete-able within the memory and time limits of the backend.
         # If you cannot perform the operation within a single operation, then you should use the
         # 'mapper' or 'custom' template instead.
```

### Comparing `django-mass-migration-0.2.1/massmigration/utils/functional.py` & `django-mass-migration-0.2.9/massmigration/utils/functional.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.2.1/massmigration/utils/transaction.py` & `django-mass-migration-0.2.9/massmigration/utils/transaction.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,12 +9,13 @@
 
 # TODO: if we want to add true multi-database support (i.e. allow migrations on two different
 # databases within the same project) then we should probably add a `connection_name` attribute to
 # the Migration class and pass that into both here and into .using() calls in various places.
 # That said, should you be allowed to run the same migration on two different databases?
 
 
-def get_transaction(db_alias):
-    engine = settings.DATABASES[db_alias]["ENGINE"]
+def get_transaction():
+    connection = router.db_for_write(MigrationRecord)
+    engine = settings.DATABASES[connection]["ENGINE"]
     if engine == "gcloudc.db.backends.datastore":
         return datastore_transaction
     return django_transaction
```

### Comparing `django-mass-migration-0.2.1/scripts/release.py` & `django-mass-migration-0.2.9/scripts/release.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.2.1/scripts/run_tests_locally.py` & `django-mass-migration-0.2.9/scripts/run_tests_locally.py`

 * *Files identical despite different names*

### Comparing `django-mass-migration-0.2.1/testing/test_settings.py` & `django-mass-migration-0.2.9/testing/test_settings.py`

 * *Files identical despite different names*

