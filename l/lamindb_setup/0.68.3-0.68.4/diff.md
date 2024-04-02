# Comparing `tmp/lamindb_setup-0.68.3.tar.gz` & `tmp/lamindb_setup-0.68.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.68.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.68.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.68.3.tar` & `lamindb_setup-0.68.4.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     8290 2024-03-29 13:22:22.689587 lamindb_setup-0.68.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2024-02-29 20:00:56.143656 lamindb_setup-0.68.3/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-02-29 20:00:56.143718 lamindb_setup-0.68.3/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1219 2024-02-29 20:00:56.143781 lamindb_setup-0.68.3/.gitignore
--rw-r--r--   0        0        0     1931 2024-02-29 20:00:56.143838 lamindb_setup-0.68.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2024-02-29 20:00:56.143925 lamindb_setup-0.68.3/LICENSE
--rw-r--r--   0        0        0      265 2024-02-29 20:00:56.143982 lamindb_setup-0.68.3/README.md
--rw-r--r--   0        0        0    94172 2024-03-30 23:41:21.154382 lamindb_setup-0.68.3/docs/changelog.md
--rw-r--r--   0        0        0     7378 2024-03-07 18:05:18.839544 lamindb_setup-0.68.3/docs/hub-cloud/01-init-on-prem-instance.ipynb
--rw-r--r--   0        0        0     4054 2024-03-07 18:05:18.839906 lamindb_setup-0.68.3/docs/hub-cloud/02-connect-on-prem-instance.ipynb
--rw-r--r--   0        0        0     5812 2024-03-07 18:05:18.840396 lamindb_setup-0.68.3/docs/hub-cloud/03-set-storage.ipynb
--rw-r--r--   0        0        0     3339 2024-03-07 00:06:34.620916 lamindb_setup-0.68.3/docs/hub-cloud/04-test-bionty.ipynb
--rw-r--r--   0        0        0     2450 2024-03-15 16:13:30.315968 lamindb_setup-0.68.3/docs/hub-cloud/05-init-hosted-instance.ipynb
--rw-r--r--   0        0        0     1913 2024-03-15 16:13:30.316560 lamindb_setup-0.68.3/docs/hub-cloud/06-connect-hosted-instance.ipynb
--rw-r--r--   0        0        0     3160 2024-03-07 16:07:21.923709 lamindb_setup-0.68.3/docs/hub-cloud/test-multi-session.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.621529 lamindb_setup-0.68.3/docs/hub-cloud/test_notebooks.py
--rw-r--r--   0        0        0     6105 2024-03-07 18:05:18.841099 lamindb_setup-0.68.3/docs/hub-prod/test-cache-management.ipynb
--rw-r--r--   0        0        0    11402 2024-03-26 10:01:31.777978 lamindb_setup-0.68.3/docs/hub-prod/test-cloud-sync.ipynb
--rw-r--r--   0        0        0     1595 2024-03-18 14:07:20.594957 lamindb_setup-0.68.3/docs/hub-prod/test-connect-anonymously.ipynb
--rw-r--r--   0        0        0     2706 2024-03-07 00:06:34.621901 lamindb_setup-0.68.3/docs/hub-prod/test-empty-init.ipynb
--rw-r--r--   0        0        0     2681 2024-03-09 06:05:04.471802 lamindb_setup-0.68.3/docs/hub-prod/test-import-schema.ipynb
--rw-r--r--   0        0        0     4394 2024-03-07 00:06:34.622152 lamindb_setup-0.68.3/docs/hub-prod/test-insufficient-user-info.ipynb
--rw-r--r--   0        0        0      994 2024-03-07 00:06:34.622232 lamindb_setup-0.68.3/docs/hub-prod/test-invalid-schema.ipynb
--rw-r--r--   0        0        0     6181 2024-03-22 15:00:34.131177 lamindb_setup-0.68.3/docs/hub-prod/test-sqlite-lock.ipynb
--rw-r--r--   0        0        0      142 2024-03-07 00:06:34.622645 lamindb_setup-0.68.3/docs/hub-prod/test_notebooks2.py
--rw-r--r--   0        0        0      120 2024-02-29 20:00:56.144347 lamindb_setup-0.68.3/docs/index.md
--rw-r--r--   0        0        0      486 2024-03-26 10:01:31.778544 lamindb_setup-0.68.3/docs/notebooks.md
--rw-r--r--   0        0        0       61 2024-02-29 20:00:56.145725 lamindb_setup-0.68.3/docs/reference.md
--rw-r--r--   0        0        0     1558 2024-03-31 00:35:59.620985 lamindb_setup-0.68.3/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     1802 2024-03-29 23:29:05.334743 lamindb_setup-0.68.3/lamindb_setup/_add_remote_storage.py
--rw-r--r--   0        0        0      809 2024-02-29 20:00:56.145929 lamindb_setup-0.68.3/lamindb_setup/_cache.py
--rw-r--r--   0        0        0       92 2024-02-29 20:00:56.145990 lamindb_setup-0.68.3/lamindb_setup/_check.py
--rw-r--r--   0        0        0     2543 2024-03-08 11:38:29.530179 lamindb_setup-0.68.3/lamindb_setup/_check_setup.py
--rw-r--r--   0        0        0     1150 2024-03-06 12:44:01.598158 lamindb_setup-0.68.3/lamindb_setup/_close.py
--rw-r--r--   0        0        0    10793 2024-03-30 23:41:21.159941 lamindb_setup-0.68.3/lamindb_setup/_connect_instance.py
--rw-r--r--   0        0        0     3111 2024-03-22 15:00:34.131907 lamindb_setup-0.68.3/lamindb_setup/_delete.py
--rw-r--r--   0        0        0     1500 2024-03-06 12:44:01.598969 lamindb_setup-0.68.3/lamindb_setup/_django.py
--rw-r--r--   0        0        0     2052 2024-03-09 06:05:04.472107 lamindb_setup-0.68.3/lamindb_setup/_exportdb.py
--rw-r--r--   0        0        0     1788 2024-02-29 20:00:56.146417 lamindb_setup-0.68.3/lamindb_setup/_importdb.py
--rw-r--r--   0        0        0    11400 2024-03-29 23:29:05.334965 lamindb_setup-0.68.3/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     7356 2024-03-08 11:38:29.531124 lamindb_setup-0.68.3/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0      795 2024-03-08 11:38:29.531409 lamindb_setup-0.68.3/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0      642 2024-03-08 11:38:29.531579 lamindb_setup-0.68.3/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     3657 2024-03-29 23:29:05.335131 lamindb_setup-0.68.3/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0     1548 2024-02-29 20:00:56.147217 lamindb_setup-0.68.3/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      490 2024-03-05 11:00:49.974555 lamindb_setup-0.68.3/lamindb_setup/core/__init__.py
--rw-r--r--   0        0        0     2403 2024-03-05 09:37:50.121079 lamindb_setup-0.68.3/lamindb_setup/core/_aws_storage.py
--rw-r--r--   0        0        0     2491 2024-03-05 09:37:50.121160 lamindb_setup-0.68.3/lamindb_setup/core/_deprecated.py
--rw-r--r--   0        0        0      240 2024-03-05 09:37:50.121230 lamindb_setup-0.68.3/lamindb_setup/core/_docs.py
--rw-r--r--   0        0        0     5215 2024-03-17 22:17:13.346585 lamindb_setup-0.68.3/lamindb_setup/core/_hub_client.py
--rw-r--r--   0        0        0    11678 2024-03-29 09:14:09.554146 lamindb_setup-0.68.3/lamindb_setup/core/_hub_core.py
--rw-r--r--   0        0        0     4505 2024-03-29 23:01:12.640293 lamindb_setup-0.68.3/lamindb_setup/core/_hub_crud.py
--rw-r--r--   0        0        0     1862 2024-03-05 09:37:50.121645 lamindb_setup-0.68.3/lamindb_setup/core/_hub_utils.py
--rw-r--r--   0        0        0     3241 2024-03-14 13:29:19.826564 lamindb_setup-0.68.3/lamindb_setup/core/_settings.py
--rw-r--r--   0        0        0    11565 2024-03-14 17:58:31.758814 lamindb_setup-0.68.3/lamindb_setup/core/_settings_instance.py
--rw-r--r--   0        0        0     3744 2024-03-14 17:58:31.759147 lamindb_setup-0.68.3/lamindb_setup/core/_settings_load.py
--rw-r--r--   0        0        0     2563 2024-03-18 14:07:20.595611 lamindb_setup-0.68.3/lamindb_setup/core/_settings_save.py
--rw-r--r--   0        0        0    11630 2024-03-22 15:00:34.133398 lamindb_setup-0.68.3/lamindb_setup/core/_settings_storage.py
--rw-r--r--   0        0        0     1929 2024-03-14 17:58:31.759632 lamindb_setup-0.68.3/lamindb_setup/core/_settings_store.py
--rw-r--r--   0        0        0     1281 2024-03-07 18:05:18.845546 lamindb_setup-0.68.3/lamindb_setup/core/_settings_user.py
--rw-r--r--   0        0        0     2908 2024-03-05 09:37:50.122398 lamindb_setup-0.68.3/lamindb_setup/core/_setup_bionty_sources.py
--rw-r--r--   0        0        0     6835 2024-03-26 10:01:31.779365 lamindb_setup-0.68.3/lamindb_setup/core/cloud_sqlite_locker.py
--rw-r--r--   0        0        0     7291 2024-03-05 09:37:50.122604 lamindb_setup-0.68.3/lamindb_setup/core/django.py
--rw-r--r--   0        0        0      275 2024-03-08 11:38:29.532093 lamindb_setup-0.68.3/lamindb_setup/core/exceptions.py
--rw-r--r--   0        0        0     2011 2024-03-12 21:48:08.236470 lamindb_setup-0.68.3/lamindb_setup/core/hashing.py
--rw-r--r--   0        0        0      308 2024-03-05 11:00:49.975018 lamindb_setup-0.68.3/lamindb_setup/core/types.py
--rw-r--r--   0        0        0    22778 2024-03-31 00:17:31.866872 lamindb_setup-0.68.3/lamindb_setup/core/upath.py
--rw-r--r--   0        0        0     4154 2024-03-26 15:38:38.001047 lamindb_setup-0.68.3/noxfile.py
--rw-r--r--   0        0        0      992 2024-03-26 10:01:31.780237 lamindb_setup-0.68.3/pyproject.toml
--rw-r--r--   0        0        0     5492 2024-03-29 23:10:03.082274 lamindb_setup-0.68.3/tests/hub-cloud/test_connect_instance.py
--rw-r--r--   0        0        0      285 2024-03-07 00:06:34.623314 lamindb_setup-0.68.3/tests/hub-cloud/test_delete_instance.py
--rw-r--r--   0        0        0     7021 2024-03-07 01:53:25.975859 lamindb_setup-0.68.3/tests/hub-cloud/test_init_instance.py
--rw-r--r--   0        0        0      502 2024-03-07 00:06:34.623653 lamindb_setup-0.68.3/tests/hub-cloud/test_login.py
--rw-r--r--   0        0        0      469 2024-03-07 00:06:34.623714 lamindb_setup-0.68.3/tests/hub-cloud/test_migrate.py
--rw-r--r--   0        0        0      338 2024-03-07 18:05:18.846365 lamindb_setup-0.68.3/tests/hub-cloud/test_set_storage.py
--rw-r--r--   0        0        0     2784 2024-03-22 15:00:34.134178 lamindb_setup-0.68.3/tests/hub-local/conftest.py
--rw-r--r--   0        0        0    11280 2024-03-29 23:01:12.640680 lamindb_setup-0.68.3/tests/hub-local/test_all.py
--rw-r--r--   0        0        0     1361 2024-03-22 15:00:34.134342 lamindb_setup-0.68.3/tests/hub-local/test_check_s3_storage_empty.py
--rw-r--r--   0        0        0     1149 2024-03-22 15:00:34.134525 lamindb_setup-0.68.3/tests/hub-local/test_hosted_instance_deletion_gate.py
--rw-r--r--   0        0        0      452 2024-03-07 00:06:34.623879 lamindb_setup-0.68.3/tests/hub-prod/conftest.py
--rw-r--r--   0        0        0      365 2024-03-07 18:05:18.846587 lamindb_setup-0.68.3/tests/hub-prod/test_auto_connect.py
--rw-r--r--   0        0        0      285 2024-03-07 00:06:34.624007 lamindb_setup-0.68.3/tests/hub-prod/test_django.py
--rw-r--r--   0        0        0     1438 2024-03-07 01:53:25.976258 lamindb_setup-0.68.3/tests/hub-prod/test_switch_and_fallback_env.py
--rw-r--r--   0        0        0      595 2024-03-07 00:06:34.624340 lamindb_setup-0.68.3/tests/hub-prod/test_upath.py
--rw-r--r--   0        0        0     1411 2024-03-12 21:17:07.347266 lamindb_setup-0.68.3/tests/storage/test_hashing.py
--rw-r--r--   0        0        0     1985 2024-03-07 18:05:18.846898 lamindb_setup-0.68.3/tests/storage/test_storage_access.py
--rw-r--r--   0        0        0      787 2024-03-28 20:35:14.618464 lamindb_setup-0.68.3/tests/storage/test_storage_basis.py
--rw-r--r--   0        0        0      842 2024-03-26 15:38:38.001397 lamindb_setup-0.68.3/tests/storage/test_storage_stats.py
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.68.3/PKG-INFO
+-rw-r--r--   0        0        0     8290 2024-03-25 10:01:42.201467 lamindb_setup-0.68.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2024-02-29 12:04:01.937708 lamindb_setup-0.68.4/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-02-29 12:04:01.937784 lamindb_setup-0.68.4/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1219 2024-02-29 12:04:01.937868 lamindb_setup-0.68.4/.gitignore
+-rw-r--r--   0        0        0     1931 2024-02-29 12:04:01.937945 lamindb_setup-0.68.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2024-02-29 12:04:01.938089 lamindb_setup-0.68.4/LICENSE
+-rw-r--r--   0        0        0      265 2024-02-29 12:04:01.938164 lamindb_setup-0.68.4/README.md
+-rw-r--r--   0        0        0    94332 2024-04-02 10:03:30.862359 lamindb_setup-0.68.4/docs/changelog.md
+-rw-r--r--   0        0        0     7378 2024-03-07 19:17:51.102161 lamindb_setup-0.68.4/docs/hub-cloud/01-init-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     4054 2024-03-07 19:17:51.102263 lamindb_setup-0.68.4/docs/hub-cloud/02-connect-on-prem-instance.ipynb
+-rw-r--r--   0        0        0     5812 2024-03-07 19:17:51.102405 lamindb_setup-0.68.4/docs/hub-cloud/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3339 2024-03-07 19:17:51.102702 lamindb_setup-0.68.4/docs/hub-cloud/04-test-bionty.ipynb
+-rw-r--r--   0        0        0     2450 2024-03-18 09:44:23.350309 lamindb_setup-0.68.4/docs/hub-cloud/05-init-hosted-instance.ipynb
+-rw-r--r--   0        0        0     1913 2024-03-18 09:44:23.350808 lamindb_setup-0.68.4/docs/hub-cloud/06-connect-hosted-instance.ipynb
+-rw-r--r--   0        0        0     3160 2024-03-07 19:17:51.103066 lamindb_setup-0.68.4/docs/hub-cloud/test-multi-session.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 19:17:51.103305 lamindb_setup-0.68.4/docs/hub-cloud/test_notebooks.py
+-rw-r--r--   0        0        0     6105 2024-03-07 19:17:51.103480 lamindb_setup-0.68.4/docs/hub-prod/test-cache-management.ipynb
+-rw-r--r--   0        0        0    11402 2024-03-25 10:01:42.202871 lamindb_setup-0.68.4/docs/hub-prod/test-cloud-sync.ipynb
+-rw-r--r--   0        0        0     1595 2024-03-19 12:58:36.468528 lamindb_setup-0.68.4/docs/hub-prod/test-connect-anonymously.ipynb
+-rw-r--r--   0        0        0     2706 2024-03-07 19:17:51.103712 lamindb_setup-0.68.4/docs/hub-prod/test-empty-init.ipynb
+-rw-r--r--   0        0        0     2681 2024-03-11 10:42:56.000471 lamindb_setup-0.68.4/docs/hub-prod/test-import-schema.ipynb
+-rw-r--r--   0        0        0     4394 2024-03-07 19:17:51.104281 lamindb_setup-0.68.4/docs/hub-prod/test-insufficient-user-info.ipynb
+-rw-r--r--   0        0        0      994 2024-03-07 19:17:51.104386 lamindb_setup-0.68.4/docs/hub-prod/test-invalid-schema.ipynb
+-rw-r--r--   0        0        0     6181 2024-03-25 10:01:42.203244 lamindb_setup-0.68.4/docs/hub-prod/test-sqlite-lock.ipynb
+-rw-r--r--   0        0        0      142 2024-03-07 19:17:51.104771 lamindb_setup-0.68.4/docs/hub-prod/test_notebooks2.py
+-rw-r--r--   0        0        0      120 2024-02-29 12:04:01.938771 lamindb_setup-0.68.4/docs/index.md
+-rw-r--r--   0        0        0      486 2024-03-25 10:01:42.203809 lamindb_setup-0.68.4/docs/notebooks.md
+-rw-r--r--   0        0        0       61 2024-02-29 12:04:01.940681 lamindb_setup-0.68.4/docs/reference.md
+-rw-r--r--   0        0        0     1558 2024-04-02 10:07:21.849290 lamindb_setup-0.68.4/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     1802 2024-03-07 19:17:51.105223 lamindb_setup-0.68.4/lamindb_setup/_add_remote_storage.py
+-rw-r--r--   0        0        0      809 2024-02-29 12:04:01.940876 lamindb_setup-0.68.4/lamindb_setup/_cache.py
+-rw-r--r--   0        0        0       92 2024-02-29 12:04:01.940945 lamindb_setup-0.68.4/lamindb_setup/_check.py
+-rw-r--r--   0        0        0     2543 2024-03-08 11:38:18.119868 lamindb_setup-0.68.4/lamindb_setup/_check_setup.py
+-rw-r--r--   0        0        0     1150 2024-03-06 12:58:52.546246 lamindb_setup-0.68.4/lamindb_setup/_close.py
+-rw-r--r--   0        0        0    10793 2024-03-31 10:37:31.609599 lamindb_setup-0.68.4/lamindb_setup/_connect_instance.py
+-rw-r--r--   0        0        0     3111 2024-03-25 10:01:42.204138 lamindb_setup-0.68.4/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0     1500 2024-03-06 12:58:52.546552 lamindb_setup-0.68.4/lamindb_setup/_django.py
+-rw-r--r--   0        0        0     2052 2024-03-11 10:42:56.001304 lamindb_setup-0.68.4/lamindb_setup/_exportdb.py
+-rw-r--r--   0        0        0     1788 2024-02-29 12:04:01.941670 lamindb_setup-0.68.4/lamindb_setup/_importdb.py
+-rw-r--r--   0        0        0    11400 2024-03-18 09:44:23.352303 lamindb_setup-0.68.4/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     7356 2024-03-08 11:38:18.122077 lamindb_setup-0.68.4/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0      795 2024-03-08 11:38:18.122391 lamindb_setup-0.68.4/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0      642 2024-03-08 11:38:18.122834 lamindb_setup-0.68.4/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     3657 2024-03-08 11:38:18.123112 lamindb_setup-0.68.4/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0     1548 2024-02-29 12:04:01.943026 lamindb_setup-0.68.4/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      490 2024-03-05 13:11:55.176273 lamindb_setup-0.68.4/lamindb_setup/core/__init__.py
+-rw-r--r--   0        0        0     2403 2024-03-05 13:11:55.176381 lamindb_setup-0.68.4/lamindb_setup/core/_aws_storage.py
+-rw-r--r--   0        0        0     2491 2024-03-05 13:11:55.176469 lamindb_setup-0.68.4/lamindb_setup/core/_deprecated.py
+-rw-r--r--   0        0        0      240 2024-03-05 13:11:55.176553 lamindb_setup-0.68.4/lamindb_setup/core/_docs.py
+-rw-r--r--   0        0        0     5215 2024-03-18 09:44:23.353370 lamindb_setup-0.68.4/lamindb_setup/core/_hub_client.py
+-rw-r--r--   0        0        0    11678 2024-03-25 10:01:42.204862 lamindb_setup-0.68.4/lamindb_setup/core/_hub_core.py
+-rw-r--r--   0        0        0     4505 2024-03-30 00:19:04.886366 lamindb_setup-0.68.4/lamindb_setup/core/_hub_crud.py
+-rw-r--r--   0        0        0     1862 2024-03-05 13:11:55.177328 lamindb_setup-0.68.4/lamindb_setup/core/_hub_utils.py
+-rw-r--r--   0        0        0     3241 2024-03-07 19:17:51.107799 lamindb_setup-0.68.4/lamindb_setup/core/_settings.py
+-rw-r--r--   0        0        0    11565 2024-03-18 09:44:23.355474 lamindb_setup-0.68.4/lamindb_setup/core/_settings_instance.py
+-rw-r--r--   0        0        0     3744 2024-03-18 09:44:23.355731 lamindb_setup-0.68.4/lamindb_setup/core/_settings_load.py
+-rw-r--r--   0        0        0     2563 2024-03-19 12:58:36.469141 lamindb_setup-0.68.4/lamindb_setup/core/_settings_save.py
+-rw-r--r--   0        0        0    11630 2024-03-25 10:01:42.206363 lamindb_setup-0.68.4/lamindb_setup/core/_settings_storage.py
+-rw-r--r--   0        0        0     1929 2024-03-18 09:44:23.356020 lamindb_setup-0.68.4/lamindb_setup/core/_settings_store.py
+-rw-r--r--   0        0        0     1281 2024-03-07 19:17:51.107921 lamindb_setup-0.68.4/lamindb_setup/core/_settings_user.py
+-rw-r--r--   0        0        0     2908 2024-03-05 13:11:55.178221 lamindb_setup-0.68.4/lamindb_setup/core/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     6835 2024-03-25 10:01:42.207152 lamindb_setup-0.68.4/lamindb_setup/core/cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     7291 2024-03-05 13:11:55.178538 lamindb_setup-0.68.4/lamindb_setup/core/django.py
+-rw-r--r--   0        0        0      275 2024-03-08 11:38:18.123347 lamindb_setup-0.68.4/lamindb_setup/core/exceptions.py
+-rw-r--r--   0        0        0     2011 2024-03-13 12:19:51.326372 lamindb_setup-0.68.4/lamindb_setup/core/hashing.py
+-rw-r--r--   0        0        0      308 2024-03-05 13:11:55.178881 lamindb_setup-0.68.4/lamindb_setup/core/types.py
+-rw-r--r--   0        0        0    22778 2024-04-02 09:56:45.661778 lamindb_setup-0.68.4/lamindb_setup/core/upath.py
+-rw-r--r--   0        0        0     4154 2024-03-28 07:58:04.166969 lamindb_setup-0.68.4/noxfile.py
+-rw-r--r--   0        0        0      992 2024-03-25 10:01:42.208566 lamindb_setup-0.68.4/pyproject.toml
+-rw-r--r--   0        0        0     5492 2024-03-30 00:19:04.887726 lamindb_setup-0.68.4/tests/hub-cloud/test_connect_instance.py
+-rw-r--r--   0        0        0      285 2024-03-07 19:17:51.108726 lamindb_setup-0.68.4/tests/hub-cloud/test_delete_instance.py
+-rw-r--r--   0        0        0     7021 2024-03-07 19:17:51.108857 lamindb_setup-0.68.4/tests/hub-cloud/test_init_instance.py
+-rw-r--r--   0        0        0      502 2024-03-07 19:17:51.108930 lamindb_setup-0.68.4/tests/hub-cloud/test_login.py
+-rw-r--r--   0        0        0      469 2024-03-07 19:17:51.109001 lamindb_setup-0.68.4/tests/hub-cloud/test_migrate.py
+-rw-r--r--   0        0        0      338 2024-03-07 19:17:51.109074 lamindb_setup-0.68.4/tests/hub-cloud/test_set_storage.py
+-rw-r--r--   0        0        0     2784 2024-03-25 10:01:42.208907 lamindb_setup-0.68.4/tests/hub-local/conftest.py
+-rw-r--r--   0        0        0    11280 2024-03-30 00:19:04.888386 lamindb_setup-0.68.4/tests/hub-local/test_all.py
+-rw-r--r--   0        0        0     1361 2024-03-25 10:01:42.209150 lamindb_setup-0.68.4/tests/hub-local/test_check_s3_storage_empty.py
+-rw-r--r--   0        0        0     1149 2024-03-25 10:01:42.209500 lamindb_setup-0.68.4/tests/hub-local/test_hosted_instance_deletion_gate.py
+-rw-r--r--   0        0        0      452 2024-03-07 19:17:51.109676 lamindb_setup-0.68.4/tests/hub-prod/conftest.py
+-rw-r--r--   0        0        0      365 2024-03-07 19:17:51.109750 lamindb_setup-0.68.4/tests/hub-prod/test_auto_connect.py
+-rw-r--r--   0        0        0      285 2024-03-07 19:17:51.110002 lamindb_setup-0.68.4/tests/hub-prod/test_django.py
+-rw-r--r--   0        0        0     1438 2024-03-07 19:17:51.110099 lamindb_setup-0.68.4/tests/hub-prod/test_switch_and_fallback_env.py
+-rw-r--r--   0        0        0      595 2024-03-07 19:17:51.110379 lamindb_setup-0.68.4/tests/hub-prod/test_upath.py
+-rw-r--r--   0        0        0     1411 2024-03-13 12:19:51.328202 lamindb_setup-0.68.4/tests/storage/test_hashing.py
+-rw-r--r--   0        0        0     1985 2024-03-07 19:17:51.110769 lamindb_setup-0.68.4/tests/storage/test_storage_access.py
+-rw-r--r--   0        0        0      787 2024-03-30 00:19:04.888658 lamindb_setup-0.68.4/tests/storage/test_storage_basis.py
+-rw-r--r--   0        0        0      842 2024-03-28 07:58:04.167485 lamindb_setup-0.68.4/tests/storage/test_storage_stats.py
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 lamindb_setup-0.68.4/PKG-INFO
```

### Comparing `lamindb_setup-0.68.3/.github/workflows/build.yml` & `lamindb_setup-0.68.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/.github/workflows/latest-changes.yml` & `lamindb_setup-0.68.4/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/.gitignore` & `lamindb_setup-0.68.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/.pre-commit-config.yaml` & `lamindb_setup-0.68.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/LICENSE` & `lamindb_setup-0.68.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/changelog.md` & `lamindb_setup-0.68.4/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚑️ Temp fix for non-hosted buckets | [700](https://github.com/laminlabs/lamindb-setup/pull/700) | [sunnyosun](https://github.com/sunnyosun) | 2024-04-02 |
 🍱 Add the scverse spatial hackathon bucket | [699](https://github.com/laminlabs/lamindb-setup/pull/699) | [falexwolf](https://github.com/falexwolf) | 2024-03-30 |
 ♻️ More fine-grained db credentials management | [698](https://github.com/laminlabs/lamindb-setup/pull/698) | [falexwolf](https://github.com/falexwolf) | 2024-03-29 | 0.68.2
 ✨ `upath.to_url()` | [695](https://github.com/laminlabs/lamindb-setup/pull/695) | [falexwolf](https://github.com/falexwolf) | 2024-03-28 |
 ♻️ Enable to choose skip_suffixes | [693](https://github.com/laminlabs/lamindb-setup/pull/693) | [falexwolf](https://github.com/falexwolf) | 2024-03-27 | 0.68.1
 ♻️ Refactor GCP compat | [692](https://github.com/laminlabs/lamindb-setup/pull/692) | [falexwolf](https://github.com/falexwolf) | 2024-03-26 |
 ✨ Rework synchronize, support directories | [687](https://github.com/laminlabs/lamindb-setup/pull/687) | [Koncopd](https://github.com/Koncopd) | 2024-03-23 | 0.68.0
 🎨 Refactor `delete_instance_by_id` and `delete_instance_by_slug` | [691](https://github.com/laminlabs/lamindb-setup/pull/691) | [bpenteado](https://github.com/bpenteado) | 2024-03-20 |
```

### Comparing `lamindb_setup-0.68.3/docs/hub-cloud/01-init-on-prem-instance.ipynb` & `lamindb_setup-0.68.4/docs/hub-cloud/01-init-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-cloud/02-connect-on-prem-instance.ipynb` & `lamindb_setup-0.68.4/docs/hub-cloud/02-connect-on-prem-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-cloud/03-set-storage.ipynb` & `lamindb_setup-0.68.4/docs/hub-cloud/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-cloud/04-test-bionty.ipynb` & `lamindb_setup-0.68.4/docs/hub-cloud/04-test-bionty.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-cloud/05-init-hosted-instance.ipynb` & `lamindb_setup-0.68.4/docs/hub-cloud/05-init-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-cloud/06-connect-hosted-instance.ipynb` & `lamindb_setup-0.68.4/docs/hub-cloud/06-connect-hosted-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-cloud/test-multi-session.ipynb` & `lamindb_setup-0.68.4/docs/hub-cloud/test-multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-prod/test-cache-management.ipynb` & `lamindb_setup-0.68.4/docs/hub-prod/test-cache-management.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-prod/test-cloud-sync.ipynb` & `lamindb_setup-0.68.4/docs/hub-prod/test-cloud-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-prod/test-connect-anonymously.ipynb` & `lamindb_setup-0.68.4/docs/hub-prod/test-connect-anonymously.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-prod/test-empty-init.ipynb` & `lamindb_setup-0.68.4/docs/hub-prod/test-empty-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-prod/test-import-schema.ipynb` & `lamindb_setup-0.68.4/docs/hub-prod/test-import-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-prod/test-insufficient-user-info.ipynb` & `lamindb_setup-0.68.4/docs/hub-prod/test-insufficient-user-info.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-prod/test-invalid-schema.ipynb` & `lamindb_setup-0.68.4/docs/hub-prod/test-invalid-schema.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/docs/hub-prod/test-sqlite-lock.ipynb` & `lamindb_setup-0.68.4/docs/hub-prod/test-sqlite-lock.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/__init__.py` & `lamindb_setup-0.68.4/lamindb_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
    settings
    core
    django
 
 """
 
-__version__ = "0.68.3"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.68.4"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import core
 from ._close import close  # noqa
 from ._delete import delete  # noqa
```

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_add_remote_storage.py` & `lamindb_setup-0.68.4/lamindb_setup/_add_remote_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_cache.py` & `lamindb_setup-0.68.4/lamindb_setup/_cache.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_check_setup.py` & `lamindb_setup-0.68.4/lamindb_setup/_check_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_close.py` & `lamindb_setup-0.68.4/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_connect_instance.py` & `lamindb_setup-0.68.4/lamindb_setup/_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_delete.py` & `lamindb_setup-0.68.4/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_django.py` & `lamindb_setup-0.68.4/lamindb_setup/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_exportdb.py` & `lamindb_setup-0.68.4/lamindb_setup/_exportdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_importdb.py` & `lamindb_setup-0.68.4/lamindb_setup/_importdb.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_init_instance.py` & `lamindb_setup-0.68.4/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_migrate.py` & `lamindb_setup-0.68.4/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_register_instance.py` & `lamindb_setup-0.68.4/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_schema.py` & `lamindb_setup-0.68.4/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_setup_user.py` & `lamindb_setup-0.68.4/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.68.4/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_aws_storage.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_aws_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_deprecated.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_hub_client.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_hub_core.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_hub_core.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_hub_crud.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_hub_crud.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_hub_utils.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_settings.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_settings_instance.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_settings_load.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_settings_save.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_settings_storage.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_settings_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_settings_store.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_settings_user.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/_setup_bionty_sources.py` & `lamindb_setup-0.68.4/lamindb_setup/core/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/cloud_sqlite_locker.py` & `lamindb_setup-0.68.4/lamindb_setup/core/cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/django.py` & `lamindb_setup-0.68.4/lamindb_setup/core/django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/hashing.py` & `lamindb_setup-0.68.4/lamindb_setup/core/hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/lamindb_setup/core/upath.py` & `lamindb_setup-0.68.4/lamindb_setup/core/upath.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,18 +439,17 @@
     Returns:
     - A string containing the public URL to the S3 object.
     """
     if upath.protocol != "s3":
         raise ValueError("The provided UPath must be an S3 path.")
     key = "/".join(upath.parts[1:])
     bucket = upath._url.netloc
-    if (
-        f"s3://{bucket}" not in hosted_buckets
-        or f"s3://{bucket}" == "s3://scverse-spatial-eu-central-1"
-    ):
+    if bucket == "scverse-spatial-eu-central-1":
+        region = "eu-central-1"
+    elif f"s3://{bucket}" not in hosted_buckets:
         metadata = upath.fs.call_s3("head_bucket", Bucket=upath._url.netloc)
         region = metadata["BucketRegion"]
     else:
         region = bucket.replace("lamin_", "")
     if region == "us-east-1":
         return f"https://{bucket}.s3.amazonaws.com/{key}"
     else:
```

### Comparing `lamindb_setup-0.68.3/noxfile.py` & `lamindb_setup-0.68.4/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/pyproject.toml` & `lamindb_setup-0.68.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/hub-cloud/test_connect_instance.py` & `lamindb_setup-0.68.4/tests/hub-cloud/test_connect_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/hub-cloud/test_init_instance.py` & `lamindb_setup-0.68.4/tests/hub-cloud/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/hub-local/conftest.py` & `lamindb_setup-0.68.4/tests/hub-local/conftest.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/hub-local/test_all.py` & `lamindb_setup-0.68.4/tests/hub-local/test_all.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/hub-local/test_check_s3_storage_empty.py` & `lamindb_setup-0.68.4/tests/hub-local/test_check_s3_storage_empty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/hub-local/test_hosted_instance_deletion_gate.py` & `lamindb_setup-0.68.4/tests/hub-local/test_hosted_instance_deletion_gate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/hub-prod/test_switch_and_fallback_env.py` & `lamindb_setup-0.68.4/tests/hub-prod/test_switch_and_fallback_env.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/hub-prod/test_upath.py` & `lamindb_setup-0.68.4/tests/hub-prod/test_upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/storage/test_hashing.py` & `lamindb_setup-0.68.4/tests/storage/test_hashing.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/storage/test_storage_access.py` & `lamindb_setup-0.68.4/tests/storage/test_storage_access.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/storage/test_storage_basis.py` & `lamindb_setup-0.68.4/tests/storage/test_storage_basis.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/tests/storage/test_storage_stats.py` & `lamindb_setup-0.68.4/tests/storage/test_storage_stats.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.68.3/PKG-INFO` & `lamindb_setup-0.68.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.68.3
+Version: 0.68.4
 Summary: Setup & configure LaminDB.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.51.0
 Requires-Dist: lamin_utils>=0.3.3
 Requires-Dist: django>4.2,<5.2.0
 Requires-Dist: dj_database_url>=1.3.0,<3.0.0
```

