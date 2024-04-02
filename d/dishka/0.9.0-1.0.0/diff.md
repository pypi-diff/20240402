# Comparing `tmp/dishka-0.9.0.tar.gz` & `tmp/dishka-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dishka-0.9.0.tar", last modified: Fri Mar 29 11:11:25 2024, max compression
+gzip compressed data, was "dishka-1.0.0.tar", last modified: Tue Apr  2 21:17:26 2024, max compression
```

## Comparing `dishka-0.9.0.tar` & `dishka-1.0.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-03-29 11:11:25.353492 dishka-0.9.0/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11357 2024-01-25 16:39:00.000000 dishka-0.9.0/LICENSE
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12015 2024-03-29 11:11:25.353492 dishka-0.9.0/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11078 2024-03-29 11:10:54.000000 dishka-0.9.0/README.md
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1097 2024-03-29 11:11:03.000000 dishka-0.9.0/pyproject.toml
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-03-29 11:11:25.353492 dishka-0.9.0/setup.cfg
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-03-29 11:11:25.349492 dishka-0.9.0/src/
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-03-29 11:11:25.353492 dishka-0.9.0/src/dishka/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      807 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/__init__.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-03-29 11:11:25.353492 dishka-0.9.0/src/dishka/_adaptix/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      635 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/_adaptix/common.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5323 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/_adaptix/feature_requirement.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-03-29 11:11:25.353492 dishka-0.9.0/src/dishka/_adaptix/type_tools/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      540 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/_adaptix/type_tools/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4756 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/_adaptix/type_tools/basic_utils.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1441 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/_adaptix/type_tools/constants.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3877 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/_adaptix/type_tools/generic_resolver.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1827 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/_adaptix/type_tools/implicit_params.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1059 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/_adaptix/type_tools/norm_utils.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    25734 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/_adaptix/type_tools/normalize_type.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6943 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/async_container.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6592 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/container.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      476 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/container_objects.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-03-29 11:11:25.353492 dishka-0.9.0/src/dishka/dependency_source/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      510 2024-03-19 22:45:31.000000 dishka-0.9.0/src/dishka/dependency_source/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1038 2024-03-19 22:45:31.000000 dishka-0.9.0/src/dishka/dependency_source/alias.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1416 2024-03-19 22:45:31.000000 dishka-0.9.0/src/dishka/dependency_source/composite.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1515 2024-03-19 22:45:31.000000 dishka-0.9.0/src/dishka/dependency_source/context_var.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1324 2024-03-19 22:45:31.000000 dishka-0.9.0/src/dishka/dependency_source/decorator.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2164 2024-03-27 22:27:14.000000 dishka-0.9.0/src/dishka/dependency_source/factory.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      905 2024-03-19 22:45:31.000000 dishka-0.9.0/src/dishka/dependency_source/make_alias.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      678 2024-03-19 22:45:31.000000 dishka-0.9.0/src/dishka/dependency_source/make_context_var.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1462 2024-03-29 11:10:54.000000 dishka-0.9.0/src/dishka/dependency_source/make_decorator.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    15058 2024-03-29 11:10:54.000000 dishka-0.9.0/src/dishka/dependency_source/make_factory.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1949 2024-03-19 22:45:31.000000 dishka-0.9.0/src/dishka/dependency_source/unpack_provides.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-03-29 11:11:25.353492 dishka-0.9.0/src/dishka/entities/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-29 00:39:11.000000 dishka-0.9.0/src/dishka/entities/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       40 2024-02-29 00:39:11.000000 dishka-0.9.0/src/dishka/entities/component.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1111 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/entities/depends_marker.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1123 2024-03-04 22:02:38.000000 dishka-0.9.0/src/dishka/entities/key.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      347 2024-03-19 22:45:31.000000 dishka-0.9.0/src/dishka/entities/provides_marker.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      783 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/entities/scope.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2730 2024-03-26 23:39:41.000000 dishka-0.9.0/src/dishka/error_rendering.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1715 2024-03-04 22:02:38.000000 dishka-0.9.0/src/dishka/exceptions.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3397 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/factory_compiler.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-03-29 11:11:25.353492 dishka-0.9.0/src/dishka/integrations/
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-08 23:15:26.000000 dishka-0.9.0/src/dishka/integrations/__init__.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2279 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/integrations/aiogram.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1232 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/integrations/aiohttp.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2445 2024-03-04 22:02:38.000000 dishka-0.9.0/src/dishka/integrations/arq.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5268 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/integrations/base.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1417 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/integrations/fastapi.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1734 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/integrations/faststream.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1421 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/integrations/flask.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1749 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/integrations/litestar.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1248 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/integrations/starlette.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1862 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/integrations/taskiq.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1379 2024-03-28 15:28:45.000000 dishka-0.9.0/src/dishka/integrations/telebot.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6369 2024-03-29 11:10:54.000000 dishka-0.9.0/src/dishka/provider.py
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-18 18:04:06.000000 dishka-0.9.0/src/dishka/py.typed
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    12796 2024-03-24 23:55:01.000000 dishka-0.9.0/src/dishka/registry.py
-drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-03-29 11:11:25.353492 dishka-0.9.0/src/dishka.egg-info/
--rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12015 2024-03-29 11:11:25.000000 dishka-0.9.0/src/dishka.egg-info/PKG-INFO
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1957 2024-03-29 11:11:25.000000 dishka-0.9.0/src/dishka.egg-info/SOURCES.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-03-29 11:11:25.000000 dishka-0.9.0/src/dishka.egg-info/dependency_links.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       50 2024-03-29 11:11:25.000000 dishka-0.9.0/src/dishka.egg-info/requires.txt
--rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        7 2024-03-29 11:11:25.000000 dishka-0.9.0/src/dishka.egg-info/top_level.txt
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.075320 dishka-1.0.0/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11357 2024-01-25 16:39:00.000000 dishka-1.0.0/LICENSE
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12015 2024-04-02 21:17:26.075320 dishka-1.0.0/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    11078 2024-04-01 21:05:02.000000 dishka-1.0.0/README.md
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1097 2024-04-02 21:17:01.000000 dishka-1.0.0/pyproject.toml
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       38 2024-04-02 21:17:26.075320 dishka-1.0.0/setup.cfg
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      807 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/__init__.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/_adaptix/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      635 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/common.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5323 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/feature_requirement.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/_adaptix/type_tools/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      540 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     4756 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/basic_utils.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1441 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/constants.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3877 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/generic_resolver.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1827 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/implicit_params.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1059 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/norm_utils.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    25734 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/_adaptix/type_tools/normalize_type.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6943 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/async_container.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6592 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/container.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      476 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/container_objects.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/dependency_source/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      510 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1038 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/alias.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1416 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/composite.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1515 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/context_var.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1324 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/decorator.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2164 2024-03-27 22:27:14.000000 dishka-1.0.0/src/dishka/dependency_source/factory.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      905 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/make_alias.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      678 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/make_context_var.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1462 2024-04-01 21:05:02.000000 dishka-1.0.0/src/dishka/dependency_source/make_decorator.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    15125 2024-04-02 21:16:55.000000 dishka-1.0.0/src/dishka/dependency_source/make_factory.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1949 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/dependency_source/unpack_provides.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/entities/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-29 00:39:11.000000 dishka-1.0.0/src/dishka/entities/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       40 2024-02-29 00:39:11.000000 dishka-1.0.0/src/dishka/entities/component.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1178 2024-04-02 21:16:55.000000 dishka-1.0.0/src/dishka/entities/depends_marker.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1123 2024-03-04 22:02:38.000000 dishka-1.0.0/src/dishka/entities/key.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      347 2024-03-19 22:45:31.000000 dishka-1.0.0/src/dishka/entities/provides_marker.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)      783 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/entities/scope.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2730 2024-03-26 23:39:41.000000 dishka-1.0.0/src/dishka/error_rendering.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1715 2024-03-04 22:02:38.000000 dishka-1.0.0/src/dishka/exceptions.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     3397 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/factory_compiler.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka/integrations/
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-08 23:15:26.000000 dishka-1.0.0/src/dishka/integrations/__init__.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2279 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/aiogram.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1232 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/aiohttp.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2445 2024-03-04 22:02:38.000000 dishka-1.0.0/src/dishka/integrations/arq.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     5268 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/base.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1417 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/fastapi.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1734 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/faststream.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1421 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/flask.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1749 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/litestar.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1248 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/integrations/starlette.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     2226 2024-04-02 21:16:55.000000 dishka-1.0.0/src/dishka/integrations/taskiq.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1379 2024-03-28 15:28:45.000000 dishka-1.0.0/src/dishka/integrations/telebot.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     6369 2024-04-01 21:05:02.000000 dishka-1.0.0/src/dishka/provider.py
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        0 2024-02-18 18:04:06.000000 dishka-1.0.0/src/dishka/py.typed
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)    12796 2024-03-24 23:55:01.000000 dishka-1.0.0/src/dishka/registry.py
+drwxrwxr-x   0 tishka17  (1000) tishka17  (1000)        0 2024-04-02 21:17:26.071320 dishka-1.0.0/src/dishka.egg-info/
+-rw-r--r--   0 tishka17  (1000) tishka17  (1000)    12015 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/PKG-INFO
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)     1957 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        1 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)       50 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/requires.txt
+-rw-rw-r--   0 tishka17  (1000) tishka17  (1000)        7 2024-04-02 21:17:26.000000 dishka-1.0.0/src/dishka.egg-info/top_level.txt
```

### Comparing `dishka-0.9.0/LICENSE` & `dishka-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/PKG-INFO` & `dishka-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dishka
-Version: 0.9.0
+Version: 1.0.0
 Summary: Minimal DI framework
 Author-email: Andrey Tikhonov <17@itishka.org>
 License: Apache-2.0
 Project-URL: Source, https://github.com/reagento/dishka
 Project-URL: Homepage, https://github.com/reagento/dishka
 Project-URL: Documentation, https://dishka.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/reagento/dishka/issues
```

### Comparing `dishka-0.9.0/README.md` & `dishka-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/pyproject.toml` & `dishka-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "dishka"
-version = "0.9.0"
+version = "1.0.0"
 readme = "README.md"
 authors = [
     { name = "Andrey Tikhonov", email = "17@itishka.org" },
 ]
 license = { text = "Apache-2.0" }
 description = "Minimal DI framework"
 requires-python = ">=3.10"
```

### Comparing `dishka-0.9.0/src/dishka/__init__.py` & `dishka-1.0.0/src/dishka/__init__.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/_adaptix/common.py` & `dishka-1.0.0/src/dishka/_adaptix/common.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/_adaptix/feature_requirement.py` & `dishka-1.0.0/src/dishka/_adaptix/feature_requirement.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/_adaptix/type_tools/__init__.py` & `dishka-1.0.0/src/dishka/_adaptix/type_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/_adaptix/type_tools/basic_utils.py` & `dishka-1.0.0/src/dishka/_adaptix/type_tools/basic_utils.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/_adaptix/type_tools/constants.py` & `dishka-1.0.0/src/dishka/_adaptix/type_tools/constants.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/_adaptix/type_tools/generic_resolver.py` & `dishka-1.0.0/src/dishka/_adaptix/type_tools/generic_resolver.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/_adaptix/type_tools/implicit_params.py` & `dishka-1.0.0/src/dishka/_adaptix/type_tools/implicit_params.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/_adaptix/type_tools/norm_utils.py` & `dishka-1.0.0/src/dishka/_adaptix/type_tools/norm_utils.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/_adaptix/type_tools/normalize_type.py` & `dishka-1.0.0/src/dishka/_adaptix/type_tools/normalize_type.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/async_container.py` & `dishka-1.0.0/src/dishka/async_container.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/container.py` & `dishka-1.0.0/src/dishka/container.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/dependency_source/alias.py` & `dishka-1.0.0/src/dishka/dependency_source/alias.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/dependency_source/composite.py` & `dishka-1.0.0/src/dishka/dependency_source/composite.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/dependency_source/context_var.py` & `dishka-1.0.0/src/dishka/dependency_source/context_var.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/dependency_source/decorator.py` & `dishka-1.0.0/src/dishka/dependency_source/decorator.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/dependency_source/factory.py` & `dishka-1.0.0/src/dishka/dependency_source/factory.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/dependency_source/make_alias.py` & `dishka-1.0.0/src/dishka/dependency_source/make_alias.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/dependency_source/make_context_var.py` & `dishka-1.0.0/src/dishka/dependency_source/make_context_var.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/dependency_source/make_decorator.py` & `dishka-1.0.0/src/dishka/dependency_source/make_decorator.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/dependency_source/make_factory.py` & `dishka-1.0.0/src/dishka/dependency_source/make_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     isgeneratorfunction,
     ismethod,
     signature,
     unwrap,
 )
 from typing import (
     Any,
+    Protocol,
     get_args,
     get_origin,
     get_type_hints,
     overload,
 )
 
 from dishka._adaptix.type_tools.basic_utils import (
@@ -39,14 +40,15 @@
 from dishka.entities.key import DependencyKey, hints_to_dependency_keys
 from dishka.entities.scope import BaseScope
 from .composite import CompositeDependencySource, ensure_composite
 from .factory import Factory, FactoryType
 from .unpack_provides import unpack_factory
 
 _empty = signature(lambda a: 0).parameters["a"].annotation
+_protocol_init = type("_stub_proto", (Protocol,), {}).__init__
 
 
 def _is_bound_method(obj):
     return ismethod(obj) and obj.__self__
 
 
 def _get_init_members(tp) -> MembersStorage[str, None]:
@@ -153,14 +155,16 @@
         return _generator_result(possible_dependency)
     return possible_dependency
 
 
 def _params_without_hints(func, *, skip_self: bool) -> Sequence[str]:
     if func is object.__init__:
         return []
+    if func is _protocol_init:
+        return []
     params = signature(func).parameters
     return [
         p.name
         for i, p in enumerate(params.values())
         if p.annotation is _empty
         if i > 0 or not skip_self
     ]
@@ -196,23 +200,22 @@
             f"Or, create a separate factory with all types imported.",
             name=e.name,
         ) from e
     hints.pop("return", _empty)
     dependencies = list(hints.values())
     if not provides:
         provides = source
-    is_to_bind = False
-    factory_type = FactoryType.FACTORY
+
     return Factory(
         dependencies=hints_to_dependency_keys(dependencies),
-        type_=factory_type,
+        type_=FactoryType.FACTORY,
         source=source,
         scope=scope,
         provides=DependencyKey(provides, None),
-        is_to_bind=is_to_bind,
+        is_to_bind=False,
         cache=cache,
     )
 
 
 def _make_factory_by_method(
         *,
         provides: Any,
```

### Comparing `dishka-0.9.0/src/dishka/dependency_source/unpack_provides.py` & `dishka-1.0.0/src/dishka/dependency_source/unpack_provides.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/entities/depends_marker.py` & `dishka-1.0.0/src/dishka/entities/depends_marker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import warnings
 from typing import TYPE_CHECKING, Annotated
 
 from .component import DEFAULT_COMPONENT, Component
 from .key import FromComponent
 
 if TYPE_CHECKING:
-    from typing import Union as FromDishka
+    from typing import TypeVar, Union
+    T = TypeVar("T")
+    FromDishka = Union[T, T]  # noqa: UP007,PYI016
 else:
     class FromDishka:
         def __init__(self, component: Component = None):
             if component is None:
                 self.component = DEFAULT_COMPONENT
                 warnings.warn(
                     "Annotated[Cls, FromDishka()] is deprecated "
```

### Comparing `dishka-0.9.0/src/dishka/entities/key.py` & `dishka-1.0.0/src/dishka/entities/key.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/entities/scope.py` & `dishka-1.0.0/src/dishka/entities/scope.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/error_rendering.py` & `dishka-1.0.0/src/dishka/error_rendering.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/exceptions.py` & `dishka-1.0.0/src/dishka/exceptions.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/factory_compiler.py` & `dishka-1.0.0/src/dishka/factory_compiler.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/aiogram.py` & `dishka-1.0.0/src/dishka/integrations/aiogram.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/aiohttp.py` & `dishka-1.0.0/src/dishka/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/arq.py` & `dishka-1.0.0/src/dishka/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/base.py` & `dishka-1.0.0/src/dishka/integrations/base.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/fastapi.py` & `dishka-1.0.0/src/dishka/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/faststream.py` & `dishka-1.0.0/src/dishka/integrations/faststream.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/flask.py` & `dishka-1.0.0/src/dishka/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/litestar.py` & `dishka-1.0.0/src/dishka/integrations/litestar.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/starlette.py` & `dishka-1.0.0/src/dishka/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/integrations/taskiq.py` & `dishka-1.0.0/src/dishka/integrations/taskiq.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,24 +28,35 @@
         super().__init__()
         self._container = container
 
     async def pre_execute(
         self,
         message: TaskiqMessage,
     ) -> TaskiqMessage:
-        container = await self._container().__aenter__()
-        message.labels[CONTAINER_NAME] = container
+        message.labels[CONTAINER_NAME] = await self._container().__aenter__()
         return message
 
+    async def on_error(
+        self,
+        message: TaskiqMessage,
+        result: TaskiqResult[Any],
+        exception: BaseException,
+    ) -> None:
+        if CONTAINER_NAME in result.labels:
+            await result.labels[CONTAINER_NAME].close()
+            del result.labels[CONTAINER_NAME]
+
     async def post_execute(
         self,
         message: TaskiqMessage,
         result: TaskiqResult[Any],
     ) -> None:
-        await message.labels[CONTAINER_NAME].close()
+        if CONTAINER_NAME in result.labels:
+            await result.labels[CONTAINER_NAME].close()
+            del result.labels[CONTAINER_NAME]
 
 
 def _get_container(
     context: Annotated[Context, TaskiqDepends()],
 ) -> Generator[AsyncGenerator, None, None]:
     yield context.message.labels[CONTAINER_NAME]
```

### Comparing `dishka-0.9.0/src/dishka/integrations/telebot.py` & `dishka-1.0.0/src/dishka/integrations/telebot.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/provider.py` & `dishka-1.0.0/src/dishka/provider.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka/registry.py` & `dishka-1.0.0/src/dishka/registry.py`

 * *Files identical despite different names*

### Comparing `dishka-0.9.0/src/dishka.egg-info/PKG-INFO` & `dishka-1.0.0/src/dishka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dishka
-Version: 0.9.0
+Version: 1.0.0
 Summary: Minimal DI framework
 Author-email: Andrey Tikhonov <17@itishka.org>
 License: Apache-2.0
 Project-URL: Source, https://github.com/reagento/dishka
 Project-URL: Homepage, https://github.com/reagento/dishka
 Project-URL: Documentation, https://dishka.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/reagento/dishka/issues
```

### Comparing `dishka-0.9.0/src/dishka.egg-info/SOURCES.txt` & `dishka-1.0.0/src/dishka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

