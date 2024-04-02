# Comparing `tmp/fluent_compiler-1.0.tar.gz` & `tmp/fluent_compiler-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluent_compiler-1.0.tar", last modified: Tue Apr 18 15:18:47 2023, max compression
+gzip compressed data, was "fluent_compiler-1.1.tar", last modified: Tue Apr  2 18:53:06 2024, max compression
```

## Comparing `fluent_compiler-1.0.tar` & `fluent_compiler-1.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.822632 fluent_compiler-1.0/
--rw-r--r--   0 luke      (1000) luke      (1000)     1250 2022-12-31 09:10:45.000000 fluent_compiler-1.0/.pre-commit-config.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)       73 2022-12-31 09:10:45.000000 fluent_compiler-1.0/.readthedocs.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)     4383 2022-12-31 09:10:45.000000 fluent_compiler-1.0/ARCHITECTURE.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     2031 2023-04-18 15:06:15.000000 fluent_compiler-1.0/CHANGELOG.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1719 2022-12-31 09:10:45.000000 fluent_compiler-1.0/CONTRIBUTING.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      551 2022-12-31 09:10:45.000000 fluent_compiler-1.0/LICENSE
--rw-r--r--   0 luke      (1000) luke      (1000)      422 2022-12-31 09:10:45.000000 fluent_compiler-1.0/MANIFEST.in
--rw-rw-rw-   0 luke      (1000) luke      (1000)     4460 2023-04-18 15:18:47.822632 fluent_compiler-1.0/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     3617 2022-12-31 09:10:45.000000 fluent_compiler-1.0/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      500 2023-02-16 18:31:40.000000 fluent_compiler-1.0/RELEASE.rst
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.814633 fluent_compiler-1.0/docs/
--rw-r--r--   0 luke      (1000) luke      (1000)      581 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/Makefile
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.814633 fluent_compiler-1.0/docs/api/
--rw-r--r--   0 luke      (1000) luke      (1000)     2421 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/api/bundle.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     4325 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/api/compiler.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      119 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/api/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1013 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/api/resource.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     5615 2023-04-18 15:14:26.000000 fluent_compiler-1.0/docs/conf.py
--rw-r--r--   0 luke      (1000) luke      (1000)       67 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/contributing.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     2271 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/errors.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     5678 2023-02-16 18:30:06.000000 fluent_compiler-1.0/docs/escaping.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     4077 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/functions.rst
--rw-r--r--   0 luke      (1000) luke      (1000)       30 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/history.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     4962 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/implementations.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      380 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      253 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/installation.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      787 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/make.bat
--rw-r--r--   0 luke      (1000) luke      (1000)       14 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/requirements.txt
--rw-r--r--   0 luke      (1000) luke      (1000)     3033 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/security.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     8721 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/usage.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      295 2022-12-31 09:10:45.000000 fluent_compiler-1.0/pyproject.toml
--rwxr-xr--   0 luke      (1000) luke      (1000)      439 2022-12-31 09:10:45.000000 fluent_compiler-1.0/release.sh
--rw-r--r--   0 luke      (1000) luke      (1000)       43 2022-12-31 09:10:45.000000 fluent_compiler-1.0/requirements-linters.txt
--rw-r--r--   0 luke      (1000) luke      (1000)      105 2022-12-31 09:10:45.000000 fluent_compiler-1.0/requirements-test.txt
--rw-r--r--   0 luke      (1000) luke      (1000)       60 2022-12-31 09:10:45.000000 fluent_compiler-1.0/requirements.txt
--rw-r--r--   0 luke      (1000) luke      (1000)     1075 2023-04-18 15:18:47.822632 fluent_compiler-1.0/setup.cfg
--rwxr-xr--   0 luke      (1000) luke      (1000)       60 2022-12-31 09:10:45.000000 fluent_compiler-1.0/setup.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.806632 fluent_compiler-1.0/src/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.814633 fluent_compiler-1.0/src/fluent_compiler/
--rw-r--r--   0 luke      (1000) luke      (1000)       20 2023-04-18 15:14:16.000000 fluent_compiler-1.0/src/fluent_compiler/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1791 2023-04-18 12:36:09.000000 fluent_compiler-1.0/src/fluent_compiler/ast_compat.py
--rw-r--r--   0 luke      (1000) luke      (1000)      158 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/builtins.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2139 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/bundle.py
--rw-r--r--   0 luke      (1000) luke      (1000)    29975 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/codegen.py
--rw-r--r--   0 luke      (1000) luke      (1000)    52647 2023-02-16 18:30:06.000000 fluent_compiler-1.0/src/fluent_compiler/compiler.py
--rw-r--r--   0 luke      (1000) luke      (1000)      660 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/errors.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5264 2023-02-16 18:30:06.000000 fluent_compiler-1.0/src/fluent_compiler/escapers.py
--rw-r--r--   0 luke      (1000) luke      (1000)      446 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/resource.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2614 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/runtime.py
--rw-r--r--   0 luke      (1000) luke      (1000)    14702 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/types.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6476 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/utils.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.814633 fluent_compiler-1.0/src/fluent_compiler.egg-info/
--rw-r-----   0 luke      (1000) luke      (1000)     4460 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/PKG-INFO
--rw-r-----   0 luke      (1000) luke      (1000)     1781 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/SOURCES.txt
--rw-r-----   0 luke      (1000) luke      (1000)        1 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/dependency_links.txt
--rw-r-----   0 luke      (1000) luke      (1000)       52 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/requires.txt
--rw-r-----   0 luke      (1000) luke      (1000)       16 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/top_level.txt
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.818632 fluent_compiler-1.0/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/__init__.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.818632 fluent_compiler-1.0/tests/format/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2568 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_arguments.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6136 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_attributes.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6771 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_builtins.py
--rw-r--r--   0 luke      (1000) luke      (1000)    16852 2023-02-16 18:30:06.000000 fluent_compiler-1.0/tests/format/test_escapers.py
--rw-r--r--   0 luke      (1000) luke      (1000)     9329 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_functions.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2222 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_isolating.py
--rw-r--r--   0 luke      (1000) luke      (1000)     9908 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_parameterized_terms.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5828 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_placeables.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5166 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_primitives.py
--rw-r--r--   0 luke      (1000) luke      (1000)    10567 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_select_expression.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6053 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_bundle.py
--rw-r--r--   0 luke      (1000) luke      (1000)    20518 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_codegen.py
--rw-r--r--   0 luke      (1000) luke      (1000)    38696 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_compiler.py
--rw-r--r--   0 luke      (1000) luke      (1000)    13981 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_types.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1560 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_utils.py
--rw-r--r--   0 luke      (1000) luke      (1000)       89 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/utils.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.806632 fluent_compiler-1.0/tools/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.822632 fluent_compiler-1.0/tools/benchmarks/
--rw-r--r--   0 luke      (1000) luke      (1000)     1077 2023-02-01 21:53:58.000000 fluent_compiler-1.0/tools/benchmarks/README.md
--rwxr-xr--   0 luke      (1000) luke      (1000)     1409 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tools/benchmarks/compiler.py
--rw-r--r--   0 luke      (1000) luke      (1000)       64 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tools/benchmarks/requirements.txt
--rwxr-xr--   0 luke      (1000) luke      (1000)     8207 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tools/benchmarks/runtime.py
--rw-r--r--   0 luke      (1000) luke      (1000)      766 2023-04-18 15:13:49.000000 fluent_compiler-1.0/tox.ini
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.286266 fluent_compiler-1.1/
+-rw-r--r--   0 luke      (1000) luke      (1000)      534 2024-04-02 18:12:57.000000 fluent_compiler-1.1/.pre-commit-config.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)      259 2024-04-02 18:12:57.000000 fluent_compiler-1.1/.readthedocs.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)     4385 2024-04-02 18:12:57.000000 fluent_compiler-1.1/ARCHITECTURE.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     2259 2024-04-02 18:49:50.000000 fluent_compiler-1.1/CHANGELOG.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1688 2024-04-02 18:12:57.000000 fluent_compiler-1.1/CONTRIBUTING.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      551 2022-12-31 09:10:45.000000 fluent_compiler-1.1/LICENSE
+-rw-r--r--   0 luke      (1000) luke      (1000)      422 2022-12-31 09:10:45.000000 fluent_compiler-1.1/MANIFEST.in
+-rw-rw-rw-   0 luke      (1000) luke      (1000)     5502 2024-04-02 18:53:06.286266 fluent_compiler-1.1/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     3808 2023-10-09 20:19:47.000000 fluent_compiler-1.1/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      408 2024-04-02 18:52:42.000000 fluent_compiler-1.1/RELEASE.rst
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.282266 fluent_compiler-1.1/docs/
+-rw-r--r--   0 luke      (1000) luke      (1000)      581 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/Makefile
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.282266 fluent_compiler-1.1/docs/api/
+-rw-r--r--   0 luke      (1000) luke      (1000)     2421 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/api/bundle.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     4325 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/api/compiler.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      119 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/api/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1013 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/api/resource.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     5648 2024-04-02 18:50:38.000000 fluent_compiler-1.1/docs/conf.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       67 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/contributing.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     2271 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/errors.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     5619 2023-10-01 15:41:45.000000 fluent_compiler-1.1/docs/escaping.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     4077 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/functions.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)       30 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/history.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     4962 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/implementations.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      380 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      253 2024-04-02 18:12:57.000000 fluent_compiler-1.1/docs/installation.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      787 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/make.bat
+-rw-r--r--   0 luke      (1000) luke      (1000)       36 2024-04-02 18:12:57.000000 fluent_compiler-1.1/docs/requirements.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)     3033 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/security.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     8721 2022-12-31 09:10:45.000000 fluent_compiler-1.1/docs/usage.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      392 2024-04-02 18:12:57.000000 fluent_compiler-1.1/pyproject.toml
+-rwxr-xr--   0 luke      (1000) luke      (1000)      512 2024-04-02 18:51:52.000000 fluent_compiler-1.1/release.sh
+-rw-r--r--   0 luke      (1000) luke      (1000)       27 2024-04-02 18:12:57.000000 fluent_compiler-1.1/requirements-linters.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)      105 2022-12-31 09:10:45.000000 fluent_compiler-1.1/requirements-test.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)       60 2022-12-31 09:10:45.000000 fluent_compiler-1.1/requirements.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)     1725 2024-04-02 18:53:06.286266 fluent_compiler-1.1/setup.cfg
+-rwxr-xr--   0 luke      (1000) luke      (1000)       60 2022-12-31 09:10:45.000000 fluent_compiler-1.1/setup.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.274266 fluent_compiler-1.1/src/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.282266 fluent_compiler-1.1/src/fluent_compiler/
+-rw-r--r--   0 luke      (1000) luke      (1000)       20 2024-04-02 18:50:27.000000 fluent_compiler-1.1/src/fluent_compiler/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2318 2024-04-02 18:12:57.000000 fluent_compiler-1.1/src/fluent_compiler/ast_compat.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      158 2022-12-31 09:10:45.000000 fluent_compiler-1.1/src/fluent_compiler/builtins.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2139 2022-12-31 09:10:45.000000 fluent_compiler-1.1/src/fluent_compiler/bundle.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    30072 2024-04-02 18:12:57.000000 fluent_compiler-1.1/src/fluent_compiler/codegen.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    52500 2024-04-02 18:30:57.000000 fluent_compiler-1.1/src/fluent_compiler/compiler.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      660 2022-12-31 09:10:45.000000 fluent_compiler-1.1/src/fluent_compiler/errors.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5264 2023-10-01 15:41:45.000000 fluent_compiler-1.1/src/fluent_compiler/escapers.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      446 2022-12-31 09:10:45.000000 fluent_compiler-1.1/src/fluent_compiler/resource.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2614 2022-12-31 09:10:45.000000 fluent_compiler-1.1/src/fluent_compiler/runtime.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    14702 2022-12-31 09:10:45.000000 fluent_compiler-1.1/src/fluent_compiler/types.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5706 2024-04-02 18:12:57.000000 fluent_compiler-1.1/src/fluent_compiler/utils.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.282266 fluent_compiler-1.1/src/fluent_compiler.egg-info/
+-rw-r--r--   0 luke      (1000) luke      (1000)     5502 2024-04-02 18:53:06.000000 fluent_compiler-1.1/src/fluent_compiler.egg-info/PKG-INFO
+-rw-r-----   0 luke      (1000) luke      (1000)     1781 2024-04-02 18:53:06.000000 fluent_compiler-1.1/src/fluent_compiler.egg-info/SOURCES.txt
+-rw-r-----   0 luke      (1000) luke      (1000)        1 2024-04-02 18:53:06.000000 fluent_compiler-1.1/src/fluent_compiler.egg-info/dependency_links.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       52 2024-04-02 18:53:06.000000 fluent_compiler-1.1/src/fluent_compiler.egg-info/requires.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       16 2024-04-02 18:53:06.000000 fluent_compiler-1.1/src/fluent_compiler.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.286266 fluent_compiler-1.1/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/__init__.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.286266 fluent_compiler-1.1/tests/format/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2568 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/test_arguments.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6136 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/test_attributes.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6771 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/test_builtins.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    16852 2024-04-02 17:34:16.000000 fluent_compiler-1.1/tests/format/test_escapers.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     9329 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/test_functions.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2222 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/test_isolating.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     9908 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/test_parameterized_terms.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5828 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/test_placeables.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5166 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/test_primitives.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    10567 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/format/test_select_expression.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6053 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/test_bundle.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    20518 2024-04-02 17:34:16.000000 fluent_compiler-1.1/tests/test_codegen.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    39970 2024-04-02 18:46:45.000000 fluent_compiler-1.1/tests/test_compiler.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    13981 2024-04-02 17:34:16.000000 fluent_compiler-1.1/tests/test_types.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1560 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/test_utils.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       89 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tests/utils.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.274266 fluent_compiler-1.1/tools/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2024-04-02 18:53:06.286266 fluent_compiler-1.1/tools/benchmarks/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1077 2023-02-01 21:53:58.000000 fluent_compiler-1.1/tools/benchmarks/README.md
+-rwxr-xr--   0 luke      (1000) luke      (1000)     1409 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tools/benchmarks/compiler.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       64 2022-12-31 09:10:45.000000 fluent_compiler-1.1/tools/benchmarks/requirements.txt
+-rwxr-xr--   0 luke      (1000) luke      (1000)     8305 2024-04-02 18:12:57.000000 fluent_compiler-1.1/tools/benchmarks/runtime.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      600 2024-04-02 18:12:57.000000 fluent_compiler-1.1/tox.ini
```

### Comparing `fluent_compiler-1.0/ARCHITECTURE.rst` & `fluent_compiler-1.1/ARCHITECTURE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
   terms.
 * We have to handle possible errors in accordance with the Fluent philosophy.
   Where possible we detect errors at compile time, in addition to the runtime
   handling shown above.
 
 We do not, in fact, generate Python code as a string, but instead generate AST
 which we can convert to executable Python functions using the builtin functions
-`compile <https://docs.python.org/3/library/functions.html#compile>`_ and `exec
+`compile <https://docs.python.org/3/library/functions.html#compile>`__ and `exec
 <https://docs.python.org/3/library/functions.html#exec>`_.
 
 Layers
 ~~~~~~
 
 The highest level code, which can be used as an entry point by users, is in
 ``fluent_compiler.bundle``. The interface provided here, however, is meant
@@ -82,15 +82,15 @@
 For generating Python code, it uses the classes provided by the
 ``fluent_compiler.codegen`` module. These are simplified versions of various
 Python constructs, with an interface that makes it easy for the ``compiler``
 module to construct correct code without worrying about lower level details.
 
 The classes in the ``codegen`` module eventually need to produce AST objects
 that can be passed to Python’s builtin `compile
-<https://docs.python.org/3/library/functions.html?highlight=compile#compile>`_
+<https://docs.python.org/3/library/functions.html?highlight=compile#compile>`__
 function. The stdlib `ast <https://docs.python.org/3/library/ast.html>`_ module
 has incompatible differences between different Python versions, so we abstract
 over these in ``fluent_compiler.ast_compat`` which allows the ``codegen`` module
 to almost entirely ignore the differences in AST for different Python.
 
 In addition to these modules, there are some runtime functions and types that
 are needed by the generated Python code, found in ``fluent_compiler.runtime``.
```

### Comparing `fluent_compiler-1.0/CHANGELOG.rst` & `fluent_compiler-1.1/CHANGELOG.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+fluent_compiler 1.1 (2024-04-02)
+--------------------------------
+
+* Fixed crasher with variable re-use when looking up the same argument more than
+  once. Thanks @ggindinson for bug report and PR.
+* Dropped Python 3.6 support
+
 fluent_compiler 1.0 (2023-04-18)
 --------------------------------
 
 * Tested against latest Python 3.11, and 3.12 alpha
 
 fluent_compiler 0.4 (2023-02-16)
 --------------------------------
```

### Comparing `fluent_compiler-1.0/CONTRIBUTING.rst` & `fluent_compiler-1.1/CONTRIBUTING.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 Contributing to fluent-compiler
 ===============================
 
 Issues
 ------
 
-You can help by filing bugs on GitHub: https://github.com/django-ftl/fluent-compiler/issues
+You can help by filing bugs on GitHub:
+https://github.com/django-ftl/fluent-compiler/issues.
 
 Please check existing issues before filing a new one.
 
+
 Development environment
 -----------------------
 
-To contribute fixes and features, you'll need to get set up for development:
+To contribute fixes and features, you'll need to get set up for
+development:
 
-1. For ``fluent_compiler`` on github
-2. Checkout a copy of the project using
-3. Create a virtualenv for development (or your preferred mechanism
-   for isolated Python environments)
+1. Fork ``fluent_compiler`` on GitHub.
+2. Clone and go to the forked repository.
+3. Create and activate a virtual environment for development (or your
+   preferred mechanism for isolated Python environments).
 4. Install the package in development mode::
 
-     ./setup.py develop
+     pip install -e .
 
 5. Install test requirements::
 
      pip install -r requirements-test.txt
 
 6. Run the tests::
 
      pytest
 
 If all that is successful, you are in good shape to start developing!
 
 We also have several linters and code formatters that we require use of,
-including `flake8 <http://flake8.pycqa.org/en/latest/>`_, `isort
-<https://github.com/timothycrosley/isort#readme>`_ and `black
-<https://github.com/psf/black>`_. These are most easily add by using `pre-commit
-<https://pre-commit.com/>`_:
+including `ruff <https://github.com/astral-sh/ruff>`_ and `black
+<https://github.com/psf/black>`_. These are most easily added by using
+`pre-commit <https://pre-commit.com/>`_:
 
-* Install pre-commit globally e.g. ``pipx install pre-commit`` if you already
-  have `pipx <https://github.com/pypa/pipx>`_.
+* Install pre-commit globally e.g. ``pipx install pre-commit`` if you
+  already have `pipx <https://github.com/pypa/pipx>`_.
 
 * Do ``pre-commit install`` in the repo.
 
 Now all the linters will run when you commit changes.
 
-To run tests on multiple Python versions locally you can also install and use
-``tox``.
+To run tests on multiple Python versions locally you can also install
+and use ``tox``.
 
 
 Fixes and features
 ------------------
 
 Please submit fixes and features by:
 
-1. First creating a branch for your changes
-2. Sending us a PR on GitHub
+1. First creating a branch for your changes.
+2. Sending us a PR on GitHub.
 
-For new features it is often better to open an issue first to see if we agree
-that the feature is a good idea, before spending a lot of time implementing it.
+For new features it is often better to open an issue first to see if we
+agree that the feature is a good idea, before spending a lot of time
+implementing it.
```

### Comparing `fluent_compiler-1.0/LICENSE` & `fluent_compiler-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/PKG-INFO` & `fluent_compiler-1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 Metadata-Version: 2.1
 Name: fluent_compiler
-Version: 1.0
+Version: 1.1
 Summary: Blazing fast implementation of Fluent localization language.
 Home-page: https://github.com/django-ftl/fluent-compiler
 Author: Luke Plant
 Author-email: L.Plant.98@cantab.net
 License: APL 2
-Keywords: fluent,localization,l10n,compiler
+Project-URL: Homepage, https://github.com/django-ftl/fluent-compiler
+Project-URL: Documentation, https://fluent-compiler.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/django-ftl/fluent-compiler
+Project-URL: Changelog, https://fluent-compiler.readthedocs.io/en/latest/history.html
+Project-URL: Tracker, https://github.com/django-ftl/fluent-compiler/issues
+Keywords: fluent,localization,l10n,compiler,projectfluent,ftl
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Compilers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Localization
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 fluent-compiler
 ===============
 
 .. image:: https://badge.fury.io/py/fluent-compiler.svg
@@ -68,19 +81,24 @@
 
 See `history <https://fluent-compiler.readthedocs.io/en/latest/history.html>`_ for a CHANGELOG.
 
 
 Status
 ------
 
-We are not planning major backwards incompatible changes to the interface, but
-we're also not guaranteeing stability yet. Also, the nature of the library is such
-that we expect most users will want to create their own wrappers anyway, which
-you are encouraged to do, in order to be able to absorb any backwards
-incompatible changes easily.
+fluent-compiler is a complete and very mature implementation of all the Fluent
+spec up to version 1.0 (the latest at the time of writing).
+
+In terms of API of this package, we are not planning backwards incompatible
+changes to the publicly documented interfaces, and will provide deprecation
+warnings for any changes.
+
+The nature of the library is such that we expect most users will want to create
+their own wrappers anyway, which you are encouraged to do, in order to be able
+to absorb any backwards incompatible changes easily.
 
 See the `issues list <https://github.com/django-ftl/fluent-compiler/issues>`_
 for planned features, and `CONTRIBUTING.rst <CONTRIBUTING.rst>`_ for information
 about how to contribute, and the `architecture docs <ARCHITECTURE.rst>`_.
 
 Contributing
 ------------
```

### Comparing `fluent_compiler-1.0/README.rst` & `fluent_compiler-1.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -46,19 +46,24 @@
 
 See `history <https://fluent-compiler.readthedocs.io/en/latest/history.html>`_ for a CHANGELOG.
 
 
 Status
 ------
 
-We are not planning major backwards incompatible changes to the interface, but
-we're also not guaranteeing stability yet. Also, the nature of the library is such
-that we expect most users will want to create their own wrappers anyway, which
-you are encouraged to do, in order to be able to absorb any backwards
-incompatible changes easily.
+fluent-compiler is a complete and very mature implementation of all the Fluent
+spec up to version 1.0 (the latest at the time of writing).
+
+In terms of API of this package, we are not planning backwards incompatible
+changes to the publicly documented interfaces, and will provide deprecation
+warnings for any changes.
+
+The nature of the library is such that we expect most users will want to create
+their own wrappers anyway, which you are encouraged to do, in order to be able
+to absorb any backwards incompatible changes easily.
 
 See the `issues list <https://github.com/django-ftl/fluent-compiler/issues>`_
 for planned features, and `CONTRIBUTING.rst <CONTRIBUTING.rst>`_ for information
 about how to contribute, and the `architecture docs <ARCHITECTURE.rst>`_.
 
 Contributing
 ------------
```

### Comparing `fluent_compiler-1.0/docs/Makefile` & `fluent_compiler-1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/docs/api/bundle.rst` & `fluent_compiler-1.1/docs/api/bundle.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/docs/api/compiler.rst` & `fluent_compiler-1.1/docs/api/compiler.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/docs/api/resource.rst` & `fluent_compiler-1.1/docs/api/resource.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/docs/conf.py` & `fluent_compiler-1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,31 +20,32 @@
 # -- Project information -----------------------------------------------------
 
 project = "fluent_compiler"
 copyright = "2019, Luke Plant"
 author = "Luke Plant"
 
 # The short X.Y version
-version = "1.0"
+version = "1.1"
 # The full version, including alpha/beta/rc tags
-release = "1.0"
+release = "1.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
+    "sphinx_rtd_theme",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -56,15 +57,15 @@
 master_doc = "index"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -72,15 +73,15 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "default"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
```

### Comparing `fluent_compiler-1.0/docs/errors.rst` & `fluent_compiler-1.1/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/docs/escaping.rst` & `fluent_compiler-1.1/docs/escaping.rst`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 
 .. code-block:: python
 
    bundle = FluentBundle('en', resources, escapers=[my_escaper])
 
 An ``escaper`` is an object that defines the following set of attributes. The
 object could be a module, or a simple namespace object you could create using
-``types.SimpleNamespace`` (or ``fluent_compiler.utils.SimpleNamespace`` on Python 2), or
-an instance of a class with appropriate methods defined. The attributes are:
+``types.SimpleNamespace``, or an instance of a class with appropriate
+methods defined. The attributes are:
 
 - ``name`` - a simple text value that is used in error messages.
 
 - ``select(**hints)``
 
   A callable that is used to decide whether or not to use this escaper for a
   given message (or message attribute). It is passed a number of hints as
```

### Comparing `fluent_compiler-1.0/docs/functions.rst` & `fluent_compiler-1.1/docs/functions.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/docs/implementations.rst` & `fluent_compiler-1.1/docs/implementations.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/docs/make.bat` & `fluent_compiler-1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/docs/security.rst` & `fluent_compiler-1.1/docs/security.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/docs/usage.rst` & `fluent_compiler-1.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/setup.cfg` & `fluent_compiler-1.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -9,39 +9,50 @@
 license = APL 2
 url = https://github.com/django-ftl/fluent-compiler
 keywords = 
 	fluent
 	localization
 	l10n
 	compiler
+	projectfluent
+	ftl
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
-	Programming Language :: Python :: 3.6
+	Operating System :: OS Independent
+	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
+	Programming Language :: Python :: Implementation :: CPython
+	Programming Language :: Python :: Implementation :: PyPy
+	Topic :: Software Development :: Compilers
+	Topic :: Software Development :: Libraries :: Python Modules
+	Topic :: Software Development :: Localization
+project_urls = 
+	Homepage = https://github.com/django-ftl/fluent-compiler
+	Documentation = https://fluent-compiler.readthedocs.io/en/latest/
+	Repository = https://github.com/django-ftl/fluent-compiler
+	Changelog = https://fluent-compiler.readthedocs.io/en/latest/history.html
+	Tracker = https://github.com/django-ftl/fluent-compiler/issues
 
 [options]
 packages = find:
 package_dir = =src
+python_requires = >=3.7
 install_requires = 
 	fluent.syntax>=0.14
 	attrs>=19.3.0
 	babel>=2.8.0
 	pytz
 
 [options.packages.find]
 where = src
 
-[flake8]
-exclude = .tox,build,.eggs
-ignore = D100,D101,W504,W503
-max-line-length = 120
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fluent_compiler-1.0/src/fluent_compiler/ast_compat.py` & `fluent_compiler-1.1/src/fluent_compiler/ast_compat.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
           return ast.OldAst(...)
 
   else:
       NewAst = ast.NewAst
 
 """
 import ast
+import sys
 
 # This is a very limited subset of Python AST:
 # - only the things needed by codegen.py
 # - only syntax features provided by the oldest Python version we support
 
 Add = ast.Add
 Assign = ast.Assign
@@ -39,34 +40,42 @@
 ExceptHandler = ast.ExceptHandler
 Expr = ast.Expr
 If = ast.If
 Index = ast.Index
 List = ast.List
 Load = ast.Load
 Module = ast.Module
-Num = ast.Num
 Or = ast.Or
 Pass = ast.Pass
 Return = ast.Return
 Store = ast.Store
-Str = ast.Str
 Subscript = ast.Subscript
 Tuple = ast.Tuple
 arguments = ast.arguments
 JoinedStr = ast.JoinedStr
 FormattedValue = ast.FormattedValue
 Attribute = ast.Attribute
 Call = ast.Call
 FunctionDef = ast.FunctionDef
 Name = ast.Name
-NameConstant = ast.NameConstant
 Try = ast.Try
 arg = ast.arg
 keyword = ast.keyword
+walk = ast.walk
 
 
-def traverse(ast_node, func):
-    """
-    Apply 'func' to ast_node (which is `ast.*` object)
-    """
-    for node in ast.walk(ast_node):
-        func(node)
+if sys.version_info >= (3, 8):
+    Constant = ast.Constant
+else:
+    # For Python 3.7, in terms of runtime behaviour we could also use
+    # Constant for Str/Num, but this seems to trigger bugs when decompiling with
+    # ast_decompiler, which is needed by tests. So we use the more normal
+    # ast that Python 3.7 use for this code.
+    def Constant(arg, **kwargs):
+        if isinstance(arg, str):
+            return ast.Str(arg, **kwargs)
+        elif isinstance(arg, (int, float)):
+            return ast.Num(arg, **kwargs)
+        elif arg is None:
+            return ast.NameConstant(arg, **kwargs)
+        else:
+            raise NotImplementedError(f"Constant not implemented for args of type {type(arg)}")
```

### Comparing `fluent_compiler-1.0/src/fluent_compiler/bundle.py` & `fluent_compiler-1.1/src/fluent_compiler/bundle.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/src/fluent_compiler/codegen.py` & `fluent_compiler-1.1/src/fluent_compiler/codegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,17 +293,15 @@
         self.statements.append(statement)
         if isinstance(statement, Block):
             if statement.parent_block is None:
                 statement.parent_block = self
             else:
                 if statement.parent_block != self:
                     raise AssertionError(
-                        "Block {} is already child of {}, can't reassign to {}".format(
-                            statement, statement.parent_block, self
-                        )
+                        f"Block {statement} is already child of {statement.parent_block}, can't reassign to {self}"
                     )
 
     # Safe alternatives to Block.statements being manipulated directly:
     def add_assignment(self, name, value, allow_multiple=False):
         """
         Adds an assigment of the form:
 
@@ -402,15 +400,15 @@
 
             # It's hard to get good line numbers for all AST objects, but
             # if we put the FTL line number of the main message on all nodes
             # this gets us a lot of the benefit for a smallish cost
             def add_lineno(node):
                 node.lineno = self.source.row
 
-            ast.traverse(func_def, add_lineno)
+            traverse(func_def, add_lineno)
         return func_def
 
     def add_return(self, value):
         self.body.add_return(value)
 
 
 class Return(Statement, PythonAst):
@@ -527,15 +525,15 @@
 
     type = str
 
     def __init__(self, string_value):
         self.string_value = string_value
 
     def as_ast(self):
-        return ast.Str(
+        return ast.Constant(
             self.string_value,
             kind=None,  # 3.8, indicates no prefix, needed only for tests
             **DEFAULT_AST_ARGS,
         )
 
     def __repr__(self):
         return f"String({repr(self.string_value)})"
@@ -548,15 +546,15 @@
     child_elements = []
 
     def __init__(self, number):
         self.number = number
         self.type = type(number)
 
     def as_ast(self):
-        return ast.Num(n=self.number, **DEFAULT_AST_ARGS)
+        return ast.Constant(self.number, **DEFAULT_AST_ARGS)
 
     def __repr__(self):
         return f"Number({repr(self.number)})"
 
 
 class List(Expression):
     child_elements = ["items"]
@@ -725,15 +723,15 @@
             return ast.Call(
                 func=ast.Name(id=self.function_name, ctx=ast.Load(), **DEFAULT_AST_ARGS),
                 args=[arg.as_ast() for arg in self.args],
                 keywords=[
                     ast.keyword(
                         arg=None,
                         value=ast.Dict(
-                            keys=[ast.Str(k, kind=None, **DEFAULT_AST_ARGS) for k in kwarg_names],
+                            keys=[ast.Constant(k, kind=None, **DEFAULT_AST_ARGS) for k in kwarg_names],
                             values=[v.as_ast() for v in kwarg_values],
                             **DEFAULT_AST_ARGS,
                         ),
                         **DEFAULT_AST_ARGS,
                     )
                 ],
                 **DEFAULT_AST_ARGS,
@@ -802,15 +800,15 @@
 ObjectCreation = FunctionCall
 
 
 class NoneExpr(Expression):
     type = type(None)
 
     def as_ast(self):
-        return ast.NameConstant(value=None, **DEFAULT_AST_ARGS)
+        return ast.Constant(value=None, **DEFAULT_AST_ARGS)
 
 
 class BinaryOperator(Expression):
     child_elements = ["left", "right"]
 
     def __init__(self, left, right):
         self.left = left
@@ -841,14 +839,22 @@
         )
 
 
 class Or(BoolOp):
     op = ast.Or
 
 
+def traverse(ast_node, func):
+    """
+    Apply 'func' to ast_node (which is `ast.*` object)
+    """
+    for node in ast.walk(ast_node):
+        func(node)
+
+
 def simplify(codegen_ast, simplifier):
     changes = [True]
 
     # Wrap `simplifier` (which takes additional `changes` arg)
     # into function that take just `node`, as required by rewriting_traverse
     def rewriter(node):
         return simplifier(node, changes)
```

### Comparing `fluent_compiler-1.0/src/fluent_compiler/compiler.py` & `fluent_compiler-1.1/src/fluent_compiler/compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,17 +727,15 @@
 
 
 def compile_term(term, block, compiler_env, new_escaper, term_args=None):
     current_escaper = compiler_env.current.escaper
     if not escapers_compatible(current_escaper, new_escaper):
         term_id = ast_to_id(term)
         error = TypeError(
-            "Escaper {} for term {} cannot be used from calling context with {} escaper".format(
-                new_escaper.name, term_id, current_escaper.name
-            )
+            f"Escaper {new_escaper.name} for term {term_id} cannot be used from calling context with {current_escaper.name} escaper"
         )
         add_static_msg_error(block, error)
         compiler_env.add_current_message_error(error)
         return make_fluent_none(term_id, block.scope)
     else:
         with compiler_env.modified(escaper=new_escaper):
             with compiler_env.modified_for_term_reference(term_args=term_args):
@@ -753,18 +751,15 @@
         args = [compile_expr(arg, block, compiler_env) for arg in reference.arguments.positional]
         kwargs = {
             kwarg.name.name: compile_expr(kwarg.value, block, compiler_env) for kwarg in reference.arguments.named
         }
 
         if args:
             args_err = FluentFormatError(
-                "{}: Ignored positional arguments passed to term '{}'".format(
-                    display_ast_location(reference.arguments, compiler_env),
-                    reference_to_id(reference),
-                )
+                f"{display_ast_location(reference.arguments, compiler_env)}: Ignored positional arguments passed to term '{reference_to_id(reference)}'"
             )
             add_static_msg_error(block, args_err)
             compiler_env.add_current_message_error(args_err)
     else:
         kwargs = None
 
     return compile_term(term, block, compiler_env, new_escaper, term_args=kwargs)
@@ -905,15 +900,15 @@
                 ],
                 {},
                 block.scope,
             )
 
     if block.scope.has_assignment(arg_tmp_name):  # already assigned to this, can re-use
         if not wrap_with_handle_argument:
-            return block.variable(arg_tmp_name)
+            return block.scope.variable(arg_tmp_name)
 
         block.add_assignment(arg_handled_tmp_name, handle_argument_func_call)
         return block.scope.variable(arg_handled_tmp_name)
 
     # Add try/except/else to lookup variable.
     try_except = codegen.Try(
         [
@@ -1022,17 +1017,15 @@
 
 
 def do_message_call(msg_id, block, compiler_env):
     current_escaper = compiler_env.current.escaper
     new_escaper = compiler_env.escaper_for_message(msg_id)
     if not escapers_compatible(current_escaper, new_escaper):
         error = TypeError(
-            "Escaper {} for message {} cannot be used from calling context with {} escaper".format(
-                new_escaper.name, msg_id, current_escaper.name
-            )
+            f"Escaper {new_escaper.name} for message {msg_id} cannot be used from calling context with {current_escaper.name} escaper"
         )
         add_static_msg_error(block, error)
         compiler_env.add_current_message_error(error)
         return make_fluent_none(msg_id, block.scope)
 
     msg_func_name = compiler_env.message_mapping[msg_id]
     if compiler_env.current.term_args is not None:
```

### Comparing `fluent_compiler-1.0/src/fluent_compiler/errors.py` & `fluent_compiler-1.1/src/fluent_compiler/errors.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/src/fluent_compiler/escapers.py` & `fluent_compiler-1.1/src/fluent_compiler/escapers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from types import SimpleNamespace
+
 from . import codegen
-from .utils import SimpleNamespace
 
 
 def identity(value):
     """
     Identity function.
     The function is also used as a sentinel value by the
     compiler for it to detect a no-op
```

### Comparing `fluent_compiler-1.0/src/fluent_compiler/runtime.py` & `fluent_compiler-1.1/src/fluent_compiler/runtime.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/src/fluent_compiler/types.py` & `fluent_compiler-1.1/src/fluent_compiler/types.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/src/fluent_compiler/utils.py` & `fluent_compiler-1.1/src/fluent_compiler/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,35 +14,14 @@
 class Any:
     pass
 
 
 Any = Any()
 
 
-# On Python 3 we could get away with just using a class, but on Python 2
-# functions defined in the class body get wrapped with UnboundMethod, which
-# causes problems.
-
-try:
-    from types import SimpleNamespace
-except ImportError:
-    # Python 2 fallback
-    class SimpleNamespace:
-        def __init__(self, **kwargs):
-            self.__dict__.update(kwargs)
-
-        def __repr__(self):
-            keys = sorted(self.__dict__)
-            items = (f"{k}={self.__dict__[k]!r}" for k in keys)
-            return f"{type(self).__name__}({', '.join(items)})"
-
-        def __eq__(self, other):
-            return self.__dict__ == other.__dict__
-
-
 # From spec:
 #    NamedArgument ::= Identifier blank? ":" blank? (StringLiteral | NumberLiteral)
 #    Identifier ::= [a-zA-Z] [a-zA-Z0-9_-]*
 
 NAMED_ARG_RE = re.compile(r"^[a-zA-Z][a-zA-Z0-9_-]*$")
 
 
@@ -65,15 +44,14 @@
     """
     Returns a string reference for an Attribute, given Attribute and parent Term or Message
     """
     return "".join([ast_to_id(parent_ast), ATTRIBUTE_SEPARATOR, attribute.id.name])
 
 
 def allowable_name(ident, for_method=False, allow_builtin=False):
-
     if keyword.iskeyword(ident):
         return False
 
     if not (for_method or allow_builtin):
         if ident in dir(builtins):
             return False
 
@@ -147,25 +125,21 @@
         sanitized_args = args
     else:
         sanitized_args = tuple(args[0:positional_arg_count])
         len_args = len(args)
         if len_args > positional_arg_count:
             errors.append(
                 TypeError(
-                    "{}() takes {} positional arguments but {} were given".format(
-                        function_name, positional_arg_count, len_args
-                    )
+                    f"{function_name}() takes {positional_arg_count} positional arguments but {len_args} were given"
                 )
             )
         elif len_args < positional_arg_count:
             errors.append(
                 TypeError(
-                    "{}() takes {} positional arguments but {} were given".format(
-                        function_name, positional_arg_count, len_args
-                    )
+                    f"{function_name}() takes {positional_arg_count} positional arguments but {len_args} were given"
                 )
             )
             match = False
 
     return (match, sanitized_args, sanitized_kwargs, errors)
 
 
@@ -182,15 +156,15 @@
     """
     if isinstance(ref, TermReference):
         start = TERM_SIGIL + ref.id.name
     else:
         start = ref.id.name
 
     if not ignore_attributes and ref.attribute:
-        return "".join([start, ATTRIBUTE_SEPARATOR, ref.attribute.name])
+        return f"{start}{ATTRIBUTE_SEPARATOR}{ref.attribute.name}"
     return start
 
 
 def sanitize_function_args(arg_spec, name, errors):
     """
     Check function arg spec is legitimate, returning a cleaned
     up version, and adding any errors to errors list.
```

### Comparing `fluent_compiler-1.0/src/fluent_compiler.egg-info/PKG-INFO` & `fluent_compiler-1.1/src/fluent_compiler.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 Metadata-Version: 2.1
 Name: fluent-compiler
-Version: 1.0
+Version: 1.1
 Summary: Blazing fast implementation of Fluent localization language.
 Home-page: https://github.com/django-ftl/fluent-compiler
 Author: Luke Plant
 Author-email: L.Plant.98@cantab.net
 License: APL 2
-Keywords: fluent,localization,l10n,compiler
+Project-URL: Homepage, https://github.com/django-ftl/fluent-compiler
+Project-URL: Documentation, https://fluent-compiler.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/django-ftl/fluent-compiler
+Project-URL: Changelog, https://fluent-compiler.readthedocs.io/en/latest/history.html
+Project-URL: Tracker, https://github.com/django-ftl/fluent-compiler/issues
+Keywords: fluent,localization,l10n,compiler,projectfluent,ftl
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Compilers
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Localization
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 fluent-compiler
 ===============
 
 .. image:: https://badge.fury.io/py/fluent-compiler.svg
@@ -68,19 +81,24 @@
 
 See `history <https://fluent-compiler.readthedocs.io/en/latest/history.html>`_ for a CHANGELOG.
 
 
 Status
 ------
 
-We are not planning major backwards incompatible changes to the interface, but
-we're also not guaranteeing stability yet. Also, the nature of the library is such
-that we expect most users will want to create their own wrappers anyway, which
-you are encouraged to do, in order to be able to absorb any backwards
-incompatible changes easily.
+fluent-compiler is a complete and very mature implementation of all the Fluent
+spec up to version 1.0 (the latest at the time of writing).
+
+In terms of API of this package, we are not planning backwards incompatible
+changes to the publicly documented interfaces, and will provide deprecation
+warnings for any changes.
+
+The nature of the library is such that we expect most users will want to create
+their own wrappers anyway, which you are encouraged to do, in order to be able
+to absorb any backwards incompatible changes easily.
 
 See the `issues list <https://github.com/django-ftl/fluent-compiler/issues>`_
 for planned features, and `CONTRIBUTING.rst <CONTRIBUTING.rst>`_ for information
 about how to contribute, and the `architecture docs <ARCHITECTURE.rst>`_.
 
 Contributing
 ------------
```

### Comparing `fluent_compiler-1.0/src/fluent_compiler.egg-info/SOURCES.txt` & `fluent_compiler-1.1/src/fluent_compiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_arguments.py` & `fluent_compiler-1.1/tests/format/test_arguments.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_attributes.py` & `fluent_compiler-1.1/tests/format/test_attributes.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_builtins.py` & `fluent_compiler-1.1/tests/format/test_builtins.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_escapers.py` & `fluent_compiler-1.1/tests/format/test_escapers.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_functions.py` & `fluent_compiler-1.1/tests/format/test_functions.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_isolating.py` & `fluent_compiler-1.1/tests/format/test_isolating.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_parameterized_terms.py` & `fluent_compiler-1.1/tests/format/test_parameterized_terms.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_placeables.py` & `fluent_compiler-1.1/tests/format/test_placeables.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_primitives.py` & `fluent_compiler-1.1/tests/format/test_primitives.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/format/test_select_expression.py` & `fluent_compiler-1.1/tests/format/test_select_expression.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/test_bundle.py` & `fluent_compiler-1.1/tests/test_bundle.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/test_codegen.py` & `fluent_compiler-1.1/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/test_compiler.py` & `fluent_compiler-1.1/tests/test_compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import unittest
+from types import SimpleNamespace
 
 from markupsafe import Markup, escape
 
 from fluent_compiler import codegen
 from fluent_compiler.compiler import compile_messages
 from fluent_compiler.errors import FluentCyclicReferenceError, FluentFormatError, FluentReferenceError
 from fluent_compiler.resource import FtlResource
-from fluent_compiler.utils import SimpleNamespace
 
 from .test_codegen import decompile_ast_list, normalize_python
 from .utils import dedent_ftl
 
 # Some TDD tests to help develop compiler. It should be possible to delete
 # the tests here and still have complete test coverage of the compiler.py module, via
 # the other FluentBundle.format tests.
@@ -1274,7 +1274,45 @@
         self.assertRaises(
             ValueError,
             compile_messages_to_python,
             "foo = bar",
             self.locale,
             escapers=[html_escaper, html_escaper],
         )
+
+    def test_variable_reuse_for_arg_lookup(self):
+        code, errs = self.compile_messages(
+            """
+            example = My name is { $name ->
+                [Peter] Peter11
+               *[other] Jane11
+              }
+              My gender is { $name ->
+                [Peter] Male
+               *[other] Female
+              }
+              """
+        )
+        assert not errs
+        # $name should only be looked up once
+        self.assertCodeEqual(
+            code,
+            """
+            def example(message_args, errors):
+                try:
+                    _arg = message_args['name']
+                except (LookupError, TypeError):
+                    errors.append(FluentReferenceError('<string>:2:24: Unknown external: name'))
+                    _arg = FluentNone('name')
+                _plural_form = plural_form_for_number(_arg)
+                if _arg == 'Peter':
+                    _ret = 'Peter11'
+                else:
+                    _ret = 'Jane11'
+                _plural_form2 = plural_form_for_number(_arg)
+                if _arg == 'Peter':
+                    _ret2 = 'Male'
+                else:
+                    _ret2 = 'Female'
+                return f'My name is {_ret}\\nMy gender is {_ret2}'
+        """,
+        )
```

### Comparing `fluent_compiler-1.0/tests/test_types.py` & `fluent_compiler-1.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tests/test_utils.py` & `fluent_compiler-1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tools/benchmarks/README.md` & `fluent_compiler-1.1/tools/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tools/benchmarks/compiler.py` & `fluent_compiler-1.1/tools/benchmarks/compiler.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-1.0/tools/benchmarks/runtime.py` & `fluent_compiler-1.1/tools/benchmarks/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,69 +126,69 @@
 def test_single_string_gettext(gettext_translations, benchmark):
     gettext_translations.gettext("Hello I am a single string literal")  # for extract process
     result = benchmark(
         unicode_gettext_method(gettext_translations),
         "Hello I am a single string literal",
     )
     assert result == "Hello I am a single string literal in Polish"
-    assert type(result) is str
+    assert type(result) is str  # noqa: E721
 
 
 def test_single_string_fluent_interpreter_cached(interpreting_fluent_bundle, benchmark):
     # `format_pattern` is very awkward pattern for performance, but we assume
     # that we can cache `get_message` return value somewhere, to give best
     # possible chance to it.
     message_val = interpreting_fluent_bundle.get_message("single-string-literal").value
     result = benchmark(interpreting_fluent_bundle.format_pattern, message_val)
     assert result[0] == "Hello I am a single string literal in Polish"
-    assert type(result[0]) is str
+    assert type(result[0]) is str  # noqa: E721
 
 
 def test_single_string_fluent_interpreter(interpreting_fluent_bundle, benchmark):
     # Without caching
     result = benchmark(
         lambda: interpreting_fluent_bundle.format_pattern(
             interpreting_fluent_bundle.get_message("single-string-literal").value
         )
     )
     assert result[0] == "Hello I am a single string literal in Polish"
-    assert type(result[0]) is str
+    assert type(result[0]) is str  # noqa: E721
 
 
 def test_single_string_fluent_compiler(compiling_fluent_bundle, benchmark):
     result = benchmark(compiling_fluent_bundle.format, "single-string-literal")
     assert result[0] == "Hello I am a single string literal in Polish"
-    assert type(result[0]) is str
+    assert type(result[0]) is str  # noqa: E721
 
 
 def test_single_interpolation_gettext(gettext_translations, benchmark):
     gettext_translations.gettext("Hello %(username)s, welcome to our website!")  # for extract process
     t = unicode_gettext_method(gettext_translations)
     args = {"username": "Mary"}
     result = benchmark(lambda: t("Hello %(username)s, welcome to our website!") % args)
     assert result == "Hello Mary, welcome to our website! in Polish"
-    assert type(result) is str
+    assert type(result) is str  # noqa: E721
 
 
 def test_single_interpolation_fluent_interpreter(interpreting_fluent_bundle, benchmark):
     args = {"username": "Mary"}
     result = benchmark(
         lambda: interpreting_fluent_bundle.format_pattern(
             interpreting_fluent_bundle.get_message("single-interpolation").value, args
         )
     )
     assert result[0] == "Hello Mary, welcome to our website! in Polish"
-    assert type(result[0]) is str
+    assert type(result[0]) is str  # noqa: E721
 
 
 def test_single_interpolation_fluent_compiler(compiling_fluent_bundle, benchmark):
     args = {"username": "Mary"}
     result = benchmark(compiling_fluent_bundle.format, "single-interpolation", args)
     assert result[0] == "Hello Mary, welcome to our website! in Polish"
-    assert type(result[0]) is str
+    assert type(result[0]) is str  # noqa: E721
 
 
 def test_plural_form_select_gettext(gettext_translations, benchmark):
     gettext_translations.ngettext("There is %(count)d thing", "There are %(count)d things", 1)  # for extract process
     t = unicode_ngettext_method(gettext_translations)
 
     def f():
```

### Comparing `fluent_compiler-1.0/tox.ini` & `fluent_compiler-1.1/tox.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,20 @@
 # This config is for local testing. Where needed changes should be duplicated into
 # .github/workflows/pythonpackage.yml
 [tox]
-envlist = py36,py37,py38,py39,py310,py311,py312,pypy3.6,flake8,isort
+envlist = py37,py38,py39,py310,py311,py312
 
 [testenv]
 deps =
      # Just '.[develop]' would be nice here.
      # Unfortunately it is super slow: https://github.com/pypa/pip/issues/2195
      # So we duplicate deps from setup.py for now.
      -r{toxinidir}/requirements.txt
      -r{toxinidir}/requirements-test.txt
      -r{toxinidir}/requirements-linters.txt
 commands = pytest
 
 
-[testenv:flake8]
-basepython = python3.9
-commands = flake8 src tests
-
-
-[testenv:isort]
-basepython = python3.9
-commands = isort -c src tests
-
 [testenv:check-manifest]
 basepython = python3.9
 deps = check-manifest
 commands = check-manifest
```

