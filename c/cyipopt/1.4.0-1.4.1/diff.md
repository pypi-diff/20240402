# Comparing `tmp/cyipopt-1.4.0.tar.gz` & `tmp/cyipopt-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyipopt-1.4.0.tar", last modified: Mon Apr  1 15:17:26 2024, max compression
+gzip compressed data, was "cyipopt-1.4.1.tar", last modified: Tue Apr  2 17:15:48 2024, max compression
```

## Comparing `cyipopt-1.4.0.tar` & `cyipopt-1.4.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      962 2024-04-01 15:14:42.000000 cyipopt-1.4.0/AUTHORS
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7849 2024-04-01 15:14:42.000000 cyipopt-1.4.0/CHANGELOG.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    14199 2023-02-19 14:17:20.000000 cyipopt-1.4.0/LICENSE
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      373 2023-11-28 14:15:09.000000 cyipopt-1.4.0/MANIFEST.in
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     3950 2024-04-01 15:17:26.098451 cyipopt-1.4.0/PKG-INFO
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3082 2023-09-15 17:50:42.000000 cyipopt-1.4.0/README.rst
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      399 2024-04-01 15:14:42.000000 cyipopt-1.4.0/cyipopt/__init__.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt/cython/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8683 2023-09-15 17:50:42.000000 cyipopt-1.4.0/cyipopt/cython/ipopt.pxd
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    46828 2024-04-01 14:32:00.000000 cyipopt-1.4.0/cyipopt/cython/ipopt_wrapper.pyx
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1356 2024-04-01 15:14:42.000000 cyipopt-1.4.0/cyipopt/exceptions.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2548 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/ipopt_wrapper.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    27367 2024-04-01 15:14:42.000000 cyipopt-1.4.0/cyipopt/scipy_interface.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt/tests/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/__init__.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     6366 2023-09-15 17:50:42.000000 cyipopt-1.4.0/cyipopt/tests/conftest.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt/tests/integration/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/integration/__init__.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8459 2023-09-15 18:27:54.000000 cyipopt-1.4.0/cyipopt/tests/integration/test_hs071.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/integration/test_lasso.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/integration/test_rosen.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/cyipopt/tests/unit/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/__init__.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_defaults.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4604 2023-09-15 17:50:42.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_deprecations.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7024 2023-11-28 14:15:09.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_deriv_errors.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_errors.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_exceptions.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    12436 2023-09-15 17:50:42.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_ipopt_funcs.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_options.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    21685 2023-11-28 14:15:09.000000 cyipopt-1.4.0/cyipopt/tests/unit/test_scipy_optional.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2854 2020-12-22 10:59:03.000000 cyipopt-1.4.0/cyipopt/utils.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      274 2024-04-01 15:15:05.000000 cyipopt-1.4.0/cyipopt/version.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.094451 cyipopt-1.4.0/cyipopt.egg-info/
--rw-r--r--   0 moorepants  (1000) moorepants  (1000)     3950 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/PKG-INFO
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1319 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/SOURCES.txt
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        1 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/dependency_links.txt
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        1 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/not-zip-safe
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       14 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/requires.txt
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       28 2024-04-01 15:17:26.000000 cyipopt-1.4.0/cyipopt.egg-info/top_level.txt
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/docs/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5577 2020-12-22 10:59:03.000000 cyipopt-1.4.0/docs/Makefile
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5107 2020-12-22 10:59:03.000000 cyipopt-1.4.0/docs/make.bat
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       28 2023-11-28 14:15:09.000000 cyipopt-1.4.0/docs/requirements.txt
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/docs/source/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8540 2024-04-01 15:14:42.000000 cyipopt-1.4.0/docs/source/conf.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1083 2021-07-18 06:03:56.000000 cyipopt-1.4.0/docs/source/development.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1433 2024-04-01 15:14:42.000000 cyipopt-1.4.0/docs/source/index.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    18639 2023-11-28 14:15:09.000000 cyipopt-1.4.0/docs/source/install.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      514 2023-09-15 18:27:54.000000 cyipopt-1.4.0/docs/source/reference.rst
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    18795 2024-04-01 14:35:21.000000 cyipopt-1.4.0/docs/source/tutorial.rst
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/examples/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4237 2024-04-01 15:14:42.000000 cyipopt-1.4.0/examples/exception_handling.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3912 2024-04-01 15:14:42.000000 cyipopt-1.4.0/examples/hs071.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1996 2022-11-28 12:13:07.000000 cyipopt-1.4.0/examples/hs071_scipy_jax.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5051 2024-04-01 15:14:42.000000 cyipopt-1.4.0/examples/lasso.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      168 2024-04-01 14:39:01.000000 cyipopt-1.4.0/examples/rosen.py
-drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-01 15:17:26.098451 cyipopt-1.4.0/ipopt/
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      486 2020-12-22 10:59:03.000000 cyipopt-1.4.0/ipopt/__init__.py
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      133 2023-11-28 14:15:09.000000 cyipopt-1.4.0/pyproject.toml
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       38 2024-04-01 15:17:26.098451 cyipopt-1.4.0/setup.cfg
--rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8286 2024-04-01 15:14:42.000000 cyipopt-1.4.0/setup.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.098017 cyipopt-1.4.1/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      962 2024-04-02 16:17:13.000000 cyipopt-1.4.1/AUTHORS
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7974 2024-04-02 17:08:41.000000 cyipopt-1.4.1/CHANGELOG.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    14199 2023-02-19 14:17:20.000000 cyipopt-1.4.1/LICENSE
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      373 2024-04-02 16:17:13.000000 cyipopt-1.4.1/MANIFEST.in
+-rw-r--r--   0 moorepants  (1000) moorepants  (1000)     3950 2024-04-02 17:15:48.098017 cyipopt-1.4.1/PKG-INFO
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3082 2023-09-15 17:50:42.000000 cyipopt-1.4.1/README.rst
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.094017 cyipopt-1.4.1/cyipopt/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      399 2024-04-02 16:17:13.000000 cyipopt-1.4.1/cyipopt/__init__.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.094017 cyipopt-1.4.1/cyipopt/cython/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8683 2023-09-15 17:50:42.000000 cyipopt-1.4.1/cyipopt/cython/ipopt.pxd
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    46831 2024-04-02 16:33:50.000000 cyipopt-1.4.1/cyipopt/cython/ipopt_wrapper.pyx
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1356 2024-04-02 16:17:13.000000 cyipopt-1.4.1/cyipopt/exceptions.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2548 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/ipopt_wrapper.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    27367 2024-04-02 16:17:13.000000 cyipopt-1.4.1/cyipopt/scipy_interface.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.094017 cyipopt-1.4.1/cyipopt/tests/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/tests/__init__.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     6366 2023-09-15 17:50:42.000000 cyipopt-1.4.1/cyipopt/tests/conftest.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.094017 cyipopt-1.4.1/cyipopt/tests/integration/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/tests/integration/__init__.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8459 2024-04-02 16:28:32.000000 cyipopt-1.4.1/cyipopt/tests/integration/test_hs071.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/tests/integration/test_lasso.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/tests/integration/test_rosen.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.098017 cyipopt-1.4.1/cyipopt/tests/unit/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/tests/unit/__init__.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/tests/unit/test_defaults.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4604 2023-09-15 17:50:42.000000 cyipopt-1.4.1/cyipopt/tests/unit/test_deprecations.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     7024 2023-11-28 14:15:09.000000 cyipopt-1.4.1/cyipopt/tests/unit/test_deriv_errors.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/tests/unit/test_errors.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/tests/unit/test_exceptions.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    13569 2024-04-02 17:05:33.000000 cyipopt-1.4.1/cyipopt/tests/unit/test_ipopt_funcs.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        0 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/tests/unit/test_options.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    21685 2024-04-02 16:17:13.000000 cyipopt-1.4.1/cyipopt/tests/unit/test_scipy_optional.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     2854 2020-12-22 10:59:03.000000 cyipopt-1.4.1/cyipopt/utils.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      274 2024-04-02 17:08:52.000000 cyipopt-1.4.1/cyipopt/version.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.098017 cyipopt-1.4.1/cyipopt.egg-info/
+-rw-r--r--   0 moorepants  (1000) moorepants  (1000)     3950 2024-04-02 17:15:48.000000 cyipopt-1.4.1/cyipopt.egg-info/PKG-INFO
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1319 2024-04-02 17:15:48.000000 cyipopt-1.4.1/cyipopt.egg-info/SOURCES.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        1 2024-04-02 17:15:48.000000 cyipopt-1.4.1/cyipopt.egg-info/dependency_links.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)        1 2024-04-02 17:15:48.000000 cyipopt-1.4.1/cyipopt.egg-info/not-zip-safe
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       14 2024-04-02 17:15:48.000000 cyipopt-1.4.1/cyipopt.egg-info/requires.txt
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       28 2024-04-02 17:15:48.000000 cyipopt-1.4.1/cyipopt.egg-info/top_level.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.098017 cyipopt-1.4.1/docs/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5577 2020-12-22 10:59:03.000000 cyipopt-1.4.1/docs/Makefile
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5107 2020-12-22 10:59:03.000000 cyipopt-1.4.1/docs/make.bat
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       28 2023-11-28 14:15:09.000000 cyipopt-1.4.1/docs/requirements.txt
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.098017 cyipopt-1.4.1/docs/source/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8540 2024-04-02 16:17:13.000000 cyipopt-1.4.1/docs/source/conf.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1083 2021-07-18 06:03:56.000000 cyipopt-1.4.1/docs/source/development.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1433 2024-04-02 16:17:13.000000 cyipopt-1.4.1/docs/source/index.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    18639 2024-04-02 16:17:13.000000 cyipopt-1.4.1/docs/source/install.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      514 2023-09-15 18:27:54.000000 cyipopt-1.4.1/docs/source/reference.rst
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)    18795 2024-04-02 16:17:13.000000 cyipopt-1.4.1/docs/source/tutorial.rst
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.098017 cyipopt-1.4.1/examples/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     4237 2024-04-02 16:17:13.000000 cyipopt-1.4.1/examples/exception_handling.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     3912 2024-04-02 16:17:13.000000 cyipopt-1.4.1/examples/hs071.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     1996 2022-11-28 12:13:07.000000 cyipopt-1.4.1/examples/hs071_scipy_jax.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     5051 2024-04-02 16:17:13.000000 cyipopt-1.4.1/examples/lasso.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      168 2024-04-01 14:39:01.000000 cyipopt-1.4.1/examples/rosen.py
+drwxrwxr-x   0 moorepants  (1000) moorepants  (1000)        0 2024-04-02 17:15:48.098017 cyipopt-1.4.1/ipopt/
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      486 2020-12-22 10:59:03.000000 cyipopt-1.4.1/ipopt/__init__.py
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)      133 2024-04-02 16:17:13.000000 cyipopt-1.4.1/pyproject.toml
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)       38 2024-04-02 17:15:48.098017 cyipopt-1.4.1/setup.cfg
+-rw-rw-r--   0 moorepants  (1000) moorepants  (1000)     8286 2024-04-02 16:17:13.000000 cyipopt-1.4.1/setup.py
```

### Comparing `cyipopt-1.4.0/AUTHORS` & `cyipopt-1.4.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/CHANGELOG.rst` & `cyipopt-1.4.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 - Removed - for now removed features.
 - Fixed - for any bug fixes.
 - Security - in case of vulnerabilities.
 
 Version History
 ---------------
 
+[1.4.1] - 2024-04-02
+~~~~~~~~~~~~~~~~~~~~
+
+Fixed
++++++
+
+- Addressed regression in return value of ``intermediate_cb``. #250
+
 [1.4.0] - 2024-04-01
 ~~~~~~~~~~~~~~~~~~~~
 
 Added
 +++++
 
 - Support for building with Cython 3. #227, #240
```

### Comparing `cyipopt-1.4.0/LICENSE` & `cyipopt-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/PKG-INFO` & `cyipopt-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyipopt
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Cython wrapper to the IPOPT optimization package
 Home-page: https://github.com/mechmotum/cyipopt
 Author: Jason K. Moore
 Author-email: moorepants@gmail.com
 License: EPL-2.0
 Keywords: coin-or,interior-point,ipopt,nlp,nonlinear programming,optimization
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cyipopt-1.4.0/README.rst` & `cyipopt-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/cython/ipopt.pxd` & `cyipopt-1.4.1/cyipopt/cython/ipopt.pxd`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/cython/ipopt_wrapper.pyx` & `cyipopt-1.4.1/cyipopt/cython/ipopt_wrapper.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1274,15 +1274,15 @@
 
         if ret_val is None:
             return True
     except:
         self.__exception = sys.exc_info()
         return True
 
-    return True
+    return ret_val
 
 
 class problem(Problem):
     """Class to continue support for old API.
 
     .. deprecated:: 1.0.0
        :class:`problem` will be removed in CyIpopt 1.1.0, it is replaced by
```

### Comparing `cyipopt-1.4.0/cyipopt/exceptions.py` & `cyipopt-1.4.1/cyipopt/exceptions.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/ipopt_wrapper.py` & `cyipopt-1.4.1/cyipopt/ipopt_wrapper.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/scipy_interface.py` & `cyipopt-1.4.1/cyipopt/scipy_interface.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/tests/conftest.py` & `cyipopt-1.4.1/cyipopt/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/tests/integration/test_hs071.py` & `cyipopt-1.4.1/cyipopt/tests/integration/test_hs071.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/tests/unit/test_deprecations.py` & `cyipopt-1.4.1/cyipopt/tests/unit/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/tests/unit/test_deriv_errors.py` & `cyipopt-1.4.1/cyipopt/tests/unit/test_deriv_errors.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/tests/unit/test_ipopt_funcs.py` & `cyipopt-1.4.1/cyipopt/tests/unit/test_ipopt_funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -387,7 +387,55 @@
     #
     iter_count = iter_counts[-1]
     assert len(pr_violations) == (1 + iter_count)
     assert len(du_violations) == (1 + iter_count)
 
     np.testing.assert_allclose(pr_violations[-1], np.zeros(m), atol=1e-8)
     np.testing.assert_allclose(du_violations[-1], np.zeros(n), atol=1e-8)
+
+
+def test_intermediate_cb(
+    hs071_initial_guess_fixture,
+    hs071_definition_instance_fixture,
+    hs071_variable_lower_bounds_fixture,
+    hs071_variable_upper_bounds_fixture,
+    hs071_constraint_lower_bounds_fixture,
+    hs071_constraint_upper_bounds_fixture,
+):
+    x0 = hs071_initial_guess_fixture
+    lb = hs071_variable_lower_bounds_fixture
+    ub = hs071_variable_upper_bounds_fixture
+    cl = hs071_constraint_lower_bounds_fixture
+    cu = hs071_constraint_upper_bounds_fixture
+    n = len(x0)
+    m = len(cl)
+
+    problem_definition = hs071_definition_instance_fixture
+
+    def intermediate(
+        alg_mod,
+        iter_count,
+        obj_value,
+        inf_pr,
+        inf_du,
+        mu,
+        d_norm,
+        regularization_size,
+        alpha_du,
+        alpha_pr,
+        ls_trials,
+    ):
+        return False
+
+    problem_definition.intermediate = intermediate
+
+    nlp = cyipopt.Problem(
+        n=n,
+        m=m,
+        problem_obj=problem_definition,
+        lb=lb,
+        ub=ub,
+        cl=cl,
+        cu=cu,
+    )
+    x, info = nlp.solve(x0)
+    assert b'premature termination' in info['status_msg']
```

### Comparing `cyipopt-1.4.0/cyipopt/tests/unit/test_scipy_optional.py` & `cyipopt-1.4.1/cyipopt/tests/unit/test_scipy_optional.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt/utils.py` & `cyipopt-1.4.1/cyipopt/utils.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/cyipopt.egg-info/PKG-INFO` & `cyipopt-1.4.1/cyipopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyipopt
-Version: 1.4.0
+Version: 1.4.1
 Summary: A Cython wrapper to the IPOPT optimization package
 Home-page: https://github.com/mechmotum/cyipopt
 Author: Jason K. Moore
 Author-email: moorepants@gmail.com
 License: EPL-2.0
 Keywords: coin-or,interior-point,ipopt,nlp,nonlinear programming,optimization
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cyipopt-1.4.0/cyipopt.egg-info/SOURCES.txt` & `cyipopt-1.4.1/cyipopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/docs/Makefile` & `cyipopt-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/docs/make.bat` & `cyipopt-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/docs/source/conf.py` & `cyipopt-1.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/docs/source/development.rst` & `cyipopt-1.4.1/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/docs/source/index.rst` & `cyipopt-1.4.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/docs/source/install.rst` & `cyipopt-1.4.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/docs/source/reference.rst` & `cyipopt-1.4.1/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/docs/source/tutorial.rst` & `cyipopt-1.4.1/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/examples/exception_handling.py` & `cyipopt-1.4.1/examples/exception_handling.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/examples/hs071.py` & `cyipopt-1.4.1/examples/hs071.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/examples/hs071_scipy_jax.py` & `cyipopt-1.4.1/examples/hs071_scipy_jax.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/examples/lasso.py` & `cyipopt-1.4.1/examples/lasso.py`

 * *Files identical despite different names*

### Comparing `cyipopt-1.4.0/setup.py` & `cyipopt-1.4.1/setup.py`

 * *Files identical despite different names*

