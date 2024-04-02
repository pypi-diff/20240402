# Comparing `tmp/pytest-order-1.2.0.tar.gz` & `tmp/pytest-order-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-order-1.2.0.tar", last modified: Sat Nov 18 12:23:15 2023, max compression
+gzip compressed data, was "pytest-order-1.2.1.tar", last modified: Tue Apr  2 19:09:00 2024, max compression
```

## Comparing `pytest-order-1.2.0.tar` & `pytest-order-1.2.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.452074 pytest-order-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-11-18 12:23:06.000000 pytest-order-1.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     8605 2023-11-18 12:23:06.000000 pytest-order-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-11-18 12:23:06.000000 pytest-order-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-11-18 12:23:06.000000 pytest-order-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2023-11-18 12:23:15.452074 pytest-order-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2023-11-18 12:23:06.000000 pytest-order-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.440074 pytest-order-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2023-11-18 12:23:06.000000 pytest-order-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6722 2023-11-18 12:23:06.000000 pytest-order-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-18 12:23:06.000000 pytest-order-1.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.444074 pytest-order-1.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     8620 2023-11-18 12:23:06.000000 pytest-order-1.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18126 2023-11-18 12:23:06.000000 pytest-order-1.2.0/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-11-18 12:23:06.000000 pytest-order-1.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2023-11-18 12:23:06.000000 pytest-order-1.2.0/docs/source/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2023-11-18 12:23:06.000000 pytest-order-1.2.0/docs/source/other_plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12936 2023-11-18 12:23:06.000000 pytest-order-1.2.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.444074 pytest-order-1.2.0/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.440074 pytest-order-1.2.0/example/order_scope_level/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.444074 pytest-order-1.2.0/example/order_scope_level/feature1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/order_scope_level/feature1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/order_scope_level/feature1/test_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/order_scope_level/feature1/test_b.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.444074 pytest-order-1.2.0/example/order_scope_level/feature2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/order_scope_level/feature2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/order_scope_level/feature2/test_a.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/order_scope_level/feature2/test_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_combined.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_module1.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_module2.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_module_a.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.448074 pytest-order-1.2.0/example/test_module_c/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_module_c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_module_c/test_submodule.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_modules_b.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_ordinal_class_mark.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_ordinals.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_quickstart.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_relative.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_relative_class_marker.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_sort_breaks_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_sort_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2023-11-18 12:23:06.000000 pytest-order-1.2.0/example/test_sparse_ordering.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.448074 pytest-order-1.2.0/pytest_order/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-18 12:23:06.000000 pytest-order-1.2.0/pytest_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7545 2023-11-18 12:23:06.000000 pytest-order-1.2.0/pytest_order/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2023-11-18 12:23:06.000000 pytest-order-1.2.0/pytest_order/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2023-11-18 12:23:06.000000 pytest-order-1.2.0/pytest_order/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    20664 2023-11-18 12:23:06.000000 pytest-order-1.2.0/pytest_order/sorter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.448074 pytest-order-1.2.0/pytest_order.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7636 2023-11-18 12:23:15.000000 pytest-order-1.2.0/pytest_order.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-11-18 12:23:15.000000 pytest-order-1.2.0/pytest_order.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 12:23:15.000000 pytest-order-1.2.0/pytest_order.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-18 12:23:15.000000 pytest-order-1.2.0/pytest_order.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2023-11-18 12:23:15.000000 pytest-order-1.2.0/pytest_order.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-18 12:23:15.000000 pytest-order-1.2.0/pytest_order.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-11-18 12:23:15.452074 pytest-order-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-11-18 12:23:06.000000 pytest-order-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:15.452074 pytest-order-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_class_marks.py
--rw-r--r--   0 runner    (1001) docker     (127)    13256 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_indulgent_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_marker_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_multiple_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_order_group_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_order_group_scope_dep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_order_group_scope_named_dep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_order_group_scope_relative.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_order_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_order_scope_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     7633 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_relative_ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_sparse_ordinals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tests/test_xdist_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-11-18 12:23:06.000000 pytest-order-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.307364 pytest-order-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-02 19:08:49.000000 pytest-order-1.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-02 19:08:49.000000 pytest-order-1.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-02 19:08:49.000000 pytest-order-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-02 19:08:49.000000 pytest-order-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-02 19:09:00.307364 pytest-order-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6184 2024-04-02 19:08:49.000000 pytest-order-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.299364 pytest-order-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-02 19:08:49.000000 pytest-order-1.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-02 19:08:49.000000 pytest-order-1.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 19:08:49.000000 pytest-order-1.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.299364 pytest-order-1.2.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-04-02 19:08:49.000000 pytest-order-1.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18126 2024-04-02 19:08:49.000000 pytest-order-1.2.1/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 19:08:49.000000 pytest-order-1.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-02 19:08:49.000000 pytest-order-1.2.1/docs/source/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-04-02 19:08:49.000000 pytest-order-1.2.1/docs/source/other_plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12936 2024-04-02 19:08:49.000000 pytest-order-1.2.1/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.303364 pytest-order-1.2.1/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.295364 pytest-order-1.2.1/example/order_scope_level/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.303364 pytest-order-1.2.1/example/order_scope_level/feature1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/order_scope_level/feature1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/order_scope_level/feature1/test_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/order_scope_level/feature1/test_b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.303364 pytest-order-1.2.1/example/order_scope_level/feature2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/order_scope_level/feature2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/order_scope_level/feature2/test_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/order_scope_level/feature2/test_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_module2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_module_a.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.303364 pytest-order-1.2.1/example/test_module_c/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_module_c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_module_c/test_submodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_modules_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_ordinal_class_mark.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_relative.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_relative_class_marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_sort_breaks_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_sort_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-02 19:08:49.000000 pytest-order-1.2.1/example/test_sparse_ordering.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.303364 pytest-order-1.2.1/pytest_order/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 19:08:49.000000 pytest-order-1.2.1/pytest_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7545 2024-04-02 19:08:49.000000 pytest-order-1.2.1/pytest_order/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-02 19:08:49.000000 pytest-order-1.2.1/pytest_order/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-02 19:08:49.000000 pytest-order-1.2.1/pytest_order/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21385 2024-04-02 19:08:49.000000 pytest-order-1.2.1/pytest_order/sorter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.307364 pytest-order-1.2.1/pytest_order.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-02 19:09:00.000000 pytest-order-1.2.1/pytest_order.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-02 19:09:00.000000 pytest-order-1.2.1/pytest_order.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:09:00.000000 pytest-order-1.2.1/pytest_order.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 19:09:00.000000 pytest-order-1.2.1/pytest_order.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-02 19:09:00.000000 pytest-order-1.2.1/pytest_order.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 19:09:00.000000 pytest-order-1.2.1/pytest_order.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 19:09:00.307364 pytest-order-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-02 19:08:49.000000 pytest-order-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:09:00.307364 pytest-order-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_class_marks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14819 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_indulgent_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_marker_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_multiple_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_order_group_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_order_group_scope_dep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_order_group_scope_named_dep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_order_group_scope_relative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_order_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_order_scope_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_relative_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_sparse_ordinals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tests/test_xdist_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-02 19:08:49.000000 pytest-order-1.2.1/tox.ini
```

### Comparing `pytest-order-1.2.0/CHANGELOG.md` & `pytest-order-1.2.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # pytest-order Release Notes
 
+## [Version 1.2.1](https://pypi.org/project/pytest-order/1.2.1/) (2024-04-02)
+Bugfix release.
+
+## Fixes
+- handle dependency markers with the same alias name (see [#71](https://github.com/pytest-dev/pytest-order/issues/71))
+- specify rootdir to recursive pytest calls to avoid searching a large directory tree unnecessarily (see [#110](https://github.com/pytest-dev/pytest-order/issues/110))
+
+## Infrastructure
+- avoid unknown marker warning in tests (see [#101](https://github.com/pytest-dev/pytest-order/issues/101))
+- added pytest 8 to CI tests
+
 ## [Version 1.2.0](https://pypi.org/project/pytest-order/1.2.0/) (2023-11-18)
 Allows using custom markers for ordering.
 
 ### New features
-* added option `--order-marker-prefix` to allow using custom markers for ordering
+- added option `--order-marker-prefix` to allow using custom markers for ordering
 
 ### Infrastructure
 - added pre-commit hook for linters
 - added Python 3.12 to supported versions
 
 ## [Version 1.1.0](https://pypi.org/project/pytest-order/1.1.0/) (2023-03-10)
 Adds support for executing tests more than once using order marks.
```

### Comparing `pytest-order-1.2.0/LICENSE` & `pytest-order-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/PKG-INFO` & `pytest-order-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-order
-Version: 1.2.0
+Version: 1.2.1
 Summary: pytest plugin to run your tests in a specific order
 Home-page: https://github.com/pytest-dev/pytest-order
 Author: mrbean-bremen
 Author-email: hansemrbean@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -79,15 +79,15 @@
 - ordering tests with `pytest-dependency` markers if using the
   [order-dependencies](https://pytest-order.readthedocs.io/en/stable/configuration.html#order-dependencies) option,
   more information about `pytest-dependency` compatibility
   [here](https://pytest-order.readthedocs.io/en/stable/other_plugins.html#relationship-with-pytest-dependency)
 - sparse ordering of tests via the
   [sparse-ordering](https://pytest-order.readthedocs.io/en/stable/configuration.html#sparse-ordering) option
 - usage of custom markers for ordering using the
-  [sparse-ordering](https://pytest-order.readthedocs.io/en/stable/configuration.html#order-marker-prefix) option
+  [order-marker-prefix](https://pytest-order.readthedocs.io/en/stable/configuration.html#order-marker-prefix) option
 
 Overview
 --------
 _(adapted from the original project)_
 
 Have you ever wanted to easily run one of your tests before any others run?
 Or run some tests last? Or run this one test before that other test? Or
```

### Comparing `pytest-order-1.2.0/README.md` & `pytest-order-1.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 - ordering tests with `pytest-dependency` markers if using the
   [order-dependencies](https://pytest-order.readthedocs.io/en/stable/configuration.html#order-dependencies) option,
   more information about `pytest-dependency` compatibility
   [here](https://pytest-order.readthedocs.io/en/stable/other_plugins.html#relationship-with-pytest-dependency)
 - sparse ordering of tests via the
   [sparse-ordering](https://pytest-order.readthedocs.io/en/stable/configuration.html#sparse-ordering) option
 - usage of custom markers for ordering using the
-  [sparse-ordering](https://pytest-order.readthedocs.io/en/stable/configuration.html#order-marker-prefix) option
+  [order-marker-prefix](https://pytest-order.readthedocs.io/en/stable/configuration.html#order-marker-prefix) option
 
 Overview
 --------
 _(adapted from the original project)_
 
 Have you ever wanted to easily run one of your tests before any others run?
 Or run some tests last? Or run this one test before that other test? Or
```

### Comparing `pytest-order-1.2.0/docs/Makefile` & `pytest-order-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/docs/make.bat` & `pytest-order-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/docs/source/conf.py` & `pytest-order-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/docs/source/configuration.rst` & `pytest-order-1.2.1/docs/source/configuration.rst`

 * *Files 1% similar despite different names*

```diff
@@ -484,15 +484,15 @@
     test_module.py:6: test_a PASSED
 
 This looks redundant and is also error-prone. If you want to order them instead
 just using your own marker (which has the order index already in the name), you can use
 the option ``--order-marker-prefix``. Running the original tests without any order marker
 gives you now::
 
-    $ pytest tests -vv -m "m2 or m3" --order-merker-prefix=m
+    $ pytest tests -vv -m "m2 or m3" --order-marker-prefix=m
     ============================= test session starts ==============================
     ...
     test_module.py:18: test_c PASSED
     test_module.py:6: test_a PASSED
 
 .. note::
   As usually, you are responsible for registering your own markers, either in the
```

### Comparing `pytest-order-1.2.0/docs/source/intro.rst` & `pytest-order-1.2.1/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/docs/source/other_plugins.rst` & `pytest-order-1.2.1/docs/source/other_plugins.rst`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/docs/source/usage.rst` & `pytest-order-1.2.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/pytest_order/item.py` & `pytest-order-1.2.1/pytest_order/item.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/pytest_order/plugin.py` & `pytest-order-1.2.1/pytest_order/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/pytest_order/settings.py` & `pytest-order-1.2.1/pytest_order/settings.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/pytest_order/sorter.py` & `pytest-order-1.2.1/pytest_order/sorter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,21 @@
+import re
 import sys
-from warnings import warn
+from collections import OrderedDict
 from contextlib import suppress
 from typing import Optional, List, Dict, Tuple, cast
+from warnings import warn
 
 from _pytest.config import Config
 from _pytest.mark import Mark
 from _pytest.python import Function
 
 from .item import Item, ItemList, ItemGroup, filter_marks, move_item, RelativeMark
 from .settings import Settings, Scope
 
-try:
-    from typing import OrderedDict
-except ImportError:
-    # In Python <3.7.2, we need to stub it
-    from collections import OrderedDict as OrderedDict_cls
-    from typing import MutableMapping, TypeVar
-
-    KT = TypeVar("KT")
-    VT = TypeVar("VT")
-
-    class OrderedDict(OrderedDict_cls, MutableMapping[KT, VT]):  # type: ignore
-        pass
-
-
 orders_map = {
     "first": 0,
     "second": 1,
     "third": 2,
     "fourth": 3,
     "fifth": 4,
     "sixth": 5,
@@ -108,15 +96,15 @@
                 sorted_list.extend(sorter.sort_items())
         return [item.item for item in sorted_list]
 
     def mark_binning(
         self,
         item: Item,
         dep_marks: Dict[Tuple[str, Scope, str], List[Item]],
-        aliases: Dict[str, Item],
+        aliases: Dict[str, List[Item]],
     ) -> None:
         """
         Collect relevant markers for the given item.
         """
         keys = item.item.keywords.keys()
         has_dependency = "dependency" in keys
         has_order = "order" in keys
@@ -134,15 +122,15 @@
             self.handle_order_marks(item)
 
     def handle_dependency_mark(
         self,
         item: Item,
         has_order: bool,
         dep_marks: Dict[Tuple[str, Scope, str], List[Item]],
-        aliases: Dict[str, Item],
+        aliases: Dict[str, List[Item]],
     ) -> None:
         # always order dependencies if an order mark is present
         # otherwise only if order-dependencies is set
         mark = item.item.get_closest_marker("dependency")
         name_mark = None
         if mark and (self.settings.order_dependencies or has_order):
             dependent_mark = mark.kwargs.get("depends")
@@ -155,15 +143,15 @@
             # we always collect the names of the dependent items, because
             # we need them in both cases
             name_mark = mark.kwargs.get("name")
         # the default name in pytest-dependency is the nodeid or a part
         # of the nodeid, depending on the scope
         if not name_mark:
             name_mark = item.node_id
-        aliases[name_mark] = item
+        aliases.setdefault(name_mark, []).append(item)
 
     def handle_order_marks(self, item: Item) -> None:
         marks = item.item.iter_markers("order")
         for mark in marks:
             self.handle_order_mark(item, mark)
 
     def handle_order_mark(self, item: Item, mark: Mark) -> None:
@@ -285,44 +273,66 @@
     def warn_about_unknown_test(item: Item, rel_mark: str) -> None:
         sys.stdout.write(
             "\nWARNING: cannot execute '{}' relative to others: "
             "'{}' - ignoring the marker.".format(item.item.name, rel_mark)
         )
 
     def collect_markers(self) -> None:
-        aliases: Dict[str, Item] = {}
+        aliases: Dict[str, List[Item]] = {}
         dep_marks: Dict[Tuple[str, Scope, str], List[Item]] = {}
         for item in self.items:
             self.mark_binning(item, dep_marks, aliases)
         self.resolve_dependency_markers(dep_marks, aliases)
 
     def resolve_dependency_markers(
         self,
         dep_marks: Dict[Tuple[str, Scope, str], List[Item]],
-        aliases: Dict[str, Item],
+        aliases: Dict[str, List[Item]],
     ) -> None:
         for (name, _, prefix), items in dep_marks.items():
             if name in aliases:
                 for item in items:
-                    self.dep_marks.append(
-                        RelativeMark(aliases[name], item, move_after=True)
-                    )
+                    alias = self.matching_alias(aliases[name], item)
+                    self.dep_marks.append(RelativeMark(alias, item, move_after=True))
             else:
                 label = "::".join((prefix, name))
                 if label in aliases:
                     for item in items:
+                        alias = self.matching_alias(aliases[label], item)
                         self.dep_marks.append(
-                            RelativeMark(aliases[label], item, move_after=True)
+                            RelativeMark(alias, item, move_after=True)
                         )
                 else:
                     sys.stdout.write(
                         "\nWARNING: Cannot resolve the dependency marker '{}' "
                         "- ignoring it.".format(name)
                     )
 
+    @staticmethod
+    def matching_alias(aliases: List[Item], item: Item) -> Item:
+        if len(aliases) == 1:
+            return aliases[0]
+
+        # handle the rare case that several tests have the same alias name
+        # we use the item that best matches the node id of the dependent item
+        max_matching_parts = 0
+        node_id_parts = re.split("(::|/)", item.node_id)
+        matching_item = aliases[0]
+        for alias_item in aliases:
+            alias_node_id_parts = re.split("(::|/)", alias_item.node_id)
+            nr_matching_parts = 0
+            for n, a in zip(node_id_parts, alias_node_id_parts):
+                if n != a:
+                    break
+                nr_matching_parts += 1
+            if nr_matching_parts > max_matching_parts:
+                max_matching_parts = nr_matching_parts
+                matching_item = alias_item
+        return matching_item
+
 
 def module_item_groups(items: List[Item]) -> Dict[str, List[Item]]:
     """
     Split items into groups per module.
     """
     module_items: OrderedDict[str, List[Item]] = OrderedDict()
     for item in items:
```

### Comparing `pytest-order-1.2.0/pytest_order.egg-info/PKG-INFO` & `pytest-order-1.2.1/pytest_order.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-order
-Version: 1.2.0
+Version: 1.2.1
 Summary: pytest plugin to run your tests in a specific order
 Home-page: https://github.com/pytest-dev/pytest-order
 Author: mrbean-bremen
 Author-email: hansemrbean@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -79,15 +79,15 @@
 - ordering tests with `pytest-dependency` markers if using the
   [order-dependencies](https://pytest-order.readthedocs.io/en/stable/configuration.html#order-dependencies) option,
   more information about `pytest-dependency` compatibility
   [here](https://pytest-order.readthedocs.io/en/stable/other_plugins.html#relationship-with-pytest-dependency)
 - sparse ordering of tests via the
   [sparse-ordering](https://pytest-order.readthedocs.io/en/stable/configuration.html#sparse-ordering) option
 - usage of custom markers for ordering using the
-  [sparse-ordering](https://pytest-order.readthedocs.io/en/stable/configuration.html#order-marker-prefix) option
+  [order-marker-prefix](https://pytest-order.readthedocs.io/en/stable/configuration.html#order-marker-prefix) option
 
 Overview
 --------
 _(adapted from the original project)_
 
 Have you ever wanted to easily run one of your tests before any others run?
 Or run some tests last? Or run this one test before that other test? Or
```

### Comparing `pytest-order-1.2.0/pytest_order.egg-info/SOURCES.txt` & `pytest-order-1.2.1/pytest_order.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/setup.py` & `pytest-order-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/conftest.py` & `pytest-order-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_class_marks.py` & `pytest-order-1.2.1/tests/test_class_marks.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_dependency.py` & `pytest-order-1.2.1/tests/test_dependency.py`

 * *Files 4% similar despite different names*

```diff
@@ -395,14 +395,69 @@
             "test_ndep2.py::test_one PASSED",
             "test_ndep1.py::Test1::test_two PASSED",
             "test_ndep2.py::test_two PASSED",
         ]
     )
 
 
+def test_equally_named_dependency_in_modules(test_path):
+    # regression test for #71
+    test_path.makepyfile(
+        test_ndep1=(
+            """
+            import pytest
+
+            class TestOne:
+
+                @pytest.mark.dependency(name="one", depends=["zero"])
+                def test_one(self):
+                    assert True
+
+                @pytest.mark.dependency(name="two", depends=["one"])
+                def test_two(self):
+                    assert True
+
+                @pytest.mark.dependency(name="three", depends=["two"])
+                def test_three(self):
+                    assert True
+
+                @pytest.mark.dependency(name="zero")
+                def test_zero(self):
+                    assert True
+            """
+        ),
+        test_ndep2=(
+            """
+            import pytest
+
+            class TestTwo:
+
+                @pytest.mark.dependency(name="one", depends=["zero"])
+                def test_one(self):
+                    assert True
+
+                @pytest.mark.dependency(name="two", depends=["one"])
+                def test_two(self):
+                    assert True
+
+                @pytest.mark.dependency(name="three", depends=["two"])
+                def test_three(self):
+                    assert True
+
+                @pytest.mark.dependency(name="zero")
+                def test_zero(self):
+                    assert True
+            """
+        ),
+    )
+
+    result = test_path.runpytest("-v", "--order-dependencies")
+    result.assert_outcomes(passed=8, failed=0, skipped=0)
+
+
 @pytest.mark.skipif(
     pytest.__version__.startswith("3.7."),
     reason="pytest-dependency < 0.5 does not support session scope",
 )
 def test_dependency_in_modules(test_path):
     test_path.makepyfile(
         test_unnamed_dep1=(
```

### Comparing `pytest-order-1.2.0/tests/test_indulgent_ordering.py` & `pytest-order-1.2.1/tests/test_indulgent_ordering.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_marker_prefix.py` & `pytest-order-1.2.1/tests/test_marker_prefix.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,22 +18,43 @@
         @pytest.mark.my2
         def test_c():
             pass
         """
     )
 
 
+@pytest.fixture(scope="module")
+def conftest_file():
+    yield (
+        """
+        def pytest_configure(config):
+            config.addinivalue_line("markers", "my1: used in marker prefix test")
+            config.addinivalue_line("markers", "my2: used in marker prefix test")
+            config.addinivalue_line("markers", "my3: used in marker prefix test")
+        """
+    )
+
+
 @pytest.fixture
-def marker_test(test_path, marker_test_file):
+def marker_test(test_path, marker_test_file, conftest_file):
+    test_path.makepyfile(conftest=conftest_file)
     test_path.makepyfile(test_marker=marker_test_file)
     yield test_path
 
 
-def test_no_ordering(marker_test_file, item_names_for):
-    assert item_names_for(marker_test_file) == ["test_a", "test_b", "test_c"]
+def test_no_ordering(marker_test):
+    result = marker_test.runpytest("-v")
+    result.assert_outcomes(passed=3, skipped=0)
+    result.stdout.fnmatch_lines(
+        [
+            "test_marker.py::test_a PASSED",
+            "test_marker.py::test_b PASSED",
+            "test_marker.py::test_c PASSED",
+        ]
+    )
 
 
 def test_order_with_marker_prefix(marker_test):
     result = marker_test.runpytest("-v", "--order-marker-prefix=my")
     result.assert_outcomes(passed=3, skipped=0)
     result.stdout.fnmatch_lines(
         [
@@ -106,15 +127,16 @@
             "test_marker.py::test_b PASSED",
             "test_marker.py::test_c PASSED",
             "test_marker.py::test_a PASSED",
         ]
     )
 
 
-def test_mix_marker_prefix_with_order_marks(test_path):
+def test_mix_marker_prefix_with_order_marks(test_path, conftest_file):
+    test_path.makepyfile(conftest=conftest_file)
     test_path.makepyfile(
         test_marker=(
             """
             import pytest
 
             @pytest.mark.order(3)
             def test_a():
```

### Comparing `pytest-order-1.2.0/tests/test_misc.py` & `pytest-order-1.2.1/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_multiple_ordering.py` & `pytest-order-1.2.1/tests/test_multiple_ordering.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_order_group_scope.py` & `pytest-order-1.2.1/tests/test_order_group_scope.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_order_group_scope_dep.py` & `pytest-order-1.2.1/tests/test_order_group_scope_dep.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_order_group_scope_named_dep.py` & `pytest-order-1.2.1/tests/test_order_group_scope_named_dep.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_order_group_scope_relative.py` & `pytest-order-1.2.1/tests/test_order_group_scope_relative.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_order_scope.py` & `pytest-order-1.2.1/tests/test_order_scope.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_order_scope_level.py` & `pytest-order-1.2.1/tests/test_order_scope_level.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_ordering.py` & `pytest-order-1.2.1/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_relative_ordering.py` & `pytest-order-1.2.1/tests/test_relative_ordering.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_sparse_ordinals.py` & `pytest-order-1.2.1/tests/test_sparse_ordinals.py`

 * *Files identical despite different names*

### Comparing `pytest-order-1.2.0/tests/test_xdist_handling.py` & `pytest-order-1.2.1/tests/test_xdist_handling.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 global val
                 assert val == "frog"
                 val = "goat"
             """
             )
         )
     # With `loadfile`, the tests should pass
-    args = ["-n3", "--dist=loadfile", str(tmpdir)]
+    args = ["-n3", "--dist=loadfile", f"--rootdir={tmpdir}", str(tmpdir)]
     ret = pytest.main(args, [pytest_order])
     assert ret == 0
 
     # Without `loadfile`, the tests should fail
-    args = ["-n3", str(tmpdir)]
+    args = ["-n3", f"--rootdir={tmpdir}", str(tmpdir)]
     ret = pytest.main(args, [pytest_order])
     assert ret == 1
```

