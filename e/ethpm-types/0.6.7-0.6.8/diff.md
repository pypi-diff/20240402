# Comparing `tmp/ethpm-types-0.6.7.tar.gz` & `tmp/ethpm-types-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ethpm-types-0.6.7.tar", last modified: Wed Jan  3 17:26:14 2024, max compression
+gzip compressed data, was "ethpm-types-0.6.8.tar", last modified: Tue Apr  2 15:32:14 2024, max compression
```

## Comparing `ethpm-types-0.6.7.tar` & `ethpm-types-0.6.8.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.827521 ethpm-types-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.799521 ethpm-types-0.6.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.799521 ethpm-types-0.6.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.803521 ethpm-types-0.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-01-03 17:26:14.827521 ethpm-types-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.803521 ethpm-types-0.6.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.803521 ethpm-types-0.6.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.803521 ethpm-types-0.6.7/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.803521 ethpm-types-0.6.7/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/methoddocs/abi.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/methoddocs/contract_type.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/methoddocs/manifest.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/methoddocs/source.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.803521 ethpm-types-0.6.7/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/docs/userguides/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.807521 ethpm-types-0.6.7/ethpm_types/
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/contract_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26552 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/ethpm_types/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-03 17:26:14.000000 ethpm-types-0.6.7/ethpm_types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.807521 ethpm-types-0.6.7/ethpm_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-01-03 17:26:14.000000 ethpm-types-0.6.7/ethpm_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-01-03 17:26:14.000000 ethpm-types-0.6.7/ethpm_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 17:26:14.000000 ethpm-types-0.6.7/ethpm_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 17:26:14.000000 ethpm-types-0.6.7/ethpm_types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-01-03 17:26:14.000000 ethpm-types-0.6.7/ethpm_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-03 17:26:14.000000 ethpm-types-0.6.7/ethpm_types.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-03 17:26:14.827521 ethpm-types-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.807521 ethpm-types-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.799521 ethpm-types-0.6.7/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.823521 ethpm-types-0.6.7/tests/data/Compiled/
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Compiled/HasError.json
--rw-r--r--   0 runner    (1001) docker     (127) 12327472 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Compiled/OpenZeppelinContracts.json
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Compiled/SolFallbackAndReceive.json
--rw-r--r--   0 runner    (1001) docker     (127)   227889 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Compiled/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Compiled/TestStrategy.srcmap
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Compiled/VyDefault.json
--rw-r--r--   0 runner    (1001) docker     (127)   230644 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Compiled/VyperContract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 17:26:14.827521 ethpm-types-0.6.7/tests/data/Sources/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Sources/SolFallbackAndReceive.sol
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Sources/SolidityContract.sol
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Sources/VyDefault.vy
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/data/Sources/VyperContract.vy
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_ast.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_cairo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12989 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_package_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_pc_map.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_schema_fuzzing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_sourcemap.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-03 17:25:55.000000 ethpm-types-0.6.7/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:14.010696 ethpm-types-0.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-02 15:32:14.010696 ethpm-types-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/abi.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/contract_type.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/manifest.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/source.md
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.986696 ethpm-types-0.6.8/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/docs/userguides/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.990696 ethpm-types-0.6.8/ethpm_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11035 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16573 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    26564 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/ethpm_types/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.990696 ethpm-types-0.6.8/ethpm_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 15:32:13.000000 ethpm-types-0.6.8/ethpm_types.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-02 15:32:14.010696 ethpm-types-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.990696 ethpm-types-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5105 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:13.982696 ethpm-types-0.6.8/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:14.006696 ethpm-types-0.6.8/tests/data/Compiled/
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/HasError.json
+-rw-r--r--   0 runner    (1001) docker     (127) 12327472 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/OpenZeppelinContracts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/SolFallbackAndReceive.json
+-rw-r--r--   0 runner    (1001) docker     (127)   227889 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/TestStrategy.srcmap
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/VyDefault.json
+-rw-r--r--   0 runner    (1001) docker     (127)   230644 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Compiled/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:32:14.010696 ethpm-types-0.6.8/tests/data/Sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/SolFallbackAndReceive.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/SolidityContract.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/VyDefault.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/data/Sources/VyperContract.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_cairo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13640 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9215 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_package_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_pc_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_schema_fuzzing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10539 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_sourcemap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 15:31:50.000000 ethpm-types-0.6.8/tests/test_utils.py
```

### Comparing `ethpm-types-0.6.7/.github/ISSUE_TEMPLATE/bug.md` & `ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/.github/ISSUE_TEMPLATE/feature.md` & `ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/.github/ISSUE_TEMPLATE/work-item.md` & `ethpm-types-0.6.8/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/.github/release-drafter.yml` & `ethpm-types-0.6.8/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/.github/workflows/commitlint.yaml` & `ethpm-types-0.6.8/.github/workflows/commitlint.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install -r cz-requirement.txt
```

### Comparing `ethpm-types-0.6.7/.github/workflows/docs.yaml` & `ethpm-types-0.6.8/.github/workflows/docs.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -9,31 +9,31 @@
         types: [opened, synchronize]
 
 jobs:
     docs:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[doc]
 
         - name: Build HTML artifact
           run: python build_docs.py
 
         - name: Upload HTML artifact
-          uses: actions/upload-artifact@v1
+          uses: actions/upload-artifact@v4
           with:
               name: DocumentationHTML
               path: docs/_build/ethpm-types
 
         - name: Commit and publish documentation changes to gh-pages branch
           run: |
               if [[ "${GITHUB_EVENT_NAME}" =~ "pull_request" ]]; then
```

### Comparing `ethpm-types-0.6.7/.github/workflows/prtitle.yaml` & `ethpm-types-0.6.8/.github/workflows/prtitle.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install -r cz-requirement.txt
 
         - name: Check PR Title
```

### Comparing `ethpm-types-0.6.7/.github/workflows/publish.yaml` & `ethpm-types-0.6.8/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ethpm-types-0.6.7/.github/workflows/test.yaml` & `ethpm-types-0.6.8/.github/workflows/test.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -13,18 +13,18 @@
    GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
@@ -38,18 +38,18 @@
         - name: Run flake8
           run: flake8 .
 
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
@@ -62,18 +62,18 @@
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
                 python-version: [3.8, 3.9, "3.10"]  # eventually add 3.11
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
@@ -85,18 +85,18 @@
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v3
+#        - uses: actions/checkout@v4
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v4
+#          uses: actions/setup-python@v5
 #          with:
 #              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ethpm-types-0.6.7/.gitignore` & `ethpm-types-0.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/.pre-commit-config.yaml` & `ethpm-types-0.6.8/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 
 -   repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.11.0
+    rev: 24.2.0
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.9.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-requests, types-setuptools, pydantic]
 
 
 default_language_version:
     python: python3
```

### Comparing `ethpm-types-0.6.7/CONTRIBUTING.md` & `ethpm-types-0.6.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/LICENSE` & `ethpm-types-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/PKG-INFO` & `ethpm-types-0.6.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.6.7
+Version: 0.6.8
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.6.7/README.md` & `ethpm-types-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/build_docs.py` & `ethpm-types-0.6.8/build_docs.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/docs/_static/custom.css` & `ethpm-types-0.6.8/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/docs/_static/custom.js` & `ethpm-types-0.6.8/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/docs/_templates/layout.html` & `ethpm-types-0.6.8/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/docs/conf.py` & `ethpm-types-0.6.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/docs/favicon.ico` & `ethpm-types-0.6.8/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/docs/logo.gif` & `ethpm-types-0.6.8/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/ethpm_types/__init__.py` & `ethpm-types-0.6.8/ethpm_types/__init__.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/ethpm_types/abi.py` & `ethpm-types-0.6.8/ethpm_types/abi.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,16 +89,15 @@
             sig += " indexed"
         if self.name:
             sig += f" {self.name}"
 
         return sig
 
 
-class BaseABI(BaseModel):
-    ...
+class BaseABI(BaseModel): ...
 
 
 class ConstructorABI(BaseABI):
     """
     An ABI describing a contract constructor.
     **NOTE**: The constructor ABI does not have a ``name`` property.
     """
```

### Comparing `ethpm-types-0.6.7/ethpm_types/ast.py` & `ethpm-types-0.6.8/ethpm_types/ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/ethpm_types/base.py` & `ethpm-types-0.6.8/ethpm_types/base.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/ethpm_types/contract_type.py` & `ethpm-types-0.6.8/ethpm_types/contract_type.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/ethpm_types/manifest.py` & `ethpm-types-0.6.8/ethpm_types/manifest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/ethpm_types/source.py` & `ethpm-types-0.6.8/ethpm_types/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,15 @@
 
         elif isinstance(model, dict) and isinstance(model.get("content"), str):
             content = model["content"]
             other_props = {k: v for k, v in model.items() if k != "content"}
 
         content_result = (
             {"content": Content(root={i + 1: x for i, x in enumerate(content.splitlines())})}
-            if content
+            if content is not None
             else model
         )
         return {**content_result, **other_props}
 
     def __repr__(self) -> str:
         repr_id = "Source"
```

### Comparing `ethpm-types-0.6.7/ethpm_types/sourcemap.py` & `ethpm-types-0.6.8/ethpm_types/sourcemap.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/ethpm_types/utils.py` & `ethpm-types-0.6.8/ethpm_types/utils.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/ethpm_types.egg-info/PKG-INFO` & `ethpm-types-0.6.8/ethpm_types.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethpm-types
-Version: 0.6.7
+Version: 0.6.8
 Summary: ethpm_types: Implementation of EIP-2678
 Home-page: https://github.com/ApeWorX/ethpm-types
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ethpm-types-0.6.7/ethpm_types.egg-info/SOURCES.txt` & `ethpm-types-0.6.8/ethpm_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/ethpm_types.egg-info/requires.txt` & `ethpm-types-0.6.8/ethpm_types.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 PyGithub<2.0,>=1.54
 hypothesis-jsonschema==0.19.0
-black<24,>=23.11.0
-mypy<2,>=1.7.1
+black<25,>=24.2.0
+mypy<2,>=1.9.0
 types-setuptools
 types-requests
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
 isort<6,>=5.10.1
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
@@ -30,26 +30,26 @@
 commitizen<2.41,>=2.40
 pre-commit
 pytest-watch
 IPython
 ipdb
 
 [doc]
-myst-parser<0.18,>=0.17.0
-sphinx-click<4.0,>=3.1.0
-Sphinx<5.0,>=4.4.0
-sphinx_rtd_theme<2,>=1.0.0
+myst-parser<2,>=1.0.0
+sphinx-click<5,>=4.4.0
+Sphinx<7,>=6.1.3
+sphinx_rtd_theme<2,>=1.2.0
 sphinxcontrib-napoleon>=0.7
 
 [lint]
-black<24,>=23.11.0
-mypy<2,>=1.7.1
+black<25,>=24.2.0
+mypy<2,>=1.9.0
 types-setuptools
 types-requests
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
 isort<6,>=5.10.1
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
```

### Comparing `ethpm-types-0.6.7/pyproject.toml` & `ethpm-types-0.6.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/setup.py` & `ethpm-types-0.6.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,32 +13,32 @@
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         # Test-only deps
         "PyGithub>=1.54,<2.0",  # Necessary to pull official schema from github
         "hypothesis-jsonschema==0.19.0",  # Fuzzes based on a json schema
     ],
     "lint": [
-        "black>=23.11.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.2.0,<25",  # Auto-formatter and linter
+        "mypy>=1.9.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
         "types-requests",  # Needed for mypy type shed
-        "flake8>=6.1.0,<7",  # Style linter
+        "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
         "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "doc": [
-        "myst-parser>=0.17.0,<0.18",  # Tools for parsing markdown files in the docs
-        "sphinx-click>=3.1.0,<4.0",  # For documenting CLI
-        "Sphinx>=4.4.0,<5.0",  # Documentation generator
-        "sphinx_rtd_theme>=1.0.0,<2",  # Readthedocs.org theme
+        "myst-parser>=1.0.0,<2",  # Parse markdown docs
+        "sphinx-click>=4.4.0,<5",  # For documenting CLI
+        "Sphinx>=6.1.3,<7",  # Documentation generator
+        "sphinx_rtd_theme>=1.2.0,<2",  # Readthedocs.org theme
         "sphinxcontrib-napoleon>=0.7",  # Allow Google-style documentation
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
         "wheel",  # Packaging tool
         "twine",  # Package upload tool
     ],
```

### Comparing `ethpm-types-0.6.7/tests/conftest.py` & `ethpm-types-0.6.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/data/Compiled/HasError.json` & `ethpm-types-0.6.8/tests/data/Compiled/HasError.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/data/Compiled/OpenZeppelinContracts.json` & `ethpm-types-0.6.8/tests/data/Compiled/OpenZeppelinContracts.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/data/Compiled/SolFallbackAndReceive.json` & `ethpm-types-0.6.8/tests/data/Compiled/SolFallbackAndReceive.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/data/Compiled/SolidityContract.json` & `ethpm-types-0.6.8/tests/data/Compiled/SolidityContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/data/Compiled/TestStrategy.srcmap` & `ethpm-types-0.6.8/tests/data/Compiled/TestStrategy.srcmap`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/data/Compiled/VyDefault.json` & `ethpm-types-0.6.8/tests/data/Compiled/VyDefault.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/data/Compiled/VyperContract.json` & `ethpm-types-0.6.8/tests/data/Compiled/VyperContract.json`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/data/Sources/SolidityContract.sol` & `ethpm-types-0.6.8/tests/data/Sources/SolidityContract.sol`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/data/Sources/VyperContract.vy` & `ethpm-types-0.6.8/tests/data/Sources/VyperContract.vy`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/test_abi.py` & `ethpm-types-0.6.8/tests/test_abi.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/test_ast.py` & `ethpm-types-0.6.8/tests/test_ast.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/test_cairo.py` & `ethpm-types-0.6.8/tests/test_cairo.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/test_contract_type.py` & `ethpm-types-0.6.8/tests/test_contract_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -345,7 +345,29 @@
     assert vyper_contract.identifier_lookup["0x8da5cb5b"].selector == "owner()"
     assert (
         vyper_contract.identifier_lookup[
             "0x1a7c56fae0af54ebae73bc4699b9de9835e7bb86b050dff7e80695b633f17abd"
         ].selector
         == "FooHappened(uint256)"
     )
+
+
+def test_get_runtime_bytecode(vyper_contract):
+    actual = vyper_contract.get_runtime_bytecode()
+    assert actual.hex().startswith("0x")
+
+
+def test_get_runtime_bytecode_no_code(vyper_contract):
+    vyper_contract.runtime_bytecode = None
+    actual = vyper_contract.get_runtime_bytecode()
+    assert actual is None
+
+
+def test_get_deployment_bytecode(vyper_contract):
+    actual = vyper_contract.get_deployment_bytecode()
+    assert actual.hex().startswith("0x")
+
+
+def test_get_deployment_bytecode_no_code(vyper_contract):
+    vyper_contract.deployment_bytecode = None
+    actual = vyper_contract.get_deployment_bytecode()
+    assert actual is None
```

### Comparing `ethpm-types-0.6.7/tests/test_package_manifest.py` & `ethpm-types-0.6.8/tests/test_package_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,18 @@
         "foobar": ContractType(contractName="foobar", abi=[]),
         "testtest": ContractType(contractName="testtest", abi=[]),
     }
 
     manifest = PackageManifest(contractTypes=contract_types)
     assert manifest.contract_types == contract_types
 
+    # Show we can also set them.
+    manifest.contract_types = {}
+    assert manifest.contract_types == {}
+
 
 def test_validate_fields(package_manifest):
     """
     Mimics a FastAPI internal behavior.
     """
 
     raw_data = package_manifest.model_dump()
```

### Comparing `ethpm-types-0.6.7/tests/test_pc_map.py` & `ethpm-types-0.6.8/tests/test_pc_map.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/test_schema_fuzzing.py` & `ethpm-types-0.6.8/tests/test_schema_fuzzing.py`

 * *Files identical despite different names*

### Comparing `ethpm-types-0.6.7/tests/test_source.py` & `ethpm-types-0.6.8/tests/test_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,7 +312,18 @@
 def test_references():
     """
     Tests against a bug where the model validation
     would accidentally ignore all extra properties.
     """
     source = Source(content="foo\n", references=["bar.txt"])
     assert source.references == ["bar.txt"]
+
+
+def test_model_validate_empty_str():
+    """
+    There was a bug where if a file was empty,
+    it would try to use the empty str as a
+    dict to create the source content, due to an improper
+    truthy check.
+    """
+    source = Source.model_validate("")
+    assert isinstance(source, Source)
```

### Comparing `ethpm-types-0.6.7/tests/test_sourcemap.py` & `ethpm-types-0.6.8/tests/test_sourcemap.py`

 * *Files identical despite different names*

