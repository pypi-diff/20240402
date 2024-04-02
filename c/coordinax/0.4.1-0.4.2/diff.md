# Comparing `tmp/coordinax-0.4.1.tar.gz` & `tmp/coordinax-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Mar 30 16:16:47 2024, max compression
+gzip compressed data, last modified: Tue Apr  2 19:39:44 2024, max compression
```

## Comparing `coordinax-0.4.1.tar` & `coordinax-0.4.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      373 2024-03-30 16:16:47.000000 coordinax-0.4.1/.copier-answers.yml
--rw-r--r--   0        0        0      125 2024-03-30 16:16:47.000000 coordinax-0.4.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2024-03-30 16:16:47.000000 coordinax-0.4.1/.gitattributes
--rw-r--r--   0        0        0     2558 2024-03-30 16:16:47.000000 coordinax-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2024-03-30 16:16:47.000000 coordinax-0.4.1/.readthedocs.yml
--rw-r--r--   0        0        0      439 2024-03-30 16:16:47.000000 coordinax-0.4.1/conftest.py
--rw-r--r--   0        0        0     2819 2024-03-30 16:16:47.000000 coordinax-0.4.1/noxfile.py
--rw-r--r--   0        0        0     2386 2024-03-30 16:16:47.000000 coordinax-0.4.1/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2024-03-30 16:16:47.000000 coordinax-0.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2024-03-30 16:16:47.000000 coordinax-0.4.1/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1540 2024-03-30 16:16:47.000000 coordinax-0.4.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1655 2024-03-30 16:16:47.000000 coordinax-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      872 2024-03-30 16:16:47.000000 coordinax-0.4.1/docs/conf.py
--rw-r--r--   0        0        0      196 2024-03-30 16:16:47.000000 coordinax-0.4.1/docs/index.md
--rw-r--r--   0        0        0     1261 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/__init__.py
--rw-r--r--   0        0        0    23548 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_base.py
--rw-r--r--   0        0        0     3937 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_base_dif.py
--rw-r--r--   0        0        0     6663 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_base_vec.py
--rw-r--r--   0        0        0     1162 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_checks.py
--rw-r--r--   0        0        0      460 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_converters.py
--rw-r--r--   0        0        0      209 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_exceptions.py
--rw-r--r--   0        0        0      871 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_typing.py
--rw-r--r--   0        0        0     2424 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_utils.py
--rw-r--r--   0        0        0      411 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_version.py
--rw-r--r--   0        0        0       82 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_version.pyi
--rw-r--r--   0        0        0        0 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/py.typed
--rw-r--r--   0        0        0      217 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/setup_package.py
--rw-r--r--   0        0        0      382 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d1/__init__.py
--rw-r--r--   0        0        0     1990 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d1/base.py
--rw-r--r--   0        0        0     5743 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d1/builtin.py
--rw-r--r--   0        0        0     1118 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d1/compat.py
--rw-r--r--   0        0        0      857 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d1/operate.py
--rw-r--r--   0        0        0     2409 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d1/transform.py
--rw-r--r--   0        0        0      398 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d2/__init__.py
--rw-r--r--   0        0        0     1264 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d2/base.py
--rw-r--r--   0        0        0     7205 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d2/builtin.py
--rw-r--r--   0        0        0     1118 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d2/compat.py
--rw-r--r--   0        0        0      857 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d2/operate.py
--rw-r--r--   0        0        0     2451 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d2/transform.py
--rw-r--r--   0        0        0      454 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d3/__init__.py
--rw-r--r--   0        0        0     1264 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d3/base.py
--rw-r--r--   0        0        0     8200 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d3/builtin.py
--rw-r--r--   0        0        0    30492 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d3/compat.py
--rw-r--r--   0        0        0     2720 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d3/operate.py
--rw-r--r--   0        0        0    10683 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d3/sphere.py
--rw-r--r--   0        0        0    20889 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d3/transform.py
--rw-r--r--   0        0        0      323 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d4/__init__.py
--rw-r--r--   0        0        0      797 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d4/base.py
--rw-r--r--   0        0        0      556 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d4/compat.py
--rw-r--r--   0        0        0     2141 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d4/operate.py
--rw-r--r--   0        0        0     9447 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_d4/spacetime.py
--rw-r--r--   0        0        0      161 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_transform/__init__.py
--rw-r--r--   0        0        0    14040 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_transform/d1.py
--rw-r--r--   0        0        0    11103 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_transform/d2.py
--rw-r--r--   0        0        0    14949 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_transform/d3.py
--rw-r--r--   0        0        0     5927 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/_transform/differentials.py
--rw-r--r--   0        0        0      496 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/__init__.py
--rw-r--r--   0        0        0     3762 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_base.py
--rw-r--r--   0        0        0     2942 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_composite.py
--rw-r--r--   0        0        0      897 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_funcs.py
--rw-r--r--   0        0        0     5051 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_identity.py
--rw-r--r--   0        0        0     3426 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_sequential.py
--rw-r--r--   0        0        0      534 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_galilean/__init__.py
--rw-r--r--   0        0        0      632 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_galilean/base.py
--rw-r--r--   0        0        0     5265 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_galilean/boost.py
--rw-r--r--   0        0        0     7313 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_galilean/composite.py
--rw-r--r--   0        0        0     9084 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_galilean/rotation.py
--rw-r--r--   0        0        0    17390 2024-03-30 16:16:47.000000 coordinax-0.4.1/src/coordinax/operators/_galilean/translation.py
--rw-r--r--   0        0        0       13 2024-03-30 16:16:47.000000 coordinax-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     7885 2024-03-30 16:16:47.000000 coordinax-0.4.1/tests/test_base.py
--rw-r--r--   0        0        0    17504 2024-03-30 16:16:47.000000 coordinax-0.4.1/tests/test_d1.py
--rw-r--r--   0        0        0    18195 2024-03-30 16:16:47.000000 coordinax-0.4.1/tests/test_d2.py
--rw-r--r--   0        0        0    42443 2024-03-30 16:16:47.000000 coordinax-0.4.1/tests/test_d3.py
--rw-r--r--   0        0        0      408 2024-03-30 16:16:47.000000 coordinax-0.4.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     1183 2024-03-30 16:16:47.000000 coordinax-0.4.1/tests/test_jax_ops.py
--rw-r--r--   0        0        0      199 2024-03-30 16:16:47.000000 coordinax-0.4.1/tests/test_package.py
--rw-r--r--   0        0        0       36 2024-03-30 16:16:47.000000 coordinax-0.4.1/tests/test_utils.py
--rw-r--r--   0        0        0     2218 2024-03-30 16:16:47.000000 coordinax-0.4.1/.gitignore
--rw-r--r--   0        0        0     1531 2024-03-30 16:16:47.000000 coordinax-0.4.1/LICENSE
--rw-r--r--   0        0        0     1526 2024-03-30 16:16:47.000000 coordinax-0.4.1/README.md
--rw-r--r--   0        0        0     6850 2024-03-30 16:16:47.000000 coordinax-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     5416 2024-03-30 16:16:47.000000 coordinax-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      373 2024-04-02 19:39:44.000000 coordinax-0.4.2/.copier-answers.yml
+-rw-r--r--   0        0        0      125 2024-04-02 19:39:44.000000 coordinax-0.4.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2024-04-02 19:39:44.000000 coordinax-0.4.2/.gitattributes
+-rw-r--r--   0        0        0     2558 2024-04-02 19:39:44.000000 coordinax-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2024-04-02 19:39:44.000000 coordinax-0.4.2/.readthedocs.yml
+-rw-r--r--   0        0        0      439 2024-04-02 19:39:44.000000 coordinax-0.4.2/conftest.py
+-rw-r--r--   0        0        0     2819 2024-04-02 19:39:44.000000 coordinax-0.4.2/noxfile.py
+-rw-r--r--   0        0        0     2386 2024-04-02 19:39:44.000000 coordinax-0.4.2/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2024-04-02 19:39:44.000000 coordinax-0.4.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2024-04-02 19:39:44.000000 coordinax-0.4.2/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1540 2024-04-02 19:39:44.000000 coordinax-0.4.2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1655 2024-04-02 19:39:44.000000 coordinax-0.4.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      872 2024-04-02 19:39:44.000000 coordinax-0.4.2/docs/conf.py
+-rw-r--r--   0        0        0      196 2024-04-02 19:39:44.000000 coordinax-0.4.2/docs/index.md
+-rw-r--r--   0        0        0     1261 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/__init__.py
+-rw-r--r--   0        0        0    23716 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_base.py
+-rw-r--r--   0        0        0     3937 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_base_dif.py
+-rw-r--r--   0        0        0     6663 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_base_vec.py
+-rw-r--r--   0        0        0     1379 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_checks.py
+-rw-r--r--   0        0        0      460 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_converters.py
+-rw-r--r--   0        0        0      209 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_exceptions.py
+-rw-r--r--   0        0        0      871 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_typing.py
+-rw-r--r--   0        0        0     2424 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_utils.py
+-rw-r--r--   0        0        0      411 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_version.py
+-rw-r--r--   0        0        0       82 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_version.pyi
+-rw-r--r--   0        0        0        0 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/py.typed
+-rw-r--r--   0        0        0      217 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/setup_package.py
+-rw-r--r--   0        0        0      382 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d1/__init__.py
+-rw-r--r--   0        0        0     1990 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d1/base.py
+-rw-r--r--   0        0        0     5743 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d1/builtin.py
+-rw-r--r--   0        0        0     1118 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d1/compat.py
+-rw-r--r--   0        0        0      857 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d1/operate.py
+-rw-r--r--   0        0        0     2409 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d1/transform.py
+-rw-r--r--   0        0        0      398 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d2/__init__.py
+-rw-r--r--   0        0        0     1264 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d2/base.py
+-rw-r--r--   0        0        0     7205 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d2/builtin.py
+-rw-r--r--   0        0        0     1118 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d2/compat.py
+-rw-r--r--   0        0        0      857 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d2/operate.py
+-rw-r--r--   0        0        0     2451 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d2/transform.py
+-rw-r--r--   0        0        0      454 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d3/__init__.py
+-rw-r--r--   0        0        0     1264 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d3/base.py
+-rw-r--r--   0        0        0     8200 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d3/builtin.py
+-rw-r--r--   0        0        0    30492 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d3/compat.py
+-rw-r--r--   0        0        0     2720 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d3/operate.py
+-rw-r--r--   0        0        0    16465 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d3/sphere.py
+-rw-r--r--   0        0        0    21691 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d3/transform.py
+-rw-r--r--   0        0        0      323 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d4/__init__.py
+-rw-r--r--   0        0        0      797 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d4/base.py
+-rw-r--r--   0        0        0      556 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d4/compat.py
+-rw-r--r--   0        0        0     2141 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d4/operate.py
+-rw-r--r--   0        0        0     9447 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_d4/spacetime.py
+-rw-r--r--   0        0        0      161 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_transform/__init__.py
+-rw-r--r--   0        0        0    14040 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_transform/d1.py
+-rw-r--r--   0        0        0    11103 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_transform/d2.py
+-rw-r--r--   0        0        0    14949 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_transform/d3.py
+-rw-r--r--   0        0        0     5927 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/_transform/differentials.py
+-rw-r--r--   0        0        0      496 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/__init__.py
+-rw-r--r--   0        0        0     3762 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_base.py
+-rw-r--r--   0        0        0     2942 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_composite.py
+-rw-r--r--   0        0        0      897 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_funcs.py
+-rw-r--r--   0        0        0     5051 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_identity.py
+-rw-r--r--   0        0        0     3426 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_sequential.py
+-rw-r--r--   0        0        0      534 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_galilean/__init__.py
+-rw-r--r--   0        0        0      632 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_galilean/base.py
+-rw-r--r--   0        0        0     5265 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_galilean/boost.py
+-rw-r--r--   0        0        0     7319 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_galilean/composite.py
+-rw-r--r--   0        0        0     9090 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_galilean/rotation.py
+-rw-r--r--   0        0        0    17396 2024-04-02 19:39:44.000000 coordinax-0.4.2/src/coordinax/operators/_galilean/translation.py
+-rw-r--r--   0        0        0       13 2024-04-02 19:39:44.000000 coordinax-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     7885 2024-04-02 19:39:44.000000 coordinax-0.4.2/tests/test_base.py
+-rw-r--r--   0        0        0    17504 2024-04-02 19:39:44.000000 coordinax-0.4.2/tests/test_d1.py
+-rw-r--r--   0        0        0    18195 2024-04-02 19:39:44.000000 coordinax-0.4.2/tests/test_d2.py
+-rw-r--r--   0        0        0    42467 2024-04-02 19:39:44.000000 coordinax-0.4.2/tests/test_d3.py
+-rw-r--r--   0        0        0      408 2024-04-02 19:39:44.000000 coordinax-0.4.2/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1183 2024-04-02 19:39:44.000000 coordinax-0.4.2/tests/test_jax_ops.py
+-rw-r--r--   0        0        0      199 2024-04-02 19:39:44.000000 coordinax-0.4.2/tests/test_package.py
+-rw-r--r--   0        0        0       36 2024-04-02 19:39:44.000000 coordinax-0.4.2/tests/test_utils.py
+-rw-r--r--   0        0        0     2218 2024-04-02 19:39:44.000000 coordinax-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1531 2024-04-02 19:39:44.000000 coordinax-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1526 2024-04-02 19:39:44.000000 coordinax-0.4.2/README.md
+-rw-r--r--   0        0        0     6850 2024-04-02 19:39:44.000000 coordinax-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     5416 2024-04-02 19:39:44.000000 coordinax-0.4.2/PKG-INFO
```

### Comparing `coordinax-0.4.1/.pre-commit-config.yaml` & `coordinax-0.4.2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   autoupdate_commit_msg: "chore: update pre-commit hooks"
   autofix_commit_msg: "style: pre-commit fixes"
 
 default_stages: [pre-commit, pre-push]
 
 repos:
   - repo: https://github.com/commitizen-tools/commitizen
-    rev: v3.20.0
+    rev: v3.21.3
     hooks:
       - id: commitizen
       # - id: commitizen-branch
       #   stages: [push]
 
   - repo: meta
     hooks:
@@ -39,22 +39,22 @@
     rev: "v1.10.0"
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.0
+    rev: 0.28.1
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: "v0.3.4"
+    rev: "v0.3.5"
     hooks:
       # Run the linter
       - id: ruff
         types_or: [python, pyi, jupyter]
         args: ["--fix", "--show-fixes"]
       # Run the formatter
       - id: ruff-format
```

### Comparing `coordinax-0.4.1/noxfile.py` & `coordinax-0.4.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/.github/CONTRIBUTING.md` & `coordinax-0.4.2/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/.github/matchers/pylint.json` & `coordinax-0.4.2/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/.github/workflows/cd.yml` & `coordinax-0.4.2/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/.github/workflows/ci.yml` & `coordinax-0.4.2/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -62,8 +62,8 @@
 
       - name: Test package
         run: >-
           python -m pytest src docs tests -ra --cov --cov-report=xml
           --cov-report=term --durations=20 --arraydiff -m"not slow"
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v4.1.0
+        uses: codecov/codecov-action@v4.1.1
```

### Comparing `coordinax-0.4.1/docs/conf.py` & `coordinax-0.4.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/__init__.py` & `coordinax-0.4.2/src/coordinax/__init__.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_base.py` & `coordinax-0.4.2/src/coordinax/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -579,26 +579,29 @@
             z=Quantity[...](value=f32[], unit=Unit("m"))
         )
 
         """
         usys = unitsystem(units)
         return replace(
             self,
-            **{k: v.to(usys[v.unit.physical_type]) for k, v in dataclass_items(self)},
+            **{
+                k: v.to_units(usys[v.unit.physical_type])
+                for k, v in dataclass_items(self)
+            },
         )
 
     @dispatch
     def to_units(
-        self, units: Mapping[u.PhysicalType | str, Unit], /
+        self, units: Mapping[u.PhysicalType | str, Unit | str], /
     ) -> "AbstractVectorBase":
         """Convert the vector to the given units.
 
         Parameters
         ----------
-        units : Mapping[PhysicalType | str, Unit]
+        units : Mapping[PhysicalType | str, Unit | str]
             The units to convert to according to the physical type of the
             components.
 
         Examples
         --------
         >>> from unxt import Quantity
         >>> from coordinax import Cartesian2DVector, SphericalVector
@@ -624,15 +627,18 @@
 
         """
         # Ensure `units_` is PT -> Unit
         units_ = {u.get_physical_type(k): v for k, v in units.items()}
         # Convert to the given units
         return replace(
             self,
-            **{k: v.to(units_[v.unit.physical_type]) for k, v in dataclass_items(self)},
+            **{
+                k: v.to_units(units_[v.unit.physical_type])
+                for k, v in dataclass_items(self)
+            },
         )
 
     @dispatch
     def to_units(
         self, _: Literal[ToUnitsOptions.consistent], /
     ) -> "AbstractVectorBase":
         """Convert the vector to a self-consistent set of units.
@@ -674,15 +680,18 @@
         for v in dataclass_values(self):
             pt = v.unit.physical_type
             if pt not in units_:
                 units_[pt] = v.unit
 
         return replace(
             self,
-            **{k: v.to(units_[v.unit.physical_type]) for k, v in dataclass_items(self)},
+            **{
+                k: v.to_units(units_[v.unit.physical_type])
+                for k, v in dataclass_items(self)
+            },
         )
 
     # ===============================================================
     # Misc
 
     def __str__(self) -> str:
         r"""Return a string representation of the vector.
```

### Comparing `coordinax-0.4.1/src/coordinax/_base_dif.py` & `coordinax-0.4.2/src/coordinax/_base_dif.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_base_vec.py` & `coordinax-0.4.2/src/coordinax/_base_vec.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_checks.py` & `coordinax-0.4.2/src/coordinax/_checks.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,32 +12,42 @@
 
 _0m = Quantity(0, "meter")
 _0d = Quantity(0, "rad")
 _pid = Quantity(180, "deg")
 _2pid = Quantity(360, "deg")
 
 
-def check_r_non_negative(r: BatchableLength) -> BatchableLength:
+def check_r_non_negative(
+    r: BatchableLength, _lower: Quantity["length"] = _0m
+) -> BatchableLength:
     """Check that the radial distance is non-negative."""
     return eqx.error_if(
         r,
-        xp.any(r < _0m),
+        xp.any(r < _lower),
         "The radial distance must be non-negative.",
     )
 
 
-def check_azimuth_range(phi: BatchableAngle) -> BatchableAngle:
+def check_azimuth_range(
+    phi: BatchableAngle,
+    _lower: Quantity["angle"] = _0d,
+    _upper: Quantity["angle"] = _2pid,
+) -> BatchableAngle:
     """Check that the polar angle is in the range [0, 2pi)."""
     return eqx.error_if(
         phi,
-        xp.any((phi < _0d) | (phi >= _2pid)),
+        xp.any((phi < _lower) | (phi >= _upper)),
         "The azimuthal (polar) angle must be in the range [0, 2pi).",
     )
 
 
-def check_polar_range(theta: BatchableAngle) -> BatchableAngle:
+def check_polar_range(
+    theta: BatchableAngle,
+    _lower: Quantity["angle"] = _0d,
+    _upper: Quantity["angle"] = _pid,
+) -> BatchableAngle:
     """Check that the inclination angle is in the range [0, pi]."""
     return eqx.error_if(
         theta,
-        xp.any((theta < _0d) | (theta > _pid)),
+        xp.any((theta < _lower) | (theta > _upper)),
         "The inclination angle must be in the range [0, pi].",
     )
```

### Comparing `coordinax-0.4.1/src/coordinax/_typing.py` & `coordinax-0.4.2/src/coordinax/_typing.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_utils.py` & `coordinax-0.4.2/src/coordinax/_utils.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d1/base.py` & `coordinax-0.4.2/src/coordinax/_d1/base.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d1/builtin.py` & `coordinax-0.4.2/src/coordinax/_d1/builtin.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d1/compat.py` & `coordinax-0.4.2/src/coordinax/_d1/compat.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d1/operate.py` & `coordinax-0.4.2/src/coordinax/_d1/operate.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d1/transform.py` & `coordinax-0.4.2/src/coordinax/_d1/transform.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d2/base.py` & `coordinax-0.4.2/src/coordinax/_d2/base.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d2/builtin.py` & `coordinax-0.4.2/src/coordinax/_d2/builtin.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d2/compat.py` & `coordinax-0.4.2/src/coordinax/_d2/compat.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d2/operate.py` & `coordinax-0.4.2/src/coordinax/_d2/operate.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d2/transform.py` & `coordinax-0.4.2/src/coordinax/_d2/transform.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d3/base.py` & `coordinax-0.4.2/src/coordinax/_d3/base.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d3/builtin.py` & `coordinax-0.4.2/src/coordinax/_d3/builtin.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d3/compat.py` & `coordinax-0.4.2/src/coordinax/_d3/compat.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d3/operate.py` & `coordinax-0.4.2/src/coordinax/_d3/operate.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d3/transform.py` & `coordinax-0.4.2/src/coordinax/_d3/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -650,7 +650,29 @@
 
     # Calculate the differential in the new system
     return target(
         d_lon=current.d_lon_coslat / xp.cos(posvec.lat),
         d_lat=current.d_lat,
         d_distance=current.d_distance,
     )
+
+
+@dispatch
+def represent_as(
+    current: LonCosLatSphericalDifferential,
+    target: type[Abstract3DVectorDifferential],
+    position: AbstractVector | Quantity["length"],
+    /,
+    **kwargs: Any,
+) -> Abstract3DVectorDifferential:
+    """LonCosLatSphericalDifferential -> Abstract3DVectorDifferential."""
+    # Parse the position to an AbstractVector
+    if isinstance(position, AbstractVector):
+        posvec = position
+    else:  # Q -> Cart<X>D
+        posvec = current.integral_cls._cartesian_cls.constructor(  # noqa: SLF001
+            position
+        )
+    # Transform the differential to LonLatSphericalDifferential
+    current = represent_as(current, LonLatSphericalDifferential, posvec)
+    # Transform the position to the required type
+    return represent_as(current, target, posvec)
```

### Comparing `coordinax-0.4.1/src/coordinax/_d4/base.py` & `coordinax-0.4.2/src/coordinax/_d4/base.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d4/compat.py` & `coordinax-0.4.2/src/coordinax/_d4/compat.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d4/operate.py` & `coordinax-0.4.2/src/coordinax/_d4/operate.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_d4/spacetime.py` & `coordinax-0.4.2/src/coordinax/_d4/spacetime.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_transform/d1.py` & `coordinax-0.4.2/src/coordinax/_transform/d1.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_transform/d2.py` & `coordinax-0.4.2/src/coordinax/_transform/d2.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_transform/d3.py` & `coordinax-0.4.2/src/coordinax/_transform/d3.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/_transform/differentials.py` & `coordinax-0.4.2/src/coordinax/_transform/differentials.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/operators/_base.py` & `coordinax-0.4.2/src/coordinax/operators/_base.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/operators/_composite.py` & `coordinax-0.4.2/src/coordinax/operators/_composite.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/operators/_funcs.py` & `coordinax-0.4.2/src/coordinax/operators/_funcs.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/operators/_identity.py` & `coordinax-0.4.2/src/coordinax/operators/_identity.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/operators/_sequential.py` & `coordinax-0.4.2/src/coordinax/operators/_sequential.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/operators/_galilean/__init__.py` & `coordinax-0.4.2/src/coordinax/operators/_galilean/__init__.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/operators/_galilean/base.py` & `coordinax-0.4.2/src/coordinax/operators/_galilean/base.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/operators/_galilean/boost.py` & `coordinax-0.4.2/src/coordinax/operators/_galilean/boost.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/src/coordinax/operators/_galilean/composite.py` & `coordinax-0.4.2/src/coordinax/operators/_galilean/composite.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     >>> w = cx.FourVector.constructor(Quantity([0, 0, 0, 0], "kpc"))
     >>> new = op(w)
     >>> new
     FourVector(
       t=Quantity[PhysicalType('time')](value=f32[], unit=Unit("kpc s / km")),
       q=Cartesian3DVector( ... )
     )
-    >>> new.t.to("Gyr").value.round(2)
+    >>> new.t.to_units("Gyr").value.round(2)
     Array(2.5, dtype=float32)
     >>> new.q.x
     Quantity['length'](Array(3.5567803, dtype=float32), unit='kpc')
 
     Also the Galilean operators can also be applied to
     :class:`vector.Abstract3DVector` and :class:`unxt.Quantity`:
```

### Comparing `coordinax-0.4.1/src/coordinax/operators/_galilean/rotation.py` & `coordinax-0.4.2/src/coordinax/operators/_galilean/rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 
 def converter(x: Any) -> Array:
     """Convert the input to a rotation matrix."""
     if isinstance(x, GalileanRotationOperator):
         out = x.rotation
     elif isinstance(x, Quantity):
-        out = x.to_value("")
+        out = x.to_units_value("")
     else:
         out = x
     return jnp.asarray(out)
 
 
 @final
 class GalileanRotationOperator(AbstractGalileanOperator):
```

### Comparing `coordinax-0.4.1/src/coordinax/operators/_galilean/translation.py` & `coordinax-0.4.2/src/coordinax/operators/_galilean/translation.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,15 +455,15 @@
 
         Apply the translation operator:
 
         >>> new = op(w)
         >>> new.x
         Quantity['length'](Array(2., dtype=float32), unit='kpc')
 
-        >>> new.t.to("Gyr")
+        >>> new.t.to_units("Gyr")
         Quantity['time'](Array(0.99999994, dtype=float32), unit='Gyr')
 
         """
         return x + self.translation
 
     @op_call_dispatch(precedence=1)
     def __call__(
```

### Comparing `coordinax-0.4.1/tests/test_base.py` & `coordinax-0.4.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/tests/test_d1.py` & `coordinax-0.4.2/tests/test_d1.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/tests/test_d2.py` & `coordinax-0.4.2/tests/test_d2.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/tests/test_d3.py` & `coordinax-0.4.2/tests/test_d3.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,26 +35,26 @@
         apycart = -apyvector.represent_as(apyc.CartesianRepresentation)
         assert np.allclose(cart.x, apycart.x, atol=5e-7)
         assert np.allclose(cart.y, apycart.y, atol=5e-7)
         assert np.allclose(cart.z, apycart.z, atol=5e-7)
 
         # # Try finding the poles
         # if hasattr(vector, "theta"):
-        #     sel = (vector.theta.to_value("deg") != 0) & (
-        #         vector.theta.to_value("deg") != 180
+        #     sel = (vector.theta.to_units_value("deg") != 0) & (
+        #         vector.theta.to_units_value("deg") != 180
         #     )
         # else:
         #     sel = slice(None)
         # vecsel = convert(-vector[sel], type(apyvector))
         # apyvecsel = -apyvector[sel]
         # for c in vecsel.components:
         #     unit = getattr(apyvecsel, c).unit
         #     assert np.allclose(
-        #         getattr(vecsel, c).to_value(unit),
-        #         getattr(apyvecsel, c).to_value(unit),
+        #         getattr(vecsel, c).to_units_value(unit),
+        #         getattr(apyvecsel, c).to_units_value(unit),
         #         atol=5e-7,
         #     )
 
 
 class TestCartesian3DVector(Abstract3DVectorTest):
     """Test :class:`coordinax.Cartesian3DVector`."""
```

### Comparing `coordinax-0.4.1/tests/test_jax_ops.py` & `coordinax-0.4.2/tests/test_jax_ops.py`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/.gitignore` & `coordinax-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/LICENSE` & `coordinax-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/README.md` & `coordinax-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/pyproject.toml` & `coordinax-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `coordinax-0.4.1/PKG-INFO` & `coordinax-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: coordinax
-Version: 0.4.1
+Version: 0.4.2
 Summary: Vectors in JAX
 Project-URL: Bug Tracker, https://github.com/GalacticDynamics/coordinax/issues
 Project-URL: Changelog, https://github.com/GalacticDynamics/coordinax/releases
 Project-URL: Discussions, https://github.com/GalacticDynamics/coordinax/discussions
 Project-URL: Homepage, https://github.com/GalacticDynamics/coordinax
 Author-email: Nathaniel Starkman <nstarman@users.noreply.github.com>
 License: BSD 3-Clause License
```

