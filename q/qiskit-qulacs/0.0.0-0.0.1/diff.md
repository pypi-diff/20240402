# Comparing `tmp/qiskit_qulacs-0.0.0.tar.gz` & `tmp/qiskit_qulacs-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_qulacs-0.0.0.tar", last modified: Tue Apr  2 14:49:05 2024, max compression
+gzip compressed data, was "dist/qiskit_qulacs-0.0.1.tar", last modified: Wed Jul 19 05:25:35 2023, max compression
```

## Comparing `qiskit_qulacs-0.0.0.tar` & `qiskit_qulacs-0.0.1.tar`

### file list

```diff
@@ -1,116 +1,83 @@
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.112045 qiskit_qulacs-0.0.0/
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/.github/
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      342 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      342 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/.github/ISSUE_TEMPLATE/enhancement_request.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      332 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      552 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      118 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/.github/dependabot.yml
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/.github/workflows/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     3747 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/.github/workflows/README.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2092 2024-04-02 14:19:25.000000 qiskit_qulacs-0.0.0/.github/workflows/citation.yml
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      869 2024-04-02 14:19:25.000000 qiskit_qulacs-0.0.0/.github/workflows/coverage.yml
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      875 2024-04-02 14:19:25.000000 qiskit_qulacs-0.0.0/.github/workflows/docs.yml
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      537 2024-04-02 14:19:25.000000 qiskit_qulacs-0.0.0/.github/workflows/lint.yml
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     1196 2024-04-02 14:19:25.000000 qiskit_qulacs-0.0.0/.github/workflows/test_latest_versions.yml
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      552 2024-03-30 11:10:34.000000 qiskit_qulacs-0.0.0/.gitignore
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    12936 2024-04-01 13:38:58.000000 qiskit_qulacs-0.0.0/.pylintrc
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      528 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/.travis.yml
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      209 2023-08-24 14:27:38.000000 qiskit_qulacs-0.0.0/CITATION.bib
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      398 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     1184 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/CONTRIBUTING.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    11416 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/LICENSE.txt
--rw-r--r--   0 gopald    (1000) gopald    (1000)    18961 2024-04-02 14:49:05.112045 qiskit_qulacs-0.0.0/PKG-INFO
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     3389 2024-04-02 14:26:46.000000 qiskit_qulacs-0.0.0/README.md
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/benchmarks/
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/benchmarks/cpu/
--rwxrwxr-x   0 gopald    (1000) gopald    (1000)      180 2024-04-02 11:47:22.000000 qiskit_qulacs-0.0.0/benchmarks/cpu/exec.sh
--rwxrwxr-x   0 gopald    (1000) gopald    (1000)       57 2024-04-02 11:59:44.000000 qiskit_qulacs-0.0.0/benchmarks/cpu/execall.sh
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit/
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.096045 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit/.benchmarks/
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit/.benchmarks/Linux-CPython-3.10-64bit/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    95460 2024-04-02 12:10:20.000000 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit/.benchmarks/Linux-CPython-3.10-64bit/0001_data.json
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     3181 2024-04-02 11:59:37.000000 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit/benchmarks.py
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit_qulacs/
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.096045 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit_qulacs/.benchmarks/
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit_qulacs/.benchmarks/Linux-CPython-3.10-64bit/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)   142555 2024-04-02 12:28:20.000000 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit_qulacs/.benchmarks/Linux-CPython-3.10-64bit/0001_data.json
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     5217 2024-04-02 11:59:31.000000 qiskit_qulacs-0.0.0/benchmarks/cpu/qiskit_qulacs/benchmarks.py
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/benchmarks/cpu/qulacs/
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.100045 qiskit_qulacs-0.0.0/benchmarks/cpu/qulacs/.benchmarks/
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.104045 qiskit_qulacs-0.0.0/benchmarks/cpu/qulacs/.benchmarks/Linux-CPython-3.10-64bit/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    74199 2024-04-02 12:10:55.000000 qiskit_qulacs-0.0.0/benchmarks/cpu/qulacs/.benchmarks/Linux-CPython-3.10-64bit/0001_data.json
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2994 2024-03-30 10:30:47.000000 qiskit_qulacs-0.0.0/benchmarks/cpu/qulacs/benchmarks.py
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.104045 qiskit_qulacs-0.0.0/benchmarks/gpu/
--rwxrwxr-x   0 gopald    (1000) gopald    (1000)      107 2023-11-01 15:46:29.000000 qiskit_qulacs-0.0.0/benchmarks/gpu/exec.sh
--rwxrwxr-x   0 gopald    (1000) gopald    (1000)       34 2023-10-19 08:02:23.000000 qiskit_qulacs-0.0.0/benchmarks/gpu/execall.sh
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.104045 qiskit_qulacs-0.0.0/benchmarks/gpu/qiskit/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2577 2024-03-25 10:58:16.000000 qiskit_qulacs-0.0.0/benchmarks/gpu/qiskit/benchmarks.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     3071 2024-04-02 13:42:32.000000 qiskit_qulacs-0.0.0/benchmarks/plot.py
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.104045 qiskit_qulacs-0.0.0/benchmarks/plots/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)   169946 2024-04-02 12:57:57.000000 qiskit_qulacs-0.0.0/benchmarks/plots/fig_compare_cpu.png
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    31504 2023-11-28 09:12:56.000000 qiskit_qulacs-0.0.0/benchmarks/plots/fig_compare_gpu.png
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.104045 qiskit_qulacs-0.0.0/docs/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)        0 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/docs/.nojekyll
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.104045 qiskit_qulacs-0.0.0/docs/_static/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      412 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/docs/_static/custom.css
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.104045 qiskit_qulacs-0.0.0/docs/_static/images/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    14116 2024-03-31 16:00:03.000000 qiskit_qulacs-0.0.0/docs/_static/images/ghz_state.png
--rw-rw-r--   0 gopald    (1000) gopald    (1000)   201546 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/docs/_static/images/logo.png
--rw-rw-r--   0 gopald    (1000) gopald    (1000)   550683 2024-03-31 16:44:36.000000 qiskit_qulacs-0.0.0/docs/_static/images/logo_extended.png
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     3192 2024-03-31 17:04:04.000000 qiskit_qulacs-0.0.0/docs/_static/images/uf.png
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.104045 qiskit_qulacs-0.0.0/docs/apidocs/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      146 2024-03-31 16:06:05.000000 qiskit_qulacs-0.0.0/docs/apidocs/index.rst
--rw-rw-r--   0 gopald    (1000) gopald    (1000)       76 2023-11-28 09:29:48.000000 qiskit_qulacs-0.0.0/docs/apidocs/modules.rst
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     1586 2023-11-28 09:29:38.000000 qiskit_qulacs-0.0.0/docs/apidocs/qiskit_qulacs.rst
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2253 2024-04-01 17:18:42.000000 qiskit_qulacs-0.0.0/docs/conf.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2609 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/docs/file-map-and-description.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     1299 2024-03-31 17:12:27.000000 qiskit_qulacs-0.0.0/docs/index.rst
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.104045 qiskit_qulacs-0.0.0/docs/intro/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     1959 2024-03-31 15:56:35.000000 qiskit_qulacs-0.0.0/docs/intro/INSTALL.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2289 2024-03-31 16:02:49.000000 qiskit_qulacs-0.0.0/docs/intro/beginners_guide.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     1467 2024-04-02 11:37:31.000000 qiskit_qulacs-0.0.0/docs/intro/project_overview.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     4048 2024-03-31 16:33:59.000000 qiskit_qulacs-0.0.0/docs/intro/quickstart_guide.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      169 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/docs/technical_docs.md
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.108045 qiskit_qulacs-0.0.0/docs/tutorials/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)   233408 2024-04-01 13:37:08.000000 qiskit_qulacs-0.0.0/docs/tutorials/01_qulacs_backend.ipynb
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    99282 2024-04-01 13:37:08.000000 qiskit_qulacs-0.0.0/docs/tutorials/02_get_started_primitives.ipynb
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    77355 2024-04-01 13:35:54.000000 qiskit_qulacs-0.0.0/docs/tutorials/03_vqe.ipynb
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      189 2024-03-31 16:13:18.000000 qiskit_qulacs-0.0.0/docs/tutorials/index.rst
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      328 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/docs/zenodo-integration.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      565 2024-04-02 09:50:30.000000 qiskit_qulacs-0.0.0/ecosystem.json
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      171 2023-07-19 13:27:25.000000 qiskit_qulacs-0.0.0/mypy.ini
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2392 2024-04-01 17:25:40.000000 qiskit_qulacs-0.0.0/pyproject.toml
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.108045 qiskit_qulacs-0.0.0/qiskit_qulacs/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      295 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/__init__.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    11980 2024-04-02 13:17:33.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/adapter.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2054 2024-03-31 18:24:48.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/backend_utils.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     6630 2024-04-02 10:52:07.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/qulacs_backend.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     4730 2024-04-02 10:54:24.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/qulacs_estimator.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     3466 2024-04-01 16:31:09.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/qulacs_estimator_gradient.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2386 2024-03-31 13:12:56.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/qulacs_job.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      832 2024-04-02 13:22:46.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/qulacs_provider.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     4931 2024-04-02 11:51:50.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/qulacs_sampler.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)       61 2024-04-02 09:47:16.000000 qiskit_qulacs-0.0.0/qiskit_qulacs/version.py
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.108045 qiskit_qulacs-0.0.0/qiskit_qulacs.egg-info/
--rw-r--r--   0 gopald    (1000) gopald    (1000)    18961 2024-04-02 14:49:05.000000 qiskit_qulacs-0.0.0/qiskit_qulacs.egg-info/PKG-INFO
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2493 2024-04-02 14:49:05.000000 qiskit_qulacs-0.0.0/qiskit_qulacs.egg-info/SOURCES.txt
--rw-rw-r--   0 gopald    (1000) gopald    (1000)        1 2024-04-02 14:49:05.000000 qiskit_qulacs-0.0.0/qiskit_qulacs.egg-info/dependency_links.txt
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      505 2024-04-02 14:49:05.000000 qiskit_qulacs-0.0.0/qiskit_qulacs.egg-info/requires.txt
--rw-rw-r--   0 gopald    (1000) gopald    (1000)       14 2024-04-02 14:49:05.000000 qiskit_qulacs-0.0.0/qiskit_qulacs.egg-info/top_level.txt
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      381 2024-04-02 13:52:02.000000 qiskit_qulacs-0.0.0/requirements-dev.txt
--rw-rw-r--   0 gopald    (1000) gopald    (1000)       98 2024-04-01 15:24:33.000000 qiskit_qulacs-0.0.0/requirements.txt
--rw-rw-r--   0 gopald    (1000) gopald    (1000)       38 2024-04-02 14:49:05.112045 qiskit_qulacs-0.0.0/setup.cfg
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      214 2023-12-01 08:15:47.000000 qiskit_qulacs-0.0.0/setup.py
-drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2024-04-02 14:49:05.108045 qiskit_qulacs-0.0.0/tests/
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2590 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/tests/README.md
--rw-rw-r--   0 gopald    (1000) gopald    (1000)        0 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.0/tests/__init__.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    15057 2024-04-01 16:57:08.000000 qiskit_qulacs-0.0.0/tests/test_adapter.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     5357 2024-04-01 13:41:25.000000 qiskit_qulacs-0.0.0/tests/test_qulacs_backend.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    13800 2024-03-31 18:26:53.000000 qiskit_qulacs-0.0.0/tests/test_qulacs_estimator.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     9934 2024-03-31 18:26:31.000000 qiskit_qulacs-0.0.0/tests/test_qulacs_estimator_gradient.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)        0 2024-03-31 13:51:35.000000 qiskit_qulacs-0.0.0/tests/test_qulacs_job.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      923 2024-03-31 18:37:02.000000 qiskit_qulacs-0.0.0/tests/test_qulacs_provider.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)    16118 2024-04-01 11:39:11.000000 qiskit_qulacs-0.0.0/tests/test_qulacs_sampler.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)     2251 2024-04-01 13:40:28.000000 qiskit_qulacs-0.0.0/tests/utils.py
--rw-rw-r--   0 gopald    (1000) gopald    (1000)      922 2024-04-01 17:27:07.000000 qiskit_qulacs-0.0.0/tox.ini
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.719467 qiskit_qulacs-0.0.1/
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/.github/
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      342 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      342 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/ISSUE_TEMPLATE/enhancement_request.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      332 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      552 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      118 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/dependabot.yml
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/.github/workflows/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     3747 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/workflows/README.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     2092 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/workflows/citation.yml
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      869 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/workflows/coverage.yml
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      875 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/workflows/docs.yml
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      558 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/workflows/ecosystem.yml
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      537 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/workflows/lint.yml
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     1189 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.github/workflows/test_latest_versions.yml
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      547 2023-07-18 14:16:34.000000 qiskit_qulacs-0.0.1/.gitignore
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)    17583 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.pylintrc
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      528 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/.travis.yml
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      398 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     1184 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/CONTRIBUTING.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     1258 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/INSTALL.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)    11416 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/LICENSE.txt
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)    17148 2023-07-19 05:25:35.719467 qiskit_qulacs-0.0.1/PKG-INFO
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     3024 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/README.md
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/benchmarks/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      784 2023-07-17 13:51:25.000000 qiskit_qulacs-0.0.1/benchmarks/benchmark_qulacs_qiskit_estimator.csv
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      757 2023-07-17 13:55:03.000000 qiskit_qulacs-0.0.1/benchmarks/benchmark_qulacs_qiskit_grad.csv
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      798 2023-07-17 13:50:42.000000 qiskit_qulacs-0.0.1/benchmarks/benchmark_qulacs_qiskit_sv_simulation.csv
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)   208111 2023-07-17 13:55:20.000000 qiskit_qulacs-0.0.1/benchmarks/qiskit-qulacs-benchmark.ipynb
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/docs/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)        0 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/.nojekyll
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/docs/_static/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      412 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/_static/custom.css
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/docs/_static/images/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)    46937 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/_static/images/est_sim.png
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)    45919 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/_static/images/grad_sim.png
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)   201546 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/_static/images/logo.png
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)   550683 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/_static/images/logo_extended.png
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)    42526 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/_static/images/sv_sim.png
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/docs/apidocs/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      146 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/apidocs/index.rst
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)       76 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/apidocs/modules.rst
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     1412 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/apidocs/qiskit_qulacs.rst
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     2336 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/beginners_guide.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     2033 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/conf.py
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     2609 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/file-map-and-description.md
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/docs/how_tos/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     3386 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/how_tos/example_how_to.ipynb
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)       31 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/how_tos/index.rst
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      480 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/index.rst
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      615 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/project_overview.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     3378 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/quickstart_guide.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      169 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/technical_docs.md
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.715468 qiskit_qulacs-0.0.1/docs/tutorials/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)    76729 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/tutorials/Variational Quantum Eigensolver (VQE).ipynb
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)       30 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/tutorials/index.rst
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      328 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/docs/zenodo-integration.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      424 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/ecosystem.json
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      171 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/mypy.ini
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     1245 2023-07-18 18:22:06.000000 qiskit_qulacs-0.0.1/pyproject.toml
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.719467 qiskit_qulacs-0.0.1/qiskit_qulacs/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      295 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/qiskit_qulacs/__init__.py
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     6871 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/qiskit_qulacs/adapter.py
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     2464 2023-07-18 18:27:08.000000 qiskit_qulacs-0.0.1/qiskit_qulacs/qulacs_backend.py
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     3955 2023-07-18 18:27:38.000000 qiskit_qulacs-0.0.1/qiskit_qulacs/qulacs_estimator.py
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     2091 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/qiskit_qulacs/qulacs_estimator_gradient.py
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     1437 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/qiskit_qulacs/qulacs_job.py
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      558 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/qiskit_qulacs/qulacs_provider.py
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)       59 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/qiskit_qulacs/version.py
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.719467 qiskit_qulacs-0.0.1/qiskit_qulacs.egg-info/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)    17148 2023-07-19 05:25:35.000000 qiskit_qulacs-0.0.1/qiskit_qulacs.egg-info/PKG-INFO
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     1831 2023-07-19 05:25:35.000000 qiskit_qulacs-0.0.1/qiskit_qulacs.egg-info/SOURCES.txt
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)        1 2023-07-19 05:25:35.000000 qiskit_qulacs-0.0.1/qiskit_qulacs.egg-info/dependency_links.txt
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      321 2023-07-19 05:25:35.000000 qiskit_qulacs-0.0.1/qiskit_qulacs.egg-info/requires.txt
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)       20 2023-07-19 05:25:35.000000 qiskit_qulacs-0.0.1/qiskit_qulacs.egg-info/top_level.txt
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)      119 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/requirements.txt
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)       38 2023-07-19 05:25:35.719467 qiskit_qulacs-0.0.1/setup.cfg
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     1664 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/setup.py
+drwxrwxr-x   0 gopald    (1000) gopald    (1000)        0 2023-07-19 05:25:35.719467 qiskit_qulacs-0.0.1/tests/
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     2590 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/tests/README.md
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)        0 2023-07-18 14:15:39.000000 qiskit_qulacs-0.0.1/tests/__init__.py
+-rw-rw-r--   0 gopald    (1000) gopald    (1000)     1094 2023-07-18 18:04:44.000000 qiskit_qulacs-0.0.1/tox.ini
```

### Comparing `qiskit_qulacs-0.0.0/.github/PULL_REQUEST_TEMPLATE.md` & `qiskit_qulacs-0.0.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `qiskit_qulacs-0.0.0/.github/workflows/README.md` & `qiskit_qulacs-0.0.1/.github/workflows/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_qulacs-0.0.0/.github/workflows/citation.yml` & `qiskit_qulacs-0.0.1/.github/workflows/citation.yml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     paths: ['CITATION.bib', '.github/workflows/citation.yml']
 
 jobs:
   build-preview:
     runs-on: ubuntu-latest
     timeout-minutes: 20
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
       - name: Check for non-ASCII characters
         run: |
           # Fail immediately if there are any non-ASCII characters in
           # the BibTeX source.  We prefer "escaped codes" rather than
           # UTF-8 characters in order to ensure the bibliography will
           # display correctly even in documents that do not contain
           # \usepackage[utf8]{inputenc}.
```

### Comparing `qiskit_qulacs-0.0.0/.github/workflows/coverage.yml` & `qiskit_qulacs-0.0.1/.github/workflows/coverage.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - 'stable/**'
 
 jobs:
   coverage:
     runs-on: ubuntu-latest
     timeout-minutes: 60
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
       - name: Set up Python 3.9
         uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install tox
         run: |
           python -m pip install --upgrade pip
```

### Comparing `qiskit_qulacs-0.0.0/.github/workflows/docs.yml` & `qiskit_qulacs-0.0.1/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       - 'stable/**'
 
 jobs:
   build_and_deploy_docs:
     runs-on: ubuntu-latest
     timeout-minutes: 60
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox
```

### Comparing `qiskit_qulacs-0.0.0/.github/workflows/lint.yml` & `qiskit_qulacs-0.0.1/.github/workflows/lint.yml`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,15 @@
       - 'stable/**'
 
 jobs:
   lint:
     runs-on: ubuntu-latest
     timeout-minutes: 30
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
       - name: Set up Python 3.9
         uses: actions/setup-python@v4
         with:
           python-version: '3.9'
       - name: Install tox
         run: |
           python -m pip install --upgrade pip
```

### Comparing `qiskit_qulacs-0.0.0/.github/workflows/test_latest_versions.yml` & `qiskit_qulacs-0.0.1/.github/workflows/test_latest_versions.yml`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,22 @@
   tests:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 60
     strategy:
       max-parallel: 4
       matrix:
         os: [ubuntu-latest]
-        python-version: [3.8, 3.9, '3.10', '3.11']
+        python-version: [3.7, 3.8, 3.9, '3.10']
         include:
           - os: macos-latest
-            python-version: 3.8
-          # - os: windows-latest
-          #   python-version: 3.8
+            python-version: 3.7
+          - os: windows-latest
+            python-version: 3.7
     steps:
-      - uses: actions/checkout@v4
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
```

### Comparing `qiskit_qulacs-0.0.0/.gitignore` & `qiskit_qulacs-0.0.1/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 .ipynb_checkpoints
 __pycache__
 .DS_Store
 
 venv/
 .idea/
 .vscode/
-.mypy_cache/
-bin/
-install.sh
-/qulacs
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
 dist/
@@ -47,12 +43,13 @@
 .python-version
 
 # dotenv
 .env
 
 # virtualenv
 ENV/
-qq/
+qislacs
 
 # Sphinx documentation
 docs/_build/
-docs/stubs/
+docs/stubs/
+qiskit-qulacs-backend.ipynb
```

### Comparing `qiskit_qulacs-0.0.0/.travis.yml` & `qiskit_qulacs-0.0.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `qiskit_qulacs-0.0.0/CONTRIBUTING.md` & `qiskit_qulacs-0.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qiskit_qulacs-0.0.0/LICENSE.txt` & `qiskit_qulacs-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit_qulacs-0.0.0/PKG-INFO` & `qiskit_qulacs-0.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_qulacs
-Version: 0.0.0
+Version: 0.0.1
 Summary: Qiskit Qulacs to execute Qiskit programs using Qulacs as backend.
 Author-email: Gopal Ramesh Dahale <dahalegopal27@gmail.com>
 License:                     Copyright 2021 IBM and its contributors
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -205,82 +205,52 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/Gopal-Dahale/qiskit-qulacs
 Project-URL: Bug Tracker, https://github.com/Gopal-Dahale/qiskit-qulacs/issues
-Project-URL: Documentation, https://qiskit-qulacs.netlify.app/
-Project-URL: Repository, https://github.com/Gopal-Dahale/qiskit-qulacs
+Keywords: qiskit qulacs quantum
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: certifi>=2021.5.30
-Requires-Dist: importlib_metadata>=4.8.1
-Requires-Dist: qiskit-aer>=0.12.2
-Requires-Dist: qiskit>=1.0.0
-Requires-Dist: qiskit-algorithms>=0.3.0
-Requires-Dist: qulacs>=0.5.0
 Provides-Extra: dev
-Requires-Dist: coverage>=5.5; extra == "dev"
-Requires-Dist: matplotlib>=3.3; extra == "dev"
-Requires-Dist: qiskit-nature>=0.7.2; extra == "dev"
-Requires-Dist: pyscf>=2.5.0; extra == "dev"
-Requires-Dist: pylatexenc>=1.4; extra == "dev"
-Requires-Dist: pylint>=2.9.5; extra == "dev"
-Requires-Dist: nbqa>=1.1.1; extra == "dev"
-Requires-Dist: treon>=0.1.3; extra == "dev"
-Requires-Dist: pytest>=6.2.5; extra == "dev"
-Requires-Dist: pytest-randomly>=1.2.0; extra == "dev"
-Requires-Dist: mypy>=0.780; extra == "dev"
-Requires-Dist: mypy-extensions>=0.4.3; extra == "dev"
-Requires-Dist: jupyter-sphinx>=0.3.2; extra == "dev"
-Requires-Dist: nbsphinx>=0.8.8; extra == "dev"
-Requires-Dist: sphinx-autodoc-typehints>=1.17.0; extra == "dev"
-Requires-Dist: reno>=3.5.0; extra == "dev"
-Requires-Dist: black[jupyter]~=22.1; extra == "dev"
-Requires-Dist: tox==3.24.5; extra == "dev"
-Requires-Dist: ddt!=1.4.0,!=1.4.3,>=1.2.0; extra == "dev"
-Requires-Dist: myst_parser>=1.0.0; extra == "dev"
-Requires-Dist: qiskit-sphinx-theme>=1.14.0; extra == "dev"
-
-![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS-informational)
-[![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational)](https://www.python.org/)
-[![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%201.0.0-6133BD)](https://github.com/Qiskit/qiskit)
+License-File: LICENSE.txt
+
+![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS%20%7C%20Windows-informational)
+[![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational)](https://www.python.org/)
+[![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.34.2-6133BD)](https://github.com/Qiskit/qiskit)
 [![License](https://img.shields.io/github/license/qiskit-community/quantum-prototype-template?label=License)](https://github.com/qiskit-community/quantum-prototype-template/blob/main/LICENSE.txt)
 [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
-[![PyPI version](https://badge.fury.io/py/qiskit-qulacs.svg)](https://badge.fury.io/py/qiskit-qulacs)
-[![Tests](https://github.com/Gopal-Dahale/qiskit-qulacs/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/Gopal-Dahale/qiskit-qulacs/actions/workflows/test_latest_versions.yml)
-[![Coverage Status](https://coveralls.io/repos/github/Gopal-Dahale/qiskit-qulacs/badge.svg?branch=main)](https://coveralls.io/github/Gopal-Dahale/qiskit-qulacs?branch=main)
+<!-- [![Tests](https://github.com/qiskit-community/quantum-prototype-template/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/qiskit-community/quantum-prototype-template/actions/workflows/test_latest_versions.yml)
+[![Coverage](https://coveralls.io/repos/github/qiskit-community/quantum-prototype-template/badge.svg?branch=main)](https://coveralls.io/github/qiskit-community/quantum-prototype-template?branch=main) -->
 
-![Qiskit-Qulacs-logo-extended](https://github.com/Gopal-Dahale/qiskit-qulacs/assets/49199003/27116cba-4109-4298-baac-0a35d04c5ab5)
+![Qiskit-Qulacs](docs/_static/images/logo_extended.png)
 
-Qiskit-Qulacs allows users to execute Qiskit programs using Qulacs backend.
+Qiskit-Qulacs allows user to execute Qiskit programs using Qulacs backend.
 
-**Qiskit-Qulacs is actively being developed, and we welcome your input and suggestions on the API and use cases. If you have any ideas or feedback, please open a GitHub issue or contact us. We are interested in hearing about your experiences using the library.**
+**Qiskit-Qulacs is actively being developed, and we welcome your input and suggestions on the API and use-cases. If you have any ideas or feedback, please feel free to open a GitHub issue or contact us. We are interested in hearing about your experiences using the library.**
 
 
-1.  [About](docs/intro/project_overview.md)
-2.  [Beginner's Guide](docs/intro/beginners_guide.md)
-3.  [Installation](docs/intro/INSTALL.md)
-4.  [Quickstart Guide](docs/intro/quickstart_guide.md)
+
+1.  [About](docs/project_overview.md)
+2.  [Beginner's Guide](docs/beginners_guide.md)
+3.  [Installation](INSTALL.md)
+4.  [Quickstart Guide](docs/quickstart_guide.md)
 5.  [Tutorials](docs/tutorials/)
 6.  [How-Tos](docs/how_tos/)
 8.  [How to Give Feedback](#how-to-give-feedback)
 9.  [Contribution Guidelines](#contribution-guidelines)
 10. [References and Acknowledgements](#references-and-acknowledgements)
 11. [License](#license)
 
@@ -298,25 +268,22 @@
 - [Opening an issue](https://github.com/Gopal-Dahale/qiskit-qulacs/issues) in the repository
 
 
 ----------------------------------------------------------------------------------------------------
 
 ### Contribution Guidelines
 
-For information on contributing to this project, please take a look at our [contribution guidelines](CONTRIBUTING.md).
+For information on how to contribute to this project, please take a look at our [contribution guidelines](CONTRIBUTING.md).
 
 
 ----------------------------------------------------------------------------------------------------
 
 ## References and Acknowledgements
 [1] Qiskit https://qiskit.org/ \
 [2] Qiskit-terra https://github.com/Qiskit/qiskit-terra \
 [3] Qulacs https://github.com/qulacs/qulacs
 
-We are proud to be supported by the [Unitary Fund microgrant program](https://unitary.fund/grants/). Thank you Unitary Fund.
-
-[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](https://unitary.fund)
 
 ----------------------------------------------------------------------------------------------------
 
 ### License
 [Apache License 2.0](LICENSE.txt)
```

### Comparing `qiskit_qulacs-0.0.0/README.md` & `qiskit_qulacs-0.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS-informational)
-[![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational)](https://www.python.org/)
-[![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%201.0.0-6133BD)](https://github.com/Qiskit/qiskit)
+![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS%20%7C%20Windows-informational)
+[![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational)](https://www.python.org/)
+[![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.34.2-6133BD)](https://github.com/Qiskit/qiskit)
 [![License](https://img.shields.io/github/license/qiskit-community/quantum-prototype-template?label=License)](https://github.com/qiskit-community/quantum-prototype-template/blob/main/LICENSE.txt)
 [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
-[![PyPI version](https://badge.fury.io/py/qiskit-qulacs.svg)](https://badge.fury.io/py/qiskit-qulacs)
-[![Tests](https://github.com/Gopal-Dahale/qiskit-qulacs/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/Gopal-Dahale/qiskit-qulacs/actions/workflows/test_latest_versions.yml)
-[![Coverage Status](https://coveralls.io/repos/github/Gopal-Dahale/qiskit-qulacs/badge.svg?branch=main)](https://coveralls.io/github/Gopal-Dahale/qiskit-qulacs?branch=main)
+<!-- [![Tests](https://github.com/qiskit-community/quantum-prototype-template/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/qiskit-community/quantum-prototype-template/actions/workflows/test_latest_versions.yml)
+[![Coverage](https://coveralls.io/repos/github/qiskit-community/quantum-prototype-template/badge.svg?branch=main)](https://coveralls.io/github/qiskit-community/quantum-prototype-template?branch=main) -->
 
-![Qiskit-Qulacs-logo-extended](https://github.com/Gopal-Dahale/qiskit-qulacs/assets/49199003/27116cba-4109-4298-baac-0a35d04c5ab5)
+![Qiskit-Qulacs](docs/_static/images/logo_extended.png)
 
-Qiskit-Qulacs allows users to execute Qiskit programs using Qulacs backend.
+Qiskit-Qulacs allows user to execute Qiskit programs using Qulacs backend.
 
-**Qiskit-Qulacs is actively being developed, and we welcome your input and suggestions on the API and use cases. If you have any ideas or feedback, please open a GitHub issue or contact us. We are interested in hearing about your experiences using the library.**
+**Qiskit-Qulacs is actively being developed, and we welcome your input and suggestions on the API and use-cases. If you have any ideas or feedback, please feel free to open a GitHub issue or contact us. We are interested in hearing about your experiences using the library.**
 
 
-1.  [About](docs/intro/project_overview.md)
-2.  [Beginner's Guide](docs/intro/beginners_guide.md)
-3.  [Installation](docs/intro/INSTALL.md)
-4.  [Quickstart Guide](docs/intro/quickstart_guide.md)
+
+1.  [About](docs/project_overview.md)
+2.  [Beginner's Guide](docs/beginners_guide.md)
+3.  [Installation](INSTALL.md)
+4.  [Quickstart Guide](docs/quickstart_guide.md)
 5.  [Tutorials](docs/tutorials/)
 6.  [How-Tos](docs/how_tos/)
 8.  [How to Give Feedback](#how-to-give-feedback)
 9.  [Contribution Guidelines](#contribution-guidelines)
 10. [References and Acknowledgements](#references-and-acknowledgements)
 11. [License](#license)
 
@@ -39,25 +39,22 @@
 - [Opening an issue](https://github.com/Gopal-Dahale/qiskit-qulacs/issues) in the repository
 
 
 ----------------------------------------------------------------------------------------------------
 
 ### Contribution Guidelines
 
-For information on contributing to this project, please take a look at our [contribution guidelines](CONTRIBUTING.md).
+For information on how to contribute to this project, please take a look at our [contribution guidelines](CONTRIBUTING.md).
 
 
 ----------------------------------------------------------------------------------------------------
 
 ## References and Acknowledgements
 [1] Qiskit https://qiskit.org/ \
 [2] Qiskit-terra https://github.com/Qiskit/qiskit-terra \
 [3] Qulacs https://github.com/qulacs/qulacs
 
-We are proud to be supported by the [Unitary Fund microgrant program](https://unitary.fund/grants/). Thank you Unitary Fund.
-
-[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](https://unitary.fund)
 
 ----------------------------------------------------------------------------------------------------
 
 ### License
-[Apache License 2.0](LICENSE.txt)
+[Apache License 2.0](LICENSE.txt)
```

### Comparing `qiskit_qulacs-0.0.0/docs/_static/images/logo.png` & `qiskit_qulacs-0.0.1/docs/_static/images/logo.png`

 * *Files identical despite different names*

### Comparing `qiskit_qulacs-0.0.0/docs/_static/images/logo_extended.png` & `qiskit_qulacs-0.0.1/docs/_static/images/logo_extended.png`

 * *Files identical despite different names*

### Comparing `qiskit_qulacs-0.0.0/docs/apidocs/qiskit_qulacs.rst` & `qiskit_qulacs-0.0.1/docs/apidocs/qiskit_qulacs.rst`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,14 @@
 -----------------------------
 
 .. automodule:: qiskit_qulacs.adapter
    :members:
    :undoc-members:
    :show-inheritance:
 
-qiskit\_qulacs.backend\_utils module
-------------------------------------
-
-.. automodule:: qiskit_qulacs.backend_utils
-   :members:
-   :undoc-members:
-   :show-inheritance:
-
 qiskit\_qulacs.qulacs\_backend module
 -------------------------------------
 
 .. automodule:: qiskit_qulacs.qulacs_backend
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `qiskit_qulacs-0.0.0/docs/conf.py` & `qiskit_qulacs-0.0.1/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,29 +12,23 @@
 
 # pylint: disable=invalid-name
 
 """
 Sphinx documentation builder
 """
 
-import datetime
-import os
-
 # General options:
 from pathlib import Path
-from typing import Any, Dict, Optional
-
+import os
+from typing import Optional, Dict, Any
 from importlib_metadata import version as metadata_version
 
 project = "Qiskit-Qulacs"
+copyright = "2023"  # pylint: disable=redefined-builtin
 author = "Gopal Ramesh Dahale"
-copyright = (
-    f"2023-{datetime.date.today().year}, {author}"  # pylint: disable=redefined-builtin
-)
-
 
 _rootdir = Path(__file__).parent.parent
 
 # The full version, including alpha/beta/rc tags
 version_path = os.path.join(
     os.path.dirname(os.path.abspath(__file__)),
     "..",
@@ -53,36 +47,30 @@
     "sphinx.ext.mathjax",
     "sphinx.ext.viewcode",
     "sphinx.ext.extlinks",
     "jupyter_sphinx",
     "sphinx_autodoc_typehints",
     "reno.sphinxext",
     "nbsphinx",
-    "myst_parser",
-    "qiskit_sphinx_theme",
 ]
 templates_path = ["_templates"]
 numfig = True
 numfig_format = {"table": "Table %s"}
 language = "en"
 pygments_style = "colorful"
 add_module_names = False
 modindex_common_prefix = ["qiskit_qulacs."]
 
 # html theme options
-html_theme = "qiskit-ecosystem"
 html_static_path = ["_static"]
-# html_logo = "_static/images/logo.png"
-html_last_updated_fmt = "%Y/%m/%d"
-html_title = f"{project} {version}"
-
+html_logo = "_static/images/logo.png"
 
 # autodoc/autosummary options
 autosummary_generate = True
 autosummary_generate_overwrite = False
 autoclass_content = "both"
 
 # nbsphinx options (for tutorials)
 nbsphinx_timeout = 180
 nbsphinx_execute = "always"
 nbsphinx_widgets_path = ""
-exclude_patterns = ["_build", "**.ipynb_checkpoints"]
+exclude_patterns = ["_build", "**.ipynb_checkpoints"]
```

### Comparing `qiskit_qulacs-0.0.0/docs/file-map-and-description.md` & `qiskit_qulacs-0.0.1/docs/file-map-and-description.md`

 * *Files identical despite different names*

### Comparing `qiskit_qulacs-0.0.0/docs/intro/INSTALL.md` & `qiskit_qulacs-0.0.1/docs/beginners_guide.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,60 @@
-# Installation Guide
+# Qiskit-Qulacs Beginner's Guide
 
-This document provides step-by-step instructions to set up the Python environment, install dependencies, and install the Qiskit-Qulacs plugin.
+Welcome to the Qiskit-Qulacs Beginner's Guide! This guide is designed to provide new users with an overview of the Qiskit-Qulacs project and its capabilities. It will walk you through the installation process, introduce you to the basics of the API, and provide an example problem to solve using the software.
 
-Setting up Python Environment
-## Setting up Python Environment
+## About the Project
 
-Create a fresh Python environment using your preferred method (e.g., virtualenv, conda).
+Qiskit-Qulacs is a plugin for Qiskit that integrates the Qulacs library as a backend. The project aims to provide users with a powerful tool for quantum computing simulations and algorithm development. By leveraging [Qulacs'](https://github.com/qulacs/qulacs#performance) high-performance quantum circuit simulator, users can explore and experiment with various quantum computing concepts and algorithms.
 
-```
-virtualenv qiskit-qulacs-env
-source qiskit-qulacs-env/bin/activate
-```
-
-Ensure that you have a compatible version of Python (e.g., Python 3.7 or higher) installed in the environment.
+## Installation
+To get started with Qiskit-Qulacs, follow these steps for installation:
 
-## Installing Qiskit-Qulacs Software
+Install Python and virtual env. Then follow the below steps.
 
-### Start locally
-
-The simplest way to get started is to use the pip package manager:
-
-```
-pip install qiskit-qulacs
-```
-
-### Install from source
-
-Installing Qiskit-Qulacs from source allows you to access the most recently updated version under development, instead of using the version in the Python Package Index (PyPI) repository.
-
-1. Clone the Qiskit Algorithms repository.
 ```
 git clone https://github.com/Gopal-Dahale/qiskit-qulacs.git
-```
-2. Cloning the repository creates a local folder called ``qiskit-qulacs``.
-```
 cd qiskit-qulacs
-```
-3. Install ``qiskit-qulacs``.
-```
+virtualenv venv
+.
+.
+.
+.venv/bin/activate
+pip install -r requirements.txt
 pip install .
 ```
-If you want to install it in editable mode, meaning that code changes to the project don't require a reinstall to be applied, you can do this with:
-```
-pip install -e .
-```
 
-## Testing the Installation
+## Usage
+
+Once installed, you can use Qiskit-Qulacs through the Qiskit API. Here are some key points to understand:
 
-Since Qiskit-Qulacs is currently under heavy development, there are no tests yet. However, you can test the installation using a simple program:
+1. You can access Qulacs Backend through `QualcsProvider` class and can perform statevector simulations.
+2. For machine learning application, we can created a `QualcsEstimator` class along with `QulacsEstimatorGradient` for efficient forward and backward passes.
+
+
+## Example Problem
+
+To demonstrate the usage of Qiskit-Qulacs, let's solve a simple example problem: creating an entangled state.
 
 ```python
-from qiskit import QuantumCircuit
+import qiskit
 from qiskit_qulacs import QulacsProvider
 
-# Create a bell state
-qc = QuantumCircuit(2)
+# Create a quantum circuit
+qc = qiskit.QuantumCircuit(2)
 qc.h(0)
 qc.cx(0, 1)
 
 # Use Qiskit-Qulacs to run the circuit
-backend = QulacsProvider().get_backend('qulacs_simulator')
+backend = QulacsProvider().get_backend('statevector_simulator')
 result = backend.run(qc).result()
 
 # Get the statevector
 statevector = result.get_statevector()
 
 # Print the statevector
 print(statevector)
+```
+
+## Conclusion
 
-# Output: [0.70710678+0.j 0.        +0.j 0.        +0.j 0.70710678+0.j]
-```
+Congratulations! You have completed the Qiskit-Qulacs Beginner's Guide. You should now have a basic understanding of the project, how to install it, and how to use the Qiskit-Qulacs API. Feel free to explore more advanced features and experiment with different quantum circuits and algorithms. Happy quantum computing!
```

### Comparing `qiskit_qulacs-0.0.0/docs/intro/quickstart_guide.md` & `qiskit_qulacs-0.0.1/docs/quickstart_guide.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quickstart Guide
 
 Welcome to the Quickstart Guide for Qiskit-Qulacs! This guide will help you quickly get started with using Qiskit-Qulacs as a backend for Qiskit and exploring its functionality.
 
 ## Installation
 
-See [Installation Guide](INSTALL.md) for instructions.
+See [INSTALL.md](INSTALL.md) for installation instructions.
 
 ## Usage
 
 Once you have installed the necessary dependencies, you can start using Qiskit-Qulacs. Here's a brief overview of the main components and their usage:
 
 ###  QulacsProvider
 The QulacsProvider uses qiskit's Provider Interface and allows you to perform local statevector simulations with Qulacs as the backend. You can import and initialize it as follows:
@@ -27,48 +27,44 @@
 
 # Create a quantum circuit
 qc = qiskit.QuantumCircuit(2)
 qc.h(0)
 qc.cx(0, 1)
 
 # Use Qiskit-Qulacs to run the circuit
-backend = QulacsProvider().get_backend('qulacs_simulator')
+backend = QulacsProvider().get_backend('statevector_simulator')
 result = backend.run(qc).result()
 
 # Get the statevector
 statevector = result.get_statevector()
 
 # Print the statevector
 print(statevector)
-
-# Output: [0.70710678+0.j 0.        +0.j 0.        +0.j 0.70710678+0.j]
 ```
 
 ### QulacsEstimator
-The QulacsEstimator is based on qiskit's estimator primitive but behind the scenes uses qulacs to compute the expectation values quickly. It allows you to estimate expectation values of observables using Qulacs. Here's a basic example of how to use it:
+The QulacsEstimator is based on qiskit's estimator primitive. It allows you to estimate expectation values of observables using Qulacs. Here's a basic example of how to use it:
 
 ```python
-import numpy as np
 from qiskit.circuit.library import TwoLocal
-from qiskit.quantum_info import SparsePauliOp
-
 from qiskit_qulacs.qulacs_estimator import QulacsEstimator
-
-np.random.seed(42)
+from qiskit.quantum_info import SparsePauliOp
+import numpy as np
 
 # Create a two-local quantum circuit with 3 qubits
-qc = TwoLocal(
-    3, ["ry", "rz", "rx"], ["cx"], "linear", 1, insert_barriers=False
-).decompose()
+qc = TwoLocal(3, ['ry', 'rz', 'rx'], ['cx'],
+              'linear',
+              1,
+              insert_barriers=False).decompose()
 
 # Generate random parameter values for the circuit
 params = np.random.rand(qc.num_parameters)
 
 # Create a SparsePauliOp observable
-obs = SparsePauliOp.from_list([("Z" * qc.num_qubits, 0.5)])
+obs = SparsePauliOp.from_list([('Z' * qc.num_qubits, 0.5)])
 
 # Initialize QulacsEstimator
 qulacs_estimator = QulacsEstimator()
 
 # Run the estimation job with the circuit, observable, and parameters
 job = qulacs_estimator.run(qc, obs, params)
 
@@ -76,48 +72,31 @@
 result = job.result()
 
 # Retrieve the expectation value from the result
 expectation_value = result.values[0]
 
 # Print the expectation value
 print("Expectation value:", expectation_value)
-
-# Output: Expectation value: -0.018581644467403284
 ```
 
 ### QulacsEstimatorGradient
-The QulacsEstimatorGradient is based to qiskit's gradient framework. It allows you to compute gradients of quantum circuits using Qulacs. Here's a basic 1 qubit example.
+The QulacsEstimatorGradient is based to qiskit's gradient framework. It allows you to compute gradients of quantum circuits using Qulacs. Here's a basic example in based on the previous code:
 
 ```python
-import numpy as np
-from qiskit import QuantumCircuit
-from qiskit.circuit import Parameter
-from qiskit.quantum_info import SparsePauliOp
-
 from qiskit_qulacs.qulacs_estimator_gradient import QulacsEstimatorGradient
 
-# Create a two-local quantum circuit with 1 qubit with a parameter
-qc = QuantumCircuit(1)
-
-x = Parameter("x")
-qc.rx(x, 0)
+qulacs_grad = QulacsEstimatorGradient(qulacs_estimator)
 
-# Create a SparsePauliOp observable
-obs = SparsePauliOp.from_list([("Z" * qc.num_qubits, 0.5)])
-
-# Initialize QulacsEstimatorGradient
-qulacs_grad = QulacsEstimatorGradient()
+job = qulacs_grad.run(
+    [qc],
+    [obs],
+    [params],
+)
 
-# Run the job with the circuit, observable, and parameters
-job = qulacs_grad.run([qc], [obs], [[np.pi / 3]])
-
-# Get the result of the job and retrieve the gradients
 result = job.result()
 gradient = result.gradients[0]
 
 print("Gradient:", gradient)
-
-# Output: Gradient: [-0.4330127]
 ```
 
 ## Conclusion
 Congratulations! You have completed the Quickstart Guide for Qiskit-Qulacs. You should now have a basic understanding of the installation process and how to use the main components of Qiskit-Qulacs. Feel free to refer to the documentation and examples for more advanced usage and explore the possibilities of quantum computing with Qiskit-Qulacs. Happy coding!
```

### Comparing `qiskit_qulacs-0.0.0/docs/tutorials/03_vqe.ipynb` & `qiskit_qulacs-0.0.1/docs/tutorials/Variational Quantum Eigensolver (VQE).ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9577567664271096%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'The tutorials requires `qiskit-nature` package which "*

 * *            'can be installed with '*

 * *            "[these](https://qiskit.org/ecosystem/nature/getting_started.html) instructions.')], "*

 * *            "delete: [2]}}, 2: {'id': '8b1f3a86', 'source': {insert: [(8, 'from "*

 * *            "qiskit.algorithms.optimizers import L_BFGS_B\\n'), (9, 'from "*

 * *            "qiskit.algorithms.minimum_eigensolvers import NumPyMinimumEigensolver, VQE\\n'), (14, "*

 * *            "'setti […]*

```diff
@@ -3,48 +3,54 @@
         {
             "cell_type": "markdown",
             "id": "0f9cd670",
             "metadata": {},
             "source": [
                 "# Variational Quantum Eigensolver (VQE)\n",
                 "\n",
-                "The tutorial requires `qiskit-nature` package which can be installed with [these](https://qiskit.org/ecosystem/nature/getting_started.html) instructions. The tutorial assumes that the user is familiar with VQE. User's can follow the [Ground State Solvers](https://qiskit-community.github.io/qiskit-nature/tutorials/03_ground_state_solvers.html) tutorial by `qiskit-nature` for the same."
+                "The tutorials requires `qiskit-nature` package which can be installed with [these](https://qiskit.org/ecosystem/nature/getting_started.html) instructions."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "id": "3e95c988",
             "metadata": {},
             "outputs": [],
             "source": [
-                "\"\"\"Variational Quantum Eigensolver (VQE) tutorial.\"\"\"\n",
-                "\n",
+                "from qiskit.utils import algorithm_globals\n",
                 "from IPython.display import clear_output\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "\n",
+                "algorithm_globals.random_seed = 42"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "id": "8b1f3a86",
+            "metadata": {},
+            "outputs": [],
+            "source": [
                 "from qiskit_nature.units import DistanceUnit\n",
                 "from qiskit_nature.second_q.drivers import PySCFDriver\n",
                 "from qiskit_nature.second_q.mappers import JordanWignerMapper\n",
                 "from qiskit_nature.second_q.circuit.library import HartreeFock\n",
                 "from qiskit_nature.second_q.algorithms import GroundStateEigensolver\n",
                 "from qiskit_nature import settings\n",
                 "\n",
-                "from qiskit_algorithms.utils import algorithm_globals\n",
                 "from qiskit.circuit.library import EfficientSU2\n",
-                "from qiskit_algorithms.optimizers import L_BFGS_B\n",
-                "from qiskit_algorithms.minimum_eigensolvers import NumPyMinimumEigensolver, VQE\n",
+                "from qiskit.algorithms.optimizers import L_BFGS_B\n",
+                "from qiskit.algorithms.minimum_eigensolvers import NumPyMinimumEigensolver, VQE\n",
                 "\n",
                 "from qiskit_qulacs.qulacs_estimator import QulacsEstimator\n",
                 "from qiskit_qulacs.qulacs_estimator_gradient import QulacsEstimatorGradient\n",
                 "\n",
-                "settings.use_pauli_sum_op = False\n",
-                "\n",
-                "algorithm_globals.random_seed = 42"
+                "settings.use_pauli_sum_op = False"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "2650770d",
             "metadata": {},
@@ -65,18 +71,18 @@
             "id": "e88319ac",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "SparsePauliOp(['IIII', 'IIZI', 'IIIZ', 'IIZZ', 'IZII', 'IZIZ', 'YYYY', 'XXYY', 'YYXX', 'XXXX', 'ZIII', 'ZIIZ', 'IZZI', 'ZIZI', 'ZZII'],\n",
-                        "              coeffs=[-0.81054798+0.j, -0.22575349+0.j,  0.17218393+0.j,  0.12091263+0.j,\n",
-                        "  0.17218393+0.j,  0.16892754+0.j,  0.0452328 +0.j,  0.0452328 +0.j,\n",
-                        "  0.0452328 +0.j,  0.0452328 +0.j, -0.22575349+0.j,  0.16614543+0.j,\n",
+                        "SparsePauliOp(['IIII', 'IIIZ', 'IIZI', 'IZII', 'ZIII', 'IIZZ', 'IZIZ', 'YYYY', 'XXYY', 'YYXX', 'XXXX', 'ZIIZ', 'IZZI', 'ZIZI', 'ZZII'],\n",
+                        "              coeffs=[-0.81054798+0.j,  0.17218393+0.j, -0.22575349+0.j,  0.17218393+0.j,\n",
+                        " -0.22575349+0.j,  0.12091263+0.j,  0.16892754+0.j,  0.0452328 +0.j,\n",
+                        "  0.0452328 +0.j,  0.0452328 +0.j,  0.0452328 +0.j,  0.16614543+0.j,\n",
                         "  0.16614543+0.j,  0.17464343+0.j,  0.12091263+0.j])\n"
                     ]
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
@@ -168,15 +174,15 @@
                     "text": [
                         "Expected ground state energy: -1.857275030202 Ha\n"
                     ]
                 }
             ],
             "source": [
                 "exact_energy = res_actual.eigenvalues[0]\n",
-                "print(f\"Expected ground state energy: {exact_energy:.12f} Ha\")"
+                "print(f'Expected ground state energy: {exact_energy:.12f} Ha')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "id": "5bd9652a",
             "metadata": {},
@@ -194,89 +200,63 @@
                 }
             ],
             "source": [
                 "# Hartree focks state\n",
                 "num_particles = problem.num_particles\n",
                 "num_spatial_orbitals = problem.num_spatial_orbitals\n",
                 "\n",
-                "init_state = HartreeFock(\n",
-                "    num_spatial_orbitals=num_spatial_orbitals,\n",
-                "    num_particles=num_particles,\n",
-                "    qubit_mapper=mapper,\n",
-                ")\n",
+                "init_state = HartreeFock(num_spatial_orbitals=num_spatial_orbitals,\n",
+                "                         num_particles=num_particles,\n",
+                "                         qubit_mapper=mapper)\n",
                 "\n",
                 "# ansatz\n",
-                "ansatz = EfficientSU2(qubit_op.num_qubits, su2_gates=[\"ry\"]).decompose()\n",
+                "ansatz = EfficientSU2(qubit_op.num_qubits, su2_gates=['ry']).decompose()\n",
                 "\n",
                 "# Add the initial state\n",
                 "init_state.barrier()\n",
                 "ansatz = init_state.compose(ansatz)\n",
-                "ansatz.draw(\"mpl\")"
+                "ansatz.draw('mpl')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 9,
             "id": "9a657acc",
             "metadata": {},
             "outputs": [],
             "source": [
                 "intermediate_info = []\n",
                 "\n",
-                "\n",
-                "def callback(eval_count, parameters, value, std):  # pylint: disable=unused-argument\n",
-                "    \"\"\"\n",
-                "    A callback that can be registered with the optimizer to store the intermediate\n",
-                "    value and parameters.\n",
-                "    \"\"\"\n",
+                "def callback(eval_count, parameters, value, std):\n",
                 "    intermediate_info.append(value)\n",
                 "    clear_output(wait=True)\n",
-                "    plt.plot(\n",
-                "        intermediate_info,\n",
-                "        color=\"purple\",\n",
-                "        lw=2,\n",
-                "        label=f\"Simulated VQE {np.round(value,4)}\",\n",
-                "    )\n",
-                "    plt.ylabel(\"Energy\")\n",
-                "    plt.xlabel(\"Iterations\")\n",
-                "\n",
+                "    plt.plot(intermediate_info, color='purple', lw=2, label=f'Simulated VQE {np.round(value,4)}')\n",
+                "    plt.ylabel('Energy')\n",
+                "    plt.xlabel('Iterations')\n",
+                "    \n",
                 "    # Exact ground state energy value\n",
-                "    plt.axhline(\n",
-                "        y=exact_energy,\n",
-                "        color=\"tab:red\",\n",
-                "        ls=\"--\",\n",
-                "        lw=2,\n",
-                "        label=\"Target: \" + str(np.round(exact_energy, 4)),\n",
-                "    )\n",
+                "    plt.axhline(y=exact_energy,color=\"tab:red\",ls=\"--\", lw=2,label=\"Target: \"+str(np.round(exact_energy,4)))\n",
                 "    plt.legend()\n",
                 "    plt.grid()\n",
                 "    plt.show()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 10,
             "id": "1c02ffd5",
             "metadata": {},
             "outputs": [],
             "source": [
                 "optimizer = L_BFGS_B(maxiter=20)"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "1f568379",
-            "metadata": {},
-            "source": [
-                "We use primitives from `qiskit-qulacs` of computing the expectation value and gradient."
-            ]
-        },
-        {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 11,
             "id": "4b84785f",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/png": "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",
                         "text/plain": [
@@ -292,82 +272,84 @@
                     "text": [
                         "'Barrier' object has no attribute 'to_matrix'\n"
                     ]
                 }
             ],
             "source": [
                 "qulacs_estimator = QulacsEstimator()\n",
-                "qulacs_gradient = QulacsEstimatorGradient()\n",
+                "qulacs_gradient = QulacsEstimatorGradient(qulacs_estimator)\n",
                 "\n",
-                "vqe = VQE(\n",
-                "    qulacs_estimator, ansatz, optimizer, callback=callback, gradient=qulacs_gradient\n",
-                ")\n",
+                "vqe = VQE(qulacs_estimator, \n",
+                "          ansatz, \n",
+                "          optimizer, \n",
+                "          callback=callback, \n",
+                "          gradient=qulacs_gradient\n",
+                "         )\n",
                 "result = vqe.compute_minimum_eigenvalue(operator=qubit_op)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 14,
+            "execution_count": 12,
             "id": "b3f9ea6c",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "{   'aux_operators_evaluated': None,\n",
                         "    'cost_function_evals': 22,\n",
-                        "    'eigenvalue': -1.8567922267701438,\n",
-                        "    'optimal_circuit': <qiskit_nature.second_q.circuit.library.initial_states.hartree_fock.HartreeFock object at 0x7f669c77cfa0>,\n",
-                        "    'optimal_parameters': {   ParameterVectorElement(\u03b8[3]): 1.2095948974450008,\n",
-                        "                              ParameterVectorElement(\u03b8[5]): 5.666947151364115,\n",
-                        "                              ParameterVectorElement(\u03b8[7]): 2.4421112354369603,\n",
-                        "                              ParameterVectorElement(\u03b8[4]): -5.154494260584259,\n",
-                        "                              ParameterVectorElement(\u03b8[6]): 2.574344487887189,\n",
-                        "                              ParameterVectorElement(\u03b8[8]): -5.4101309605422525,\n",
-                        "                              ParameterVectorElement(\u03b8[9]): -1.261167613800019,\n",
-                        "                              ParameterVectorElement(\u03b8[10]): -0.9072274382237647,\n",
-                        "                              ParameterVectorElement(\u03b8[11]): 4.9799372946641896,\n",
-                        "                              ParameterVectorElement(\u03b8[12]): 2.755549835643393,\n",
-                        "                              ParameterVectorElement(\u03b8[13]): 3.4937762155898797,\n",
-                        "                              ParameterVectorElement(\u03b8[14]): 0.1388660021481062,\n",
-                        "                              ParameterVectorElement(\u03b8[15]): -3.654455036700619,\n",
-                        "                              ParameterVectorElement(\u03b8[2]): 5.325935798233085,\n",
-                        "                              ParameterVectorElement(\u03b8[1]): -1.3110309933023812,\n",
-                        "                              ParameterVectorElement(\u03b8[0]): 3.596756540143767},\n",
+                        "    'eigenvalue': -1.856792226770143,\n",
+                        "    'optimal_circuit': <qiskit_nature.second_q.circuit.library.initial_states.hartree_fock.HartreeFock object at 0x7f4423d17910>,\n",
+                        "    'optimal_parameters': {   ParameterVectorElement(\u03b8[1]): -1.311030993302368,\n",
+                        "                              ParameterVectorElement(\u03b8[2]): 5.325935798233073,\n",
+                        "                              ParameterVectorElement(\u03b8[3]): 1.2095948974450152,\n",
+                        "                              ParameterVectorElement(\u03b8[4]): -5.154494260584239,\n",
+                        "                              ParameterVectorElement(\u03b8[5]): 5.666947151364108,\n",
+                        "                              ParameterVectorElement(\u03b8[6]): 2.5743444878871973,\n",
+                        "                              ParameterVectorElement(\u03b8[7]): 2.44211123543697,\n",
+                        "                              ParameterVectorElement(\u03b8[8]): -5.410130960542249,\n",
+                        "                              ParameterVectorElement(\u03b8[9]): -1.2611676138000247,\n",
+                        "                              ParameterVectorElement(\u03b8[10]): -0.9072274382237897,\n",
+                        "                              ParameterVectorElement(\u03b8[11]): 4.979937294664183,\n",
+                        "                              ParameterVectorElement(\u03b8[12]): 2.7555498356433916,\n",
+                        "                              ParameterVectorElement(\u03b8[13]): 3.493776215589881,\n",
+                        "                              ParameterVectorElement(\u03b8[14]): 0.13886600214810552,\n",
+                        "                              ParameterVectorElement(\u03b8[15]): -3.6544550367006066,\n",
+                        "                              ParameterVectorElement(\u03b8[0]): 3.596756540143773},\n",
                         "    'optimal_point': array([ 3.59675654, -1.31103099,  5.3259358 ,  1.2095949 , -5.15449426,\n",
                         "        5.66694715,  2.57434449,  2.44211124, -5.41013096, -1.26116761,\n",
                         "       -0.90722744,  4.97993729,  2.75554984,  3.49377622,  0.138866  ,\n",
                         "       -3.65445504]),\n",
-                        "    'optimal_value': -1.8567922267701438,\n",
+                        "    'optimal_value': -1.856792226770143,\n",
                         "    'optimizer_evals': None,\n",
-                        "    'optimizer_result': <qiskit.algorithms.optimizers.optimizer.OptimizerResult object at 0x7f674c3e9460>,\n",
-                        "    'optimizer_time': 2.306807518005371}\n"
+                        "    'optimizer_result': <qiskit.algorithms.optimizers.optimizer.OptimizerResult object at 0x7f446dee56d0>,\n",
+                        "    'optimizer_time': 2.1536550521850586}\n"
                     ]
                 }
             ],
             "source": [
                 "print(result)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 15,
+            "execution_count": 13,
             "id": "9030a71b",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def rel_err(target, measured):\n",
-                "    \"\"\"Compute the relative error.\"\"\"\n",
                 "    return abs((target - measured) / target)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 14,
             "id": "66f8c8d8",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -377,35 +359,43 @@
                     ]
                 }
             ],
             "source": [
                 "# Compute the relative error between the expected ground state energy and the VQE's output\n",
                 "rel_error = rel_err(exact_energy, result.eigenvalue)\n",
                 "\n",
-                "print(f\"Expected ground state energy: {exact_energy:.12f}\")\n",
-                "print(f\"Computed ground state energy: {result.eigenvalue:.12f}\")\n",
-                "print(f\"Relative error: {rel_error:.12f}\")"
+                "print(f'Expected ground state energy: {exact_energy:.12f}')\n",
+                "print(f'Computed ground state energy: {result.eigenvalue:.12f}')\n",
+                "print(f'Relative error: {rel_error:.12f}')"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "1208e56f",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3 (ipykernel)",
+            "display_name": "Python (qislacs)",
             "language": "python",
-            "name": "python3"
+            "name": "qislacs"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.0"
+            "version": "3.8.1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `qiskit_qulacs-0.0.0/pyproject.toml` & `qiskit_qulacs-0.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,88 +2,53 @@
 
 [project]
 name = "qiskit_qulacs"
 dynamic = [
     "version",
 ]
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 description = "Qiskit Qulacs to execute Qiskit programs using Qulacs as backend."
 authors = [
    { name = "Gopal Ramesh Dahale", email = "dahalegopal27@gmail.com"},
 ]
-classifiers=[
-    "Intended Audience :: Developers",
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: Apache Software License",
-    "Natural Language :: English",
-    "Operating System :: MacOS",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: Microsoft :: Windows",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
-    "Topic :: Scientific/Engineering :: Physics",
-]
 
 dependencies = [
     "certifi>=2021.5.30",
     "importlib_metadata>=4.8.1",
-    "qiskit-aer>=0.12.2",
-    "qiskit>=1.0.0",
-    "qiskit-algorithms>=0.3.0",
-    "qulacs>=0.5.0",
+    "qiskit-aer>=0.10.3",
+    "qiskit-terra>=0.19.2",
 ]
 
 [project.optional-dependencies]
 # Dev dependencies.
 dev = [
     "coverage>=5.5",
-    "matplotlib>=3.3",
-    "qiskit-nature>=0.7.2",
-    "pyscf>=2.5.0",
-    "pylatexenc>=1.4",
     "pylint>=2.9.5",
     "nbqa>=1.1.1",
     "treon>=0.1.3",
     "pytest>=6.2.5",
     "pytest-randomly>=1.2.0",
     "mypy>=0.780",
     "mypy-extensions>=0.4.3",
     "jupyter-sphinx>=0.3.2",
     "nbsphinx>=0.8.8",
     "sphinx-autodoc-typehints>=1.17.0",
     "reno>=3.5.0",
     # Black's formatting rules can change between major versions, so we use
     # the ~= specifier for it.
     "black[jupyter]~=22.1",
-    "tox==3.24.5",
-    "ddt>=1.2.0,!=1.4.0,!=1.4.3",
-    "myst_parser>=1.0.0",
-    "qiskit-sphinx-theme >=1.14.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Gopal-Dahale/qiskit-qulacs"
 "Bug Tracker" = "https://github.com/Gopal-Dahale/qiskit-qulacs/issues"
-"Documentation" = "https://qiskit-qulacs.netlify.app/"
-"Repository" = "https://github.com/Gopal-Dahale/qiskit-qulacs"
 
 [build-system]
 requires = [
     "setuptools>=61.0",
     "wheel",
     "toml",
     "setuptools-scm",
 ]
 build-backend = "setuptools.build_meta"
-
-[tool.setuptools]
-py-modules = []
-
-[tool.setuptools.packages.find]
-include = ['qiskit_qulacs*']
-exclude = ['qiskit_qulacs*tests']
```

### Comparing `qiskit_qulacs-0.0.0/qiskit_qulacs/qulacs_estimator.py` & `qiskit_qulacs-0.0.1/qiskit_qulacs/qulacs_estimator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,135 +1,117 @@
-"""QulacsEstimator class."""
-
 from __future__ import annotations
 
-import time
 from collections.abc import Sequence
 from typing import Any
+import typing
 
 import numpy as np
+
 from qiskit.circuit import QuantumCircuit
 from qiskit.exceptions import QiskitError
-from qiskit.primitives import Estimator
-from qiskit.primitives.base import EstimatorResult
-from qiskit.primitives.primitive_job import PrimitiveJob
-from qiskit.primitives.utils import _circuit_key, _observable_key, init_observable
-from qiskit.quantum_info import SparsePauliOp
 from qiskit.quantum_info.operators.base_operator import BaseOperator
 
-import qulacs
-from qiskit_qulacs.adapter import (
-    convert_qiskit_to_qulacs_circuit,
-    convert_sparse_pauliop_to_qulacs_obs,
+from qiskit.primitives.base import EstimatorResult
+from qiskit.primitives import Estimator
+from qiskit.primitives.primitive_job import PrimitiveJob
+from qiskit_qulacs.adapter import convert_qiskit_to_qulacs_circuit
+from qiskit_qulacs.adapter import convert_sparse_pauliop_to_qulacs_observable
+from qulacs import QuantumState
+from qiskit.primitives.utils import (
+    _circuit_key,
+    _observable_key,
+    init_observable,
 )
-from qulacs.circuit import QuantumCircuitOptimizer
 
+if typing.TYPE_CHECKING:
+    from qiskit.opflow import PauliSumOp
 
-class QulacsEstimator(Estimator):
-    """QulacsEstimator class."""
 
+class QulacsEstimator(Estimator):
     def __init__(self, *, options: dict | None = None):
         """
         Args:
         options: Default options.
 
         Raises:
-                QiskitError: if some classical bits are not used for measurements.
+            QiskitError: if some classical bits are not used for measurements.
         """
         super().__init__(options=options)
-        self._circuit_ids = {}  # type: ignore
-        self._observable_ids = {}  # type: ignore
-        self._states = ["QuantumState", "QuantumStateGpu"]
-        self.qc_opt = QuantumCircuitOptimizer()
+        self._circuit_ids = {}
+        self._observable_ids = {}
 
     def _call(
         self,
         circuits: Sequence[int],
         observables: Sequence[int],
         parameter_values: Sequence[Sequence[float]],
         **run_options,
     ) -> EstimatorResult:
-        # Initialize metadata
-        gpu = run_options.pop("gpu", False)
-        qco_enable = run_options.pop("qco_enable", False)
-        qco_method = run_options.pop("qco_method", "light")
-        qco_max_block_size = run_options.pop("qco_max_block_size", 2)
 
+        # Initialize metadata
         metadata: list[dict[str, Any]] = [{} for _ in range(len(circuits))]
 
         bound_circuits = []
         for i, value in zip(circuits, parameter_values):
             if len(value) != len(self._parameters[i]):
                 raise QiskitError(
                     f"The number of values ({len(value)}) does not match "
                     f"the number of parameters ({len(self._parameters[i])})."
                 )
 
-            bound_circuits.append(self._circuits[i](np.array(value))[0])
-
-        sorted_obs = [self._observables[i] for i in observables]
-        expectation_values = np.zeros(len(bound_circuits))
-
-        for i, (circ, obs, metadatum) in enumerate(
-            zip(bound_circuits, sorted_obs, metadata)
-        ):
+            bound_circuits.append(self._circuits[i](np.array(value)))
 
-            start = time.time()  # Start timer
-
-            state = getattr(qulacs, self._states[gpu])(circ.get_qubit_count())
-
-            if qco_enable:
-                if qco_method == "light":
-                    self.qc_opt.optimize_light(circ)
-                elif qco_method == "greedy":
-                    self.qc_opt.optimize(circ, qco_max_block_size)
+        sorted_observables = [self._observables[i] for i in observables]
+        expectation_values = []
 
+        for circ, obs, metadatum in zip(bound_circuits, sorted_observables, metadata):
+            state = QuantumState(circ.get_qubit_count())
             circ.update_quantum_state(state)
-            expectation_values[i] = obs.get_expectation_value(state)
-
-            metadatum["time_taken"] = time.time() - start  # End timer
+            expectation_value = obs.get_expectation_value(state)
+            expectation_values.append(expectation_value)
 
         return EstimatorResult(np.real_if_close(expectation_values), metadata)
 
     def _run(
         self,
         circuits: tuple[QuantumCircuit, ...],
-        observables: tuple[BaseOperator | SparsePauliOp, ...],
+        observables: tuple[BaseOperator | PauliSumOp, ...],
         parameter_values: tuple[tuple[float, ...], ...],
         **run_options,
     ):
+
         circuit_indices = []
         for circuit in circuits:
             key = _circuit_key(circuit)
             index = self._circuit_ids.get(key)
             if index is not None:
                 circuit_indices.append(index)
             else:
                 circuit_indices.append(len(self._circuits))
                 self._circuit_ids[key] = len(self._circuits)
-                self._circuits.append(convert_qiskit_to_qulacs_circuit(circuit))
+                self._circuits.append(convert_qiskit_to_qulacs_circuit(circuit)[0])
                 self._parameters.append(circuit.parameters)
 
         observable_indices = []
         for observable in observables:
             observable = init_observable(observable)
             index = self._observable_ids.get(_observable_key(observable))
             if index is not None:
                 observable_indices.append(index)
             else:
                 observable_indices.append(len(self._observables))
                 self._observable_ids[_observable_key(observable)] = len(
                     self._observables
                 )
                 self._observables.append(
-                    convert_sparse_pauliop_to_qulacs_obs(observable)
+                    convert_sparse_pauliop_to_qulacs_observable(observable)
                 )
 
         job = PrimitiveJob(
             self._call,
             circuit_indices,
             observable_indices,
             parameter_values,
             **run_options,
         )
-        job._submit()
+        job.submit()
         return job
```

### Comparing `qiskit_qulacs-0.0.0/qiskit_qulacs/qulacs_estimator_gradient.py` & `qiskit_qulacs-0.0.1/qiskit_qulacs/qulacs_estimator_gradient.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,52 @@
-"""QulacsEstimatorGradient class."""
-
 from __future__ import annotations
 
-import time
+import sys
 from collections.abc import Sequence
-from typing import Any
 
 import numpy as np
-import sympy as sp
+
 from qiskit.circuit import Parameter, QuantumCircuit
-from qiskit.primitives import Estimator
+from qiskit.opflow import PauliSumOp
+from qiskit.primitives import BaseEstimator
 from qiskit.providers import Options
-from qiskit.quantum_info import SparsePauliOp
 from qiskit.quantum_info.operators.base_operator import BaseOperator
-from qiskit_algorithms.gradients import BaseEstimatorGradient
-from qiskit_algorithms.gradients.base.estimator_gradient_result import (
-    EstimatorGradientResult,
-)
-
-from qiskit_qulacs.adapter import (
-    convert_qiskit_to_qulacs_circuit,
-    convert_sparse_pauliop_to_qulacs_obs,
-)
 
+from qiskit.algorithms.gradients import BaseEstimatorGradient
+from qiskit.algorithms.gradients.estimator_gradient_result import EstimatorGradientResult
+from qiskit_qulacs.adapter import convert_qiskit_to_qulacs_circuit, convert_sparse_pauliop_to_qulacs_observable
+from qiskit.algorithms.exceptions import AlgorithmError
 
 class QulacsEstimatorGradient(BaseEstimatorGradient):
-    """QulacsEstimatorGradient class."""
-
     def __init__(
         self,
+        estimator: BaseEstimator,
         options: Options | None = None,
     ):
-        # this is required by the base class, but not used
-        dummy_estimator = Estimator()
-        super().__init__(dummy_estimator, options)
+        super().__init__(estimator, options)
 
     def _run(
         self,
         circuits: Sequence[QuantumCircuit],
-        observables: Sequence[BaseOperator | SparsePauliOp],
+        observables: Sequence[BaseOperator | PauliSumOp],
         parameter_values: Sequence[Sequence[float]],
         parameters: Sequence[Sequence[Parameter]],
         **options,
     ) -> EstimatorGradientResult:
         """Compute the estimator gradients on the given circuits."""
 
         gradients = []
-        metadata: list[dict[str, Any]] = [{} for _ in range(len(circuits))]
-
-        for circuit, observable, parameter_values_, parameters_, metadatum in zip(
-            circuits, observables, parameter_values, parameters, metadata
+        for circuit, observable, parameter_values_, parameters_ in zip(
+            circuits, observables, parameter_values, parameters
         ):
+            qulacs_circuit, metadata = convert_qiskit_to_qulacs_circuit(circuit)
+            parameter_mapping = metadata['paramater_mapping']
+            gradient = np.negative(qulacs_circuit(parameter_values_).backprop(convert_sparse_pauliop_to_qulacs_observable(observable)))
 
-            qulacs_circuit = convert_qiskit_to_qulacs_circuit(circuit)
-            qulacs_obs = convert_sparse_pauliop_to_qulacs_obs(observable)
-
-            start = time.time()  # Start timer
-
-            params_values = np.array(parameter_values_)
-            circ, metadata = qulacs_circuit(params_values)
-            parameter_mapping = metadata["parameter_mapping"]  # type: ignore
-            parameter_exprs = metadata["parameter_exprs"]  # type: ignore
-
-            # Compute gradient using qulacs
-            # `np.negative` is used because the gradients computed
-            # differ by minus sign
-            gradient = np.negative(circ.backprop(qulacs_obs))
-
-            # Evaluate the parameter expressions differentiation and
-            # multiply it by the gradient to take into account the
-            # expression's differentiation
-            for i, idx in enumerate(parameter_mapping):
-                f_params, f_expr = parameter_exprs[i]
-                f = sp.lambdify(f_params, sp.diff(f_expr))
-                gradient[i] = f(params_values[idx]) * gradient[i]
-
-            # The ordering of parameters is changed during circuit conversion.
-            # `parameter_mapping` holds this mapping
-
-            # Permute the obtained gradients to match with qiskit's ordering
-            gradient[parameter_mapping] = gradient[range(len(parameter_mapping))]
+            gradient[parameter_mapping] = gradient[np.arange(len(parameter_mapping))]
 
             # Indices of parameters to be differentiated
             indices = [circuit.parameters.data.index(p) for p in parameters_]
             gradients.append(gradient[indices])
 
-            metadatum["time_taken"] = time.time() - start  # End timer
-
         opt = self._get_local_options(options)
-        return EstimatorGradientResult(
-            gradients=gradients, metadata=metadata, options=opt
-        )
+        return EstimatorGradientResult(gradients=gradients, metadata={}, options=opt)
```

### Comparing `qiskit_qulacs-0.0.0/qiskit_qulacs/qulacs_provider.py` & `qiskit_qulacs-0.0.1/qiskit_qulacs/qulacs_provider.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-"""QulacsProvider class."""
 from qiskit.providers import ProviderV1 as Provider
 from qiskit.providers.providerutils import filter_backends
 
 from .qulacs_backend import QulacsBackend
 
-
 class QulacsProvider(Provider):
-    """QulacsProvider class."""
-
-    @staticmethod
-    def _get_backends():
-        return [("qulacs_simulator", QulacsBackend)]
-
-    def get_backend(self, name=None, **kwargs):
-        return super().get_backend(name=name, **kwargs)
+    def __init__(self, token=None):
+        super().__init__()
+        self.token = token
 
     def backends(self, name=None, filters=None, **kwargs):
-        backends = []
-        for backend_name, backend_cls in self._get_backends():
-            if name is None or backend_name == name:
-                backends.append(backend_cls(provider=self))
-        return filter_backends(backends, filters=filters, **kwargs)
+        backends = [QulacsBackend()]
+
+        if name:
+            backends = [
+                backend for backend in backends if backend.name == name]
 
-    def __str__(self):
-        return "QulacsProvider"
+        return filter_backends(backends, filters=filters, **kwargs)
```

### Comparing `qiskit_qulacs-0.0.0/qiskit_qulacs.egg-info/PKG-INFO` & `qiskit_qulacs-0.0.1/qiskit_qulacs.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qiskit_qulacs
-Version: 0.0.0
+Name: qiskit-qulacs
+Version: 0.0.1
 Summary: Qiskit Qulacs to execute Qiskit programs using Qulacs as backend.
 Author-email: Gopal Ramesh Dahale <dahalegopal27@gmail.com>
 License:                     Copyright 2021 IBM and its contributors
         
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -205,82 +205,52 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/Gopal-Dahale/qiskit-qulacs
 Project-URL: Bug Tracker, https://github.com/Gopal-Dahale/qiskit-qulacs/issues
-Project-URL: Documentation, https://qiskit-qulacs.netlify.app/
-Project-URL: Repository, https://github.com/Gopal-Dahale/qiskit-qulacs
+Keywords: qiskit qulacs quantum
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: certifi>=2021.5.30
-Requires-Dist: importlib_metadata>=4.8.1
-Requires-Dist: qiskit-aer>=0.12.2
-Requires-Dist: qiskit>=1.0.0
-Requires-Dist: qiskit-algorithms>=0.3.0
-Requires-Dist: qulacs>=0.5.0
 Provides-Extra: dev
-Requires-Dist: coverage>=5.5; extra == "dev"
-Requires-Dist: matplotlib>=3.3; extra == "dev"
-Requires-Dist: qiskit-nature>=0.7.2; extra == "dev"
-Requires-Dist: pyscf>=2.5.0; extra == "dev"
-Requires-Dist: pylatexenc>=1.4; extra == "dev"
-Requires-Dist: pylint>=2.9.5; extra == "dev"
-Requires-Dist: nbqa>=1.1.1; extra == "dev"
-Requires-Dist: treon>=0.1.3; extra == "dev"
-Requires-Dist: pytest>=6.2.5; extra == "dev"
-Requires-Dist: pytest-randomly>=1.2.0; extra == "dev"
-Requires-Dist: mypy>=0.780; extra == "dev"
-Requires-Dist: mypy-extensions>=0.4.3; extra == "dev"
-Requires-Dist: jupyter-sphinx>=0.3.2; extra == "dev"
-Requires-Dist: nbsphinx>=0.8.8; extra == "dev"
-Requires-Dist: sphinx-autodoc-typehints>=1.17.0; extra == "dev"
-Requires-Dist: reno>=3.5.0; extra == "dev"
-Requires-Dist: black[jupyter]~=22.1; extra == "dev"
-Requires-Dist: tox==3.24.5; extra == "dev"
-Requires-Dist: ddt!=1.4.0,!=1.4.3,>=1.2.0; extra == "dev"
-Requires-Dist: myst_parser>=1.0.0; extra == "dev"
-Requires-Dist: qiskit-sphinx-theme>=1.14.0; extra == "dev"
-
-![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS-informational)
-[![Python](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-informational)](https://www.python.org/)
-[![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%201.0.0-6133BD)](https://github.com/Qiskit/qiskit)
+License-File: LICENSE.txt
+
+![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20macOS%20%7C%20Windows-informational)
+[![Python](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10-informational)](https://www.python.org/)
+[![Qiskit](https://img.shields.io/badge/Qiskit-%E2%89%A5%200.34.2-6133BD)](https://github.com/Qiskit/qiskit)
 [![License](https://img.shields.io/github/license/qiskit-community/quantum-prototype-template?label=License)](https://github.com/qiskit-community/quantum-prototype-template/blob/main/LICENSE.txt)
 [![Code style: Black](https://img.shields.io/badge/Code%20style-Black-000.svg)](https://github.com/psf/black)
-[![PyPI version](https://badge.fury.io/py/qiskit-qulacs.svg)](https://badge.fury.io/py/qiskit-qulacs)
-[![Tests](https://github.com/Gopal-Dahale/qiskit-qulacs/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/Gopal-Dahale/qiskit-qulacs/actions/workflows/test_latest_versions.yml)
-[![Coverage Status](https://coveralls.io/repos/github/Gopal-Dahale/qiskit-qulacs/badge.svg?branch=main)](https://coveralls.io/github/Gopal-Dahale/qiskit-qulacs?branch=main)
+<!-- [![Tests](https://github.com/qiskit-community/quantum-prototype-template/actions/workflows/test_latest_versions.yml/badge.svg)](https://github.com/qiskit-community/quantum-prototype-template/actions/workflows/test_latest_versions.yml)
+[![Coverage](https://coveralls.io/repos/github/qiskit-community/quantum-prototype-template/badge.svg?branch=main)](https://coveralls.io/github/qiskit-community/quantum-prototype-template?branch=main) -->
 
-![Qiskit-Qulacs-logo-extended](https://github.com/Gopal-Dahale/qiskit-qulacs/assets/49199003/27116cba-4109-4298-baac-0a35d04c5ab5)
+![Qiskit-Qulacs](docs/_static/images/logo_extended.png)
 
-Qiskit-Qulacs allows users to execute Qiskit programs using Qulacs backend.
+Qiskit-Qulacs allows user to execute Qiskit programs using Qulacs backend.
 
-**Qiskit-Qulacs is actively being developed, and we welcome your input and suggestions on the API and use cases. If you have any ideas or feedback, please open a GitHub issue or contact us. We are interested in hearing about your experiences using the library.**
+**Qiskit-Qulacs is actively being developed, and we welcome your input and suggestions on the API and use-cases. If you have any ideas or feedback, please feel free to open a GitHub issue or contact us. We are interested in hearing about your experiences using the library.**
 
 
-1.  [About](docs/intro/project_overview.md)
-2.  [Beginner's Guide](docs/intro/beginners_guide.md)
-3.  [Installation](docs/intro/INSTALL.md)
-4.  [Quickstart Guide](docs/intro/quickstart_guide.md)
+
+1.  [About](docs/project_overview.md)
+2.  [Beginner's Guide](docs/beginners_guide.md)
+3.  [Installation](INSTALL.md)
+4.  [Quickstart Guide](docs/quickstart_guide.md)
 5.  [Tutorials](docs/tutorials/)
 6.  [How-Tos](docs/how_tos/)
 8.  [How to Give Feedback](#how-to-give-feedback)
 9.  [Contribution Guidelines](#contribution-guidelines)
 10. [References and Acknowledgements](#references-and-acknowledgements)
 11. [License](#license)
 
@@ -298,25 +268,22 @@
 - [Opening an issue](https://github.com/Gopal-Dahale/qiskit-qulacs/issues) in the repository
 
 
 ----------------------------------------------------------------------------------------------------
 
 ### Contribution Guidelines
 
-For information on contributing to this project, please take a look at our [contribution guidelines](CONTRIBUTING.md).
+For information on how to contribute to this project, please take a look at our [contribution guidelines](CONTRIBUTING.md).
 
 
 ----------------------------------------------------------------------------------------------------
 
 ## References and Acknowledgements
 [1] Qiskit https://qiskit.org/ \
 [2] Qiskit-terra https://github.com/Qiskit/qiskit-terra \
 [3] Qulacs https://github.com/qulacs/qulacs
 
-We are proud to be supported by the [Unitary Fund microgrant program](https://unitary.fund/grants/). Thank you Unitary Fund.
-
-[![Unitary Fund](https://img.shields.io/badge/Supported%20By-UNITARY%20FUND-brightgreen.svg?style=for-the-badge)](https://unitary.fund)
 
 ----------------------------------------------------------------------------------------------------
 
 ### License
 [Apache License 2.0](LICENSE.txt)
```

### Comparing `qiskit_qulacs-0.0.0/tests/README.md` & `qiskit_qulacs-0.0.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_qulacs-0.0.0/tox.ini` & `qiskit_qulacs-0.0.1/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 [tox]
 minversion = 2.1
-envlist = py38, py39, py310, py311, py312, lint, coverage, docs
-skipsdist = true
+envlist = py37, py38, py39, py310, lint, coverage
+# CI: skip-next-line
+skip_missing_interpreters = true
 
 [testenv]
+# CI: skip-next-line
 usedevelop = true
 install_command = pip install -U {opts} {packages}
 setenv =
-	VIRTUAL_ENV={envdir}
-	LANGUAGE=en_US
-	LC_ALL=en_US.utf-8
-deps = -rrequirements.txt
-	   -rrequirements-dev.txt
+  VIRTUAL_ENV={envdir}
+  LANGUAGE=en_US
+  LC_ALL=en_US.utf-8
+extras = dev
 commands =
-	pip check
-	python -m pytest tests -v --doctest-modules
+  pip check
+  python -m pytest -v --doctest-modules
+  treon docs --threads 2
 
 [testenv:lint]
 envdir = .tox/lint
+extras = dev
 commands =
-	black --check .
-	pylint -rn --fail-under=9 qiskit_qulacs tests
-	mypy --install-types --non-interactive qiskit_qulacs tests docs --exclude docs/_build
+  black --check .
+  pylint -rn prototype_template tests
+  nbqa pylint -rn docs/
+  mypy .
+
+[testenv:black]
+envdir = .tox/lint
+skip_install = true
+commands = black .
 
 [testenv:coverage]
 basepython = python3
 setenv =
-	{[testenv]setenv}
+  {[testenv]setenv}
 commands =
-	coverage3 run --source qiskit_qulacs --parallel-mode -m pytest tests --doctest-modules
-	coverage3 combine
-	coverage3 report --fail-under=80
+  coverage3 run --source prototype_template --parallel-mode -m pytest --doctest-modules
+  coverage3 combine
+  coverage3 report --fail-under=80
 
 [testenv:docs]
-deps =
-    -r{toxinidir}/requirements-dev.txt
-    .
+skip_install = false
+extras = dev
+commands =
+  sphinx-build -b html -W -T --keep-going {posargs} docs/ docs/_build/html
+
+[testenv:ecosystem]
+allowlist_externals = /bin/bash
 commands =
-	sphinx-build -b html {posargs} docs/ docs/_build/html
+  /bin/bash -ec 'cat ecosystem.json | jq empty'
```

