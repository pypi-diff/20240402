# Comparing `tmp/swh.objstorage-2.9.1.tar.gz` & `tmp/swh.objstorage-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.objstorage-2.9.1.tar", last modified: Mon Mar 25 15:50:15 2024, max compression
+gzip compressed data, was "swh.objstorage-2.9.2.tar", last modified: Tue Apr  2 15:01:08 2024, max compression
```

## Comparing `swh.objstorage-2.9.1.tar` & `swh.objstorage-2.9.2.tar`

### file list

```diff
@@ -1,139 +1,141 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.567144 swh.objstorage-2.9.1/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1095 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4448 2024-03-25 15:50:15.567144 swh.objstorage-2.9.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.531144 swh.objstorage-2.9.1/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/bin/swh-objstorage-azure
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.535144 swh.objstorage-2.9.1/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.535144 swh.objstorage-2.9.1/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.535144 swh.objstorage-2.9.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/docs/winery.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2000 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      130 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/requirements-azure.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/requirements-libcloud.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      165 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/requirements-winery.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      297 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-03-25 15:50:15.567144 swh.objstorage-2.9.1/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.523144 swh.objstorage-2.9.1/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.539144 swh.objstorage-2.9.1/swh/objstorage/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.539144 swh.objstorage-2.9.1/swh/objstorage/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1915 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4975 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/api/server.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.539144 swh.objstorage-2.9.1/swh/objstorage/backends/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18057 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5150 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3638 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2163 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9287 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/libcloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12594 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/pathslicing.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.543144 swh.objstorage-2.9.1/swh/objstorage/backends/seaweedfs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/seaweedfs/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/seaweedfs/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5731 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/seaweedfs/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.543144 swh.objstorage-2.9.1/swh/objstorage/backends/winery/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       55 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/winery/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8317 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/winery/database.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14830 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/winery/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14565 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/winery/roshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3283 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/winery/rwshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18323 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/winery/sharedbase.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/winery/sleep.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/winery/stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7079 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/backends/winery/throttler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12577 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      547 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/constants.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1184 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2970 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/factory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8530 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/interface.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.547144 swh.objstorage-2.9.1/swh/objstorage/multiplexer/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      121 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/multiplexer/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.547144 swh.objstorage-2.9.1/swh/objstorage/multiplexer/filter/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2617 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/multiplexer/filter/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2721 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/multiplexer/filter/filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      785 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/multiplexer/filter/read_write_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10697 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/multiplexer/multiplexer_objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4838 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)      956 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.551144 swh.objstorage-2.9.1/swh/objstorage/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13333 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/objstorage_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_api.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12746 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7159 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_cloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4609 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_instantiation.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2322 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_multiplexer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5377 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_pathslicing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_random_generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10331 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_seaweedfs.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    38507 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_winery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_pathslicer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2928 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_readonly_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20137 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/winery_benchmark.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6707 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/tests/winery_testing_helpers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      541 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/swh/objstorage/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.559144 swh.objstorage-2.9.1/swh.objstorage.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4448 2024-03-25 15:50:15.000000 swh.objstorage-2.9.1/swh.objstorage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4049 2024-03-25 15:50:15.000000 swh.objstorage-2.9.1/swh.objstorage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-03-25 15:50:15.000000 swh.objstorage-2.9.1/swh.objstorage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-03-25 15:50:15.000000 swh.objstorage-2.9.1/swh.objstorage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      471 2024-03-25 15:50:15.000000 swh.objstorage-2.9.1/swh.objstorage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-03-25 15:50:15.000000 swh.objstorage-2.9.1/swh.objstorage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1560 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/tox.ini
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.559144 swh.objstorage-2.9.1/winery-test-environment/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/README.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/ansible.cfg
--rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/bootstrap.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/build-vms.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/ceph.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/fed4fire.rspec
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/fed4fire.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/grid5000.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.559144 swh.objstorage-2.9.1/winery-test-environment/inventory/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.523144 swh.objstorage-2.9.1/winery-test-environment/inventory/group_vars/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.559144 swh.objstorage-2.9.1/winery-test-environment/inventory/group_vars/all/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/inventory/group_vars/all/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/inventory/groups.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/inventory/hosts.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/inventory/osd.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/libvirt.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:15.559144 swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/README.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/mitogen.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/mitogen_free.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/mitogen_linear.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/osd.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/remote-tox.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/render-stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/rng.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-03-25 15:50:08.000000 swh.objstorage-2.9.1/winery-test-environment/tests.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.754988 swh.objstorage-2.9.2/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/bin/swh-objstorage-azure
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.754988 swh.objstorage-2.9.2/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.754988 swh.objstorage-2.9.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.754988 swh.objstorage-2.9.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/docs/winery.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-azure.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-libcloud.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements-winery.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      297 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.746988 swh.objstorage-2.9.2/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.758988 swh.objstorage-2.9.2/swh/objstorage/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.758988 swh.objstorage-2.9.2/swh/objstorage/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1974 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5013 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/api/server.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.758988 swh.objstorage-2.9.2/swh/objstorage/backends/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17381 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5150 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1780 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8283 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/libcloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11190 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/pathslicing.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.762988 swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4925 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.762988 swh.objstorage-2.9.2/swh/objstorage/backends/winery/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       55 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8317 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/database.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14679 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14565 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/roshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3283 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/rwshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18323 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/sharedbase.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/sleep.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7079 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/backends/winery/throttler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12577 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      547 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/constants.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1466 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2970 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/factory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8544 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/interface.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.762988 swh.objstorage-2.9.2/swh/objstorage/multiplexer/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      121 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.762988 swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2617 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2721 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      785 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/read_write_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10925 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/multiplexer/multiplexer_objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7416 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      956 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.766988 swh.objstorage-2.9.2/swh/objstorage/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13564 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/objstorage_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_api.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7083 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_cloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4694 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_instantiation.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2322 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_multiplexer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5672 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_pathslicing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_random_generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_seaweedfs.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    38512 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_winery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_pathslicer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2952 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_readonly_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20137 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/winery_benchmark.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6707 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/tests/winery_testing_helpers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      541 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/swh/objstorage/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/swh.objstorage.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4453 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4097 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      476 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-02 15:01:08.000000 swh.objstorage-2.9.2/swh.objstorage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.770988 swh.objstorage-2.9.2/winery-test-environment/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/README.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/ansible.cfg
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/bootstrap.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/build-vms.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/ceph.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/fed4fire.rspec
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/fed4fire.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/grid5000.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.770988 swh.objstorage-2.9.2/winery-test-environment/inventory/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.750988 swh.objstorage-2.9.2/winery-test-environment/inventory/group_vars/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.770988 swh.objstorage-2.9.2/winery-test-environment/inventory/group_vars/all/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/inventory/group_vars/all/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/inventory/groups.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/inventory/hosts.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/inventory/osd.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/libvirt.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:08.774988 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/README.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_free.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_linear.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/osd.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/remote-tox.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/render-stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/rng.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-04-02 15:01:04.000000 swh.objstorage-2.9.2/winery-test-environment/tests.yml
```

### Comparing `swh.objstorage-2.9.1/CODE_OF_CONDUCT.md` & `swh.objstorage-2.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/LICENSE` & `swh.objstorage-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/PKG-INFO` & `swh.objstorage-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 2.9.1
+Version: 2.9.2
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
@@ -29,15 +29,15 @@
 Provides-Extra: libcloud
 Requires-Dist: apache-libcloud; extra == "libcloud"
 Provides-Extra: winery
 Requires-Dist: psycopg[c,pool]; extra == "winery"
 Requires-Dist: systemd-python; extra == "winery"
 Provides-Extra: testing
 Requires-Dist: moto[s3,server]<5; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: requests_mock[fixture]>=1.9; extra == "testing"
 Requires-Dist: requests_toolbelt; extra == "testing"
 Requires-Dist: swh.core[testing]>=3.0.0; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
 Requires-Dist: pytest-postgresql>5; extra == "testing"
```

### Comparing `swh.objstorage-2.9.1/README.rst` & `swh.objstorage-2.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/bin/swh-objstorage-azure` & `swh.objstorage-2.9.2/bin/swh-objstorage-azure`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/docs/winery.rst` & `swh.objstorage-2.9.2/docs/winery.rst`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/mypy.ini` & `swh.objstorage-2.9.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/pyproject.toml` & `swh.objstorage-2.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [project]
 name = "swh.objstorage"
 authors = [
-	{name="Software Heritage developers", email="swh-devel@inria.fr"},
+    {name="Software Heritage developers", email="swh-devel@inria.fr"},
 ]
+
 description = "Software Heritage object storage"
 readme = {file = "README.rst", content-type = "text/x-rst"}
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/api/client.py` & `swh.objstorage-2.9.2/swh/objstorage/api/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-# Copyright (C) 2015-2022  The Software Heritage developers
+# Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from typing import Any, Dict, Iterator, Optional
 
 import msgpack
 
 from swh.core.api import RPCClient
 from swh.objstorage.constants import DEFAULT_LIMIT
-from swh.objstorage.exc import Error, ObjNotFoundError, ObjStorageAPIError
+from swh.objstorage.exc import (
+    Error,
+    ObjCorruptedError,
+    ObjNotFoundError,
+    ObjStorageAPIError,
+)
 from swh.objstorage.interface import CompositeObjId, ObjId, ObjStorageInterface
 from swh.objstorage.objstorage import objid_to_default_hex
 
 
 class RemoteObjStorage(RPCClient):
     """Proxy to a remote object storage.
 
@@ -24,15 +29,15 @@
         url (string): The url of the server to connect. Must end
             with a '/'
         session: The session to send requests.
 
     """
 
     api_exception = ObjStorageAPIError
-    reraise_exceptions = [ObjNotFoundError, Error]
+    reraise_exceptions = [ObjNotFoundError, Error, ObjCorruptedError]
     backend_class = ObjStorageInterface
 
     def restore(self: ObjStorageInterface, content: bytes, obj_id: ObjId) -> None:
         return self.add(content, obj_id, check_presence=False)
 
     def __iter__(self) -> Iterator[CompositeObjId]:
         yield from self.list_content()
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/api/server.py` & `swh.objstorage-2.9.2/swh/objstorage/api/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2015-2022  The Software Heritage developers
+# Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import contextlib
 import functools
 import logging
@@ -13,15 +13,15 @@
 import msgpack
 
 from swh.core.api import RPCServerApp
 from swh.core.api import encode_data_server as encode_data
 from swh.core.api import error_handler
 from swh.core.config import read as config_read
 from swh.core.statsd import statsd
-from swh.objstorage.exc import Error, ObjNotFoundError
+from swh.objstorage.exc import Error, ObjCorruptedError, ObjNotFoundError
 from swh.objstorage.factory import get_objstorage as get_swhobjstorage
 from swh.objstorage.interface import ObjStorageInterface
 
 
 def timed(f):
     @functools.wraps(f)
     def w(*a, **kw):
@@ -46,15 +46,15 @@
     if objstorage is None:
         objstorage = get_swhobjstorage(**app.config["objstorage"])
 
     return objstorage
 
 
 class ObjStorageServerApp(RPCServerApp):
-    client_exception_classes = (ObjNotFoundError, Error)
+    client_exception_classes = (ObjNotFoundError, ObjCorruptedError, Error)
     method_decorators = [timed]
 
     def pre_add(self, kw):
         """Called before the 'add' method."""
         statsd.increment(
             "swh_objstorage_in_bytes_total",
             len(kw["content"]),
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/azure.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/azure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2016-2023  The Software Heritage developers
+# Copyright (C) 2016-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import asyncio
 import contextlib
 from datetime import datetime, timedelta
@@ -16,25 +16,19 @@
     BlobSasPermissions,
     ContainerClient,
     ContainerSasPermissions,
     generate_blob_sas,
     generate_container_sas,
 )
 from azure.storage.blob.aio import ContainerClient as AsyncContainerClient
-from typing_extensions import Literal
 
 from swh.model import hashutil
-from swh.objstorage.exc import Error, ObjNotFoundError
+from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
-from swh.objstorage.objstorage import (
-    ObjStorage,
-    compressors,
-    compute_hash,
-    decompressors,
-)
+from swh.objstorage.objstorage import CompressionFormat, ObjStorage
 from swh.objstorage.utils import call_async
 
 
 def get_container_url(
     account_name: str,
     account_key: str,
     container_name: str,
@@ -107,24 +101,24 @@
       The container url should contain the credentials via a "Shared Access
       Signature". The :func:`get_container_url` helper can be used to generate
       such a URL from the account's access keys. The ``account_name``,
       ``api_secret_key`` and ``container_name`` arguments are deprecated.
 
     """
 
-    PRIMARY_HASH: Literal["sha1"] = "sha1"
+    PRIMARY_HASH = "sha1"
 
     def __init__(
         self,
         container_url: Optional[str] = None,
         account_name: Optional[str] = None,
         api_secret_key: Optional[str] = None,
         container_name: Optional[str] = None,
         connection_string: Optional[str] = None,
-        compression="gzip",
+        compression: CompressionFormat = "gzip",
         use_secondary_endpoint_for_downloads=False,
         **kwargs,
     ):
         if container_url is None and connection_string is None:
             if account_name is None or api_secret_key is None or container_name is None:
                 raise ValueError(
                     "AzureCloudObjStorage must have a container_url, a connection_string,"
@@ -248,17 +242,15 @@
         """Add an obj in storage if it's not there already."""
         if check_presence and obj_id in self:
             return
 
         hex_obj_id = self._internal_id(obj_id)
 
         # Send the compressed content
-        compressor = compressors[self.compression]()
-        data = compressor.compress(content)
-        data += compressor.flush()
+        data = self.compress(content)
 
         client = self.get_blob_client(hex_obj_id)
         try:
             client.upload_blob(data=data, length=len(data))
         except ResourceExistsError:
             # There's a race condition between check_presence and upload_blob,
             # that we can't get rid of as the azure api doesn't allow atomic
@@ -295,19 +287,15 @@
         try:
             download = await client.download_blob()
         except ResourceNotFoundError:
             raise ObjNotFoundError(obj_id) from None
         else:
             data = await download.content_as_bytes()
 
-        decompressor = decompressors[self.compression]()
-        ret = decompressor.decompress(data)
-        if decompressor.unused_data:
-            raise Error("Corrupt object %s: trailing data found" % hex_obj_id)
-        return ret
+        return self.decompress(data, hex_obj_id)
 
     async def _get_async_or_none(self, obj_id, container_clients):
         """Like ``get_async(obj_id)``, but returns None instead of raising
         ResourceNotFoundError. Used by ``get_batch`` so other blobs can be returned
         even if one is missing."""
         try:
             return await self._get_async(obj_id, container_clients)
@@ -323,23 +311,14 @@
                 ]
             )
 
     def get_batch(self, obj_ids: Iterable[ObjId]) -> Iterator[Optional[bytes]]:
         """Retrieve objects' raw content in bulk from storage, concurrently."""
         return call_async(self._get_batch_async, obj_ids)
 
-    def check(self, obj_id: ObjId) -> None:
-        """Check the content integrity."""
-        obj_content = self.get(obj_id)
-        content_obj_id = compute_hash(obj_content)
-        if isinstance(obj_id, dict):
-            obj_id = obj_id[self.PRIMARY_HASH]
-        if content_obj_id != obj_id:
-            raise Error(obj_id)
-
     def delete(self, obj_id: ObjId):
         """Delete an object."""
         super().delete(obj_id)  # Check delete permission
         hex_obj_id = self._internal_id(obj_id)
         client = self.get_blob_client(hex_obj_id)
         try:
             client.delete_blob()
@@ -382,15 +361,15 @@
     accounts is a dict containing entries of the form:
         <prefix>: <container_url_for_prefix>
     """
 
     def __init__(
         self,
         accounts: Mapping[str, Union[str, Mapping[str, str]]],
-        compression="gzip",
+        compression: CompressionFormat = "gzip",
         **kwargs,
     ):
         # shortcut AzureCloudObjStorage __init__
         ObjStorage.__init__(self, **kwargs)
 
         self.compression = compression
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/generator.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/generator.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/http.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/http.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
-# Copyright (C) 2021-2023  The Software Heritage developers
+# Copyright (C) 2021-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from datetime import timedelta
 import logging
 from typing import Iterator, Optional
 from urllib.parse import urljoin
 
 import requests
 
 from swh.model import hashutil
-from swh.objstorage import exc
 from swh.objstorage.constants import ID_HASH_ALGO
+from swh.objstorage.exc import (
+    NonIterableObjStorage,
+    ObjNotFoundError,
+    ReadOnlyObjStorage,
+)
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
     DEFAULT_LIMIT,
+    CompressionFormat,
     ObjStorage,
-    compute_hash,
-    decompressors,
     objid_to_default_hex,
 )
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.ERROR)
 
 
@@ -32,15 +35,15 @@
     For example, can be used to retrieve objects from S3:
 
     objstorage:
       cls: http
       url: https://softwareheritage.s3.amazonaws.com/content/
     """
 
-    def __init__(self, url=None, compression=None, **kwargs):
+    def __init__(self, url=None, compression: CompressionFormat = "none", **kwargs):
         super().__init__(**kwargs)
         self.session = requests.sessions.Session()
         self.root_path = url
         if not self.root_path.endswith("/"):
             self.root_path += "/"
         self.compression = compression
 
@@ -49,66 +52,52 @@
         return True
 
     def __contains__(self, obj_id: ObjId) -> bool:
         resp = self.session.head(self._path(obj_id))
         return resp.status_code == 200
 
     def __iter__(self) -> Iterator[CompositeObjId]:
-        raise exc.NonIterableObjStorage("__iter__")
+        raise NonIterableObjStorage("__iter__")
 
     def __len__(self):
-        raise exc.NonIterableObjStorage("__len__")
+        raise NonIterableObjStorage("__len__")
 
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
-        raise exc.ReadOnlyObjStorage("add")
+        raise ReadOnlyObjStorage("add")
 
     def delete(self, obj_id: ObjId):
-        raise exc.ReadOnlyObjStorage("delete")
+        raise ReadOnlyObjStorage("delete")
 
     def restore(self, content: bytes, obj_id: ObjId) -> None:
-        raise exc.ReadOnlyObjStorage("restore")
+        raise ReadOnlyObjStorage("restore")
 
     def list_content(
         self,
         last_obj_id: Optional[ObjId] = None,
         limit: Optional[int] = DEFAULT_LIMIT,
     ) -> Iterator[CompositeObjId]:
-        raise exc.NonIterableObjStorage("__len__")
+        raise NonIterableObjStorage("__len__")
 
     def get(self, obj_id: ObjId) -> bytes:
         try:
             resp = self.session.get(self._path(obj_id))
             resp.raise_for_status()
         except Exception:
-            raise exc.ObjNotFoundError(obj_id)
+            raise ObjNotFoundError(obj_id)
 
-        ret: bytes = resp.content
-        if self.compression:
-            d = decompressors[self.compression]()
-            ret = d.decompress(ret)
-            if d.unused_data:
-                hex_obj_id = objid_to_default_hex(obj_id)
-                raise exc.Error("Corrupt object %s: trailing data found" % hex_obj_id)
-        return ret
+        return self.decompress(resp.content, objid_to_default_hex(obj_id))
 
     def download_url(
         self,
         obj_id: ObjId,
         content_disposition: Optional[str] = None,
         expiry: Optional[timedelta] = None,
     ) -> Optional[str]:
         return self._path(obj_id)
 
-    def check(self, obj_id: ObjId) -> None:
-        # Check the content integrity
-        obj_content = self.get(obj_id)
-        content_obj_id = compute_hash(obj_content)
-        if content_obj_id != self._hash(obj_id):
-            raise exc.Error(obj_id)
-
     def _hash(self, obj_id: ObjId) -> bytes:
         if isinstance(obj_id, dict):
             return obj_id[ID_HASH_ALGO]
         else:
             return obj_id
 
     def _path(self, obj_id):
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/in_memory.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/in_memory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# Copyright (C) 2017-2022  The Software Heritage developers
+# Copyright (C) 2017-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from typing import Dict, Iterator
 
-from typing_extensions import Literal
-
-from swh.objstorage.exc import Error, ObjNotFoundError
+from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
-from swh.objstorage.objstorage import ObjStorage, compute_hash, objid_to_default_hex
+from swh.objstorage.objstorage import ObjStorage
 
 
 class InMemoryObjStorage(ObjStorage):
     """In-Memory objstorage.
 
     Intended for test purposes.
 
     """
 
-    PRIMARY_HASH: Literal["sha1"] = "sha1"
+    PRIMARY_HASH = "sha1"
 
     def __init__(self, **args):
         super().__init__()
         self.state: Dict[bytes, bytes] = {}
 
     def check_config(self, *, check_write):
         return True
@@ -49,20 +47,14 @@
 
     def get(self, obj_id: ObjId) -> bytes:
         if obj_id not in self:
             raise ObjNotFoundError(obj_id)
 
         return self.state[self._state_key(obj_id)]
 
-    def check(self, obj_id: ObjId) -> None:
-        if obj_id not in self:
-            raise ObjNotFoundError(obj_id)
-        if compute_hash(self.state[self._state_key(obj_id)]) != self._state_key(obj_id):
-            raise Error("Corrupt object %s" % objid_to_default_hex(obj_id))
-
     def delete(self, obj_id: ObjId):
         super().delete(obj_id)  # Check delete permission
         if obj_id not in self:
             raise ObjNotFoundError(obj_id)
 
         self.state.pop(self._state_key(obj_id))
         return True
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/libcloud.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/libcloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-# Copyright (C) 2016-2023  The Software Heritage developers
+# Copyright (C) 2016-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import abc
 from collections import OrderedDict
 from datetime import timedelta
+from io import BytesIO
 from typing import Iterator, Optional
 from urllib.parse import urlencode
 
 from libcloud.storage import providers
 import libcloud.storage.drivers.s3
 from libcloud.storage.types import ObjectDoesNotExistError, Provider
-from typing_extensions import Literal
 
 from swh.model import hashutil
-from swh.objstorage.exc import Error, ObjNotFoundError
+from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
+    CompressionFormat,
     ObjStorage,
-    compressors,
-    compute_hash,
-    decompressors,
     objid_to_default_hex,
 )
 
 
 def patch_libcloud_s3_urlencode():
     """Patches libcloud's S3 backend to properly sign queries.
 
@@ -57,20 +55,20 @@
       container_name: Name of the base container
       path_prefix: prefix to prepend to object paths in the container,
                    separated with a slash
       compression: compression algorithm to use for objects
       kwargs: extra arguments are passed through to the LibCloud driver
     """
 
-    PRIMARY_HASH: Literal["sha1"] = "sha1"
+    PRIMARY_HASH = "sha1"
 
     def __init__(
         self,
         container_name: str,
-        compression: str = "gzip",
+        compression: CompressionFormat = "gzip",
         path_prefix: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.driver = self._get_driver(**kwargs)
         self.container_name = container_name
         self.container = self.driver.get_container(container_name=container_name)
@@ -168,40 +166,24 @@
         self._put_object(content, obj_id)
 
     def restore(self, content: bytes, obj_id: ObjId) -> None:
         return self.add(content, obj_id, check_presence=False)
 
     def get(self, obj_id: ObjId) -> bytes:
         obj = b"".join(self._get_object(obj_id).as_stream())
-        d = decompressors[self.compression]()
-        ret = d.decompress(obj)
-        if d.unused_data:
-            hex_obj_id = objid_to_default_hex(obj_id)
-            raise Error("Corrupt object %s: trailing data found" % hex_obj_id)
-        return ret
+        return self.decompress(obj, objid_to_default_hex(obj_id))
 
     def download_url(
         self,
         obj_id: ObjId,
         content_disposition: Optional[str] = None,
         expiry: Optional[timedelta] = None,
     ) -> Optional[str]:
         return self._get_object(obj_id).get_cdn_url()
 
-    def check(self, obj_id: ObjId) -> None:
-        # Check that the file exists, as _get_object raises ObjNotFoundError
-        self._get_object(obj_id)
-        # Check the content integrity
-        obj_content = self.get(obj_id)
-        content_obj_id = compute_hash(obj_content)
-        if isinstance(obj_id, dict):
-            obj_id = obj_id[self.PRIMARY_HASH]
-        if content_obj_id != obj_id:
-            raise Error(obj_id)
-
     def delete(self, obj_id: ObjId):
         super().delete(obj_id)  # Check delete permission
         obj = self._get_object(obj_id)
         return self.driver.delete_object(obj)
 
     def _object_path(self, obj_id: ObjId) -> str:
         """Get the full path to an object"""
@@ -224,37 +206,26 @@
         object_path = self._object_path(obj_id)
 
         try:
             return self.driver.get_object(self.container_name, object_path)
         except ObjectDoesNotExistError:
             raise ObjNotFoundError(obj_id)
 
-    def _compressor(self, data):
-        comp = compressors[self.compression]()
-        for chunk in data:
-            cchunk = comp.compress(chunk)
-            if cchunk:
-                yield cchunk
-        trail = comp.flush()
-        if trail:
-            yield trail
-
     def _put_object(self, content, obj_id):
         """Create an object in the cloud storage.
 
         Created object will contain the content and be referenced by
         the given id.
 
         """
         object_path = self._object_path(obj_id)
-
-        if not isinstance(content, Iterator):
-            content = (content,)
         self.driver.upload_object_via_stream(
-            self._compressor(content), self.container, object_path
+            BytesIO(self.compress(content)),
+            self.container,
+            object_path,
         )
 
 
 class AwsCloudObjStorage(CloudObjStorage):
     """Amazon's S3 Cloud-based object storage"""
 
     def _get_provider(self):
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/noop.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/noop.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/pathslicing.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/pathslicing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-# Copyright (C) 2015-2022  The Software Heritage developers
+# Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from contextlib import contextmanager
 from itertools import islice
 import os
 import tempfile
 from typing import Iterator, List, Optional
 
-from typing_extensions import Literal
-
-from swh.model import hashutil
 from swh.objstorage.constants import DEFAULT_LIMIT, ID_HASH_ALGO, ID_HEXDIGEST_LENGTH
-from swh.objstorage.exc import Error, ObjNotFoundError
+from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
+    CompressionFormat,
     ObjStorage,
     compressors,
-    decompressors,
     objid_to_default_hex,
 )
 
 BUFSIZ = 1048576
 
 DIR_MODE = 0o755
 FILE_MODE = 0o644
@@ -150,17 +147,19 @@
             the disk.
         slicing (str): string that indicates the slicing to perform
             on the hash of the content to know the path where it should
             be stored (see the documentation of the PathSlicer class).
 
     """
 
-    PRIMARY_HASH: Literal["sha1"] = "sha1"
+    PRIMARY_HASH = "sha1"
 
-    def __init__(self, root, slicing, compression="gzip", **kwargs):
+    def __init__(
+        self, root, slicing, compression: CompressionFormat = "gzip", **kwargs
+    ):
         super().__init__(**kwargs)
         self.root = root
         self.slicer = PathSlicer(root, slicing)
 
         self.use_fdatasync = hasattr(os, "fdatasync")
         self.compression = compression
 
@@ -234,56 +233,25 @@
         check_presence: bool = True,
     ) -> None:
         if check_presence and obj_id in self:
             # If the object is already present, return immediately.
             return
 
         hex_obj_id = objid_to_default_hex(obj_id)
-        compressor = compressors[self.compression]()
         with self._write_obj_file(hex_obj_id) as f:
-            f.write(compressor.compress(content))
-            f.write(compressor.flush())
+            f.write(self.compress(content))
 
     def get(self, obj_id: ObjId) -> bytes:
         if obj_id not in self:
             raise ObjNotFoundError(obj_id)
 
         # Open the file and return its content as bytes
         hex_obj_id = objid_to_default_hex(obj_id)
-        d = decompressors[self.compression]()
         with open(self.slicer.get_path(hex_obj_id), "rb") as f:
-            out = d.decompress(f.read())
-        if d.unused_data:
-            raise Error(
-                "Corrupt object %s: trailing data found" % hex_obj_id,
-            )
-
-        return out
-
-    def check(self, obj_id: ObjId) -> None:
-        try:
-            data = self.get(obj_id)
-        except OSError:
-            hex_obj_id = objid_to_default_hex(obj_id)
-            raise Error(
-                "Corrupt object %s: not a proper compressed file" % hex_obj_id,
-            )
-
-        checksums = hashutil.MultiHash.from_data(
-            data, hash_names=[ID_HASH_ALGO]
-        ).digest()
-
-        actual_obj_sha1 = checksums[ID_HASH_ALGO]
-        hex_obj_id = objid_to_default_hex(obj_id)
-
-        if hex_obj_id != hashutil.hash_to_hex(actual_obj_sha1):
-            raise Error(
-                "Corrupt object %s should have id %s"
-                % (objid_to_default_hex(obj_id), hashutil.hash_to_hex(actual_obj_sha1))
-            )
+            return self.decompress(f.read(), hex_obj_id)
 
     def delete(self, obj_id: ObjId):
         super().delete(obj_id)  # Check delete permission
         if obj_id not in self:
             raise ObjNotFoundError(obj_id)
 
         hex_obj_id = objid_to_default_hex(obj_id)
@@ -291,22 +259,14 @@
             os.remove(self.slicer.get_path(hex_obj_id))
         except FileNotFoundError:
             raise ObjNotFoundError(obj_id)
         return True
 
     # Streaming methods
 
-    @contextmanager
-    def chunk_writer(self, obj_id):
-        hex_obj_id = objid_to_default_hex(obj_id)
-        compressor = compressors[self.compression]()
-        with self._write_obj_file(hex_obj_id) as f:
-            yield lambda c: f.write(compressor.compress(c))
-            f.write(compressor.flush())
-
     def list_content(
         self, last_obj_id: Optional[ObjId] = None, limit: Optional[int] = DEFAULT_LIMIT
     ) -> Iterator[CompositeObjId]:
         if last_obj_id:
             it = self.iter_from(last_obj_id)
         else:
             it = iter(self)
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/seaweedfs/http.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/http.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/seaweedfs/objstorage.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/seaweedfs/objstorage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,51 @@
-# Copyright (C) 2019-2023  The Software Heritage developers
+# Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from datetime import timedelta
 import io
 from itertools import islice
 import logging
 from typing import Iterator, Optional
 from urllib.parse import urlparse
 
-from typing_extensions import Literal
-
 from swh.model import hashutil
 from swh.objstorage.backends.pathslicing import PathSlicer
-from swh.objstorage.exc import Error, ObjNotFoundError
+from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import (
     DEFAULT_LIMIT,
+    CompressionFormat,
     ObjStorage,
-    compressors,
-    compute_hash,
-    decompressors,
     objid_to_default_hex,
 )
 
 from .http import HttpFiler
 
 LOGGER = logging.getLogger(__name__)
 
 
 class SeaweedFilerObjStorage(ObjStorage):
     """ObjStorage with seaweedfs abilities, using the Filer API.
 
     https://github.com/chrislusf/seaweedfs/wiki/Filer-Server-API
     """
 
-    PRIMARY_HASH: Literal["sha1"] = "sha1"
+    PRIMARY_HASH = "sha1"
 
-    def __init__(self, url, compression=None, slicing="", pool_maxsize=100, **kwargs):
+    def __init__(
+        self,
+        url,
+        compression: CompressionFormat = "none",
+        slicing="",
+        pool_maxsize=100,
+        **kwargs,
+    ):
         super().__init__(**kwargs)
         self.wf = HttpFiler(url, pool_maxsize=pool_maxsize)
         self.root_path = urlparse(url).path
         if not self.root_path.endswith("/"):
             self.root_path += "/"
         self.slicer = PathSlicer(self.root_path, slicing)
         self.compression = compression
@@ -81,62 +84,39 @@
         """
         return sum(1 for i in self)
 
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
         if check_presence and obj_id in self:
             return
 
-        def compressor(data):
-            comp = compressors[self.compression]()
-            yield comp.compress(data)
-            yield comp.flush()
-
-        assert isinstance(
-            content, bytes
-        ), "list of content chunks is not supported anymore"
-
-        self.wf.put(io.BytesIO(b"".join(compressor(content))), self._path(obj_id))
+        self.wf.put(io.BytesIO(self.compress(content)), self._path(obj_id))
 
     def restore(self, content: bytes, obj_id: ObjId) -> None:
         return self.add(content, obj_id, check_presence=False)
 
     def get(self, obj_id: ObjId) -> bytes:
         try:
             obj = self.wf.get(self._path(obj_id))
         except Exception as exc:
             LOGGER.info("Failed to get object %s: %r", self._path(obj_id), exc)
             raise ObjNotFoundError(obj_id)
 
-        d = decompressors[self.compression]()
-        ret = d.decompress(obj)
-        if d.unused_data:
-            hex_obj_id = objid_to_default_hex(obj_id)
-            raise Error("Corrupt object %s: trailing data found" % hex_obj_id)
-        return ret
+        return self.decompress(obj, objid_to_default_hex(obj_id))
 
     def download_url(
         self,
         obj_id: ObjId,
         content_disposition: Optional[str] = None,
         expiry: Optional[timedelta] = None,
     ) -> Optional[str]:
         path = self._path(obj_id)
         if not self.wf.exists(path):
             raise ObjNotFoundError(obj_id)
         return self.wf.build_url(path)
 
-    def check(self, obj_id: ObjId) -> None:
-        # Check the content integrity
-        obj_content = self.get(obj_id)
-        content_obj_id = compute_hash(obj_content)
-        if isinstance(obj_id, dict):
-            obj_id = obj_id[self.PRIMARY_HASH]
-        if content_obj_id != obj_id:
-            raise Error(obj_id)
-
     def delete(self, obj_id: ObjId):
         super().delete(obj_id)  # Check delete permission
         if obj_id not in self:
             raise ObjNotFoundError(obj_id)
         self.wf.delete(self._path(obj_id))
         return True
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/winery/database.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/winery/database.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/winery/objstorage.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/winery/objstorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import logging
 from multiprocessing import Process
 from typing import Callable, Optional, Tuple
 
-from typing_extensions import Literal
-
-from swh.objstorage import exc
+from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.interface import ObjId
 from swh.objstorage.objstorage import ObjStorage
 
 from .roshard import (
     DEFAULT_IMAGE_FEATURES_UNSUPPORTED,
     Pool,
     ROShard,
@@ -25,15 +23,15 @@
 from .sleep import sleep_exponential
 from .stats import Stats
 
 logger = logging.getLogger(__name__)
 
 
 class WineryObjStorage(ObjStorage):
-    PRIMARY_HASH: Literal["sha256"] = "sha256"
+    PRIMARY_HASH = "sha256"
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         if kwargs.get("readonly"):
             self.winery = WineryReader(**kwargs)
         else:
             self.winery = WineryWriter(**kwargs)
@@ -49,17 +47,14 @@
 
     def __contains__(self, obj_id: ObjId) -> bool:
         return self._hash(obj_id) in self.winery
 
     def add(self, content: bytes, obj_id: ObjId, check_presence: bool = True) -> None:
         self.winery.add(content, self._hash(obj_id), check_presence)
 
-    def check(self, obj_id: ObjId) -> None:
-        return self.winery.check(self._hash(obj_id))
-
     def delete(self, obj_id: ObjId):
         if not self.allow_delete:
             raise PermissionError("Delete is not allowed.")
         return self.winery.delete(obj_id)
 
     def _hash(self, obj_id: ObjId) -> bytes:
         if isinstance(obj_id, dict):
@@ -106,26 +101,26 @@
             shard = RWShard(name, **self.args)
             self.rw_shards[name] = shard
         return self.rw_shards[name]
 
     def get(self, obj_id: ObjId) -> bytes:
         shard_info = self.base.get(obj_id)
         if shard_info is None:
-            raise exc.ObjNotFoundError(obj_id)
+            raise ObjNotFoundError(obj_id)
         name, state = shard_info
         content: Optional[bytes] = None
         if state.image_available:
             roshard = self.roshard(name)
             if roshard:
                 content = roshard.get(obj_id)
         if content is None:
             rwshard = self.rwshard(name)
             content = rwshard.get(obj_id)
         if content is None:
-            raise exc.ObjNotFoundError(obj_id)
+            raise ObjNotFoundError(obj_id)
         return content
 
     def uninit(self):
         for shard in self.rw_shards.values():
             shard.uninit()
         self.rw_shards = {}
         for shard in self.ro_shards.values():
@@ -223,15 +218,15 @@
                 # Switch shards
                 self.uninit()
                 self.init()
 
     def delete(self, obj_id: ObjId):
         shard_info = self.base.get(obj_id)
         if shard_info is None:
-            raise exc.ObjNotFoundError(obj_id)
+            raise ObjNotFoundError(obj_id)
         name, state = shard_info
         # We only care about RWShard for now. ROShards will be
         # taken care in a batch job.
         if not state.image_available:
             rwshard = self.rwshard(name)
             try:
                 rwshard.delete(obj_id)
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/winery/roshard.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/winery/roshard.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/winery/rwshard.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/winery/rwshard.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/winery/sharedbase.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/winery/sharedbase.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/winery/sleep.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/winery/sleep.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/winery/stats.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/winery/stats.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/backends/winery/throttler.py` & `swh.objstorage-2.9.2/swh/objstorage/backends/winery/throttler.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/cli.py` & `swh.objstorage-2.9.2/swh/objstorage/cli.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/constants.py` & `swh.objstorage-2.9.2/swh/objstorage/constants.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/factory.py` & `swh.objstorage-2.9.2/swh/objstorage/factory.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/interface.py` & `swh.objstorage-2.9.2/swh/objstorage/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         the object id.
 
         Args:
             obj_id: object identifier.
 
         Raises:
             ObjNotFoundError: if the requested object is missing.
-            Error: if the request object is corrupted.
+            ObjCorruptedError: if the requested object is corrupted.
 
         """
         ...
 
     @remote_api_endpoint("content/delete")
     def delete(self, obj_id: ObjId):
         """Delete an object.
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/multiplexer/filter/__init__.py` & `swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/multiplexer/filter/filter.py` & `swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/filter.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/multiplexer/filter/read_write_filter.py` & `swh.objstorage-2.9.2/swh/objstorage/multiplexer/filter/read_write_filter.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/multiplexer/multiplexer_objstorage.py` & `swh.objstorage-2.9.2/swh/objstorage/multiplexer/multiplexer_objstorage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (C) 2015-2023  The Software Heritage developers
+# Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import queue
 import threading
-from typing import Dict, Iterable, Iterator, Mapping, Tuple, Union
+from typing import Dict, Iterable, Iterator, Mapping, Optional, Tuple, Union
 
 from swh.model.model import Sha1
-from swh.objstorage.exc import ObjNotFoundError
+from swh.objstorage.exc import ObjCorruptedError, ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjId
 from swh.objstorage.objstorage import ObjStorage
 
 
 class ObjStorageThread(threading.Thread):
     def __init__(self, storage):
         super().__init__(daemon=True)
@@ -290,24 +290,29 @@
             except ObjNotFoundError:
                 continue
         # If no storage contains this content, raise the error
         raise ObjNotFoundError(obj_id)
 
     def check(self, obj_id: ObjId) -> None:
         nb_present = 0
+        nb_corrupted = 0
+        exception: Optional[Exception] = None
         for storage in self.get_read_threads(obj_id):
             try:
                 storage.check(obj_id)
-            except ObjNotFoundError:
+            except ObjNotFoundError as e:
+                exception = e
                 continue
+            except ObjCorruptedError as e:
+                exception = e
+                nb_corrupted += 1
             else:
                 nb_present += 1
-        # If there is an Error because of a corrupted file, then let it pass.
 
-        # Raise the ObjNotFoundError only if the content couldn't be found in
-        # all the storages.
-        if nb_present == 0:
-            raise ObjNotFoundError(obj_id)
+        # Raise exception only if the content could not be found in all the storages
+        # or is corrupted in all the storages
+        if exception and (nb_present == 0 or nb_corrupted == len(self.storages)):
+            raise exception
 
     def delete(self, obj_id: ObjId):
         super().delete(obj_id)  # Check delete permission
         return all(self.wrap_call(self.get_write_threads(obj_id), "delete", obj_id))
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/objstorage.py` & `swh.objstorage-2.9.2/swh/objstorage/objstorage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,85 @@
-# Copyright (C) 2015-2023  The Software Heritage developers
+# Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import abc
 import bz2
 import collections
 from datetime import timedelta
 from itertools import dropwhile, islice
 import lzma
-from typing import Callable, Dict, Iterable, Iterator, Mapping, Optional, Tuple, Union
+from typing import (
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    Literal,
+    Mapping,
+    Optional,
+    Tuple,
+    Union,
+)
 import zlib
 
 from typing_extensions import Protocol
 
 from swh.model import hashutil
 from swh.model.model import Sha1
+from swh.objstorage.constants import DEFAULT_LIMIT, ID_HASH_ALGO
+from swh.objstorage.exc import ObjCorruptedError, ObjNotFoundError
+from swh.objstorage.interface import CompositeObjId, ObjId, ObjStorageInterface
 
-from .constants import DEFAULT_LIMIT, ID_HASH_ALGO
-from .exc import ObjNotFoundError
-from .interface import CompositeObjId, ObjId, ObjStorageInterface
 
-
-def objid_to_default_hex(obj_id: ObjId) -> str:
+def objid_to_default_hex(
+    obj_id: ObjId, algo: Literal["sha1", "sha256"] = ID_HASH_ALGO
+) -> str:
     """Converts SHA1 hashes and multi-hashes to the hexadecimal representation
     of the SHA1."""
     if isinstance(obj_id, bytes):
         return hashutil.hash_to_hex(obj_id)
     elif isinstance(obj_id, str):
         return obj_id
     else:
-        return hashutil.hash_to_hex(obj_id[ID_HASH_ALGO])
+        return hashutil.hash_to_hex(obj_id[algo])
+
+
+def compute_hashes(
+    content: bytes, hash_names: Iterable[str] = hashutil.DEFAULT_ALGORITHMS
+) -> Dict[str, bytes]:
+    """Compute the content's hashes.
+
+    Args:
+        content: The raw content to hash
+        hash_names: Names of hashing algorithms
+            (default to :const:`swh.model.hashutil.DEFAULT_ALGORITHMS`)
+
+    Returns:
+        A dict mapping algo name to hash value
+
+    """
+    return hashutil.MultiHash.from_data(
+        content,
+        hash_names=hash_names,
+    ).digest()
 
 
-def compute_hash(content, algo=ID_HASH_ALGO):
+def compute_hash(content: bytes, algo: str = ID_HASH_ALGO) -> bytes:
     """Compute the content's hash.
 
     Args:
-        content (bytes): The raw content to hash
-        hash_name (str): Hash's name (default to ID_HASH_ALGO)
+        content: The raw content to hash
+        hash_name: Hash's name
 
     Returns:
-        The ID_HASH_ALGO for the content
+        The computed hash for the content
 
     """
-    return (
-        hashutil.MultiHash.from_data(
-            content,
-            hash_names=[algo],
-        )
-        .digest()
-        .get(algo)
-    )
+    return compute_hashes(content, [algo])[algo]
 
 
 class NullCompressor:
     def compress(self, data):
         return data
 
     def flush(self):
@@ -98,16 +122,21 @@
     "bz2": bz2.BZ2Compressor,
     "lzma": lzma.LZMACompressor,
     "gzip": lambda: zlib.compressobj(wbits=31),
     "zlib": zlib.compressobj,
     "none": NullCompressor,
 }
 
+CompressionFormat = Literal["bz2", "lzma", "gzip", "zlib", "none"]
+
 
 class ObjStorage(metaclass=abc.ABCMeta):
+    PRIMARY_HASH: Literal["sha1", "sha256"] = "sha1"
+    compression: CompressionFormat = "none"
+
     def __init__(self, *, allow_delete=False, **kwargs):
         # A more complete permission system could be used in place of that if
         # it becomes needed
         self.allow_delete = allow_delete
 
     def add_batch(
         self: ObjStorageInterface,
@@ -160,7 +189,51 @@
     def download_url(
         self,
         obj_id: ObjId,
         content_disposition: Optional[str] = None,
         expiry: Optional[timedelta] = None,
     ) -> Optional[str]:
         return None
+
+    @abc.abstractmethod
+    def get(self, obj_id: ObjId) -> bytes:
+        raise NotImplementedError()
+
+    def check(self, obj_id: ObjId) -> None:
+        """Check if a content is found and recompute its hash to check integrity."""
+        obj_content = self.get(obj_id)
+        hash_algos = [str(self.PRIMARY_HASH)]
+        if isinstance(obj_id, dict):
+            hash_algos += [algo for algo in obj_id if algo != self.PRIMARY_HASH]
+        actual_hashes = compute_hashes(obj_content, hash_algos)
+        for algo in hash_algos:
+            actual_obj_id = actual_hashes[algo]
+            expected_obj_id = obj_id
+            if isinstance(obj_id, dict):
+                expected_obj_id = obj_id[algo]  # type: ignore[literal-required]
+            if actual_obj_id != expected_obj_id:
+                raise ObjCorruptedError(
+                    f"expected {algo} hash is {hashutil.hash_to_hex(expected_obj_id)}, "
+                    f"actual {algo} hash is {hashutil.hash_to_hex(actual_obj_id)}"
+                )
+
+    def compress(self, data: bytes) -> bytes:
+        compressor = compressors[self.compression]()
+        compressed = compressor.compress(data)
+        compressed += compressor.flush()
+        return compressed
+
+    def decompress(self, data: bytes, hex_obj_id: str) -> bytes:
+        decompressor = decompressors[self.compression]()
+        try:
+            ret = decompressor.decompress(data)
+        except (zlib.error, lzma.LZMAError, OSError):
+            raise ObjCorruptedError(
+                f"content with {self.PRIMARY_HASH} hash {hex_obj_id} is not a proper "
+                "compressed file"
+            )
+        if decompressor.unused_data:
+            raise ObjCorruptedError(
+                f"trailing data found when decompressing content with {self.PRIMARY_HASH} "
+                f"{hex_obj_id}"
+            )
+        return ret
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/pytest_plugin.py` & `swh.objstorage-2.9.2/swh/objstorage/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/conftest.py` & `swh.objstorage-2.9.2/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/objstorage_testing.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/objstorage_testing.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import inspect
 from typing import Tuple
 
 import pytest
 import requests
 
-from swh.objstorage import exc
+from swh.objstorage.exc import ObjCorruptedError, ObjNotFoundError
 from swh.objstorage.interface import CompositeObjId, ObjStorageInterface
 from swh.objstorage.objstorage import compute_hash, decompressors
 
 
 class ObjStorageTestFixture:
     num_objects = 1200
 
@@ -142,85 +142,87 @@
 
     def test_restore_content(self):
         self.storage.allow_delete = True
 
         valid_content, valid_obj_id = self.hash_content(b"restore_content")
         invalid_content = b"unexpected content"
         self.storage.add(invalid_content, valid_obj_id)
-        with pytest.raises(exc.Error):
+        with pytest.raises((ObjCorruptedError, ObjNotFoundError)):
+            # raise Corrupted except read only storage that raises NotFound,
             self.storage.check(valid_obj_id)
+        assert valid_obj_id in self.storage
         self.storage.restore(valid_content, valid_obj_id)
         self.assertContentMatch(valid_obj_id, valid_content)
 
     def test_get_missing(self):
         content, obj_id = self.hash_content(b"get_missing")
-        with pytest.raises(exc.ObjNotFoundError) as e:
+        with pytest.raises(ObjNotFoundError) as e:
             self.storage.get(obj_id)
 
         assert obj_id in e.value.args
 
     def test_get_missing_composite(self):
         content, obj_id = self.compositehash_content(b"get_missing")
-        with pytest.raises(exc.ObjNotFoundError) as e:
+        with pytest.raises(ObjNotFoundError) as e:
             self.storage.get(obj_id)
 
         assert obj_id in e.value.args
 
     def test_check_missing(self):
         content, obj_id = self.hash_content(b"check_missing")
-        with pytest.raises(exc.Error):
+        with pytest.raises(ObjNotFoundError):
             self.storage.check(obj_id)
 
     def test_check_missing_composite(self):
         content, obj_id = self.compositehash_content(b"check_missing")
-        with pytest.raises(exc.Error):
+        with pytest.raises(ObjNotFoundError):
             self.storage.check(obj_id)
 
     def test_check_present(self):
         content, obj_id = self.hash_content(b"check_present")
         self.storage.add(content, obj_id)
         try:
             self.storage.check(obj_id)
-        except exc.Error:
+        except ObjCorruptedError:
             self.fail("Integrity check failed")
 
     def test_check_present_composite(self):
         content, obj_id = self.compositehash_content(b"check_present")
         self.storage.add(content, obj_id)
         try:
             self.storage.check(obj_id)
-        except exc.Error:
+        except ObjCorruptedError:
             self.fail("Integrity check failed")
 
     def test_delete_missing(self):
         self.storage.allow_delete = True
         content, obj_id = self.hash_content(b"missing_content_to_delete")
-        with pytest.raises(exc.Error):
+        with pytest.raises(ObjNotFoundError):
             self.storage.delete(obj_id)
 
     def test_delete_missing_composite(self):
         self.storage.allow_delete = True
         content, obj_id = self.compositehash_content(b"missing_content_to_delete")
-        with pytest.raises(exc.Error):
+        with pytest.raises(ObjNotFoundError):
             self.storage.delete(obj_id)
 
     def test_delete_present(self):
         self.storage.allow_delete = True
         content, obj_id = self.hash_content(b"content_to_delete")
         self.storage.add(content, obj_id=obj_id)
         assert self.storage.delete(obj_id)
-        with pytest.raises(exc.Error):
+        with pytest.raises(ObjNotFoundError):
             self.storage.get(obj_id)
 
     def test_delete_present_composite(self):
         self.storage.allow_delete = True
         content, obj_id = self.compositehash_content(b"content_to_delete")
         self.storage.add(content, obj_id=obj_id)
         assert self.storage.delete(obj_id)
-        with pytest.raises(exc.Error):
+        with pytest.raises(ObjNotFoundError):
             self.storage.get(obj_id)
 
     def test_delete_not_allowed(self):
         self.storage.allow_delete = False
         content, obj_id = self.hash_content(b"content_to_delete")
         self.storage.add(content, obj_id=obj_id)
         with pytest.raises(PermissionError):
@@ -352,9 +354,9 @@
         obj_id = compute_hash(content)
         self.storage.add(content, obj_id)
         url = self.storage.download_url(obj_id)
         if url is not None:
             decompress = decompressors[self.storage.compression]().decompress
             assert decompress(requests.get(url).content) == content
 
-            with pytest.raises(exc.ObjNotFoundError):
+            with pytest.raises(ObjNotFoundError):
                 self.storage.download_url(b"\xff" * 20)
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_interface.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_api.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_api.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_azure.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from azure.core.exceptions import ResourceExistsError, ResourceNotFoundError
 from azure.storage.blob import BlobServiceClient
 import pytest
 
 from swh.model.hashutil import hash_to_hex
 import swh.objstorage.backends.azure
-from swh.objstorage.exc import Error
+from swh.objstorage.exc import ObjCorruptedError
 from swh.objstorage.factory import get_objstorage
 from swh.objstorage.objstorage import decompressors
 
 from .objstorage_testing import ObjStorageTestFixture
 
 AZURITE_EXE = shutil.which(
     "azurite-blob", path=os.environ.get("AZURITE_PATH", os.environ.get("PATH"))
@@ -254,21 +254,19 @@
         blob_client = self.storage.get_blob_client(internal_id)
         raw_blob = blob_client.download_blob().content_as_bytes()
         new_data = raw_blob + b"trailing garbage"
 
         blob_client.delete_blob()
         blob_client.upload_blob(data=new_data, length=len(new_data))
 
-        if self.compression == "none":
-            with pytest.raises(Error) as e:
-                self.storage.check(obj_id)
-        else:
-            with pytest.raises(Error) as e:
-                self.storage.get(obj_id)
-            assert "trailing data" in e.value.args[0]
+        with pytest.raises(ObjCorruptedError) as e:
+            self.storage.check(obj_id)
+
+        if self.compression != "none":
+            assert "trailing data found" in e.value.args[0]
 
     @pytest.mark.skip("makes no sense to test this for the mocked azure")
     def test_download_url(self):
         pass
 
 
 class TestMockedAzureCloudObjStorageGzip(TestMockedAzureCloudObjStorage):
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_cloud.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     ContainerDoesNotExistError,
     ObjectDoesNotExistError,
     Provider,
 )
 import pytest
 
 from swh.objstorage.backends.libcloud import CloudObjStorage
-from swh.objstorage.exc import Error
+from swh.objstorage.exc import ObjCorruptedError
 from swh.objstorage.objstorage import decompressors
 
 from .objstorage_testing import ObjStorageTestFixture
 
 API_KEY = "API_KEY"
 API_SECRET_KEY = "API SECRET KEY"
 CONTAINER_NAME = "test_container"
@@ -129,21 +129,19 @@
     def test_trailing_data_on_stored_blob(self):
         content, obj_id = self.hash_content(b"test content without garbage")
         self.storage.add(content, obj_id=obj_id)
 
         libcloud_object = self.storage._get_object(obj_id)
         libcloud_object.content.append(b"trailing garbage")
 
-        if self.compression == "none":
-            with pytest.raises(Error) as e:
-                self.storage.check(obj_id)
-        else:
-            with pytest.raises(Error) as e:
-                self.storage.get(obj_id)
-            assert "trailing data" in e.value.args[0]
+        with pytest.raises(ObjCorruptedError) as e:
+            self.storage.check(obj_id)
+
+        if self.compression != "none":
+            assert "trailing data found" in e.value.args[0]
 
     @pytest.mark.skip("makes no sense to test this for the mocked libcloud")
     def test_download_url(self):
         pass
 
 
 @pytest.mark.all_compression_methods
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_http.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_http.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,24 @@
-# Copyright (C) 2021-2023  The Software Heritage developers
+# Copyright (C) 2021-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import pytest
 import requests
 import requests_mock
 from requests_mock.contrib import fixture
 
 from swh.model import hashutil
-from swh.objstorage import exc
+from swh.objstorage.exc import (
+    NonIterableObjStorage,
+    ObjCorruptedError,
+    ObjNotFoundError,
+    ReadOnlyObjStorage,
+)
 from swh.objstorage.factory import get_objstorage
 from swh.objstorage.objstorage import compute_hash
 
 
 def build_objstorage(multi_hash=False):
     """Build an HTTPReadOnlyObjStorage suitable for tests
 
@@ -76,53 +81,53 @@
 
     assert b"\x00" * 20 not in sto_front
 
 
 def test_http_objstorage_get_missing():
     sto_front, sto_back, objids = build_objstorage()
 
-    with pytest.raises(exc.ObjNotFoundError):
+    with pytest.raises(ObjNotFoundError):
         sto_front.get(b"\x00" * 20)
 
 
 @pytest.mark.parametrize("multi_hash", [False, True])
 def test_http_objstorage_check(multi_hash):
     sto_front, sto_back, objids = build_objstorage(multi_hash)
     for objid in objids:
         assert sto_front.check(objid) is None  # no Exception means OK
 
     # create an invalid object in the in-memory objstorage
     invalid_content = b"p0wn3d content"
-    fake_objid = "\x01" * 20
+    fake_objid = b"\x01" * 20
     sto_back.add(invalid_content, fake_objid)
 
     # the http objstorage should report it as invalid
-    with pytest.raises(exc.Error):
+    with pytest.raises(ObjCorruptedError):
         sto_front.check(fake_objid)
 
 
 def test_http_objstorage_read_only():
     sto_front, sto_back, objids = build_objstorage()
 
     content = b""
     obj_id = compute_hash(content)
-    with pytest.raises(exc.ReadOnlyObjStorage):
+    with pytest.raises(ReadOnlyObjStorage):
         sto_front.add(content, obj_id=obj_id)
-    with pytest.raises(exc.ReadOnlyObjStorage):
+    with pytest.raises(ReadOnlyObjStorage):
         sto_front.restore(b"", obj_id=compute_hash(b""))
-    with pytest.raises(exc.ReadOnlyObjStorage):
+    with pytest.raises(ReadOnlyObjStorage):
         sto_front.delete(b"\x00" * 20)
 
 
 def test_http_objstorage_not_iterable():
     sto_front, sto_back, objids = build_objstorage()
 
-    with pytest.raises(exc.NonIterableObjStorage):
+    with pytest.raises(NonIterableObjStorage):
         len(sto_front)
-    with pytest.raises(exc.NonIterableObjStorage):
+    with pytest.raises(NonIterableObjStorage):
         iter(sto_front)
 
 
 def test_http_cannonical_url():
     url = "http://127.0.0.1/content"
     sto = get_objstorage(cls="http", url=url)
     assert sto.root_path == url + "/"
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_instantiation.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_instantiation.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_multiplexer.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_multiplexer.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_noop.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_noop.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_pathslicing.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_pathslicing.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 
 import pytest
 
 from swh.model import hashutil
-from swh.objstorage import exc
 from swh.objstorage.constants import ID_DIGEST_LENGTH
+from swh.objstorage.exc import ObjCorruptedError
 
 from .objstorage_testing import ObjStorageTestFixture
 
 
 class TestPathSlicingObjStorage(ObjStorageTestFixture):
     compression = "none"
 
@@ -41,25 +41,20 @@
         self.storage.add(content, obj_id=obj_id)
         assert len(self.storage) == 1
 
     def test_check_ok(self):
         content, obj_id = self.hash_content(b"check_ok")
         self.storage.add(content, obj_id=obj_id)
         assert self.storage.check(obj_id) is None
-        assert self.storage.check(obj_id.hex()) is None
 
     def test_check_id_mismatch(self):
-        content, obj_id = self.hash_content(b"check_id_mismatch")
+        _, obj_id = self.hash_content(b"check_id_mismatch")
         self.storage.add(b"unexpected content", obj_id=obj_id)
-        with pytest.raises(exc.Error) as error:
+        with pytest.raises(ObjCorruptedError, match="Object corrupted"):
             self.storage.check(obj_id)
-        assert (
-            "Corrupt object %s should have id "
-            "12ebb2d6c81395bcc5cab965bdff640110cb67ff" % obj_id.hex(),
-        ) == error.value.args
 
     def test_iterate_from(self):
         all_ids = []
         for i in range(100):
             content, obj_id = self.hash_content(b"content %d" % i)
             self.storage.add(content, obj_id=obj_id)
             all_ids.append({self.storage.PRIMARY_HASH: obj_id})
@@ -113,26 +108,34 @@
         patched = mocker.patch.multiple(
             "os", fsync=mocker.DEFAULT, fdatasync=mocker.DEFAULT
         )
         self.storage.add(content, obj_id=obj_id)
         assert patched["fdatasync"].call_count == 0
         assert patched["fsync"].call_count == 1
 
-    def test_check_not_compressed(self):
+    def test_check_not_compressed_trailing_data(self):
         content, obj_id = self.hash_content(b"check_not_compressed")
         self.storage.add(content, obj_id=obj_id)
         with open(self.content_path(obj_id), "ab") as f:  # Add garbage.
             f.write(b"garbage")
-        with pytest.raises(exc.Error) as error:
+        with pytest.raises(ObjCorruptedError, match="Object corrupted") as error:
             self.storage.check(obj_id)
-        if self.compression == "none":
-            assert "Corrupt object" in error.value.args[0]
-        else:
+        if self.compression != "none":
             assert "trailing data found" in error.value.args[0]
 
+    def test_check_not_compressed(self):
+        content, obj_id = self.hash_content(b"check_not_compressed")
+        self.storage.add(content, obj_id=obj_id)
+        with open(self.content_path(obj_id), "wb") as f:  # Replace by garbage.
+            f.write(b"garbage")
+        with pytest.raises(ObjCorruptedError, match="Object corrupted") as error:
+            self.storage.check(obj_id)
+        if self.compression != "none":
+            assert "not a proper compressed file" in error.value.args[0]
+
 
 class TestPathSlicingObjStorageGzip(TestPathSlicingObjStorage):
     compression = "gzip"
 
 
 @pytest.mark.all_compression_methods
 class TestPathSlicingObjStorageZlib(TestPathSlicingObjStorage):
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_random_generator.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_random_generator.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_seaweedfs.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_seaweedfs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 import pytest
 from requests.utils import get_encoding_from_headers
 import requests_mock
 from requests_mock.contrib import fixture
 
 from swh.objstorage.backends.pathslicing import PathSlicer
-from swh.objstorage.exc import Error
-from swh.objstorage.objstorage import compressors, compute_hash, decompressors
+from swh.objstorage.exc import ObjCorruptedError
+from swh.objstorage.objstorage import compute_hash, decompressors
 from swh.objstorage.tests.objstorage_testing import ObjStorageTestFixture
 
 
 class PathDict:
     """A dict-like object that handles "path-like" keys in a recursive dict
     structure.
 
@@ -239,25 +239,21 @@
             "slicing": self.slicing,
         }
 
     def fill_objstorage(self, num_objects):
         # override default implelentation to speed things up a bit, shortcuting
         # the HTTP request path to put objects directly in the objstorage
         # mocker.
-        def compressor(data):
-            comp = compressors[self.compression]()
-            yield comp.compress(data)
-            yield comp.flush()
 
         path = self.storage._path
         all_ids = []
         for i in range(num_objects):
             content = b"content %d" % i
             obj_id = compute_hash(content)
-            self.mock.content[path(obj_id)] = b"".join(compressor(content))
+            self.mock.content[path(obj_id)] = self.storage.compress(content)
             all_ids.append({"sha1": obj_id})
         all_ids.sort(key=lambda d: d["sha1"])
         return all_ids
 
     def test_compression(self):
         content, obj_id = self.hash_content(b"test compression")
         self.storage.add(content, obj_id=obj_id)
@@ -274,21 +270,19 @@
     def test_trailing_data_on_stored_blob(self):
         content, obj_id = self.hash_content(b"test content without garbage")
         self.storage.add(content, obj_id=obj_id)
 
         path = self.storage._path(obj_id)
         self.mock.content[path] += b"trailing garbage"
 
-        if self.compression == "none":
-            with pytest.raises(Error) as e:
-                self.storage.check(obj_id)
-        else:
-            with pytest.raises(Error) as e:
-                self.storage.get(obj_id)
-            assert "trailing data" in e.value.args[0]
+        with pytest.raises(ObjCorruptedError) as e:
+            self.storage.check(obj_id)
+
+        if self.compression != "none":
+            assert "trailing data found" in e.value.args[0]
 
     def test_slicing(self):
         slicer = PathSlicer(urlparse(self.url).path, self.slicing)
         for i in range(20):
             content, obj_id = self.hash_content(b"test slicing %i" % i)
             self.storage.add(content, obj_id=obj_id)
             assert slicer.get_path(obj_id.hex()) in self.mock.content
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_objstorage_winery.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_objstorage_winery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2023  The Software Heritage developers
+# Copyright (C) 2021-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import Counter
 from dataclasses import asdict, dataclass
 import datetime
@@ -12,15 +12,14 @@
 import time
 from typing import Any, Dict
 
 from click.testing import CliRunner
 import pytest
 import yaml
 
-from swh.objstorage import exc
 from swh.objstorage.backends.winery.database import DatabaseAdmin
 from swh.objstorage.backends.winery.objstorage import (
     cleanup_rw_shard,
     deleted_objects_cleaner,
     pack,
     rw_shard_cleaner,
     shard_packer,
@@ -32,14 +31,15 @@
 from swh.objstorage.backends.winery.throttler import (
     BandwidthCalculator,
     IOThrottler,
     LeakyBucket,
     Throttler,
 )
 from swh.objstorage.cli import swh_cli_group
+from swh.objstorage.exc import ObjNotFoundError
 from swh.objstorage.factory import get_objstorage
 from swh.objstorage.objstorage import compute_hash
 from swh.objstorage.utils import call_async
 
 from .winery_benchmark import (
     Bench,
     PackWorker,
@@ -247,15 +247,15 @@
         == "866878b165607851782d8d233edf0c261172ff67926330d3bbd10c705b92d24f"
     )
     winery.add(content=content, obj_id=obj_id)
     winery.add(content=content, obj_id=obj_id)
     winery.add(content=content, obj_id=obj_id, check_presence=False)
     assert winery.base.locked_shard == shard
     assert winery.get(obj_id) == content
-    with pytest.raises(exc.ObjNotFoundError):
+    with pytest.raises(ObjNotFoundError):
         winery.get(b"unknown")
     winery.shard.drop()
 
 
 @pytest.mark.shard_max_size(1)
 def test_winery_add_and_pack(winery, mocker):
     mocker.patch("swh.objstorage.backends.winery.objstorage.pack", return_value=True)
@@ -273,15 +273,15 @@
     shard = winery.base.locked_shard
     content = b"SOMETHING"
     obj_id = compute_hash(content, "sha256")
     winery.add(content=content, obj_id=obj_id)
     assert winery.base.locked_shard == shard
     assert winery.get(obj_id) == content
     winery.delete(obj_id)
-    with pytest.raises(exc.ObjNotFoundError):
+    with pytest.raises(ObjNotFoundError):
         winery.get(obj_id)
 
 
 @pytest.mark.shard_max_size(1)
 @pytest.mark.pack_immediately(True)
 def test_winery_delete_on_roshard(winery, file_backed_pool):
     shard = winery.base.locked_shard
@@ -293,15 +293,15 @@
     for packer in winery.packers:
         packer.join()
     assert winery.get(obj_id) == content
     # This will only mark as deleted in SharedBase
     winery.delete(obj_id)
     assert len(list(winery.base.deleted_objects())) == 1
     # We still should not be able to access it
-    with pytest.raises(exc.ObjNotFoundError):
+    with pytest.raises(ObjNotFoundError):
         winery.get(obj_id)
     # The content is still present in the roshard image at this point
     image_path = file_backed_pool.image_path(shard)
     with open(image_path, "rb") as image:
         assert b"SOMETHING" in image.read()
     # Perform cleanup
     file_backed_pool.image_unmap(shard)
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_pathslicer.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_pathslicer.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_readonly_filter.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_readonly_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # See top-level LICENSE file for more information
 
 import random
 from string import ascii_lowercase
 
 import pytest
 
-from swh.objstorage.exc import Error, ObjNotFoundError
+from swh.objstorage.exc import ObjCorruptedError, ObjNotFoundError
 from swh.objstorage.factory import get_objstorage
 from swh.objstorage.multiplexer.filter import read_only
 from swh.objstorage.objstorage import compute_hash
 
 
 def get_random_content():
     return bytes("".join(random.sample(ascii_lowercase, 10)), "utf8")
@@ -60,15 +60,15 @@
     def test_can_get(self):
         assert self.valid_content == self.storage.get(self.valid_id)
         assert self.invalid_content == self.storage.get(self.invalid_id)
 
     def test_can_check(self):
         with pytest.raises(ObjNotFoundError):
             self.storage.check(self.absent_id)
-        with pytest.raises(Error):
+        with pytest.raises(ObjCorruptedError):
             self.storage.check(self.invalid_id)
         self.storage.check(self.valid_id)
 
     def test_cannot_add(self):
         new_id = self.storage.add(b"New content")
         result = self.storage.add(self.valid_content, self.valid_id)
         assert new_id is None
```

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/test_server.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/winery_benchmark.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/winery_benchmark.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/tests/winery_testing_helpers.py` & `swh.objstorage-2.9.2/swh/objstorage/tests/winery_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh/objstorage/utils.py` & `swh.objstorage-2.9.2/swh/objstorage/utils.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/swh.objstorage.egg-info/PKG-INFO` & `swh.objstorage-2.9.2/swh.objstorage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 2.9.1
+Version: 2.9.2
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
@@ -29,15 +29,15 @@
 Provides-Extra: libcloud
 Requires-Dist: apache-libcloud; extra == "libcloud"
 Provides-Extra: winery
 Requires-Dist: psycopg[c,pool]; extra == "winery"
 Requires-Dist: systemd-python; extra == "winery"
 Provides-Extra: testing
 Requires-Dist: moto[s3,server]<5; extra == "testing"
-Requires-Dist: pytest; extra == "testing"
+Requires-Dist: pytest>=8.1; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
 Requires-Dist: requests_mock[fixture]>=1.9; extra == "testing"
 Requires-Dist: requests_toolbelt; extra == "testing"
 Requires-Dist: swh.core[testing]>=3.0.0; extra == "testing"
 Requires-Dist: types-pyyaml; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
 Requires-Dist: pytest-postgresql>5; extra == "testing"
```

### Comparing `swh.objstorage-2.9.1/swh.objstorage.egg-info/SOURCES.txt` & `swh.objstorage-2.9.2/swh.objstorage.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 AUTHORS
 CODE_OF_CONDUCT.md
 CONTRIBUTORS
 LICENSE
 Makefile
 Makefile.local
 README.rst
+conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 requirements-azure.txt
 requirements-libcloud.txt
 requirements-swh.txt
 requirements-test.txt
@@ -42,14 +43,15 @@
 swh/objstorage/interface.py
 swh/objstorage/objstorage.py
 swh/objstorage/py.typed
 swh/objstorage/pytest_plugin.py
 swh/objstorage/utils.py
 swh/objstorage/api/client.py
 swh/objstorage/api/server.py
+swh/objstorage/backends/__init__.py
 swh/objstorage/backends/azure.py
 swh/objstorage/backends/generator.py
 swh/objstorage/backends/http.py
 swh/objstorage/backends/in_memory.py
 swh/objstorage/backends/libcloud.py
 swh/objstorage/backends/noop.py
 swh/objstorage/backends/pathslicing.py
@@ -66,15 +68,15 @@
 swh/objstorage/backends/winery/stats.py
 swh/objstorage/backends/winery/throttler.py
 swh/objstorage/multiplexer/__init__.py
 swh/objstorage/multiplexer/multiplexer_objstorage.py
 swh/objstorage/multiplexer/filter/__init__.py
 swh/objstorage/multiplexer/filter/filter.py
 swh/objstorage/multiplexer/filter/read_write_filter.py
-swh/objstorage/tests/conftest.py
+swh/objstorage/tests/__init__.py
 swh/objstorage/tests/objstorage_testing.py
 swh/objstorage/tests/test_interface.py
 swh/objstorage/tests/test_objstorage_api.py
 swh/objstorage/tests/test_objstorage_azure.py
 swh/objstorage/tests/test_objstorage_cloud.py
 swh/objstorage/tests/test_objstorage_http.py
 swh/objstorage/tests/test_objstorage_in_memory.py
```

### Comparing `swh.objstorage-2.9.1/tox.ini` & `swh.objstorage-2.9.2/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -4,32 +4,28 @@
   black
   flake8
   mypy
   py3
   winery
 
 [testenv]
+usedevelop = true
 extras =
   testing
 passenv =
   AZURITE_PATH
   USE_CEPH
 deps =
   pytest-cov
 commands =
   pytest --doctest-modules \
-         --rootdir {envsitepackagesdir} \
-         --cov={envsitepackagesdir}/swh/objstorage \
+         --cov=swh/objstorage \
          --cov-branch \
-         --cov-report term-missing \
-         {envsitepackagesdir}/swh/objstorage \
+         swh/objstorage \
          {posargs}
-# --rootdir (with --import-mode from pytest.ini) are required to make tests
-# that depends on the test file to be a proper submodule of the swh namespace
-# after migration to PEP420 (implicit namespace).
 
 [testenv:winery]
 allowlist_externals = bash
 passenv = *
 commands =
   bash {toxinidir}/winery-test-environment/remote-tox.sh {posargs}
```

### Comparing `swh.objstorage-2.9.1/winery-test-environment/README.md` & `swh.objstorage-2.9.2/winery-test-environment/README.md`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/bootstrap.yml` & `swh.objstorage-2.9.2/winery-test-environment/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/build-vms.sh` & `swh.objstorage-2.9.2/winery-test-environment/build-vms.sh`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/ceph.yml` & `swh.objstorage-2.9.2/winery-test-environment/ceph.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/fed4fire.rspec` & `swh.objstorage-2.9.2/winery-test-environment/fed4fire.rspec`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/fed4fire.sh` & `swh.objstorage-2.9.2/winery-test-environment/fed4fire.sh`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/grid5000.yml` & `swh.objstorage-2.9.2/winery-test-environment/grid5000.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/inventory/hosts.yml` & `swh.objstorage-2.9.2/winery-test-environment/inventory/hosts.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/mitogen.py` & `swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/mitogen_free.py` & `swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py` & `swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/mitogen-strategy/mitogen_linear.py` & `swh.objstorage-2.9.2/winery-test-environment/mitogen-strategy/mitogen_linear.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/osd.yml` & `swh.objstorage-2.9.2/winery-test-environment/osd.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/remote-tox.sh` & `swh.objstorage-2.9.2/winery-test-environment/remote-tox.sh`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/render-stats.py` & `swh.objstorage-2.9.2/winery-test-environment/render-stats.py`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/rw.yml` & `swh.objstorage-2.9.2/winery-test-environment/rw.yml`

 * *Files identical despite different names*

### Comparing `swh.objstorage-2.9.1/winery-test-environment/tests.yml` & `swh.objstorage-2.9.2/winery-test-environment/tests.yml`

 * *Files identical despite different names*

