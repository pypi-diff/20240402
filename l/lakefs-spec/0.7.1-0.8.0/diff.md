# Comparing `tmp/lakefs-spec-0.7.1.tar.gz` & `tmp/lakefs-spec-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakefs-spec-0.7.1.tar", last modified: Thu Feb 29 07:23:43 2024, max compression
+gzip compressed data, was "lakefs-spec-0.8.0.tar", last modified: Tue Apr  2 08:38:52 2024, max compression
```

## Comparing `lakefs-spec-0.7.1.tar` & `lakefs-spec-0.8.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.932764 lakefs-spec-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.916765 lakefs-spec-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.920765 lakefs-spec-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.github/ISSUE_TEMPLATE/bug-report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.github/ISSUE_TEMPLATE/feature-request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.912764 lakefs-spec-0.7.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.920765 lakefs-spec-0.7.1/.github/actions/mike-docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.github/actions/mike-docs/action.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.920765 lakefs-spec-0.7.1/.github/actions/python-deps/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.github/actions/python-deps/action.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.github/pull-request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.920765 lakefs-spec-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.github/workflows/python.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-02-29 07:23:43.932764 lakefs-spec-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.920765 lakefs-spec-0.7.1/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/assets/lakefs-spec-logo-all.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.920765 lakefs-spec-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.920765 lakefs-spec-0.7.1/docs/_code/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_code/duckdb_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_code/pandas_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_code/polars_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_code/pyarrow_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_code/quickstart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.920765 lakefs-spec-0.7.1/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_images/aai-favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    26004 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_images/aai-logo-cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_images/lakefs-spec-favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_images/lakefs-spec-logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    31995 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_images/lakefs-spec-logo-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    40636 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_images/quickstart-lakefs-repositories.png
--rw-r--r--   0 runner    (1001) docker     (127)   123174 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_images/quickstart-lakefs-sample-repo.png
--rw-r--r--   0 runner    (1001) docker     (127)    32617 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_images/quickstart-lakefs-ui.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.924764 lakefs-spec-0.7.1/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_scripts/gen_api_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_scripts/jupytext_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.924764 lakefs-spec-0.7.1/docs/_styles/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_styles/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)    41136 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_styles/neoteroi-mkdocs.css
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_styles/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.924764 lakefs-spec-0.7.1/docs/_theme_overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_theme_overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.924764 lakefs-spec-0.7.1/docs/_theme_overrides/partials/
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/_theme_overrides/partials/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.924764 lakefs-spec-0.7.1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/guides/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/guides/filesystem-usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/guides/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/guides/integrations.md
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/guides/transactions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.924764 lakefs-spec-0.7.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/tutorials/.lakectl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/tutorials/demo_data_science_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/docs/tutorials/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.924764 lakefs-spec-0.7.1/hack/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/hack/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.924764 lakefs-spec-0.7.1/hack/config/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/hack/config/s3.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/hack/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/hack/lakefs-s3-local.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/hack/lock-deps.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 07:23:43.932764 lakefs-spec-0.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.916765 lakefs-spec-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.928764 lakefs-spec-0.7.1/src/lakefs_spec/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/src/lakefs_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/src/lakefs_spec/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/src/lakefs_spec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30047 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/src/lakefs_spec/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/src/lakefs_spec/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/src/lakefs_spec/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.932764 lakefs-spec-0.7.1/src/lakefs_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-02-29 07:23:43.000000 lakefs-spec-0.7.1/src/lakefs_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-02-29 07:23:43.000000 lakefs-spec-0.7.1/src/lakefs_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 07:23:43.000000 lakefs-spec-0.7.1/src/lakefs_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-29 07:23:43.000000 lakefs-spec-0.7.1/src/lakefs_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 07:23:43.000000 lakefs-spec-0.7.1/src/lakefs_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.928764 lakefs-spec-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 07:23:43.932764 lakefs-spec-0.7.1/tests/smoke_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/smoke_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/smoke_tests/test_abstractfilesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/smoke_tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_lakefs_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_put_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_spec_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-02-29 07:22:48.000000 lakefs-spec-0.7.1/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/bug-report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/feature-request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.838780 lakefs-spec-0.8.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/actions/mike-docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/actions/mike-docs/action.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/actions/python-deps/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/actions/python-deps/action.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/pull-request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/workflows/python.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/assets/lakefs-spec-logo-all.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/docs/_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/duckdb_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/pandas_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/polars_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/pyarrow_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/quickstart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/aai-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26004 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/aai-logo-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/lakefs-spec-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/lakefs-spec-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31995 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/lakefs-spec-logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40636 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-repositories.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123174 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-sample-repo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32617 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-ui.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_scripts/gen_api_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_scripts/jupytext_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_styles/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)    41136 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_styles/neoteroi-mkdocs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_styles/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_theme_overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_theme_overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_theme_overrides/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_theme_overrides/partials/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/filesystem-usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/integrations.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/transactions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/tutorials/.lakectl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/tutorials/demo_data_science_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/tutorials/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/hack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/hack/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/config/s3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/lakefs-s3-local.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/lock-deps.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.838780 lakefs-spec-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.850780 lakefs-spec-0.8.0/src/lakefs_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30309 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/tests/smoke_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/smoke_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/smoke_tests/test_abstractfilesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/smoke_tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_lakefs_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_put_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_spec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/util.py
```

### Comparing `lakefs-spec-0.7.1/.github/ISSUE_TEMPLATE/bug-report.yaml` & `lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/bug-report.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/.github/ISSUE_TEMPLATE/feature-request.yaml` & `lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/feature-request.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/.github/actions/mike-docs/action.yaml` & `lakefs-spec-0.8.0/.github/actions/mike-docs/action.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/.github/actions/python-deps/action.yaml` & `lakefs-spec-0.8.0/.github/actions/python-deps/action.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 name: Install Python dependencies
 description: Install all core and optional Python dependencies
 inputs:
   pythonVersion:
-    description: Python version to set up (see actions/setup-python@v4)
+    description: Python version to set up (see actions/setup-python@v5)
     required: true
 runs:
   using: "composite"
   steps:
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: ${{ inputs.pythonVersion }}
-        cache: 'pip'
+        cache: "pip"
         cache-dependency-path: |
           requirements-dev.txt
           requirements-docs.txt
           pyproject.toml
     - name: Install dependencies
       run: |
         pip install -r requirements-dev.txt -r requirements-docs.txt
```

### Comparing `lakefs-spec-0.7.1/.github/workflows/python.yaml` & `lakefs-spec-0.8.0/.github/workflows/python.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -16,39 +16,39 @@
     name: Run code checks and formatting hooks
     runs-on: ubuntu-latest
     env:
       MYPY_CACHE_DIR: "${{ github.workspace }}/.cache/mypy"
       RUFF_CACHE_DIR: "${{ github.workspace }}/.cache/ruff"
       PRE_COMMIT_HOME: "${{ github.workspace }}/.cache/pre-commit"
     steps:
-    - uses: actions/checkout@v4
-      with:
-        fetch-depth: 0 # for documentation builds
-    - name: Set up Python
-      uses: actions/setup-python@v5
-      with:
-        python-version: 3.11
-        cache: pip
-        cache-dependency-path: |
-          requirements-dev.txt
-          pyproject.toml
-    - name: Install dependencies
-      run: |
-        pip install -r requirements-dev.txt
-        pip install . --no-deps
-    - name: Cache pre-commit tools
-      uses: actions/cache@v4
-      with:
-        path: |
-          ${{ env.MYPY_CACHE_DIR }}
-          ${{ env.RUFF_CACHE_DIR }}
-          ${{ env.PRE_COMMIT_HOME }}
-        key: ${{ runner.os }}-${{ hashFiles('requirements-dev.txt', '.pre-commit-config.yaml') }}-linter-cache
-    - name: Run pre-commit checks
-      run: pre-commit run --all-files --verbose --show-diff-on-failure
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0 # for documentation builds
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: 3.11
+          cache: pip
+          cache-dependency-path: |
+            requirements-dev.txt
+            pyproject.toml
+      - name: Install dependencies
+        run: |
+          pip install -r requirements-dev.txt
+          pip install . --no-deps
+      - name: Cache pre-commit tools
+        uses: actions/cache@v4
+        with:
+          path: |
+            ${{ env.MYPY_CACHE_DIR }}
+            ${{ env.RUFF_CACHE_DIR }}
+            ${{ env.PRE_COMMIT_HOME }}
+          key: ${{ runner.os }}-${{ hashFiles('requirements-dev.txt', '.pre-commit-config.yaml') }}-linter-cache
+      - name: Run pre-commit checks
+        run: pre-commit run --all-files --verbose --show-diff-on-failure
   test:
     name: Test lakefs-spec on ubuntu-latest
     runs-on: ubuntu-latest
     services:
       lakefs:
         image: treeverse/lakefs:latest
         ports:
@@ -57,30 +57,30 @@
           LAKEFS_INSTALLATION_USER_NAME: "quickstart"
           LAKEFS_INSTALLATION_ACCESS_KEY_ID: "AKIAIOSFOLQUICKSTART"
           LAKEFS_INSTALLATION_SECRET_ACCESS_KEY: "wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY"
           LAKEFS_DATABASE_TYPE: "local"
           LAKEFS_AUTH_ENCRYPT_SECRET_KEY: "THIS_MUST_BE_CHANGED_IN_PRODUCTION"
           LAKEFS_BLOCKSTORE_TYPE: "local"
     steps:
-    - uses: actions/checkout@v4
-      with:
-        fetch-depth: 0
-    - name: Set up oldest supported Python (3.9) for testing
-      uses: actions/setup-python@v5
-      with:
-        python-version: 3.9
-    - name: Test on oldest supported Python
-      run: |
-        python -m pip install -r requirements-dev.txt
-        python -m pip install -e .
-        pytest -s --cov=src --cov=fsspec --cov-branch --cov-report=xml
-    - name: Upload coverage reports to Codecov
-      uses: codecov/codecov-action@v3
-      env:
-        CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+      - name: Set up oldest supported Python (3.9) for testing
+        uses: actions/setup-python@v5
+        with:
+          python-version: 3.9
+      - name: Test on oldest supported Python
+        run: |
+          python -m pip install -r requirements-dev.txt
+          python -m pip install -e .
+          pytest -s --cov=src --cov=fsspec --cov-branch --cov-report=xml
+      - name: Upload coverage reports to Codecov
+        uses: codecov/codecov-action@v4
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
   docs:
     name: Build documentation for lakefs-spec
     runs-on: ubuntu-latest
     services:
       lakefs:
         image: treeverse/lakefs:latest
         ports:
@@ -89,28 +89,28 @@
           LAKEFS_INSTALLATION_USER_NAME: "quickstart"
           LAKEFS_INSTALLATION_ACCESS_KEY_ID: "AKIAIOSFOLQUICKSTART"
           LAKEFS_INSTALLATION_SECRET_ACCESS_KEY: "wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY"
           LAKEFS_DATABASE_TYPE: "local"
           LAKEFS_AUTH_ENCRYPT_SECRET_KEY: "THIS_MUST_BE_CHANGED_IN_PRODUCTION"
           LAKEFS_BLOCKSTORE_TYPE: "local"
     steps:
-    - uses: actions/checkout@v4
-      with:
-        fetch-depth: 0
-    - name: Set up Python 3.11 for docs build
-      uses: actions/setup-python@v5
-      with:
-        python-version: 3.11
-        cache: pip
-        cache-dependency-path: |
-          requirements-docs.txt
-          pyproject.toml
-    - name: Install dependencies
-      run: |
-        pip install -r requirements-docs.txt
-        pip install . --no-deps
-    - name: Build documentation using mike
-      uses: ./.github/actions/mike-docs
-      with:
-        version: development
-        pre_release: true # include pre-release notification banner
-        push: ${{ github.ref == 'refs/heads/main' }} # build always, publish on 'main' only to prevent version clutter
+      - uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+      - name: Set up Python 3.11 for docs build
+        uses: actions/setup-python@v5
+        with:
+          python-version: 3.11
+          cache: pip
+          cache-dependency-path: |
+            requirements-docs.txt
+            pyproject.toml
+      - name: Install dependencies
+        run: |
+          pip install -r requirements-docs.txt
+          pip install . --no-deps
+      - name: Build documentation using mike
+        uses: ./.github/actions/mike-docs
+        with:
+          version: development
+          pre_release: true # include pre-release notification banner
+          push: ${{ github.ref == 'refs/heads/main' }} # build always, publish on 'main' only to prevent version clutter
```

### Comparing `lakefs-spec-0.7.1/.github/workflows/release.yaml` & `lakefs-spec-0.8.0/.github/workflows/release.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 jobs:
   build:
     name: Build source distribution and wheel
     runs-on: ubuntu-latest
     services:
       lakefs: # required for building documentation
-        image: treeverse/lakefs:1.7.0
+        image: treeverse/lakefs:latest
         ports:
           - 8000:8000
         env:
           LAKEFS_INSTALLATION_USER_NAME: "quickstart"
           LAKEFS_INSTALLATION_ACCESS_KEY_ID: "AKIAIOSFOLQUICKSTART"
           LAKEFS_INSTALLATION_SECRET_ACCESS_KEY: "wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY"
           LAKEFS_DATABASE_TYPE: "local"
@@ -31,15 +31,15 @@
         uses: ./.github/actions/python-deps
         with:
           pythonVersion: 3.11
       - name: Build and check
         run: |
           python -m build
       - name: Upload build artifacts
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: dist
           path: dist
       - name: Publish documentation
         uses: ./.github/actions/mike-docs
         with:
           version: ${{ github.event.release.tag_name }}
@@ -49,15 +49,15 @@
     name: Publish wheels to PyPI
     needs: [build]
     runs-on: ubuntu-latest
     permissions:
       id-token: write
     steps:
       - name: Download build artifacts
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: dist
           path: dist
       - name: Publish distribution 📦 to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           skip-existing: true # tolerate release package file duplicates
```

### Comparing `lakefs-spec-0.7.1/.gitignore` & `lakefs-spec-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/.pre-commit-config.yaml` & `lakefs-spec-0.8.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     rev: v1.8.0
     hooks:
       # See https://github.com/pre-commit/mirrors-mypy/blob/main/.pre-commit-hooks.yaml
       - id: mypy
         types_or: [python, pyi]
         args: [--ignore-missing-imports, --scripts-are-modules]
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.2
+    rev: v0.3.1
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.7
     hooks:
@@ -31,15 +31,15 @@
         args: [-c, pyproject.toml]
         additional_dependencies: ["bandit[toml]"]
   - repo: https://github.com/jsh9/pydoclint
     rev: 0.4.1
     hooks:
       - id: pydoclint
   - repo: https://github.com/jazzband/pip-tools
-    rev: 7.4.0
+    rev: 7.4.1
     hooks:
       - id: pip-compile
         name: pip-compile requirements-dev.txt
         args:
           - --no-annotate
           - --extra=dev
           - --output-file=requirements-dev.txt
```

### Comparing `lakefs-spec-0.7.1/CONTRIBUTING.md` & `lakefs-spec-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/LICENSE` & `lakefs-spec-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/PKG-INFO` & `lakefs-spec-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-spec
-Version: 0.7.1
+Version: 0.8.0
 Summary: An fsspec implementation for lakeFS.
 Author-email: appliedAI Institute for Europe <lakefs-spec@appliedai-institute.de>
 Maintainer-email: Nicholas Junge <n.junge@appliedai-institute.de>, Max Mynter <m.mynter@appliedai-institute.de>, Adrian Rumpold <a.rumpold@appliedai-institute.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/aai-institute/lakefs-spec
 Project-URL: Repository, https://github.com/aai-institute/lakefs-spec.git
 Project-URL: Issues, https://github.com/aai-institute/lakefs-spec/issues
@@ -52,14 +52,15 @@
 Requires-Dist: neoteroi-mkdocs; extra == "docs"
 Requires-Dist: mknotebooks; extra == "docs"
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: black; extra == "docs"
 Requires-Dist: mike; extra == "docs"
 Requires-Dist: appnope; extra == "docs"
+Requires-Dist: docstring-parser; extra == "docs"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/_images/lakefs-spec-logo-light.png">
   <img alt="lakeFS-spec logo" src="docs/_images/lakefs-spec-logo-dark.png">
 </picture>
 
 # lakeFS-spec: An fsspec backend for lakeFS
@@ -94,15 +95,15 @@
 $ poetry add lakefs-spec
 ```
 
 ## Usage
 
 The following usage examples showcase two major ways of using lakeFS-spec: as a low-level filesystem abstraction, and through third-party (data science) libraries.
 
-For a more thorough overview of the features and use cases for lakeFS-spec, see the [user guide](https://lakefs-spec.org/latest/guides/overview/) and [tutorials](https://lakefs-spec.org/latest/guides/tutorials/) sections in the documentation.
+For a more thorough overview of the features and use cases for lakeFS-spec, see the [user guide](https://lakefs-spec.org/latest/guides/) and [tutorials](https://lakefs-spec.org/latest/tutorials/) sections in the documentation.
 
 ### Low-level: As a fsspec filesystem 
 
 The following example shows how to upload a file, create a commit, and read back the committed data using the bare lakeFS filesystem implementation.
 It assumes you have already created a repository named `repo` and have `lakectl` credentials set up on your machine in `~/.lakectl.yaml` (see the [lakeFS quickstart guide](https://docs.lakefs.io/quickstart/) if you are new to lakeFS and need guidance).
 
 ```python
```

### Comparing `lakefs-spec-0.7.1/README.md` & `lakefs-spec-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 $ poetry add lakefs-spec
 ```
 
 ## Usage
 
 The following usage examples showcase two major ways of using lakeFS-spec: as a low-level filesystem abstraction, and through third-party (data science) libraries.
 
-For a more thorough overview of the features and use cases for lakeFS-spec, see the [user guide](https://lakefs-spec.org/latest/guides/overview/) and [tutorials](https://lakefs-spec.org/latest/guides/tutorials/) sections in the documentation.
+For a more thorough overview of the features and use cases for lakeFS-spec, see the [user guide](https://lakefs-spec.org/latest/guides/) and [tutorials](https://lakefs-spec.org/latest/tutorials/) sections in the documentation.
 
 ### Low-level: As a fsspec filesystem 
 
 The following example shows how to upload a file, create a commit, and read back the committed data using the bare lakeFS filesystem implementation.
 It assumes you have already created a repository named `repo` and have `lakectl` credentials set up on your machine in `~/.lakectl.yaml` (see the [lakeFS quickstart guide](https://docs.lakefs.io/quickstart/) if you are new to lakeFS and need guidance).
 
 ```python
```

### Comparing `lakefs-spec-0.7.1/assets/lakefs-spec-logo-all.svg` & `lakefs-spec-0.8.0/assets/lakefs-spec-logo-all.svg`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/CONTRIBUTING.md` & `lakefs-spec-0.8.0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_code/pyarrow_example.py` & `lakefs-spec-0.8.0/docs/_code/pyarrow_example.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_code/quickstart.py` & `lakefs-spec-0.8.0/docs/_code/quickstart.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_images/aai-favicon.png` & `lakefs-spec-0.8.0/docs/_images/aai-favicon.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_images/aai-logo-cropped.png` & `lakefs-spec-0.8.0/docs/_images/aai-logo-cropped.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_images/lakefs-spec-favicon.png` & `lakefs-spec-0.8.0/docs/_images/lakefs-spec-favicon.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_images/lakefs-spec-logo-dark.png` & `lakefs-spec-0.8.0/docs/_images/lakefs-spec-logo-dark.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_images/lakefs-spec-logo-light.png` & `lakefs-spec-0.8.0/docs/_images/lakefs-spec-logo-light.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_images/quickstart-lakefs-repositories.png` & `lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-repositories.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_images/quickstart-lakefs-sample-repo.png` & `lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-sample-repo.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_images/quickstart-lakefs-ui.png` & `lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-ui.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_scripts/jupytext_convert.py` & `lakefs-spec-0.8.0/docs/_scripts/jupytext_convert.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_styles/extra.css` & `lakefs-spec-0.8.0/docs/_styles/extra.css`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_styles/neoteroi-mkdocs.css` & `lakefs-spec-0.8.0/docs/_styles/neoteroi-mkdocs.css`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_styles/theme.css` & `lakefs-spec-0.8.0/docs/_styles/theme.css`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/_theme_overrides/partials/header.html` & `lakefs-spec-0.8.0/docs/_theme_overrides/partials/header.html`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/guides/configuration.md` & `lakefs-spec-0.8.0/docs/guides/configuration.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/guides/filesystem-usage.md` & `lakefs-spec-0.8.0/docs/guides/filesystem-usage.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/guides/index.md` & `lakefs-spec-0.8.0/docs/guides/index.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/guides/integrations.md` & `lakefs-spec-0.8.0/docs/guides/integrations.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/guides/transactions.md` & `lakefs-spec-0.8.0/docs/guides/transactions.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/index.md` & `lakefs-spec-0.8.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/quickstart.md` & `lakefs-spec-0.8.0/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/docs/tutorials/demo_data_science_project.py` & `lakefs-spec-0.8.0/docs/tutorials/demo_data_science_project.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/hack/README.md` & `lakefs-spec-0.8.0/hack/README.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/hack/docker-compose.yml` & `lakefs-spec-0.8.0/hack/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/hack/lakefs-s3-local.yml` & `lakefs-spec-0.8.0/hack/lakefs-s3-local.yml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/mkdocs.yml` & `lakefs-spec-0.8.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/pyproject.toml` & `lakefs-spec-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     "neoteroi-mkdocs",
     "mknotebooks",
     "jupyter",
     "jupytext",                                  # conversion between Jupytext and ipynb notebooks
     "black",                                     # formatting of signatures in docs
     "mike",
     "appnope",                                   # required only on Darwin, but need to include in lockfile
+    "docstring-parser",
 ]
 
 [tool.setuptools]
 package-dir = { "" = "src" }
 
 [tool.setuptools.packages.find]
 where = ["src"]
@@ -131,11 +132,8 @@
 log_cli_level = "WARNING"
 
 [tool.pydoclint]
 style = 'numpy'
 exclude = '\.git|venv'
 
 [tool.coverage.report]
-exclude_also = [
-    "@overload",
-    "raise NotImplementedError"
-]
+exclude_also = ["@overload", "raise NotImplementedError"]
```

### Comparing `lakefs-spec-0.7.1/requirements-dev.txt` & `lakefs-spec-0.8.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/requirements-docs.txt` & `lakefs-spec-0.8.0/requirements-docs.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
 comm==0.2.1
 debugpy==1.8.0
 decorator==5.1.1
 defusedxml==0.7.1
+docstring-parser==0.16
 essentials==1.1.5
 essentials-openapi==1.0.9
 executing==2.0.1
 fastjsonschema==2.19.1
 fqdn==1.5.1
 fsspec==2024.2.0
 ghp-import==2.1.0
```

### Comparing `lakefs-spec-0.7.1/src/lakefs_spec/errors.py` & `lakefs-spec-0.8.0/src/lakefs_spec/errors.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/src/lakefs_spec/spec.py` & `lakefs-spec-0.8.0/src/lakefs_spec/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
-Core interface definitions for file system interaction with lakeFS from Python,
-namely the ``LakeFSFileSystem`` and ``LakeFSFile`` classes.
+Core interface definitions for file system interaction with lakeFS from Python.
+
+In particular, the core ``LakeFSFileSystem`` and ``LakeFSFile`` classes.
 """
 
 from __future__ import annotations
 
 import errno
 import logging
 import operator
@@ -114,21 +115,19 @@
     @cached_property
     def _lakefs_server_version(self):
         with self.wrapped_api_call():
             return tuple(int(t) for t in self.client.version.split("."))
 
     @classmethod
     @overload
-    def _strip_protocol(cls, path: str | os.PathLike[str] | Path) -> str:
-        ...
+    def _strip_protocol(cls, path: str | os.PathLike[str] | Path) -> str: ...
 
     @classmethod
     @overload
-    def _strip_protocol(cls, path: list[str | os.PathLike[str] | Path]) -> list[str]:
-        ...
+    def _strip_protocol(cls, path: list[str | os.PathLike[str] | Path]) -> list[str]: ...
 
     @classmethod
     def _strip_protocol(cls, path):
         """Copied verbatim from the base class, save for the slash rstrip."""
         if isinstance(path, list):
             return [cls._strip_protocol(p) for p in path]
         spath = super()._strip_protocol(path)
@@ -233,15 +232,21 @@
         PermissionError
             If the user does not have sufficient permissions to query object existence.
         """
         path = stringify_path(path)
         repository, ref, resource = parse(path)
         try:
             reference = lakefs.Reference(repository, ref, client=self.client)
-            return reference.object(resource).exists()
+            if reference.object(resource).exists():
+                return True
+            # if it isn't an object, it might be a common prefix (i.e. "directory").
+            children = reference.objects(
+                max_amount=1, prefix=resource.rstrip("/") + "/", delimiter="/"
+            )
+            return len(list(children)) > 0
         except ServerException as e:
             # in case of an error other than "not found", existence cannot be
             # decided, so raise the translated error.
             raise translate_lakefs_error(e)
 
     def cp_file(
         self, path1: str | os.PathLike[str], path2: str | os.PathLike[str], **kwargs: Any
@@ -432,34 +437,31 @@
 
     @overload
     def ls(
         self,
         path: str | os.PathLike[str],
         detail: Literal[True] = ...,
         **kwargs: Any,
-    ) -> list[dict[str, Any]]:
-        ...
+    ) -> list[dict[str, Any]]: ...
 
     @overload
     def ls(
         self,
         path: str | os.PathLike[str],
         detail: Literal[False],
         **kwargs: Any,
-    ) -> list[str]:
-        ...
+    ) -> list[str]: ...
 
     @overload
     def ls(
         self,
         path: str | os.PathLike[str],
         detail: bool = True,
         **kwargs: Any,
-    ) -> list[str] | list[dict[str, Any]]:
-        ...
+    ) -> list[str] | list[dict[str, Any]]: ...
 
     def ls(
         self,
         path: str | os.PathLike[str],
         detail: bool = True,
         **kwargs: Any,
     ) -> list[str] | list[dict[str, Any]]:
```

### Comparing `lakefs-spec-0.7.1/src/lakefs_spec/transaction.py` & `lakefs-spec-0.8.0/src/lakefs_spec/transaction.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/src/lakefs_spec/util.py` & `lakefs-spec-0.8.0/src/lakefs_spec/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Useful utilities for handling lakeFS URIs and results of lakeFS API calls.
 """
+
 from __future__ import annotations
 
 import hashlib
 import os
 import re
 from typing import Any, Callable, Generator, Protocol
```

### Comparing `lakefs-spec-0.7.1/src/lakefs_spec.egg-info/PKG-INFO` & `lakefs-spec-0.8.0/src/lakefs_spec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-spec
-Version: 0.7.1
+Version: 0.8.0
 Summary: An fsspec implementation for lakeFS.
 Author-email: appliedAI Institute for Europe <lakefs-spec@appliedai-institute.de>
 Maintainer-email: Nicholas Junge <n.junge@appliedai-institute.de>, Max Mynter <m.mynter@appliedai-institute.de>, Adrian Rumpold <a.rumpold@appliedai-institute.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/aai-institute/lakefs-spec
 Project-URL: Repository, https://github.com/aai-institute/lakefs-spec.git
 Project-URL: Issues, https://github.com/aai-institute/lakefs-spec/issues
@@ -52,14 +52,15 @@
 Requires-Dist: neoteroi-mkdocs; extra == "docs"
 Requires-Dist: mknotebooks; extra == "docs"
 Requires-Dist: jupyter; extra == "docs"
 Requires-Dist: jupytext; extra == "docs"
 Requires-Dist: black; extra == "docs"
 Requires-Dist: mike; extra == "docs"
 Requires-Dist: appnope; extra == "docs"
+Requires-Dist: docstring-parser; extra == "docs"
 
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/_images/lakefs-spec-logo-light.png">
   <img alt="lakeFS-spec logo" src="docs/_images/lakefs-spec-logo-dark.png">
 </picture>
 
 # lakeFS-spec: An fsspec backend for lakeFS
@@ -94,15 +95,15 @@
 $ poetry add lakefs-spec
 ```
 
 ## Usage
 
 The following usage examples showcase two major ways of using lakeFS-spec: as a low-level filesystem abstraction, and through third-party (data science) libraries.
 
-For a more thorough overview of the features and use cases for lakeFS-spec, see the [user guide](https://lakefs-spec.org/latest/guides/overview/) and [tutorials](https://lakefs-spec.org/latest/guides/tutorials/) sections in the documentation.
+For a more thorough overview of the features and use cases for lakeFS-spec, see the [user guide](https://lakefs-spec.org/latest/guides/) and [tutorials](https://lakefs-spec.org/latest/tutorials/) sections in the documentation.
 
 ### Low-level: As a fsspec filesystem 
 
 The following example shows how to upload a file, create a commit, and read back the committed data using the bare lakeFS filesystem implementation.
 It assumes you have already created a repository named `repo` and have `lakectl` credentials set up on your machine in `~/.lakectl.yaml` (see the [lakeFS quickstart guide](https://docs.lakefs.io/quickstart/) if you are new to lakeFS and need guidance).
 
 ```python
```

### Comparing `lakefs-spec-0.7.1/src/lakefs_spec.egg-info/SOURCES.txt` & `lakefs-spec-0.8.0/src/lakefs_spec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/conftest.py` & `lakefs-spec-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/smoke_tests/test_abstractfilesystem.py` & `lakefs-spec-0.8.0/tests/smoke_tests/test_abstractfilesystem.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/smoke_tests/test_integrations.py` & `lakefs-spec-0.8.0/tests/smoke_tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_checksum.py` & `lakefs-spec-0.8.0/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_copy.py` & `lakefs-spec-0.8.0/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_errors.py` & `lakefs-spec-0.8.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_exists.py` & `lakefs-spec-0.8.0/tests/test_exists.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_fs.py` & `lakefs-spec-0.8.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_get_file.py` & `lakefs-spec-0.8.0/tests/test_get_file.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_info.py` & `lakefs-spec-0.8.0/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_internals.py` & `lakefs-spec-0.8.0/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_lakefs_file.py` & `lakefs-spec-0.8.0/tests/test_lakefs_file.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_ls.py` & `lakefs-spec-0.8.0/tests/test_ls.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_put_file.py` & `lakefs-spec-0.8.0/tests/test_put_file.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_rm.py` & `lakefs-spec-0.8.0/tests/test_rm.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_spec_utils.py` & `lakefs-spec-0.8.0/tests/test_spec_utils.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/test_transactions.py` & `lakefs-spec-0.8.0/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.7.1/tests/util.py` & `lakefs-spec-0.8.0/tests/util.py`

 * *Files identical despite different names*

