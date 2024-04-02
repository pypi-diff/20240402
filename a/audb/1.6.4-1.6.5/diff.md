# Comparing `tmp/audb-1.6.4.tar.gz` & `tmp/audb-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audb-1.6.4.tar", last modified: Fri Feb 23 13:20:30 2024, max compression
+gzip compressed data, was "audb-1.6.5.tar", last modified: Tue Apr  2 07:03:29 2024, max compression
```

## Comparing `audb-1.6.4.tar` & `audb-1.6.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.953601 audb-1.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.937601 audb-1.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.941601 audb-1.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-02-23 13:20:22.000000 audb-1.6.4/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-02-23 13:20:22.000000 audb-1.6.4/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-02-23 13:20:22.000000 audb-1.6.4/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-23 13:20:22.000000 audb-1.6.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-23 13:20:22.000000 audb-1.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-23 13:20:22.000000 audb-1.6.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13836 2024-02-23 13:20:22.000000 audb-1.6.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-23 13:20:22.000000 audb-1.6.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-23 13:20:22.000000 audb-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-02-23 13:20:30.953601 audb-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-02-23 13:20:22.000000 audb-1.6.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.941601 audb-1.6.4/audb/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-23 13:20:22.000000 audb-1.6.4/audb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.945601 audb-1.6.4/audb/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/define.py
--rw-r--r--   0 runner    (1001) docker     (127)    17005 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.945601 audb-1.6.4/audb/core/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/etc/audb.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    48691 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/load_to.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    26391 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-02-23 13:20:22.000000 audb-1.6.4/audb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.945601 audb-1.6.4/audb/info/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-02-23 13:20:22.000000 audb-1.6.4/audb/info/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.953601 audb-1.6.4/audb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-02-23 13:20:30.000000 audb-1.6.4/audb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-02-23 13:20:30.000000 audb-1.6.4/audb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 13:20:30.000000 audb-1.6.4/audb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-23 13:20:30.000000 audb-1.6.4/audb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-23 13:20:30.000000 audb-1.6.4/audb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.945601 audb-1.6.4/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     9361 2024-02-23 13:20:22.000000 audb-1.6.4/benchmarks/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-02-23 13:20:22.000000 audb-1.6.4/benchmarks/benchmark-dependencies-methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    15770 2024-02-23 13:20:22.000000 audb-1.6.4/benchmarks/benchmark-dependencies-save-and-load.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-23 13:20:22.000000 audb-1.6.4/benchmarks/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.949601 audb-1.6.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.949601 audb-1.6.4/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-23 13:20:22.000000 audb-1.6.4/docs/api-src/audb.info.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-23 13:20:22.000000 audb-1.6.4/docs/api-src/audb.rst
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-23 13:20:22.000000 audb-1.6.4/docs/authentication.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-02-23 13:20:22.000000 audb-1.6.4/docs/caching.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-23 13:20:22.000000 audb-1.6.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-02-23 13:20:22.000000 audb-1.6.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-23 13:20:22.000000 audb-1.6.4/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-23 13:20:22.000000 audb-1.6.4/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-23 13:20:22.000000 audb-1.6.4/docs/dependencies.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-23 13:20:22.000000 audb-1.6.4/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-23 13:20:22.000000 audb-1.6.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-02-23 13:20:22.000000 audb-1.6.4/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-02-23 13:20:22.000000 audb-1.6.4/docs/load.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-23 13:20:22.000000 audb-1.6.4/docs/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.949601 audb-1.6.4/docs/pics/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-23 13:20:22.000000 audb-1.6.4/docs/pics/load.dot
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-23 13:20:22.000000 audb-1.6.4/docs/pics/publish.dot
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-02-23 13:20:22.000000 audb-1.6.4/docs/publish.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-02-23 13:20:22.000000 audb-1.6.4/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-23 13:20:22.000000 audb-1.6.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-02-23 13:20:22.000000 audb-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-23 13:20:22.000000 audb-1.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 13:20:30.953601 audb-1.6.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 13:20:30.953601 audb-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-02-23 13:20:22.000000 audb-1.6.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-23 13:20:22.000000 audb-1.6.4/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    22462 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_load_on_demand.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_lock_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    42307 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-02-23 13:20:22.000000 audb-1.6.4/tests/test_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.905200 audb-1.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.893200 audb-1.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.897200 audb-1.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-02 07:03:23.000000 audb-1.6.5/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-02 07:03:23.000000 audb-1.6.5/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-02 07:03:23.000000 audb-1.6.5/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-02 07:03:23.000000 audb-1.6.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 07:03:23.000000 audb-1.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 07:03:23.000000 audb-1.6.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14059 2024-04-02 07:03:23.000000 audb-1.6.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-02 07:03:23.000000 audb-1.6.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-02 07:03:23.000000 audb-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-02 07:03:29.905200 audb-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-02 07:03:23.000000 audb-1.6.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.897200 audb-1.6.5/audb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-02 07:03:23.000000 audb-1.6.5/audb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.901200 audb-1.6.5/audb/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/define.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.901200 audb-1.6.5/audb/core/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/etc/audb.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48691 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/load_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26391 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-02 07:03:23.000000 audb-1.6.5/audb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.901200 audb-1.6.5/audb/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-02 07:03:23.000000 audb-1.6.5/audb/info/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.905200 audb-1.6.5/audb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-02 07:03:29.000000 audb-1.6.5/audb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-02 07:03:29.000000 audb-1.6.5/audb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:03:29.000000 audb-1.6.5/audb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 07:03:29.000000 audb-1.6.5/audb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 07:03:29.000000 audb-1.6.5/audb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.901200 audb-1.6.5/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9361 2024-04-02 07:03:23.000000 audb-1.6.5/benchmarks/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-04-02 07:03:23.000000 audb-1.6.5/benchmarks/benchmark-dependencies-methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15770 2024-04-02 07:03:23.000000 audb-1.6.5/benchmarks/benchmark-dependencies-save-and-load.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 07:03:23.000000 audb-1.6.5/benchmarks/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.901200 audb-1.6.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.901200 audb-1.6.5/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-02 07:03:23.000000 audb-1.6.5/docs/api-src/audb.info.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-02 07:03:23.000000 audb-1.6.5/docs/api-src/audb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 07:03:23.000000 audb-1.6.5/docs/authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-02 07:03:23.000000 audb-1.6.5/docs/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-02 07:03:23.000000 audb-1.6.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-02 07:03:23.000000 audb-1.6.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 07:03:23.000000 audb-1.6.5/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 07:03:23.000000 audb-1.6.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-02 07:03:23.000000 audb-1.6.5/docs/dependencies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 07:03:23.000000 audb-1.6.5/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-02 07:03:23.000000 audb-1.6.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-02 07:03:23.000000 audb-1.6.5/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-02 07:03:23.000000 audb-1.6.5/docs/load.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-02 07:03:23.000000 audb-1.6.5/docs/overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.905200 audb-1.6.5/docs/pics/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 07:03:23.000000 audb-1.6.5/docs/pics/load.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 07:03:23.000000 audb-1.6.5/docs/pics/publish.dot
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-02 07:03:23.000000 audb-1.6.5/docs/publish.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-02 07:03:23.000000 audb-1.6.5/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 07:03:23.000000 audb-1.6.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-04-02 07:03:23.000000 audb-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-02 07:03:23.000000 audb-1.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:03:29.905200 audb-1.6.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:03:29.905200 audb-1.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-04-02 07:03:23.000000 audb-1.6.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 07:03:23.000000 audb-1.6.5/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22462 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_load_on_demand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_lock_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42307 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-02 07:03:23.000000 audb-1.6.5/tests/test_remove.py
```

### Comparing `audb-1.6.4/.github/workflows/doc.yml` & `audb-1.6.5/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/.github/workflows/linter.yml` & `audb-1.6.5/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/.github/workflows/publish.yml` & `audb-1.6.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/.github/workflows/test.yml` & `audb-1.6.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/.pre-commit-config.yaml` & `audb-1.6.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/CHANGELOG.rst` & `audb-1.6.5/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.6.5 (2024-03-28)
+--------------------------
+
+* Added: ``audb.Dependencies.__eq__()``
+  to compare two dependency tables
+* Fixed: let ``audb.available()``
+  skip incomplete datasets
+  instead of raising an error
+
+
 Version 1.6.4 (2024-02-23)
 --------------------------
 
 * Fixed: in ``audb.publish()``
   updating of multi-file archives
   that have been published
   before the version
```

### Comparing `audb-1.6.4/CONTRIBUTING.rst` & `audb-1.6.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/LICENSE` & `audb-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/PKG-INFO` & `audb-1.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audb
-Version: 1.6.4
+Version: 1.6.5
 Summary: Load and publish databases in audformat
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>
 License: MIT License
         
         Copyright (c) 2018-present audEERING GmbH and Contributors
         
         Authors:
```

### Comparing `audb-1.6.4/README.rst` & `audb-1.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/__init__.py` & `audb-1.6.5/audb/__init__.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/api.py` & `audb-1.6.5/audb/core/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,24 +47,29 @@
             backend = utils.access_backend(repository)
             if isinstance(backend, audbackend.Artifactory):
                 # avoid backend.ls('/')
                 # which is very slow on Artifactory
                 # see https://github.com/audeering/audbackend/issues/132
                 for p in backend._repo.path:
                     name = p.name
-                    for version in [str(x).split("/")[-1] for x in p / "db"]:
-                        databases.append(
-                            [
-                                name,
-                                repository.backend,
-                                repository.host,
-                                repository.name,
-                                version,
-                            ]
-                        )
+                    try:
+                        for version in [str(x).split("/")[-1] for x in p / "db"]:
+                            databases.append(
+                                [
+                                    name,
+                                    repository.backend,
+                                    repository.host,
+                                    repository.name,
+                                    version,
+                                ]
+                            )
+                    except FileNotFoundError:
+                        # If the `db` folder does not exist,
+                        # we do not include the dataset
+                        pass
             else:
                 for path, version in backend.ls("/"):
                     if path.endswith(define.HEADER_FILE):
                         name = path.split("/")[1]
                         databases.append(
                             [
                                 name,
```

### Comparing `audb-1.6.4/audb/core/cache.py` & `audb-1.6.5/audb/core/cache.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/config.py` & `audb-1.6.5/audb/core/config.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/conftest.py` & `audb-1.6.5/audb/core/conftest.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/define.py` & `audb-1.6.5/audb/core/define.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/dependencies.py` & `audb-1.6.5/audb/core/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,26 @@
 
         Returns:
             ``True`` if a dependency to the file exists
 
         """
         return file in self._df.index
 
+    def __eq__(self, other: "Dependencies") -> bool:
+        r"""Check if two dependency tables are equal.
+
+        Args:
+            other: dependency table to compare against
+
+        Returns:
+            ``True`` if both dependency tables have the same entries
+
+        """
+        return self._df.equals(other._df)
+
     def __getitem__(self, file: str) -> typing.List:
         r"""File information.
 
         Args:
             file: relative file path
 
         Returns:
```

### Comparing `audb-1.6.4/audb/core/flavor.py` & `audb-1.6.5/audb/core/flavor.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/info.py` & `audb-1.6.5/audb/core/info.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/load.py` & `audb-1.6.5/audb/core/load.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/load_to.py` & `audb-1.6.5/audb/core/load_to.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/lock.py` & `audb-1.6.5/audb/core/lock.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/publish.py` & `audb-1.6.5/audb/core/publish.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/core/utils.py` & `audb-1.6.5/audb/core/utils.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb/info/__init__.py` & `audb-1.6.5/audb/info/__init__.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/audb.egg-info/PKG-INFO` & `audb-1.6.5/audb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audb
-Version: 1.6.4
+Version: 1.6.5
 Summary: Load and publish databases in audformat
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Johannes Wagner <jwagner@audeering.com>
 License: MIT License
         
         Copyright (c) 2018-present audEERING GmbH and Contributors
         
         Authors:
```

### Comparing `audb-1.6.4/audb.egg-info/SOURCES.txt` & `audb-1.6.5/audb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/benchmarks/README.md` & `audb-1.6.5/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/benchmarks/benchmark-dependencies-methods.py` & `audb-1.6.5/benchmarks/benchmark-dependencies-methods.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/benchmarks/benchmark-dependencies-save-and-load.py` & `audb-1.6.5/benchmarks/benchmark-dependencies-save-and-load.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/api-src/audb.info.rst` & `audb-1.6.5/docs/api-src/audb.info.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/caching.rst` & `audb-1.6.5/docs/caching.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/conf.py` & `audb-1.6.5/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "pandas",
 ]
 graphviz_output_format = "svg"
 
 apipages_hidden_methods = [
     "__call__",
     "__contains__",
+    "__eq__",
     "__getitem__",
     "__len__",
 ]
 
 # HTML --------------------------------------------------------------------
 html_theme = "sphinx_audeering_theme"
 html_theme_options = {
```

### Comparing `audb-1.6.4/docs/configuration.rst` & `audb-1.6.5/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/dependencies.rst` & `audb-1.6.5/docs/dependencies.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/index.rst` & `audb-1.6.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/install.rst` & `audb-1.6.5/docs/install.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/load.rst` & `audb-1.6.5/docs/load.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/overview.rst` & `audb-1.6.5/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/pics/load.dot` & `audb-1.6.5/docs/pics/load.dot`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/pics/publish.dot` & `audb-1.6.5/docs/pics/publish.dot`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/publish.rst` & `audb-1.6.5/docs/publish.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/docs/quickstart.rst` & `audb-1.6.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/pyproject.toml` & `audb-1.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/conftest.py` & `audb-1.6.5/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,26 +178,28 @@
 @pytest.fixture(scope="module", autouse=False)
 def private_and_public_repository():
     r"""Private and public repository on Artifactory.
 
     Configure the following repositories:
     * data-private: repo on public Artifactory without access
     * data-public: repo on public Artifactory with anonymous access
+    * data-public2: repo on public Artifactory with anonymous access
 
     Note, that the order of the repos is important.
     audb will visit the repos in the given order
     until it finds the requested database.
 
     """
     host = "https://audeering.jfrog.io/artifactory"
     backend = "artifactory"
     current_repositories = audb.config.REPOSITORIES
     audb.config.REPOSITORIES = [
         audb.Repository("data-private", host, backend),
         audb.Repository("data-public", host, backend),
+        audb.Repository("data-public2", host, backend),
     ]
 
     yield repository
 
     audb.config.REPOSITORIES = current_repositories
```

### Comparing `audb-1.6.4/tests/test_backend.py` & `audb-1.6.5/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_cache.py` & `audb-1.6.5/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_config.py` & `audb-1.6.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_convert.py` & `audb-1.6.5/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_dependencies.py` & `audb-1.6.5/tests/test_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,30 @@
 
 def test_contains(deps):
     assert "db.files.csv" in deps
     assert "file.wav" in deps
     assert "not.csv" not in deps
 
 
+def test_equals(deps):
+    # empty table vs. empty table
+    _deps = audb.Dependencies()
+    assert _deps == _deps
+    assert _deps == audb.Dependencies()
+    # empty table vs. example table
+    assert deps != audb.Dependencies()
+    # example table vs. example table
+    assert deps == deps
+    _deps._df = deps._df.copy()
+    assert deps == _deps
+    # example table vs. different table
+    _deps._df.loc["db.files.csv", "channels"] = 4
+    assert deps != _deps
+
+
 def test_get_item(deps):
     assert deps["db.files.csv"] == list(ROWS[0].values())[1:]
     assert deps["file.wav"] == list(ROWS[1].values())[1:]
     with pytest.raises(KeyError, match="non.existing"):
         deps["non.existing"]
```

### Comparing `audb-1.6.4/tests/test_filter.py` & `audb-1.6.5/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_flavor.py` & `audb-1.6.5/tests/test_flavor.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_info.py` & `audb-1.6.5/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_load.py` & `audb-1.6.5/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_load_on_demand.py` & `audb-1.6.5/tests/test_load_on_demand.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_lock.py` & `audb-1.6.5/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_lock_db.py` & `audb-1.6.5/tests/test_lock_db.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_publish.py` & `audb-1.6.5/tests/test_publish.py`

 * *Files identical despite different names*

### Comparing `audb-1.6.4/tests/test_remove.py` & `audb-1.6.5/tests/test_remove.py`

 * *Files identical despite different names*

