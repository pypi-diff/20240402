# Comparing `tmp/dkist-processing-core-3.1.0rc1.tar.gz` & `tmp/dkist-processing-core-3.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-core-3.1.0rc1.tar", last modified: Wed Feb 21 17:26:41 2024, max compression
+gzip compressed data, was "dkist-processing-core-3.1.0rc2.tar", last modified: Tue Mar 12 21:18:01 2024, max compression
```

## Comparing `dkist-processing-core-3.1.0rc1.tar` & `dkist-processing-core-3.1.0rc2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.308958 dkist-processing-core-3.1.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2448 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     5409 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     7965 2024-02-21 17:26:41.308958 dkist-processing-core-3.1.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7351 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2816 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.304958 dkist-processing-core-3.1.0rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/changelog/30.misc.rst
--rwxrwxrwx   0 root         (0) root         (0)      436 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.304958 dkist-processing-core-3.1.0rc1/dkist_processing_core/
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3272 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     5506 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/_node.py
--rw-rw-rw-   0 root         (0) root         (0)     6096 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/resource_queue.py
--rw-rw-rw-   0 root         (0) root         (0)    10204 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/task.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.304958 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.304958 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/invalid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/invalid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/invalid_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/task_example.py
--rw-rw-rw-   0 root         (0) root         (0)     3470 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_export.py
--rw-rw-rw-   0 root         (0) root         (0)     4030 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     4525 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.304958 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/valid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/valid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/valid_workflow_package/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.304958 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/zero_node_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    10181 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.304958 dkist-processing-core-3.1.0rc1/dkist_processing_core.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7965 2024-02-21 17:26:41.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1676 2024-02-21 17:26:41.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-21 17:26:41.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-02-21 17:26:41.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-02-21 17:26:41.000000 dkist-processing-core-3.1.0rc1/dkist_processing_core.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.308958 dkist-processing-core-3.1.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    85295 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/docs/auto-proc-concept-model.png
--rw-rw-rw-   0 root         (0) root         (0)    26060 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/docs/auto_proc_brick.png
--rw-rw-rw-   0 root         (0) root         (0)   267222 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/docs/automated-processing-deployed.png
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1854 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-21 17:26:41.308958 dkist-processing-core-3.1.0rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1334 2024-02-21 17:26:41.308958 dkist-processing-core-3.1.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-02-21 17:26:35.000000 dkist-processing-core-3.1.0rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5409 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7965 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7351 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2816 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.061446 dkist-processing-core-3.1.0rc2/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/changelog/32.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      436 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.061446 dkist-processing-core-3.1.0rc2/dkist_processing_core/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3272 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     5525 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     6096 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/resource_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)    10316 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/task.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4533 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/invalid_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/invalid_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/invalid_workflow_package/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/task_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     4030 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     4525 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/valid_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/valid_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/valid_workflow_package/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/zero_node_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    10181 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.061446 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     7965 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      278 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    85295 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/auto-proc-concept-model.png
+-rw-rw-rw-   0 root         (0) root         (0)    26060 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/auto_proc_brick.png
+-rw-rw-rw-   0 root         (0) root         (0)   267222 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/automated-processing-deployed.png
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/setup.py
```

### Comparing `dkist-processing-core-3.1.0rc1/.gitignore` & `dkist-processing-core-3.1.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/.pre-commit-config.yaml` & `dkist-processing-core-3.1.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/CHANGELOG.rst` & `dkist-processing-core-3.1.0rc2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/PKG-INFO` & `dkist-processing-core-3.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 3.1.0rc1
+Version: 3.1.0rc2
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-core-3.1.0rc1/README.rst` & `dkist-processing-core-3.1.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/bitbucket-pipelines.yml` & `dkist-processing-core-3.1.0rc2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/_failure_callback.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/_failure_callback.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/_node.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         return eval(self.operator_definition)
 
     @property
     def notebook_cell(self) -> str:
         """Render the node as python code for a notebook cell."""
         lines = [
             f"from {self.task.__module__} import {self.task.__name__}",
-            f"with {self.task.__name__}(recipe_run_id=recipe_run_id, workflow_name='{self.workflow_name}', workflow_version='{self.workflow_version}') as t:\n    #t.is_task_manual = True\n    t()",
+            f"with {self.task.__name__}(recipe_run_id=recipe_run_id, workflow_name='{self.workflow_name}', workflow_version='{self.workflow_version}') as t:\n    #t.is_task_manual = True\n    t()\n    #t.rollback()",
         ]
         return "\n".join(lines)
 
     @property
     def operator_definition(self) -> str:
         """Airflow style command to define a bash operator."""
         return f"""BashOperator(
```

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/build_utils.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/build_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/task.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,14 +216,17 @@
     @abstractmethod
     def run(self) -> None:
         """Abstract method that must be overridden to execute the desired DAG task."""
 
     def post_run(self) -> None:
         """Intended to be overridden and will execute after run() with Elastic APM span capturing."""
 
+    def rollback(self) -> None:
+        """Rollback any changes to persistent stores performed by the task."""
+
     def __call__(self) -> None:
         """
         DAG task wrapper. Execution is instrumented with Application Performance Monitoring if configured.
 
         The standard execution sequence is:
 
         1 run
```

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/conftest.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/task_example.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/task_example.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_build_utils.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_build_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_export.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_failure_callback.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_failure_callback.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_node.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_task.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/test_workflow.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/tests/valid_workflow_package/workflow.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/valid_workflow_package/workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core/workflow.py` & `dkist-processing-core-3.1.0rc2/dkist_processing_core/workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core.egg-info/PKG-INFO` & `dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 3.1.0rc1
+Version: 3.1.0rc2
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-core-3.1.0rc1/dkist_processing_core.egg-info/SOURCES.txt` & `dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
-changelog/30.misc.rst
+changelog/32.feature.rst
 dkist_processing_core/__init__.py
 dkist_processing_core/_failure_callback.py
 dkist_processing_core/_node.py
 dkist_processing_core/build_utils.py
 dkist_processing_core/resource_queue.py
 dkist_processing_core/task.py
 dkist_processing_core/workflow.py
```

### Comparing `dkist-processing-core-3.1.0rc1/docs/Makefile` & `dkist-processing-core-3.1.0rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/docs/auto-proc-concept-model.png` & `dkist-processing-core-3.1.0rc2/docs/auto-proc-concept-model.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/docs/auto_proc_brick.png` & `dkist-processing-core-3.1.0rc2/docs/auto_proc_brick.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/docs/automated-processing-deployed.png` & `dkist-processing-core-3.1.0rc2/docs/automated-processing-deployed.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/docs/conf.py` & `dkist-processing-core-3.1.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/docs/make.bat` & `dkist-processing-core-3.1.0rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/licenses/LICENSE.rst` & `dkist-processing-core-3.1.0rc2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/pyproject.toml` & `dkist-processing-core-3.1.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc1/setup.cfg` & `dkist-processing-core-3.1.0rc2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	apache-airflow[postgres, celery] == 2.8.1
+	apache-airflow[postgres, celery] == 2.7.3
 	elastic-apm < 7.0.0
 	requests >= 2.23
 	talus >= 0.2.0
 	pendulum
 	nbformat >= 5.9.2
 
 [options.extras_require]
```

