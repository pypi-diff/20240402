# Comparing `tmp/sciline-24.2.1.tar.gz` & `tmp/sciline-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sciline-24.2.1.tar", last modified: Mon Feb 19 09:14:57 2024, max compression
+gzip compressed data, was "sciline-24.4.0.tar", last modified: Tue Apr  2 13:19:07 2024, max compression
```

## Comparing `sciline-24.2.1.tar` & `sciline-24.4.0.tar`

### file list

```diff
@@ -1,125 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.538624 sciline-24.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-19 09:14:47.000000 sciline-24.2.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.526624 sciline-24.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-19 09:14:47.000000 sciline-24.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.526624 sciline-24.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-19 09:14:47.000000 sciline-24.2.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-19 09:14:47.000000 sciline-24.2.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-19 09:14:47.000000 sciline-24.2.1/.github/workflows/nightly_at_main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-19 09:14:47.000000 sciline-24.2.1/.github/workflows/nightly_at_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-19 09:14:47.000000 sciline-24.2.1/.github/workflows/python-version-ci
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-02-19 09:14:47.000000 sciline-24.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-02-19 09:14:47.000000 sciline-24.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-19 09:14:47.000000 sciline-24.2.1/.github/workflows/unpinned.yml
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-19 09:14:47.000000 sciline-24.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-19 09:14:47.000000 sciline-24.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-02-19 09:14:47.000000 sciline-24.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-02-19 09:14:47.000000 sciline-24.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-19 09:14:47.000000 sciline-24.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-19 09:14:47.000000 sciline-24.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-02-19 09:14:57.538624 sciline-24.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-02-19 09:14:47.000000 sciline-24.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.526624 sciline-24.2.1/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-19 09:14:47.000000 sciline-24.2.1/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.526624 sciline-24.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.526624 sciline-24.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/_static/anaconda-icon.js
--rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    75109 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/_static/logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    75109 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.526624 sciline-24.2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/_templates/class-template.rst
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/_templates/doc_version.html
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/_templates/module-template.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.526624 sciline-24.2.1/docs/about/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/about/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.526624 sciline-24.2.1/docs/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.530624 sciline-24.2.1/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.530624 sciline-24.2.1/docs/developer/architecture-and-design/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/developer/architecture-and-design/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/developer/architecture-and-design/workflow-design.md
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/developer/coding-conventions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/developer/dependency-management.md
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/developer/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/developer/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.530624 sciline-24.2.1/docs/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/recipes/applying-decorators.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/recipes/continue-from-intermediate-results.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/recipes/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/recipes/replacing-providers.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/recipes/side-effects-and-file-writing.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.530624 sciline-24.2.1/docs/user-guide/
--rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/user-guide/generic-providers.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/user-guide/getting-started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/user-guide/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-02-19 09:14:47.000000 sciline-24.2.1/docs/user-guide/parameter-tables.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-19 09:14:47.000000 sciline-24.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.534624 sciline-24.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/basetest.in
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/basetest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/make_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/mypy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/nightly.in
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/nightly.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/static.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/test-dask.in
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/test-dask.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/wheels.in
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-19 09:14:47.000000 sciline-24.2.1/requirements/wheels.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.534624 sciline-24.2.1/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-02-19 09:14:47.000000 sciline-24.2.1/resources/sciline.svg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-19 09:14:57.538624 sciline-24.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.522624 sciline-24.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.534624 sciline-24.2.1/src/sciline/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/param_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    35451 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.538624 sciline-24.2.1/src/sciline/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/sphinxext/domain_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/task_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-02-19 09:14:47.000000 sciline-24.2.1/src/sciline/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.538624 sciline-24.2.1/src/sciline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-02-19 09:14:57.000000 sciline-24.2.1/src/sciline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-02-19 09:14:57.000000 sciline-24.2.1/src/sciline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 09:14:57.000000 sciline-24.2.1/src/sciline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-19 09:14:57.000000 sciline-24.2.1/src/sciline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 09:14:57.538624 sciline-24.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/_provider_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/complex_workflow_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/dask_scheduler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/domain_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/param_table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    37130 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/pipeline_with_optional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24333 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/pipeline_with_param_table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/pipeline_with_postponed_annotations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/task_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-02-19 09:14:47.000000 sciline-24.2.1/tests/visualize_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-02-19 09:14:47.000000 sciline-24.2.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.089929 sciline-24.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-02 13:18:56.000000 sciline-24.4.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.069929 sciline-24.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/nightly_at_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/nightly_at_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/python-version-ci
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-02 13:18:56.000000 sciline-24.4.0/.github/workflows/unpinned.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-02 13:18:56.000000 sciline-24.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-02 13:18:56.000000 sciline-24.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-02 13:18:56.000000 sciline-24.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-02 13:18:56.000000 sciline-24.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-02 13:18:56.000000 sciline-24.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 13:18:56.000000 sciline-24.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-02 13:19:07.089929 sciline-24.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-02 13:18:56.000000 sciline-24.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-02 13:18:56.000000 sciline-24.4.0/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_static/anaconda-icon.js
+-rw-r--r--   0 runner    (1001) docker     (127)   137750 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    75109 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_static/logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    75109 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_templates/class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_templates/doc_version.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/_templates/module-template.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/about/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/about/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.073929 sciline-24.4.0/docs/developer/architecture-and-design/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/architecture-and-design/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/architecture-and-design/workflow-design.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/coding-conventions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/dependency-management.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/developer/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.077929 sciline-24.4.0/docs/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/applying-decorators.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/continue-from-intermediate-results.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4601 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/replacing-providers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/recipes/side-effects-and-file-writing.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.077929 sciline-24.4.0/docs/user-guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/generic-providers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/getting-started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14937 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/parameter-tables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-02 13:18:56.000000 sciline-24.4.0/docs/user-guide/provenance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-02 13:18:56.000000 sciline-24.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.081929 sciline-24.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/basetest.in
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/basetest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/make_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/mypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/nightly.in
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/nightly.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/static.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/test-dask.in
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/test-dask.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/wheels.in
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-02 13:18:56.000000 sciline-24.4.0/requirements/wheels.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.081929 sciline-24.4.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-04-02 13:18:56.000000 sciline-24.4.0/resources/sciline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 13:19:07.089929 sciline-24.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.069929 sciline-24.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.081929 sciline-24.4.0/src/sciline/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/param_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35503 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/src/sciline/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/serialize/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/serialize/graph_json_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/src/sciline/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5257 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/sphinxext/domain_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/task_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-04-02 13:18:56.000000 sciline-24.4.0/src/sciline/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/src/sciline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-02 13:19:07.000000 sciline-24.4.0/src/sciline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-02 13:19:07.000000 sciline-24.4.0/src/sciline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:19:07.000000 sciline-24.4.0/src/sciline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-02 13:19:07.000000 sciline-24.4.0/src/sciline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/_provider_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/complex_workflow_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/dask_scheduler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/param_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40014 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/pipeline_with_optional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24917 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/pipeline_with_param_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/pipeline_with_postponed_annotations_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:19:07.085929 sciline-24.4.0/tests/serialize/
+-rw-r--r--   0 runner    (1001) docker     (127)    11394 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/serialize/json_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/task_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-02 13:18:56.000000 sciline-24.4.0/tests/visualize_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-02 13:18:56.000000 sciline-24.4.0/tox.ini
```

### Comparing `sciline-24.2.1/.github/workflows/ci.yml` & `sciline-24.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/.github/workflows/docs.yml` & `sciline-24.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/.github/workflows/nightly_at_main.yml` & `sciline-24.4.0/.github/workflows/nightly_at_main.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/.github/workflows/nightly_at_release.yml` & `sciline-24.4.0/.github/workflows/nightly_at_release.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/.github/workflows/release.yml` & `sciline-24.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/.github/workflows/test.yml` & `sciline-24.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/.github/workflows/unpinned.yml` & `sciline-24.4.0/.github/workflows/unpinned.yml`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/.pre-commit-config.yaml` & `sciline-24.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/CODE_OF_CONDUCT.md` & `sciline-24.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/CONTRIBUTING.md` & `sciline-24.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/LICENSE` & `sciline-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/PKG-INFO` & `sciline-24.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciline
-Version: 24.2.1
+Version: 24.4.0
 Summary: Build scientific pipelines for your data
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `sciline-24.2.1/README.md` & `sciline-24.4.0/README.md`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/conda/meta.yaml` & `sciline-24.4.0/conda/meta.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 test:
   imports:
     - sciline
   requires:
     - dask
     - python-graphviz
+    - jsonschema
     - numpy
     - pytest
   source_files:
     - pyproject.toml
     - tests/
   commands:
     # We ignore warnings during release package builds
```

### Comparing `sciline-24.2.1/docs/_static/anaconda-icon.js` & `sciline-24.4.0/docs/_static/anaconda-icon.js`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/_static/favicon.ico` & `sciline-24.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/_static/logo-dark.svg` & `sciline-24.4.0/docs/_static/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/_static/logo.svg` & `sciline-24.4.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/_templates/class-template.rst` & `sciline-24.4.0/docs/_templates/class-template.rst`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/_templates/module-template.rst` & `sciline-24.4.0/docs/_templates/module-template.rst`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/about/index.md` & `sciline-24.4.0/docs/about/index.md`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/api-reference/index.md` & `sciline-24.4.0/docs/api-reference/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    ParamTable
    Pipeline
    Scope
    Series
    scheduler.Scheduler
    scheduler.DaskScheduler
    scheduler.NaiveScheduler
-   task_graph.TaskGraph
+   TaskGraph
 ```
 
 ## Exceptions
 
 ```{eval-rst}
 .. autosummary::
    :toctree: ../generated/classes
@@ -37,9 +37,10 @@
 
 ```{eval-rst}
 .. autosummary::
    :toctree: ../generated/modules
    :template: module-template.rst
    :recursive:
 
+   serialize
    sphinxext
 ```
```

### Comparing `sciline-24.2.1/docs/conf.py` & `sciline-24.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/developer/architecture-and-design/workflow-design.md` & `sciline-24.4.0/docs/developer/architecture-and-design/workflow-design.md`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/developer/coding-conventions.md` & `sciline-24.4.0/docs/developer/coding-conventions.md`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/developer/dependency-management.md` & `sciline-24.4.0/docs/developer/dependency-management.md`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/developer/getting-started.md` & `sciline-24.4.0/docs/developer/getting-started.md`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/index.md` & `sciline-24.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/recipes/applying-decorators.ipynb` & `sciline-24.4.0/docs/recipes/applying-decorators.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/recipes/continue-from-intermediate-results.ipynb` & `sciline-24.4.0/docs/recipes/continue-from-intermediate-results.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/recipes/replacing-providers.ipynb` & `sciline-24.4.0/docs/recipes/replacing-providers.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/recipes/side-effects-and-file-writing.ipynb` & `sciline-24.4.0/docs/recipes/side-effects-and-file-writing.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/user-guide/generic-providers.ipynb` & `sciline-24.4.0/docs/user-guide/generic-providers.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/user-guide/getting-started.ipynb` & `sciline-24.4.0/docs/user-guide/getting-started.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/docs/user-guide/parameter-tables.ipynb` & `sciline-24.4.0/docs/user-guide/parameter-tables.ipynb`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/pyproject.toml` & `sciline-24.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 --strict-markers
 -ra
 -v
 """
 testpaths = "tests"
 filterwarnings = [
   "error",
+    # From jsonschema
+    "ignore:datetime.datetime.utcfromtimestamp:DeprecationWarning",
 ]
 
 [tool.bandit]
 # Excluding tests because bandit doesn't like `assert`.
 exclude_dirs = ["docs/conf.py", "tests"]
 
 [tool.black]
```

### Comparing `sciline-24.2.1/requirements/base.txt` & `sciline-24.4.0/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/requirements/ci.txt` & `sciline-24.4.0/requirements/ci.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 cachetools==5.3.2
     # via tox
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 chardet==5.2.0
     # via tox
 charset-normalizer==3.3.2
     # via requests
 colorama==0.4.6
     # via tox
@@ -19,38 +19,38 @@
     # via virtualenv
 filelock==3.13.1
     # via
     #   tox
     #   virtualenv
 gitdb==4.0.11
     # via gitpython
-gitpython==3.1.40
+gitpython==3.1.41
     # via -r ci.in
 idna==3.6
     # via requests
 packaging==23.2
     # via
     #   -r ci.in
     #   pyproject-api
     #   tox
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via
     #   tox
     #   virtualenv
-pluggy==1.3.0
+pluggy==1.4.0
     # via tox
 pyproject-api==1.6.1
     # via tox
 requests==2.31.0
     # via -r ci.in
 smmap==5.0.1
     # via gitdb
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
-tox==4.11.4
+tox==4.12.1
     # via -r ci.in
-urllib3==2.1.0
+urllib3==2.2.0
     # via requests
 virtualenv==20.25.0
     # via tox
```

### Comparing `sciline-24.2.1/requirements/dev.txt` & `sciline-24.4.0/requirements/dev.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,85 +11,94 @@
 -r mypy.txt
 -r static.txt
 -r test.txt
 -r wheels.txt
 annotated-types==0.6.0
     # via pydantic
 anyio==4.2.0
-    # via jupyter-server
+    # via
+    #   httpx
+    #   jupyter-server
 argon2-cffi==23.1.0
     # via jupyter-server
 argon2-cffi-bindings==21.2.0
     # via argon2-cffi
 arrow==1.3.0
     # via isoduration
 async-lru==2.0.4
     # via jupyterlab
 cffi==1.16.0
     # via argon2-cffi-bindings
 click==8.1.7
     # via
     #   pip-compile-multi
     #   pip-tools
-copier==9.1.0
+copier==9.1.1
     # via -r dev.in
-dunamai==1.19.0
+dunamai==1.19.1
     # via copier
 fqdn==1.5.1
     # via jsonschema
 funcy==2.0
     # via copier
+h11==0.14.0
+    # via httpcore
+httpcore==1.0.2
+    # via httpx
+httpx==0.26.0
+    # via jupyterlab
 isoduration==20.11.0
     # via jsonschema
 jinja2-ansible-filters==1.3.2
     # via copier
 json5==0.9.14
     # via jupyterlab-server
 jsonpointer==2.4
     # via jsonschema
-jsonschema[format-nongpl]==4.20.0
+jsonschema[format-nongpl]==4.21.1
     # via
+    #   -r basetest.in
     #   jupyter-events
     #   jupyterlab-server
     #   nbformat
 jupyter-events==0.9.0
     # via jupyter-server
-jupyter-lsp==2.2.1
+jupyter-lsp==2.2.2
     # via jupyterlab
-jupyter-server==2.12.2
+jupyter-server==2.12.5
     # via
     #   jupyter-lsp
     #   jupyterlab
     #   jupyterlab-server
     #   notebook-shim
-jupyter-server-terminals==0.5.1
+jupyter-server-terminals==0.5.2
     # via jupyter-server
-jupyterlab==4.0.10
+jupyterlab==4.1.1
     # via -r dev.in
 jupyterlab-server==2.25.2
     # via jupyterlab
 notebook-shim==0.2.3
     # via jupyterlab
-overrides==7.4.0
+overrides==7.7.0
     # via jupyter-server
 pathspec==0.12.1
     # via copier
 pip-compile-multi==2.6.3
     # via -r dev.in
 pip-tools==7.3.0
     # via pip-compile-multi
 plumbum==1.8.2
     # via copier
 prometheus-client==0.19.0
     # via jupyter-server
 pycparser==2.21
     # via cffi
-pydantic==2.5.3
+pydantic==2.6.1
     # via copier
-pydantic-core==2.14.6
+pydantic-core==2.16.2
     # via pydantic
 python-json-logger==2.0.7
     # via jupyter-events
 pyyaml-include==1.3.2
     # via copier
 questionary==2.0.1
     # via copier
@@ -100,15 +109,17 @@
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
 send2trash==1.8.2
     # via jupyter-server
 sniffio==1.3.0
-    # via anyio
+    # via
+    #   anyio
+    #   httpx
 terminado==0.18.0
     # via
     #   jupyter-server
     #   jupyter-server-terminals
 toposort==1.10
     # via pip-compile-multi
 types-python-dateutil==2.8.19.20240106
```

### Comparing `sciline-24.2.1/requirements/docs.txt` & `sciline-24.4.0/requirements/docs.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
-alabaster==0.7.15
+alabaster==0.7.16
     # via sphinx
 attrs==23.2.0
     # via
     #   jsonschema
     #   referencing
 babel==2.14.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
-beautifulsoup4==4.12.2
+beautifulsoup4==4.12.3
     # via
     #   nbconvert
     #   pydata-sphinx-theme
 bleach==6.1.0
     # via nbconvert
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 comm==0.2.1
     # via ipykernel
-debugpy==1.8.0
+debugpy==1.8.1
     # via ipykernel
 defusedxml==0.7.1
     # via nbconvert
 docutils==0.20.1
     # via
     #   myst-parser
     #   nbsphinx
@@ -49,23 +49,23 @@
 imagesize==1.4.1
     # via sphinx
 importlib-metadata==7.0.1
     # via
     #   jupyter-client
     #   nbconvert
     #   sphinx
-ipykernel==6.28.0
+ipykernel==6.29.2
     # via -r docs.in
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   myst-parser
     #   nbconvert
     #   nbsphinx
     #   sphinx
-jsonschema==4.20.0
+jsonschema==4.21.1
     # via nbformat
 jsonschema-specifications==2023.12.1
     # via jsonschema
 jupyter-client==8.6.0
     # via
     #   ipykernel
     #   nbclient
@@ -78,68 +78,68 @@
     #   nbformat
 jupyterlab-pygments==0.3.0
     # via nbconvert
 markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
-markupsafe==2.1.3
+markupsafe==2.1.5
     # via
     #   jinja2
     #   nbconvert
 mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
 mistune==3.0.2
     # via nbconvert
 myst-parser==2.0.0
     # via -r docs.in
 nbclient==0.9.0
     # via nbconvert
-nbconvert==7.14.0
+nbconvert==7.16.0
     # via nbsphinx
 nbformat==5.9.2
     # via
     #   nbclient
     #   nbconvert
     #   nbsphinx
 nbsphinx==0.9.3
     # via -r docs.in
-nest-asyncio==1.5.8
+nest-asyncio==1.6.0
     # via ipykernel
 packaging==23.2
     # via
     #   ipykernel
     #   nbconvert
     #   pydata-sphinx-theme
     #   sphinx
-pandocfilters==1.5.0
+pandocfilters==1.5.1
     # via nbconvert
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via jupyter-core
-psutil==5.9.7
+psutil==5.9.8
     # via ipykernel
-pydata-sphinx-theme==0.15.1
+pydata-sphinx-theme==0.15.2
     # via -r docs.in
 python-dateutil==2.8.2
     # via jupyter-client
 pyyaml==6.0.1
     # via myst-parser
 pyzmq==25.1.2
     # via
     #   ipykernel
     #   jupyter-client
-referencing==0.32.1
+referencing==0.33.0
     # via
     #   jsonschema
     #   jsonschema-specifications
 requests==2.31.0
     # via sphinx
-rpds-py==0.16.2
+rpds-py==0.17.1
     # via
     #   jsonschema
     #   referencing
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
@@ -148,46 +148,41 @@
     #   -r docs.in
     #   myst-parser
     #   nbsphinx
     #   pydata-sphinx-theme
     #   sphinx-autodoc-typehints
     #   sphinx-copybutton
     #   sphinx-design
-    #   sphinxcontrib-applehelp
-    #   sphinxcontrib-devhelp
-    #   sphinxcontrib-htmlhelp
-    #   sphinxcontrib-qthelp
-    #   sphinxcontrib-serializinghtml
-sphinx-autodoc-typehints==1.25.2
+sphinx-autodoc-typehints==2.0.0
     # via -r docs.in
 sphinx-copybutton==0.5.2
     # via -r docs.in
 sphinx-design==0.5.0
     # via -r docs.in
-sphinxcontrib-applehelp==1.0.7
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.5
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.4
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.6
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.9
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 tinycss2==1.2.1
     # via nbconvert
 tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
 typing-extensions==4.9.0
     # via pydata-sphinx-theme
-urllib3==2.1.0
+urllib3==2.2.0
     # via requests
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
 zipp==3.17.0
     # via importlib-metadata
```

### Comparing `sciline-24.2.1/requirements/make_base.py` & `sciline-24.4.0/requirements/make_base.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/requirements/static.txt` & `sciline-24.4.0/requirements/static.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 #
 cfgv==3.4.0
     # via pre-commit
 distlib==0.3.8
     # via virtualenv
 filelock==3.13.1
     # via virtualenv
-identify==2.5.33
+identify==2.5.34
     # via pre-commit
 nodeenv==1.8.0
     # via pre-commit
-platformdirs==4.1.0
+platformdirs==4.2.0
     # via virtualenv
-pre-commit==3.6.0
+pre-commit==3.6.1
     # via -r static.in
 pyyaml==6.0.1
     # via pre-commit
 virtualenv==20.25.0
     # via pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `sciline-24.2.1/requirements/test-dask.txt` & `sciline-24.4.0/requirements/test-dask.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 #    pip-compile-multi
 #
 -r test.txt
 click==8.1.7
     # via dask
 cloudpickle==3.0.0
     # via dask
-dask==2023.12.1
+dask==2024.2.0
     # via -r test-dask.in
-fsspec==2023.12.2
+fsspec==2024.2.0
     # via dask
 importlib-metadata==7.0.1
     # via dask
 locket==1.0.0
     # via partd
 partd==1.4.1
     # via dask
 pyyaml==6.0.1
     # via dask
-toolz==0.12.0
+toolz==0.12.1
     # via
     #   dask
     #   partd
 zipp==3.17.0
     # via importlib-metadata
```

### Comparing `sciline-24.2.1/resources/sciline.svg` & `sciline-24.4.0/resources/sciline.svg`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/src/sciline/__init__.py` & `sciline-24.4.0/src/sciline/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,23 +16,25 @@
     HandleAsBuildTimeException,
     HandleAsComputeTimeException,
     UnsatisfiedRequirement,
 )
 from .param_table import ParamTable
 from .pipeline import AmbiguousProvider, Pipeline
 from .series import Series
+from .task_graph import TaskGraph
 
 __all__ = [
     "AmbiguousProvider",
-    "Series",
     "ParamTable",
     "Pipeline",
+    "scheduler",
+    "Series",
     "Scope",
     "ScopeTwoParams",
+    'TaskGraph',
     "UnboundTypeVar",
     "UnsatisfiedRequirement",
-    "scheduler",
     "HandleAsBuildTimeException",
     "HandleAsComputeTimeException",
 ]
 
 del importlib
```

### Comparing `sciline-24.2.1/src/sciline/display.py` & `sciline-24.4.0/src/sciline/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 from html import escape
 from typing import Iterable, List, Tuple, TypeVar, Union
 
 from ._provider import Provider
+from ._utils import groupby, key_name
 from .typing import Item, Key
-from .utils import groupby, keyname
 
 
 def _details(summary: str, body: str) -> str:
     return f'''
     <details>
       <summary>{summary}</summary>
       {body}
@@ -20,27 +20,27 @@
 def _provider_name(
     p: Tuple[Key, Tuple[Union[Key, TypeVar], ...], List[Provider]]
 ) -> str:
     key, args, _ = p
     if args:
         # This is always the case, but mypy complains
         if hasattr(key, '__getitem__'):
-            return escape(keyname(key[args]))
-    return escape(keyname(key))
+            return escape(key_name(key[args]))
+    return escape(key_name(key))
 
 
 def _provider_source(
     p: Tuple[Key, Tuple[Union[Key, TypeVar], ...], List[Provider]]
 ) -> str:
     key, _, (v, *rest) = p
     if v.kind == 'table_cell':
         # This is always the case, but mypy complains
         if isinstance(key, Item):
             return escape(
-                f'ParamTable({keyname(key.label[0].tp)}, length={len((v, *rest))})'
+                f'ParamTable({key_name(key.label[0].tp)}, length={len((v, *rest))})'
             )
     if v.kind == 'function':
         return _details(
             escape(v.location.name),
             escape(f'{v.location.module}.{v.location.name}'),
         )
     return ''
```

### Comparing `sciline-24.2.1/src/sciline/domain.py` & `sciline-24.4.0/src/sciline/domain.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/src/sciline/handler.py` & `sciline-24.4.0/src/sciline/handler.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/src/sciline/param_table.py` & `sciline-24.4.0/src/sciline/param_table.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/src/sciline/pipeline.py` & `sciline-24.4.0/src/sciline/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,27 +24,27 @@
     get_type_hints,
     overload,
 )
 
 from sciline.task_graph import TaskGraph
 
 from ._provider import ArgSpec, Provider, ProviderLocation, ToProvider
+from ._utils import key_name
 from .display import pipeline_html_repr
 from .domain import Scope, ScopeTwoParams
 from .handler import (
     ErrorHandler,
     HandleAsBuildTimeException,
     HandleAsComputeTimeException,
     UnsatisfiedRequirement,
 )
 from .param_table import ParamTable
 from .scheduler import Scheduler
 from .series import Series
 from .typing import Graph, Item, Key, Label, get_optional, get_union
-from .utils import keyname
 
 T = TypeVar('T')
 KeyType = TypeVar('KeyType', bound=Key)
 ValueType = TypeVar('ValueType', bound=Key)
 IndexType = TypeVar('IndexType', bound=Key)
 LabelType = TypeVar('LabelType', bound=Key)
 
@@ -123,14 +123,16 @@
     """Find all paths from start to end in a DAG."""
     if start == end:
         return [[start]]
     if start not in dependencies:
         return []
     paths = []
     for node in dependencies[start]:
+        if start == node:
+            continue
         for path in _find_all_paths(dependencies, node, end):
             paths.append([start] + path)
     return paths
 
 
 def _find_nodes_in_paths(graph: Graph, end: Key) -> List[Key]:
     """
@@ -580,20 +582,20 @@
                 if typevars_in_expression:
                     explanation = [
                         ''.join(
                             map(
                                 str,
                                 (
                                     'Note that ',
-                                    keyname(origin[typevars_in_expression]),
+                                    key_name(origin[typevars_in_expression]),
                                     ' has constraints ',
                                     (
                                         {
-                                            keyname(tv): tuple(
-                                                map(keyname, tv.__constraints__)
+                                            key_name(tv): tuple(
+                                                map(key_name, tv.__constraints__)
                                             )
                                             for tv in typevars_in_expression
                                         }
                                     ),
                                 ),
                             )
                         )
```

### Comparing `sciline-24.2.1/src/sciline/scheduler.py` & `sciline-24.4.0/src/sciline/scheduler.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/src/sciline/series.py` & `sciline-24.4.0/src/sciline/series.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/src/sciline/sphinxext/domain_types.py` & `sciline-24.4.0/src/sciline/sphinxext/domain_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         f'{_internal_link(annotation, "class", prefix)}'
         f' ({_link(annotation.__supertype__, "class",aliases)})'
     )
 
 
 def _is_type_alias_type(annotation: Any) -> bool:
     try:
-        from typing import TypeAliasType  # type: ignore[attr-defined]
+        from typing import TypeAliasType  # type: ignore[attr-defined, unused-ignore]
 
         return isinstance(annotation, TypeAliasType)
     except ImportError:
         return False  # pre python 3.12
 
 
 def _format_type_alias_type(
```

### Comparing `sciline-24.2.1/src/sciline/task_graph.py` & `sciline-24.4.0/src/sciline/task_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 from __future__ import annotations
 
 from html import escape
 from typing import Any, Generator, Optional, Sequence, Tuple, TypeVar, Union
 
+from ._utils import key_name
 from .scheduler import DaskScheduler, NaiveScheduler, Scheduler
-from .typing import Graph, Item, Key
-from .utils import keyname
+from .serialize import json_serialize_task_graph
+from .typing import Graph, Item, Json, Key
 
 T = TypeVar("T")
 
 
 def _list_items(items: Sequence[str]) -> str:
     return '\n'.join(
         (
@@ -137,26 +138,39 @@
         kwargs:
             Keyword arguments passed to :py:class:`graphviz.Digraph`.
         """
         from .visualize import to_graphviz
 
         return to_graphviz(self._graph, **kwargs)
 
+    def serialize(self) -> dict[str, Json]:
+        """Serialize the graph to JSON.
+
+        See the user guide on
+        `Serializing Providers <../../user-guide/serialization.rst>`_.
+
+        Returns
+        -------
+        :
+            A JSON object representing the graph.
+        """
+        return json_serialize_task_graph(self._graph)
+
     def _repr_html_(self) -> str:
         leafs = sorted(
             [
-                escape(keyname(key))
+                escape(key_name(key))
                 for key in (
                     self._keys if isinstance(self._keys, tuple) else [self._keys]
                 )
             ]
         )
         roots = sorted(
             {
-                escape(keyname(key))
+                escape(key_name(key))
                 for key, provider in self._graph.items()
                 if provider.kind != 'function'
             }
         )
         scheduler = escape(str(self._scheduler))
 
         def head(word: str) -> str:
```

### Comparing `sciline-24.2.1/src/sciline/typing.py` & `sciline-24.4.0/src/sciline/typing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # SPDX-License-Identifier: BSD-3-Clause
 # Copyright (c) 2023 Scipp contributors (https://github.com/scipp)
 from dataclasses import dataclass
 from typing import (
     Any,
+    Dict,
     Generic,
+    List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
@@ -31,14 +33,17 @@
     tp: Type[T]
 
 
 Key = Union[type, Item[Any]]
 Graph = dict[Key, Provider]
 
 
+Json = Union[Dict[str, "Json"], List["Json"], str, int, float, bool, None]
+
+
 def get_optional(tp: Key) -> Optional[Any]:
     if get_origin(tp) != Union:
         return None
     args = get_args(tp)
     if len(args) != 2 or type(None) not in args:
         return None
     return args[0] if args[1] == type(None) else args[1]  # noqa: E721
```

### Comparing `sciline-24.2.1/src/sciline/visualize.py` & `sciline-24.4.0/src/sciline/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,26 +79,24 @@
                 else:
                     dot_subgraph.attr(style='filled', color=cluster_color)
             _add_subgraph(subgraph, dot, dot_subgraph)
     return dot
 
 
 def _to_subgraphs(graph: FormattedGraph) -> Dict[str, FormattedGraph]:
-    def get_subgraph_name(name: str) -> str:
-        sgname = name.split('[')[0]
-        if sgname == 'Series':
+    def get_subgraph_name(name: str, kind: str) -> str:
+        if kind == 'series':
             # Example: Series[RowId, Material[Country]] -> RowId, Material[Country]
             return name.partition('[')[-1].rpartition(']')[0]
-        return sgname
+        return name
 
     subgraphs: Dict[str, FormattedGraph] = {}
     for p, formatted_p in graph.items():
-        subgraph_name = get_subgraph_name(formatted_p.ret.name)
-        if subgraph_name not in subgraphs:
-            subgraphs[subgraph_name] = {}
+        subgraph_name = get_subgraph_name(formatted_p.ret.name, formatted_p.kind)
+        subgraphs.setdefault(subgraph_name, {})
         subgraphs[subgraph_name][p] = formatted_p
     return subgraphs
 
 
 def _add_subgraph(graph: FormattedGraph, dot: Digraph, subgraph: Digraph) -> None:
     for p, formatted_p in graph.items():
         if formatted_p.kind == 'unsatisfied':
```

### Comparing `sciline-24.2.1/src/sciline.egg-info/PKG-INFO` & `sciline-24.4.0/src/sciline.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciline
-Version: 24.2.1
+Version: 24.4.0
 Summary: Build scientific pipelines for your data
 Author: Scipp contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Scipp contributors (https://github.com/scipp)
         All rights reserved.
```

### Comparing `sciline-24.2.1/src/sciline.egg-info/SOURCES.txt` & `sciline-24.4.0/src/sciline.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 docs/recipes/index.md
 docs/recipes/replacing-providers.ipynb
 docs/recipes/side-effects-and-file-writing.ipynb
 docs/user-guide/generic-providers.ipynb
 docs/user-guide/getting-started.ipynb
 docs/user-guide/index.md
 docs/user-guide/parameter-tables.ipynb
+docs/user-guide/provenance.ipynb
 requirements/base.in
 requirements/base.txt
 requirements/basetest.in
 requirements/basetest.txt
 requirements/ci.in
 requirements/ci.txt
 requirements/dev.in
@@ -67,38 +68,43 @@
 requirements/test.in
 requirements/test.txt
 requirements/wheels.in
 requirements/wheels.txt
 resources/sciline.svg
 src/sciline/__init__.py
 src/sciline/_provider.py
+src/sciline/_utils.py
 src/sciline/display.py
 src/sciline/domain.py
 src/sciline/handler.py
 src/sciline/param_table.py
 src/sciline/pipeline.py
 src/sciline/py.typed
 src/sciline/scheduler.py
 src/sciline/series.py
 src/sciline/task_graph.py
 src/sciline/typing.py
-src/sciline/utils.py
 src/sciline/visualize.py
 src/sciline.egg-info/PKG-INFO
 src/sciline.egg-info/SOURCES.txt
 src/sciline.egg-info/dependency_links.txt
 src/sciline.egg-info/top_level.txt
+src/sciline/serialize/__init__.py
+src/sciline/serialize/_json.py
+src/sciline/serialize/graph_json_schema.json
 src/sciline/sphinxext/__init__.py
 src/sciline/sphinxext/domain_types.py
 tests/_provider_test.py
 tests/complex_workflow_test.py
 tests/conftest.py
 tests/dask_scheduler_test.py
 tests/domain_test.py
 tests/package_test.py
 tests/param_table_test.py
 tests/pipeline_test.py
 tests/pipeline_with_optional_test.py
 tests/pipeline_with_param_table_test.py
 tests/pipeline_with_postponed_annotations_test.py
 tests/task_graph_test.py
-tests/visualize_test.py
+tests/utils_test.py
+tests/visualize_test.py
+tests/serialize/json_test.py
```

### Comparing `sciline-24.2.1/tests/_provider_test.py` & `sciline-24.4.0/tests/_provider_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 
 from typing import List, Tuple, TypeVar
 
 from sciline._provider import ArgSpec
 
 
 def test_arg_spec() -> None:
-    arg_spec = ArgSpec(args={'a': int}, kwargs={'b': str})
+    arg_spec = ArgSpec(args={'a': int}, kwargs={'b': str}, return_=list[str])
     assert list(arg_spec.args) == [int]
     assert dict(arg_spec.kwargs) == {'b': str}
+    assert arg_spec.return_ == list[str]
 
 
 def combine_numbers(a: int, *, b: float) -> str:
     return f"{a} and {b}"
 
 
 T = TypeVar('T', int, float)
```

### Comparing `sciline-24.2.1/tests/complex_workflow_test.py` & `sciline-24.4.0/tests/complex_workflow_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/tests/conftest.py` & `sciline-24.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/tests/domain_test.py` & `sciline-24.4.0/tests/domain_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/tests/param_table_test.py` & `sciline-24.4.0/tests/param_table_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/tests/pipeline_test.py` & `sciline-24.4.0/tests/pipeline_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1435,7 +1435,111 @@
     @deco
     def foo(*, k: int) -> float:
         return float(k)
 
     provider = deco(foo)
     pipeline = sl.Pipeline([provider], params={int: 3})
     assert pipeline.compute(float) == 3.0
+
+
+R = TypeVar('R')
+
+
+def wrapping_decorator(f: Callable[..., R]) -> Callable[..., R]:
+    @functools.wraps(f)
+    def wrapper(*args: Any, **kwargs: Any) -> R:
+        return f(*args, **kwargs)
+
+    return wrapper
+
+
+def null_decorator(f: Callable[..., R]) -> Callable[..., R]:
+    return f
+
+
+@pytest.mark.parametrize('deco', (null_decorator, wrapping_decorator))
+def test_pipeline_lambda_provider(deco: Callable[..., Any]) -> None:
+    lam = lambda x: str(x)  # noqa: E731
+    lam.__annotations__['x'] = int
+    lam.__annotations__['return'] = str
+    func = deco(lam)
+
+    pipeline = sl.Pipeline([func], params={int: 3})
+    assert pipeline.compute(str) == '3'
+
+
+@pytest.mark.parametrize('deco', (null_decorator, wrapping_decorator))
+def test_pipeline_instance_method_provider(deco: Callable[..., Any]) -> None:
+    class C:
+        @deco
+        def to_string(self, x: int) -> str:
+            return str(x)
+
+    c = C()
+    pipeline = sl.Pipeline([c.to_string], params={int: 3})
+    assert pipeline.compute(str) == '3'
+
+
+# Must be outside of test because of string annotation
+class ClassWithSelfAnnotation:
+    def to_string(self: "ClassWithSelfAnnotation", x: int) -> str:
+        return str(x)
+
+
+def test_pipeline_instance_method_with_self_annotation_provider() -> None:
+    c = ClassWithSelfAnnotation()
+    pipeline = sl.Pipeline([c.to_string], params={int: 3})
+    assert pipeline.compute(str) == '3'
+
+
+@pytest.mark.parametrize('deco', (null_decorator, wrapping_decorator))
+def test_pipeline_class_method_provider(deco: Callable[..., Any]) -> None:
+    class C:
+        @classmethod
+        @deco
+        def to_string(cls, x: int) -> str:
+            return str(x)
+
+    pipeline = sl.Pipeline([C.to_string], params={int: 3})
+    assert pipeline.compute(str) == '3'
+
+
+@pytest.mark.parametrize('deco', (null_decorator, wrapping_decorator))
+def test_pipeline_static_method_provider(deco: Callable[..., Any]) -> None:
+    class C:
+        @staticmethod
+        @deco
+        def to_string(x: int) -> str:
+            return str(x)
+
+    pipeline = sl.Pipeline([C.to_string], params={int: 3})
+    assert pipeline.compute(str) == '3'
+
+
+def test_pipeline_callable_instance_provider() -> None:
+    class C:
+        def __init__(self, y: int) -> None:
+            self.y = y
+
+        def __call__(self, x: int) -> str:
+            return str(x + self.y)
+
+    pipeline = sl.Pipeline([C(4)], params={int: 3})
+    assert pipeline.compute(str) == "7"
+
+
+def test_pipeline_class_init_provider() -> None:
+    class C:
+        def __init__(self, x: int) -> None:
+            self.x = x
+
+    with pytest.raises(TypeError):
+        sl.Pipeline([C], params={int: 3})
+
+
+def test_pipeline_class_new_provider() -> None:
+    class C:
+        def __new__(cls, x: int) -> str:  # type: ignore[misc]
+            return str(x)
+
+    with pytest.raises(TypeError):
+        sl.Pipeline([C], params={int: 3})
```

### Comparing `sciline-24.2.1/tests/pipeline_with_optional_test.py` & `sciline-24.4.0/tests/pipeline_with_optional_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/tests/pipeline_with_param_table_test.py` & `sciline-24.4.0/tests/pipeline_with_param_table_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -715,7 +715,27 @@
 
     def to_str(x: int) -> str:
         return str(x)
 
     pl = sl.Pipeline((to_str,))
     pl.set_param_series(int, ints)
     assert pl.compute(sl.Series[int, str]) == sl.Series(int, {1: '1', 2: '2', 3: '3'})
+
+
+def test_multiple_param_series_can_be_broadcast() -> None:
+    ints = [1, 2, 3]
+    floats = [1.0, 2.0]
+
+    def to_str(x: int, y: float) -> str:
+        return str(x) + str(y)
+
+    pl = sl.Pipeline((to_str,))
+    pl.set_param_series(int, ints)
+    pl.set_param_series(float, floats)
+    assert pl.compute(sl.Series[int, sl.Series[float, str]]) == sl.Series(
+        int,
+        {
+            1: sl.Series(float, {1.0: '11.0', 2.0: '12.0'}),
+            2: sl.Series(float, {1.0: '21.0', 2.0: '22.0'}),
+            3: sl.Series(float, {1.0: '31.0', 2.0: '32.0'}),
+        },
+    )
```

### Comparing `sciline-24.2.1/tests/pipeline_with_postponed_annotations_test.py` & `sciline-24.4.0/tests/pipeline_with_postponed_annotations_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/tests/task_graph_test.py` & `sciline-24.4.0/tests/task_graph_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/tests/visualize_test.py` & `sciline-24.4.0/tests/visualize_test.py`

 * *Files identical despite different names*

### Comparing `sciline-24.2.1/tox.ini` & `sciline-24.4.0/tox.ini`

 * *Files identical despite different names*

