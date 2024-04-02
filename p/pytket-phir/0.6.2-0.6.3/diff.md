# Comparing `tmp/pytket-phir-0.6.2.tar.gz` & `tmp/pytket-phir-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytket-phir-0.6.2.tar", last modified: Wed Mar 27 19:49:08 2024, max compression
+gzip compressed data, was "pytket-phir-0.6.3.tar", last modified: Tue Apr  2 14:50:35 2024, max compression
```

## Comparing `pytket-phir-0.6.2.tar` & `pytket-phir-0.6.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.626425 pytket-phir-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.614425 pytket-phir-0.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.614425 pytket-phir-0.6.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.614425 pytket-phir-0.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/.github/workflows/pre-commit-au.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/.github/workflows/python-app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-03-27 19:49:08.626425 pytket-phir-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.614425 pytket-phir-0.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.618425 pytket-phir-0.6.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/docs/source/pytket.phir.rebasing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/docs/source/pytket.phir.rst
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/docs/source/pytket.phir.sharding.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.614425 pytket-phir-0.6.2/pytket/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.618425 pytket-phir-0.6.2/pytket/phir/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    14306 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/phirgen.py
--rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/phirgen_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/place_and_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/placement.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/qtm_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.618425 pytket-phir-0.6.2/pytket/phir/rebasing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/rebasing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/rebasing/rebaser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/routing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.618425 pytket-phir-0.6.2/pytket/phir/sharding/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/sharding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/sharding/shard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/sharding/sharder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/pytket/phir/sharding/shards2ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.626425 pytket-phir-0.6.2/pytket_phir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-03-27 19:49:08.000000 pytket-phir-0.6.2/pytket_phir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-03-27 19:49:08.000000 pytket-phir-0.6.2/pytket_phir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:49:08.000000 pytket-phir-0.6.2/pytket_phir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-27 19:49:08.000000 pytket-phir-0.6.2/pytket_phir.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-27 19:49:08.000000 pytket-phir-0.6.2/pytket_phir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 19:49:08.000000 pytket-phir-0.6.2/pytket_phir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:49:08.626425 pytket-phir-0.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.622425 pytket-phir-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.614425 pytket-phir-0.6.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.626425 pytket-phir-0.6.2/tests/data/qasm/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/arbitrary_qreg_names.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/baby.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/baby_with_rollup.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/barrier_complex.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/big_gate.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/bv_n10.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/classical_hazards.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/classical_ordering.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/cond_1.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/cond_barrier.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/cond_classical.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/exec_order_two_qubits.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/eztest.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/group_ordering.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/n10_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/oned_brickwork_circuit_n20.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/parallelization_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)    81132 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/qv20_0.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/rxrz.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/rz_exec_order_three_qubits.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/simple.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/simple_cond.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/single_qubit_parallel_test.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/sleep.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/tk2_diff_angles.qasm
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/qasm/tk2_same_angle.qasm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:49:08.626425 pytket-phir-0.6.2/tests/data/wasm/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/wasm/add.wat
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/data/wasm/testfile.wat
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/e2e_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/test_parallel_tk2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/test_parallelization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5942 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/test_phirgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/test_placement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/test_rebaser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/test_sharder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-03-27 19:49:03.000000 pytket-phir-0.6.2/tests/test_wasm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/workflows/pre-commit-au.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/workflows/python-app.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.127381 pytket-phir-0.6.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/pytket.phir.rebasing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/pytket.phir.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/docs/source/pytket.phir.sharding.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.123381 pytket-phir-0.6.3/pytket/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.131381 pytket-phir-0.6.3/pytket/phir/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14653 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/phirgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15216 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/phirgen_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/place_and_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/qtm_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.131381 pytket-phir-0.6.3/pytket/phir/rebasing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/rebasing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/rebasing/rebaser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/routing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.131381 pytket-phir-0.6.3/pytket/phir/sharding/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/sharding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/sharding/shard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9939 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/sharding/sharder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/pytket/phir/sharding/shards2ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/pytket_phir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 14:50:35.000000 pytket-phir-0.6.3/pytket_phir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.135382 pytket-phir-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.123381 pytket-phir-0.6.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/tests/data/qasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/arbitrary_qreg_names.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/baby.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/baby_with_rollup.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/barrier_complex.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/big_gate.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/bv_n10.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/classical_hazards.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/classical_ordering.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/cond_1.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/cond_barrier.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/cond_classical.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/exec_order_two_qubits.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/eztest.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/group_ordering.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/n10_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/oned_brickwork_circuit_n20.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/parallelization_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)    81132 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/qv20_0.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/rxrz.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/rz_exec_order_three_qubits.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/simple.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/simple_cond.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/single_qubit_parallel_test.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/sleep.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/tk2_diff_angles.qasm
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/qasm/tk2_same_angle.qasm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:50:35.139382 pytket-phir-0.6.3/tests/data/wasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/wasm/add.wat
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/data/wasm/testfile.wat
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/e2e_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_parallel_tk2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_parallelization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_phirgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_rebaser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16148 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_sharder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-02 14:50:30.000000 pytket-phir-0.6.3/tests/test_wasm.py
```

### Comparing `pytket-phir-0.6.2/.github/ISSUE_TEMPLATE/feature_request.md` & `pytket-phir-0.6.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/.github/pull_request_template.md` & `pytket-phir-0.6.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/.github/workflows/pre-commit-au.yml` & `pytket-phir-0.6.3/.github/workflows/pre-commit-au.yml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/.github/workflows/python-app.yml` & `pytket-phir-0.6.3/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/.github/workflows/python-publish.yml` & `pytket-phir-0.6.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/.gitignore` & `pytket-phir-0.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/CHANGELOG.md` & `pytket-phir-0.6.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.6.3] - 2024-04-02
+
+### Fixed
+
+* wasm/phirgen: correct arguments for conditional wasm functions in https://github.com/CQCL/pytket-phir/pull/157
+
+## [0.6.2] - 2024-03-27
+
+### Fixed
+
+* phirgen: don't rely on args when qubits carries correct info in https://github.com/CQCL/pytket-phir/pull/155
+
 ## [0.6.1] - 2024-03-26
 
 ### Fixed
 
 * Remove unneeded logic for comments for conditionals in https://github.com/CQCL/pytket-phir/pull/152
   * Fixes `make_comment_text` repeats the condition for conditional ops (https://github.com/CQCL/pytket-phir/issues/149)
 * Invalid reordering of operations involving classical bits in https://github.com/CQCL/pytket-phir/pull/151
@@ -153,10 +165,12 @@
 [0.4.2]: https://github.com/CQCL/pytket-phir/compare/v0.4.1...v0.4.2
 [0.4.3]: https://github.com/CQCL/pytket-phir/compare/v0.4.2...v0.4.3
 [0.4.4]: https://github.com/CQCL/pytket-phir/compare/v0.4.3...v0.4.4
 [0.5.0]: https://github.com/CQCL/pytket-phir/compare/v0.4.4...v0.5.0
 [0.5.1]: https://github.com/CQCL/pytket-phir/compare/v0.5.0...v0.5.1
 [0.6.0]: https://github.com/CQCL/pytket-phir/compare/v0.5.1...v0.6.0
 [0.6.1]: https://github.com/CQCL/pytket-phir/compare/v0.6.0...v0.6.1
-[unreleased]: https://github.com/CQCL/pytket-phir/compare/v0.6.1...HEAD
+[0.6.2]: https://github.com/CQCL/pytket-phir/compare/v0.6.1...v0.6.2
+[0.6.3]: https://github.com/CQCL/pytket-phir/compare/v0.6.2...v0.6.3
+[unreleased]: https://github.com/CQCL/pytket-phir/compare/v0.6.3...HEAD
 
 <!-- markdownlint-configure-file {"MD024": {"siblings_only" : true}, "MD034": false} -->
```

### Comparing `pytket-phir-0.6.2/LICENSE` & `pytket-phir-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/PKG-INFO` & `pytket-phir-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-phir
-Version: 0.6.2
+Version: 0.6.3
 Summary: A circuit analyzer and translator from pytket to PHIR
 Author: Quantinuum
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pytket-phir-0.6.2/README.md` & `pytket-phir-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/docs/Makefile` & `pytket-phir-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/docs/source/conf.py` & `pytket-phir-0.6.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/docs/source/index.rst` & `pytket-phir-0.6.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/docs/source/pytket.phir.rst` & `pytket-phir-0.6.3/docs/source/pytket.phir.rst`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/docs/source/pytket.phir.sharding.rst` & `pytket-phir-0.6.3/docs/source/pytket.phir.sharding.rst`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pyproject.toml` & `pytket-phir-0.6.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -61,7 +61,10 @@
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.setuptools_scm]
 version_scheme = "python-simplified-semver"
 
 [tool.refurb]
 python_version = "3.10"
+
+[tool.typos]
+default.extend-words = { lst = "lst" }
```

### Comparing `pytket-phir-0.6.2/pytket/phir/api.py` & `pytket-phir-0.6.3/pytket/phir/api.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/cli.py` & `pytket-phir-0.6.3/pytket/phir/cli.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/machine.py` & `pytket-phir-0.6.3/pytket/phir/machine.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/phirgen.py` & `pytket-phir-0.6.3/pytket/phir/phirgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,19 +226,19 @@
     out: JsonDict | None = None
     match op:  # non-quantum op
         case tk.BarrierOp():
             if op.data:
                 # See https://github.com/CQCL/tket/blob/0ec603986821d994caa3a0fb9c4640e5bc6c0a24/pytket/pytket/qasm/qasm.py#L419-L459
                 match op.data[0:5]:
                     case "sleep":
-                        dur = op.data.removeprefix("sleep(").removesuffix(")")
+                        duration = op.data.removeprefix("sleep(").removesuffix(")")
                         out = {
                             "mop": "Idle",
                             "args": [arg_to_bit(qbit) for qbit in cmd.qubits],
-                            "duration": (float(dur), "s"),
+                            "duration": (float(duration), "s"),
                         }
                     case "order" | "group":
                         raise NotImplementedError(op.data)
                     case _:
                         raise TypeError(op.data)
             else:
                 out = {
@@ -353,35 +353,46 @@
 
 
 def extract_wasm_args_and_returns(
     command: tk.Command, op: tk.WASMOp
 ) -> tuple[list[str], list[str]]:
     """Extract the wasm args and return values as whole register names."""
     # This slice removes the extra `_w` cregs (wires) that are not part of the
-    # circuit, and the output args which are appended after the input args
+    # circuit and the output args, which are appended after the input args
     slice_index = op.num_w + sum(op.output_widths)
     only_args = command.args[:-slice_index]
+    # Eliminate conditional bits from the front of the args
+    input_args = only_args[len(only_args) - op.n_inputs :]
     return (
-        dedupe_bits_to_registers(only_args),
+        dedupe_bits_to_registers(input_args),
         dedupe_bits_to_registers(command.bits),
     )
 
 
 def dedupe_bits_to_registers(bits: "Sequence[UnitID]") -> list[str]:
     """Dedupes a list of bits to their registers, keeping order intact."""
     return list(dict.fromkeys([bit.reg_name for bit in bits]))
 
 
 def make_comment_text(cmd: tk.Command, op: tk.Op) -> str:
     """Converts a command + op to the PHIR comment spec."""
     comment = str(cmd)
     match op:
+        case tk.Conditional():
+            conditional_text = str(cmd)
+            cleaned = (
+                conditional_text[: conditional_text.find("THEN") + 5]
+                if isinstance(op.op, tk.WASMOp)
+                else ""
+            )
+            comment = f"{cleaned}{make_comment_text(cmd, op.op)}"
+
         case tk.WASMOp():
             args, returns = extract_wasm_args_and_returns(cmd, op)
-            comment = f"WASM function={op.func_name} args={args} returns={returns}"
+            comment = f"WASM_function='{op.func_name}' args={args} returns={returns};"
 
         case tk.BarrierOp():
             comment = op.data + " " + str(cmd.args[0]) + ";" if op.data else str(cmd)
 
         case tk.ClassicalExpBox():
             exp = op.get_exp()
             match exp:
@@ -391,16 +402,14 @@
                     comment = str(cmd.bits[0].reg_name) + " = " + str(op.get_exp())
 
     return comment
 
 
 def get_decls(qbits: set["Qubit"], cbits: set[tkBit]) -> list[dict[str, str | int]]:
     """Format the qvar and cvar define PHIR elements."""
-    # TODO(kartik): this may not always be accurate
-    # https://github.com/CQCL/pytket-phir/issues/24
     qvar_dim: dict[str, int] = {}
     for qbit in qbits:
         qvar_dim.setdefault(qbit.reg_name, 0)
         qvar_dim[qbit.reg_name] += 1
 
     cvar_dim: dict[str, int] = {}
     for cbit in cbits:
```

### Comparing `pytket-phir-0.6.2/pytket/phir/phirgen_parallel.py` & `pytket-phir-0.6.3/pytket/phir/phirgen_parallel.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/place_and_route.py` & `pytket-phir-0.6.3/pytket/phir/place_and_route.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/placement.py` & `pytket-phir-0.6.3/pytket/phir/placement.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/qtm_machine.py` & `pytket-phir-0.6.3/pytket/phir/qtm_machine.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/rebasing/rebaser.py` & `pytket-phir-0.6.3/pytket/phir/rebasing/rebaser.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/routing.py` & `pytket-phir-0.6.3/pytket/phir/routing.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/sharding/shard.py` & `pytket-phir-0.6.3/pytket/phir/sharding/shard.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/sharding/sharder.py` & `pytket-phir-0.6.3/pytket/phir/sharding/sharder.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket/phir/sharding/shards2ops.py` & `pytket-phir-0.6.3/pytket/phir/sharding/shards2ops.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/pytket_phir.egg-info/PKG-INFO` & `pytket-phir-0.6.3/pytket_phir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-phir
-Version: 0.6.2
+Version: 0.6.3
 Summary: A circuit analyzer and translator from pytket to PHIR
 Author: Quantinuum
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, Quantinuum LLC
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `pytket-phir-0.6.2/pytket_phir.egg-info/SOURCES.txt` & `pytket-phir-0.6.3/pytket_phir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/data/qasm/arbitrary_qreg_names.qasm` & `pytket-phir-0.6.3/tests/data/qasm/arbitrary_qreg_names.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/data/qasm/bv_n10.qasm` & `pytket-phir-0.6.3/tests/data/qasm/bv_n10.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/data/qasm/oned_brickwork_circuit_n20.qasm` & `pytket-phir-0.6.3/tests/data/qasm/oned_brickwork_circuit_n20.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/data/qasm/qv20_0.qasm` & `pytket-phir-0.6.3/tests/data/qasm/qv20_0.qasm`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/data/wasm/add.wat` & `pytket-phir-0.6.3/tests/data/wasm/add.wat`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/data/wasm/testfile.wat` & `pytket-phir-0.6.3/tests/data/wasm/testfile.wat`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/e2e_test.py` & `pytket-phir-0.6.3/tests/e2e_test.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/test_api.py` & `pytket-phir-0.6.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/test_parallel_tk2.py` & `pytket-phir-0.6.3/tests/test_parallel_tk2.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/test_parallelization.py` & `pytket-phir-0.6.3/tests/test_parallelization.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,26 +60,26 @@
 
 
 def test_parallel_subcommand_relative_ordering() -> None:
     """Make sure the proper relative ordering of sub-commands is preserved."""
     phir = get_phir_json(QasmFile.rxrz, rebase=True)
     # make sure it is ordered like the qasm file
     ops = phir["ops"]
-    frst_sc = ops[3]
-    scnd_sc = ops[5]
-    thrd_sc = ops[7]
-    frth_sc = ops[9]
-    assert frst_sc["qop"] == "RZ"
-    assert frst_sc["angles"] == [[0.5], "pi"]
-    assert scnd_sc["qop"] == "R1XY"
-    assert scnd_sc["angles"] == [[3.5, 0.0], "pi"]
-    assert thrd_sc["qop"] == "R1XY"
-    assert thrd_sc["angles"] == [[0.5, 0.0], "pi"]
-    assert frth_sc["qop"] == "RZ"
-    assert frth_sc["angles"] == [[3.5], "pi"]
+    sc1 = ops[3]
+    sc2 = ops[5]
+    sc3 = ops[7]
+    sc4 = ops[9]
+    assert sc1["qop"] == "RZ"
+    assert sc1["angles"] == [[0.5], "pi"]
+    assert sc2["qop"] == "R1XY"
+    assert sc2["angles"] == [[3.5, 0.0], "pi"]
+    assert sc3["qop"] == "R1XY"
+    assert sc3["angles"] == [[0.5, 0.0], "pi"]
+    assert sc4["qop"] == "RZ"
+    assert sc4["angles"] == [[3.5], "pi"]
 
 
 def test_single_qubit_circuit_with_parallel() -> None:
     """Make sure there are no parallel blocks present in the 1qubit circuit."""
     phir_with_parallel_phirgen = get_phir_json(
         QasmFile.single_qubit_parallel_test, rebase=True
     )
```

### Comparing `pytket-phir-0.6.2/tests/test_phirgen.py` & `pytket-phir-0.6.3/tests/test_phirgen.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,26 @@
     assert phir["ops"][5] == {
         "block": "if",
         "condition": {"cop": "==", "args": ["m", 0]},
         "true_branch": [{"meta": "barrier", "args": [["q", 0], ["q", 1]]}],
     }
 
 
+def test_simple_cond_classical() -> None:
+    """Ensure conditional classical operation are correctly generated."""
+    circ = get_qasm_as_circuit(QasmFile.simple_cond)
+    phir = json.loads(pytket_to_phir(circ))
+    assert phir["ops"][-6] == {"//": "IF ([c[0]] == 1) THEN SetBits(1) z[0];"}
+    assert phir["ops"][-5] == {
+        "block": "if",
+        "condition": {"cop": "==", "args": [["c", 0], 1]},
+        "true_branch": [{"cop": "=", "returns": [["z", 0]], "args": [1]}],
+    }
+
+
 def test_nested_bitwise_op() -> None:
     """From https://github.com/CQCL/pytket-phir/issues/133 ."""
     circ = Circuit(4)
     a = circ.add_c_register("a", 4)
     b = circ.add_c_register("b", 1)
     circ.add_classicalexpbox_bit(a[0] ^ a[1] ^ a[2] ^ a[3], [b[0]])
 
@@ -179,12 +191,13 @@
 def test_conditional_measure() -> None:
     """From https://github.com/CQCL/pytket-phir/issues/154 ."""
     c = Circuit(2, 2)
     c.H(0).H(1)
     c.Measure(0, 0)
     c.Measure(1, 1, condition_bits=[0], condition_value=1)
     phir = json.loads(pytket_to_phir(c))
+    assert phir["ops"][-2] == {"//": "IF ([c[0]] == 1) THEN Measure q[1] --> c[1];"}
     assert phir["ops"][-1] == {
         "block": "if",
         "condition": {"cop": "==", "args": [["c", 0], 1]},
         "true_branch": [{"qop": "Measure", "returns": [["c", 1]], "args": [["q", 1]]}],
     }
```

### Comparing `pytket-phir-0.6.2/tests/test_placement.py` & `pytket-phir-0.6.3/tests/test_placement.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/test_rebaser.py` & `pytket-phir-0.6.3/tests/test_rebaser.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/test_sharder.py` & `pytket-phir-0.6.3/tests/test_sharder.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/test_utils.py` & `pytket-phir-0.6.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pytket-phir-0.6.2/tests/test_wasm.py` & `pytket-phir-0.6.3/tests/test_wasm.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,126 +13,167 @@
 import json
 import logging
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 import pytest
 
-from pytket.circuit import Circuit
+from pytket.circuit import Circuit, Qubit
 from pytket.phir.api import pytket_to_phir, qasm_to_phir
 from pytket.phir.qtm_machine import QtmMachine
 from pytket.wasm.wasm import WasmFileHandler
 
 from .test_utils import WatFile, get_wat_as_wasm_bytes
 
 logger = logging.getLogger(__name__)
 
 
-class TestWASM:
-    def test_qasm_to_phir_with_wasm(self) -> None:
-        """Test the qasm string entrypoint works with WASM."""
-        qasm = """
-        OPENQASM 2.0;
-        include "qelib1.inc";
-
-        qreg q[2];
-        h q;
-        ZZ q[1],q[0];
-        creg cr[3];
-        creg cs[3];
-        creg co[3];
-        measure q[0]->cr[0];
-        measure q[1]->cr[1];
-
-        cs = cr;
-        co = add(cr, cs);
-        """
-
-        wasm_bytes = get_wat_as_wasm_bytes(WatFile.add)
-
-        wasm_uid = hashlib.sha256(base64.b64encode(wasm_bytes)).hexdigest()
-
-        phir_str = qasm_to_phir(qasm, QtmMachine.H1, wasm_bytes=wasm_bytes)
-        phir = json.loads(phir_str)
-
-        expected_metadata = {"ff_object": (f"WASM module uid: {wasm_uid}")}
-
-        assert phir["ops"][21] == {
-            "metadata": expected_metadata,
-            "cop": "ffcall",
-            "function": "add",
-            "args": ["cr", "cs"],
-            "returns": ["co"],
-        }
-
-    @pytest.mark.order("first")
-    def test_pytket_with_wasm(self) -> None:
-        wasm_bytes = get_wat_as_wasm_bytes(WatFile.testfile)
-        phir_str: str
-        try:
-            wasm_file = NamedTemporaryFile(suffix=".wasm", delete=False)
-            wasm_file.write(wasm_bytes)
-            wasm_file.flush()
-            wasm_file.close()
-
-            w = WasmFileHandler(wasm_file.name)
-
-            c = Circuit(6, 6)
-            c0 = c.add_c_register("c0", 3)
-            c1 = c.add_c_register("c1", 4)
-            c2 = c.add_c_register("c2", 5)
-
-            c.add_wasm_to_reg("multi", w, [c0, c1], [c2])
-            c.add_wasm_to_reg("add_one", w, [c2], [c2])
-            c.add_wasm_to_reg("no_return", w, [c2], [])
-            c.add_wasm_to_reg("no_parameters", w, [], [c2])
-
-            c.add_wasm_to_reg("add_one", w, [c0], [c0], condition=c1[0])
-
-            phir_str = pytket_to_phir(c, QtmMachine.H1)
-        finally:
-            Path.unlink(Path(wasm_file.name))
-
-        phir = json.loads(phir_str)
-
-        expected_metadata = {"ff_object": (f"WASM module uid: {w!s}")}
-
-        assert phir["ops"][4] == {
-            "metadata": expected_metadata,
-            "cop": "ffcall",
-            "function": "multi",
-            "args": ["c0", "c1"],
-            "returns": ["c2"],
-        }
-        assert phir["ops"][7] == {
-            "metadata": expected_metadata,
-            "cop": "ffcall",
-            "function": "add_one",
-            "args": ["c2"],
-            "returns": ["c2"],
-        }
-        assert phir["ops"][9] == {
-            "block": "if",
-            "condition": {"cop": "==", "args": [["c1", 0], 1]},
-            "true_branch": [
-                {
-                    "metadata": expected_metadata,
-                    "cop": "ffcall",
-                    "returns": ["c0"],
-                    "function": "add_one",
-                    "args": ["c1", "c0"],
-                }
-            ],
-        }
-        assert phir["ops"][12] == {
-            "metadata": expected_metadata,
-            "cop": "ffcall",
-            "function": "no_return",
-            "args": ["c2"],
-        }
-        assert phir["ops"][15] == {
-            "metadata": expected_metadata,
-            "cop": "ffcall",
-            "function": "no_parameters",
-            "args": [],
-            "returns": ["c2"],
-        }
+def test_qasm_to_phir_with_wasm() -> None:
+    """Test the qasm string entrypoint works with WASM."""
+    qasm = """
+    OPENQASM 2.0;
+    include "qelib1.inc";
+
+    qreg q[2];
+    h q;
+    ZZ q[1],q[0];
+    creg cr[3];
+    creg cs[3];
+    creg co[3];
+    measure q[0]->cr[0];
+    measure q[1]->cr[1];
+
+    cs = cr;
+    co = add(cr, cs);
+    """
+
+    wasm_bytes = get_wat_as_wasm_bytes(WatFile.add)
+
+    wasm_uid = hashlib.sha256(base64.b64encode(wasm_bytes)).hexdigest()
+
+    phir_str = qasm_to_phir(qasm, QtmMachine.H1, wasm_bytes=wasm_bytes)
+    phir = json.loads(phir_str)
+
+    expected_metadata = {"ff_object": (f"WASM module uid: {wasm_uid}")}
+
+    assert phir["ops"][21] == {
+        "metadata": expected_metadata,
+        "cop": "ffcall",
+        "function": "add",
+        "args": ["cr", "cs"],
+        "returns": ["co"],
+    }
+
+
+@pytest.mark.order("first")
+def test_pytket_with_wasm() -> None:
+    """Test whether pytket works with WASM."""
+    wasm_bytes = get_wat_as_wasm_bytes(WatFile.testfile)
+    phir_str: str
+    try:
+        wasm_file = NamedTemporaryFile(suffix=".wasm", delete=False)
+        wasm_file.write(wasm_bytes)
+        wasm_file.flush()
+        wasm_file.close()
+
+        w = WasmFileHandler(wasm_file.name)
+
+        c = Circuit(6, 6)
+        c0 = c.add_c_register("c0", 3)
+        c1 = c.add_c_register("c1", 4)
+        c2 = c.add_c_register("c2", 5)
+
+        c.add_wasm_to_reg("multi", w, [c0, c1], [c2])
+        c.add_wasm_to_reg("add_one", w, [c2], [c2])
+        c.add_wasm_to_reg("no_return", w, [c2], [])
+        c.add_wasm_to_reg("no_parameters", w, [], [c2])
+
+        c.add_wasm_to_reg("add_one", w, [c0], [c0], condition=c1[0])
+
+        phir_str = pytket_to_phir(c, QtmMachine.H1)
+    finally:
+        Path.unlink(Path(wasm_file.name))
+
+    phir = json.loads(phir_str)
+
+    expected_metadata = {"ff_object": (f"WASM module uid: {w!s}")}
+
+    assert phir["ops"][4] == {
+        "metadata": expected_metadata,
+        "cop": "ffcall",
+        "function": "multi",
+        "args": ["c0", "c1"],
+        "returns": ["c2"],
+    }
+    assert phir["ops"][7] == {
+        "metadata": expected_metadata,
+        "cop": "ffcall",
+        "function": "add_one",
+        "args": ["c2"],
+        "returns": ["c2"],
+    }
+    assert phir["ops"][8] == {
+        "//": "IF ([c1[0]] == 1) THEN WASM_function='add_one' args=['c0'] returns=['c0'];"  # noqa: E501
+    }
+    assert phir["ops"][9] == {
+        "block": "if",
+        "condition": {"cop": "==", "args": [["c1", 0], 1]},
+        "true_branch": [
+            {
+                "metadata": expected_metadata,
+                "cop": "ffcall",
+                "returns": ["c0"],
+                "function": "add_one",
+                "args": ["c0"],
+            }
+        ],
+    }
+    assert phir["ops"][12] == {
+        "metadata": expected_metadata,
+        "cop": "ffcall",
+        "function": "no_return",
+        "args": ["c2"],
+    }
+    assert phir["ops"][15] == {
+        "metadata": expected_metadata,
+        "cop": "ffcall",
+        "function": "no_parameters",
+        "args": [],
+        "returns": ["c2"],
+    }
+
+
+def test_conditional_wasm() -> None:
+    """From https://github.com/CQCL/pytket-phir/issues/156 ."""
+    wasm_bytes = get_wat_as_wasm_bytes(WatFile.testfile)
+    try:
+        wasm_file = NamedTemporaryFile(suffix=".wasm", delete=False)
+        wasm_file.write(wasm_bytes)
+        wasm_file.flush()
+        wasm_file.close()
+
+        w = WasmFileHandler(wasm_file.name)
+
+        c = Circuit(1)
+        areg = c.add_c_register("a", 2)
+        breg = c.add_c_register("b", 1)
+        c.H(0)
+        c.Measure(Qubit(0), breg[0])
+        c.add_wasm(
+            funcname="add_one",
+            filehandler=w,
+            list_i=[1],
+            list_o=[1],
+            args=[areg[0], areg[1]],
+            args_wasm=[0],
+            condition_bits=[breg[0]],
+            condition_value=1,
+        )
+    finally:
+        Path.unlink(Path(wasm_file.name))
+
+    phir = json.loads(pytket_to_phir(c))
+
+    assert phir["ops"][-2] == {
+        "//": "IF ([b[0]] == 1) THEN WASM_function='add_one' args=['a'] returns=['a'];"
+    }
+    assert phir["ops"][-1]["true_branch"][0]["args"] == ["a"]
```

