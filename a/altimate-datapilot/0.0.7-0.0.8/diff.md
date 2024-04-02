# Comparing `tmp/altimate-datapilot-0.0.7.tar.gz` & `tmp/altimate-datapilot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altimate-datapilot-0.0.7.tar", last modified: Fri Mar 29 16:57:06 2024, max compression
+gzip compressed data, was "altimate-datapilot-0.0.8.tar", last modified: Tue Apr  2 00:54:47 2024, max compression
```

## Comparing `altimate-datapilot-0.0.7.tar` & `altimate-datapilot-0.0.8.tar`

### file list

```diff
@@ -1,249 +1,249 @@
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.908233 altimate-datapilot-0.0.7/
--rw-r--r--   0 anandgupta   (501) staff       (20)      420 2024-03-29 16:56:44.000000 altimate-datapilot-0.0.7/.bumpversion.cfg
--rw-r--r--   0 anandgupta   (501) staff       (20)     1988 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.7/.cookiecutterrc
--rw-r--r--   0 anandgupta   (501) staff       (20)      149 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/.coveragerc
--rw-r--r--   0 anandgupta   (501) staff       (20)      353 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/.editorconfig
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.850852 altimate-datapilot-0.0.7/.github/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.858161 altimate-datapilot-0.0.7/.github/workflows/
--rw-r--r--   0 anandgupta   (501) staff       (20)    10794 2024-01-25 04:30:47.000000 altimate-datapilot-0.0.7/.github/workflows/github-actions.yml
--rw-r--r--   0 anandgupta   (501) staff       (20)      688 2024-01-30 03:12:39.000000 altimate-datapilot-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 anandgupta   (501) staff       (20)      204 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/.pre-commit-hooks.yaml
--rw-r--r--   0 anandgupta   (501) staff       (20)      282 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/.readthedocs.yml
--rw-r--r--   0 anandgupta   (501) staff       (20)       50 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/AUTHORS.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       86 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/CHANGELOG.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     2332 2024-01-25 04:45:20.000000 altimate-datapilot-0.0.7/CONTRIBUTING.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1100 2024-01-25 04:37:04.000000 altimate-datapilot-0.0.7/LICENSE
--rw-r--r--   0 anandgupta   (501) staff       (20)      495 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/MANIFEST.in
--rw-r--r--   0 anandgupta   (501) staff       (20)     2159 2024-03-29 16:57:06.908082 altimate-datapilot-0.0.7/PKG-INFO
--rw-r--r--   0 anandgupta   (501) staff       (20)    11531 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/README.md
--rw-r--r--   0 anandgupta   (501) staff       (20)     1575 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.7/README.rst
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.858416 altimate-datapilot-0.0.7/ci/
--rwxr-xr-x   0 anandgupta   (501) staff       (20)     2867 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/ci/bootstrap.py
--rw-r--r--   0 anandgupta   (501) staff       (20)       72 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/ci/requirements.txt
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.851179 altimate-datapilot-0.0.7/ci/templates/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.851272 altimate-datapilot-0.0.7/ci/templates/.github/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.858537 altimate-datapilot-0.0.7/ci/templates/.github/workflows/
--rw-r--r--   0 anandgupta   (501) staff       (20)     1965 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/ci/templates/.github/workflows/github-actions.yml
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.863899 altimate-datapilot-0.0.7/docs/
--rw-r--r--   0 anandgupta   (501) staff       (20)       28 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/docs/authors.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       30 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/docs/changelog.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1099 2024-03-29 16:56:44.000000 altimate-datapilot-0.0.7/docs/conf.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2433 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.7/docs/configuration.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       33 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/docs/contributing.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1776 2024-03-09 02:10:20.000000 altimate-datapilot-0.0.7/docs/features.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1635 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/docs/hooks.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)      221 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/docs/index.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)    35144 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/docs/insights.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1084 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.7/docs/installation.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     2361 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.7/docs/introduction.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1926 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/docs/performance.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       27 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/docs/readme.rst
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.864368 altimate-datapilot-0.0.7/docs/reference/
--rw-r--r--   0 anandgupta   (501) staff       (20)      106 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/docs/reference/datapilot.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       61 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/docs/reference/index.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)       29 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.7/docs/requirements.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)      109 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/docs/spelling_wordlist.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)       70 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/docs/usage.rst
--rw-r--r--   0 anandgupta   (501) staff       (20)     1194 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/pyproject.toml
--rw-r--r--   0 anandgupta   (501) staff       (20)      903 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/pytest.ini
--rw-r--r--   0 anandgupta   (501) staff       (20)       38 2024-03-29 16:57:06.910592 altimate-datapilot-0.0.7/setup.cfg
--rwxr-xr-x   0 anandgupta   (501) staff       (20)     3043 2024-03-29 16:56:44.000000 altimate-datapilot-0.0.7/setup.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.851617 altimate-datapilot-0.0.7/src/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.867957 altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/
--rw-r--r--   0 anandgupta   (501) staff       (20)     2159 2024-03-29 16:57:06.000000 altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/PKG-INFO
--rw-r--r--   0 anandgupta   (501) staff       (20)     9717 2024-03-29 16:57:06.000000 altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/SOURCES.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)        1 2024-03-29 16:57:06.000000 altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/dependency_links.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)      141 2024-03-29 16:57:06.000000 altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/entry_points.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)        1 2024-03-29 16:57:04.000000 altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/not-zip-safe
--rw-r--r--   0 anandgupta   (501) staff       (20)      110 2024-03-29 16:57:06.000000 altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/requires.txt
--rw-r--r--   0 anandgupta   (501) staff       (20)       10 2024-03-29 16:57:06.000000 altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/top_level.txt
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.868208 altimate-datapilot-0.0.7/src/datapilot/
--rw-r--r--   0 anandgupta   (501) staff       (20)       22 2024-03-29 16:56:44.000000 altimate-datapilot-0.0.7/src/datapilot/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      380 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/__main__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.868414 altimate-datapilot-0.0.7/src/datapilot/cli/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/cli/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      181 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/cli/main.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.868538 altimate-datapilot-0.0.7/src/datapilot/clients/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.7/src/datapilot/clients/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.868943 altimate-datapilot-0.0.7/src/datapilot/clients/altimate/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.7/src/datapilot/clients/altimate/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3107 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.7/src/datapilot/clients/altimate/client.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2629 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.7/src/datapilot/clients/altimate/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.869276 altimate-datapilot-0.0.7/src/datapilot/config/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/config/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      403 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.7/src/datapilot/config/config.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1146 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/config/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.869404 altimate-datapilot-0.0.7/src/datapilot/core/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.869860 altimate-datapilot-0.0.7/src/datapilot/core/insights/
--rw-r--r--   0 anandgupta   (501) staff       (20)       18 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.870072 altimate-datapilot-0.0.7/src/datapilot/core/insights/base/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/base/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      883 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/base/insight.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      596 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/report.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      413 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/schema.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.870184 altimate-datapilot-0.0.7/src/datapilot/core/insights/sql/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/sql/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.870348 altimate-datapilot-0.0.7/src/datapilot/core/insights/sql/base/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/sql/base/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      471 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/sql/base/insight.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.870466 altimate-datapilot-0.0.7/src/datapilot/core/insights/sql/runtime/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/sql/runtime/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.870553 altimate-datapilot-0.0.7/src/datapilot/core/insights/sql/static/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/sql/static/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      535 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/insights/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.870787 altimate-datapilot-0.0.7/src/datapilot/core/platforms/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.872562 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.873181 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/cli/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/cli/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4146 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/cli/cli.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      502 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/constants.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      110 2024-03-09 02:10:20.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/exceptions.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6562 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/executor.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1095 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/factory.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1638 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/formatting.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.873459 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/hooks/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/hooks/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2966 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/hooks/executor_hook.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.874091 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/
--rw-r--r--   0 anandgupta   (501) staff       (20)     7547 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5260 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/base.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.880406 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      824 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4609 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_column_desc_are_same.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     7222 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_column_name_contract.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3185 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_macro_args_have_desc.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2802 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_macro_has_desc.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4277 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_all_columns.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5183 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_labels_keys.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5016 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_meta_keys.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2968 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_properties_file.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5706 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_group.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5187 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_name.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5590 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_type.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6096 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_materialization_by_childs.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6037 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_name_contract.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6330 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_and_childs.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4889 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_database.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4882 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_schema.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3555 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_tags.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4254 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_childs.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4453 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_columns_have_desc.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4650 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_all_columns.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4111 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_freshness.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5256 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_labels_keys.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2772 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_loader.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5246 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_meta_keys.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3711 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5550 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_group.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5159 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_name.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5566 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_type.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2852 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_table_has_description.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3117 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_tags.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.881186 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/dbt_test/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/dbt_test/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      739 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/dbt_test/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5672 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/dbt_test/missing_primary_key_tests.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5216 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/dbt_test/test_coverage.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.882195 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      743 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5718 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/documentation_on_stale_columns.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4306 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/exposures_dependent_on_private_models.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4100 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/public_models_without_contracts.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6394 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/undocumented_columns.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5092 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/undocumented_public_models.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.886763 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/
--rw-r--r--   0 anandgupta   (501) staff       (20)      419 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/README.md
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1009 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     6585 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/direct_join_to_source.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5790 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/downstream_models_dependent_on_source.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3937 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/duplicate_sources.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3671 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/hard_coded_references.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3937 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/joining_of_upstream_concepts.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5223 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/model_fanout.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3753 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/multiple_sources_joined.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3993 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/root_model.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4550 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/source_fanout.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4976 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_downstream_models.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4261 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_staging_models.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2780 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/unused_sources.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.887271 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/performance/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/performance/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      829 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/performance/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3627 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/performance/chain_view_linking.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4689 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/performance/exposure_parent_materializations.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2657 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/schema.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.888268 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1101 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/base.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4382 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/model_directories_structure.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     4999 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/model_naming_conventions.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3675 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/source_directories_structure.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     3484 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/test_directory_structure.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      267 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.888586 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/schemas/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/schemas/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1878 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/schemas/catalog.py
--rw-r--r--   0 anandgupta   (501) staff       (20)    14117 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/schemas/manifest.py
--rw-r--r--   0 anandgupta   (501) staff       (20)    18577 2024-03-09 02:10:20.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.888882 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.889102 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/catalog/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/catalog/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.889322 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      832 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/wrapper.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      196 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/catalog/wrapper.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.889544 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.890409 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1523 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/schemas.py
--rw-r--r--   0 anandgupta   (501) staff       (20)    17274 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/wrapper.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1078 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/wrapper.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.890707 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/run_results/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/run_results/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1267 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/run_results/run_results.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.890907 altimate-datapilot-0.0.7/src/datapilot/exceptions/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/exceptions/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      162 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/exceptions/exceptions.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.891324 altimate-datapilot-0.0.7/src/datapilot/schemas/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/schemas/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      190 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/schemas/constants.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      319 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/schemas/nodes.py
--rw-r--r--   0 anandgupta   (501) staff       (20)      193 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/schemas/sql.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.891506 altimate-datapilot-0.0.7/src/datapilot/utils/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/utils/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.891743 altimate-datapilot-0.0.7/src/datapilot/utils/formatting/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/utils/formatting/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1377 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/src/datapilot/utils/formatting/utils.py
--rw-r--r--   0 anandgupta   (501) staff       (20)    11150 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.7/src/datapilot/utils/utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.854734 altimate-datapilot-0.0.7/tests/
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.891853 altimate-datapilot-0.0.7/tests/core/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/tests/core/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.891930 altimate-datapilot-0.0.7/tests/core/platform/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/tests/core/platform/__init__.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.892206 altimate-datapilot-0.0.7/tests/core/platform/dbt/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/tests/core/platform/dbt/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1298 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.7/tests/core/platform/dbt/test_cli.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     5717 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.7/tests/core/platform/dbt/test_utils.py
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.892863 altimate-datapilot-0.0.7/tests/data/
--rw-r--r--   0 anandgupta   (501) staff       (20)   181355 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/tests/data/catalog_v1.json
--rw-r--r--   0 anandgupta   (501) staff       (20)      397 2024-01-30 02:44:52.000000 altimate-datapilot-0.0.7/tests/data/config.yml
--rw-r--r--   0 anandgupta   (501) staff       (20)  2187651 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.7/tests/data/manifest_v11.json
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.905396 altimate-datapilot-0.0.7/tests/data/manifests/
--rw-r--r--   0 anandgupta   (501) staff       (20)   440290 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.7/tests/data/manifests/manifest_js.json
--rw-r--r--   0 anandgupta   (501) staff       (20)   496433 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.7/tests/data/manifests/manifest_js2.json
--rw-r--r--   0 anandgupta   (501) staff       (20)   451985 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.7/tests/data/manifests/manifest_js3.json
--rw-r--r--   0 anandgupta   (501) staff       (20)   451995 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.7/tests/data/manifests/manifest_tuva.json
--rw-r--r--   0 anandgupta   (501) staff       (20)   511945 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.7/tests/data/manifests/manifest_tuva2.json
--rw-r--r--   0 anandgupta   (501) staff       (20)  3176176 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.7/tests/data/manifests/manifest_tuva3.json
-drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:57:06.907803 altimate-datapilot-0.0.7/tests/utils/
--rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.7/tests/utils/__init__.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     2491 2024-03-09 02:10:20.000000 altimate-datapilot-0.0.7/tests/utils/test_utils.py
--rw-r--r--   0 anandgupta   (501) staff       (20)     1764 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.7/tox.ini
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.344351 altimate-datapilot-0.0.8/
+-rw-r--r--   0 anandgupta   (501) staff       (20)      420 2024-04-02 00:54:06.000000 altimate-datapilot-0.0.8/.bumpversion.cfg
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1988 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.8/.cookiecutterrc
+-rw-r--r--   0 anandgupta   (501) staff       (20)      149 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/.coveragerc
+-rw-r--r--   0 anandgupta   (501) staff       (20)      353 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/.editorconfig
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.308488 altimate-datapilot-0.0.8/.github/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.313902 altimate-datapilot-0.0.8/.github/workflows/
+-rw-r--r--   0 anandgupta   (501) staff       (20)    10794 2024-01-25 04:30:47.000000 altimate-datapilot-0.0.8/.github/workflows/github-actions.yml
+-rw-r--r--   0 anandgupta   (501) staff       (20)      688 2024-01-30 03:12:39.000000 altimate-datapilot-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 anandgupta   (501) staff       (20)      204 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/.pre-commit-hooks.yaml
+-rw-r--r--   0 anandgupta   (501) staff       (20)      282 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/.readthedocs.yml
+-rw-r--r--   0 anandgupta   (501) staff       (20)       50 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/AUTHORS.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       86 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/CHANGELOG.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2332 2024-01-25 04:45:20.000000 altimate-datapilot-0.0.8/CONTRIBUTING.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1100 2024-01-25 04:37:04.000000 altimate-datapilot-0.0.8/LICENSE
+-rw-r--r--   0 anandgupta   (501) staff       (20)      495 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/MANIFEST.in
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2159 2024-04-02 00:54:47.344203 altimate-datapilot-0.0.8/PKG-INFO
+-rw-r--r--   0 anandgupta   (501) staff       (20)    11531 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/README.md
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1575 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.8/README.rst
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.314139 altimate-datapilot-0.0.8/ci/
+-rwxr-xr-x   0 anandgupta   (501) staff       (20)     2867 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/ci/bootstrap.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)       72 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/ci/requirements.txt
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.308684 altimate-datapilot-0.0.8/ci/templates/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.308732 altimate-datapilot-0.0.8/ci/templates/.github/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.314253 altimate-datapilot-0.0.8/ci/templates/.github/workflows/
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1965 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.316033 altimate-datapilot-0.0.8/docs/
+-rw-r--r--   0 anandgupta   (501) staff       (20)       28 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/docs/authors.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       30 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/docs/changelog.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1099 2024-04-02 00:54:06.000000 altimate-datapilot-0.0.8/docs/conf.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2433 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.8/docs/configuration.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       33 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/docs/contributing.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1776 2024-03-09 02:10:20.000000 altimate-datapilot-0.0.8/docs/features.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1635 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/docs/hooks.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)      221 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/docs/index.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)    35144 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/docs/insights.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1084 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.8/docs/installation.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2361 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.8/docs/introduction.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1926 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/docs/performance.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       27 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/docs/readme.rst
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.316244 altimate-datapilot-0.0.8/docs/reference/
+-rw-r--r--   0 anandgupta   (501) staff       (20)      106 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/docs/reference/datapilot.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       61 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/docs/reference/index.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)       29 2024-01-31 00:25:08.000000 altimate-datapilot-0.0.8/docs/requirements.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)      109 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/docs/spelling_wordlist.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)       70 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/docs/usage.rst
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1194 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/pyproject.toml
+-rw-r--r--   0 anandgupta   (501) staff       (20)      903 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/pytest.ini
+-rw-r--r--   0 anandgupta   (501) staff       (20)       38 2024-04-02 00:54:47.344408 altimate-datapilot-0.0.8/setup.cfg
+-rwxr-xr-x   0 anandgupta   (501) staff       (20)     3043 2024-04-02 00:54:06.000000 altimate-datapilot-0.0.8/setup.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.309033 altimate-datapilot-0.0.8/src/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.317123 altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2159 2024-04-02 00:54:47.000000 altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/PKG-INFO
+-rw-r--r--   0 anandgupta   (501) staff       (20)     9717 2024-04-02 00:54:47.000000 altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/SOURCES.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)        1 2024-04-02 00:54:47.000000 altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/dependency_links.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)      141 2024-04-02 00:54:47.000000 altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/entry_points.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)        1 2024-04-02 00:54:45.000000 altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/not-zip-safe
+-rw-r--r--   0 anandgupta   (501) staff       (20)      110 2024-04-02 00:54:47.000000 altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/requires.txt
+-rw-r--r--   0 anandgupta   (501) staff       (20)       10 2024-04-02 00:54:47.000000 altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/top_level.txt
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.317357 altimate-datapilot-0.0.8/src/datapilot/
+-rw-r--r--   0 anandgupta   (501) staff       (20)       22 2024-04-02 00:54:06.000000 altimate-datapilot-0.0.8/src/datapilot/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      380 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/__main__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.317549 altimate-datapilot-0.0.8/src/datapilot/cli/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/cli/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      181 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/cli/main.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.317672 altimate-datapilot-0.0.8/src/datapilot/clients/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.8/src/datapilot/clients/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.317963 altimate-datapilot-0.0.8/src/datapilot/clients/altimate/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.8/src/datapilot/clients/altimate/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3107 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.8/src/datapilot/clients/altimate/client.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2629 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.8/src/datapilot/clients/altimate/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.318267 altimate-datapilot-0.0.8/src/datapilot/config/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/config/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      403 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.8/src/datapilot/config/config.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1146 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/config/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.318387 altimate-datapilot-0.0.8/src/datapilot/core/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.318791 altimate-datapilot-0.0.8/src/datapilot/core/insights/
+-rw-r--r--   0 anandgupta   (501) staff       (20)       18 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.318975 altimate-datapilot-0.0.8/src/datapilot/core/insights/base/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/base/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      883 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/base/insight.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      596 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/report.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      413 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/schema.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.319089 altimate-datapilot-0.0.8/src/datapilot/core/insights/sql/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/sql/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.319252 altimate-datapilot-0.0.8/src/datapilot/core/insights/sql/base/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/sql/base/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      471 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/sql/base/insight.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.319386 altimate-datapilot-0.0.8/src/datapilot/core/insights/sql/runtime/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/sql/runtime/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.319467 altimate-datapilot-0.0.8/src/datapilot/core/insights/sql/static/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/sql/static/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      535 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/insights/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.319545 altimate-datapilot-0.0.8/src/datapilot/core/platforms/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.320286 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.320544 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/cli/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/cli/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4146 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/cli/cli.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      502 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/constants.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      110 2024-03-09 02:10:20.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/exceptions.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6562 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/executor.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1095 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/factory.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1638 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/formatting.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.320755 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/hooks/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/hooks/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2966 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/hooks/executor_hook.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.321234 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/
+-rw-r--r--   0 anandgupta   (501) staff       (20)     7547 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5260 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/base.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.325491 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      824 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4609 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_column_desc_are_same.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     7222 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_column_name_contract.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3185 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_macro_args_have_desc.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2802 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_macro_has_desc.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4277 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_all_columns.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5183 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_labels_keys.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5016 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_meta_keys.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2968 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_properties_file.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5706 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_group.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5187 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_name.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5590 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_type.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6098 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_materialization_by_childs.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6037 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_name_contract.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6319 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_and_childs.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4665 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_database.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4658 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_schema.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3555 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_tags.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4254 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_childs.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4453 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_columns_have_desc.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4650 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_all_columns.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4111 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_freshness.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5256 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_labels_keys.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2772 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_loader.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5246 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_meta_keys.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3711 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5550 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_group.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5159 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_name.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5566 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_type.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2852 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_table_has_description.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3117 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_tags.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.325991 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      739 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5672 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/missing_primary_key_tests.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5216 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/test_coverage.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.326835 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      743 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5718 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/documentation_on_stale_columns.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4306 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/exposures_dependent_on_private_models.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4100 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/public_models_without_contracts.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6394 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/undocumented_columns.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5092 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/undocumented_public_models.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.329108 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/
+-rw-r--r--   0 anandgupta   (501) staff       (20)      419 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/README.md
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1009 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     6585 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/direct_join_to_source.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5790 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/downstream_models_dependent_on_source.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3937 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/duplicate_sources.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3671 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/hard_coded_references.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3937 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/joining_of_upstream_concepts.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5223 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/model_fanout.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3753 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/multiple_sources_joined.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3993 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/root_model.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4550 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/source_fanout.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4976 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_downstream_models.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4261 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_staging_models.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2780 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/unused_sources.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.329665 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      829 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3627 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/chain_view_linking.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4689 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/exposure_parent_materializations.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2657 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/schema.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.330359 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1101 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/base.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4382 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/model_directories_structure.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     4999 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/model_naming_conventions.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3675 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/source_directories_structure.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     3484 2024-04-02 00:54:00.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/test_directory_structure.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      267 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.330709 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/schemas/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/schemas/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1878 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/schemas/catalog.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)    14117 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/schemas/manifest.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)    18577 2024-03-09 02:10:20.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.330910 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.331102 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.331340 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      832 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/wrapper.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      196 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/wrapper.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.331570 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.331899 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1523 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/schemas.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)    17274 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/wrapper.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1078 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/wrapper.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.332111 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/run_results/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/run_results/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1267 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/run_results/run_results.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.332312 altimate-datapilot-0.0.8/src/datapilot/exceptions/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/exceptions/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      162 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/exceptions/exceptions.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.332705 altimate-datapilot-0.0.8/src/datapilot/schemas/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/schemas/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      190 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/schemas/constants.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      319 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/schemas/nodes.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)      193 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/schemas/sql.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.332892 altimate-datapilot-0.0.8/src/datapilot/utils/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/utils/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.333075 altimate-datapilot-0.0.8/src/datapilot/utils/formatting/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/utils/formatting/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1377 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/src/datapilot/utils/formatting/utils.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)    11150 2024-03-29 16:47:02.000000 altimate-datapilot-0.0.8/src/datapilot/utils/utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.311771 altimate-datapilot-0.0.8/tests/
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.333180 altimate-datapilot-0.0.8/tests/core/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/tests/core/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.333268 altimate-datapilot-0.0.8/tests/core/platform/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/tests/core/platform/__init__.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.333538 altimate-datapilot-0.0.8/tests/core/platform/dbt/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/tests/core/platform/dbt/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1298 2024-02-14 00:53:49.000000 altimate-datapilot-0.0.8/tests/core/platform/dbt/test_cli.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     5717 2024-01-30 03:15:47.000000 altimate-datapilot-0.0.8/tests/core/platform/dbt/test_utils.py
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.334148 altimate-datapilot-0.0.8/tests/data/
+-rw-r--r--   0 anandgupta   (501) staff       (20)   181355 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/tests/data/catalog_v1.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)      397 2024-01-30 02:44:52.000000 altimate-datapilot-0.0.8/tests/data/config.yml
+-rw-r--r--   0 anandgupta   (501) staff       (20)  2187651 2024-01-30 04:41:49.000000 altimate-datapilot-0.0.8/tests/data/manifest_v11.json
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.341289 altimate-datapilot-0.0.8/tests/data/manifests/
+-rw-r--r--   0 anandgupta   (501) staff       (20)   440290 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.8/tests/data/manifests/manifest_js.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)   496433 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.8/tests/data/manifests/manifest_js2.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)   451985 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.8/tests/data/manifests/manifest_js3.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)   451995 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.8/tests/data/manifests/manifest_tuva.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)   511945 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.8/tests/data/manifests/manifest_tuva2.json
+-rw-r--r--   0 anandgupta   (501) staff       (20)  3176176 2024-01-30 22:07:56.000000 altimate-datapilot-0.0.8/tests/data/manifests/manifest_tuva3.json
+drwxr-xr-x   0 anandgupta   (501) staff       (20)        0 2024-04-02 00:54:47.343993 altimate-datapilot-0.0.8/tests/utils/
+-rw-r--r--   0 anandgupta   (501) staff       (20)        0 2024-01-29 21:19:17.000000 altimate-datapilot-0.0.8/tests/utils/__init__.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     2491 2024-03-09 02:10:20.000000 altimate-datapilot-0.0.8/tests/utils/test_utils.py
+-rw-r--r--   0 anandgupta   (501) staff       (20)     1764 2024-01-25 04:30:38.000000 altimate-datapilot-0.0.8/tox.ini
```

### Comparing `altimate-datapilot-0.0.7/.cookiecutterrc` & `altimate-datapilot-0.0.8/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/.github/workflows/github-actions.yml` & `altimate-datapilot-0.0.8/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/.pre-commit-config.yaml` & `altimate-datapilot-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/CONTRIBUTING.rst` & `altimate-datapilot-0.0.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/LICENSE` & `altimate-datapilot-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/PKG-INFO` & `altimate-datapilot-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altimate-datapilot
-Version: 0.0.7
+Version: 0.0.8
 Summary: Assistant for Data Teams
 Home-page: https://github.com/AltimateAI/datapilot
 Author: Anand Gupta
 Author-email: info@altimate.ai
 License: MIT
 Project-URL: Documentation, https://datapilot.readthedocs.io/
 Project-URL: Changelog, https://datapilot.readthedocs.io/en/latest/changelog.html
```

### Comparing `altimate-datapilot-0.0.7/README.md` & `altimate-datapilot-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/README.rst` & `altimate-datapilot-0.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/ci/bootstrap.py` & `altimate-datapilot-0.0.8/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/ci/templates/.github/workflows/github-actions.yml` & `altimate-datapilot-0.0.8/ci/templates/.github/workflows/github-actions.yml`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/docs/conf.py` & `altimate-datapilot-0.0.8/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 source_suffix = ".rst"
 master_doc = "index"
 project = "datapilot"
 year = "2024"
 author = "Anand Gupta"
 copyright = f"{year}, {author}"
-version = release = "0.0.7"
+version = release = "0.0.8"
 
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/AltimateAI/datapilot/issues/%s", "#"),
     "pr": ("https://github.com/AltimateAI/datapilot/pull/%s", "PR #"),
 }
```

### Comparing `altimate-datapilot-0.0.7/docs/configuration.rst` & `altimate-datapilot-0.0.8/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/docs/features.rst` & `altimate-datapilot-0.0.8/docs/features.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/docs/hooks.rst` & `altimate-datapilot-0.0.8/docs/hooks.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/docs/insights.rst` & `altimate-datapilot-0.0.8/docs/insights.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/docs/installation.rst` & `altimate-datapilot-0.0.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/docs/introduction.rst` & `altimate-datapilot-0.0.8/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/docs/performance.rst` & `altimate-datapilot-0.0.8/docs/performance.rst`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/pyproject.toml` & `altimate-datapilot-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/pytest.ini` & `altimate-datapilot-0.0.8/pytest.ini`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/setup.py` & `altimate-datapilot-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def read(*names, **kwargs):
     with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
         return fh.read()
 
 
 setup(
     name="altimate-datapilot",
-    version="0.0.7",
+    version="0.0.8",
     license="MIT",
     description="Assistant for Data Teams",
     long_description="{}\n{}".format(
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Anand Gupta",
```

### Comparing `altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/PKG-INFO` & `altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: altimate-datapilot
-Version: 0.0.7
+Version: 0.0.8
 Summary: Assistant for Data Teams
 Home-page: https://github.com/AltimateAI/datapilot
 Author: Anand Gupta
 Author-email: info@altimate.ai
 License: MIT
 Project-URL: Documentation, https://datapilot.readthedocs.io/
 Project-URL: Changelog, https://datapilot.readthedocs.io/en/latest/changelog.html
```

### Comparing `altimate-datapilot-0.0.7/src/altimate_datapilot.egg-info/SOURCES.txt` & `altimate-datapilot-0.0.8/src/altimate_datapilot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/clients/altimate/client.py` & `altimate-datapilot-0.0.8/src/datapilot/clients/altimate/client.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/clients/altimate/utils.py` & `altimate-datapilot-0.0.8/src/datapilot/clients/altimate/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/config/utils.py` & `altimate-datapilot-0.0.8/src/datapilot/config/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/insights/base/insight.py` & `altimate-datapilot-0.0.8/src/datapilot/core/insights/base/insight.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/insights/report.py` & `altimate-datapilot-0.0.8/src/datapilot/core/insights/report.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/insights/utils.py` & `altimate-datapilot-0.0.8/src/datapilot/core/insights/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/cli/cli.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/cli/cli.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/executor.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/executor.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/factory.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/factory.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/formatting.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/formatting.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/hooks/executor_hook.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/hooks/executor_hook.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/__init__.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/base.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/base.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_column_desc_are_same.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_column_desc_are_same.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_column_name_contract.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_column_name_contract.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_macro_args_have_desc.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_macro_args_have_desc.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_macro_has_desc.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_macro_has_desc.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckMacroHasDesc(ChecksInsight):
-    NAME = "Macro has Documentation"
+    NAME = "Macro has documentation"
     ALIAS = "check_macro_has_desc"
     DESCRIPTION = "Macros should be documented."
     REASON_TO_FLAG = "Undocumented macros can cause misunderstandings and inefficiencies in data modeling and analysis, as they make it difficult to understand their purpose and usage. Clear descriptions are vital for accuracy and streamlined workflow."
 
     def _build_failure_result(
         self,
         node_id: str,
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_all_columns.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_all_columns.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_labels_keys.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_labels_keys.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_meta_keys.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_meta_keys.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_properties_file.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_properties_file.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_group.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckModelHasTestsByGroup(ChecksInsight):
-    NAME = "Model Has Tests By Group"
+    NAME = "Model has tests by group"
     ALIAS = "check_model_has_tests_by_group"
     DESCRIPTION = "Check if models have a number of tests for specific test groups."
     REASON_TO_FLAG = "Models should have tests with specific groups for proper validation."
     TESTS_LIST_STR = "tests"
     TEST_GROUP_STR = "test_group"
     TEST_COUNT_STR = "min_count"
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_name.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckModelHasTestsByName(ChecksInsight):
-    NAME = "Model Has Tests By Name"
+    NAME = "Model has tests by name"
     ALIAS = "check_model_has_tests_by_name"
     DESCRIPTION = "Checks that the model has tests with specific names."
     REASON_TO_FLAG = "Models should have tests with specific names for proper validation."
     TESTS_LIST_STR = "tests"
     TEST_NAME_STR = "test"
     TEST_COUNT_STR = "min_count"
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_type.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_has_tests_by_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckModelHasTestsByType(ChecksInsight):
-    NAME = "Model Has Tests By Type"
+    NAME = "Model has tests by type"
     ALIAS = "check_model_has_tests_by_type"
     DESCRIPTION = "Checks that the model has tests with specific types."
     REASON_TO_FLAG = "Models should have tests with specific types for proper validation."
     TESTS_LIST_STR = "tests"
     TEST_TYPE_STR = "test"
     TEST_COUNT_STR = "min_count"
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_materialization_by_childs.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_materialization_by_childs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datapilot.core.platforms.dbt.constants import VIEW
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 
 
 class CheckModelMaterializationByChilds(ChecksInsight):
-    NAME = "Model Materialization By Childs"
+    NAME = "Model materialization by children"
     ALIAS = "check_model_materialization_by_childs"
     DESCRIPTION = "Fewer children than threshold ideally should be view or ephemeral, more or equal should be table or incremental."
     REASON_TO_FLAG = "The model is flagged due to inappropriate materialization: models with child counts above the threshold require robust and efficient data processing, hence they should be materialized as tables or incrementals for optimized query performance and data management."
     THRESHOLD_CHILDS_STR = "threshold_childs"
 
     def _build_failure_result_view_materialization(
         self,
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_name_contract.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_name_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 from datapilot.utils.utils import is_superset_path
 
 
 class CheckModelNameContract(ChecksInsight):
-    NAME = "Valid Model Name by Folder"
+    NAME = "Valid Mmdel name by folder"
     ALIAS = "model_name_by_folder"
     DESCRIPTION = (
         "Check that model name abides to a contract (similar to check-column-name-contract). A contract consists of a regex pattern."
     )
     REASON_TO_FLAG = "Model naming convention is not as expected"
     DEFAULT_PATTERN_STR = "default_pattern"
     PATTERNS_LIST_STR = "patterns"
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_and_childs.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_and_childs.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,26 +108,24 @@
     @classmethod
     def get_config_schema(cls):
         config_schema = super().get_config_schema()
         config_schema["config"] = {
             "$schema": "http://json-schema.org/draft-07/schema#",
             "type": "object",
             "properties": {
-                cls.MAX_CHILDS_STR: {
-                    "type": "integer",
-                    "description": "The maximum number of childs a model can have.",
-                },
+                cls.MAX_CHILDS_STR: {"type": "integer", "description": "The maximum number of childs a model can have.", "default": 3},
                 cls.MIN_CHILDS_STR: {
                     "type": "integer",
                     "description": "The minimum number of childs a model can have.",
                     "default": 0,
                 },
                 cls.MAX_PARENTS_STR: {
                     "type": "integer",
                     "description": "The maximum number of parents a model can have.",
+                    "default": 3,
                 },
                 cls.MIN_PARENTS_STR: {
                     "type": "integer",
                     "description": "The minimum number of parents a model can have.",
                     "default": 0,
                 },
             },
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_database.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_database.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckModelParentsDatabase(ChecksInsight):
-    NAME = "Check Model Parents Database"
+    NAME = "Check model parents database"
     ALIAS = "check_model_parents_database"
     DESCRIPTION = "Ensures the parent models or sources are from certain database."
     REASON_TO_FLAG = "The model has a different database as parent model or source."
     WHITELIST_STR = "whitelist"
     BLACKLIST_STR = "blacklist"
 
     def _build_failure_result(
@@ -101,13 +101,9 @@
                 },
                 cls.BLACKLIST_STR: {
                     "type": "array",
                     "items": {"type": "string"},
                     "description": "List of databases that are not allowed as parent models or sources.",
                 },
             },
-            "oneOf": [
-                {"required": [cls.WHITELIST_STR], "not": {"required": [cls.BLACKLIST_STR]}},
-                {"required": [cls.BLACKLIST_STR], "not": {"required": [cls.WHITELIST_STR]}},
-            ],
         }
         return config_schema
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_schema.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_parents_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -101,13 +101,9 @@
                 },
                 cls.BLACKLIST_STR: {
                     "type": "array",
                     "items": {"type": "string"},
                     "description": "List of schemas that are not allowed as parent models or sources.",
                 },
             },
-            "oneOf": [
-                {"required": [cls.WHITELIST_STR], "not": {"required": [cls.BLACKLIST_STR]}},
-                {"required": [cls.BLACKLIST_STR], "not": {"required": [cls.WHITELIST_STR]}},
-            ],
         }
         return config_schema
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_model_tags.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_model_tags.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_childs.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_childs.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_columns_have_desc.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_columns_have_desc.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 from datapilot.core.platforms.dbt.wrappers.catalog.wrapper import BaseCatalogWrapper
 from datapilot.utils.formatting.utils import numbered_list
 
 
 class CheckSourceColumnsHaveDescriptions(ChecksInsight):
-    NAME = "Source Columns Have Descriptions"
+    NAME = "Source columns have descriptions"
     ALIAS = "check_source_columns_have_desc"
     DESCRIPTION = "Ensures that the source has columns with descriptions in the properties file (usually schema.yml)."
     REASON_TO_FLAG = "Missing descriptions for columns in the source can lead to confusion and inconsistency in analysis. "
 
     def __init__(self, catalog_wrapper: BaseCatalogWrapper, *args, **kwargs):
         self.catalog = catalog_wrapper
         super().__init__(*args, **kwargs)
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_all_columns.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_all_columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 from datapilot.core.platforms.dbt.wrappers.catalog.wrapper import BaseCatalogWrapper
 from datapilot.utils.formatting.utils import numbered_list
 
 
 class CheckSourceHasAllColumns(ChecksInsight):
-    NAME = "Source Has All Columns"
+    NAME = "Source has all columns"
     ALIAS = "check_source_has_all_columns"
     DESCRIPTION = "Ensures that all columns in the database are also specified in the properties file. (usually schema.yml)."
     REASON_TO_FLAG = "Missing columns in the source can lead to confusion and inconsistency in analysis. "
     FILES_REQUIRED: ClassVar = ["Manifest", "Catalog"]
 
     def __init__(self, catalog_wrapper: BaseCatalogWrapper, *args, **kwargs):
         self.catalog = catalog_wrapper
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_freshness.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_freshness.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckSourceHasFreshness(ChecksInsight):
-    NAME = "Source Has Freshness Options"
+    NAME = "Source has freshness options"
     ALIAS = "check_source_has_freshness"
     DESCRIPTION = "Ensures that the source has freshness options"
     REASON_TO_FLAG = "Missing freshness options for the source can lead to confusion and inconsistency in analysis. "
     FRESHNESS_STR = "freshness"
 
     def _build_failure_result(self, source_id: int, missing_keys) -> DBTInsightResult:
         """
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_labels_keys.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_labels_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 from datapilot.utils.formatting.utils import numbered_list
 
 
 class CheckSourceHasLabelsKeys(ChecksInsight):
-    NAME = "Check Source Has Labels Keys"
+    NAME = "Check source has labels keys"
     ALIAS = "check_source_has_labels_keys"
     DESCRIPTION = (
         "Checks that the source has the specified labels keys as defined in the properties file. "
         "Ensuring that the source has the required labels keys helps in maintaining metadata consistency and understanding."
     )
     REASON_TO_FLAG = (
         "Missing labels keys in the source can lead to inconsistency in metadata management and understanding of the source. "
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_loader.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckSourceHasLoader(ChecksInsight):
-    NAME = "Source Has Loader"
+    NAME = "Source has loader"
     ALIAS = "check_source_has_loader"
     DESCRIPTION = "Check if the source has a loader"
     REASON_TO_FLAG = "Missing loader for the source can lead to confusion and inconsistency in analysis. "
 
     def _build_failure_result(self, source_id: int) -> DBTInsightResult:
         """
         Build failure result for the insight if a model's parent schema is not whitelist or in blacklist.
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_meta_keys.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_meta_keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 from datapilot.utils.formatting.utils import numbered_list
 
 
 class CheckSourceHasMetaKeys(ChecksInsight):
-    NAME = "Source has required metadata Keys"
+    NAME = "Source has required metadata keys"
     ALIAS = "check_source_has_meta_keys"
     DESCRIPTION = "Check if the source has required metadata keys"
     REASON_TO_FLAG = "Missing meta keys in the source can lead to inconsistency in metadata management and understanding of the source. It's important to ensure that the source includes all the required meta keys as per the configuration."
     META_KEYS_STR = "meta_keys"
     ALLOW_EXTRA_KEYS_STR = "allow_extra_keys"
 
     def _build_failure_result(
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckSourceHasTests(ChecksInsight):
-    NAME = "Source Has Tests"
+    NAME = "Source has tests"
     ALIAS = "check_source_has_tests"
     DESCRIPTION = "Check if the source has tests"
     REASON_TO_FLAG = "The source table is missing tests. Ensure that the source table has tests."
     TESTS_STR = "tests"
 
     def generate(self, *args, **kwargs) -> List[DBTModelInsightResponse]:
         insights = []
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_group.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckSourceHasTestsByGroup(ChecksInsight):
-    NAME = "Source Has Tests By Group"
+    NAME = "Source has tests by group"
     ALIAS = "check_source_has_tests_by_group"
     DESCRIPTION = "Check if sources have a number of tests for specific test groups."
     REASON_TO_FLAG = "Sources should have tests with specific groups for proper validation."
     TESTS_LIST_STR = "tests"
     TEST_GROUP_STR = "test_group"
     TEST_COUNT_STR = "min_count"
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_name.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckSourceHasTestsByName(ChecksInsight):
-    NAME = "Source Has Tests By Name"
+    NAME = "Source has tests by name"
     ALIAS = "check_source_has_tests_by_name"
     DESCRIPTION = "Checks that the source has tests with specific names."
     REASON_TO_FLAG = "Sources should have tests with specific names for proper validation."
     TESTS_LIST_STR = "tests"
     TEST_NAME_STR = "test"
     TEST_COUNT_STR = "min_count"
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_type.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_has_tests_by_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckSourceHasTestsByType(ChecksInsight):
-    NAME = "Source Has Tests By Type"
+    NAME = "Source has tests by type"
     ALIAS = "check_source_has_tests_by_type"
     DESCRIPTION = "Checks that the source has tests with specific types."
     REASON_TO_FLAG = "Sources should have tests with specific types for proper validation."
     TESTS_LIST_STR = "tests"
     TEST_TYPE_STR = "test"
     TEST_COUNT_STR = "min_count"
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_table_has_description.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_table_has_description.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckSourceTableHasDescription(ChecksInsight):
-    NAME = "Source Table Has Description"
+    NAME = "Source table has description"
     ALIAS = "check_source_table_has_desc"
     DESCRIPTION = "Ensures that the source table has a description"
     REASON_TO_FLAG = "Missing description for the source table can lead to confusion and inconsistency in analysis. "
 
     def _build_failure_result(self, source_id: int) -> DBTInsightResult:
         """
         Build failure result for the insight if a model's parent schema is not whitelist or in blacklist.
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/checks/check_source_tags.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/checks/check_source_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datapilot.core.platforms.dbt.insights.checks.base import ChecksInsight
 from datapilot.core.platforms.dbt.insights.schema import DBTInsightResult
 from datapilot.core.platforms.dbt.insights.schema import DBTModelInsightResponse
 from datapilot.core.platforms.dbt.schemas.manifest import AltimateResourceType
 
 
 class CheckSourceTags(ChecksInsight):
-    NAME = "Source has Tags"
+    NAME = "Source has tags"
     ALIAS = "check_source_tags"
     DESCRIPTION = "The source has only valid tags from the provided list."
     REASON_TO_FLAG = "The source has tags that are not in the valid tags list"
     TESTS_STR = "tags"
 
     def _build_failure_result(
         self,
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/dbt_test/base.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/dbt_test/missing_primary_key_tests.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/missing_primary_key_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     This class generates insights for each model that lacks proper primary key tests.
     """
 
     _ALL_TESTS_KEY = "_all_tests"
     NOT_NULL = "not_null"
     UNIQUE = "unique"
     UNIQUE_COMBINATION_OF_COLUMNS = "unique_combination_of_columns"
-    NAME = "Missing Primary Key Tests"
+    NAME = "Missing primary key tests"
     ALIAS = "missing_primary_key_tests"
     DESCRIPTION = "Checks if the model has a primary key test. "
     REASON_TO_FLAG = (
         "dbt tests play a crucial role in asserting data correctness. The absence of primary key tests can increase "
         "the risk of data integrity issues, affecting project reliability and scalability."
     )
     FAILURE_MESSAGE = (
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/dbt_test/test_coverage.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/dbt_test/test_coverage.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class DBTTestCoverage(DBTTestInsight):
     """
     This class identifies DBT models with test coverage below a specified threshold.
     It aims to ensure that a minimum percentage of tests are applied to each model to maintain data integrity.
     """
 
-    NAME = "Low Test Coverage in dbt Models"
+    NAME = "Low test coverage in dbt models"
     ALIAS = "dbt_low_test_coverage"
     DESCRIPTION = "Checks if the project test coverage is below the minimum threshold. "
     REASON_TO_FLAG = (
         "dbt models should have a minimum test coverage percentage to ensure the reliability and accuracy "
         "of data transformations. Low test coverage can lead to data quality issues."
     )
     FAILURE_MESSAGE = (
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/base.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/documentation_on_stale_columns.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/documentation_on_stale_columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class DBTDocumentationStaleColumns(DBTGovernanceInsight):
     """
     DBTDocumentationStaleColumns identifies columns that have been documented but are no longer present in the model.
     """
 
-    NAME = "Documentation of Stale Columns"
+    NAME = "Documentation of stale columns"
     ALIAS = "documentation_on_stale_columns"
     DESCRIPTION = (
         "Identify columns that have been documented but are no longer present in the model. "
         "This insight helps in maintaining accurate and up-to-date documentation."
     )
     REASON_TO_FLAG = (
         "A column has been documented but is no longer present in the model/database. "
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/exposures_dependent_on_private_models.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/exposures_dependent_on_private_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class DBTExposureDependentOnPrivateModels(DBTGovernanceInsight):
     """
     DBTExposureDependentOnPrivateModels identifies exposures that are dependent on private models.
     """
 
-    NAME = "Exposures Dependent on Private Models"
+    NAME = "Exposures dependent on private models"
     ALIAS = "exposures_dependent_on_private_models"
     DESCRIPTION = "Identify exposures that are dependent on private models. "
     REASON_TO_FLAG = (
         "Exposures illustrate how and where data is consumed in downstream tools. These tools should utilize "
         "data from public, trusted, and contracted sources to ensure data reliability and integrity."
     )
     FAILURE_MESSAGE = (
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/public_models_without_contracts.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/public_models_without_contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class DBTPublicModelWithoutContracts(DBTGovernanceInsight):
     """
     DBTUndocumentedPublicModels identifies public models that are not documented.
     """
 
-    NAME = "Public Models Without Contracts"
+    NAME = "Public models without contracts"
     ALIAS = "public_models_without_contracts"
     DESCRIPTION = "Identify public models that don't have contracts."
     REASON_TO_FLAG = (
         "Public models are accessible to all downstream consumers, making it crucial to have clear "
         "contracts that specify data types and columns. This ensures consistency and predictability "
         "in data consumption."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/undocumented_columns.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/undocumented_columns.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class DBTMissingDocumentation(DBTGovernanceInsight):
     """
     DBTDocumentationStaleColumns identifies columns that have been documented but are no longer present in the model.
     """
 
-    NAME = "Missing Documentation"
+    NAME = "Missing documentation"
     ALIAS = "missing_documentation"
     DESCRIPTION = (
         "Detects columns and models in the dbt project that lack documentation. Proper documentation is essential "
         "for understanding data structures and facilitating collaboration and usage of the dbt project."
     )
     REASON_TO_FLAG = (
         "Missing documentation for columns and models can lead to confusion and hinder effective data "
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/governance/undocumented_public_models.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/governance/undocumented_public_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # TODO: Include catalog information to make this better!
 class DBTUndocumentedPublicModels(DBTGovernanceInsight):
     """
     DBTUndocumentedPublicModels identifies public models that are not documented.
     """
 
-    NAME = "Undocumented Public Models"
+    NAME = "Undocumented public models"
     ALIAS = "undocumented_public_models"
     DESCRIPTION = "Identify public models that don't have documentation."
     REASON_TO_FLAG = (
         "Public models are accessible to a wide range of data consumers. To promote understanding and usability, "
         "it's essential to document these models comprehensively."
     )
     FAILURE_MESSAGE = (
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/base.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/direct_join_to_source.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/direct_join_to_source.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/downstream_models_dependent_on_source.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/downstream_models_dependent_on_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class DBTDownstreamModelsDependentOnSource(DBTModellingInsight):
     """
     DBTDownstreamModelsDependentOnSource identifies downstream models (either marts or intermediate)
     in a dbt project that depend directly on a source node.
     """
 
-    NAME = "Downstream Models Dependent on Source"
+    NAME = "Downstream models dependent on source"
     ALIAS = "downstream_source_dependence"
     DESCRIPTION = "Downstream models should not depend directly on source nodes. "
     REASON_TO_FLAG = (
         "Direct dependency of marts or intermediate models on a source node suggests a missing staging model. "
         "Staging models serve as atomic units, maintaining a one-to-one relationship with source data tables, "
         "while providing a consistent format for downstream consumption."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/duplicate_sources.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/duplicate_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class DBTDuplicateSources(DBTModellingInsight):
     """
     Check if the DBT project has duplicate sources.
     Ref: https://github.com/dbt-labs/dbt-project-evaluator/blob/main/models/marts/dag/fct_duplicate_sources.sql
     """
 
-    NAME = "Duplicate Sources"
+    NAME = "Duplicate sources"
     ALIAS = "Duplicate_Sources"
     DESCRIPTION = "Duplicate sources should be avoided."
     REASON_TO_FLAG = (
         "Having multiple source nodes pointing to the same database location can lead to an inaccurate "
         "representation of data lineage and potential confusion in data management."
     )
     FAILURE_MESSAGE = (
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/hard_coded_references.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/hard_coded_references.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class DBTHardCodedReferences(DBTModellingInsight):
     """
     Checks if the dbt model has hard coded references to other models.
     """
 
-    NAME = "Hard Coded References"
+    NAME = "Hard coded references"
     ALIAS = "hard_coded_references"
     DESCRIPTION = "Models should not have hard-coded references to tables"
     REASON_TO_FLAG = (
         "Hard-coded references in SQL prevent easy identification and tracking of data lineage, "
         "and can lead to issues in maintainability and scalability of the data models."
     )
     SOURCE_FANOUT_THRESHOLD = 1  # Default threshold, can be overridden as needed
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/joining_of_upstream_concepts.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/joining_of_upstream_concepts.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 class DBTRejoiningOfUpstreamConcepts(DBTModellingInsight):
     """
     DBTRejoiningOfUpstreamConcepts identifies cases in the dbt project where a parent model's direct child
     is also the direct child of another one of the parent's direct children, with the condition that the intermediate
     model has no other downstream dependencies.
     """
 
-    NAME = "Rejoining of Upstream Concepts"
+    NAME = "Rejoining of upstream Concepts"
     ALIAS = "rejoining_upstream_concepts"
     DESCRIPTION = (
         "Detects scenarios where a parent's direct child is also a direct child of another one " "of the parent's direct children."
     )
     REASON_TO_FLAG = (
         "Flagged to identify cases where a parent model has a direct child that is also a direct child "
         "of another one of the parent's direct children. Such patterns can suggest loops or redundancies in the DAG."
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/model_fanout.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/model_fanout.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class DBTModelFanout(DBTModellingInsight):
     """
     DBTModelFanout identifies parent models in a dbt project with more than a specified number
     of direct leaf children, indicating a high model fanout.
     """
 
-    NAME = "Model Fanout Analysis"
+    NAME = "Model fanout analysis"
     ALIAS = "model_fanout"
     DESCRIPTION = "Identifies parent models with an unusually high number of children. "
     REASON_TO_FLAG = (
         "Flagged to highlight parent models with an unusually high number of leaf children. This can suggest areas "
         "in the data pipeline where complexity is increased and transformations might be optimized."
     )
     FANOUT_THRESHOLD = 3  # Default threshold, can be overridden as needed
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/multiple_sources_joined.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/multiple_sources_joined.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class DBTModelsMultipleSourcesJoined(DBTModellingInsight):
     """
     DBTModelsMultipleSourcesJoined identifies models in a dbt project that reference more than one source.
     """
 
-    NAME = "Multiple Sources Joined"
+    NAME = "Multiple sources joined"
     ALIAS = "multiple_sources_joined"
     DESCRIPTION = "Models should not directly join multiple sources."
     REASON_TO_FLAG = (
         "Best practice is to have a single staging model per source and use this staging model as a "
         "dependency for downstream models. Directly joining multiple sources in a single model can "
         "lead to data management complexities and inconsistencies."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/root_model.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/root_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class DBTRootModel(DBTModellingInsight):
     """
     DBTRootModels is used to identify models in a dbt project with 0 direct parents,
     meaning these models cannot be traced back to a declared source or model.
     """
 
-    NAME = "Root Model Traceability"
+    NAME = "Root model traceability"
     ALIAS = "root_model"
     DESCRIPTION = "Identifies models in a dbt project with 0 direct parents, meaning these models cannot be traced back to a declared source or model."
     REASON_TO_FLAG = (
         "Best Practice is to ensure all models can be traced back to a source or another model in the project. "
         "Root models with no direct parents can lead to challenges in tracking data lineage and understanding"
         " the overall data model."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/source_fanout.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/source_fanout.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class DBTSourceFanout(DBTModellingInsight):
     """
     DBTSourceFanout identifies instances where a source is the direct parent of multiple resources in the DAG.
     """
 
-    NAME = "Source Fanout Analysis"
+    NAME = "Source fanout analysis"
     ALIAS = "source_fanout"
     DESCRIPTION = "Identifies sources with a high number of direct children."
     REASON_TO_FLAG = (
         "Identifying sources with high fanout can indicate areas where the data model might be overly complex "
         "or dependent on a single source. Such dependencies can introduce risks and "
         "complicate maintenance and scalability."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_downstream_models.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_downstream_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 class DBTStagingModelsDependentOnDownstreamModels(DBTModellingInsight):
     """
     DBTStagingModelsDependentOnDownstream identifies staging models in a dbt project that depend on downstream models.
     """
 
-    NAME = "Staging Models Dependency Check"
+    NAME = "Staging models dependency check"
     ALIAS = "staging_models_dependency"
     DESCRIPTION = "Staging models should not depend on downstream models."
     REASON_TO_FLAG = (
         "Best practice is for staging models to depend on source or raw data models, not on downstream models. "
         "Dependencies in the wrong direction can lead to complications in data processing and lineage tracing."
     )
     FAILURE_MESSAGE = (
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_staging_models.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/staging_model_dependent_on_staging_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 class DBTStagingModelsDependentOnStagingModels(DBTModellingInsight):
     """
     DBTStagingModelsDependentOnStagingModels identifies staging models in a dbt project that depend on staging models.
     """
 
-    NAME = "Staging Models Dependency on Staging Models"
+    NAME = "Staging models dependency on staging Models"
     ALIAS = "staging_models_on_staging"
     DESCRIPTION = "Staging models should not directly depend on other staging models."
     REASON_TO_FLAG = (
         "Best practice is for staging models to depend on source or raw data models, not on other staging models. "
         "Dependencies among staging models can lead to complicated data flows and hinder data lineage tracking."
     )
     FAILURE_MESSAGE = (
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/modelling/unused_sources.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/modelling/unused_sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class DBTUnusedSources(DBTModellingInsight):
     """
     DBTUnusedSources identifies sources in a dbt project that are not being referenced by any models.
     """
 
-    NAME = "Unused Sources Detection"
+    NAME = "Unused sources detection"
     ALIAS = "unused_sources"
     DESCRIPTION = "Detects sources in the dbt project that are not being referenced by any models."
     REASON_TO_FLAG = (
         "Unused sources, either defined in YML but not used in any model or leftover from deprecated models, "
         "represent unnecessary complexity in the project. It's important to keep the dbt project lean and relevant."
     )
     FAILURE_MESSAGE = "Source `{source_unique_id}` is not being referenced by any model, indicating it is unused."
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/performance/base.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/performance/chain_view_linking.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/chain_view_linking.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class DBTChainViewLinking(DBTPerformanceInsight):
     """
     Checks if the dbt model has a chain of views in it
     """
 
     CHAIN_LENGTH_STR = "chain_length"
-    NAME = "Chain View Linking"
+    NAME = "Chain view linking"
     ALIAS = "chain_view_linking"
     CHAIN_LENGTH = 4  # Default chain length, can be adjusted as needed
     DESCRIPTION = "Checks for long chains of view/ephemeral models in the dbt project. Long chains can lead to slow computation "
     REASON_TO_FLAG = (
         "Long runtime can occur for a model when it is built on top of a long chain of 'non-physically-materialized'"
         " models. Identifying these chains is crucial to optimize performance and reduce computation overhead."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/performance/exposure_parent_materializations.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/performance/exposure_parent_materializations.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class DBTExposureParentMaterialization(DBTPerformanceInsight):
     """
     Checks if the dbt model has hard coded references to other models.
     """
 
-    NAME = "Exposure Parent Materialization Check"
+    NAME = "Exposure parent materialization check"
     ALIAS = "exposure_parent_bad_materialization"
     DESCRIPTION = "Exposures should depend on transformed data models or metrics, not raw untransformed sources. "
     REASON_TO_FLAG = (
         "Exposures should depend on transformed data models or metrics, not raw untransformed sources. "
         "Moreover, parent models of exposures, being heavily used in downstream systems, "
         "should be materialized efficiently to ensure performance when queried."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/schema.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/schema.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/base.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/base.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/model_directories_structure.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/model_directories_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class DBTModelDirectoryStructure(DBTStructureInsight):
     """
     DBTModelDirectoryStructure checks if models are placed in the correct directories.
     """
 
-    NAME = "Bad Model Directory Structure"
+    NAME = "Bad model directory structure"
     ALIAS = "model_directory_structure"
     DESCRIPTION = "This rule identifies models that are not placed in their correct directories. "
     REASON_TO_FLAG = (
         "Placing models in the correct directories is vital for maintaining a structured and "
         "efficient data warehouse. Incorrectly placed models can lead to confusion, hinder "
         "discoverability, and complicate maintenance and scaling of the dbt project."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/model_naming_conventions.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/model_naming_conventions.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class DBTModelNamingConvention(DBTStructureInsight):
     """
     DBTModelNamingConvention identifies models that do not follow the naming convention.
     """
 
-    NAME = "Bad Model Naming Convention"
+    NAME = "Bad model naming convention"
     ALIAS = "model_naming_convention_check"
     DESCRIPTION = "This rule identifies models that do not follow the naming convention."
     REASON_TO_FLAG = (
         "Inconsistent or unclear naming conventions can lead to confusion and errors in querying the data warehouse. "
         "A well-defined naming convention clarifies the model type and purpose, promoting better understanding "
         "and effective data management. This rule flags models that deviate from established naming standards."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/source_directories_structure.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/source_directories_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 class DBTSourceDirectoryStructure(DBTStructureInsight):
     """
     DBTSourcesDirectoryStructure checks if sources are placed in the correct directories.
     """
 
-    NAME = "Bad Source Directory Structure"
+    NAME = "Bad source directory structure"
     ALIAS = "source_directory_structure"
     DESCRIPTION = "This rule identifies sources that are not placed in their correct directories. "
     REASON_TO_FLAG = (
         "Sources need to be organized in the correct directories to ensure an efficient and "
         "maintainable data architecture. Proper directory structure facilitates easy navigation, "
         "improves readability, and aids in managing the data sources effectively."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/insights/structure/test_directory_structure.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/insights/structure/test_directory_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class DBTTestDirectoryStructure(DBTStructureInsight):
     """
     DBTTestDirectoryStructure checks if tests are placed in the correct directories.
     """
 
-    NAME = "Bad Test Directory Structure"
+    NAME = "Bad test directory structure"
     ALIAS = "test_directory_structure"
     DESCRIPTION = "This rule checks if tests are correctly placed in the same directories as their corresponding models."
     REASON_TO_FLAG = (
         "It is important for tests to be placed in the same directory as their corresponding models to maintain "
         "a coherent and easy-to-navigate project structure. This practice enhances the ease of understanding "
         "and updating tests in parallel with model changes."
     )
```

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/schemas/catalog.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/schemas/catalog.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/schemas/manifest.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/utils.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/wrapper.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/catalog/v1/wrapper.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/schemas.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/schemas.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/wrapper.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/v11/wrapper.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/manifest/wrapper.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/manifest/wrapper.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/core/platforms/dbt/wrappers/run_results/run_results.py` & `altimate-datapilot-0.0.8/src/datapilot/core/platforms/dbt/wrappers/run_results/run_results.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/utils/formatting/utils.py` & `altimate-datapilot-0.0.8/src/datapilot/utils/formatting/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/src/datapilot/utils/utils.py` & `altimate-datapilot-0.0.8/src/datapilot/utils/utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/core/platform/dbt/test_cli.py` & `altimate-datapilot-0.0.8/tests/core/platform/dbt/test_cli.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/core/platform/dbt/test_utils.py` & `altimate-datapilot-0.0.8/tests/core/platform/dbt/test_utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/data/catalog_v1.json` & `altimate-datapilot-0.0.8/tests/data/catalog_v1.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/data/manifest_v11.json` & `altimate-datapilot-0.0.8/tests/data/manifest_v11.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/data/manifests/manifest_js.json` & `altimate-datapilot-0.0.8/tests/data/manifests/manifest_js.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/data/manifests/manifest_js2.json` & `altimate-datapilot-0.0.8/tests/data/manifests/manifest_js2.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/data/manifests/manifest_js3.json` & `altimate-datapilot-0.0.8/tests/data/manifests/manifest_js3.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/data/manifests/manifest_tuva.json` & `altimate-datapilot-0.0.8/tests/data/manifests/manifest_tuva.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/data/manifests/manifest_tuva2.json` & `altimate-datapilot-0.0.8/tests/data/manifests/manifest_tuva2.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/data/manifests/manifest_tuva3.json` & `altimate-datapilot-0.0.8/tests/data/manifests/manifest_tuva3.json`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tests/utils/test_utils.py` & `altimate-datapilot-0.0.8/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `altimate-datapilot-0.0.7/tox.ini` & `altimate-datapilot-0.0.8/tox.ini`

 * *Files identical despite different names*

