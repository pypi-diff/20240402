# Comparing `tmp/dbt-metabase-1.2.1.tar.gz` & `tmp/dbt-metabase-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-metabase-1.2.1.tar", last modified: Sat Mar 30 03:32:46 2024, max compression
+gzip compressed data, was "dbt-metabase-1.3.0.tar", last modified: Tue Apr  2 03:23:08 2024, max compression
```

## Comparing `dbt-metabase-1.2.1.tar` & `dbt-metabase-1.3.0.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.965352 dbt-metabase-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.937353 dbt-metabase-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.941352 dbt-metabase-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/.github/workflows/master.yml
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-03-30 03:32:46.965352 dbt-metabase-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.965352 dbt-metabase-1.2.1/dbt_metabase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-03-30 03:32:46.000000 dbt-metabase-1.2.1/dbt_metabase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-03-30 03:32:46.000000 dbt-metabase-1.2.1/dbt_metabase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 03:32:46.000000 dbt-metabase-1.2.1/dbt_metabase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-30 03:32:46.000000 dbt-metabase-1.2.1/dbt_metabase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-30 03:32:46.000000 dbt-metabase-1.2.1/dbt_metabase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-30 03:32:46.000000 dbt-metabase-1.2.1/dbt_metabase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.945352 dbt-metabase-1.2.1/dbtmetabase/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/dbtmetabase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11257 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/dbtmetabase/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/dbtmetabase/_exposures.py
--rw-r--r--   0 runner    (1001) docker     (127)    17748 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/dbtmetabase/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-30 03:32:46.000000 dbt-metabase-1.2.1/dbtmetabase/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/dbtmetabase/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/dbtmetabase/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/dbtmetabase/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/dbtmetabase/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/dbtmetabase/metabase.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.945352 dbt-metabase-1.2.1/sandbox/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/.env
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/dbt_project.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)     6856 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.945352 dbt-metabase-1.2.1/sandbox/models/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/models/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/models/customers.sql
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/models/orders.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/models/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.945352 dbt-metabase-1.2.1/sandbox/models/staging/
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/models/staging/schema.yml
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/models/staging/stg_customers.sql
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/models/staging/stg_orders.sql
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/models/staging/stg_payments.sql
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.949353 dbt-metabase-1.2.1/sandbox/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/seeds/raw_customers.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/seeds/raw_orders.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/sandbox/seeds/raw_payments.csv
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 03:32:46.965352 dbt-metabase-1.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1541 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.949353 dbt-metabase-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/_mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.949353 dbt-metabase-1.2.1/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.949353 dbt-metabase-1.2.1/tests/fixtures/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.953353 dbt-metabase-1.2.1/tests/fixtures/api/card/
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/10.json
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/11.json
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/12.json
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/13.json
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/14.json
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/15.json
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/16.json
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/17.json
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/2.json
--rw-r--r--   0 runner    (1001) docker     (127)    16081 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/23.json
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/24.json
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/3.json
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/4.json
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/5.json
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/6.json
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/7.json
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/8.json
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card/9.json
--rw-r--r--   0 runner    (1001) docker     (127)   112720 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/card.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.953353 dbt-metabase-1.2.1/tests/fixtures/api/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/collection/1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.953353 dbt-metabase-1.2.1/tests/fixtures/api/collection/2/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/collection/2/items.json
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/collection/2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.953353 dbt-metabase-1.2.1/tests/fixtures/api/collection/3/
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/collection/3/items.json
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/collection/3.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.953353 dbt-metabase-1.2.1/tests/fixtures/api/collection/root/
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/collection/root/items.json
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/collection.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.953353 dbt-metabase-1.2.1/tests/fixtures/api/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)    91893 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/dashboard/1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/dashboard.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.953353 dbt-metabase-1.2.1/tests/fixtures/api/database/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.953353 dbt-metabase-1.2.1/tests/fixtures/api/database/2/
--rw-r--r--   0 runner    (1001) docker     (127)    65455 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/database/2/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/database/2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/database.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.961352 dbt-metabase-1.2.1/tests/fixtures/api/field/
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/37.json
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/38.json
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/39.json
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/40.json
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/41.json
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/42.json
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/43.json
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/44.json
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/45.json
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/46.json
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/47.json
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/48.json
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/49.json
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/50.json
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/51.json
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/52.json
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/53.json
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/54.json
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/55.json
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/56.json
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/57.json
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/58.json
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/59.json
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/60.json
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/61.json
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/62.json
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/63.json
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/65.json
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/68.json
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/69.json
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/72.json
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/field/74.json
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/metric.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.961352 dbt-metabase-1.2.1/tests/fixtures/api/table/
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/table/10.json
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/table/11.json
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/table/12.json
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/table/5.json
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/table/6.json
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/table/7.json
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/table/8.json
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/table/9.json
--rw-r--r--   0 runner    (1001) docker     (127)    17835 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/table.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.961352 dbt-metabase-1.2.1/tests/fixtures/api/user/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/user/1.json
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/api/user.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.941352 dbt-metabase-1.2.1/tests/fixtures/exposure/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.961352 dbt-metabase-1.2.1/tests/fixtures/exposure/collection/
--rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/collection/a_look_at_your_customers_table.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/collection/our_analytics.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.961352 dbt-metabase-1.2.1/tests/fixtures/exposure/default/
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/default/exposures.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.941352 dbt-metabase-1.2.1/tests/fixtures/exposure/type/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.965352 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/1.yml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/11.yml
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/12.yml
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/13.yml
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/14.yml
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/15.yml
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/16.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/17.yml
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/2.yml
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/24.yml
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/3.yml
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/4.yml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/5.yml
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/6.yml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/8.yml
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/9.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 03:32:46.965352 dbt-metabase-1.2.1/tests/fixtures/exposure/type/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/exposure/type/dashboard/1.yml
--rw-r--r--   0 runner    (1001) docker     (127)   437372 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/manifest-v11-disabled.json
--rw-r--r--   0 runner    (1001) docker     (127)   609280 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/manifest-v11.json
--rw-r--r--   0 runner    (1001) docker     (127)   304390 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/manifest-v2.json
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/fixtures/test_dump_yaml.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/test_exposures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/test_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    17634 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/test_metabase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-03-30 03:32:16.000000 dbt-metabase-1.2.1/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.825464 dbt-metabase-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.801464 dbt-metabase-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.805464 dbt-metabase-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/.github/workflows/master.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-02 03:23:08.825464 dbt-metabase-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.825464 dbt-metabase-1.3.0/dbt_metabase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-04-02 03:23:08.000000 dbt-metabase-1.3.0/dbt_metabase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2024-04-02 03:23:08.000000 dbt-metabase-1.3.0/dbt_metabase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:23:08.000000 dbt-metabase-1.3.0/dbt_metabase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 03:23:08.000000 dbt-metabase-1.3.0/dbt_metabase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 03:23:08.000000 dbt-metabase-1.3.0/dbt_metabase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 03:23:08.000000 dbt-metabase-1.3.0/dbt_metabase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.805464 dbt-metabase-1.3.0/dbtmetabase/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/dbtmetabase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11612 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/dbtmetabase/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14876 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/dbtmetabase/_exposures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17748 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/dbtmetabase/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 03:23:08.000000 dbt-metabase-1.3.0/dbtmetabase/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/dbtmetabase/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/dbtmetabase/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/dbtmetabase/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13910 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/dbtmetabase/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/dbtmetabase/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.805464 dbt-metabase-1.3.0/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/.env
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/dbt_project.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6856 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.809464 dbt-metabase-1.3.0/sandbox/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/models/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/models/customers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/models/orders.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/models/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.809464 dbt-metabase-1.3.0/sandbox/models/staging/
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/models/staging/schema.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/models/staging/stg_customers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/models/staging/stg_orders.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/models/staging/stg_payments.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.809464 dbt-metabase-1.3.0/sandbox/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/seeds/raw_customers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/seeds/raw_orders.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/sandbox/seeds/raw_payments.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:23:08.825464 dbt-metabase-1.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1541 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.809464 dbt-metabase-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/_mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.809464 dbt-metabase-1.3.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.813464 dbt-metabase-1.3.0/tests/fixtures/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.813464 dbt-metabase-1.3.0/tests/fixtures/api/card/
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/11.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/12.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/13.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/14.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/15.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/16.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/17.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16081 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/23.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/24.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/8.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card/9.json
+-rw-r--r--   0 runner    (1001) docker     (127)   112720 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/card.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.813464 dbt-metabase-1.3.0/tests/fixtures/api/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/collection/1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.813464 dbt-metabase-1.3.0/tests/fixtures/api/collection/2/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/collection/2/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/collection/2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.817464 dbt-metabase-1.3.0/tests/fixtures/api/collection/3/
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/collection/3/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/collection/3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.817464 dbt-metabase-1.3.0/tests/fixtures/api/collection/root/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/collection/root/items.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/collection.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.817464 dbt-metabase-1.3.0/tests/fixtures/api/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)    91893 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/dashboard/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/dashboard.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.817464 dbt-metabase-1.3.0/tests/fixtures/api/database/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.817464 dbt-metabase-1.3.0/tests/fixtures/api/database/2/
+-rw-r--r--   0 runner    (1001) docker     (127)    65455 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/database/2/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/database/2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/database.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.821464 dbt-metabase-1.3.0/tests/fixtures/api/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/37.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/38.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/39.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/40.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/41.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/42.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/43.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/44.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/45.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/46.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/47.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/48.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/49.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/50.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/51.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/52.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/53.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/54.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/55.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/56.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/57.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/58.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/59.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/60.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/61.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/62.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/63.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/65.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/68.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/69.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/72.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/field/74.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/metric.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.821464 dbt-metabase-1.3.0/tests/fixtures/api/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/table/10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/table/11.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/table/12.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/table/5.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/table/6.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/table/7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/table/8.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/table/9.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17835 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/table.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.821464 dbt-metabase-1.3.0/tests/fixtures/api/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/user/1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/api/user.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.801464 dbt-metabase-1.3.0/tests/fixtures/exposure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.821464 dbt-metabase-1.3.0/tests/fixtures/exposure/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/collection/a_look_at_your_customers_table.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/collection/our_analytics.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.821464 dbt-metabase-1.3.0/tests/fixtures/exposure/default/
+-rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/default/exposures.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.801464 dbt-metabase-1.3.0/tests/fixtures/exposure/type/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.825464 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/11.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/12.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/13.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/14.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/15.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/16.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/17.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/24.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/4.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/5.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/6.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/8.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/9.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:08.825464 dbt-metabase-1.3.0/tests/fixtures/exposure/type/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/exposure/type/dashboard/1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   437372 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/manifest-v11-disabled.json
+-rw-r--r--   0 runner    (1001) docker     (127)   609280 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/manifest-v11.json
+-rw-r--r--   0 runner    (1001) docker     (127)   304390 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/manifest-v2.json
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/fixtures/test_dump_yaml.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/test_exposures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17634 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/test_metabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-02 03:22:45.000000 dbt-metabase-1.3.0/tests/test_models.py
```

### Comparing `dbt-metabase-1.2.1/.github/workflows/codeql-analysis.yml` & `dbt-metabase-1.3.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/.github/workflows/master.yml` & `dbt-metabase-1.3.0/.github/workflows/master.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/.github/workflows/pull_request.yml` & `dbt-metabase-1.3.0/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/.gitignore` & `dbt-metabase-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/CONTRIBUTING.md` & `dbt-metabase-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/LICENSE` & `dbt-metabase-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/Makefile` & `dbt-metabase-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/PKG-INFO` & `dbt-metabase-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-metabase
-Version: 1.2.1
+Version: 1.3.0
 Summary: dbt + Metabase integration.
 Home-page: https://github.com/gouline/dbt-metabase
 Author: Mike Gouline
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -57,14 +57,23 @@
 
 Before running dbt-metabase, you need a compiled `manifest.json` file to parse. These are part of the [dbt artifact](https://docs.getdbt.com/reference/artifacts/dbt-artifacts) generated during compilation.
 
 Once `dbt compile` finishes, `manifest.json` can be found in the `target/` directory of your dbt project.
 
 See [dbt documentation](https://docs.getdbt.com/docs/running-a-dbt-project/run-your-dbt-projects) for more information.
 
+## Metabase API
+
+All commands require authentication against the [Metabase API](https://www.metabase.com/docs/latest/api-documentation) using one of these methods:
+
+* API key (`--metabase-api-key`) 
+  - Strongly **recommended** for automation, see [documentation](https://www.metabase.com/docs/latest/people-and-groups/api-keys) (Metabase 49 or later).
+* Username and password (`--metabase-username` / `--metabase-password`)
+  - Fallback for older versions of Metabase and smaller instances.
+
 ## Exporting Models
 
 Let's start by defining a short sample `schema.yml` as below.
 
 ```yaml
 models:
   - name: stg_users
@@ -102,16 +111,15 @@
 
 This is already enough to propagate the primary keys, foreign keys and descriptions to Metabase:
 
 ```
 dbt-metabase models \
     --manifest-path target/manifest.json \
     --metabase-url https://metabase.example.com \
-    --metabase-username user@example.com \
-    --metabase-password Password123 \
+    --metabase-api-key mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX= \
     --metabase-database business \
     --include-schemas public
 ```
 
 Open Metabase and go to Settings > Admin Settings > Table Metadata, you will notice that `id` column in `stg_users` is now marked as "Entity Key" and `group_id` is a "Foreign Key" pointing to `id` in `stg_groups`.
 
 Try running `dbt-metabase models --help` to see all the options available for fine tuning.
@@ -229,16 +237,15 @@
 
 dbt-metabase allows you to extract questions and dashboards from Metabase as [dbt exposures](https://docs.getdbt.com/docs/building-a-dbt-project/exposures) in your project:
 
 ```
 dbt-metabase exposures \
     --manifest-path ./target/manifest.json \
     --metabase-url https://metabase.example.com \
-    --metabase-username user@example.com \
-    --metabase-password Password123 \
+    --metabase-api-key mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX= \
     --output-path models/ \
     --exclude-collections "temp*"
 ```
 
 Once the execution completes, check your output path for exposures files containing descriptions, creator details and links for Metabase questions and dashboards:
 
 ```yaml
@@ -280,16 +287,15 @@
 
 A configuration file can be created in `~/.dbt-metabase/config.yml` for dbt-metabase to pick it up automatically or anywhere else by specifying `dbt-metabase --config-path path/to/config.yml` (must come **before** the command). Here is an example YAML file:
 
 ```yaml
 config:
     manifest_path: target/manifest.json
     metabase_url: https://metabase.example.com
-    metabase_username: user@example.com
-    metabase_password: Password123
+    metabase_api_key: mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX=
     # Configuration specific to models command
     models:
       metabase_database: business
     # Configuration specific to exposures command
     exposures:
       output_path: models
 ```
@@ -303,16 +309,15 @@
 ```python
 from dbtmetabase import DbtMetabase, Filter
 
 # Initializing instance
 c = DbtMetabase(
     manifest_path="target/manifest.json",
     metabase_url="https://metabase.example.com",
-    metabase_username="user@example.com",
-    metabase_password="Password123",
+    metabase_api_key="mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX=",
 )
 
 # Exporting models
 c.export_models(
     metabase_database="business",
     schema_filter=Filter(include=["public"]),
 )
```

### Comparing `dbt-metabase-1.2.1/README.md` & `dbt-metabase-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,23 @@
 
 Before running dbt-metabase, you need a compiled `manifest.json` file to parse. These are part of the [dbt artifact](https://docs.getdbt.com/reference/artifacts/dbt-artifacts) generated during compilation.
 
 Once `dbt compile` finishes, `manifest.json` can be found in the `target/` directory of your dbt project.
 
 See [dbt documentation](https://docs.getdbt.com/docs/running-a-dbt-project/run-your-dbt-projects) for more information.
 
+## Metabase API
+
+All commands require authentication against the [Metabase API](https://www.metabase.com/docs/latest/api-documentation) using one of these methods:
+
+* API key (`--metabase-api-key`) 
+  - Strongly **recommended** for automation, see [documentation](https://www.metabase.com/docs/latest/people-and-groups/api-keys) (Metabase 49 or later).
+* Username and password (`--metabase-username` / `--metabase-password`)
+  - Fallback for older versions of Metabase and smaller instances.
+
 ## Exporting Models
 
 Let's start by defining a short sample `schema.yml` as below.
 
 ```yaml
 models:
   - name: stg_users
@@ -77,16 +86,15 @@
 
 This is already enough to propagate the primary keys, foreign keys and descriptions to Metabase:
 
 ```
 dbt-metabase models \
     --manifest-path target/manifest.json \
     --metabase-url https://metabase.example.com \
-    --metabase-username user@example.com \
-    --metabase-password Password123 \
+    --metabase-api-key mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX= \
     --metabase-database business \
     --include-schemas public
 ```
 
 Open Metabase and go to Settings > Admin Settings > Table Metadata, you will notice that `id` column in `stg_users` is now marked as "Entity Key" and `group_id` is a "Foreign Key" pointing to `id` in `stg_groups`.
 
 Try running `dbt-metabase models --help` to see all the options available for fine tuning.
@@ -204,16 +212,15 @@
 
 dbt-metabase allows you to extract questions and dashboards from Metabase as [dbt exposures](https://docs.getdbt.com/docs/building-a-dbt-project/exposures) in your project:
 
 ```
 dbt-metabase exposures \
     --manifest-path ./target/manifest.json \
     --metabase-url https://metabase.example.com \
-    --metabase-username user@example.com \
-    --metabase-password Password123 \
+    --metabase-api-key mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX= \
     --output-path models/ \
     --exclude-collections "temp*"
 ```
 
 Once the execution completes, check your output path for exposures files containing descriptions, creator details and links for Metabase questions and dashboards:
 
 ```yaml
@@ -255,16 +262,15 @@
 
 A configuration file can be created in `~/.dbt-metabase/config.yml` for dbt-metabase to pick it up automatically or anywhere else by specifying `dbt-metabase --config-path path/to/config.yml` (must come **before** the command). Here is an example YAML file:
 
 ```yaml
 config:
     manifest_path: target/manifest.json
     metabase_url: https://metabase.example.com
-    metabase_username: user@example.com
-    metabase_password: Password123
+    metabase_api_key: mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX=
     # Configuration specific to models command
     models:
       metabase_database: business
     # Configuration specific to exposures command
     exposures:
       output_path: models
 ```
@@ -278,16 +284,15 @@
 ```python
 from dbtmetabase import DbtMetabase, Filter
 
 # Initializing instance
 c = DbtMetabase(
     manifest_path="target/manifest.json",
     metabase_url="https://metabase.example.com",
-    metabase_username="user@example.com",
-    metabase_password="Password123",
+    metabase_api_key="mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX=",
 )
 
 # Exporting models
 c.export_models(
     metabase_database="business",
     schema_filter=Filter(include=["public"]),
 )
```

### Comparing `dbt-metabase-1.2.1/dbt_metabase.egg-info/PKG-INFO` & `dbt-metabase-1.3.0/dbt_metabase.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-metabase
-Version: 1.2.1
+Version: 1.3.0
 Summary: dbt + Metabase integration.
 Home-page: https://github.com/gouline/dbt-metabase
 Author: Mike Gouline
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -57,14 +57,23 @@
 
 Before running dbt-metabase, you need a compiled `manifest.json` file to parse. These are part of the [dbt artifact](https://docs.getdbt.com/reference/artifacts/dbt-artifacts) generated during compilation.
 
 Once `dbt compile` finishes, `manifest.json` can be found in the `target/` directory of your dbt project.
 
 See [dbt documentation](https://docs.getdbt.com/docs/running-a-dbt-project/run-your-dbt-projects) for more information.
 
+## Metabase API
+
+All commands require authentication against the [Metabase API](https://www.metabase.com/docs/latest/api-documentation) using one of these methods:
+
+* API key (`--metabase-api-key`) 
+  - Strongly **recommended** for automation, see [documentation](https://www.metabase.com/docs/latest/people-and-groups/api-keys) (Metabase 49 or later).
+* Username and password (`--metabase-username` / `--metabase-password`)
+  - Fallback for older versions of Metabase and smaller instances.
+
 ## Exporting Models
 
 Let's start by defining a short sample `schema.yml` as below.
 
 ```yaml
 models:
   - name: stg_users
@@ -102,16 +111,15 @@
 
 This is already enough to propagate the primary keys, foreign keys and descriptions to Metabase:
 
 ```
 dbt-metabase models \
     --manifest-path target/manifest.json \
     --metabase-url https://metabase.example.com \
-    --metabase-username user@example.com \
-    --metabase-password Password123 \
+    --metabase-api-key mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX= \
     --metabase-database business \
     --include-schemas public
 ```
 
 Open Metabase and go to Settings > Admin Settings > Table Metadata, you will notice that `id` column in `stg_users` is now marked as "Entity Key" and `group_id` is a "Foreign Key" pointing to `id` in `stg_groups`.
 
 Try running `dbt-metabase models --help` to see all the options available for fine tuning.
@@ -229,16 +237,15 @@
 
 dbt-metabase allows you to extract questions and dashboards from Metabase as [dbt exposures](https://docs.getdbt.com/docs/building-a-dbt-project/exposures) in your project:
 
 ```
 dbt-metabase exposures \
     --manifest-path ./target/manifest.json \
     --metabase-url https://metabase.example.com \
-    --metabase-username user@example.com \
-    --metabase-password Password123 \
+    --metabase-api-key mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX= \
     --output-path models/ \
     --exclude-collections "temp*"
 ```
 
 Once the execution completes, check your output path for exposures files containing descriptions, creator details and links for Metabase questions and dashboards:
 
 ```yaml
@@ -280,16 +287,15 @@
 
 A configuration file can be created in `~/.dbt-metabase/config.yml` for dbt-metabase to pick it up automatically or anywhere else by specifying `dbt-metabase --config-path path/to/config.yml` (must come **before** the command). Here is an example YAML file:
 
 ```yaml
 config:
     manifest_path: target/manifest.json
     metabase_url: https://metabase.example.com
-    metabase_username: user@example.com
-    metabase_password: Password123
+    metabase_api_key: mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX=
     # Configuration specific to models command
     models:
       metabase_database: business
     # Configuration specific to exposures command
     exposures:
       output_path: models
 ```
@@ -303,16 +309,15 @@
 ```python
 from dbtmetabase import DbtMetabase, Filter
 
 # Initializing instance
 c = DbtMetabase(
     manifest_path="target/manifest.json",
     metabase_url="https://metabase.example.com",
-    metabase_username="user@example.com",
-    metabase_password="Password123",
+    metabase_api_key="mb_XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX=",
 )
 
 # Exporting models
 c.export_models(
     metabase_database="business",
     schema_filter=Filter(include=["public"]),
 )
```

### Comparing `dbt-metabase-1.2.1/dbt_metabase.egg-info/SOURCES.txt` & `dbt-metabase-1.3.0/dbt_metabase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/dbtmetabase/__main__.py` & `dbt-metabase-1.3.0/dbtmetabase/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,36 +92,45 @@
         envvar="METABASE_URL",
         show_envvar=True,
         required=True,
         type=click.STRING,
         help="Metabase URL, e.g. 'https://metabase.example.com'.",
     )
     @click.option(
+        "--metabase-api-key",
+        metavar="API_KEY",
+        envvar="METABASE_API_KEY",
+        show_envvar=True,
+        type=click.STRING,
+        help="Metabase API key (required unless providing username/password).",
+    )
+    @click.option(
         "--metabase-username",
         metavar="USERNAME",
         envvar="METABASE_USERNAME",
         show_envvar=True,
         type=click.STRING,
-        help="Metabase username (required unless providing session ID).",
+        help="Metabase username (required unless providing API key).",
     )
     @click.option(
         "--metabase-password",
         metavar="PASSWORD",
         envvar="METABASE_PASSWORD",
         show_envvar=True,
         type=click.STRING,
-        help="Metabase password (required unless providing session ID).",
+        help="Metabase password (required unless providing API key).",
     )
     @click.option(
         "--metabase-session-id",
         metavar="TOKEN",
         envvar="METABASE_SESSION_ID",
         show_envvar=True,
         type=click.STRING,
-        help="Metabase session ID (alternative to username/password).",
+        help="Metabase session ID (deprecated and will be removed in future).",
+        hidden=True,
     )
     @click.option(
         "--skip-verify",
         envvar="SKIP_VERIFY",
         show_envvar=True,
         help="Skip TLS certificate verification (not recommended).",
     )
@@ -156,14 +165,15 @@
         is_flag=True,
         help="Enable verbose logging.",
     )
     @functools.wraps(func)
     def wrapper(
         manifest_path: str,
         metabase_url: str,
+        metabase_api_key: str,
         metabase_username: str,
         metabase_password: str,
         metabase_session_id: Optional[str],
         skip_verify: bool,
         cert: Optional[str],
         http_timeout: int,
         http_headers: Sequence[Tuple[str, str]],
@@ -175,14 +185,15 @@
             path=Path.home().absolute() / ".dbt-metabase" / "logs" / "dbtmetabase.log",
         )
 
         return func(
             core=DbtMetabase(
                 manifest_path=manifest_path,
                 metabase_url=metabase_url,
+                metabase_api_key=metabase_api_key,
                 metabase_username=metabase_username,
                 metabase_password=metabase_password,
                 metabase_session_id=metabase_session_id,
                 skip_verify=skip_verify,
                 cert=cert,
                 http_timeout=http_timeout,
                 http_headers={k: v for k, v in http_headers},
```

### Comparing `dbt-metabase-1.2.1/dbtmetabase/_exposures.py` & `dbt-metabase-1.3.0/dbtmetabase/_exposures.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/dbtmetabase/_models.py` & `dbt-metabase-1.3.0/dbtmetabase/_models.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/dbtmetabase/core.py` & `dbt-metabase-1.3.0/dbtmetabase/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,43 +19,46 @@
 
     DEFAULT_HTTP_TIMEOUT = 15
 
     def __init__(
         self,
         manifest_path: Union[str, Path],
         metabase_url: str,
+        metabase_api_key: Optional[str] = None,
         metabase_username: Optional[str] = None,
         metabase_password: Optional[str] = None,
         metabase_session_id: Optional[str] = None,
         skip_verify: bool = False,
         cert: Optional[Union[str, Tuple[str, str]]] = None,
         http_timeout: int = DEFAULT_HTTP_TIMEOUT,
         http_headers: Optional[dict] = None,
         http_adapter: Optional[HTTPAdapter] = None,
     ):
         """dbt + Metabase integration.
 
         Args:
             manifest_path (Union[str,Path]): Path to dbt manifest.json, usually in target/ directory after compilation.
             metabase_url (str): Metabase URL, e.g. "https://metabase.example.com".
-            metabase_username (Optional[str], optional): Metabase username (required unless providing session ID). Defaults to None.
-            metabase_password (Optional[str], optional): Metabase password (required unless providing session ID). Defaults to None.
-            metabase_session_id (Optional[str], optional): Metabase session ID. Defaults to None.
+            metabase_api_key (Optional[str], optional): Metabase API key (required unless providing username/password or session ID). Defaults to None.
+            metabase_username (Optional[str], optional): Metabase username (required unless providing API key or session ID). Defaults to None.
+            metabase_password (Optional[str], optional): Metabase password (required unless providing API key or session ID). Defaults to None.
+            metabase_session_id (Optional[str], optional): Metabase session ID (deprecated and will be removed in future). Defaults to None.
             skip_verify (bool, optional): Skip TLS certificate verification (not recommended). Defaults to False.
             cert (Optional[Union[str, Tuple[str, str]]], optional): Path to a custom certificate. Defaults to None.
             http_timeout (int, optional): HTTP request timeout in secs. Defaults to 15.
             http_headers (Optional[dict], optional): Additional HTTP headers. Defaults to None.
             http_adapter (Optional[HTTPAdapter], optional): Custom requests HTTP adapter. Defaults to None.
         """
 
         self._manifest = Manifest(
             path=manifest_path,
         )
         self._metabase = Metabase(
             url=metabase_url,
+            api_key=metabase_api_key,
             username=metabase_username,
             password=metabase_password,
             session_id=metabase_session_id,
             skip_verify=skip_verify,
             cert=cert,
             http_timeout=http_timeout,
             http_headers=http_headers,
```

### Comparing `dbt-metabase-1.2.1/dbtmetabase/format.py` & `dbt-metabase-1.3.0/dbtmetabase/format.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/dbtmetabase/manifest.py` & `dbt-metabase-1.3.0/dbtmetabase/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/dbtmetabase/metabase.py` & `dbt-metabase-1.3.0/dbtmetabase/metabase.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 _logger = logging.getLogger(__name__)
 
 
 class Metabase:
     def __init__(
         self,
         url: str,
+        api_key: Optional[str],
         username: Optional[str],
         password: Optional[str],
         session_id: Optional[str],
         skip_verify: bool,
         cert: Optional[Union[str, Tuple[str, str]]],
         http_timeout: int,
         http_headers: Optional[dict],
@@ -34,27 +35,32 @@
             self.session.headers.update(http_headers)
 
         self.session.mount(
             self.url,
             http_adapter or HTTPAdapter(max_retries=Retry(total=3, backoff_factor=1)),
         )
 
-        if not session_id:
-            if username and password:
-                session = dict(
-                    self._api(
-                        method="post",
-                        path="/api/session",
-                        json={"username": username, "password": password},
-                    )
+        if api_key:
+            self.session.headers["X-API-KEY"] = api_key
+        elif username and password:
+            session = dict(
+                self._api(
+                    method="post",
+                    path="/api/session",
+                    json={"username": username, "password": password},
                 )
-                session_id = str(session["id"])
-            else:
-                raise ArgumentError("Metabase credentials or session ID required")
-        self.session.headers["X-Metabase-Session"] = session_id
+            )
+            self.session.headers["X-Metabase-Session"] = str(session["id"])
+        elif session_id:
+            _logger.warning(
+                "Metabase session ID is deprecated and will be removed in future, use API key or username/password instead"
+            )
+            self.session.headers["X-Metabase-Session"] = session_id
+        else:
+            raise ArgumentError("Metabase API key or username/password required")
 
         _logger.info("Metabase session established")
 
     def _api(
         self,
         method: str,
         path: str,
```

### Comparing `dbt-metabase-1.2.1/sandbox/docker-compose.yml` & `dbt-metabase-1.3.0/sandbox/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/sandbox/entrypoint.py` & `dbt-metabase-1.3.0/sandbox/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/sandbox/models/customers.sql` & `dbt-metabase-1.3.0/sandbox/models/customers.sql`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/sandbox/models/orders.sql` & `dbt-metabase-1.3.0/sandbox/models/orders.sql`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/sandbox/models/schema.yml` & `dbt-metabase-1.3.0/sandbox/models/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/sandbox/models/staging/schema.yml` & `dbt-metabase-1.3.0/sandbox/models/staging/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/sandbox/seeds/raw_customers.csv` & `dbt-metabase-1.3.0/sandbox/seeds/raw_customers.csv`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/sandbox/seeds/raw_orders.csv` & `dbt-metabase-1.3.0/sandbox/seeds/raw_orders.csv`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/sandbox/seeds/raw_payments.csv` & `dbt-metabase-1.3.0/sandbox/seeds/raw_payments.csv`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/setup.py` & `dbt-metabase-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/_mocks.py` & `dbt-metabase-1.3.0/tests/_mocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 TMP_PATH = Path("tests") / "tmp"
 
 
 class MockMetabase(Metabase):
     def __init__(self, url: str):
         super().__init__(
             url=url,
+            api_key=None,
             username=None,
             password=None,
             session_id="dummy",
             skip_verify=False,
             cert=None,
             http_timeout=1,
             http_headers=None,
```

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/1.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/1.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/10.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/10.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/11.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/11.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/12.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/12.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/13.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/13.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/14.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/14.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/15.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/15.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/16.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/16.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/17.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/17.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/2.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/2.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/23.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/23.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/24.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/24.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/3.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/3.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/4.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/4.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/5.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/5.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/6.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/6.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/7.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/7.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/8.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/8.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card/9.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card/9.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/card.json` & `dbt-metabase-1.3.0/tests/fixtures/api/card.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/collection/1.json` & `dbt-metabase-1.3.0/tests/fixtures/api/collection/1.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/collection/2.json` & `dbt-metabase-1.3.0/tests/fixtures/api/collection/2.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/collection/3/items.json` & `dbt-metabase-1.3.0/tests/fixtures/api/collection/3/items.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/collection/3.json` & `dbt-metabase-1.3.0/tests/fixtures/api/collection/3.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/collection/root/items.json` & `dbt-metabase-1.3.0/tests/fixtures/api/collection/root/items.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/collection.json` & `dbt-metabase-1.3.0/tests/fixtures/api/collection.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/dashboard/1.json` & `dbt-metabase-1.3.0/tests/fixtures/api/dashboard/1.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/dashboard.json` & `dbt-metabase-1.3.0/tests/fixtures/api/dashboard.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/database/2/metadata.json` & `dbt-metabase-1.3.0/tests/fixtures/api/database/2/metadata.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/database/2.json` & `dbt-metabase-1.3.0/tests/fixtures/api/database/2.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/database.json` & `dbt-metabase-1.3.0/tests/fixtures/api/database.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/37.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/37.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/38.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/38.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/39.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/39.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/40.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/40.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/41.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/41.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/42.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/42.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/43.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/43.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/44.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/44.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/45.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/45.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/46.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/46.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/47.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/47.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/48.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/48.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/49.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/49.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/50.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/50.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/51.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/51.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/52.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/52.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/53.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/53.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/54.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/54.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/55.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/55.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/56.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/56.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/57.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/57.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/58.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/58.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/59.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/59.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/60.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/60.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/61.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/61.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/62.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/62.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/63.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/63.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/65.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/65.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/68.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/68.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/69.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/69.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/72.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/72.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/field/74.json` & `dbt-metabase-1.3.0/tests/fixtures/api/field/74.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/table/10.json` & `dbt-metabase-1.3.0/tests/fixtures/api/table/10.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/table/11.json` & `dbt-metabase-1.3.0/tests/fixtures/api/table/11.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/table/12.json` & `dbt-metabase-1.3.0/tests/fixtures/api/table/12.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/table/5.json` & `dbt-metabase-1.3.0/tests/fixtures/api/table/5.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/table/6.json` & `dbt-metabase-1.3.0/tests/fixtures/api/table/6.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/table/7.json` & `dbt-metabase-1.3.0/tests/fixtures/api/table/7.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/table/8.json` & `dbt-metabase-1.3.0/tests/fixtures/api/table/8.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/table/9.json` & `dbt-metabase-1.3.0/tests/fixtures/api/table/9.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/table.json` & `dbt-metabase-1.3.0/tests/fixtures/api/table.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/api/user.json` & `dbt-metabase-1.3.0/tests/fixtures/api/user.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/exposure/collection/a_look_at_your_customers_table.yml` & `dbt-metabase-1.3.0/tests/fixtures/exposure/collection/a_look_at_your_customers_table.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/exposure/collection/our_analytics.yml` & `dbt-metabase-1.3.0/tests/fixtures/exposure/collection/our_analytics.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/exposure/default/exposures.yml` & `dbt-metabase-1.3.0/tests/fixtures/exposure/default/exposures.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/exposure/type/card/1.yml` & `dbt-metabase-1.3.0/tests/fixtures/exposure/type/card/1.yml`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/manifest-v11-disabled.json` & `dbt-metabase-1.3.0/tests/fixtures/manifest-v11-disabled.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/manifest-v11.json` & `dbt-metabase-1.3.0/tests/fixtures/manifest-v11.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/fixtures/manifest-v2.json` & `dbt-metabase-1.3.0/tests/fixtures/manifest-v2.json`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/test_exposures.py` & `dbt-metabase-1.3.0/tests/test_exposures.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/test_format.py` & `dbt-metabase-1.3.0/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/test_manifest.py` & `dbt-metabase-1.3.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/test_metabase.py` & `dbt-metabase-1.3.0/tests/test_metabase.py`

 * *Files identical despite different names*

### Comparing `dbt-metabase-1.2.1/tests/test_models.py` & `dbt-metabase-1.3.0/tests/test_models.py`

 * *Files identical despite different names*

