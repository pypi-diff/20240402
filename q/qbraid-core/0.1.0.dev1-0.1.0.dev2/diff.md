# Comparing `tmp/qbraid-core-0.1.0.dev1.tar.gz` & `tmp/qbraid-core-0.1.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbraid-core-0.1.0.dev1.tar", last modified: Wed Mar 27 21:56:52 2024, max compression
+gzip compressed data, was "qbraid-core-0.1.0.dev2.tar", last modified: Tue Apr  2 16:52:26 2024, max compression
```

## Comparing `qbraid-core-0.1.0.dev1.tar` & `qbraid-core-0.1.0.dev2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.134991 qbraid-core-0.1.0.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.118991 qbraid-core-0.1.0.dev1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.118991 qbraid-core-0.1.0.dev1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.122990 qbraid-core-0.1.0.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.github/workflows/test-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-03-27 21:56:52.134991 qbraid-core-0.1.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.122990 qbraid-core-0.1.0.dev1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.122990 qbraid-core-0.1.0.dev1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.122990 qbraid-core-0.1.0.dev1/docs/_static/cards/
--rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/_static/cards/jupyter.png
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/_static/cards/python.png
--rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/_static/cards/terminal.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.122990 qbraid-core-0.1.0.dev1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/_static/css/s4defs-roles.css
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/_static/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.122990 qbraid-core-0.1.0.dev1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/api/qbraid_core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/api/qbraid_core.services.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/api/qbraid_core.system.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.126991 qbraid-core-0.1.0.dev1/qbraid_core/
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-27 21:56:52.000000 qbraid-core-0.1.0.dev1/qbraid_core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.126991 qbraid-core-0.1.0.dev1/qbraid_core/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.126991 qbraid-core-0.1.0.dev1/qbraid_core/services/environments/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/environments/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/environments/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/environments/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/environments/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/environments/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/environments/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.130991 qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.130991 qbraid-core-0.1.0.dev1/qbraid_core/system/
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/system/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/system/executables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/system/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/system/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/qbraid_core/system/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.130991 qbraid-core-0.1.0.dev1/qbraid_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-03-27 21:56:52.000000 qbraid-core-0.1.0.dev1/qbraid_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-27 21:56:52.000000 qbraid-core-0.1.0.dev1/qbraid_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 21:56:52.000000 qbraid-core-0.1.0.dev1/qbraid_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-27 21:56:52.000000 qbraid-core-0.1.0.dev1/qbraid_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 21:56:52.000000 qbraid-core-0.1.0.dev1/qbraid_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 21:56:52.134991 qbraid-core-0.1.0.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.130991 qbraid-core-0.1.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.130991 qbraid-core-0.1.0.dev1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/tests/fixtures/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/tests/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:56:52.130991 qbraid-core-0.1.0.dev1/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-03-27 21:56:44.000000 qbraid-core-0.1.0.dev1/tools/verify_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.894622 qbraid-core-0.1.0.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.878622 qbraid-core-0.1.0.dev2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.882622 qbraid-core-0.1.0.dev2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.882622 qbraid-core-0.1.0.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.github/workflows/test-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-02 16:52:26.894622 qbraid-core-0.1.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.882622 qbraid-core-0.1.0.dev2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.882622 qbraid-core-0.1.0.dev2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.882622 qbraid-core-0.1.0.dev2/docs/_static/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)     6497 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/_static/cards/jupyter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/_static/cards/python.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26055 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/_static/cards/terminal.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.882622 qbraid-core-0.1.0.dev2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     5914 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/_static/css/s4defs-roles.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   154811 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/_static/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.886622 qbraid-core-0.1.0.dev2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/api/qbraid_core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/api/qbraid_core.services.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/api/qbraid_core.system.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.886622 qbraid-core-0.1.0.dev2/qbraid_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-02 16:52:26.000000 qbraid-core-0.1.0.dev2/qbraid_core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.886622 qbraid-core-0.1.0.dev2/qbraid_core/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.890622 qbraid-core-0.1.0.dev2/qbraid_core/services/environments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/environments/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/environments/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/environments/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/environments/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/environments/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/environments/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.890622 qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.890622 qbraid-core-0.1.0.dev2/qbraid_core/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/system/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/system/executables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/system/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/system/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/qbraid_core/system/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.890622 qbraid-core-0.1.0.dev2/qbraid_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5666 2024-04-02 16:52:26.000000 qbraid-core-0.1.0.dev2/qbraid_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-02 16:52:26.000000 qbraid-core-0.1.0.dev2/qbraid_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:52:26.000000 qbraid-core-0.1.0.dev2/qbraid_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 16:52:26.000000 qbraid-core-0.1.0.dev2/qbraid_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 16:52:26.000000 qbraid-core-0.1.0.dev2/qbraid_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 16:52:26.894622 qbraid-core-0.1.0.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.890622 qbraid-core-0.1.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.890622 qbraid-core-0.1.0.dev2/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/tests/fixtures/environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/tests/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:52:26.890622 qbraid-core-0.1.0.dev2/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-02 16:52:18.000000 qbraid-core-0.1.0.dev2/tools/verify_headers.py
```

### Comparing `qbraid-core-0.1.0.dev1/.github/ISSUE_TEMPLATE/bug_report.yml` & `qbraid-core-0.1.0.dev2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/.github/ISSUE_TEMPLATE/feature_request.yml` & `qbraid-core-0.1.0.dev2/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/.github/workflows/docs.yml` & `qbraid-core-0.1.0.dev2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/.github/workflows/format.yml` & `qbraid-core-0.1.0.dev2/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/.github/workflows/main.yml` & `qbraid-core-0.1.0.dev2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/.github/workflows/publish.yml` & `qbraid-core-0.1.0.dev2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/.github/workflows/test-publish.yml` & `qbraid-core-0.1.0.dev2/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/.gitignore` & `qbraid-core-0.1.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/LICENSE` & `qbraid-core-0.1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/PKG-INFO` & `qbraid-core-0.1.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.0.dev1/README.md` & `qbraid-core-0.1.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/Makefile` & `qbraid-core-0.1.0.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/_static/cards/jupyter.png` & `qbraid-core-0.1.0.dev2/docs/_static/cards/jupyter.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/_static/cards/python.png` & `qbraid-core-0.1.0.dev2/docs/_static/cards/python.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/_static/cards/terminal.png` & `qbraid-core-0.1.0.dev2/docs/_static/cards/terminal.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/_static/css/custom.css` & `qbraid-core-0.1.0.dev2/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/_static/css/s4defs-roles.css` & `qbraid-core-0.1.0.dev2/docs/_static/css/s4defs-roles.css`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/_static/favicon.ico` & `qbraid-core-0.1.0.dev2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/_static/logo.png` & `qbraid-core-0.1.0.dev2/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/conf.py` & `qbraid-core-0.1.0.dev2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/index.rst` & `qbraid-core-0.1.0.dev2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/docs/make.bat` & `qbraid-core-0.1.0.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/pyproject.toml` & `qbraid-core-0.1.0.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qbraid-core"
-version = "0.1.0.dev1"
+version = "0.1.0.dev2"
 authors = [
     {name = "qBraid Development Team", email = "contact@qbraid.com"},
 ]
 description = "Python library with core abstractions for software development in the qBraid ecosystem."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["qbraid", "quantum", "cloud"]
```

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/__init__.py` & `qbraid-core-0.1.0.dev2/qbraid_core/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/client.py` & `qbraid-core-0.1.0.dev2/qbraid_core/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/exceptions.py` & `qbraid-core-0.1.0.dev2/qbraid_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/registry.py` & `qbraid-core-0.1.0.dev2/qbraid_core/registry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/retry.py` & `qbraid-core-0.1.0.dev2/qbraid_core/retry.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/environments/__init__.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/environments/client.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/environments/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/environments/create.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/environments/create.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/environments/paths.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/environments/paths.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/environments/state.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/environments/state.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/environments/validate.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/environments/validate.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/__init__.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/adapter.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/adapter.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/client.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/services/quantum/proxy.py` & `qbraid-core-0.1.0.dev2/qbraid_core/services/quantum/proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,55 +18,56 @@
 logger = logging.getLogger(__name__)
 
 SUPPORTED_QJOB_LIBS = ["braket"]
 
 
 def _check_proxy(
     proxy_spec: Tuple[str, ...], slug_path: Optional[Path] = None
-) -> Tuple[bool, bool]:
+) -> Tuple[bool, bool, Path]:
     """
     Checks if the specified proxy file exists and contains the string 'qbraid'.
 
     Args:
         proxy_spec (Tuple[str, ...]): A tuple specifying the path components from 'site-packages'
                                       to the target proxy file, e.g. ("botocore", "httpsession.py").
         slug_path (optional, Path): The base path to prepend to the 'pyenv' directory.
 
     Returns:
-        A tuple of two booleans: The first indicates whether the specified proxy file exists;
-        the second, if the file exists, is True if it contains 'qbraid', False otherwise.
+        A tuple of two booleans and sitepackages path: The first bool indicates whether the specified proxy file exists;
+        the second bool, if the file exists, is True if it contains 'qbraid', False otherwise. The sitepackages path gives
+        the location of the site-packages directory where the proxy file is located.
     """
     try:
         if slug_path is None:
             site_packages: str = get_active_site_packages_path()
             site_packages_path = Path(site_packages)
         else:
             site_packages_path = get_venv_site_packages_path(slug_path / "pyenv")
     except QbraidException as err:
         logger.debug(err)
-        return False, False
+        return False, False, site_packages_path
 
     target_file_path = site_packages_path.joinpath(*proxy_spec)
 
     if not target_file_path.exists():
-        return False, False
+        return False, False, site_packages_path
 
     try:
         with target_file_path.open("r", encoding="utf-8") as file:
             for line in file:
                 if "qbraid" in line:
                     return True, True, site_packages_path
-        return True, False
+        return True, False, site_packages_path
     except Exception as err:  # pylint: disable=broad-exception-caught
         logger.debug("Unexpected error checking qBraid proxy: %s", err)
 
-    return True, False
+    return True, False, site_packages_path
 
 
-def quantum_lib_proxy_state(device_lib: str) -> Dict[str, Union[str, bool]]:
+def quantum_lib_proxy_state(device_lib: str, **kwargs) -> Dict[str, Union[str, bool]]:
     """Checks if qBraid Quantum Jobs are supported and if so, checks whether they are enabled.
     Returns dictionary providing information about the state of qBraid Quantum Jobs support
     and configuration for the given quantum device library.
 
     Args:
         device_lib (str): The name of the quantum device library, e.g., "braket".
 
@@ -87,15 +88,16 @@
 
     if device_lib not in SUPPORTED_QJOB_LIBS:
         raise ValueError(f"Unsupported quantum job library. Expected one of {SUPPORTED_QJOB_LIBS}")
 
     if device_lib == "braket":
         proxy_lib = "botocore"
         proxy_spec = (proxy_lib, "httpsession.py")
-        supported, enabled = _check_proxy(proxy_spec)
+        supported, enabled, path = _check_proxy(proxy_spec, **kwargs)
 
     # add more device libraries here as needed
 
     state["proxy_lib"] = proxy_lib
     state["supported"] = supported
     state["enabled"] = enabled
+    state["path"] = str(path)
     return state
```

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/session.py` & `qbraid-core-0.1.0.dev2/qbraid_core/session.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/system/__init__.py` & `qbraid-core-0.1.0.dev2/qbraid_core/system/__init__.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/system/executables.py` & `qbraid-core-0.1.0.dev2/qbraid_core/system/executables.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/system/generic.py` & `qbraid-core-0.1.0.dev2/qbraid_core/system/generic.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/system/packages.py` & `qbraid-core-0.1.0.dev2/qbraid_core/system/packages.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core/system/threader.py` & `qbraid-core-0.1.0.dev2/qbraid_core/system/threader.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core.egg-info/PKG-INFO` & `qbraid-core-0.1.0.dev2/qbraid_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbraid-core
-Version: 0.1.0.dev1
+Version: 0.1.0.dev2
 Summary: Python library with core abstractions for software development in the qBraid ecosystem.
 Author-email: qBraid Development Team <contact@qbraid.com>
 License: Proprietary
 Project-URL: Homepage, https://www.qbraid.com/
 Project-URL: Documentation, https://docs.qbraid.com/projects/core/en/latest/
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
 Project-URL: Discord, https://discord.gg/KugF6Cnncm
```

### Comparing `qbraid-core-0.1.0.dev1/qbraid_core.egg-info/SOURCES.txt` & `qbraid-core-0.1.0.dev2/qbraid_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/tests/fixtures/environments.py` & `qbraid-core-0.1.0.dev2/tests/fixtures/environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/tests/test_client.py` & `qbraid-core-0.1.0.dev2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/tests/test_environments.py` & `qbraid-core-0.1.0.dev2/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/tests/test_session.py` & `qbraid-core-0.1.0.dev2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/tests/test_system.py` & `qbraid-core-0.1.0.dev2/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `qbraid-core-0.1.0.dev1/tools/verify_headers.py` & `qbraid-core-0.1.0.dev2/tools/verify_headers.py`

 * *Files identical despite different names*

