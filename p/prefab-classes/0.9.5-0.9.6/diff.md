# Comparing `tmp/prefab_classes-0.9.5.tar.gz` & `tmp/prefab_classes-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefab_classes-0.9.5.tar", last modified: Wed Sep 20 10:18:01 2023, max compression
+gzip compressed data, was "prefab_classes-0.9.6.tar", last modified: Mon Nov 20 12:30:40 2023, max compression
```

## Comparing `prefab_classes-0.9.5.tar` & `prefab_classes-0.9.6.tar`

### file list

```diff
@@ -1,37 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 10:18:01.130360 prefab_classes-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2023-09-20 10:18:01.130360 prefab_classes-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-20 10:18:01.130360 prefab_classes-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 10:18:01.122360 prefab_classes-0.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 10:18:01.126360 prefab_classes-0.9.5/src/prefab_classes/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 10:18:01.126360 prefab_classes-0.9.5/src/prefab_classes/compiled/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/compiled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40746 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/compiled/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/compiled/rewrite_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 10:18:01.126360 prefab_classes-0.9.5/src/prefab_classes/dynamic/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/dynamic/_attribute_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 10:18:01.126360 prefab_classes-0.9.5/src/prefab_classes/dynamic/_attribute_class_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/dynamic/autogen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11293 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/dynamic/method_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)    15519 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/dynamic/prefab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes/sentinels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 10:18:01.126360 prefab_classes-0.9.5/src/prefab_classes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2023-09-20 10:18:01.000000 prefab_classes-0.9.5/src/prefab_classes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-09-20 10:18:01.000000 prefab_classes-0.9.5/src/prefab_classes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-20 10:18:01.000000 prefab_classes-0.9.5/src/prefab_classes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-09-20 10:18:01.000000 prefab_classes-0.9.5/src/prefab_classes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-09-20 10:18:01.000000 prefab_classes-0.9.5/src/prefab_classes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 10:18:01.126360 prefab_classes-0.9.5/src/prefab_classes_hook/
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/src/prefab_classes_hook/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-20 10:18:01.126360 prefab_classes-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2023-09-20 10:17:49.000000 prefab_classes-0.9.5/tests/test_versions_match.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.871753 prefab_classes-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2023-11-20 12:30:40.871753 prefab_classes-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.855753 prefab_classes-0.9.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4931 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/compiled_construction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/dynamic_and_compiled.md
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/dynamic_construction.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14647 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/evil_imports.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.855753 prefab_classes-0.9.6/docs/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/extra/dataclasses_differences.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/extra/performance_tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/pre_post_init.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/docs/why_not_dataclasses.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 12:30:40.871753 prefab_classes-0.9.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.851753 prefab_classes-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.859753 prefab_classes-0.9.6/src/prefab_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.859753 prefab_classes-0.9.6/src/prefab_classes/compiled/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/compiled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40746 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/compiled/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/compiled/rewrite_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.859753 prefab_classes-0.9.6/src/prefab_classes/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/dynamic/_attribute_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.859753 prefab_classes-0.9.6/src/prefab_classes/dynamic/_attribute_class_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/dynamic/autogen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11293 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/dynamic/method_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15519 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/dynamic/prefab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes/sentinels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.859753 prefab_classes-0.9.6/src/prefab_classes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2023-11-20 12:30:40.000000 prefab_classes-0.9.6/src/prefab_classes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2023-11-20 12:30:40.000000 prefab_classes-0.9.6/src/prefab_classes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 12:30:40.000000 prefab_classes-0.9.6/src/prefab_classes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-20 12:30:40.000000 prefab_classes-0.9.6/src/prefab_classes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-20 12:30:40.000000 prefab_classes-0.9.6/src/prefab_classes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.859753 prefab_classes-0.9.6/src/prefab_classes_hook/
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/src/prefab_classes_hook/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.859753 prefab_classes-0.9.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.863753 prefab_classes-0.9.6/tests/compiled/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.863753 prefab_classes-0.9.6/tests/compiled/compile_targets/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_import_clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_import_clear2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_import_clear3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_import_clear4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_import_noclear_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_import_noclear_dynamic2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_import_noclear_makeprefab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_importfail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_mixed_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_no_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_plain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_to_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/compile_targets/example_to_compile_expected.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/test_clearimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/test_import_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/test_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/test_resulting_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/test_rewrite_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/compiled/test_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.863753 prefab_classes-0.9.6/tests/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/dynamic/test_attribute_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/dynamic/test_dynamic_construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/dynamic/test_dynamic_internals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.867753 prefab_classes-0.9.6/tests/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.867753 prefab_classes-0.9.6/tests/shared/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/config_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/creation_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/dunders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 12:30:40.871753 prefab_classes-0.9.6/tests/shared/examples/fails/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/fails/creation_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/fails/creation_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/fails/creation_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/fails/creation_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/fails/inheritance_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/fails/inheritance_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/frozen_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/funcs_prefabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/init_ex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/examples/repr_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_dunders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_hint_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/shared/test_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2023-11-20 12:30:30.000000 prefab_classes-0.9.6/tests/test_versions_match.py
```

### Comparing `prefab_classes-0.9.5/LICENSE.md` & `prefab_classes-0.9.6/LICENSE.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # License #
 # Prefab Classes License #
 
 ```
 MIT License
 
-Copyright (c) 2022 David C Ellis
+Copyright (c) 2022-2023 David C Ellis
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -54,15 +54,15 @@
 greater good.
 ```
 
 
 ### PSF License for Python ###
 
 This isn't here just because this is a python project:
-the `PrefabHacker.get_code` method in `src/prefab_classes/compiled/import_hook.py`
+the `PrefabHacker.get_code` method in `src/prefab_classes_hook/__init__.py`
 is a modified copy of the `SourceLoader.get_code` method in
 [_bootstrap_external.py](https://github.com/python/cpython/blob/85dd6cb6df996b1197266d1a50ecc9187a91e481/Lib/importlib/_bootstrap_external.py#L1074)
 
 The whole method needed to be modified to generate the different hash for mutual
 invalidation.
 
 Full License: https://github.com/python/cpython/blob/main/LICENSE
```

### Comparing `prefab_classes-0.9.5/README.md` & `prefab_classes-0.9.6/README.md`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/pyproject.toml` & `prefab_classes-0.9.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 readme="README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
-    "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ['version']
+license = {file = "LICENSE.md"}
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
 version = {attr = "prefab_classes.__version__"}
```

### Comparing `prefab_classes-0.9.5/src/prefab_classes/_typing.py` & `prefab_classes-0.9.6/src/prefab_classes/_typing.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/compiled/generator.py` & `prefab_classes-0.9.6/src/prefab_classes/compiled/generator.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/compiled/rewrite_source.py` & `prefab_classes-0.9.6/src/prefab_classes/compiled/rewrite_source.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/dynamic/_attribute_class.py` & `prefab_classes-0.9.6/src/prefab_classes/dynamic/_attribute_class.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py` & `prefab_classes-0.9.6/src/prefab_classes/dynamic/_attribute_class_maker/_attribute_template.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py` & `prefab_classes-0.9.6/src/prefab_classes/dynamic/_attribute_class_maker/regenerate_attribute.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/dynamic/autogen.py` & `prefab_classes-0.9.6/src/prefab_classes/dynamic/autogen.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/dynamic/method_generators.py` & `prefab_classes-0.9.6/src/prefab_classes/dynamic/method_generators.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/dynamic/prefab.py` & `prefab_classes-0.9.6/src/prefab_classes/dynamic/prefab.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/exceptions.py` & `prefab_classes-0.9.6/src/prefab_classes/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes/funcs.py` & `prefab_classes-0.9.6/src/prefab_classes/funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,26 +124,29 @@
     inst,
     *,
     excludes: None | tuple[str, ...] = None,
     dumps_func: None | Callable[..., str] = None,  # noqa: false pycharm error
     **kwargs,
 ) -> str:
     """
-    Output the class attributes as JSON
+    Output the instance attributes as JSON.
 
-    If no dumps function it will attempt to reuse the basic encoder
+    If no dumps function is given and no kwargs are used a basic
+    encoder will be reused.
 
     :param inst: instance of prefab class
     :param excludes: tuple of attribute names to exclude from json
+                     caching used internally requires this to be a tuple
+                     and not a list
                      **note that these attribute names will be excluded
                      from all prefabs encountered during serialization**
     :param dumps_func: function equivalent to stdlib's json.dumps
-                       making it easier to use third party json libraries.
+                       making it easier to use third party json libraries
     :param kwargs: keyword arguments passed directly to dumps_func
-    :return: String of JSON data from the class attributes
+    :return: string of JSON data from the class attributes
     """
     if dumps_func is None and not kwargs:
         encoder = _get_json_encoder(excludes)
         return encoder.encode(inst)
     else:
         default = kwargs.pop("default", None)
```

### Comparing `prefab_classes-0.9.5/src/prefab_classes/sentinels.py` & `prefab_classes-0.9.6/src/prefab_classes/sentinels.py`

 * *Files identical despite different names*

### Comparing `prefab_classes-0.9.5/src/prefab_classes_hook/__init__.py` & `prefab_classes-0.9.6/src/prefab_classes_hook/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 # We probably shouldn't be importing from here, but it also halves the import time.
 try:
     from _frozen_importlib_external import PathFinder, SourceFileLoader  # type: ignore
 except ImportError:
     from importlib.machinery import PathFinder, SourceFileLoader
 
-__version__ = "v0.9.5"
-PREFAB_MAGIC_BYTES = b"PREFAB_CLASSES_v0.9.5"
+__version__ = "v0.9.6"
+PREFAB_MAGIC_BYTES = b"PREFAB_CLASSES_v0.9.6"
 
 __all__ = ["prefab_compiler", "insert_prefab_importhook", "remove_prefab_importhook"]
 
 
 HOOK_REWRITE = "# COMPILE_PREFABS"
```

